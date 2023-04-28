# Comparing `tmp/iniUts-1.0.3.tar.gz` & `tmp/iniUts-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iniUts-1.0.3.tar", last modified: Wed Apr 26 20:12:53 2023, max compression
+gzip compressed data, was "iniUts-1.0.4.tar", last modified: Fri Apr 28 14:48:46 2023, max compression
```

## Comparing `iniUts-1.0.3.tar` & `iniUts-1.0.4.tar`

### file list

```diff
@@ -1,833 +1,833 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:53.337242 iniUts-1.0.3/
--rw-rw-rw-   0        0        0      270 2023-04-26 20:12:27.000000 iniUts-1.0.3/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1058 2023-04-26 17:09:25.000000 iniUts-1.0.3/LICENCE.txt
--rw-rw-rw-   0        0        0       30 2023-04-26 17:09:25.000000 iniUts-1.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     3340 2023-04-26 20:12:53.336244 iniUts-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2536 2023-04-26 18:58:33.000000 iniUts-1.0.3/README.md
--rw-rw-rw-   0        0        0      122 2023-04-26 17:09:25.000000 iniUts-1.0.3/commands.txt
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:51.770413 iniUts-1.0.3/iniUts/
--rw-rw-rw-   0        0        0     2938 2023-04-26 20:12:44.000000 iniUts-1.0.3/iniUts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:51.795346 iniUts-1.0.3/iniUts.egg-info/
--rw-rw-rw-   0        0        0     3340 2023-04-26 20:12:51.000000 iniUts-1.0.3/iniUts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    42544 2023-04-26 20:12:51.000000 iniUts-1.0.3/iniUts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 20:12:51.000000 iniUts-1.0.3/iniUts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-26 20:12:51.000000 iniUts-1.0.3/iniUts.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-26 20:12:51.000000 iniUts-1.0.3/iniUts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-26 20:12:53.338238 iniUts-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      751 2023-04-26 20:12:33.000000 iniUts-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:51.688692 iniUts-1.0.3/venv/
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:51.688692 iniUts-1.0.3/venv/Lib/
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:51.744482 iniUts-1.0.3/venv/Lib/site-packages/
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:51.798339 iniUts-1.0.3/venv/Lib/site-packages/_distutils_hack/
--rw-rw-rw-   0        0        0     6128 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/_distutils_hack/__init__.py
--rw-rw-rw-   0        0        0       44 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/_distutils_hack/override.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:51.799335 iniUts-1.0.3/venv/Lib/site-packages/dateUts/
--rw-rw-rw-   0        0        0     4751 2023-04-26 17:23:17.000000 iniUts-1.0.3/venv/Lib/site-packages/dateUts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:51.802327 iniUts-1.0.3/venv/Lib/site-packages/dateUts-0.1.5.dist-info/
--rw-rw-rw-   0        0        0     1058 2023-04-26 17:23:17.000000 iniUts-1.0.3/venv/Lib/site-packages/dateUts-0.1.5.dist-info/LICENCE.txt
--rw-rw-rw-   0        0        0        8 2023-04-26 17:23:17.000000 iniUts-1.0.3/venv/Lib/site-packages/dateUts-0.1.5.dist-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:51.806317 iniUts-1.0.3/venv/Lib/site-packages/pip/
--rw-rw-rw-   0        0        0      357 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/__init__.py
--rw-rw-rw-   0        0        0     1198 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/__main__.py
--rw-rw-rw-   0        0        0     1444 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/__pip-runner__.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:51.825266 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/
--rw-rw-rw-   0        0        0      573 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/__init__.py
--rw-rw-rw-   0        0        0    10243 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/build_env.py
--rw-rw-rw-   0        0        0     9661 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/cache.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:51.847207 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/cli/
--rw-rw-rw-   0        0        0      132 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/cli/__init__.py
--rw-rw-rw-   0        0        0     6676 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/cli/autocompletion.py
--rw-rw-rw-   0        0        0     8176 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/cli/base_command.py
--rw-rw-rw-   0        0        0    30030 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/cli/cmdoptions.py
--rw-rw-rw-   0        0        0      774 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/cli/command_context.py
--rw-rw-rw-   0        0        0     2816 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/cli/main.py
--rw-rw-rw-   0        0        0     4338 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/cli/main_parser.py
--rw-rw-rw-   0        0        0    10817 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/cli/parser.py
--rw-rw-rw-   0        0        0     1968 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/cli/progress_bars.py
--rw-rw-rw-   0        0        0    18328 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/cli/req_command.py
--rw-rw-rw-   0        0        0     5118 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/cli/spinners.py
--rw-rw-rw-   0        0        0      116 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/cli/status_codes.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:51.871143 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/commands/
--rw-rw-rw-   0        0        0     3882 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/commands/__init__.py
--rw-rw-rw-   0        0        0     7581 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/commands/cache.py
--rw-rw-rw-   0        0        0     1684 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/commands/check.py
--rw-rw-rw-   0        0        0     4129 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/commands/completion.py
--rw-rw-rw-   0        0        0     9815 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/commands/configuration.py
--rw-rw-rw-   0        0        0     6591 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/commands/debug.py
--rw-rw-rw-   0        0        0     5182 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/commands/download.py
--rw-rw-rw-   0        0        0     2951 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/commands/freeze.py
--rw-rw-rw-   0        0        0     1703 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/commands/hash.py
--rw-rw-rw-   0        0        0     1132 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/commands/help.py
--rw-rw-rw-   0        0        0     4793 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/commands/index.py
--rw-rw-rw-   0        0        0     3188 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/commands/inspect.py
--rw-rw-rw-   0        0        0    28722 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/commands/install.py
--rw-rw-rw-   0        0        0    12343 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/commands/list.py
--rw-rw-rw-   0        0        0     5697 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/commands/search.py
--rw-rw-rw-   0        0        0     6419 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/commands/show.py
--rw-rw-rw-   0        0        0     3886 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/commands/uninstall.py
--rw-rw-rw-   0        0        0     6324 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/commands/wheel.py
--rw-rw-rw-   0        0        0    13529 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/configuration.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:51.879122 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/distributions/
--rw-rw-rw-   0        0        0      858 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/distributions/__init__.py
--rw-rw-rw-   0        0        0     1221 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/distributions/base.py
--rw-rw-rw-   0        0        0      729 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/distributions/installed.py
--rw-rw-rw-   0        0        0     6494 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/distributions/sdist.py
--rw-rw-rw-   0        0        0     1164 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/distributions/wheel.py
--rw-rw-rw-   0        0        0    23741 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:51.886103 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/index/
--rw-rw-rw-   0        0        0       30 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/index/__init__.py
--rw-rw-rw-   0        0        0    16504 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/index/collector.py
--rw-rw-rw-   0        0        0    37873 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/index/package_finder.py
--rw-rw-rw-   0        0        0     6556 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/index/sources.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:51.890092 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/locations/
--rw-rw-rw-   0        0        0    15365 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/locations/__init__.py
--rw-rw-rw-   0        0        0     6100 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/locations/_distutils.py
--rw-rw-rw-   0        0        0     7680 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/locations/_sysconfig.py
--rw-rw-rw-   0        0        0     2556 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/locations/base.py
--rw-rw-rw-   0        0        0      340 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/main.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:51.898071 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/metadata/
--rw-rw-rw-   0        0        0     4280 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/metadata/__init__.py
--rw-rw-rw-   0        0        0     2595 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/metadata/_json.py
--rw-rw-rw-   0        0        0    25277 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/metadata/base.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:51.903057 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/metadata/importlib/
--rw-rw-rw-   0        0        0      107 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/metadata/importlib/__init__.py
--rw-rw-rw-   0        0        0     1882 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/metadata/importlib/_compat.py
--rw-rw-rw-   0        0        0     8181 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/metadata/importlib/_dists.py
--rw-rw-rw-   0        0        0     7457 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/metadata/importlib/_envs.py
--rw-rw-rw-   0        0        0     9773 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/metadata/pkg_resources.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:51.923004 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/models/
--rw-rw-rw-   0        0        0       63 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/models/__init__.py
--rw-rw-rw-   0        0        0      990 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/models/candidate.py
--rw-rw-rw-   0        0        0     6931 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/models/direct_url.py
--rw-rw-rw-   0        0        0     2520 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/models/format_control.py
--rw-rw-rw-   0        0        0     1030 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/models/index.py
--rw-rw-rw-   0        0        0     2619 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/models/installation_report.py
--rw-rw-rw-   0        0        0    18817 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/models/link.py
--rw-rw-rw-   0        0        0      738 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/models/scheme.py
--rw-rw-rw-   0        0        0     4643 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/models/search_scope.py
--rw-rw-rw-   0        0        0     1907 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/models/selection_prefs.py
--rw-rw-rw-   0        0        0     3858 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/models/target_python.py
--rw-rw-rw-   0        0        0     3600 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/models/wheel.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:51.939959 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/network/
--rw-rw-rw-   0        0        0       50 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/network/__init__.py
--rw-rw-rw-   0        0        0    20435 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/network/auth.py
--rw-rw-rw-   0        0        0     2145 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/network/cache.py
--rw-rw-rw-   0        0        0     6096 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/network/download.py
--rw-rw-rw-   0        0        0     7638 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/network/lazy_wheel.py
--rw-rw-rw-   0        0        0    18442 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/network/session.py
--rw-rw-rw-   0        0        0     4073 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/network/utils.py
--rw-rw-rw-   0        0        0     1791 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/network/xmlrpc.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:51.947937 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/operations/
--rw-rw-rw-   0        0        0        0 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/operations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:51.958909 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/operations/build/
--rw-rw-rw-   0        0        0        0 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/operations/build/__init__.py
--rw-rw-rw-   0        0        0     4133 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/operations/build/build_tracker.py
--rw-rw-rw-   0        0        0     1422 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/operations/build/metadata.py
--rw-rw-rw-   0        0        0     1474 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/operations/build/metadata_editable.py
--rw-rw-rw-   0        0        0     2198 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/operations/build/metadata_legacy.py
--rw-rw-rw-   0        0        0     1075 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/operations/build/wheel.py
--rw-rw-rw-   0        0        0     1417 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/operations/build/wheel_editable.py
--rw-rw-rw-   0        0        0     3064 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/operations/build/wheel_legacy.py
--rw-rw-rw-   0        0        0     5122 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/operations/check.py
--rw-rw-rw-   0        0        0     9816 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/operations/freeze.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:51.961900 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/operations/install/
--rw-rw-rw-   0        0        0       51 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/operations/install/__init__.py
--rw-rw-rw-   0        0        0     1282 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/operations/install/editable_legacy.py
--rw-rw-rw-   0        0        0    27475 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/operations/install/wheel.py
--rw-rw-rw-   0        0        0    27696 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/operations/prepare.py
--rw-rw-rw-   0        0        0     7161 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/pyproject.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:51.968882 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/req/
--rw-rw-rw-   0        0        0     2738 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/req/__init__.py
--rw-rw-rw-   0        0        0    16610 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/req/constructors.py
--rw-rw-rw-   0        0        0    17872 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/req/req_file.py
--rw-rw-rw-   0        0        0    32782 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/req/req_install.py
--rw-rw-rw-   0        0        0     2858 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/req/req_set.py
--rw-rw-rw-   0        0        0    24678 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/req/req_uninstall.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:51.970876 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/resolution/
--rw-rw-rw-   0        0        0        0 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/resolution/__init__.py
--rw-rw-rw-   0        0        0      583 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/resolution/base.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:51.973868 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/resolution/legacy/
--rw-rw-rw-   0        0        0        0 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/resolution/legacy/__init__.py
--rw-rw-rw-   0        0        0    24128 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/resolution/legacy/resolver.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:51.986834 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/
--rw-rw-rw-   0        0        0        0 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/__init__.py
--rw-rw-rw-   0        0        0     5220 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/base.py
--rw-rw-rw-   0        0        0    18864 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/candidates.py
--rw-rw-rw-   0        0        0    27845 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/factory.py
--rw-rw-rw-   0        0        0     5705 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
--rw-rw-rw-   0        0        0     9824 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/provider.py
--rw-rw-rw-   0        0        0     3094 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/reporter.py
--rw-rw-rw-   0        0        0     5454 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/requirements.py
--rw-rw-rw-   0        0        0    11538 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/resolver.py
--rw-rw-rw-   0        0        0     8167 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/self_outdated_check.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:52.052657 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/utils/
--rw-rw-rw-   0        0        0        0 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/utils/__init__.py
--rw-rw-rw-   0        0        0     3351 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/utils/_jaraco_text.py
--rw-rw-rw-   0        0        0     1015 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/utils/_log.py
--rw-rw-rw-   0        0        0     1665 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/utils/appdirs.py
--rw-rw-rw-   0        0        0     1884 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/utils/compat.py
--rw-rw-rw-   0        0        0     5377 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/utils/compatibility_tags.py
--rw-rw-rw-   0        0        0      242 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/utils/datetime.py
--rw-rw-rw-   0        0        0     3627 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/utils/deprecation.py
--rw-rw-rw-   0        0        0     3206 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/utils/direct_url_helpers.py
--rw-rw-rw-   0        0        0     2118 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/utils/egg_link.py
--rw-rw-rw-   0        0        0     1169 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/utils/encoding.py
--rw-rw-rw-   0        0        0     3064 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/utils/entrypoints.py
--rw-rw-rw-   0        0        0     5122 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/utils/filesystem.py
--rw-rw-rw-   0        0        0      716 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/utils/filetypes.py
--rw-rw-rw-   0        0        0     3110 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/utils/glibc.py
--rw-rw-rw-   0        0        0     5118 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/utils/hashes.py
--rw-rw-rw-   0        0        0      795 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/utils/inject_securetransport.py
--rw-rw-rw-   0        0        0    11632 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/utils/logging.py
--rw-rw-rw-   0        0        0    22216 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/utils/misc.py
--rw-rw-rw-   0        0        0     1193 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/utils/models.py
--rw-rw-rw-   0        0        0     2108 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/utils/packaging.py
--rw-rw-rw-   0        0        0     4435 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/utils/setuptools_build.py
--rw-rw-rw-   0        0        0     9200 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/utils/subprocess.py
--rw-rw-rw-   0        0        0     7702 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/utils/temp_dir.py
--rw-rw-rw-   0        0        0     8821 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/utils/unpacking.py
--rw-rw-rw-   0        0        0     1759 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/utils/urls.py
--rw-rw-rw-   0        0        0     3456 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/utils/virtualenv.py
--rw-rw-rw-   0        0        0     4549 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/utils/wheel.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:52.060636 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/vcs/
--rw-rw-rw-   0        0        0      596 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/vcs/__init__.py
--rw-rw-rw-   0        0        0     3519 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/vcs/bazaar.py
--rw-rw-rw-   0        0        0    18116 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/vcs/git.py
--rw-rw-rw-   0        0        0     5238 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/vcs/mercurial.py
--rw-rw-rw-   0        0        0    11729 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/vcs/subversion.py
--rw-rw-rw-   0        0        0    22811 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/vcs/versioncontrol.py
--rw-rw-rw-   0        0        0    11842 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/wheel_builder.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:52.066619 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/
--rw-rw-rw-   0        0        0     4966 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:52.082577 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/cachecontrol/
--rw-rw-rw-   0        0        0      465 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/cachecontrol/__init__.py
--rw-rw-rw-   0        0        0     1379 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/cachecontrol/_cmd.py
--rw-rw-rw-   0        0        0     5033 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/cachecontrol/adapter.py
--rw-rw-rw-   0        0        0     1535 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/cachecontrol/cache.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:52.086566 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/
--rw-rw-rw-   0        0        0      242 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
--rw-rw-rw-   0        0        0     5271 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
--rw-rw-rw-   0        0        0     1033 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
--rw-rw-rw-   0        0        0      778 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/cachecontrol/compat.py
--rw-rw-rw-   0        0        0    16416 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/cachecontrol/controller.py
--rw-rw-rw-   0        0        0     3946 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/cachecontrol/filewrapper.py
--rw-rw-rw-   0        0        0     4154 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/cachecontrol/heuristics.py
--rw-rw-rw-   0        0        0     7105 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/cachecontrol/serialize.py
--rw-rw-rw-   0        0        0      774 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/cachecontrol/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:52.089558 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/certifi/
--rw-rw-rw-   0        0        0       94 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/certifi/__init__.py
--rw-rw-rw-   0        0        0      255 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/certifi/__main__.py
--rw-rw-rw-   0        0        0     4279 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/certifi/core.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:52.161367 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/
--rw-rw-rw-   0        0        0     4797 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/__init__.py
--rw-rw-rw-   0        0        0    31274 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/big5freq.py
--rw-rw-rw-   0        0        0     1763 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/big5prober.py
--rw-rw-rw-   0        0        0    10032 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/chardistribution.py
--rw-rw-rw-   0        0        0     3915 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/charsetgroupprober.py
--rw-rw-rw-   0        0        0     5420 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/charsetprober.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:52.163361 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/cli/
--rw-rw-rw-   0        0        0        0 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/cli/__init__.py
--rw-rw-rw-   0        0        0     3242 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/cli/chardetect.py
--rw-rw-rw-   0        0        0     3732 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachine.py
--rw-rw-rw-   0        0        0      542 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachinedict.py
--rw-rw-rw-   0        0        0     1860 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/cp949prober.py
--rw-rw-rw-   0        0        0     1683 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/enums.py
--rw-rw-rw-   0        0        0     4006 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/escprober.py
--rw-rw-rw-   0        0        0    12176 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/escsm.py
--rw-rw-rw-   0        0        0     3934 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/eucjpprober.py
--rw-rw-rw-   0        0        0    13566 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/euckrfreq.py
--rw-rw-rw-   0        0        0     1753 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/euckrprober.py
--rw-rw-rw-   0        0        0    36913 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/euctwfreq.py
--rw-rw-rw-   0        0        0     1753 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/euctwprober.py
--rw-rw-rw-   0        0        0    20735 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/gb2312freq.py
--rw-rw-rw-   0        0        0     1759 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/gb2312prober.py
--rw-rw-rw-   0        0        0    14537 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/hebrewprober.py
--rw-rw-rw-   0        0        0    25796 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/jisfreq.py
--rw-rw-rw-   0        0        0    42498 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/johabfreq.py
--rw-rw-rw-   0        0        0     1752 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/johabprober.py
--rw-rw-rw-   0        0        0    27055 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/jpcntx.py
--rw-rw-rw-   0        0        0   104562 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
--rw-rw-rw-   0        0        0    98484 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/langgreekmodel.py
--rw-rw-rw-   0        0        0    98196 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/langhebrewmodel.py
--rw-rw-rw-   0        0        0   101363 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/langhungarianmodel.py
--rw-rw-rw-   0        0        0   128035 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/langrussianmodel.py
--rw-rw-rw-   0        0        0   102774 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/langthaimodel.py
--rw-rw-rw-   0        0        0    95372 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/langturkishmodel.py
--rw-rw-rw-   0        0        0     5380 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/latin1prober.py
--rw-rw-rw-   0        0        0     6077 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/macromanprober.py
--rw-rw-rw-   0        0        0     3715 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/mbcharsetprober.py
--rw-rw-rw-   0        0        0     2131 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
--rw-rw-rw-   0        0        0    30391 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/mbcssm.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:52.165356 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/metadata/
--rw-rw-rw-   0        0        0        0 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/metadata/__init__.py
--rw-rw-rw-   0        0        0    13560 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/metadata/languages.py
--rw-rw-rw-   0        0        0      402 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/resultdict.py
--rw-rw-rw-   0        0        0     6400 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/sbcharsetprober.py
--rw-rw-rw-   0        0        0     4137 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
--rw-rw-rw-   0        0        0     4007 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/sjisprober.py
--rw-rw-rw-   0        0        0    14848 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/universaldetector.py
--rw-rw-rw-   0        0        0     8505 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/utf1632prober.py
--rw-rw-rw-   0        0        0     2812 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/utf8prober.py
--rw-rw-rw-   0        0        0      244 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/version.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:52.172337 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/colorama/
--rw-rw-rw-   0        0        0      266 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/colorama/__init__.py
--rw-rw-rw-   0        0        0     2522 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/colorama/ansi.py
--rw-rw-rw-   0        0        0    11128 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/colorama/ansitowin32.py
--rw-rw-rw-   0        0        0     3325 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/colorama/initialise.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:52.183308 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/colorama/tests/
--rw-rw-rw-   0        0        0       75 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/colorama/tests/__init__.py
--rw-rw-rw-   0        0        0     2839 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/colorama/tests/ansi_test.py
--rw-rw-rw-   0        0        0    10678 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py
--rw-rw-rw-   0        0        0     6741 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/colorama/tests/initialise_test.py
--rw-rw-rw-   0        0        0     1866 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/colorama/tests/isatty_test.py
--rw-rw-rw-   0        0        0     1079 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/colorama/tests/utils.py
--rw-rw-rw-   0        0        0     3709 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/colorama/tests/winterm_test.py
--rw-rw-rw-   0        0        0     6181 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/colorama/win32.py
--rw-rw-rw-   0        0        0     7134 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/colorama/winterm.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:52.202257 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/distlib/
--rw-rw-rw-   0        0        0      581 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/distlib/__init__.py
--rw-rw-rw-   0        0        0    41259 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/distlib/compat.py
--rw-rw-rw-   0        0        0    51697 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/distlib/database.py
--rw-rw-rw-   0        0        0    20834 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/distlib/index.py
--rw-rw-rw-   0        0        0    51991 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/distlib/locators.py
--rw-rw-rw-   0        0        0    14811 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/distlib/manifest.py
--rw-rw-rw-   0        0        0     5058 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/distlib/markers.py
--rw-rw-rw-   0        0        0    39801 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/distlib/metadata.py
--rw-rw-rw-   0        0        0    10820 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/distlib/resources.py
--rw-rw-rw-   0        0        0    18102 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/distlib/scripts.py
--rw-rw-rw-   0        0        0    66262 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/distlib/util.py
--rw-rw-rw-   0        0        0    23513 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/distlib/version.py
--rw-rw-rw-   0        0        0    43898 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/distlib/wheel.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:52.207244 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/distro/
--rw-rw-rw-   0        0        0      981 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/distro/__init__.py
--rw-rw-rw-   0        0        0       64 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/distro/__main__.py
--rw-rw-rw-   0        0        0    49330 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/distro/distro.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:52.219212 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/idna/
--rw-rw-rw-   0        0        0      849 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/idna/__init__.py
--rw-rw-rw-   0        0        0     3374 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/idna/codec.py
--rw-rw-rw-   0        0        0      321 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/idna/compat.py
--rw-rw-rw-   0        0        0    12950 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/idna/core.py
--rw-rw-rw-   0        0        0    44375 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/idna/idnadata.py
--rw-rw-rw-   0        0        0     1881 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/idna/intranges.py
--rw-rw-rw-   0        0        0       21 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/idna/package_data.py
--rw-rw-rw-   0        0        0   206539 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/idna/uts46data.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:52.226193 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/msgpack/
--rw-rw-rw-   0        0        0     1132 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/msgpack/__init__.py
--rw-rw-rw-   0        0        0     1081 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/msgpack/exceptions.py
--rw-rw-rw-   0        0        0     6079 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/msgpack/ext.py
--rw-rw-rw-   0        0        0    34544 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/msgpack/fallback.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:52.242151 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/packaging/
--rw-rw-rw-   0        0        0      661 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/packaging/__about__.py
--rw-rw-rw-   0        0        0      497 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/packaging/__init__.py
--rw-rw-rw-   0        0        0    11488 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/packaging/_manylinux.py
--rw-rw-rw-   0        0        0     4378 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/packaging/_musllinux.py
--rw-rw-rw-   0        0        0     1431 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/packaging/_structures.py
--rw-rw-rw-   0        0        0     8487 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/packaging/markers.py
--rw-rw-rw-   0        0        0     4676 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/packaging/requirements.py
--rw-rw-rw-   0        0        0    30110 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/packaging/specifiers.py
--rw-rw-rw-   0        0        0    15699 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/packaging/tags.py
--rw-rw-rw-   0        0        0     4200 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/packaging/utils.py
--rw-rw-rw-   0        0        0    14665 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/packaging/version.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:52.244145 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pkg_resources/
--rw-rw-rw-   0        0        0   109388 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pkg_resources/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:52.256113 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/platformdirs/
--rw-rw-rw-   0        0        0    18003 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/platformdirs/__init__.py
--rw-rw-rw-   0        0        0     1198 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/platformdirs/__main__.py
--rw-rw-rw-   0        0        0     4303 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/platformdirs/android.py
--rw-rw-rw-   0        0        0     5706 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/platformdirs/api.py
--rw-rw-rw-   0        0        0     2800 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/platformdirs/macos.py
--rw-rw-rw-   0        0        0     7448 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/platformdirs/unix.py
--rw-rw-rw-   0        0        0      160 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/platformdirs/version.py
--rw-rw-rw-   0        0        0     7098 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/platformdirs/windows.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:52.282043 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/
--rw-rw-rw-   0        0        0     2999 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/__init__.py
--rw-rw-rw-   0        0        0      353 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/__main__.py
--rw-rw-rw-   0        0        0    23685 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/cmdline.py
--rw-rw-rw-   0        0        0     1697 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/console.py
--rw-rw-rw-   0        0        0     1938 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/filter.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:52.284038 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/filters/
--rw-rw-rw-   0        0        0    40386 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/filters/__init__.py
--rw-rw-rw-   0        0        0     2917 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/formatter.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:52.318945 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/formatters/
--rw-rw-rw-   0        0        0     4800 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/formatters/__init__.py
--rw-rw-rw-   0        0        0     4104 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/formatters/_mapping.py
--rw-rw-rw-   0        0        0     3314 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/formatters/bbcode.py
--rw-rw-rw-   0        0        0     5086 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/formatters/groff.py
--rw-rw-rw-   0        0        0    35601 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/formatters/html.py
--rw-rw-rw-   0        0        0    21938 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/formatters/img.py
--rw-rw-rw-   0        0        0     4981 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/formatters/irc.py
--rw-rw-rw-   0        0        0    19351 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/formatters/latex.py
--rw-rw-rw-   0        0        0     5073 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/formatters/other.py
--rw-rw-rw-   0        0        0     2212 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
--rw-rw-rw-   0        0        0     5014 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/formatters/rtf.py
--rw-rw-rw-   0        0        0     7335 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/formatters/svg.py
--rw-rw-rw-   0        0        0     4674 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal.py
--rw-rw-rw-   0        0        0    11753 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal256.py
--rw-rw-rw-   0        0        0    32064 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/lexer.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:52.327921 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/lexers/
--rw-rw-rw-   0        0        0    11164 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/lexers/__init__.py
--rw-rw-rw-   0        0        0    71556 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/lexers/_mapping.py
--rw-rw-rw-   0        0        0    53572 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/lexers/python.py
--rw-rw-rw-   0        0        0      986 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/modeline.py
--rw-rw-rw-   0        0        0     2591 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/plugin.py
--rw-rw-rw-   0        0        0     3072 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/regexopt.py
--rw-rw-rw-   0        0        0     3092 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/scanner.py
--rw-rw-rw-   0        0        0     6882 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/sphinxext.py
--rw-rw-rw-   0        0        0     6257 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/style.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:52.329916 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/styles/
--rw-rw-rw-   0        0        0     3419 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/styles/__init__.py
--rw-rw-rw-   0        0        0     6184 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/token.py
--rw-rw-rw-   0        0        0    63187 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/unistring.py
--rw-rw-rw-   0        0        0     9110 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/util.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:52.354849 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pyparsing/
--rw-rw-rw-   0        0        0     9171 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pyparsing/__init__.py
--rw-rw-rw-   0        0        0     6426 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pyparsing/actions.py
--rw-rw-rw-   0        0        0    12936 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pyparsing/common.py
--rw-rw-rw-   0        0        0   213344 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pyparsing/core.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:52.356844 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pyparsing/diagram/
--rw-rw-rw-   0        0        0    23685 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
--rw-rw-rw-   0        0        0     9023 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pyparsing/exceptions.py
--rw-rw-rw-   0        0        0    39129 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pyparsing/helpers.py
--rw-rw-rw-   0        0        0    25341 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pyparsing/results.py
--rw-rw-rw-   0        0        0    13402 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pyparsing/testing.py
--rw-rw-rw-   0        0        0    10787 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pyparsing/unicode.py
--rw-rw-rw-   0        0        0     6805 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pyparsing/util.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:52.364822 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/
--rw-rw-rw-   0        0        0      491 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/__init__.py
--rw-rw-rw-   0        0        0      138 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_compat.py
--rw-rw-rw-   0        0        0    11920 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_impl.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:52.385766 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/
--rw-rw-rw-   0        0        0      546 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py
--rw-rw-rw-   0        0        0    10927 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:52.419675 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/requests/
--rw-rw-rw-   0        0        0     5178 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/requests/__init__.py
--rw-rw-rw-   0        0        0      435 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/requests/__version__.py
--rw-rw-rw-   0        0        0     1397 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/requests/_internal_utils.py
--rw-rw-rw-   0        0        0    21443 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/requests/adapters.py
--rw-rw-rw-   0        0        0     6377 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/requests/api.py
--rw-rw-rw-   0        0        0    10187 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/requests/auth.py
--rw-rw-rw-   0        0        0      575 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/requests/certs.py
--rw-rw-rw-   0        0        0     1286 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/requests/compat.py
--rw-rw-rw-   0        0        0    18560 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/requests/cookies.py
--rw-rw-rw-   0        0        0     3823 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/requests/exceptions.py
--rw-rw-rw-   0        0        0     3879 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/requests/help.py
--rw-rw-rw-   0        0        0      733 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/requests/hooks.py
--rw-rw-rw-   0        0        0    35288 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/requests/models.py
--rw-rw-rw-   0        0        0      695 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/requests/packages.py
--rw-rw-rw-   0        0        0    30180 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/requests/sessions.py
--rw-rw-rw-   0        0        0     4235 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/requests/status_codes.py
--rw-rw-rw-   0        0        0     2912 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/requests/structures.py
--rw-rw-rw-   0        0        0    33240 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/requests/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:52.432641 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/resolvelib/
--rw-rw-rw-   0        0        0      537 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/resolvelib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:52.436630 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/resolvelib/compat/
--rw-rw-rw-   0        0        0        0 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/resolvelib/compat/__init__.py
--rw-rw-rw-   0        0        0      156 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
--rw-rw-rw-   0        0        0     5871 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/resolvelib/providers.py
--rw-rw-rw-   0        0        0     1601 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/resolvelib/reporters.py
--rw-rw-rw-   0        0        0    20511 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/resolvelib/resolvers.py
--rw-rw-rw-   0        0        0     4963 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/resolvelib/structs.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:52.600192 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/
--rw-rw-rw-   0        0        0     6090 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/__init__.py
--rw-rw-rw-   0        0        0     8478 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/__main__.py
--rw-rw-rw-   0        0        0    10096 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/_cell_widths.py
--rw-rw-rw-   0        0        0   140235 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/_emoji_codes.py
--rw-rw-rw-   0        0        0     1064 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/_emoji_replace.py
--rw-rw-rw-   0        0        0     2100 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/_export_format.py
--rw-rw-rw-   0        0        0      265 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/_extension.py
--rw-rw-rw-   0        0        0      799 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/_fileno.py
--rw-rw-rw-   0        0        0     9695 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/_inspect.py
--rw-rw-rw-   0        0        0     3225 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/_log_render.py
--rw-rw-rw-   0        0        0     1236 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/_loop.py
--rw-rw-rw-   0        0        0     1387 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/_null_file.py
--rw-rw-rw-   0        0        0     7063 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/_palettes.py
--rw-rw-rw-   0        0        0      423 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/_pick.py
--rw-rw-rw-   0        0        0     5472 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/_ratio.py
--rw-rw-rw-   0        0        0    19919 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/_spinners.py
--rw-rw-rw-   0        0        0      351 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/_stack.py
--rw-rw-rw-   0        0        0      417 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/_timer.py
--rw-rw-rw-   0        0        0    22820 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/_win32_console.py
--rw-rw-rw-   0        0        0     1926 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/_windows.py
--rw-rw-rw-   0        0        0     2783 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/_windows_renderer.py
--rw-rw-rw-   0        0        0     1840 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/_wrap.py
--rw-rw-rw-   0        0        0      890 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/abc.py
--rw-rw-rw-   0        0        0    10368 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/align.py
--rw-rw-rw-   0        0        0     6906 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/ansi.py
--rw-rw-rw-   0        0        0     3264 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/bar.py
--rw-rw-rw-   0        0        0     9842 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/box.py
--rw-rw-rw-   0        0        0     4509 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/cells.py
--rw-rw-rw-   0        0        0    18224 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/color.py
--rw-rw-rw-   0        0        0     1054 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/color_triplet.py
--rw-rw-rw-   0        0        0     7131 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/columns.py
--rw-rw-rw-   0        0        0    99195 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/console.py
--rw-rw-rw-   0        0        0     1288 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/constrain.py
--rw-rw-rw-   0        0        0     5497 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/containers.py
--rw-rw-rw-   0        0        0     6630 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/control.py
--rw-rw-rw-   0        0        0     8082 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/default_styles.py
--rw-rw-rw-   0        0        0      972 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/diagnose.py
--rw-rw-rw-   0        0        0     2501 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/emoji.py
--rw-rw-rw-   0        0        0      642 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/errors.py
--rw-rw-rw-   0        0        0     1683 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/file_proxy.py
--rw-rw-rw-   0        0        0     2508 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/filesize.py
--rw-rw-rw-   0        0        0     9584 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/highlighter.py
--rw-rw-rw-   0        0        0     5032 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/json.py
--rw-rw-rw-   0        0        0     3252 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/jupyter.py
--rw-rw-rw-   0        0        0    14007 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/layout.py
--rw-rw-rw-   0        0        0    14273 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/live.py
--rw-rw-rw-   0        0        0     3667 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/live_render.py
--rw-rw-rw-   0        0        0    11903 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/logging.py
--rw-rw-rw-   0        0        0     8198 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/markup.py
--rw-rw-rw-   0        0        0     5305 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/measure.py
--rw-rw-rw-   0        0        0     4970 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/padding.py
--rw-rw-rw-   0        0        0      828 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/pager.py
--rw-rw-rw-   0        0        0     3396 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/palette.py
--rw-rw-rw-   0        0        0    10574 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/panel.py
--rw-rw-rw-   0        0        0    35852 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/pretty.py
--rw-rw-rw-   0        0        0    59706 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/progress.py
--rw-rw-rw-   0        0        0     8165 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/progress_bar.py
--rw-rw-rw-   0        0        0    11303 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/prompt.py
--rw-rw-rw-   0        0        0     1391 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/protocol.py
--rw-rw-rw-   0        0        0      166 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/region.py
--rw-rw-rw-   0        0        0     4431 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/repr.py
--rw-rw-rw-   0        0        0     4602 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/rule.py
--rw-rw-rw-   0        0        0     2843 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/scope.py
--rw-rw-rw-   0        0        0     1591 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/screen.py
--rw-rw-rw-   0        0        0    24247 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/segment.py
--rw-rw-rw-   0        0        0     4339 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/spinner.py
--rw-rw-rw-   0        0        0     4425 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/status.py
--rw-rw-rw-   0        0        0    27073 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/style.py
--rw-rw-rw-   0        0        0     1258 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/styled.py
--rw-rw-rw-   0        0        0    35153 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/syntax.py
--rw-rw-rw-   0        0        0    39684 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/table.py
--rw-rw-rw-   0        0        0     3370 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/terminal_theme.py
--rw-rw-rw-   0        0        0    45525 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/text.py
--rw-rw-rw-   0        0        0     3777 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/theme.py
--rw-rw-rw-   0        0        0      102 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/themes.py
--rw-rw-rw-   0        0        0    29604 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/traceback.py
--rw-rw-rw-   0        0        0     9169 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/tree.py
--rw-rw-rw-   0        0        0    34549 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/six.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:52.622133 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/tenacity/
--rw-rw-rw-   0        0        0    20493 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/tenacity/__init__.py
--rw-rw-rw-   0        0        0     3551 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/tenacity/_asyncio.py
--rw-rw-rw-   0        0        0     2179 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/tenacity/_utils.py
--rw-rw-rw-   0        0        0     1682 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/tenacity/after.py
--rw-rw-rw-   0        0        0     1562 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/tenacity/before.py
--rw-rw-rw-   0        0        0     2372 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/tenacity/before_sleep.py
--rw-rw-rw-   0        0        0     1383 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/tenacity/nap.py
--rw-rw-rw-   0        0        0     8746 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/tenacity/retry.py
--rw-rw-rw-   0        0        0     3086 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/tenacity/stop.py
--rw-rw-rw-   0        0        0     2142 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/tenacity/tornadoweb.py
--rw-rw-rw-   0        0        0     8024 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/tenacity/wait.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:52.638090 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/tomli/
--rw-rw-rw-   0        0        0      396 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/tomli/__init__.py
--rw-rw-rw-   0        0        0    22633 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/tomli/_parser.py
--rw-rw-rw-   0        0        0     2943 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/tomli/_re.py
--rw-rw-rw-   0        0        0      254 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/tomli/_types.py
--rw-rw-rw-   0        0        0    84101 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/typing_extensions.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:52.660032 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/
--rw-rw-rw-   0        0        0     3333 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/__init__.py
--rw-rw-rw-   0        0        0    10811 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/_collections.py
--rw-rw-rw-   0        0        0       64 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/_version.py
--rw-rw-rw-   0        0        0    20300 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/connection.py
--rw-rw-rw-   0        0        0    39128 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/connectionpool.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:52.670006 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/
--rw-rw-rw-   0        0        0        0 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/__init__.py
--rw-rw-rw-   0        0        0      957 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:52.677984 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/
--rw-rw-rw-   0        0        0        0 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
--rw-rw-rw-   0        0        0    17632 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
--rw-rw-rw-   0        0        0    13922 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
--rw-rw-rw-   0        0        0    11036 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/appengine.py
--rw-rw-rw-   0        0        0     4528 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
--rw-rw-rw-   0        0        0    17081 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
--rw-rw-rw-   0        0        0    34448 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
--rw-rw-rw-   0        0        0     7097 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/socks.py
--rw-rw-rw-   0        0        0     8217 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/exceptions.py
--rw-rw-rw-   0        0        0     8579 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/fields.py
--rw-rw-rw-   0        0        0     2440 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/filepost.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:52.679979 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/packages/
--rw-rw-rw-   0        0        0        0 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/packages/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:52.682971 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/
--rw-rw-rw-   0        0        0        0 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
--rw-rw-rw-   0        0        0     1417 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
--rw-rw-rw-   0        0        0    34665 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/packages/six.py
--rw-rw-rw-   0        0        0    19786 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/poolmanager.py
--rw-rw-rw-   0        0        0     5985 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/request.py
--rw-rw-rw-   0        0        0    30641 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/response.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:52.708902 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/util/
--rw-rw-rw-   0        0        0     1155 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/util/__init__.py
--rw-rw-rw-   0        0        0     4901 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/util/connection.py
--rw-rw-rw-   0        0        0     1605 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/util/proxy.py
--rw-rw-rw-   0        0        0      498 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/util/queue.py
--rw-rw-rw-   0        0        0     3997 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/util/request.py
--rw-rw-rw-   0        0        0     3510 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/util/response.py
--rw-rw-rw-   0        0        0    22003 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/util/retry.py
--rw-rw-rw-   0        0        0    17177 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_.py
--rw-rw-rw-   0        0        0     5758 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
--rw-rw-rw-   0        0        0     6895 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssltransport.py
--rw-rw-rw-   0        0        0    10168 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/util/timeout.py
--rw-rw-rw-   0        0        0    14296 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/util/url.py
--rw-rw-rw-   0        0        0     5403 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/util/wait.py
--rw-rw-rw-   0        0        0      476 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/vendor.txt
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:52.715883 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/webencodings/
--rw-rw-rw-   0        0        0    10579 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/webencodings/__init__.py
--rw-rw-rw-   0        0        0     8979 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/webencodings/labels.py
--rw-rw-rw-   0        0        0     1305 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/webencodings/mklabels.py
--rw-rw-rw-   0        0        0     6563 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/webencodings/tests.py
--rw-rw-rw-   0        0        0     4307 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/webencodings/x_user_defined.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:51.813298 iniUts-1.0.3/venv/Lib/site-packages/pip-23.1.2.dist-info/
--rw-rw-rw-   0        0        0     9953 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip-23.1.2.dist-info/AUTHORS.txt
--rw-rw-rw-   0        0        0     1093 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip-23.1.2.dist-info/LICENSE.txt
--rw-rw-rw-   0        0        0      125 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip-23.1.2.dist-info/entry_points.txt
--rw-rw-rw-   0        0        0        4 2023-04-26 17:15:05.000000 iniUts-1.0.3/venv/Lib/site-packages/pip-23.1.2.dist-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:52.716880 iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/
--rw-rw-rw-   0        0        0   108568 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:52.720870 iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/
--rw-rw-rw-   0        0        0        0 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/__init__.py
--rw-rw-rw-   0        0        0    24701 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/appdirs.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:52.732837 iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/
--rw-rw-rw-   0        0        0      506 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/__init__.py
--rw-rw-rw-   0        0        0     4504 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py
--rw-rw-rw-   0        0        0     2741 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_common.py
--rw-rw-rw-   0        0        0     2706 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py
--rw-rw-rw-   0        0        0      884 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py
--rw-rw-rw-   0        0        0     3494 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py
--rw-rw-rw-   0        0        0     3886 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/abc.py
--rw-rw-rw-   0        0        0     3566 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/readers.py
--rw-rw-rw-   0        0        0     2836 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/simple.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:52.739818 iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/
--rw-rw-rw-   0        0        0        0 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/__init__.py
--rw-rw-rw-   0        0        0     5420 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/context.py
--rw-rw-rw-   0        0        0    13515 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/functools.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:52.743808 iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/text/
--rw-rw-rw-   0        0        0    15526 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:52.748795 iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/
--rw-rw-rw-   0        0        0       83 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/__init__.py
--rw-rw-rw-   0        0        0   132569 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/more.py
--rw-rw-rw-   0        0        0    18410 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/recipes.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:52.822597 iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/packaging/
--rw-rw-rw-   0        0        0      661 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/packaging/__about__.py
--rw-rw-rw-   0        0        0      497 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/packaging/__init__.py
--rw-rw-rw-   0        0        0    11488 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_manylinux.py
--rw-rw-rw-   0        0        0     4378 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_musllinux.py
--rw-rw-rw-   0        0        0     1431 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_structures.py
--rw-rw-rw-   0        0        0     8496 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/packaging/markers.py
--rw-rw-rw-   0        0        0     4706 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/packaging/requirements.py
--rw-rw-rw-   0        0        0    30110 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/packaging/specifiers.py
--rw-rw-rw-   0        0        0    15699 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/packaging/tags.py
--rw-rw-rw-   0        0        0     4200 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/packaging/utils.py
--rw-rw-rw-   0        0        0    14665 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/packaging/version.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:52.850523 iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/
--rw-rw-rw-   0        0        0     9159 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/__init__.py
--rw-rw-rw-   0        0        0     6426 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/actions.py
--rw-rw-rw-   0        0        0    12936 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/common.py
--rw-rw-rw-   0        0        0   213310 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/core.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:52.853515 iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/diagram/
--rw-rw-rw-   0        0        0    23668 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/diagram/__init__.py
--rw-rw-rw-   0        0        0     9023 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/exceptions.py
--rw-rw-rw-   0        0        0    39129 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/helpers.py
--rw-rw-rw-   0        0        0    25341 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/results.py
--rw-rw-rw-   0        0        0    13402 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/testing.py
--rw-rw-rw-   0        0        0    10787 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/unicode.py
--rw-rw-rw-   0        0        0     6805 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/util.py
--rw-rw-rw-   0        0        0     8425 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/zipp.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:52.861493 iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/extern/
--rw-rw-rw-   0        0        0     2426 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/extern/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:52.919338 iniUts-1.0.3/venv/Lib/site-packages/setuptools/
--rw-rw-rw-   0        0        0     8429 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/__init__.py
--rw-rw-rw-   0        0        0      218 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_deprecation_warning.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:53.053001 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/
--rw-rw-rw-   0        0        0      537 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/__init__.py
--rw-rw-rw-   0        0        0     1330 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/_collections.py
--rw-rw-rw-   0        0        0      411 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/_functools.py
--rw-rw-rw-   0        0        0      239 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/_macos_compat.py
--rw-rw-rw-   0        0        0    19672 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/_msvccompiler.py
--rw-rw-rw-   0        0        0     8603 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/archive_util.py
--rw-rw-rw-   0        0        0    14789 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/bcppcompiler.py
--rw-rw-rw-   0        0        0    47369 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/ccompiler.py
--rw-rw-rw-   0        0        0    17973 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/cmd.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:53.088906 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/
--rw-rw-rw-   0        0        0      430 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/__init__.py
--rw-rw-rw-   0        0        0     1614 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/_framework_compat.py
--rw-rw-rw-   0        0        0     5441 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/bdist.py
--rw-rw-rw-   0        0        0     4701 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/bdist_dumb.py
--rw-rw-rw-   0        0        0    22051 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/bdist_rpm.py
--rw-rw-rw-   0        0        0     5617 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/build.py
--rw-rw-rw-   0        0        0     7728 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/build_clib.py
--rw-rw-rw-   0        0        0    31558 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/build_ext.py
--rw-rw-rw-   0        0        0    16568 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/build_py.py
--rw-rw-rw-   0        0        0     5624 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/build_scripts.py
--rw-rw-rw-   0        0        0     4888 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/check.py
--rw-rw-rw-   0        0        0     2603 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/clean.py
--rw-rw-rw-   0        0        0    13137 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/config.py
--rw-rw-rw-   0        0        0    30221 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/install.py
--rw-rw-rw-   0        0        0     2779 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/install_data.py
--rw-rw-rw-   0        0        0     2785 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/install_egg_info.py
--rw-rw-rw-   0        0        0     1189 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/install_headers.py
--rw-rw-rw-   0        0        0     8434 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/install_lib.py
--rw-rw-rw-   0        0        0     1936 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/install_scripts.py
--rw-rw-rw-   0        0        0      672 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/py37compat.py
--rw-rw-rw-   0        0        0    11765 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/register.py
--rw-rw-rw-   0        0        0    19241 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/sdist.py
--rw-rw-rw-   0        0        0     7477 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/upload.py
--rw-rw-rw-   0        0        0     4920 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/config.py
--rw-rw-rw-   0        0        0     9451 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/core.py
--rw-rw-rw-   0        0        0    12537 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/cygwinccompiler.py
--rw-rw-rw-   0        0        0      139 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/debug.py
--rw-rw-rw-   0        0        0     3423 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/dep_util.py
--rw-rw-rw-   0        0        0     8082 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/dir_util.py
--rw-rw-rw-   0        0        0    50186 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/dist.py
--rw-rw-rw-   0        0        0     3589 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/errors.py
--rw-rw-rw-   0        0        0    10270 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/extension.py
--rw-rw-rw-   0        0        0    17910 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/fancy_getopt.py
--rw-rw-rw-   0        0        0     8226 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/file_util.py
--rw-rw-rw-   0        0        0    13713 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/filelist.py
--rw-rw-rw-   0        0        0     1972 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/log.py
--rw-rw-rw-   0        0        0    30235 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/msvc9compiler.py
--rw-rw-rw-   0        0        0    23602 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/msvccompiler.py
--rw-rw-rw-   0        0        0      217 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/py38compat.py
--rw-rw-rw-   0        0        0      639 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/py39compat.py
--rw-rw-rw-   0        0        0     3517 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/spawn.py
--rw-rw-rw-   0        0        0    18858 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/sysconfig.py
--rw-rw-rw-   0        0        0    12096 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/text_file.py
--rw-rw-rw-   0        0        0    15641 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/unixccompiler.py
--rw-rw-rw-   0        0        0    18128 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/util.py
--rw-rw-rw-   0        0        0    12952 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/version.py
--rw-rw-rw-   0        0        0     5248 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/versionpredicate.py
--rw-rw-rw-   0        0        0     1972 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_entry_points.py
--rw-rw-rw-   0        0        0     2392 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_imp.py
--rw-rw-rw-   0        0        0     1311 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_importlib.py
--rw-rw-rw-   0        0        0      675 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_itertools.py
--rw-rw-rw-   0        0        0      749 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_path.py
--rw-rw-rw-   0        0        0      501 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_reqs.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:53.101870 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/
--rw-rw-rw-   0        0        0        0 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:53.121817 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/
--rw-rw-rw-   0        0        0    30130 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/__init__.py
--rw-rw-rw-   0        0        0     1862 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py
--rw-rw-rw-   0        0        0      743 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_collections.py
--rw-rw-rw-   0        0        0     1828 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_compat.py
--rw-rw-rw-   0        0        0     2895 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_functools.py
--rw-rw-rw-   0        0        0     2068 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py
--rw-rw-rw-   0        0        0     1154 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_meta.py
--rw-rw-rw-   0        0        0     2166 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_text.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:53.185647 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/
--rw-rw-rw-   0        0        0      506 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/__init__.py
--rw-rw-rw-   0        0        0     4504 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_adapters.py
--rw-rw-rw-   0        0        0     2741 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_common.py
--rw-rw-rw-   0        0        0     2706 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_compat.py
--rw-rw-rw-   0        0        0      884 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_itertools.py
--rw-rw-rw-   0        0        0     3494 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_legacy.py
--rw-rw-rw-   0        0        0     3886 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/abc.py
--rw-rw-rw-   0        0        0     3566 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/readers.py
--rw-rw-rw-   0        0        0     2836 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/simple.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:53.194622 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/jaraco/
--rw-rw-rw-   0        0        0        0 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/jaraco/__init__.py
--rw-rw-rw-   0        0        0     5420 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/jaraco/context.py
--rw-rw-rw-   0        0        0    13512 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/jaraco/functools.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:53.196617 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/jaraco/text/
--rw-rw-rw-   0        0        0    15517 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/jaraco/text/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:53.205593 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/more_itertools/
--rw-rw-rw-   0        0        0       82 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/more_itertools/__init__.py
--rw-rw-rw-   0        0        0   117959 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/more_itertools/more.py
--rw-rw-rw-   0        0        0    16256 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/more_itertools/recipes.py
--rw-rw-rw-   0        0        0    15130 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/ordered_set.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:53.224543 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/packaging/
--rw-rw-rw-   0        0        0      661 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/packaging/__about__.py
--rw-rw-rw-   0        0        0      497 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/packaging/__init__.py
--rw-rw-rw-   0        0        0    11488 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/packaging/_manylinux.py
--rw-rw-rw-   0        0        0     4378 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/packaging/_musllinux.py
--rw-rw-rw-   0        0        0     1431 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/packaging/_structures.py
--rw-rw-rw-   0        0        0     8493 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/packaging/markers.py
--rw-rw-rw-   0        0        0     4700 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/packaging/requirements.py
--rw-rw-rw-   0        0        0    30110 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/packaging/specifiers.py
--rw-rw-rw-   0        0        0    15699 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/packaging/tags.py
--rw-rw-rw-   0        0        0     4200 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/packaging/utils.py
--rw-rw-rw-   0        0        0    14665 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/packaging/version.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:53.249475 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/pyparsing/
--rw-rw-rw-   0        0        0     9159 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/pyparsing/__init__.py
--rw-rw-rw-   0        0        0     6426 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/pyparsing/actions.py
--rw-rw-rw-   0        0        0    12936 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/pyparsing/common.py
--rw-rw-rw-   0        0        0   213310 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/pyparsing/core.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:53.251470 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/pyparsing/diagram/
--rw-rw-rw-   0        0        0    23668 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/pyparsing/diagram/__init__.py
--rw-rw-rw-   0        0        0     9023 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/pyparsing/exceptions.py
--rw-rw-rw-   0        0        0    39129 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/pyparsing/helpers.py
--rw-rw-rw-   0        0        0    25341 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/pyparsing/results.py
--rw-rw-rw-   0        0        0    13402 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/pyparsing/testing.py
--rw-rw-rw-   0        0        0    10787 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/pyparsing/unicode.py
--rw-rw-rw-   0        0        0     6805 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/pyparsing/util.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:53.260447 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/tomli/
--rw-rw-rw-   0        0        0      396 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/tomli/__init__.py
--rw-rw-rw-   0        0        0    22633 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/tomli/_parser.py
--rw-rw-rw-   0        0        0     2943 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/tomli/_re.py
--rw-rw-rw-   0        0        0      254 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/tomli/_types.py
--rw-rw-rw-   0        0        0    87149 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/typing_extensions.py
--rw-rw-rw-   0        0        0     8425 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/zipp.py
--rw-rw-rw-   0        0        0     7346 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/archive_util.py
--rw-rw-rw-   0        0        0    19539 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/build_meta.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:53.312309 iniUts-1.0.3/venv/Lib/site-packages/setuptools/command/
--rw-rw-rw-   0        0        0      396 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/command/__init__.py
--rw-rw-rw-   0        0        0     2381 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/command/alias.py
--rw-rw-rw-   0        0        0    16623 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/command/bdist_egg.py
--rw-rw-rw-   0        0        0     1182 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/command/bdist_rpm.py
--rw-rw-rw-   0        0        0     6595 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/command/build.py
--rw-rw-rw-   0        0        0     4415 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/command/build_clib.py
--rw-rw-rw-   0        0        0    15821 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/command/build_ext.py
--rw-rw-rw-   0        0        0    14115 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/command/build_py.py
--rw-rw-rw-   0        0        0     7012 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/command/develop.py
--rw-rw-rw-   0        0        0     4800 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/command/dist_info.py
--rw-rw-rw-   0        0        0    85662 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/command/easy_install.py
--rw-rw-rw-   0        0        0    31188 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/command/editable_wheel.py
--rw-rw-rw-   0        0        0    26795 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/command/egg_info.py
--rw-rw-rw-   0        0        0     5163 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/command/install.py
--rw-rw-rw-   0        0        0     2226 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/command/install_egg_info.py
--rw-rw-rw-   0        0        0     3875 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/command/install_lib.py
--rw-rw-rw-   0        0        0     2612 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/command/install_scripts.py
--rw-rw-rw-   0        0        0     4946 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/command/py36compat.py
--rw-rw-rw-   0        0        0      468 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/command/register.py
--rw-rw-rw-   0        0        0     2128 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/command/rotate.py
--rw-rw-rw-   0        0        0      658 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/command/saveopts.py
--rw-rw-rw-   0        0        0     7071 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/command/sdist.py
--rw-rw-rw-   0        0        0     5086 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/command/setopt.py
--rw-rw-rw-   0        0        0     8102 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/command/test.py
--rw-rw-rw-   0        0        0      462 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/command/upload.py
--rw-rw-rw-   0        0        0     7494 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/command/upload_docs.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:53.318292 iniUts-1.0.3/venv/Lib/site-packages/setuptools/config/
--rw-rw-rw-   0        0        0     1121 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/config/__init__.py
--rw-rw-rw-   0        0        0    13398 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/config/_apply_pyprojecttoml.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:53.331257 iniUts-1.0.3/venv/Lib/site-packages/setuptools/config/_validate_pyproject/
--rw-rw-rw-   0        0        0     1038 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/config/_validate_pyproject/__init__.py
--rw-rw-rw-   0        0        0    11266 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/config/_validate_pyproject/error_reporting.py
--rw-rw-rw-   0        0        0     1153 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/config/_validate_pyproject/extra_validations.py
--rw-rw-rw-   0        0        0     1612 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py
--rw-rw-rw-   0        0        0   269900 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py
--rw-rw-rw-   0        0        0     8736 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/config/_validate_pyproject/formats.py
--rw-rw-rw-   0        0        0    16319 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/config/expand.py
--rw-rw-rw-   0        0        0    19304 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/config/pyprojecttoml.py
--rw-rw-rw-   0        0        0    25198 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/config/setupcfg.py
--rw-rw-rw-   0        0        0      949 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/dep_util.py
--rw-rw-rw-   0        0        0     5499 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/depends.py
--rw-rw-rw-   0        0        0    20799 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/discovery.py
--rw-rw-rw-   0        0        0    45578 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/dist.py
--rw-rw-rw-   0        0        0     2464 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/errors.py
--rw-rw-rw-   0        0        0     5591 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/extension.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:53.333251 iniUts-1.0.3/venv/Lib/site-packages/setuptools/extern/
--rw-rw-rw-   0        0        0     2512 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/extern/__init__.py
--rw-rw-rw-   0        0        0     4873 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/glob.py
--rw-rw-rw-   0        0        0     3824 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/installer.py
--rw-rw-rw-   0        0        0      812 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/launch.py
--rw-rw-rw-   0        0        0     1210 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/logging.py
--rw-rw-rw-   0        0        0     4857 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/monkey.py
--rw-rw-rw-   0        0        0    47724 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/msvc.py
--rw-rw-rw-   0        0        0     3093 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/namespaces.py
--rw-rw-rw-   0        0        0    40020 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/package_index.py
--rw-rw-rw-   0        0        0      245 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/py34compat.py
--rw-rw-rw-   0        0        0    14348 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/sandbox.py
--rw-rw-rw-   0        0        0      941 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/unicode_utils.py
--rw-rw-rw-   0        0        0      144 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/version.py
--rw-rw-rw-   0        0        0     8376 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/wheel.py
--rw-rw-rw-   0        0        0      718 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools/windows_support.py
-drwxrwxrwx   0        0        0        0 2023-04-26 20:12:52.953247 iniUts-1.0.3/venv/Lib/site-packages/setuptools-65.5.0.dist-info/
--rw-rw-rw-   0        0        0     2740 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools-65.5.0.dist-info/entry_points.txt
--rw-rw-rw-   0        0        0       41 2023-04-26 17:14:53.000000 iniUts-1.0.3/venv/Lib/site-packages/setuptools-65.5.0.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:46.060032 iniUts-1.0.4/
+-rw-rw-rw-   0        0        0      338 2023-04-28 14:48:16.000000 iniUts-1.0.4/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1058 2023-04-26 17:09:25.000000 iniUts-1.0.4/LICENCE.txt
+-rw-rw-rw-   0        0        0       30 2023-04-26 17:09:25.000000 iniUts-1.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     3408 2023-04-28 14:48:46.057041 iniUts-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2536 2023-04-26 18:58:33.000000 iniUts-1.0.4/README.md
+-rw-rw-rw-   0        0        0      122 2023-04-26 17:09:25.000000 iniUts-1.0.4/commands.txt
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:34.820111 iniUts-1.0.4/iniUts/
+-rw-rw-rw-   0        0        0     3430 2023-04-28 14:47:00.000000 iniUts-1.0.4/iniUts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:34.947765 iniUts-1.0.4/iniUts.egg-info/
+-rw-rw-rw-   0        0        0     3408 2023-04-28 14:48:34.000000 iniUts-1.0.4/iniUts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    42544 2023-04-28 14:48:34.000000 iniUts-1.0.4/iniUts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 14:48:34.000000 iniUts-1.0.4/iniUts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-28 14:48:34.000000 iniUts-1.0.4/iniUts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-28 14:48:34.000000 iniUts-1.0.4/iniUts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-28 14:48:46.060032 iniUts-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      751 2023-04-28 14:47:47.000000 iniUts-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:34.626626 iniUts-1.0.4/venv/
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:34.627623 iniUts-1.0.4/venv/Lib/
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:34.700429 iniUts-1.0.4/venv/Lib/site-packages/
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:34.976689 iniUts-1.0.4/venv/Lib/site-packages/_distutils_hack/
+-rw-rw-rw-   0        0        0     6128 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/_distutils_hack/__init__.py
+-rw-rw-rw-   0        0        0       44 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/_distutils_hack/override.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:34.978684 iniUts-1.0.4/venv/Lib/site-packages/dateUts/
+-rw-rw-rw-   0        0        0     4751 2023-04-26 17:23:17.000000 iniUts-1.0.4/venv/Lib/site-packages/dateUts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:35.048497 iniUts-1.0.4/venv/Lib/site-packages/dateUts-0.1.5.dist-info/
+-rw-rw-rw-   0        0        0     1058 2023-04-26 17:23:17.000000 iniUts-1.0.4/venv/Lib/site-packages/dateUts-0.1.5.dist-info/LICENCE.txt
+-rw-rw-rw-   0        0        0        8 2023-04-26 17:23:17.000000 iniUts-1.0.4/venv/Lib/site-packages/dateUts-0.1.5.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:35.147233 iniUts-1.0.4/venv/Lib/site-packages/pip/
+-rw-rw-rw-   0        0        0      357 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/__init__.py
+-rw-rw-rw-   0        0        0     1198 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/__main__.py
+-rw-rw-rw-   0        0        0     1444 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/__pip-runner__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:35.278880 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/
+-rw-rw-rw-   0        0        0      573 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/__init__.py
+-rw-rw-rw-   0        0        0    10243 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/build_env.py
+-rw-rw-rw-   0        0        0     9661 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/cache.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:35.438454 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/cli/
+-rw-rw-rw-   0        0        0      132 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/cli/__init__.py
+-rw-rw-rw-   0        0        0     6676 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/cli/autocompletion.py
+-rw-rw-rw-   0        0        0     8176 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/cli/base_command.py
+-rw-rw-rw-   0        0        0    30030 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/cli/cmdoptions.py
+-rw-rw-rw-   0        0        0      774 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/cli/command_context.py
+-rw-rw-rw-   0        0        0     2816 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/cli/main.py
+-rw-rw-rw-   0        0        0     4338 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/cli/main_parser.py
+-rw-rw-rw-   0        0        0    10817 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/cli/parser.py
+-rw-rw-rw-   0        0        0     1968 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/cli/progress_bars.py
+-rw-rw-rw-   0        0        0    18328 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/cli/req_command.py
+-rw-rw-rw-   0        0        0     5118 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/cli/spinners.py
+-rw-rw-rw-   0        0        0      116 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/cli/status_codes.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:35.686789 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/commands/
+-rw-rw-rw-   0        0        0     3882 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/commands/__init__.py
+-rw-rw-rw-   0        0        0     7581 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/commands/cache.py
+-rw-rw-rw-   0        0        0     1684 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/commands/check.py
+-rw-rw-rw-   0        0        0     4129 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/commands/completion.py
+-rw-rw-rw-   0        0        0     9815 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/commands/configuration.py
+-rw-rw-rw-   0        0        0     6591 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/commands/debug.py
+-rw-rw-rw-   0        0        0     5182 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/commands/download.py
+-rw-rw-rw-   0        0        0     2951 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/commands/freeze.py
+-rw-rw-rw-   0        0        0     1703 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/commands/hash.py
+-rw-rw-rw-   0        0        0     1132 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/commands/help.py
+-rw-rw-rw-   0        0        0     4793 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/commands/index.py
+-rw-rw-rw-   0        0        0     3188 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/commands/inspect.py
+-rw-rw-rw-   0        0        0    28722 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/commands/install.py
+-rw-rw-rw-   0        0        0    12343 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/commands/list.py
+-rw-rw-rw-   0        0        0     5697 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/commands/search.py
+-rw-rw-rw-   0        0        0     6419 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/commands/show.py
+-rw-rw-rw-   0        0        0     3886 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/commands/uninstall.py
+-rw-rw-rw-   0        0        0     6324 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/commands/wheel.py
+-rw-rw-rw-   0        0        0    13529 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/configuration.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:35.801482 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/distributions/
+-rw-rw-rw-   0        0        0      858 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/distributions/__init__.py
+-rw-rw-rw-   0        0        0     1221 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/distributions/base.py
+-rw-rw-rw-   0        0        0      729 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/distributions/installed.py
+-rw-rw-rw-   0        0        0     6494 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/distributions/sdist.py
+-rw-rw-rw-   0        0        0     1164 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/distributions/wheel.py
+-rw-rw-rw-   0        0        0    23741 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:35.850351 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/index/
+-rw-rw-rw-   0        0        0       30 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/index/__init__.py
+-rw-rw-rw-   0        0        0    16504 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/index/collector.py
+-rw-rw-rw-   0        0        0    37873 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/index/package_finder.py
+-rw-rw-rw-   0        0        0     6556 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/index/sources.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:35.943103 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/locations/
+-rw-rw-rw-   0        0        0    15365 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/locations/__init__.py
+-rw-rw-rw-   0        0        0     6100 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/locations/_distutils.py
+-rw-rw-rw-   0        0        0     7680 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/locations/_sysconfig.py
+-rw-rw-rw-   0        0        0     2556 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/locations/base.py
+-rw-rw-rw-   0        0        0      340 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/main.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:35.999951 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/metadata/
+-rw-rw-rw-   0        0        0     4280 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/metadata/__init__.py
+-rw-rw-rw-   0        0        0     2595 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/metadata/_json.py
+-rw-rw-rw-   0        0        0    25277 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/metadata/base.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:36.076745 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/metadata/importlib/
+-rw-rw-rw-   0        0        0      107 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/metadata/importlib/__init__.py
+-rw-rw-rw-   0        0        0     1882 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/metadata/importlib/_compat.py
+-rw-rw-rw-   0        0        0     8181 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/metadata/importlib/_dists.py
+-rw-rw-rw-   0        0        0     7457 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/metadata/importlib/_envs.py
+-rw-rw-rw-   0        0        0     9773 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/metadata/pkg_resources.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:36.484653 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/models/
+-rw-rw-rw-   0        0        0       63 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/models/__init__.py
+-rw-rw-rw-   0        0        0      990 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/models/candidate.py
+-rw-rw-rw-   0        0        0     6931 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/models/direct_url.py
+-rw-rw-rw-   0        0        0     2520 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/models/format_control.py
+-rw-rw-rw-   0        0        0     1030 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/models/index.py
+-rw-rw-rw-   0        0        0     2619 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/models/installation_report.py
+-rw-rw-rw-   0        0        0    18817 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/models/link.py
+-rw-rw-rw-   0        0        0      738 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/models/scheme.py
+-rw-rw-rw-   0        0        0     4643 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/models/search_scope.py
+-rw-rw-rw-   0        0        0     1907 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/models/selection_prefs.py
+-rw-rw-rw-   0        0        0     3858 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/models/target_python.py
+-rw-rw-rw-   0        0        0     3600 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/models/wheel.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:36.617299 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/network/
+-rw-rw-rw-   0        0        0       50 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/network/__init__.py
+-rw-rw-rw-   0        0        0    20435 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/network/auth.py
+-rw-rw-rw-   0        0        0     2145 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/network/cache.py
+-rw-rw-rw-   0        0        0     6096 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/network/download.py
+-rw-rw-rw-   0        0        0     7638 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/network/lazy_wheel.py
+-rw-rw-rw-   0        0        0    18442 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/network/session.py
+-rw-rw-rw-   0        0        0     4073 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/network/utils.py
+-rw-rw-rw-   0        0        0     1791 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/network/xmlrpc.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:36.670158 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/operations/
+-rw-rw-rw-   0        0        0        0 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/operations/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:36.746952 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/operations/build/
+-rw-rw-rw-   0        0        0        0 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/operations/build/__init__.py
+-rw-rw-rw-   0        0        0     4133 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/operations/build/build_tracker.py
+-rw-rw-rw-   0        0        0     1422 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/operations/build/metadata.py
+-rw-rw-rw-   0        0        0     1474 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/operations/build/metadata_editable.py
+-rw-rw-rw-   0        0        0     2198 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/operations/build/metadata_legacy.py
+-rw-rw-rw-   0        0        0     1075 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/operations/build/wheel.py
+-rw-rw-rw-   0        0        0     1417 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/operations/build/wheel_editable.py
+-rw-rw-rw-   0        0        0     3064 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/operations/build/wheel_legacy.py
+-rw-rw-rw-   0        0        0     5122 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/operations/check.py
+-rw-rw-rw-   0        0        0     9816 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/operations/freeze.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:36.801806 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/operations/install/
+-rw-rw-rw-   0        0        0       51 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/operations/install/__init__.py
+-rw-rw-rw-   0        0        0     1282 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/operations/install/editable_legacy.py
+-rw-rw-rw-   0        0        0    27475 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/operations/install/wheel.py
+-rw-rw-rw-   0        0        0    27696 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/operations/prepare.py
+-rw-rw-rw-   0        0        0     7161 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/pyproject.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:36.926473 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/req/
+-rw-rw-rw-   0        0        0     2738 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/req/__init__.py
+-rw-rw-rw-   0        0        0    16610 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/req/constructors.py
+-rw-rw-rw-   0        0        0    17872 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/req/req_file.py
+-rw-rw-rw-   0        0        0    32782 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/req/req_install.py
+-rw-rw-rw-   0        0        0     2858 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/req/req_set.py
+-rw-rw-rw-   0        0        0    24678 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/req/req_uninstall.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:36.937444 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/resolution/
+-rw-rw-rw-   0        0        0        0 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/resolution/__init__.py
+-rw-rw-rw-   0        0        0      583 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/resolution/base.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:36.956392 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/resolution/legacy/
+-rw-rw-rw-   0        0        0        0 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/resolution/legacy/__init__.py
+-rw-rw-rw-   0        0        0    24128 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/resolution/legacy/resolver.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:37.070088 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/
+-rw-rw-rw-   0        0        0        0 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/__init__.py
+-rw-rw-rw-   0        0        0     5220 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/base.py
+-rw-rw-rw-   0        0        0    18864 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/candidates.py
+-rw-rw-rw-   0        0        0    27845 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/factory.py
+-rw-rw-rw-   0        0        0     5705 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
+-rw-rw-rw-   0        0        0     9824 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/provider.py
+-rw-rw-rw-   0        0        0     3094 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/reporter.py
+-rw-rw-rw-   0        0        0     5454 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/requirements.py
+-rw-rw-rw-   0        0        0    11538 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/resolver.py
+-rw-rw-rw-   0        0        0     8167 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/self_outdated_check.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:37.410178 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/utils/__init__.py
+-rw-rw-rw-   0        0        0     3351 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/utils/_jaraco_text.py
+-rw-rw-rw-   0        0        0     1015 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/utils/_log.py
+-rw-rw-rw-   0        0        0     1665 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/utils/appdirs.py
+-rw-rw-rw-   0        0        0     1884 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/utils/compat.py
+-rw-rw-rw-   0        0        0     5377 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/utils/compatibility_tags.py
+-rw-rw-rw-   0        0        0      242 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/utils/datetime.py
+-rw-rw-rw-   0        0        0     3627 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/utils/deprecation.py
+-rw-rw-rw-   0        0        0     3206 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/utils/direct_url_helpers.py
+-rw-rw-rw-   0        0        0     2118 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/utils/egg_link.py
+-rw-rw-rw-   0        0        0     1169 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/utils/encoding.py
+-rw-rw-rw-   0        0        0     3064 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/utils/entrypoints.py
+-rw-rw-rw-   0        0        0     5122 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/utils/filesystem.py
+-rw-rw-rw-   0        0        0      716 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/utils/filetypes.py
+-rw-rw-rw-   0        0        0     3110 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/utils/glibc.py
+-rw-rw-rw-   0        0        0     5118 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/utils/hashes.py
+-rw-rw-rw-   0        0        0      795 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/utils/inject_securetransport.py
+-rw-rw-rw-   0        0        0    11632 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/utils/logging.py
+-rw-rw-rw-   0        0        0    22216 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/utils/misc.py
+-rw-rw-rw-   0        0        0     1193 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/utils/models.py
+-rw-rw-rw-   0        0        0     2108 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/utils/packaging.py
+-rw-rw-rw-   0        0        0     4435 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/utils/setuptools_build.py
+-rw-rw-rw-   0        0        0     9200 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/utils/subprocess.py
+-rw-rw-rw-   0        0        0     7702 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/utils/temp_dir.py
+-rw-rw-rw-   0        0        0     8821 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/utils/unpacking.py
+-rw-rw-rw-   0        0        0     1759 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/utils/urls.py
+-rw-rw-rw-   0        0        0     3456 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/utils/virtualenv.py
+-rw-rw-rw-   0        0        0     4549 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/utils/wheel.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:37.480988 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/vcs/
+-rw-rw-rw-   0        0        0      596 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/vcs/__init__.py
+-rw-rw-rw-   0        0        0     3519 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/vcs/bazaar.py
+-rw-rw-rw-   0        0        0    18116 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/vcs/git.py
+-rw-rw-rw-   0        0        0     5238 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/vcs/mercurial.py
+-rw-rw-rw-   0        0        0    11729 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/vcs/subversion.py
+-rw-rw-rw-   0        0        0    22811 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/vcs/versioncontrol.py
+-rw-rw-rw-   0        0        0    11842 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/wheel_builder.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:37.536838 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/
+-rw-rw-rw-   0        0        0     4966 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:37.743287 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/cachecontrol/
+-rw-rw-rw-   0        0        0      465 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/cachecontrol/__init__.py
+-rw-rw-rw-   0        0        0     1379 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/cachecontrol/_cmd.py
+-rw-rw-rw-   0        0        0     5033 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/cachecontrol/adapter.py
+-rw-rw-rw-   0        0        0     1535 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/cachecontrol/cache.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:37.907846 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/
+-rw-rw-rw-   0        0        0      242 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
+-rw-rw-rw-   0        0        0     5271 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
+-rw-rw-rw-   0        0        0     1033 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
+-rw-rw-rw-   0        0        0      778 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/cachecontrol/compat.py
+-rw-rw-rw-   0        0        0    16416 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/cachecontrol/controller.py
+-rw-rw-rw-   0        0        0     3946 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/cachecontrol/filewrapper.py
+-rw-rw-rw-   0        0        0     4154 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/cachecontrol/heuristics.py
+-rw-rw-rw-   0        0        0     7105 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/cachecontrol/serialize.py
+-rw-rw-rw-   0        0        0      774 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/cachecontrol/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:37.947740 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/certifi/
+-rw-rw-rw-   0        0        0       94 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/certifi/__init__.py
+-rw-rw-rw-   0        0        0      255 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/certifi/__main__.py
+-rw-rw-rw-   0        0        0     4279 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/certifi/core.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:38.716682 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/
+-rw-rw-rw-   0        0        0     4797 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/__init__.py
+-rw-rw-rw-   0        0        0    31274 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/big5freq.py
+-rw-rw-rw-   0        0        0     1763 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/big5prober.py
+-rw-rw-rw-   0        0        0    10032 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/chardistribution.py
+-rw-rw-rw-   0        0        0     3915 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/charsetgroupprober.py
+-rw-rw-rw-   0        0        0     5420 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/charsetprober.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:38.732639 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/cli/
+-rw-rw-rw-   0        0        0        0 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/cli/__init__.py
+-rw-rw-rw-   0        0        0     3242 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/cli/chardetect.py
+-rw-rw-rw-   0        0        0     3732 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachine.py
+-rw-rw-rw-   0        0        0      542 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachinedict.py
+-rw-rw-rw-   0        0        0     1860 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/cp949prober.py
+-rw-rw-rw-   0        0        0     1683 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/enums.py
+-rw-rw-rw-   0        0        0     4006 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/escprober.py
+-rw-rw-rw-   0        0        0    12176 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/escsm.py
+-rw-rw-rw-   0        0        0     3934 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/eucjpprober.py
+-rw-rw-rw-   0        0        0    13566 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/euckrfreq.py
+-rw-rw-rw-   0        0        0     1753 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/euckrprober.py
+-rw-rw-rw-   0        0        0    36913 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/euctwfreq.py
+-rw-rw-rw-   0        0        0     1753 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/euctwprober.py
+-rw-rw-rw-   0        0        0    20735 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/gb2312freq.py
+-rw-rw-rw-   0        0        0     1759 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/gb2312prober.py
+-rw-rw-rw-   0        0        0    14537 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/hebrewprober.py
+-rw-rw-rw-   0        0        0    25796 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/jisfreq.py
+-rw-rw-rw-   0        0        0    42498 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/johabfreq.py
+-rw-rw-rw-   0        0        0     1752 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/johabprober.py
+-rw-rw-rw-   0        0        0    27055 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/jpcntx.py
+-rw-rw-rw-   0        0        0   104562 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
+-rw-rw-rw-   0        0        0    98484 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/langgreekmodel.py
+-rw-rw-rw-   0        0        0    98196 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/langhebrewmodel.py
+-rw-rw-rw-   0        0        0   101363 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/langhungarianmodel.py
+-rw-rw-rw-   0        0        0   128035 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/langrussianmodel.py
+-rw-rw-rw-   0        0        0   102774 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/langthaimodel.py
+-rw-rw-rw-   0        0        0    95372 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/langturkishmodel.py
+-rw-rw-rw-   0        0        0     5380 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/latin1prober.py
+-rw-rw-rw-   0        0        0     6077 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/macromanprober.py
+-rw-rw-rw-   0        0        0     3715 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/mbcharsetprober.py
+-rw-rw-rw-   0        0        0     2131 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
+-rw-rw-rw-   0        0        0    30391 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/mbcssm.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:38.749593 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/metadata/
+-rw-rw-rw-   0        0        0        0 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/metadata/__init__.py
+-rw-rw-rw-   0        0        0    13560 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/metadata/languages.py
+-rw-rw-rw-   0        0        0      402 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/resultdict.py
+-rw-rw-rw-   0        0        0     6400 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/sbcharsetprober.py
+-rw-rw-rw-   0        0        0     4137 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
+-rw-rw-rw-   0        0        0     4007 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/sjisprober.py
+-rw-rw-rw-   0        0        0    14848 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/universaldetector.py
+-rw-rw-rw-   0        0        0     8505 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/utf1632prober.py
+-rw-rw-rw-   0        0        0     2812 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/utf8prober.py
+-rw-rw-rw-   0        0        0      244 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/version.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:38.857306 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/colorama/
+-rw-rw-rw-   0        0        0      266 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/colorama/__init__.py
+-rw-rw-rw-   0        0        0     2522 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/colorama/ansi.py
+-rw-rw-rw-   0        0        0    11128 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/colorama/ansitowin32.py
+-rw-rw-rw-   0        0        0     3325 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/colorama/initialise.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:38.955044 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/colorama/tests/
+-rw-rw-rw-   0        0        0       75 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/colorama/tests/__init__.py
+-rw-rw-rw-   0        0        0     2839 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/colorama/tests/ansi_test.py
+-rw-rw-rw-   0        0        0    10678 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py
+-rw-rw-rw-   0        0        0     6741 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/colorama/tests/initialise_test.py
+-rw-rw-rw-   0        0        0     1866 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/colorama/tests/isatty_test.py
+-rw-rw-rw-   0        0        0     1079 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/colorama/tests/utils.py
+-rw-rw-rw-   0        0        0     3709 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/colorama/tests/winterm_test.py
+-rw-rw-rw-   0        0        0     6181 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/colorama/win32.py
+-rw-rw-rw-   0        0        0     7134 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/colorama/winterm.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:39.239283 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/distlib/
+-rw-rw-rw-   0        0        0      581 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/distlib/__init__.py
+-rw-rw-rw-   0        0        0    41259 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/distlib/compat.py
+-rw-rw-rw-   0        0        0    51697 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/distlib/database.py
+-rw-rw-rw-   0        0        0    20834 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/distlib/index.py
+-rw-rw-rw-   0        0        0    51991 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/distlib/locators.py
+-rw-rw-rw-   0        0        0    14811 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/distlib/manifest.py
+-rw-rw-rw-   0        0        0     5058 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/distlib/markers.py
+-rw-rw-rw-   0        0        0    39801 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/distlib/metadata.py
+-rw-rw-rw-   0        0        0    10820 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/distlib/resources.py
+-rw-rw-rw-   0        0        0    18102 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/distlib/scripts.py
+-rw-rw-rw-   0        0        0    66262 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/distlib/util.py
+-rw-rw-rw-   0        0        0    23513 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/distlib/version.py
+-rw-rw-rw-   0        0        0    43898 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/distlib/wheel.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:39.374921 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/distro/
+-rw-rw-rw-   0        0        0      981 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/distro/__init__.py
+-rw-rw-rw-   0        0        0       64 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/distro/__main__.py
+-rw-rw-rw-   0        0        0    49330 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/distro/distro.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:39.501581 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/idna/
+-rw-rw-rw-   0        0        0      849 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/idna/__init__.py
+-rw-rw-rw-   0        0        0     3374 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/idna/codec.py
+-rw-rw-rw-   0        0        0      321 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/idna/compat.py
+-rw-rw-rw-   0        0        0    12950 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/idna/core.py
+-rw-rw-rw-   0        0        0    44375 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/idna/idnadata.py
+-rw-rw-rw-   0        0        0     1881 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/idna/intranges.py
+-rw-rw-rw-   0        0        0       21 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/idna/package_data.py
+-rw-rw-rw-   0        0        0   206539 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/idna/uts46data.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:39.545464 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/msgpack/
+-rw-rw-rw-   0        0        0     1132 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/msgpack/__init__.py
+-rw-rw-rw-   0        0        0     1081 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/msgpack/exceptions.py
+-rw-rw-rw-   0        0        0     6079 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/msgpack/ext.py
+-rw-rw-rw-   0        0        0    34544 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/msgpack/fallback.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:39.670131 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/packaging/
+-rw-rw-rw-   0        0        0      661 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/packaging/__about__.py
+-rw-rw-rw-   0        0        0      497 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/packaging/__init__.py
+-rw-rw-rw-   0        0        0    11488 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/packaging/_manylinux.py
+-rw-rw-rw-   0        0        0     4378 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/packaging/_musllinux.py
+-rw-rw-rw-   0        0        0     1431 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/packaging/_structures.py
+-rw-rw-rw-   0        0        0     8487 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/packaging/markers.py
+-rw-rw-rw-   0        0        0     4676 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/packaging/requirements.py
+-rw-rw-rw-   0        0        0    30110 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/packaging/specifiers.py
+-rw-rw-rw-   0        0        0    15699 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/packaging/tags.py
+-rw-rw-rw-   0        0        0     4200 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/packaging/utils.py
+-rw-rw-rw-   0        0        0    14665 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/packaging/version.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:39.692073 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pkg_resources/
+-rw-rw-rw-   0        0        0   109388 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pkg_resources/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:39.823719 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/platformdirs/
+-rw-rw-rw-   0        0        0    18003 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/platformdirs/__init__.py
+-rw-rw-rw-   0        0        0     1198 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/platformdirs/__main__.py
+-rw-rw-rw-   0        0        0     4303 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/platformdirs/android.py
+-rw-rw-rw-   0        0        0     5706 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/platformdirs/api.py
+-rw-rw-rw-   0        0        0     2800 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/platformdirs/macos.py
+-rw-rw-rw-   0        0        0     7448 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/platformdirs/unix.py
+-rw-rw-rw-   0        0        0      160 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/platformdirs/version.py
+-rw-rw-rw-   0        0        0     7098 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/platformdirs/windows.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:40.063079 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/
+-rw-rw-rw-   0        0        0     2999 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/__init__.py
+-rw-rw-rw-   0        0        0      353 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/__main__.py
+-rw-rw-rw-   0        0        0    23685 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/cmdline.py
+-rw-rw-rw-   0        0        0     1697 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/console.py
+-rw-rw-rw-   0        0        0     1938 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/filter.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:40.075047 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/filters/
+-rw-rw-rw-   0        0        0    40386 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/filters/__init__.py
+-rw-rw-rw-   0        0        0     2917 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/formatter.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:40.404166 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/formatters/
+-rw-rw-rw-   0        0        0     4800 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/formatters/__init__.py
+-rw-rw-rw-   0        0        0     4104 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/formatters/_mapping.py
+-rw-rw-rw-   0        0        0     3314 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/formatters/bbcode.py
+-rw-rw-rw-   0        0        0     5086 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/formatters/groff.py
+-rw-rw-rw-   0        0        0    35601 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/formatters/html.py
+-rw-rw-rw-   0        0        0    21938 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/formatters/img.py
+-rw-rw-rw-   0        0        0     4981 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/formatters/irc.py
+-rw-rw-rw-   0        0        0    19351 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/formatters/latex.py
+-rw-rw-rw-   0        0        0     5073 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/formatters/other.py
+-rw-rw-rw-   0        0        0     2212 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
+-rw-rw-rw-   0        0        0     5014 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/formatters/rtf.py
+-rw-rw-rw-   0        0        0     7335 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/formatters/svg.py
+-rw-rw-rw-   0        0        0     4674 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal.py
+-rw-rw-rw-   0        0        0    11753 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal256.py
+-rw-rw-rw-   0        0        0    32064 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/lexer.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:40.461014 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/lexers/
+-rw-rw-rw-   0        0        0    11164 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/lexers/__init__.py
+-rw-rw-rw-   0        0        0    71556 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/lexers/_mapping.py
+-rw-rw-rw-   0        0        0    53572 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/lexers/python.py
+-rw-rw-rw-   0        0        0      986 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/modeline.py
+-rw-rw-rw-   0        0        0     2591 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/plugin.py
+-rw-rw-rw-   0        0        0     3072 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/regexopt.py
+-rw-rw-rw-   0        0        0     3092 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/scanner.py
+-rw-rw-rw-   0        0        0     6882 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/sphinxext.py
+-rw-rw-rw-   0        0        0     6257 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/style.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:40.476972 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/styles/
+-rw-rw-rw-   0        0        0     3419 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/styles/__init__.py
+-rw-rw-rw-   0        0        0     6184 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/token.py
+-rw-rw-rw-   0        0        0    63187 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/unistring.py
+-rw-rw-rw-   0        0        0     9110 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/util.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:40.649510 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pyparsing/
+-rw-rw-rw-   0        0        0     9171 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pyparsing/__init__.py
+-rw-rw-rw-   0        0        0     6426 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pyparsing/actions.py
+-rw-rw-rw-   0        0        0    12936 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pyparsing/common.py
+-rw-rw-rw-   0        0        0   213344 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pyparsing/core.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:40.661477 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pyparsing/diagram/
+-rw-rw-rw-   0        0        0    23685 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
+-rw-rw-rw-   0        0        0     9023 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pyparsing/exceptions.py
+-rw-rw-rw-   0        0        0    39129 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pyparsing/helpers.py
+-rw-rw-rw-   0        0        0    25341 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pyparsing/results.py
+-rw-rw-rw-   0        0        0    13402 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pyparsing/testing.py
+-rw-rw-rw-   0        0        0    10787 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pyparsing/unicode.py
+-rw-rw-rw-   0        0        0     6805 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pyparsing/util.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:40.825040 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/
+-rw-rw-rw-   0        0        0      491 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/__init__.py
+-rw-rw-rw-   0        0        0      138 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_compat.py
+-rw-rw-rw-   0        0        0    11920 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_impl.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:40.856955 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/
+-rw-rw-rw-   0        0        0      546 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py
+-rw-rw-rw-   0        0        0    10927 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:41.111275 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/requests/
+-rw-rw-rw-   0        0        0     5178 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/requests/__init__.py
+-rw-rw-rw-   0        0        0      435 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/requests/__version__.py
+-rw-rw-rw-   0        0        0     1397 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/requests/_internal_utils.py
+-rw-rw-rw-   0        0        0    21443 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/requests/adapters.py
+-rw-rw-rw-   0        0        0     6377 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/requests/api.py
+-rw-rw-rw-   0        0        0    10187 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/requests/auth.py
+-rw-rw-rw-   0        0        0      575 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/requests/certs.py
+-rw-rw-rw-   0        0        0     1286 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/requests/compat.py
+-rw-rw-rw-   0        0        0    18560 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/requests/cookies.py
+-rw-rw-rw-   0        0        0     3823 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/requests/exceptions.py
+-rw-rw-rw-   0        0        0     3879 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/requests/help.py
+-rw-rw-rw-   0        0        0      733 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/requests/hooks.py
+-rw-rw-rw-   0        0        0    35288 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/requests/models.py
+-rw-rw-rw-   0        0        0      695 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/requests/packages.py
+-rw-rw-rw-   0        0        0    30180 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/requests/sessions.py
+-rw-rw-rw-   0        0        0     4235 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/requests/status_codes.py
+-rw-rw-rw-   0        0        0     2912 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/requests/structures.py
+-rw-rw-rw-   0        0        0    33240 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/requests/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:41.163136 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/resolvelib/
+-rw-rw-rw-   0        0        0      537 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/resolvelib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:41.174106 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/resolvelib/compat/
+-rw-rw-rw-   0        0        0        0 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/resolvelib/compat/__init__.py
+-rw-rw-rw-   0        0        0      156 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
+-rw-rw-rw-   0        0        0     5871 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/resolvelib/providers.py
+-rw-rw-rw-   0        0        0     1601 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/resolvelib/reporters.py
+-rw-rw-rw-   0        0        0    20511 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/resolvelib/resolvers.py
+-rw-rw-rw-   0        0        0     4963 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/resolvelib/structs.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:42.442712 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/
+-rw-rw-rw-   0        0        0     6090 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/__init__.py
+-rw-rw-rw-   0        0        0     8478 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/__main__.py
+-rw-rw-rw-   0        0        0    10096 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/_cell_widths.py
+-rw-rw-rw-   0        0        0   140235 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/_emoji_codes.py
+-rw-rw-rw-   0        0        0     1064 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/_emoji_replace.py
+-rw-rw-rw-   0        0        0     2100 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/_export_format.py
+-rw-rw-rw-   0        0        0      265 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/_extension.py
+-rw-rw-rw-   0        0        0      799 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/_fileno.py
+-rw-rw-rw-   0        0        0     9695 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/_inspect.py
+-rw-rw-rw-   0        0        0     3225 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/_log_render.py
+-rw-rw-rw-   0        0        0     1236 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/_loop.py
+-rw-rw-rw-   0        0        0     1387 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/_null_file.py
+-rw-rw-rw-   0        0        0     7063 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/_palettes.py
+-rw-rw-rw-   0        0        0      423 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/_pick.py
+-rw-rw-rw-   0        0        0     5472 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/_ratio.py
+-rw-rw-rw-   0        0        0    19919 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/_spinners.py
+-rw-rw-rw-   0        0        0      351 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/_stack.py
+-rw-rw-rw-   0        0        0      417 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/_timer.py
+-rw-rw-rw-   0        0        0    22820 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/_win32_console.py
+-rw-rw-rw-   0        0        0     1926 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/_windows.py
+-rw-rw-rw-   0        0        0     2783 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/_windows_renderer.py
+-rw-rw-rw-   0        0        0     1840 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/_wrap.py
+-rw-rw-rw-   0        0        0      890 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/abc.py
+-rw-rw-rw-   0        0        0    10368 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/align.py
+-rw-rw-rw-   0        0        0     6906 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/ansi.py
+-rw-rw-rw-   0        0        0     3264 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/bar.py
+-rw-rw-rw-   0        0        0     9842 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/box.py
+-rw-rw-rw-   0        0        0     4509 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/cells.py
+-rw-rw-rw-   0        0        0    18224 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/color.py
+-rw-rw-rw-   0        0        0     1054 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/color_triplet.py
+-rw-rw-rw-   0        0        0     7131 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/columns.py
+-rw-rw-rw-   0        0        0    99195 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/console.py
+-rw-rw-rw-   0        0        0     1288 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/constrain.py
+-rw-rw-rw-   0        0        0     5497 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/containers.py
+-rw-rw-rw-   0        0        0     6630 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/control.py
+-rw-rw-rw-   0        0        0     8082 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/default_styles.py
+-rw-rw-rw-   0        0        0      972 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/diagnose.py
+-rw-rw-rw-   0        0        0     2501 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/emoji.py
+-rw-rw-rw-   0        0        0      642 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/errors.py
+-rw-rw-rw-   0        0        0     1683 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/file_proxy.py
+-rw-rw-rw-   0        0        0     2508 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/filesize.py
+-rw-rw-rw-   0        0        0     9584 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/highlighter.py
+-rw-rw-rw-   0        0        0     5032 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/json.py
+-rw-rw-rw-   0        0        0     3252 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/jupyter.py
+-rw-rw-rw-   0        0        0    14007 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/layout.py
+-rw-rw-rw-   0        0        0    14273 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/live.py
+-rw-rw-rw-   0        0        0     3667 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/live_render.py
+-rw-rw-rw-   0        0        0    11903 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/logging.py
+-rw-rw-rw-   0        0        0     8198 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/markup.py
+-rw-rw-rw-   0        0        0     5305 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/measure.py
+-rw-rw-rw-   0        0        0     4970 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/padding.py
+-rw-rw-rw-   0        0        0      828 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/pager.py
+-rw-rw-rw-   0        0        0     3396 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/palette.py
+-rw-rw-rw-   0        0        0    10574 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/panel.py
+-rw-rw-rw-   0        0        0    35852 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/pretty.py
+-rw-rw-rw-   0        0        0    59706 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/progress.py
+-rw-rw-rw-   0        0        0     8165 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/progress_bar.py
+-rw-rw-rw-   0        0        0    11303 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/prompt.py
+-rw-rw-rw-   0        0        0     1391 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/protocol.py
+-rw-rw-rw-   0        0        0      166 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/region.py
+-rw-rw-rw-   0        0        0     4431 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/repr.py
+-rw-rw-rw-   0        0        0     4602 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/rule.py
+-rw-rw-rw-   0        0        0     2843 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/scope.py
+-rw-rw-rw-   0        0        0     1591 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/screen.py
+-rw-rw-rw-   0        0        0    24247 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/segment.py
+-rw-rw-rw-   0        0        0     4339 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/spinner.py
+-rw-rw-rw-   0        0        0     4425 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/status.py
+-rw-rw-rw-   0        0        0    27073 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/style.py
+-rw-rw-rw-   0        0        0     1258 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/styled.py
+-rw-rw-rw-   0        0        0    35153 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/syntax.py
+-rw-rw-rw-   0        0        0    39684 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/table.py
+-rw-rw-rw-   0        0        0     3370 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/terminal_theme.py
+-rw-rw-rw-   0        0        0    45525 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/text.py
+-rw-rw-rw-   0        0        0     3777 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/theme.py
+-rw-rw-rw-   0        0        0      102 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/themes.py
+-rw-rw-rw-   0        0        0    29604 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/traceback.py
+-rw-rw-rw-   0        0        0     9169 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/tree.py
+-rw-rw-rw-   0        0        0    34549 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/six.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:42.561394 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/tenacity/
+-rw-rw-rw-   0        0        0    20493 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/tenacity/__init__.py
+-rw-rw-rw-   0        0        0     3551 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/tenacity/_asyncio.py
+-rw-rw-rw-   0        0        0     2179 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/tenacity/_utils.py
+-rw-rw-rw-   0        0        0     1682 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/tenacity/after.py
+-rw-rw-rw-   0        0        0     1562 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/tenacity/before.py
+-rw-rw-rw-   0        0        0     2372 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/tenacity/before_sleep.py
+-rw-rw-rw-   0        0        0     1383 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/tenacity/nap.py
+-rw-rw-rw-   0        0        0     8746 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/tenacity/retry.py
+-rw-rw-rw-   0        0        0     3086 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/tenacity/stop.py
+-rw-rw-rw-   0        0        0     2142 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/tenacity/tornadoweb.py
+-rw-rw-rw-   0        0        0     8024 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/tenacity/wait.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:42.611261 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/tomli/
+-rw-rw-rw-   0        0        0      396 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/tomli/__init__.py
+-rw-rw-rw-   0        0        0    22633 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/tomli/_parser.py
+-rw-rw-rw-   0        0        0     2943 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/tomli/_re.py
+-rw-rw-rw-   0        0        0      254 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/tomli/_types.py
+-rw-rw-rw-   0        0        0    84101 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/typing_extensions.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:42.765847 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/
+-rw-rw-rw-   0        0        0     3333 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/__init__.py
+-rw-rw-rw-   0        0        0    10811 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/_collections.py
+-rw-rw-rw-   0        0        0       64 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/_version.py
+-rw-rw-rw-   0        0        0    20300 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/connection.py
+-rw-rw-rw-   0        0        0    39128 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/connectionpool.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:42.906471 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/
+-rw-rw-rw-   0        0        0        0 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/__init__.py
+-rw-rw-rw-   0        0        0      957 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:42.968306 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/
+-rw-rw-rw-   0        0        0        0 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
+-rw-rw-rw-   0        0        0    17632 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
+-rw-rw-rw-   0        0        0    13922 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
+-rw-rw-rw-   0        0        0    11036 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/appengine.py
+-rw-rw-rw-   0        0        0     4528 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
+-rw-rw-rw-   0        0        0    17081 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
+-rw-rw-rw-   0        0        0    34448 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
+-rw-rw-rw-   0        0        0     7097 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/socks.py
+-rw-rw-rw-   0        0        0     8217 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/exceptions.py
+-rw-rw-rw-   0        0        0     8579 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/fields.py
+-rw-rw-rw-   0        0        0     2440 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/filepost.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:42.996231 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/packages/
+-rw-rw-rw-   0        0        0        0 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/packages/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:43.011191 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/
+-rw-rw-rw-   0        0        0        0 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
+-rw-rw-rw-   0        0        0     1417 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
+-rw-rw-rw-   0        0        0    34665 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/packages/six.py
+-rw-rw-rw-   0        0        0    19786 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/poolmanager.py
+-rw-rw-rw-   0        0        0     5985 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/request.py
+-rw-rw-rw-   0        0        0    30641 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/response.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:43.250549 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/util/
+-rw-rw-rw-   0        0        0     1155 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/util/__init__.py
+-rw-rw-rw-   0        0        0     4901 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/util/connection.py
+-rw-rw-rw-   0        0        0     1605 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/util/proxy.py
+-rw-rw-rw-   0        0        0      498 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/util/queue.py
+-rw-rw-rw-   0        0        0     3997 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/util/request.py
+-rw-rw-rw-   0        0        0     3510 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/util/response.py
+-rw-rw-rw-   0        0        0    22003 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/util/retry.py
+-rw-rw-rw-   0        0        0    17177 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_.py
+-rw-rw-rw-   0        0        0     5758 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
+-rw-rw-rw-   0        0        0     6895 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssltransport.py
+-rw-rw-rw-   0        0        0    10168 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/util/timeout.py
+-rw-rw-rw-   0        0        0    14296 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/util/url.py
+-rw-rw-rw-   0        0        0     5403 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/util/wait.py
+-rw-rw-rw-   0        0        0      476 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/vendor.txt
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:43.340310 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/webencodings/
+-rw-rw-rw-   0        0        0    10579 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/webencodings/__init__.py
+-rw-rw-rw-   0        0        0     8979 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/webencodings/labels.py
+-rw-rw-rw-   0        0        0     1305 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/webencodings/mklabels.py
+-rw-rw-rw-   0        0        0     6563 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/webencodings/tests.py
+-rw-rw-rw-   0        0        0     4307 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/webencodings/x_user_defined.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:35.175158 iniUts-1.0.4/venv/Lib/site-packages/pip-23.1.2.dist-info/
+-rw-rw-rw-   0        0        0     9953 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip-23.1.2.dist-info/AUTHORS.txt
+-rw-rw-rw-   0        0        0     1093 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip-23.1.2.dist-info/LICENSE.txt
+-rw-rw-rw-   0        0        0      125 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip-23.1.2.dist-info/entry_points.txt
+-rw-rw-rw-   0        0        0        4 2023-04-26 17:15:05.000000 iniUts-1.0.4/venv/Lib/site-packages/pip-23.1.2.dist-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:43.360257 iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/
+-rw-rw-rw-   0        0        0   108568 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:43.396160 iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/
+-rw-rw-rw-   0        0        0        0 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/__init__.py
+-rw-rw-rw-   0        0        0    24701 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/appdirs.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:43.562714 iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/
+-rw-rw-rw-   0        0        0      506 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/__init__.py
+-rw-rw-rw-   0        0        0     4504 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py
+-rw-rw-rw-   0        0        0     2741 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_common.py
+-rw-rw-rw-   0        0        0     2706 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py
+-rw-rw-rw-   0        0        0      884 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py
+-rw-rw-rw-   0        0        0     3494 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py
+-rw-rw-rw-   0        0        0     3886 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/abc.py
+-rw-rw-rw-   0        0        0     3566 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/readers.py
+-rw-rw-rw-   0        0        0     2836 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/simple.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:43.631531 iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/
+-rw-rw-rw-   0        0        0        0 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/__init__.py
+-rw-rw-rw-   0        0        0     5420 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/context.py
+-rw-rw-rw-   0        0        0    13515 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/functools.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:43.644497 iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/text/
+-rw-rw-rw-   0        0        0    15526 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:43.687383 iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/
+-rw-rw-rw-   0        0        0       83 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/__init__.py
+-rw-rw-rw-   0        0        0   132569 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/more.py
+-rw-rw-rw-   0        0        0    18410 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/recipes.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:43.761184 iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/packaging/
+-rw-rw-rw-   0        0        0      661 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/packaging/__about__.py
+-rw-rw-rw-   0        0        0      497 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/packaging/__init__.py
+-rw-rw-rw-   0        0        0    11488 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_manylinux.py
+-rw-rw-rw-   0        0        0     4378 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_musllinux.py
+-rw-rw-rw-   0        0        0     1431 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_structures.py
+-rw-rw-rw-   0        0        0     8496 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/packaging/markers.py
+-rw-rw-rw-   0        0        0     4706 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/packaging/requirements.py
+-rw-rw-rw-   0        0        0    30110 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/packaging/specifiers.py
+-rw-rw-rw-   0        0        0    15699 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/packaging/tags.py
+-rw-rw-rw-   0        0        0     4200 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/packaging/utils.py
+-rw-rw-rw-   0        0        0    14665 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/packaging/version.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:43.893829 iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/
+-rw-rw-rw-   0        0        0     9159 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/__init__.py
+-rw-rw-rw-   0        0        0     6426 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/actions.py
+-rw-rw-rw-   0        0        0    12936 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/common.py
+-rw-rw-rw-   0        0        0   213310 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/core.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:43.904803 iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/diagram/
+-rw-rw-rw-   0        0        0    23668 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/diagram/__init__.py
+-rw-rw-rw-   0        0        0     9023 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/exceptions.py
+-rw-rw-rw-   0        0        0    39129 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/helpers.py
+-rw-rw-rw-   0        0        0    25341 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/results.py
+-rw-rw-rw-   0        0        0    13402 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/testing.py
+-rw-rw-rw-   0        0        0    10787 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/unicode.py
+-rw-rw-rw-   0        0        0     6805 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/util.py
+-rw-rw-rw-   0        0        0     8425 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/zipp.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:43.917765 iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/extern/
+-rw-rw-rw-   0        0        0     2426 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/extern/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:44.291765 iniUts-1.0.4/venv/Lib/site-packages/setuptools/
+-rw-rw-rw-   0        0        0     8429 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/__init__.py
+-rw-rw-rw-   0        0        0      218 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_deprecation_warning.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:44.784446 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/
+-rw-rw-rw-   0        0        0      537 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/__init__.py
+-rw-rw-rw-   0        0        0     1330 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/_collections.py
+-rw-rw-rw-   0        0        0      411 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/_functools.py
+-rw-rw-rw-   0        0        0      239 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/_macos_compat.py
+-rw-rw-rw-   0        0        0    19672 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/_msvccompiler.py
+-rw-rw-rw-   0        0        0     8603 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/archive_util.py
+-rw-rw-rw-   0        0        0    14789 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/bcppcompiler.py
+-rw-rw-rw-   0        0        0    47369 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/ccompiler.py
+-rw-rw-rw-   0        0        0    17973 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/cmd.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:45.091624 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/command/
+-rw-rw-rw-   0        0        0      430 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/command/__init__.py
+-rw-rw-rw-   0        0        0     1614 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/command/_framework_compat.py
+-rw-rw-rw-   0        0        0     5441 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/command/bdist.py
+-rw-rw-rw-   0        0        0     4701 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/command/bdist_dumb.py
+-rw-rw-rw-   0        0        0    22051 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/command/bdist_rpm.py
+-rw-rw-rw-   0        0        0     5617 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/command/build.py
+-rw-rw-rw-   0        0        0     7728 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/command/build_clib.py
+-rw-rw-rw-   0        0        0    31558 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/command/build_ext.py
+-rw-rw-rw-   0        0        0    16568 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/command/build_py.py
+-rw-rw-rw-   0        0        0     5624 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/command/build_scripts.py
+-rw-rw-rw-   0        0        0     4888 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/command/check.py
+-rw-rw-rw-   0        0        0     2603 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/command/clean.py
+-rw-rw-rw-   0        0        0    13137 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/command/config.py
+-rw-rw-rw-   0        0        0    30221 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/command/install.py
+-rw-rw-rw-   0        0        0     2779 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/command/install_data.py
+-rw-rw-rw-   0        0        0     2785 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/command/install_egg_info.py
+-rw-rw-rw-   0        0        0     1189 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/command/install_headers.py
+-rw-rw-rw-   0        0        0     8434 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/command/install_lib.py
+-rw-rw-rw-   0        0        0     1936 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/command/install_scripts.py
+-rw-rw-rw-   0        0        0      672 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/command/py37compat.py
+-rw-rw-rw-   0        0        0    11765 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/command/register.py
+-rw-rw-rw-   0        0        0    19241 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/command/sdist.py
+-rw-rw-rw-   0        0        0     7477 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/command/upload.py
+-rw-rw-rw-   0        0        0     4920 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/config.py
+-rw-rw-rw-   0        0        0     9451 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/core.py
+-rw-rw-rw-   0        0        0    12537 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/cygwinccompiler.py
+-rw-rw-rw-   0        0        0      139 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/debug.py
+-rw-rw-rw-   0        0        0     3423 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/dep_util.py
+-rw-rw-rw-   0        0        0     8082 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/dir_util.py
+-rw-rw-rw-   0        0        0    50186 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/dist.py
+-rw-rw-rw-   0        0        0     3589 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/errors.py
+-rw-rw-rw-   0        0        0    10270 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/extension.py
+-rw-rw-rw-   0        0        0    17910 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/fancy_getopt.py
+-rw-rw-rw-   0        0        0     8226 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/file_util.py
+-rw-rw-rw-   0        0        0    13713 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/filelist.py
+-rw-rw-rw-   0        0        0     1972 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/log.py
+-rw-rw-rw-   0        0        0    30235 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/msvc9compiler.py
+-rw-rw-rw-   0        0        0    23602 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/msvccompiler.py
+-rw-rw-rw-   0        0        0      217 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/py38compat.py
+-rw-rw-rw-   0        0        0      639 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/py39compat.py
+-rw-rw-rw-   0        0        0     3517 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/spawn.py
+-rw-rw-rw-   0        0        0    18858 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/sysconfig.py
+-rw-rw-rw-   0        0        0    12096 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/text_file.py
+-rw-rw-rw-   0        0        0    15641 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/unixccompiler.py
+-rw-rw-rw-   0        0        0    18128 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/util.py
+-rw-rw-rw-   0        0        0    12952 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/version.py
+-rw-rw-rw-   0        0        0     5248 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/versionpredicate.py
+-rw-rw-rw-   0        0        0     1972 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_entry_points.py
+-rw-rw-rw-   0        0        0     2392 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_imp.py
+-rw-rw-rw-   0        0        0     1311 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_importlib.py
+-rw-rw-rw-   0        0        0      675 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_itertools.py
+-rw-rw-rw-   0        0        0      749 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_path.py
+-rw-rw-rw-   0        0        0      501 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_reqs.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:45.134509 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/
+-rw-rw-rw-   0        0        0        0 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:45.228258 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/
+-rw-rw-rw-   0        0        0    30130 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/__init__.py
+-rw-rw-rw-   0        0        0     1862 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py
+-rw-rw-rw-   0        0        0      743 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_collections.py
+-rw-rw-rw-   0        0        0     1828 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_compat.py
+-rw-rw-rw-   0        0        0     2895 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_functools.py
+-rw-rw-rw-   0        0        0     2068 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py
+-rw-rw-rw-   0        0        0     1154 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_meta.py
+-rw-rw-rw-   0        0        0     2166 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_text.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:45.258178 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/
+-rw-rw-rw-   0        0        0      506 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/__init__.py
+-rw-rw-rw-   0        0        0     4504 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_adapters.py
+-rw-rw-rw-   0        0        0     2741 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_common.py
+-rw-rw-rw-   0        0        0     2706 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_compat.py
+-rw-rw-rw-   0        0        0      884 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_itertools.py
+-rw-rw-rw-   0        0        0     3494 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_legacy.py
+-rw-rw-rw-   0        0        0     3886 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/abc.py
+-rw-rw-rw-   0        0        0     3566 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/readers.py
+-rw-rw-rw-   0        0        0     2836 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/simple.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:45.279123 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/jaraco/
+-rw-rw-rw-   0        0        0        0 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/jaraco/__init__.py
+-rw-rw-rw-   0        0        0     5420 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/jaraco/context.py
+-rw-rw-rw-   0        0        0    13512 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/jaraco/functools.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:45.292089 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/jaraco/text/
+-rw-rw-rw-   0        0        0    15517 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/jaraco/text/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:45.327991 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/more_itertools/
+-rw-rw-rw-   0        0        0       82 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/more_itertools/__init__.py
+-rw-rw-rw-   0        0        0   117959 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/more_itertools/more.py
+-rw-rw-rw-   0        0        0    16256 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/more_itertools/recipes.py
+-rw-rw-rw-   0        0        0    15130 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/ordered_set.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:45.400797 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/packaging/
+-rw-rw-rw-   0        0        0      661 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/packaging/__about__.py
+-rw-rw-rw-   0        0        0      497 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/packaging/__init__.py
+-rw-rw-rw-   0        0        0    11488 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/packaging/_manylinux.py
+-rw-rw-rw-   0        0        0     4378 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/packaging/_musllinux.py
+-rw-rw-rw-   0        0        0     1431 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/packaging/_structures.py
+-rw-rw-rw-   0        0        0     8493 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/packaging/markers.py
+-rw-rw-rw-   0        0        0     4700 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/packaging/requirements.py
+-rw-rw-rw-   0        0        0    30110 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/packaging/specifiers.py
+-rw-rw-rw-   0        0        0    15699 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/packaging/tags.py
+-rw-rw-rw-   0        0        0     4200 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/packaging/utils.py
+-rw-rw-rw-   0        0        0    14665 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/packaging/version.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:45.505517 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/pyparsing/
+-rw-rw-rw-   0        0        0     9159 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/pyparsing/__init__.py
+-rw-rw-rw-   0        0        0     6426 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/pyparsing/actions.py
+-rw-rw-rw-   0        0        0    12936 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/pyparsing/common.py
+-rw-rw-rw-   0        0        0   213310 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/pyparsing/core.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:45.516487 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/pyparsing/diagram/
+-rw-rw-rw-   0        0        0    23668 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/pyparsing/diagram/__init__.py
+-rw-rw-rw-   0        0        0     9023 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/pyparsing/exceptions.py
+-rw-rw-rw-   0        0        0    39129 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/pyparsing/helpers.py
+-rw-rw-rw-   0        0        0    25341 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/pyparsing/results.py
+-rw-rw-rw-   0        0        0    13402 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/pyparsing/testing.py
+-rw-rw-rw-   0        0        0    10787 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/pyparsing/unicode.py
+-rw-rw-rw-   0        0        0     6805 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/pyparsing/util.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:45.561367 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/tomli/
+-rw-rw-rw-   0        0        0      396 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/tomli/__init__.py
+-rw-rw-rw-   0        0        0    22633 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/tomli/_parser.py
+-rw-rw-rw-   0        0        0     2943 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/tomli/_re.py
+-rw-rw-rw-   0        0        0      254 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/tomli/_types.py
+-rw-rw-rw-   0        0        0    87149 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/typing_extensions.py
+-rw-rw-rw-   0        0        0     8425 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/zipp.py
+-rw-rw-rw-   0        0        0     7346 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/archive_util.py
+-rw-rw-rw-   0        0        0    19539 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/build_meta.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:45.878518 iniUts-1.0.4/venv/Lib/site-packages/setuptools/command/
+-rw-rw-rw-   0        0        0      396 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/command/__init__.py
+-rw-rw-rw-   0        0        0     2381 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/command/alias.py
+-rw-rw-rw-   0        0        0    16623 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/command/bdist_egg.py
+-rw-rw-rw-   0        0        0     1182 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/command/bdist_rpm.py
+-rw-rw-rw-   0        0        0     6595 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/command/build.py
+-rw-rw-rw-   0        0        0     4415 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/command/build_clib.py
+-rw-rw-rw-   0        0        0    15821 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/command/build_ext.py
+-rw-rw-rw-   0        0        0    14115 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/command/build_py.py
+-rw-rw-rw-   0        0        0     7012 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/command/develop.py
+-rw-rw-rw-   0        0        0     4800 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/command/dist_info.py
+-rw-rw-rw-   0        0        0    85662 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/command/easy_install.py
+-rw-rw-rw-   0        0        0    31188 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/command/editable_wheel.py
+-rw-rw-rw-   0        0        0    26795 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/command/egg_info.py
+-rw-rw-rw-   0        0        0     5163 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/command/install.py
+-rw-rw-rw-   0        0        0     2226 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/command/install_egg_info.py
+-rw-rw-rw-   0        0        0     3875 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/command/install_lib.py
+-rw-rw-rw-   0        0        0     2612 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/command/install_scripts.py
+-rw-rw-rw-   0        0        0     4946 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/command/py36compat.py
+-rw-rw-rw-   0        0        0      468 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/command/register.py
+-rw-rw-rw-   0        0        0     2128 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/command/rotate.py
+-rw-rw-rw-   0        0        0      658 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/command/saveopts.py
+-rw-rw-rw-   0        0        0     7071 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/command/sdist.py
+-rw-rw-rw-   0        0        0     5086 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/command/setopt.py
+-rw-rw-rw-   0        0        0     8102 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/command/test.py
+-rw-rw-rw-   0        0        0      462 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/command/upload.py
+-rw-rw-rw-   0        0        0     7494 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/command/upload_docs.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:45.938360 iniUts-1.0.4/venv/Lib/site-packages/setuptools/config/
+-rw-rw-rw-   0        0        0     1121 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/config/__init__.py
+-rw-rw-rw-   0        0        0    13398 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/config/_apply_pyprojecttoml.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:46.042081 iniUts-1.0.4/venv/Lib/site-packages/setuptools/config/_validate_pyproject/
+-rw-rw-rw-   0        0        0     1038 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/config/_validate_pyproject/__init__.py
+-rw-rw-rw-   0        0        0    11266 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/config/_validate_pyproject/error_reporting.py
+-rw-rw-rw-   0        0        0     1153 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/config/_validate_pyproject/extra_validations.py
+-rw-rw-rw-   0        0        0     1612 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py
+-rw-rw-rw-   0        0        0   269900 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py
+-rw-rw-rw-   0        0        0     8736 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/config/_validate_pyproject/formats.py
+-rw-rw-rw-   0        0        0    16319 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/config/expand.py
+-rw-rw-rw-   0        0        0    19304 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/config/pyprojecttoml.py
+-rw-rw-rw-   0        0        0    25198 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/config/setupcfg.py
+-rw-rw-rw-   0        0        0      949 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/dep_util.py
+-rw-rw-rw-   0        0        0     5499 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/depends.py
+-rw-rw-rw-   0        0        0    20799 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/discovery.py
+-rw-rw-rw-   0        0        0    45578 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/dist.py
+-rw-rw-rw-   0        0        0     2464 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/errors.py
+-rw-rw-rw-   0        0        0     5591 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/extension.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:46.051056 iniUts-1.0.4/venv/Lib/site-packages/setuptools/extern/
+-rw-rw-rw-   0        0        0     2512 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/extern/__init__.py
+-rw-rw-rw-   0        0        0     4873 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/glob.py
+-rw-rw-rw-   0        0        0     3824 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/installer.py
+-rw-rw-rw-   0        0        0      812 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/launch.py
+-rw-rw-rw-   0        0        0     1210 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/logging.py
+-rw-rw-rw-   0        0        0     4857 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/monkey.py
+-rw-rw-rw-   0        0        0    47724 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/msvc.py
+-rw-rw-rw-   0        0        0     3093 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/namespaces.py
+-rw-rw-rw-   0        0        0    40020 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/package_index.py
+-rw-rw-rw-   0        0        0      245 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/py34compat.py
+-rw-rw-rw-   0        0        0    14348 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/sandbox.py
+-rw-rw-rw-   0        0        0      941 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/unicode_utils.py
+-rw-rw-rw-   0        0        0      144 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/version.py
+-rw-rw-rw-   0        0        0     8376 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/wheel.py
+-rw-rw-rw-   0        0        0      718 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools/windows_support.py
+drwxrwxrwx   0        0        0        0 2023-04-28 14:48:44.300740 iniUts-1.0.4/venv/Lib/site-packages/setuptools-65.5.0.dist-info/
+-rw-rw-rw-   0        0        0     2740 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools-65.5.0.dist-info/entry_points.txt
+-rw-rw-rw-   0        0        0       41 2023-04-26 17:14:53.000000 iniUts-1.0.4/venv/Lib/site-packages/setuptools-65.5.0.dist-info/top_level.txt
```

### Comparing `iniUts-1.0.3/LICENCE.txt` & `iniUts-1.0.4/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/PKG-INFO` & `iniUts-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iniUts
-Version: 1.0.3
+Version: 1.0.4
 Summary: Ini file manipulator
 Home-page: 
 Author: Melque Lima
 Author-email: melque_ex@yahoo.com.br
 License: MIT
 Keywords: iniUts
 Classifier: Development Status :: 5 - Production/Stable
@@ -187,7 +187,11 @@
 1.0.2 (2023-04-26)
 ------------------
 - Upercase Bug Fixed
 
 1.0.3 (2023-04-26)
 ------------------
 - Upercase Write Bug Fixed
+
+1.0.4 (2023-04-28)
+------------------
+- Update Class bug fixed
```

### Comparing `iniUts-1.0.3/README.md` & `iniUts-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/iniUts/__init__.py` & `iniUts-1.0.4/iniUts/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from datetime import datetime
 import re
 
 
 class IniUts():
     def __init__(self,_file):
         self.file = _file
+        self.delimiters = {}
+        self.dateFormats = {}
 
 
     def write(self,sec,key,value):
         config = cp.RawConfigParser()
         config.optionxform = str
         config.read(self.file)
         if not sec in config.sections():
@@ -53,46 +55,57 @@
             if not k in dtClass.__annotations__:
                 if not skip_missing:
                     raise Exception(f"please create the key '{k}' in data class object")
                 else:
                     continue
             cls = dtClass.__annotations__[k]
             if cls == tuple:
-                isFormatDefined = k in [x for x in dir(dtClass) if not re.search("__.*__", x)]
-                delimiter = getattr(dtClass,k) if isFormatDefined else ','
-                v = tuple(v.split(delimiter))
+                name =  f"{str(dtClass)}_{k}"
+                if not name in self.delimiters:
+                    isFormatDefined = k in [x for x in dir(dtClass) if not re.search("__.*__", x)]
+                    delimiter = getattr(dtClass,k) if isFormatDefined else ','
+                    self.delimiters[name]=delimiter
+                    a = 2
+
+                v = tuple(v.split(self.delimiters[name]))
             if cls == datetime:
-                isFormatDefined = k in [x for x in dir(dtClass) if not re.search("__.*__", x)]
-                fmt = getattr(dtClass,k) if isFormatDefined else '%Y-%m-%d'
-                v = datetime.strptime(v,fmt)
+                name =  f"{str(dtClass)}_{k}"
+                if not name in self.dateFormats:
+                    isFormatDefined = k in [x for x in dir(dtClass) if not re.search("__.*__", x)]
+                    delimiter = getattr(dtClass,k) if isFormatDefined else '%Y-%m-%d'
+                    self.dateFormats[name]=delimiter
+                    a = 2
+
+                v = datetime.strptime(v,self.dateFormats[name])
             else:
                 v = cls(v)
 
             setattr(dtClass, k, v)
         
         MissingKeysFromClass = list(set(dtClass.__annotations__.keys())  - set(dt.keys()))
         if not skip_missing and MissingKeysFromClass:
             raise Exception(f"Cound not find '{MissingKeysFromClass}' keys at ini file")
 
 
 
-# @dataclass
-# class Person():
-#     NAME   : str
-#     age    : int
-#     amount : float
-#     friends: tuple = ','
-#     dob    : datetime = "%Y-%m-%d"
-
-
-#ini = IniUts('test.ini')
-
-# ini.section2DataClass('PERSON',Person)
-# print(Person.NAME)
+@dataclass
+class Person():
+    NAME   : str
+    age    : int
+    amount : float
+    friends: tuple = ','
+    dob    : datetime = "%Y-%m-%d"
+
+
+ini = IniUts('test.ini')
+
+ini.section2DataClass('PERSON',Person)
+ini.section2DataClass('PERSON',Person)
+print(Person.NAME)
 
-#a  =1
+a  =1
```

### Comparing `iniUts-1.0.3/iniUts.egg-info/PKG-INFO` & `iniUts-1.0.4/iniUts.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iniUts
-Version: 1.0.3
+Version: 1.0.4
 Summary: Ini file manipulator
 Home-page: 
 Author: Melque Lima
 Author-email: melque_ex@yahoo.com.br
 License: MIT
 Keywords: iniUts
 Classifier: Development Status :: 5 - Production/Stable
@@ -187,7 +187,11 @@
 1.0.2 (2023-04-26)
 ------------------
 - Upercase Bug Fixed
 
 1.0.3 (2023-04-26)
 ------------------
 - Upercase Write Bug Fixed
+
+1.0.4 (2023-04-28)
+------------------
+- Update Class bug fixed
```

### Comparing `iniUts-1.0.3/iniUts.egg-info/SOURCES.txt` & `iniUts-1.0.4/iniUts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/setup.py` & `iniUts-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='iniUts',
-  version='1.0.3',
+  version='1.0.4',
   description='Ini file manipulator',
   long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
   long_description_content_type='text/markdown',
   url='',  
   author='Melque Lima',
   author_email='melque_ex@yahoo.com.br',
   license='MIT',
```

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/_distutils_hack/__init__.py` & `iniUts-1.0.4/venv/Lib/site-packages/_distutils_hack/__init__.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/dateUts/__init__.py` & `iniUts-1.0.4/venv/Lib/site-packages/dateUts/__init__.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/dateUts-0.1.5.dist-info/LICENCE.txt` & `iniUts-1.0.4/venv/Lib/site-packages/dateUts-0.1.5.dist-info/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/__main__.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/__main__.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/__pip-runner__.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/__pip-runner__.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/__init__.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/build_env.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/build_env.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/cache.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/cache.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/cli/autocompletion.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/cli/autocompletion.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/cli/base_command.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/cli/base_command.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/cli/cmdoptions.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/cli/cmdoptions.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/cli/command_context.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/cli/command_context.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/cli/main.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/cli/main.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/cli/main_parser.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/cli/main_parser.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/cli/parser.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/cli/parser.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/cli/progress_bars.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/cli/progress_bars.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/cli/req_command.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/cli/req_command.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/cli/spinners.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/cli/spinners.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/commands/__init__.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/commands/cache.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/commands/cache.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/commands/check.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/commands/check.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/commands/completion.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/commands/completion.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/commands/configuration.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/commands/configuration.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/commands/debug.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/commands/debug.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/commands/download.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/commands/download.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/commands/freeze.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/commands/freeze.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/commands/hash.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/commands/hash.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/commands/help.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/commands/help.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/commands/index.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/commands/index.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/commands/inspect.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/commands/inspect.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/commands/install.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/commands/install.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/commands/list.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/commands/list.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/commands/search.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/commands/search.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/commands/show.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/commands/show.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/commands/uninstall.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/commands/uninstall.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/commands/wheel.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/commands/wheel.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/configuration.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/configuration.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/distributions/__init__.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/distributions/base.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/distributions/base.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/distributions/installed.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/distributions/installed.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/distributions/sdist.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/distributions/sdist.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/distributions/wheel.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/distributions/wheel.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/exceptions.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/exceptions.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/index/collector.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/index/collector.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/index/package_finder.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/index/package_finder.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/index/sources.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/index/sources.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/locations/__init__.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/locations/__init__.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/locations/_distutils.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/locations/_distutils.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/locations/_sysconfig.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/locations/_sysconfig.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/locations/base.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/locations/base.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/metadata/__init__.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/metadata/_json.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/metadata/_json.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/metadata/base.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/metadata/base.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/metadata/importlib/_compat.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/metadata/importlib/_compat.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/metadata/importlib/_dists.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/metadata/importlib/_dists.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/metadata/importlib/_envs.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/metadata/importlib/_envs.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/metadata/pkg_resources.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/metadata/pkg_resources.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/models/candidate.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/models/candidate.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/models/direct_url.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/models/direct_url.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/models/format_control.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/models/format_control.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/models/index.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/models/index.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/models/installation_report.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/models/installation_report.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/models/link.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/models/link.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/models/scheme.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/models/scheme.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/models/search_scope.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/models/search_scope.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/models/selection_prefs.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/models/selection_prefs.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/models/target_python.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/models/target_python.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/models/wheel.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/models/wheel.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/network/auth.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/network/auth.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/network/cache.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/network/cache.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/network/download.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/network/download.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/network/lazy_wheel.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/network/lazy_wheel.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/network/session.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/network/session.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/network/utils.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/network/utils.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/network/xmlrpc.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/network/xmlrpc.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/operations/build/build_tracker.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/operations/build/build_tracker.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/operations/build/metadata.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/operations/build/metadata.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/operations/build/metadata_editable.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/operations/build/metadata_editable.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/operations/build/metadata_legacy.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/operations/build/metadata_legacy.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/operations/build/wheel.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/operations/build/wheel.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/operations/build/wheel_editable.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/operations/build/wheel_editable.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/operations/build/wheel_legacy.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/operations/build/wheel_legacy.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/operations/check.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/operations/check.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/operations/freeze.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/operations/freeze.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/operations/install/editable_legacy.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/operations/install/editable_legacy.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/operations/install/wheel.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/operations/install/wheel.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/operations/prepare.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/operations/prepare.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/pyproject.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/pyproject.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/req/__init__.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/req/__init__.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/req/constructors.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/req/constructors.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/req/req_file.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/req/req_file.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/req/req_install.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/req/req_install.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/req/req_set.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/req/req_set.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/req/req_uninstall.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/req/req_uninstall.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/resolution/base.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/resolution/base.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/resolution/legacy/resolver.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/resolution/legacy/resolver.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/base.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/base.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/candidates.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/candidates.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/factory.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/factory.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/provider.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/provider.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/reporter.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/reporter.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/requirements.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/requirements.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/resolver.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/resolver.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/self_outdated_check.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/self_outdated_check.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/utils/_jaraco_text.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/utils/_jaraco_text.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/utils/_log.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/utils/_log.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/utils/appdirs.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/utils/appdirs.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/utils/compat.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/utils/compat.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/utils/compatibility_tags.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/utils/compatibility_tags.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/utils/deprecation.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/utils/direct_url_helpers.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/utils/direct_url_helpers.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/utils/egg_link.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/utils/egg_link.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/utils/encoding.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/utils/entrypoints.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/utils/entrypoints.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/utils/filesystem.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/utils/filetypes.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/utils/filetypes.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/utils/glibc.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/utils/glibc.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/utils/hashes.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/utils/hashes.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/utils/inject_securetransport.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/utils/inject_securetransport.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/utils/logging.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/utils/logging.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/utils/misc.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/utils/misc.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/utils/models.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/utils/models.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/utils/packaging.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/utils/packaging.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/utils/setuptools_build.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/utils/setuptools_build.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/utils/subprocess.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/utils/subprocess.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/utils/temp_dir.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/utils/temp_dir.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/utils/unpacking.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/utils/unpacking.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/utils/urls.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/utils/urls.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/utils/virtualenv.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/utils/virtualenv.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/utils/wheel.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/utils/wheel.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/vcs/__init__.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/vcs/__init__.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/vcs/bazaar.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/vcs/bazaar.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/vcs/git.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/vcs/git.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/vcs/mercurial.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/vcs/mercurial.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/vcs/subversion.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/vcs/subversion.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/vcs/versioncontrol.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/vcs/versioncontrol.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_internal/wheel_builder.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_internal/wheel_builder.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/__init__.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/__init__.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/cachecontrol/_cmd.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/cachecontrol/_cmd.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/cachecontrol/adapter.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/cachecontrol/adapter.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/cachecontrol/cache.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/cachecontrol/cache.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/cachecontrol/compat.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/cachecontrol/compat.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/cachecontrol/controller.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/cachecontrol/controller.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/cachecontrol/filewrapper.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/cachecontrol/filewrapper.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/cachecontrol/heuristics.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/cachecontrol/heuristics.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/cachecontrol/serialize.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/cachecontrol/serialize.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/cachecontrol/wrapper.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/cachecontrol/wrapper.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/certifi/core.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/certifi/core.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/__init__.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/__init__.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/big5freq.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/big5freq.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/big5prober.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/big5prober.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/chardistribution.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/chardistribution.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/charsetgroupprober.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/charsetgroupprober.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/charsetprober.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/charsetprober.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/cli/chardetect.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/cli/chardetect.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachine.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachine.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachinedict.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachinedict.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/cp949prober.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/cp949prober.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/enums.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/enums.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/escprober.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/escprober.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/escsm.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/escsm.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/eucjpprober.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/eucjpprober.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/euckrfreq.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/euckrfreq.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/euckrprober.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/euckrprober.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/euctwfreq.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/euctwfreq.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/euctwprober.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/euctwprober.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/gb2312freq.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/gb2312freq.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/gb2312prober.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/gb2312prober.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/hebrewprober.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/hebrewprober.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/jisfreq.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/jisfreq.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/johabfreq.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/johabfreq.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/johabprober.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/johabprober.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/jpcntx.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/jpcntx.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/langbulgarianmodel.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/langbulgarianmodel.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/langgreekmodel.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/langgreekmodel.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/langhebrewmodel.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/langhebrewmodel.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/langhungarianmodel.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/langhungarianmodel.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/langrussianmodel.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/langrussianmodel.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/langthaimodel.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/langthaimodel.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/langturkishmodel.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/langturkishmodel.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/latin1prober.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/latin1prober.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/macromanprober.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/macromanprober.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/mbcharsetprober.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/mbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/mbcsgroupprober.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/mbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/mbcssm.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/mbcssm.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/metadata/languages.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/metadata/languages.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/sbcharsetprober.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/sbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/sbcsgroupprober.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/sbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/sjisprober.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/sjisprober.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/universaldetector.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/universaldetector.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/utf1632prober.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/utf1632prober.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/chardet/utf8prober.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/chardet/utf8prober.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/colorama/ansi.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/colorama/ansitowin32.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/colorama/initialise.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/colorama/tests/ansi_test.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/colorama/tests/ansi_test.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/colorama/tests/initialise_test.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/colorama/tests/initialise_test.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/colorama/tests/isatty_test.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/colorama/tests/isatty_test.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/colorama/tests/utils.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/colorama/tests/utils.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/colorama/tests/winterm_test.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/colorama/tests/winterm_test.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/colorama/win32.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/colorama/winterm.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/distlib/__init__.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/distlib/__init__.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/distlib/compat.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/distlib/compat.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/distlib/database.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/distlib/database.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/distlib/index.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/distlib/index.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/distlib/locators.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/distlib/locators.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/distlib/manifest.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/distlib/manifest.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/distlib/markers.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/distlib/markers.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/distlib/metadata.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/distlib/metadata.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/distlib/resources.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/distlib/resources.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/distlib/scripts.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/distlib/scripts.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/distlib/util.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/distlib/util.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/distlib/version.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/distlib/version.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/distlib/wheel.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/distlib/wheel.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/distro/__init__.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/distro/__init__.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/distro/distro.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/distro/distro.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/idna/__init__.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/idna/__init__.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/idna/codec.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/idna/codec.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/idna/core.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/idna/core.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/idna/idnadata.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/idna/idnadata.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/idna/intranges.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/idna/intranges.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/idna/uts46data.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/idna/uts46data.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/msgpack/__init__.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/msgpack/__init__.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/msgpack/exceptions.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/msgpack/exceptions.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/msgpack/ext.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/msgpack/ext.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/msgpack/fallback.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/msgpack/fallback.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/packaging/__about__.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/packaging/_manylinux.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/packaging/_musllinux.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/packaging/_structures.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/packaging/markers.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/packaging/requirements.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/packaging/specifiers.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/packaging/tags.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/packaging/utils.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/packaging/version.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pkg_resources/__init__.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/platformdirs/__init__.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/platformdirs/__init__.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/platformdirs/__main__.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/platformdirs/__main__.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/platformdirs/android.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/platformdirs/android.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/platformdirs/api.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/platformdirs/api.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/platformdirs/macos.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/platformdirs/macos.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/platformdirs/unix.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/platformdirs/unix.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/platformdirs/windows.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/platformdirs/windows.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/__init__.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/__init__.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/cmdline.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/cmdline.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/console.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/console.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/filter.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/filter.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/filters/__init__.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/formatter.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/formatter.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/formatters/__init__.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/formatters/__init__.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/formatters/_mapping.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/formatters/_mapping.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/formatters/bbcode.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/formatters/bbcode.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/formatters/groff.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/formatters/groff.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/formatters/html.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/formatters/html.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/formatters/img.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/formatters/img.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/formatters/irc.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/formatters/irc.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/formatters/latex.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/formatters/latex.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/formatters/other.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/formatters/other.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/formatters/rtf.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/formatters/rtf.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/formatters/svg.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/formatters/svg.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal256.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal256.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/lexer.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/lexer.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/lexers/__init__.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/lexers/__init__.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/lexers/_mapping.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/lexers/_mapping.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/lexers/python.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/lexers/python.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/modeline.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/modeline.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/plugin.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/plugin.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/regexopt.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/regexopt.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/scanner.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/scanner.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/sphinxext.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/sphinxext.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/style.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/style.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/styles/__init__.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/token.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/token.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/unistring.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/unistring.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pygments/util.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pygments/util.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pyparsing/__init__.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pyparsing/__init__.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pyparsing/actions.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pyparsing/actions.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pyparsing/common.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pyparsing/common.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pyparsing/core.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pyparsing/core.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pyparsing/diagram/__init__.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pyparsing/diagram/__init__.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pyparsing/exceptions.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pyparsing/exceptions.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pyparsing/helpers.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pyparsing/helpers.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pyparsing/results.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pyparsing/results.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pyparsing/testing.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pyparsing/testing.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pyparsing/unicode.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pyparsing/unicode.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pyparsing/util.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pyparsing/util.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_impl.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_impl.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/requests/__init__.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/requests/_internal_utils.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/requests/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/requests/adapters.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/requests/adapters.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/requests/api.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/requests/api.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/requests/auth.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/requests/auth.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/requests/certs.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/requests/certs.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/requests/compat.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/requests/compat.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/requests/cookies.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/requests/cookies.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/requests/exceptions.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/requests/help.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/requests/help.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/requests/hooks.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/requests/hooks.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/requests/models.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/requests/models.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/requests/packages.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/requests/packages.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/requests/sessions.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/requests/status_codes.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/requests/status_codes.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/requests/structures.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/requests/structures.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/requests/utils.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/requests/utils.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/resolvelib/__init__.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/resolvelib/__init__.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/resolvelib/providers.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/resolvelib/providers.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/resolvelib/reporters.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/resolvelib/reporters.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/resolvelib/resolvers.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/resolvelib/resolvers.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/resolvelib/structs.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/resolvelib/structs.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/__init__.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/__init__.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/__main__.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/__main__.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/_cell_widths.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/_cell_widths.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/_emoji_codes.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/_emoji_codes.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/_emoji_replace.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/_emoji_replace.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/_export_format.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/_export_format.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/_fileno.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/_fileno.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/_inspect.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/_inspect.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/_log_render.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/_log_render.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/_loop.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/_loop.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/_null_file.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/_null_file.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/_palettes.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/_palettes.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/_ratio.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/_ratio.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/_spinners.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/_spinners.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/_win32_console.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/_win32_console.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/_windows.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/_windows.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/_windows_renderer.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/_windows_renderer.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/_wrap.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/_wrap.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/abc.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/abc.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/align.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/align.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/ansi.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/ansi.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/bar.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/bar.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/box.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/box.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/cells.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/cells.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/color.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/color.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/color_triplet.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/color_triplet.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/columns.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/columns.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/console.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/console.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/constrain.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/constrain.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/containers.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/containers.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/control.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/control.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/default_styles.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/default_styles.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/diagnose.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/diagnose.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/emoji.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/emoji.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/errors.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/errors.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/file_proxy.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/file_proxy.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/filesize.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/filesize.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/highlighter.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/highlighter.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/json.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/json.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/jupyter.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/jupyter.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/layout.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/layout.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/live.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/live.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/live_render.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/live_render.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/logging.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/logging.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/markup.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/markup.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/measure.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/measure.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/padding.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/padding.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/pager.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/pager.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/palette.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/palette.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/panel.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/panel.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/pretty.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/pretty.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/progress.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/progress.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/progress_bar.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/progress_bar.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/prompt.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/prompt.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/protocol.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/protocol.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/repr.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/repr.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/rule.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/rule.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/scope.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/scope.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/screen.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/screen.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/segment.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/segment.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/spinner.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/spinner.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/status.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/status.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/style.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/style.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/styled.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/styled.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/syntax.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/syntax.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/table.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/table.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/terminal_theme.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/terminal_theme.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/text.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/text.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/theme.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/theme.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/traceback.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/traceback.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/rich/tree.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/rich/tree.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/six.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/six.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/tenacity/__init__.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/tenacity/__init__.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/tenacity/_asyncio.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/tenacity/_asyncio.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/tenacity/_utils.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/tenacity/_utils.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/tenacity/after.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/tenacity/after.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/tenacity/before.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/tenacity/before.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/tenacity/before_sleep.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/tenacity/before_sleep.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/tenacity/nap.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/tenacity/nap.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/tenacity/retry.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/tenacity/retry.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/tenacity/stop.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/tenacity/stop.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/tenacity/tornadoweb.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/tenacity/tornadoweb.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/tenacity/wait.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/tenacity/wait.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/tomli/_parser.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/tomli/_re.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/typing_extensions.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/__init__.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/_collections.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/connection.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/connectionpool.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/appengine.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/appengine.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/securetransport.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/securetransport.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/socks.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/exceptions.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/fields.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/filepost.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/packages/six.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/packages/six.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/poolmanager.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/request.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/request.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/response.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/util/__init__.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/util/connection.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/util/proxy.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/util/request.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/util/response.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/util/retry.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssltransport.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/util/timeout.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/util/url.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/urllib3/util/wait.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/webencodings/__init__.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/webencodings/__init__.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/webencodings/labels.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/webencodings/labels.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/webencodings/mklabels.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/webencodings/mklabels.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/webencodings/tests.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/webencodings/tests.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip/_vendor/webencodings/x_user_defined.py` & `iniUts-1.0.4/venv/Lib/site-packages/pip/_vendor/webencodings/x_user_defined.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip-23.1.2.dist-info/AUTHORS.txt` & `iniUts-1.0.4/venv/Lib/site-packages/pip-23.1.2.dist-info/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pip-23.1.2.dist-info/LICENSE.txt` & `iniUts-1.0.4/venv/Lib/site-packages/pip-23.1.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/__init__.py` & `iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/appdirs.py` & `iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/appdirs.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py` & `iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_common.py` & `iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_common.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py` & `iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py` & `iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py` & `iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/abc.py` & `iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/abc.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/readers.py` & `iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/readers.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/simple.py` & `iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/simple.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/context.py` & `iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/context.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/functools.py` & `iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/functools.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py` & `iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/more.py` & `iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/more.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/recipes.py` & `iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/recipes.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/packaging/__about__.py` & `iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_manylinux.py` & `iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_musllinux.py` & `iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_structures.py` & `iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/packaging/markers.py` & `iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/packaging/requirements.py` & `iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/packaging/specifiers.py` & `iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/packaging/tags.py` & `iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/packaging/utils.py` & `iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/packaging/version.py` & `iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/__init__.py` & `iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/__init__.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/actions.py` & `iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/actions.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/common.py` & `iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/common.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/core.py` & `iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/core.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/diagram/__init__.py` & `iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/diagram/__init__.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/exceptions.py` & `iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/exceptions.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/helpers.py` & `iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/helpers.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/results.py` & `iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/results.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/testing.py` & `iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/testing.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/unicode.py` & `iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/unicode.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/util.py` & `iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/util.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/_vendor/zipp.py` & `iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/_vendor/zipp.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/pkg_resources/extern/__init__.py` & `iniUts-1.0.4/venv/Lib/site-packages/pkg_resources/extern/__init__.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/__init__.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/__init__.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/__init__.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/__init__.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/_collections.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/_collections.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/_msvccompiler.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/_msvccompiler.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/archive_util.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/archive_util.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/bcppcompiler.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/bcppcompiler.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/ccompiler.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/ccompiler.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/cmd.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/cmd.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/_framework_compat.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/command/_framework_compat.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/bdist.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/command/bdist.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/bdist_dumb.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/command/bdist_dumb.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/bdist_rpm.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/command/bdist_rpm.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/build.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/command/build.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/build_clib.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/command/build_clib.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/build_ext.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/command/build_ext.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/build_py.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/command/build_py.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/build_scripts.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/command/build_scripts.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/check.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/command/check.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/clean.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/command/clean.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/config.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/command/config.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/install.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/command/install.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/install_data.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/command/install_data.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/install_egg_info.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/command/install_egg_info.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/install_headers.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/command/install_headers.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/install_lib.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/command/install_lib.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/install_scripts.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/command/install_scripts.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/py37compat.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/command/py37compat.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/register.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/command/register.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/sdist.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/command/sdist.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/command/upload.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/command/upload.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/config.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/config.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/core.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/core.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/cygwinccompiler.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/cygwinccompiler.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/dep_util.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/dep_util.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/dir_util.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/dir_util.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/dist.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/dist.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/errors.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/errors.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/extension.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/extension.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/fancy_getopt.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/fancy_getopt.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/file_util.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/file_util.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/filelist.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/filelist.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/log.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/log.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/msvc9compiler.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/msvc9compiler.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/msvccompiler.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/msvccompiler.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/py39compat.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/py39compat.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/spawn.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/spawn.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/sysconfig.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/sysconfig.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/text_file.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/text_file.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/unixccompiler.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/unixccompiler.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/util.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/util.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/version.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/version.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_distutils/versionpredicate.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_distutils/versionpredicate.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_entry_points.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_entry_points.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_imp.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_imp.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_importlib.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_importlib.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_itertools.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_itertools.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_path.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_path.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/__init__.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_collections.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_collections.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_compat.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_compat.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_functools.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_functools.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_meta.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_meta.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_text.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_text.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_adapters.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_adapters.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_common.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_common.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_compat.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_compat.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_itertools.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_itertools.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_legacy.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_legacy.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/abc.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/abc.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/readers.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/readers.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/simple.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/simple.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/jaraco/context.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/jaraco/context.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/jaraco/functools.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/jaraco/functools.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/jaraco/text/__init__.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/jaraco/text/__init__.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/more_itertools/more.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/more_itertools/more.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/more_itertools/recipes.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/more_itertools/recipes.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/ordered_set.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/ordered_set.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/packaging/__about__.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/packaging/_manylinux.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/packaging/_musllinux.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/packaging/_structures.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/packaging/markers.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/packaging/requirements.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/packaging/specifiers.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/packaging/tags.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/packaging/utils.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/packaging/version.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/pyparsing/__init__.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/pyparsing/__init__.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/pyparsing/actions.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/pyparsing/actions.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/pyparsing/common.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/pyparsing/common.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/pyparsing/core.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/pyparsing/core.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/pyparsing/diagram/__init__.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/pyparsing/diagram/__init__.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/pyparsing/exceptions.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/pyparsing/exceptions.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/pyparsing/helpers.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/pyparsing/helpers.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/pyparsing/results.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/pyparsing/results.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/pyparsing/testing.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/pyparsing/testing.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/pyparsing/unicode.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/pyparsing/unicode.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/pyparsing/util.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/pyparsing/util.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/tomli/_parser.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/tomli/_re.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/typing_extensions.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/_vendor/zipp.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/_vendor/zipp.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/archive_util.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/archive_util.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/build_meta.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/build_meta.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/command/alias.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/command/alias.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/command/bdist_egg.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/command/bdist_egg.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/command/bdist_rpm.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/command/bdist_rpm.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/command/build.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/command/build.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/command/build_clib.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/command/build_clib.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/command/build_ext.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/command/build_ext.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/command/build_py.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/command/build_py.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/command/develop.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/command/develop.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/command/dist_info.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/command/dist_info.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/command/easy_install.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/command/easy_install.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/command/editable_wheel.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/command/editable_wheel.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/command/egg_info.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/command/egg_info.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/command/install.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/command/install.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/command/install_egg_info.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/command/install_egg_info.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/command/install_lib.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/command/install_lib.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/command/install_scripts.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/command/install_scripts.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/command/py36compat.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/command/py36compat.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/command/rotate.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/command/rotate.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/command/saveopts.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/command/saveopts.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/command/sdist.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/command/sdist.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/command/setopt.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/command/setopt.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/command/test.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/command/test.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/command/upload_docs.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/command/upload_docs.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/config/__init__.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/config/__init__.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/config/_apply_pyprojecttoml.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/config/_apply_pyprojecttoml.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/config/_validate_pyproject/__init__.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/config/_validate_pyproject/__init__.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/config/_validate_pyproject/error_reporting.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/config/_validate_pyproject/error_reporting.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/config/_validate_pyproject/extra_validations.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/config/_validate_pyproject/extra_validations.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/config/_validate_pyproject/formats.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/config/_validate_pyproject/formats.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/config/expand.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/config/expand.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/config/pyprojecttoml.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/config/pyprojecttoml.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/config/setupcfg.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/config/setupcfg.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/dep_util.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/dep_util.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/depends.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/depends.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/discovery.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/discovery.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/dist.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/dist.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/errors.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/errors.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/extension.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/extension.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/extern/__init__.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/extern/__init__.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/glob.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/glob.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/installer.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/installer.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/launch.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/launch.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/logging.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/logging.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/monkey.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/monkey.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/msvc.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/msvc.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/namespaces.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/namespaces.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/package_index.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/package_index.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/sandbox.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/sandbox.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/unicode_utils.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/unicode_utils.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/wheel.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/wheel.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools/windows_support.py` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools/windows_support.py`

 * *Files identical despite different names*

### Comparing `iniUts-1.0.3/venv/Lib/site-packages/setuptools-65.5.0.dist-info/entry_points.txt` & `iniUts-1.0.4/venv/Lib/site-packages/setuptools-65.5.0.dist-info/entry_points.txt`

 * *Files identical despite different names*

