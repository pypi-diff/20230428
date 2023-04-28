# Comparing `tmp/elasticsearch_curator-8.0.3.tar.gz` & `tmp/elasticsearch_curator-8.0.4.tar.gz`

## Comparing `elasticsearch_curator-8.0.3.tar` & `elasticsearch_curator-8.0.4.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/curator/__init__.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/curator/_version.py
--rw-r--r--   0        0        0     9608 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/curator/classdef.py
--rw-r--r--   0        0        0    14845 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/curator/cli.py
--rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/curator/config_utils.py
--rwxr-xr-x   0        0        0      285 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/curator/curator_cli.py
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/curator/exceptions.py
--rw-r--r--   0        0        0    56567 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/curator/indexlist.py
--rw-r--r--   0        0        0     5110 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/curator/logtools.py
--rw-r--r--   0        0        0    23556 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/curator/repomgrcli.py
--rw-r--r--   0        0        0     6841 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/curator/singletons.py
--rw-r--r--   0        0        0    22898 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/curator/snapshotlist.py
--rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/curator/actions/__init__.py
--rw-r--r--   0        0        0     6905 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/curator/actions/alias.py
--rw-r--r--   0        0        0     4401 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/curator/actions/allocation.py
--rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/curator/actions/close.py
--rw-r--r--   0        0        0     4374 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/curator/actions/cluster_routing.py
--rw-r--r--   0        0        0    12778 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/curator/actions/cold2frozen.py
--rw-r--r--   0        0        0     4096 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/curator/actions/create_index.py
--rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/curator/actions/delete_indices.py
--rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/curator/actions/forcemerge.py
--rw-r--r--   0        0        0     5603 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/curator/actions/index_settings.py
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/curator/actions/open.py
--rw-r--r--   0        0        0    17631 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/curator/actions/reindex.py
--rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/curator/actions/replicas.py
--rw-r--r--   0        0        0     5228 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/curator/actions/rollover.py
--rw-r--r--   0        0        0    24570 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/curator/actions/shrink.py
--rw-r--r--   0        0        0    21632 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/curator/actions/snapshot.py
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/curator/cli_singletons/__init__.py
--rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/curator/cli_singletons/alias.py
--rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/curator/cli_singletons/allocation.py
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/curator/cli_singletons/close.py
--rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/curator/cli_singletons/delete.py
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/curator/cli_singletons/forcemerge.py
--rw-r--r--   0        0        0     9687 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/curator/cli_singletons/object_class.py
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/curator/cli_singletons/open_indices.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/curator/cli_singletons/replicas.py
--rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/curator/cli_singletons/restore.py
--rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/curator/cli_singletons/rollover.py
--rw-r--r--   0        0        0     4377 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/curator/cli_singletons/show.py
--rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/curator/cli_singletons/shrink.py
--rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/curator/cli_singletons/snapshot.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/curator/cli_singletons/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/curator/defaults/__init__.py
--rw-r--r--   0        0        0    11383 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/curator/defaults/filter_elements.py
--rw-r--r--   0        0        0     8082 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/curator/defaults/filtertypes.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/curator/defaults/logging_defaults.py
--rw-r--r--   0        0        0    18383 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/curator/defaults/option_defaults.py
--rw-r--r--   0        0        0     6479 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/curator/defaults/settings.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/curator/helpers/__init__.py
--rw-r--r--   0        0        0    23308 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/curator/helpers/date_ops.py
--rw-r--r--   0        0        0    10761 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/curator/helpers/getters.py
--rw-r--r--   0        0        0    14093 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/curator/helpers/testers.py
--rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/curator/helpers/utils.py
--rw-r--r--   0        0        0    12704 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/curator/helpers/waiters.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/curator/validators/__init__.py
--rw-r--r--   0        0        0     2873 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/curator/validators/actions.py
--rw-r--r--   0        0        0     3178 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/curator/validators/filter_functions.py
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/curator/validators/logconfig.py
--rw-r--r--   0        0        0     6494 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/curator/validators/options.py
--rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/curator/validators/schemacheck.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/.gitignore
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/LICENSE
--rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/NOTICE
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/README.rst
--rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/pyproject.toml
--rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.3/PKG-INFO
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/__init__.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/_version.py
+-rw-r--r--   0        0        0     9608 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/classdef.py
+-rw-r--r--   0        0        0    15002 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/cli.py
+-rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/config_utils.py
+-rwxr-xr-x   0        0        0      285 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/curator_cli.py
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/exceptions.py
+-rw-r--r--   0        0        0    56567 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/indexlist.py
+-rw-r--r--   0        0        0     5110 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/logtools.py
+-rw-r--r--   0        0        0    23556 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/repomgrcli.py
+-rw-r--r--   0        0        0     6998 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/singletons.py
+-rw-r--r--   0        0        0    22898 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/snapshotlist.py
+-rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/actions/__init__.py
+-rw-r--r--   0        0        0     6905 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/actions/alias.py
+-rw-r--r--   0        0        0     4401 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/actions/allocation.py
+-rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/actions/close.py
+-rw-r--r--   0        0        0     4374 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/actions/cluster_routing.py
+-rw-r--r--   0        0        0     8770 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/actions/cold2frozen.py
+-rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/actions/create_index.py
+-rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/actions/delete_indices.py
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/actions/forcemerge.py
+-rw-r--r--   0        0        0     5603 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/actions/index_settings.py
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/actions/open.py
+-rw-r--r--   0        0        0    17631 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/actions/reindex.py
+-rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/actions/replicas.py
+-rw-r--r--   0        0        0     5228 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/actions/rollover.py
+-rw-r--r--   0        0        0    24570 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/actions/shrink.py
+-rw-r--r--   0        0        0    21632 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/actions/snapshot.py
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/cli_singletons/__init__.py
+-rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/cli_singletons/alias.py
+-rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/cli_singletons/allocation.py
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/cli_singletons/close.py
+-rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/cli_singletons/delete.py
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/cli_singletons/forcemerge.py
+-rw-r--r--   0        0        0     9687 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/cli_singletons/object_class.py
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/cli_singletons/open_indices.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/cli_singletons/replicas.py
+-rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/cli_singletons/restore.py
+-rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/cli_singletons/rollover.py
+-rw-r--r--   0        0        0     4377 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/cli_singletons/show.py
+-rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/cli_singletons/shrink.py
+-rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/cli_singletons/snapshot.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/cli_singletons/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/defaults/__init__.py
+-rw-r--r--   0        0        0    11383 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/defaults/filter_elements.py
+-rw-r--r--   0        0        0     8082 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/defaults/filtertypes.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/defaults/logging_defaults.py
+-rw-r--r--   0        0        0    18383 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/defaults/option_defaults.py
+-rw-r--r--   0        0        0     6479 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/defaults/settings.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/helpers/__init__.py
+-rw-r--r--   0        0        0    23308 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/helpers/date_ops.py
+-rw-r--r--   0        0        0    13903 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/helpers/getters.py
+-rw-r--r--   0        0        0    15381 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/helpers/testers.py
+-rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/helpers/utils.py
+-rw-r--r--   0        0        0    12704 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/helpers/waiters.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/validators/__init__.py
+-rw-r--r--   0        0        0     2873 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/validators/actions.py
+-rw-r--r--   0        0        0     3178 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/validators/filter_functions.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/validators/logconfig.py
+-rw-r--r--   0        0        0     6494 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/validators/options.py
+-rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/curator/validators/schemacheck.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/.gitignore
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/LICENSE
+-rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/NOTICE
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/README.rst
+-rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 elasticsearch_curator-8.0.4/PKG-INFO
```

### Comparing `elasticsearch_curator-8.0.3/curator/classdef.py` & `elasticsearch_curator-8.0.4/curator/classdef.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.3/curator/cli.py` & `elasticsearch_curator-8.0.4/curator/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -237,14 +237,15 @@
     logger.info('All actions completed.')
 
 # pylint: disable=unused-argument, redefined-builtin
 @click.command(context_settings=get_width())
 @click.option('--config', help='Path to configuration file.', type=click.Path(exists=True), default=settings.config_file())
 @click.option('--hosts', help='Elasticsearch URL to connect to', multiple=True)
 @click.option('--cloud_id', help='Shorthand to connect to Elastic Cloud instance')
+@click.option('--api_token', help='The base64 encoded API Key token', type=str)
 @click.option('--id', help='API Key "id" value', type=str)
 @click.option('--api_key', help='API Key "api_key" value', type=str)
 @click.option('--username', help='Username used to create "basic_auth" tuple')
 @click.option('--password', help='Password used to create "basic_auth" tuple')
 @click.option('--bearer_auth', type=str)
 @click.option('--opaque_id', type=str)
 @click.option('--request_timeout', help='Request timeout in seconds', type=float)
@@ -262,15 +263,15 @@
 @click.option('--loglevel', help='Log level', type=click.Choice(['DEBUG', 'INFO', 'WARNING', 'ERROR', 'CRITICAL']))
 @click.option('--logfile', help='log file')
 @click.option('--logformat', help='Log output format', type=click.Choice(['default', 'logstash', 'json', 'ecs']))
 @click.argument('action_file', type=click.Path(exists=True), nargs=1)
 @click.version_option(version=__version__)
 @click.pass_context
 def cli(
-    ctx, config, hosts, cloud_id, id, api_key, username, password, bearer_auth,
+    ctx, config, hosts, cloud_id, api_token, id, api_key, username, password, bearer_auth,
     opaque_id, request_timeout, http_compress, verify_certs, ca_certs, client_cert, client_key,
     ssl_assert_hostname, ssl_assert_fingerprint, ssl_version, master_only, skip_version_test,
     dry_run, loglevel, logfile, logformat, action_file
 ):
     """
     Curator for Elasticsearch indices.
 
@@ -308,19 +309,20 @@
     cli_other = prune_nones({
         'master_only': master_only,
         'skip_version_test': skip_version_test,
         'username': username,
         'password': password,
         'api_key': {
             'id': id,
-            'api_key': api_key
+            'api_key': api_key,
+            'token': api_token,
         }
     })
-    # Remove `api_key` root key if `id` and `api_key` are both None
-    if id is None and api_key is None:
+    # Remove `api_key` root key if `id` and `api_key` and `token` are all None
+    if id is None and api_key is None and api_token is None:
         del cli_other['api_key']
 
     # If hosts are in the config file, but cloud_id is specified at the command-line,
     # we need to remove the hosts parameter as cloud_id and hosts are mutually exclusive
     if cloud_id:
         click.echo('cloud_id provided at CLI, superseding any other configured hosts')
         client_args.hosts = None
```

### Comparing `elasticsearch_curator-8.0.3/curator/config_utils.py` & `elasticsearch_curator-8.0.4/curator/config_utils.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.3/curator/exceptions.py` & `elasticsearch_curator-8.0.4/curator/exceptions.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.3/curator/indexlist.py` & `elasticsearch_curator-8.0.4/curator/indexlist.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.3/curator/logtools.py` & `elasticsearch_curator-8.0.4/curator/logtools.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.3/curator/repomgrcli.py` & `elasticsearch_curator-8.0.4/curator/repomgrcli.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.3/curator/singletons.py` & `elasticsearch_curator-8.0.4/curator/singletons.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from curator.cli_singletons.utils import get_width
 
 # pylint: disable=unused-argument, redefined-builtin
 @click.group(context_settings=get_width())
 @click.option('--config', help='Path to configuration file.', type=click.Path(exists=True), default=settings.config_file())
 @click.option('--hosts', help='Elasticsearch URL to connect to', multiple=True)
 @click.option('--cloud_id', help='Shorthand to connect to Elastic Cloud instance')
+@click.option('--api_token', help='The base64 encoded API Key token', type=str)
 @click.option('--id', help='API Key "id" value', type=str)
 @click.option('--api_key', help='API Key "api_key" value', type=str)
 @click.option('--username', help='Username used to create "basic_auth" tuple')
 @click.option('--password', help='Password used to create "basic_auth" tuple')
 @click.option('--bearer_auth', type=str)
 @click.option('--opaque_id', type=str)
 @click.option('--request_timeout', help='Request timeout in seconds', type=float)
@@ -37,15 +38,15 @@
 @click.option('--dry-run', is_flag=True, help='Do not perform any changes.')
 @click.option('--loglevel', help='Log level', type=click.Choice(['DEBUG', 'INFO', 'WARNING', 'ERROR', 'CRITICAL']))
 @click.option('--logfile', help='log file')
 @click.option('--logformat', help='Log output format', type=click.Choice(['default', 'logstash', 'json', 'ecs']))
 @click.version_option(version=__version__)
 @click.pass_context
 def cli(
-    ctx, config, hosts, cloud_id, id, api_key, username, password, bearer_auth,
+    ctx, config, hosts, cloud_id, api_token, id, api_key, username, password, bearer_auth,
     opaque_id, request_timeout, http_compress, verify_certs, ca_certs, client_cert, client_key,
     ssl_assert_hostname, ssl_assert_fingerprint, ssl_version, master_only, skip_version_test,
     dry_run, loglevel, logfile, logformat
 ):
     """CLI input"""
     client_args = ClientArgs()
     other_args = OtherArgs()
@@ -95,19 +96,20 @@
     cli_other = prune_nones({
         'master_only': master_only,
         'skip_version_test': skip_version_test,
         'username': username,
         'password': password,
         'api_key': {
             'id': id,
-            'api_key': api_key
+            'api_key': api_key,
+            'token': api_token,
         }
     })
-    # Remove `api_key` root key if `id` and `api_key` are both None
-    if id is None and api_key is None:
+    # Remove `api_key` root key if `id` and `api_key` and `token` are all None
+    if id is None and api_key is None and api_token is None:
         del cli_other['api_key']
 
     # If hosts are in the config file, but cloud_id is specified at the command-line,
     # we need to remove the hosts parameter as cloud_id and hosts are mutually exclusive
     if cloud_id:
         click.echo('cloud_id provided at CLI, superseding any other configured hosts')
         client_args.hosts = None
```

### Comparing `elasticsearch_curator-8.0.3/curator/snapshotlist.py` & `elasticsearch_curator-8.0.4/curator/snapshotlist.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.3/curator/actions/__init__.py` & `elasticsearch_curator-8.0.4/curator/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.3/curator/actions/alias.py` & `elasticsearch_curator-8.0.4/curator/actions/alias.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.3/curator/actions/allocation.py` & `elasticsearch_curator-8.0.4/curator/actions/allocation.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.3/curator/actions/close.py` & `elasticsearch_curator-8.0.4/curator/actions/close.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.3/curator/actions/cluster_routing.py` & `elasticsearch_curator-8.0.4/curator/actions/cluster_routing.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.3/curator/actions/cold2frozen.py` & `elasticsearch_curator-8.0.4/curator/actions/cold2frozen.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Snapshot and Restore action classes"""
 import logging
-import re
-from curator.helpers.getters import get_data_tiers
-from curator.helpers.testers import verify_index_list
+from curator.helpers.getters import get_alias_actions, get_frozen_prefix, get_tier_preference
+from curator.helpers.testers import has_lifecycle_name, is_idx_partial, verify_index_list
 from curator.helpers.utils import report_failure
 from curator.exceptions import CuratorException, FailedExecution, SearchableSnapshotException
 
 class Cold2Frozen:
     """Cold to Frozen Tier Searchable Snapshot Action Class
 
     For manually migrating snapshots not associated with ILM from the cold tier to the frozen tier.
@@ -65,146 +64,45 @@
         # It ignores any non-relevant kwargs
         for key, value in self.DEFAULTS.items():
             if key in kwargs:
                 setattr(self, key, kwargs[key])
             else:
                 setattr(self, key, value)
 
-    def get_alias_actions(self, oldidx, newidx, aliases):
-        """
-        :param oldidx: The old index name
-        :param newidx: The new index name
-        :param aliases: The aliases
-
-        :type oldidx: str
-        :type newidx: str
-        :type aliases: dict
-
-        :returns: A list of actions suitable for
-            :py:meth:`~.elasticsearch.client.IndicesClient.update_aliases` ``actions`` kwarg.
-        :rtype: list
-        """
-        actions = []
-        for alias in aliases.keys():
-            actions.append({'remove': {'index': oldidx, 'alias': alias}})
-            actions.append({'add': {'index': newidx, 'alias': alias}})
-        return actions
-
-    def get_frozen_prefix(self, oldidx, curridx):
-        """
-        Use regular expression magic to extract the prefix from the current index, and then use
-        that with ``partial-`` in front to name the resulting index.
-
-        If there is no prefix, then we just send back ``partial-``
-
-        :param oldidx: The index name before it was mounted in cold tier
-        :param curridx: The current name of the index, as mounted in cold tier
-
-        :type oldidx: str
-        :type curridx: str
-
-        :returns: The prefix to prepend the index name with for mounting as frozen
-        :rtype: str
-        """
-        pattern = f'^(.*){oldidx}$'
-        regexp = re.compile(pattern)
-        match = regexp.match(curridx)
-        prefix = match.group(1)
-        self.loggit.debug('Detected match group for prefix: %s', prefix)
-        if not prefix:
-            return 'partial-'
-        return f'partial-{prefix}'
-
-    def get_tier_preference(self):
-        """Do the tier preference thing in reverse order from coldest to hottest
-
-        :returns: A suitable tier preference string in csv format
-        :rtype: str
-        """
-        tiers = get_data_tiers(self.client)
-        # We're migrating from cold to frozen here. If a frozen tier exists, frozen ss mounts
-        # should only ever go to the frozen tier.
-        if 'data_frozen' in tiers and tiers['data_frozen']:
-            return 'data_frozen'
-        # If there are no  nodes with the 'data_frozen' role...
-        preflist = []
-        for key in ['data_cold', 'data_warm', 'data_hot']:
-            # This ordering ensures that colder tiers are prioritized
-            if key in tiers and tiers[key]:
-                preflist.append(key)
-        # If all of these are false, then we have no data tiers and must use 'data_content'
-        if not preflist:
-            return 'data_content'
-        # This will join from coldest to hottest as csv string, e.g. 'data_cold,data_warm,data_hot'
-        return ','.join(preflist)
-
-    def has_lifecycle_name(self, idx_settings):
-        """
-        :param idx_settings: The settings for an index being tested
-        :type idx_settings: dict
-
-        :returns: ``True`` if a lifecycle name exists in settings, else ``False``
-        :rtype: bool
-        """
-        if 'lifecycle' in idx_settings:
-            if 'name' in idx_settings['lifecycle']:
-                return True
-        return False
-
-    def is_idx_partial(self, idx_settings):
-        """
-        :param idx_settings: The settings for an index being tested
-        :type idx_settings: dict
-
-        :returns: ``True`` if store.snapshot.partial exists in settings, else ``False``
-        :rtype: bool
-        """
-        if 'store' in idx_settings:
-            if 'snapshot' in idx_settings['store']:
-                if 'partial' in idx_settings['store']['snapshot']:
-                    if idx_settings['store']['snapshot']['partial']:
-                        return True
-                    # store.snapshot.partial exists but is False -- Not a frozen tier mount
-                    return False
-                # store.snapshot exists, but partial isn't there -- Possibly a cold tier mount
-                return False
-            raise SearchableSnapshotException('Index not a mounted searchable snapshot')
-        raise SearchableSnapshotException('Index not a mounted searchable snapshot')
-
     def action_generator(self):
         """Yield a dict for use in :py:meth:`do_action` and :py:meth:`do_dry_run`
 
         :returns: A generator object containing the settings necessary to migrate indices from cold
             to frozen
         :rtype: dict
         """
         for idx in self.index_list.indices:
             idx_settings = self.client.indices.get(index=idx)[idx]['settings']['index']
-            if self.has_lifecycle_name(idx_settings):
+            if has_lifecycle_name(idx_settings):
                 self.loggit.critical(
                     'Index %s is associated with an ILM policy and this action will never work on '
                     'an index associated with an ILM policy', idx)
                 raise CuratorException(f'Index {idx} is associated with an ILM policy')
-            if self.is_idx_partial(idx_settings):
+            if is_idx_partial(idx_settings):
                 self.loggit.critical('Index %s is already in the frozen tier', idx)
                 raise SearchableSnapshotException('Index is already in frozen tier')
             snap = idx_settings['store']['snapshot']['snapshot_name']
             snap_idx = idx_settings['store']['snapshot']['index_name']
             repo = idx_settings['store']['snapshot']['repository_name']
             aliases = self.client.indices.get(index=idx)[idx]['aliases']
 
-            prefix = self.get_frozen_prefix(snap_idx, idx)
+            prefix = get_frozen_prefix(snap_idx, idx)
             renamed = f'{prefix}{snap_idx}'
 
             if not self.index_settings:
                 self.index_settings = {
                     "routing": {
                         "allocation": {
                             "include": {
-                                "_tier_preference": self.get_tier_preference()
+                                "_tier_preference": get_tier_preference(self.client)
                             }
                         }
                     }
                 }
             yield {
                 'repository': repo, 'snapshot': snap, 'index': snap_idx,
                 'renamed_index': renamed, 'index_settings': self.index_settings,
@@ -251,27 +149,27 @@
                 newidx = kwargs['renamed_index']
                 # Actually do the mount
                 self.loggit.debug('Mounting new index %s in frozen tier...', newidx)
                 self.client.searchable_snapshots.mount(**kwargs)
                 # Verify it's mounted as a partial now:
                 self.loggit.debug('Verifying new index %s is mounted properly...', newidx)
                 idx_settings = self.client.indices.get(index=newidx)[newidx]
-                if self.is_idx_partial(idx_settings['settings']['index']):
+                if is_idx_partial(idx_settings['settings']['index']):
                     self.loggit.info('Index %s is mounted for frozen tier', newidx)
                 else:
                     raise SearchableSnapshotException(
                         f'Index {newidx} not a mounted searchable snapshot')
                 # Update Aliases
                 alias_names = aliases.keys()
                 if not alias_names:
                     self.loggit.warning('No aliases associated with index %s', current_idx)
                 else:
                     self.loggit.debug('Transferring aliases to new index %s', newidx)
                     self.client.indices.update_aliases(
-                        actions=self.get_alias_actions(current_idx, newidx, aliases))
+                        actions=get_alias_actions(current_idx, newidx, aliases))
                     verify = self.client.indices.get(index=newidx)[newidx]['aliases'].keys()
                     if alias_names != verify:
                         self.loggit.error(
                             'Alias names do not match! %s does not match: %s', alias_names, verify)
                         raise FailedExecution('Aliases failed to transfer to new index')
                 # Clean up old index
                 self.loggit.debug('Deleting old index: %s', current_idx)
```

### Comparing `elasticsearch_curator-8.0.3/curator/actions/create_index.py` & `elasticsearch_curator-8.0.4/curator/actions/create_index.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,18 +60,21 @@
         self.loggit.info(msg)
 
     def do_action(self):
         """
         :py:meth:`~.elasticsearch.client.IndicesClient.create` index identified by :py:attr:`name`
         with values from :py:attr:`aliases`, :py:attr:`mappings`, and :py:attr:`settings`
         """
-        msg = (f'Creating index "{self.name}" with settings: {self.extra_settings}')
+        msg = f'Creating index "{self.name}" with settings: {self.extra_settings}'
         self.loggit.info(msg)
         try:
-            self.client.indices.create(index=self.name, aliases=self.aliases, mappings=self.mappings, settings=self.settings)
+            self.client.indices.create(
+                index=self.name, aliases=self.aliases, mappings=self.mappings,
+                settings=self.settings
+            )
         # Most likely error is a 400, `resource_already_exists_exception`
         except RequestError as err:
             match_list = ["index_already_exists_exception", "resource_already_exists_exception"]
             if err.error in match_list and self.ignore_existing:
                 self.loggit.warning('Index %s already exists.', self.name)
             else:
                 raise FailedExecution(f'Index {self.name} already exists.') from err
```

### Comparing `elasticsearch_curator-8.0.3/curator/actions/delete_indices.py` & `elasticsearch_curator-8.0.4/curator/actions/delete_indices.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.3/curator/actions/forcemerge.py` & `elasticsearch_curator-8.0.4/curator/actions/forcemerge.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.3/curator/actions/index_settings.py` & `elasticsearch_curator-8.0.4/curator/actions/index_settings.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.3/curator/actions/open.py` & `elasticsearch_curator-8.0.4/curator/actions/open.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.3/curator/actions/reindex.py` & `elasticsearch_curator-8.0.4/curator/actions/reindex.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.3/curator/actions/replicas.py` & `elasticsearch_curator-8.0.4/curator/actions/replicas.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.3/curator/actions/rollover.py` & `elasticsearch_curator-8.0.4/curator/actions/rollover.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.3/curator/actions/shrink.py` & `elasticsearch_curator-8.0.4/curator/actions/shrink.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.3/curator/actions/snapshot.py` & `elasticsearch_curator-8.0.4/curator/actions/snapshot.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.3/curator/cli_singletons/__init__.py` & `elasticsearch_curator-8.0.4/curator/cli_singletons/__init__.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.3/curator/cli_singletons/alias.py` & `elasticsearch_curator-8.0.4/curator/cli_singletons/alias.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.3/curator/cli_singletons/allocation.py` & `elasticsearch_curator-8.0.4/curator/cli_singletons/allocation.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.3/curator/cli_singletons/close.py` & `elasticsearch_curator-8.0.4/curator/cli_singletons/close.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.3/curator/cli_singletons/delete.py` & `elasticsearch_curator-8.0.4/curator/cli_singletons/delete.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.3/curator/cli_singletons/forcemerge.py` & `elasticsearch_curator-8.0.4/curator/cli_singletons/forcemerge.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.3/curator/cli_singletons/object_class.py` & `elasticsearch_curator-8.0.4/curator/cli_singletons/object_class.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.3/curator/cli_singletons/open_indices.py` & `elasticsearch_curator-8.0.4/curator/cli_singletons/open_indices.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.3/curator/cli_singletons/replicas.py` & `elasticsearch_curator-8.0.4/curator/cli_singletons/replicas.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.3/curator/cli_singletons/restore.py` & `elasticsearch_curator-8.0.4/curator/cli_singletons/restore.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.3/curator/cli_singletons/rollover.py` & `elasticsearch_curator-8.0.4/curator/cli_singletons/rollover.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.3/curator/cli_singletons/show.py` & `elasticsearch_curator-8.0.4/curator/cli_singletons/show.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.3/curator/cli_singletons/shrink.py` & `elasticsearch_curator-8.0.4/curator/cli_singletons/shrink.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.3/curator/cli_singletons/snapshot.py` & `elasticsearch_curator-8.0.4/curator/cli_singletons/snapshot.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.3/curator/cli_singletons/utils.py` & `elasticsearch_curator-8.0.4/curator/cli_singletons/utils.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.3/curator/defaults/filter_elements.py` & `elasticsearch_curator-8.0.4/curator/defaults/filter_elements.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.3/curator/defaults/filtertypes.py` & `elasticsearch_curator-8.0.4/curator/defaults/filtertypes.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.3/curator/defaults/logging_defaults.py` & `elasticsearch_curator-8.0.4/curator/defaults/logging_defaults.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.3/curator/defaults/option_defaults.py` & `elasticsearch_curator-8.0.4/curator/defaults/option_defaults.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.3/curator/defaults/settings.py` & `elasticsearch_curator-8.0.4/curator/defaults/settings.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.3/curator/helpers/date_ops.py` & `elasticsearch_curator-8.0.4/curator/helpers/date_ops.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.3/curator/helpers/getters.py` & `elasticsearch_curator-8.0.4/curator/helpers/waiters.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,306 +1,306 @@
-"""Utility functions that get things"""
-# :pylint disable=
-import logging
-from elasticsearch8 import exceptions as es8exc
-from es_client.defaults import VERSION_MAX, VERSION_MIN
-from es_client.builder import Builder
-from curator.exceptions import ClientException, CuratorException, FailedExecution, MissingArgument
-
-def byte_size(num, suffix='B'):
-    """
-    :param num: The number of byte
-    :param suffix: An arbitrary suffix, like ``Bytes``
-
-    :type num: int
-    :type suffix: str
-
-    :returns: A formatted string indicating the size in bytes, with the proper unit,
-        e.g. KB, MB, GB, TB, etc.
-    :rtype: float
-    """
-    for unit in ['', 'K', 'M', 'G', 'T', 'P', 'E', 'Z']:
-        if abs(num) < 1024.0:
-            return f'{num:3.1f}{unit}{suffix}'
-        num /= 1024.0
-    return f'{num:.1f}Y{suffix}'
-
-def get_client(
-    configdict=None, configfile=None, autoconnect=False, version_min=VERSION_MIN,
-    version_max=VERSION_MAX):
-    """Get an Elasticsearch Client using :py:class:`es_client.Builder`
-
-    Build a client out of settings from `configfile` or `configdict`
-    If neither `configfile` nor `configdict` is provided, empty defaults will be used.
-    If both are provided, `configdict` will be used, and `configfile` ignored.
-
-    :param configdict: A configuration dictionary
-    :param configfile: A configuration file
-    :param autoconnect: Connect to client automatically
-    :param verion_min: Minimum acceptable version of Elasticsearch (major, minor, patch)
-    :param verion_max: Maximum acceptable version of Elasticsearch (major, minor, patch)
-
-    :type configdict: dict
-    :type configfile: str
-    :type autoconnect: bool
-    :type version_min: tuple
-    :type version_max: tuple
-
-    :returns: A client connection object
-    :rtype: :py:class:`~.elasticsearch.Elasticsearch`
-    """
-    logger = logging.getLogger(__name__)
-    logger.info('Creating client object and testing connection')
+"""The function that waits
 
-    builder = Builder(
-        configdict=configdict, configfile=configfile, autoconnect=autoconnect,
-        version_min=version_min, version_max=version_max
-    )
-
-    try:
-        builder.connect()
-    except Exception as exc:
-        logger.critical('Exception encountered: %s', exc)
-        raise ClientException from exc
-
-    return builder.client
+...and its helpers
+"""
+import logging
+from time import localtime, sleep, strftime
+from datetime import datetime
+from curator.exceptions import (
+    ActionTimeout, ConfigurationError, CuratorException, FailedReindex, MissingArgument)
+from curator.helpers.utils import chunk_index_list
+
+def health_check(client, **kwargs):
+    """
+    This function calls `client.cluster.` :py:meth:`~.elasticsearch.client.ClusterClient.health` and, based on the
+    params provided, will return ``True`` or ``False`` depending on whether that particular keyword
+    appears in the output, and has the expected value.
 
-def get_data_tiers(client):
-    """
-    Get all valid data tiers from the node roles of each node in the cluster by polling each node
+    If multiple keys are provided, all must match for a ``True`` response.
 
     :param client: A client connection object
-    :type client: :py:class:`~.elasticsearch.Elasticsearch`
 
-    :returns: The available data tiers in ``tier: bool`` form.
-    :rtype: dict
-    """
-    def role_check(role, node_info):
-        if role in node_info['roles']:
-            return True
-        return False
-    info = client.nodes.info()['nodes']
-    retval = {'data_hot': False, 'data_warm': False, 'data_cold': False, 'data_frozen': False}
-    for node in info:
-        for role in ['data_hot', 'data_warm', 'data_cold', 'data_frozen']:
-            # This guarantees we don't overwrite a True with a False. We only add True values
-            if role_check(role, info[node]):
-                retval[role] = True
-    return retval
-
-def get_indices(client):
-    """
-    Calls :py:meth:`~.elasticsearch.client.IndicesClient.get_settings`
-
-    :param client: A client connection object
     :type client: :py:class:`~.elasticsearch.Elasticsearch`
 
-    :returns: The current list of indices from the cluster
-    :rtype: list
+    :rtype: bool
     """
     logger = logging.getLogger(__name__)
-    try:
-        indices = list(client.indices.get_settings(index='*', expand_wildcards='open,closed'))
-        logger.debug('All indices: %s', indices)
-        return indices
-    except Exception as err:
-        raise FailedExecution(f'Failed to get indices. Error: {err}') from err
-
-def get_repository(client, repository=''):
-    """
-    Calls :py:meth:`~.elasticsearch.client.SnapshotClient.get_repository`
+    logger.debug('KWARGS= "%s"', kwargs)
+    klist = list(kwargs.keys())
+    if not klist:
+        raise MissingArgument('Must provide at least one keyword argument')
+    hc_data = client.cluster.health()
+    response = True
+
+    for k in klist:
+        # First, verify that all kwargs are in the list
+        if not k in list(hc_data.keys()):
+            raise ConfigurationError('Key "{0}" not in cluster health output')
+        if not hc_data[k] == kwargs[k]:
+            msg = f'NO MATCH: Value for key "{kwargs[k]}", health check data: {hc_data[k]}'
+            logger.debug(msg)
+            response = False
+        else:
+            msg = f'MATCH: Value for key "{kwargs[k]}", health check data: {hc_data[k]}'
+            logger.debug(msg)
+    if response:
+        logger.info('Health Check for all provided keys passed.')
+    return response
+
+def relocate_check(client, index):
+    """
+    This function calls `client.cluster.` :py:meth:`~.elasticsearch.client.ClusterClient.state`
+    with a given index to check if all of the shards for that index are in the ``STARTED`` state.
+    It will return ``True`` if all primary and replica shards are in the ``STARTED`` state, and it
+    will return ``False`` if any shard is in a different state.
 
     :param client: A client connection object
-    :param repository: The Elasticsearch snapshot repository to use
+    :param index: The index name
 
     :type client: :py:class:`~.elasticsearch.Elasticsearch`
-    :type repository: str
+    :type index: str
 
-    :returns: Configuration information for ``repository``.
-    :rtype: dict
+    :rtype: bool
     """
-    try:
-        return client.snapshot.get_repository(name=repository)
-    except (es8exc.TransportError, es8exc.NotFoundError) as err:
-        msg = (
-            f'Unable to get repository {repository}.  Error: {err} Check Elasticsearch '
-            f'logs for more information.'
+    logger = logging.getLogger(__name__)
+    shard_state_data = (
+        client.cluster.state(index=index)['routing_table']['indices'][index]['shards']
+    )
+    finished_state = (
+        all(
+            all(
+                shard['state'] == "STARTED" for shard in shards
+            )
+            for shards in shard_state_data.values()
         )
-        raise CuratorException(msg) from err
+    )
+    if finished_state:
+        logger.info('Relocate Check for index: "%s" has passed.', index)
+    return finished_state
 
-def get_snapshot(client, repository=None, snapshot=''):
+def restore_check(client, index_list):
     """
-    Calls :py:meth:`~.elasticsearch.client.SnapshotClient.get`
+    This function calls `client.indices.` :py:meth:`~.elasticsearch.client.IndicesClient.recovery`
+    with the list of indices to check for complete recovery.  It will return ``True`` if recovery
+    of those indices is complete, and ``False`` otherwise.  It is designed to fail fast: if a
+    single shard is encountered that is still recovering (not in ``DONE`` stage), it will
+    immediately return ``False``, rather than complete iterating over the rest of the response.
 
     :param client: A client connection object
-    :param repository: The Elasticsearch snapshot repository to use
-    :param snapshot: The snapshot name, or a comma-separated list of snapshots
+    :param index_list: The list of indices to verify having been restored.
 
     :type client: :py:class:`~.elasticsearch.Elasticsearch`
-    :type repository: str
-    :type snapshot: str
-
-    :returns: Information about the provided ``snapshot``, a snapshot (or a comma-separated list of
-        snapshots). If no snapshot specified, it will collect info for all snapshots.  If none
-        exist, an empty :py:class:`dict` will be returned.
-    :rtype: dict
-    """
-    if not repository:
-        raise MissingArgument('No value for "repository" provided')
-    snapname = '*' if snapshot == '' else snapshot
-    try:
-        return client.snapshot.get(repository=repository, snapshot=snapshot)
-    except (es8exc.TransportError, es8exc.NotFoundError) as err:
-        msg = (
-            f'Unable to get information about snapshot {snapname} from repository: '
-            f'{repository}.  Error: {err}'
-        )
-        raise FailedExecution(msg) from err
+    :type index_list: list
 
-def get_snapshot_data(client, repository=None):
+    :rtype: bool
     """
-    Get all snapshots from repository and return a list.
-    Calls :py:meth:`~.elasticsearch.client.SnapshotClient.get`
+    logger = logging.getLogger(__name__)
+    response = {}
+    for chunk in chunk_index_list(index_list):
+        try:
+            chunk_response = client.indices.recovery(index=chunk, human=True)
+        except Exception as err:
+            msg = f'Unable to obtain recovery information for specified indices. Error: {err}'
+            raise CuratorException(msg) from err
+        if chunk_response == {}:
+            logger.info('_recovery returned an empty response. Trying again.')
+            return False
+        response.update(chunk_response)
+    logger.info('Provided indices: %s', index_list)
+    logger.info('Found indices: %s', list(response.keys()))
+    # pylint: disable=consider-using-dict-items
+    for index in response:
+        for shard in range(0, len(response[index]['shards'])):
+            stage = response[index]['shards'][shard]['stage']
+            if stage != 'DONE':
+                logger.info('Index "%s" is still in stage "%s"', index, stage)
+                return False
+
+    # If we've gotten here, all of the indices have recovered
+    return True
+
+def snapshot_check(client, snapshot=None, repository=None):
+    """
+    This function calls `client.snapshot.` :py:meth:`~.elasticsearch.client.SnapshotClient.get` and tests to see
+    whether the snapshot is complete, and if so, with what status.  It will log errors according
+    to the result. If the snapshot is still ``IN_PROGRESS``, it will return ``False``.  ``SUCCESS``
+    will be an ``INFO`` level message, ``PARTIAL`` nets a ``WARNING`` message, ``FAILED`` is an
+    ``ERROR``, message, and all others will be a ``WARNING`` level message.
 
     :param client: A client connection object
-    :param repository: The Elasticsearch snapshot repository to use
+    :param snapshot: The snapshot name
+    :param repository: The repository name
 
     :type client: :py:class:`~.elasticsearch.Elasticsearch`
+    :type snapshot: str
     :type repository: str
 
-    :returns: The list of all snapshots from ``repository``
-    :rtype: list
-    """
-    if not repository:
-        raise MissingArgument('No value for "repository" provided')
-    try:
-        return client.snapshot.get(repository=repository, snapshot="*")['snapshots']
-    except (es8exc.TransportError, es8exc.NotFoundError) as err:
-        msg = (
-            f'Unable to get snapshot information from repository: '
-            f'{repository}. Error: {err}'
-        )
-        raise FailedExecution(msg) from err
-
-def get_write_index(client, alias):
-    """
-    Calls :py:meth:`~.elasticsearch.client.IndicesClient.get_alias`
-
-    :param client: A client connection object
-    :param alias: An alias name
-
-    :type client: :py:class:`~.elasticsearch.Elasticsearch`
-    :type alias: str
-
-    :returns: The the index name associated with the alias that is designated ``is_write_index``
-    :rtype: str
+    :rtype: bool
     """
+    logger = logging.getLogger(__name__)
+    logger.debug('SNAPSHOT: %s', snapshot)
+    logger.debug('REPOSITORY: %s', repository)
     try:
-        response = client.indices.get_alias(index=alias)
-    except Exception as exc:
-        raise CuratorException(f'Alias {alias} not found') from exc
-    # If there are more than one in the list, one needs to be the write index
-    # otherwise the alias is a one to many, and can't do rollover.
-    if len(list(response.keys())) > 1:
-        for index in list(response.keys()):
-            try:
-                if response[index]['aliases'][alias]['is_write_index']:
-                    return index
-            except KeyError as exc:
-                raise FailedExecution(
-                    'Invalid alias: is_write_index not found in 1 to many alias') from exc
+        result = client.snapshot.get(repository=repository, snapshot=snapshot)
+        logger.debug('RESULT: %s', result)
+    except Exception as err:
+        raise CuratorException(
+            f'Unable to obtain information for snapshot "{snapshot}" in repository '
+            f'"{repository}". Error: {err}'
+        ) from err
+    state = result['snapshots'][0]['state']
+    logger.debug('Snapshot state = %s', state)
+    retval = True
+    if state == 'IN_PROGRESS':
+        logger.info('Snapshot %s still in progress.', snapshot)
+        retval = False
+    elif state == 'SUCCESS':
+        logger.info('Snapshot %s successfully completed.', snapshot)
+    elif state == 'PARTIAL':
+        logger.warning('Snapshot %s completed with state PARTIAL.', snapshot)
+    elif state == 'FAILED':
+        logger.error('Snapshot %s completed with state FAILED.', snapshot)
     else:
-        # There's only one, so this is it
-        return list(response.keys())[0]
-
-def index_size(client, idx, value='total'):
-    """
-    Calls :py:meth:`~.elasticsearch.client.IndicesClient.stats`
-
-    :param client: A client connection object
-    :param idx: An index name
-    :param value: One of either ``primaries`` or ``total``
-
-    :type client: :py:class:`~.elasticsearch.Elasticsearch`
-    :type idx: str
-    :type value: str
-
-    :returns: The sum of either ``primaries`` or ``total`` shards for index ``idx``
-    :rtype: integer
-    """
-    return client.indices.stats(index=idx)['indices'][idx][value]['store']['size_in_bytes']
-
-def name_to_node_id(client, name):
-    """
-    Calls :py:meth:`~.elasticsearch.client.NodesClient.stats`
-
-    :param client: A client connection object
-    :param name: The node ``name``
-
-    :type client: :py:class:`~.elasticsearch.Elasticsearch`
-    :type name: str
-
-    :returns: The node_id of the node identified by ``name``
-    :rtype: str
-    """
-    logger = logging.getLogger(__name__)
-    stats = client.nodes.stats()
-    for node in stats['nodes']:
-        if stats['nodes'][node]['name'] == name:
-            logger.debug('Found node_id "%s" for name "%s".', node, name)
-            return node
-    logger.error('No node_id found matching name: "%s"', name)
-    return None
+        logger.warning('Snapshot %s completed with state: %s', snapshot, state)
+    return retval
 
-def node_id_to_name(client, node_id):
+def task_check(client, task_id=None):
     """
-    Calls :py:meth:`~.elasticsearch.client.NodesClient.stats`
+    This function calls `client.tasks.` :py:meth:`~.elasticsearch.client.TasksClient.get` with the
+    provided ``task_id``.  If the task data contains ``'completed': True``, then it will return
+    ``True``. If the task is not completed, it will log some information about the task and return
+    ``False``
 
     :param client: A client connection object
-    :param node_id: The node ``node_id``
+    :param task_id: The task id
 
     :type client: :py:class:`~.elasticsearch.Elasticsearch`
-    :type node_id: str
+    :type task_id: str
 
-    :returns: The name of the node identified by ``node_id``
-    :rtype: str
+    :rtype: bool
     """
     logger = logging.getLogger(__name__)
-    stats = client.nodes.stats()
-    name = None
-    if node_id in stats['nodes']:
-        name = stats['nodes'][node_id]['name']
+    try:
+        task_data = client.tasks.get(task_id=task_id)
+    except Exception as err:
+        msg = f'Unable to obtain task information for task_id "{task_id}". Exception {err}'
+        raise CuratorException(msg) from err
+    task = task_data['task']
+    completed = task_data['completed']
+    if task['action'] == 'indices:data/write/reindex':
+        logger.debug('It\'s a REINDEX TASK')
+        logger.debug('TASK_DATA: %s', task_data)
+        logger.debug('TASK_DATA keys: %s', list(task_data.keys()))
+        if 'response' in task_data:
+            response = task_data['response']
+            if response['failures']:
+                msg = f'Failures found in reindex response: {response["failures"]}'
+                raise FailedReindex(msg)
+    running_time = 0.000000001 * task['running_time_in_nanos']
+    logger.debug('Running time: %s seconds', running_time)
+    descr = task['description']
+
+    if completed:
+        completion_time = ((running_time * 1000) + task['start_time_in_millis'])
+        time_string = strftime('%Y-%m-%dT%H:%M:%SZ', localtime(completion_time/1000))
+        logger.info('Task "%s" completed at %s.', descr, time_string)
+        retval = True
     else:
-        logger.error('No node_id found matching: "%s"', node_id)
-    logger.debug('Name associated with node_id "%s": %s', node_id, name)
-    return name
+        # Log the task status here.
+        logger.debug('Full Task Data: %s', task_data)
+        msg = (
+            f'Task "{descr}" with task_id "{task_id}" has been running for {running_time} seconds'
+        )
+        logger.info(msg)
+        retval = False
+    return retval
 
-def node_roles(client, node_id):
-    """
-    Calls :py:meth:`~.elasticsearch.client.NodesClient.info`
+# pylint: disable=too-many-locals, too-many-arguments
+def wait_for_it(
+        client, action, task_id=None, snapshot=None, repository=None, index=None, index_list=None,
+        wait_interval=9, max_wait=-1
+    ):
+    """
+    This function becomes one place to do all ``wait_for_completion`` type behaviors
 
     :param client: A client connection object
-    :param node_id: The node ``node_id``
+    :param action: The action name that will identify how to wait
+    :param task_id: If the action provided a task_id, this is where it must be declared.
+    :param snapshot: The name of the snapshot.
+    :param repository: The Elasticsearch snapshot repository to use
+    :param wait_interval: Seconds to wait between completion checks.
+    :param max_wait: Maximum number of seconds to ``wait_for_completion``
 
     :type client: :py:class:`~.elasticsearch.Elasticsearch`
-    :type node_id: str
-
-    :returns: The list of roles assigned to the node identified by ``node_id``
-    :rtype: list
-    """
-    return client.nodes.info()['nodes'][node_id]['roles']
-
-def single_data_path(client, node_id):
+    :type action: str
+    :type task_id: str
+    :type snapshot: str
+    :type repository: str
+    :type wait_interval: int
+    :type max_wait: int
+    :rtype: None
     """
-    In order for a shrink to work, it should be on a single filesystem, as shards cannot span
-    filesystems. Calls :py:meth:`~.elasticsearch.client.NodesClient.stats`
-
-    :param client: A client connection object
-    :param node_id: The node ``node_id``
-
-    :type client: :py:class:`~.elasticsearch.Elasticsearch`
-    :type node_id: str
+    logger = logging.getLogger(__name__)
+    action_map = {
+        'allocation':{'function': health_check, 'args': {'relocating_shards':0}},
+        'replicas':{'function': health_check, 'args': {'status':'green'}},
+        'cluster_routing':{'function': health_check, 'args': {'relocating_shards':0}},
+        'snapshot':{
+            'function':snapshot_check, 'args':{'snapshot':snapshot, 'repository':repository}},
+        'restore':{'function':restore_check, 'args':{'index_list':index_list}},
+        'reindex':{'function':task_check, 'args':{'task_id':task_id}},
+        'shrink':{'function': health_check, 'args': {'status':'green'}},
+        'relocate':{'function': relocate_check, 'args': {'index':index}},
+    }
+    wait_actions = list(action_map.keys())
+
+    if action not in wait_actions:
+        raise ConfigurationError(f'"action" must be one of {wait_actions}')
+    if action == 'reindex' and task_id is None:
+        raise MissingArgument(f'A task_id must accompany "action" {action}')
+    if action == 'snapshot' and ((snapshot is None) or (repository is None)):
+        raise MissingArgument(
+            f'A snapshot and repository must accompany "action" {action}. snapshot: '
+            f'{snapshot}, repository: {repository}'
+        )
+    if action == 'restore' and index_list is None:
+        raise MissingArgument(f'An index_list must accompany "action" {action}')
+    if action == 'reindex':
+        try:
+            _ = client.tasks.get(task_id=task_id)
+        except Exception as err:
+            # This exception should only exist in API usage. It should never
+            # occur in regular Curator usage.
+            raise CuratorException(f'Unable to find task_id {task_id}. Exception: {err}') from err
+
+    # Now with this mapped, we can perform the wait as indicated.
+    start_time = datetime.now()
+    result = False
+    while True:
+        elapsed = int((datetime.now() - start_time).total_seconds())
+        logger.debug('Elapsed time: %s seconds', elapsed)
+        response = action_map[action]['function'](client, **action_map[action]['args'])
+        logger.debug('Response: %s', response)
+        # Success
+        if response:
+            logger.debug(
+                'Action "%s" finished executing (may or may not have been successful)', action)
+            result = True
+            break
+        # Not success, and reached maximum wait (if defined)
+        if (max_wait != -1) and (elapsed >= max_wait):
+            msg = f'Unable to complete action "{action}" within max_wait ({max_wait}) seconds.'
+            logger.error(msg)
+            break
+        # Not success, so we wait.
+        msg = (
+            f'Action "{action}" not yet complete, {elapsed} total seconds elapsed. '
+            f'Waiting {wait_interval} seconds before checking again.'
+        )
+        logger.debug(msg)
+        sleep(wait_interval)
 
-    :returns: ``True`` if the node has a single filesystem, else ``False``
-    :rtype: bool
-    """
-    return len(client.nodes.stats()['nodes'][node_id]['fs']['data']) == 1
+    logger.debug('Result: %s', result)
+    if not result:
+        raise ActionTimeout(
+            f'Action "{action}" failed to complete in the max_wait period of {max_wait} seconds'
+        )
```

### Comparing `elasticsearch_curator-8.0.3/curator/helpers/testers.py` & `elasticsearch_curator-8.0.4/curator/helpers/testers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,54 @@
 """Utility functions that get things"""
 import logging
 from voluptuous import Schema
 from elasticsearch8 import Elasticsearch
 from elasticsearch8.exceptions import NotFoundError
 from es_client.helpers.utils import prune_nones
 from curator.helpers.getters import get_repository, get_write_index
-from curator.exceptions import ConfigurationError, MissingArgument, RepositoryException
+from curator.exceptions import (
+    ConfigurationError, MissingArgument, RepositoryException, SearchableSnapshotException)
 from curator.defaults.settings import index_filtertypes, snapshot_actions, snapshot_filtertypes
 from curator.validators import SchemaCheck, actions, options
 from curator.validators.filter_functions import validfilters
 from curator.helpers.utils import report_failure
 
+def has_lifecycle_name(idx_settings):
+    """
+    :param idx_settings: The settings for an index being tested
+    :type idx_settings: dict
+
+    :returns: ``True`` if a lifecycle name exists in settings, else ``False``
+    :rtype: bool
+    """
+    if 'lifecycle' in idx_settings:
+        if 'name' in idx_settings['lifecycle']:
+            return True
+    return False
+
+def is_idx_partial(idx_settings):
+    """
+    :param idx_settings: The settings for an index being tested
+    :type idx_settings: dict
+
+    :returns: ``True`` if store.snapshot.partial exists in settings, else ``False``
+    :rtype: bool
+    """
+    if 'store' in idx_settings:
+        if 'snapshot' in idx_settings['store']:
+            if 'partial' in idx_settings['store']['snapshot']:
+                if idx_settings['store']['snapshot']['partial']:
+                    return True
+                # store.snapshot.partial exists but is False -- Not a frozen tier mount
+                return False
+            # store.snapshot exists, but partial isn't there -- Possibly a cold tier mount
+            return False
+        raise SearchableSnapshotException('Index not a mounted searchable snapshot')
+    raise SearchableSnapshotException('Index not a mounted searchable snapshot')
+
 def ilm_policy_check(client, alias):
     """Test if alias is associated with an ILM policy
 
     Calls :py:meth:`~.elasticsearch.client.IndicesClient.get_settings`
 
     :param client: A client connection object
     :param alias: The alias name
@@ -276,16 +310,16 @@
 
 def verify_index_list(test):
     """
     :param test: The variable or object to test
 
     :type test: :py:class:`~.curator.IndexList`
 
-    :returns: ``None`` if ``test`` is a proper :py:class:`~.curator.indexlist.IndexList` object, else
-        raise a :py:class:`TypeError` exception.
+    :returns: ``None`` if ``test`` is a proper :py:class:`~.curator.indexlist.IndexList` object,
+        else raise a :py:class:`TypeError` exception.
     :rtype: None
     """
     # It breaks if this import isn't local to this function:
     # ImportError: cannot import name 'IndexList' from partially initialized module
     # 'curator.indexlist' (most likely due to a circular import)
     # pylint: disable=import-outside-toplevel
     from curator.indexlist import IndexList
@@ -323,15 +357,15 @@
                 )
             else:
                 msg = (
                     f'--- Got a {err.meta.status} response from Elasticsearch.  '
                     f'Error message: {err.error}'
                 )
         except AttributeError:
-            msg = (f'--- Error message: {err}'.format())
+            msg = f'--- Error message: {err}'.format()
         report = f'Failed to verify all nodes have repository access: {msg}'
         raise RepositoryException(report) from err
 
 def verify_snapshot_list(test):
     """
     :param test: The variable or object to test
```

### Comparing `elasticsearch_curator-8.0.3/curator/helpers/utils.py` & `elasticsearch_curator-8.0.4/curator/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.3/curator/helpers/waiters.py` & `elasticsearch_curator-8.0.4/curator/helpers/getters.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,306 +1,395 @@
-"""The function that waits
-
-...and its helpers
-"""
+"""Utility functions that get things"""
+# :pylint disable=
 import logging
-from time import localtime, sleep, strftime
-from datetime import datetime
-from curator.exceptions import (
-    ActionTimeout, ConfigurationError, CuratorException, FailedReindex, MissingArgument)
-from curator.helpers.utils import chunk_index_list
-
-def health_check(client, **kwargs):
-    """
-    This function calls `client.cluster.` :py:meth:`~.elasticsearch.client.ClusterClient.health` and, based on the
-    params provided, will return ``True`` or ``False`` depending on whether that particular keyword
-    appears in the output, and has the expected value.
+import re
+from elasticsearch8 import exceptions as es8exc
+from es_client.defaults import VERSION_MAX, VERSION_MIN
+from es_client.builder import Builder
+from curator.exceptions import ClientException, CuratorException, FailedExecution, MissingArgument
+
+def byte_size(num, suffix='B'):
+    """
+    :param num: The number of byte
+    :param suffix: An arbitrary suffix, like ``Bytes``
+
+    :type num: int
+    :type suffix: str
+
+    :returns: A formatted string indicating the size in bytes, with the proper unit,
+        e.g. KB, MB, GB, TB, etc.
+    :rtype: float
+    """
+    for unit in ['', 'K', 'M', 'G', 'T', 'P', 'E', 'Z']:
+        if abs(num) < 1024.0:
+            return f'{num:3.1f}{unit}{suffix}'
+        num /= 1024.0
+    return f'{num:.1f}Y{suffix}'
+
+def get_alias_actions(oldidx, newidx, aliases):
+    """
+    :param oldidx: The old index name
+    :param newidx: The new index name
+    :param aliases: The aliases
+
+    :type oldidx: str
+    :type newidx: str
+    :type aliases: dict
+
+    :returns: A list of actions suitable for
+        :py:meth:`~.elasticsearch.client.IndicesClient.update_aliases` ``actions`` kwarg.
+    :rtype: list
+    """
+    actions = []
+    for alias in aliases.keys():
+        actions.append({'remove': {'index': oldidx, 'alias': alias}})
+        actions.append({'add': {'index': newidx, 'alias': alias}})
+    return actions
+
+def get_client(
+    configdict=None, configfile=None, autoconnect=False, version_min=VERSION_MIN,
+    version_max=VERSION_MAX):
+    """Get an Elasticsearch Client using :py:class:`es_client.Builder`
+
+    Build a client out of settings from `configfile` or `configdict`
+    If neither `configfile` nor `configdict` is provided, empty defaults will be used.
+    If both are provided, `configdict` will be used, and `configfile` ignored.
+
+    :param configdict: A configuration dictionary
+    :param configfile: A configuration file
+    :param autoconnect: Connect to client automatically
+    :param verion_min: Minimum acceptable version of Elasticsearch (major, minor, patch)
+    :param verion_max: Maximum acceptable version of Elasticsearch (major, minor, patch)
+
+    :type configdict: dict
+    :type configfile: str
+    :type autoconnect: bool
+    :type version_min: tuple
+    :type version_max: tuple
+
+    :returns: A client connection object
+    :rtype: :py:class:`~.elasticsearch.Elasticsearch`
+    """
+    logger = logging.getLogger(__name__)
+    logger.info('Creating client object and testing connection')
+
+    builder = Builder(
+        configdict=configdict, configfile=configfile, autoconnect=autoconnect,
+        version_min=version_min, version_max=version_max
+    )
+
+    try:
+        builder.connect()
+    except Exception as exc:
+        logger.critical('Exception encountered: %s', exc)
+        raise ClientException from exc
 
-    If multiple keys are provided, all must match for a ``True`` response.
+    return builder.client
+
+def get_data_tiers(client):
+    """
+    Get all valid data tiers from the node roles of each node in the cluster by polling each node
 
     :param client: A client connection object
+    :type client: :py:class:`~.elasticsearch.Elasticsearch`
 
+    :returns: The available data tiers in ``tier: bool`` form.
+    :rtype: dict
+    """
+    def role_check(role, node_info):
+        if role in node_info['roles']:
+            return True
+        return False
+    info = client.nodes.info()['nodes']
+    retval = {'data_hot': False, 'data_warm': False, 'data_cold': False, 'data_frozen': False}
+    for node in info:
+        for role in ['data_hot', 'data_warm', 'data_cold', 'data_frozen']:
+            # This guarantees we don't overwrite a True with a False. We only add True values
+            if role_check(role, info[node]):
+                retval[role] = True
+    return retval
+
+def get_frozen_prefix(oldidx, curridx):
+    """
+    Use regular expression magic to extract the prefix from the current index, and then use
+    that with ``partial-`` in front to name the resulting index.
+
+    If there is no prefix, then we just send back ``partial-``
+
+    :param oldidx: The index name before it was mounted in cold tier
+    :param curridx: The current name of the index, as mounted in cold tier
+
+    :type oldidx: str
+    :type curridx: str
+
+    :returns: The prefix to prepend the index name with for mounting as frozen
+    :rtype: str
+    """
+    logger = logging.getLogger(__name__)
+    pattern = f'^(.*){oldidx}$'
+    regexp = re.compile(pattern)
+    match = regexp.match(curridx)
+    prefix = match.group(1)
+    logger.debug('Detected match group for prefix: %s', prefix)
+    if not prefix:
+        return 'partial-'
+    return f'partial-{prefix}'
+
+def get_indices(client):
+    """
+    Calls :py:meth:`~.elasticsearch.client.IndicesClient.get_settings`
+
+    :param client: A client connection object
     :type client: :py:class:`~.elasticsearch.Elasticsearch`
 
-    :rtype: bool
+    :returns: The current list of indices from the cluster
+    :rtype: list
     """
     logger = logging.getLogger(__name__)
-    logger.debug('KWARGS= "%s"', kwargs)
-    klist = list(kwargs.keys())
-    if not klist:
-        raise MissingArgument('Must provide at least one keyword argument')
-    hc_data = client.cluster.health()
-    response = True
-
-    for k in klist:
-        # First, verify that all kwargs are in the list
-        if not k in list(hc_data.keys()):
-            raise ConfigurationError('Key "{0}" not in cluster health output')
-        if not hc_data[k] == kwargs[k]:
-            msg = f'NO MATCH: Value for key "{kwargs[k]}", health check data: {hc_data[k]}'
-            logger.debug(msg)
-            response = False
-        else:
-            msg = f'MATCH: Value for key "{kwargs[k]}", health check data: {hc_data[k]}'
-            logger.debug(msg)
-    if response:
-        logger.info('Health Check for all provided keys passed.')
-    return response
-
-def relocate_check(client, index):
-    """
-    This function calls `client.cluster.` :py:meth:`~.elasticsearch.client.ClusterClient.state`
-    with a given index to check if all of the shards for that index are in the ``STARTED`` state.
-    It will return ``True`` if all primary and replica shards are in the ``STARTED`` state, and it
-    will return ``False`` if any shard is in a different state.
+    try:
+        indices = list(client.indices.get_settings(index='*', expand_wildcards='open,closed'))
+        logger.debug('All indices: %s', indices)
+        return indices
+    except Exception as err:
+        raise FailedExecution(f'Failed to get indices. Error: {err}') from err
+
+def get_repository(client, repository=''):
+    """
+    Calls :py:meth:`~.elasticsearch.client.SnapshotClient.get_repository`
 
     :param client: A client connection object
-    :param index: The index name
+    :param repository: The Elasticsearch snapshot repository to use
 
     :type client: :py:class:`~.elasticsearch.Elasticsearch`
-    :type index: str
+    :type repository: str
 
-    :rtype: bool
+    :returns: Configuration information for ``repository``.
+    :rtype: dict
     """
-    logger = logging.getLogger(__name__)
-    shard_state_data = (
-        client.cluster.state(index=index)['routing_table']['indices'][index]['shards']
-    )
-    finished_state = (
-        all(
-            all(
-                shard['state'] == "STARTED" for shard in shards
-            )
-            for shards in shard_state_data.values()
+    try:
+        return client.snapshot.get_repository(name=repository)
+    except (es8exc.TransportError, es8exc.NotFoundError) as err:
+        msg = (
+            f'Unable to get repository {repository}.  Error: {err} Check Elasticsearch '
+            f'logs for more information.'
         )
-    )
-    if finished_state:
-        logger.info('Relocate Check for index: "%s" has passed.', index)
-    return finished_state
+        raise CuratorException(msg) from err
 
-def restore_check(client, index_list):
+def get_snapshot(client, repository=None, snapshot=''):
     """
-    This function calls `client.indices.` :py:meth:`~.elasticsearch.client.IndicesClient.recovery`
-    with the list of indices to check for complete recovery.  It will return ``True`` if recovery
-    of those indices is complete, and ``False`` otherwise.  It is designed to fail fast: if a
-    single shard is encountered that is still recovering (not in ``DONE`` stage), it will
-    immediately return ``False``, rather than complete iterating over the rest of the response.
+    Calls :py:meth:`~.elasticsearch.client.SnapshotClient.get`
 
     :param client: A client connection object
-    :param index_list: The list of indices to verify having been restored.
+    :param repository: The Elasticsearch snapshot repository to use
+    :param snapshot: The snapshot name, or a comma-separated list of snapshots
 
     :type client: :py:class:`~.elasticsearch.Elasticsearch`
-    :type index_list: list
+    :type repository: str
+    :type snapshot: str
 
-    :rtype: bool
+    :returns: Information about the provided ``snapshot``, a snapshot (or a comma-separated list of
+        snapshots). If no snapshot specified, it will collect info for all snapshots.  If none
+        exist, an empty :py:class:`dict` will be returned.
+    :rtype: dict
+    """
+    if not repository:
+        raise MissingArgument('No value for "repository" provided')
+    snapname = '*' if snapshot == '' else snapshot
+    try:
+        return client.snapshot.get(repository=repository, snapshot=snapshot)
+    except (es8exc.TransportError, es8exc.NotFoundError) as err:
+        msg = (
+            f'Unable to get information about snapshot {snapname} from repository: '
+            f'{repository}.  Error: {err}'
+        )
+        raise FailedExecution(msg) from err
+
+def get_snapshot_data(client, repository=None):
     """
-    logger = logging.getLogger(__name__)
-    response = {}
-    for chunk in chunk_index_list(index_list):
-        try:
-            chunk_response = client.indices.recovery(index=chunk, human=True)
-        except Exception as err:
-            msg = f'Unable to obtain recovery information for specified indices. Error: {err}'
-            raise CuratorException(msg) from err
-        if chunk_response == {}:
-            logger.info('_recovery returned an empty response. Trying again.')
-            return False
-        response.update(chunk_response)
-    logger.info('Provided indices: %s', index_list)
-    logger.info('Found indices: %s', list(response.keys()))
-    # pylint: disable=consider-using-dict-items
-    for index in response:
-        for shard in range(0, len(response[index]['shards'])):
-            stage = response[index]['shards'][shard]['stage']
-            if stage != 'DONE':
-                logger.info('Index "%s" is still in stage "%s"', index, stage)
-                return False
-
-    # If we've gotten here, all of the indices have recovered
-    return True
-
-def snapshot_check(client, snapshot=None, repository=None):
-    """
-    This function calls `client.snapshot.` :py:meth:`~.elasticsearch.client.SnapshotClient.get` and tests to see
-    whether the snapshot is complete, and if so, with what status.  It will log errors according
-    to the result. If the snapshot is still ``IN_PROGRESS``, it will return ``False``.  ``SUCCESS``
-    will be an ``INFO`` level message, ``PARTIAL`` nets a ``WARNING`` message, ``FAILED`` is an
-    ``ERROR``, message, and all others will be a ``WARNING`` level message.
+    Get all snapshots from repository and return a list.
+    Calls :py:meth:`~.elasticsearch.client.SnapshotClient.get`
 
     :param client: A client connection object
-    :param snapshot: The snapshot name
-    :param repository: The repository name
+    :param repository: The Elasticsearch snapshot repository to use
 
     :type client: :py:class:`~.elasticsearch.Elasticsearch`
-    :type snapshot: str
     :type repository: str
 
-    :rtype: bool
+    :returns: The list of all snapshots from ``repository``
+    :rtype: list
     """
-    logger = logging.getLogger(__name__)
-    logger.debug('SNAPSHOT: %s', snapshot)
-    logger.debug('REPOSITORY: %s', repository)
+    if not repository:
+        raise MissingArgument('No value for "repository" provided')
     try:
-        result = client.snapshot.get(repository=repository, snapshot=snapshot)
-        logger.debug('RESULT: %s', result)
-    except Exception as err:
-        raise CuratorException(
-            f'Unable to obtain information for snapshot "{snapshot}" in repository '
-            f'"{repository}". Error: {err}'
-        ) from err
-    state = result['snapshots'][0]['state']
-    logger.debug('Snapshot state = %s', state)
-    retval = True
-    if state == 'IN_PROGRESS':
-        logger.info('Snapshot %s still in progress.', snapshot)
-        retval = False
-    elif state == 'SUCCESS':
-        logger.info('Snapshot %s successfully completed.', snapshot)
-    elif state == 'PARTIAL':
-        logger.warning('Snapshot %s completed with state PARTIAL.', snapshot)
-    elif state == 'FAILED':
-        logger.error('Snapshot %s completed with state FAILED.', snapshot)
-    else:
-        logger.warning('Snapshot %s completed with state: %s', snapshot, state)
-    return retval
+        return client.snapshot.get(repository=repository, snapshot="*")['snapshots']
+    except (es8exc.TransportError, es8exc.NotFoundError) as err:
+        msg = (
+            f'Unable to get snapshot information from repository: '
+            f'{repository}. Error: {err}'
+        )
+        raise FailedExecution(msg) from err
+
+def get_tier_preference(client, target_tier='data_frozen'):
+    """Do the tier preference thing in reverse order from coldest to hottest
+    Based on the value of ``target_tier``, build out the list to use.
 
-def task_check(client, task_id=None):
+    :param client: A client connection object
+    :param target_tier: The target data tier, e.g. data_warm.
+
+    :type client: :py:class:`~.elasticsearch.Elasticsearch`
+    :type target_tier: str
+
+    :returns: A suitable tier preference string in csv format
+    :rtype: str
     """
-    This function calls `client.tasks.` :py:meth:`~.elasticsearch.client.TasksClient.get` with the
-    provided ``task_id``.  If the task data contains ``'completed': True``, then it will return
-    ``True``. If the task is not completed, it will log some information about the task and return
-    ``False``
+    tiermap = {
+        'data_content': 0,
+        'data_hot': 1,
+        'data_warm': 2,
+        'data_cold': 3,
+        'data_frozen': 4,
+    }
+    tiers = get_data_tiers(client)
+    test_list = []
+    for tier in ['data_hot', 'data_warm', 'data_cold', 'data_frozen']:
+        if tier in tiers and tiermap[tier] <= tiermap[target_tier]:
+            test_list.insert(0, tier)
+    if target_tier == 'data_frozen':
+        # We're migrating to frozen here. If a frozen tier exists, frozen searchable snapshot
+        # mounts should only ever go to the frozen tier.
+        if 'data_frozen' in tiers and tiers['data_frozen']:
+            return 'data_frozen'
+    # If there are no  nodes with the 'data_frozen' role...
+    preflist = []
+    for key in test_list:
+        # This ordering ensures that colder tiers are prioritized
+        if key in tiers and tiers[key]:
+            preflist.append(key)
+    # If all of these are false, then we have no data tiers and must use 'data_content'
+    if not preflist:
+        return 'data_content'
+    # This will join from coldest to hottest as csv string, e.g. 'data_cold,data_warm,data_hot'
+    return ','.join(preflist)
+
+def get_write_index(client, alias):
+    """
+    Calls :py:meth:`~.elasticsearch.client.IndicesClient.get_alias`
 
     :param client: A client connection object
-    :param task_id: The task id
+    :param alias: An alias name
 
     :type client: :py:class:`~.elasticsearch.Elasticsearch`
-    :type task_id: str
+    :type alias: str
 
-    :rtype: bool
+    :returns: The the index name associated with the alias that is designated ``is_write_index``
+    :rtype: str
     """
-    logger = logging.getLogger(__name__)
     try:
-        task_data = client.tasks.get(task_id=task_id)
-    except Exception as err:
-        msg = f'Unable to obtain task information for task_id "{task_id}". Exception {err}'
-        raise CuratorException(msg) from err
-    task = task_data['task']
-    completed = task_data['completed']
-    if task['action'] == 'indices:data/write/reindex':
-        logger.debug('It\'s a REINDEX TASK')
-        logger.debug('TASK_DATA: %s', task_data)
-        logger.debug('TASK_DATA keys: %s', list(task_data.keys()))
-        if 'response' in task_data:
-            response = task_data['response']
-            if response['failures']:
-                msg = f'Failures found in reindex response: {response["failures"]}'
-                raise FailedReindex(msg)
-    running_time = 0.000000001 * task['running_time_in_nanos']
-    logger.debug('Running time: %s seconds', running_time)
-    descr = task['description']
-
-    if completed:
-        completion_time = ((running_time * 1000) + task['start_time_in_millis'])
-        time_string = strftime('%Y-%m-%dT%H:%M:%SZ', localtime(completion_time/1000))
-        logger.info('Task "%s" completed at %s.', descr, time_string)
-        retval = True
+        response = client.indices.get_alias(index=alias)
+    except Exception as exc:
+        raise CuratorException(f'Alias {alias} not found') from exc
+    # If there are more than one in the list, one needs to be the write index
+    # otherwise the alias is a one to many, and can't do rollover.
+    if len(list(response.keys())) > 1:
+        for index in list(response.keys()):
+            try:
+                if response[index]['aliases'][alias]['is_write_index']:
+                    return index
+            except KeyError as exc:
+                raise FailedExecution(
+                    'Invalid alias: is_write_index not found in 1 to many alias') from exc
     else:
-        # Log the task status here.
-        logger.debug('Full Task Data: %s', task_data)
-        msg = (
-            f'Task "{descr}" with task_id "{task_id}" has been running for {running_time} seconds'
-        )
-        logger.info(msg)
-        retval = False
-    return retval
+        # There's only one, so this is it
+        return list(response.keys())[0]
 
-# pylint: disable=too-many-locals, too-many-arguments
-def wait_for_it(
-        client, action, task_id=None, snapshot=None, repository=None, index=None, index_list=None,
-        wait_interval=9, max_wait=-1
-    ):
-    """
-    This function becomes one place to do all ``wait_for_completion`` type behaviors
+def index_size(client, idx, value='total'):
+    """
+    Calls :py:meth:`~.elasticsearch.client.IndicesClient.stats`
 
     :param client: A client connection object
-    :param action: The action name that will identify how to wait
-    :param task_id: If the action provided a task_id, this is where it must be declared.
-    :param snapshot: The name of the snapshot.
-    :param repository: The Elasticsearch snapshot repository to use
-    :param wait_interval: Seconds to wait between completion checks.
-    :param max_wait: Maximum number of seconds to ``wait_for_completion``
+    :param idx: An index name
+    :param value: One of either ``primaries`` or ``total``
 
     :type client: :py:class:`~.elasticsearch.Elasticsearch`
-    :type action: str
-    :type task_id: str
-    :type snapshot: str
-    :type repository: str
-    :type wait_interval: int
-    :type max_wait: int
-    :rtype: None
+    :type idx: str
+    :type value: str
+
+    :returns: The sum of either ``primaries`` or ``total`` shards for index ``idx``
+    :rtype: integer
+    """
+    return client.indices.stats(index=idx)['indices'][idx][value]['store']['size_in_bytes']
+
+def name_to_node_id(client, name):
+    """
+    Calls :py:meth:`~.elasticsearch.client.NodesClient.stats`
+
+    :param client: A client connection object
+    :param name: The node ``name``
+
+    :type client: :py:class:`~.elasticsearch.Elasticsearch`
+    :type name: str
+
+    :returns: The node_id of the node identified by ``name``
+    :rtype: str
     """
     logger = logging.getLogger(__name__)
-    action_map = {
-        'allocation':{'function': health_check, 'args': {'relocating_shards':0}},
-        'replicas':{'function': health_check, 'args': {'status':'green'}},
-        'cluster_routing':{'function': health_check, 'args': {'relocating_shards':0}},
-        'snapshot':{
-            'function':snapshot_check, 'args':{'snapshot':snapshot, 'repository':repository}},
-        'restore':{'function':restore_check, 'args':{'index_list':index_list}},
-        'reindex':{'function':task_check, 'args':{'task_id':task_id}},
-        'shrink':{'function': health_check, 'args': {'status':'green'}},
-        'relocate':{'function': relocate_check, 'args': {'index':index}},
-    }
-    wait_actions = list(action_map.keys())
+    stats = client.nodes.stats()
+    for node in stats['nodes']:
+        if stats['nodes'][node]['name'] == name:
+            logger.debug('Found node_id "%s" for name "%s".', node, name)
+            return node
+    logger.error('No node_id found matching name: "%s"', name)
+    return None
 
-    if action not in wait_actions:
-        raise ConfigurationError(f'"action" must be one of {wait_actions}')
-    if action == 'reindex' and task_id is None:
-        raise MissingArgument(f'A task_id must accompany "action" {action}')
-    if action == 'snapshot' and ((snapshot is None) or (repository is None)):
-        raise MissingArgument(
-            f'A snapshot and repository must accompany "action" {action}. snapshot: '
-            f'{snapshot}, repository: {repository}'
-        )
-    if action == 'restore' and index_list is None:
-        raise MissingArgument(f'An index_list must accompany "action" {action}')
-    if action == 'reindex':
-        try:
-            _ = client.tasks.get(task_id=task_id)
-        except Exception as err:
-            # This exception should only exist in API usage. It should never
-            # occur in regular Curator usage.
-            raise CuratorException(f'Unable to find task_id {task_id}. Exception: {err}') from err
-
-    # Now with this mapped, we can perform the wait as indicated.
-    start_time = datetime.now()
-    result = False
-    while True:
-        elapsed = int((datetime.now() - start_time).total_seconds())
-        logger.debug('Elapsed time: %s seconds', elapsed)
-        response = action_map[action]['function'](client, **action_map[action]['args'])
-        logger.debug('Response: %s', response)
-        # Success
-        if response:
-            logger.debug(
-                'Action "%s" finished executing (may or may not have been successful)', action)
-            result = True
-            break
-        # Not success, and reached maximum wait (if defined)
-        if (max_wait != -1) and (elapsed >= max_wait):
-            msg = f'Unable to complete action "{action}" within max_wait ({max_wait}) seconds.'
-            logger.error(msg)
-            break
-        # Not success, so we wait.
-        msg = (
-            f'Action "{action}" not yet complete, {elapsed} total seconds elapsed. '
-            f'Waiting {wait_interval} seconds before checking again.'
-        )
-        logger.debug(msg)
-        sleep(wait_interval)
+def node_id_to_name(client, node_id):
+    """
+    Calls :py:meth:`~.elasticsearch.client.NodesClient.stats`
 
-    logger.debug('Result: %s', result)
-    if not result:
-        raise ActionTimeout(
-            f'Action "{action}" failed to complete in the max_wait period of {max_wait} seconds'
-        )
+    :param client: A client connection object
+    :param node_id: The node ``node_id``
+
+    :type client: :py:class:`~.elasticsearch.Elasticsearch`
+    :type node_id: str
+
+    :returns: The name of the node identified by ``node_id``
+    :rtype: str
+    """
+    logger = logging.getLogger(__name__)
+    stats = client.nodes.stats()
+    name = None
+    if node_id in stats['nodes']:
+        name = stats['nodes'][node_id]['name']
+    else:
+        logger.error('No node_id found matching: "%s"', node_id)
+    logger.debug('Name associated with node_id "%s": %s', node_id, name)
+    return name
+
+def node_roles(client, node_id):
+    """
+    Calls :py:meth:`~.elasticsearch.client.NodesClient.info`
+
+    :param client: A client connection object
+    :param node_id: The node ``node_id``
+
+    :type client: :py:class:`~.elasticsearch.Elasticsearch`
+    :type node_id: str
+
+    :returns: The list of roles assigned to the node identified by ``node_id``
+    :rtype: list
+    """
+    return client.nodes.info()['nodes'][node_id]['roles']
+
+def single_data_path(client, node_id):
+    """
+    In order for a shrink to work, it should be on a single filesystem, as shards cannot span
+    filesystems. Calls :py:meth:`~.elasticsearch.client.NodesClient.stats`
+
+    :param client: A client connection object
+    :param node_id: The node ``node_id``
+
+    :type client: :py:class:`~.elasticsearch.Elasticsearch`
+    :type node_id: str
+
+    :returns: ``True`` if the node has a single filesystem, else ``False``
+    :rtype: bool
+    """
+    return len(client.nodes.stats()['nodes'][node_id]['fs']['data']) == 1
```

### Comparing `elasticsearch_curator-8.0.3/curator/validators/actions.py` & `elasticsearch_curator-8.0.4/curator/validators/actions.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.3/curator/validators/filter_functions.py` & `elasticsearch_curator-8.0.4/curator/validators/filter_functions.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.3/curator/validators/options.py` & `elasticsearch_curator-8.0.4/curator/validators/options.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.3/curator/validators/schemacheck.py` & `elasticsearch_curator-8.0.4/curator/validators/schemacheck.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.3/LICENSE` & `elasticsearch_curator-8.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.3/NOTICE` & `elasticsearch_curator-8.0.4/NOTICE`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.3/README.rst` & `elasticsearch_curator-8.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `elasticsearch_curator-8.0.3/pyproject.toml` & `elasticsearch_curator-8.0.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 keywords = [
     'elasticsearch',
     'time-series',
     'indexed',
     'index-expiry'
 ]
 dependencies = [
-    "elasticsearch8==8.6.2",
-    "es_client==8.6.2",
+    "elasticsearch8==8.7.0",
+    "es_client==8.7.0",
     "ecs-logging==2.0.0",
     "click==8.1.3",
     "pyyaml==6.0.0",
     "voluptuous>=0.13.1",
     "certifi>=2022.12.7",
     "six>=1.16.0",
 ]
@@ -99,15 +99,15 @@
 step4 = "step3 ; echo 'Tests complete! Destroying Docker test environment...' "
 full = "step4 ; $(docker_test/scripts/destroy.sh 2&>1 /dev/null ) ;  exit $EXITCODE"
 run-coverage = "pytest --cov-config=pyproject.toml --cov=curator --cov=tests"
 run = "run-coverage --no-cov"
 
 [[tool.hatch.envs.test.matrix]]
 python = ["3.9", "3.10", "3.11"]
-version = ["8.0.2"]
+version = ["8.0.4"]
 
 [tool.pytest.ini_options]
 pythonpath = [".", "curator"]
 minversion = "7.2"
 addopts = "-ra -q"
 testpaths = [
     "tests/unit",
```

### Comparing `elasticsearch_curator-8.0.3/PKG-INFO` & `elasticsearch_curator-8.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elasticsearch-curator
-Version: 8.0.3
+Version: 8.0.4
 Summary: Tending your Elasticsearch indices and snapshots
 Project-URL: Homepage, https://github.com/elastic/curator
 Project-URL: Bug Tracker, https://github.com/elastic/curator/issues
 Author-email: Elastic <info@elastic.co>
 License: Apache-2.0
 License-File: LICENSE
 License-File: NOTICE
@@ -18,16 +18,16 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Requires-Dist: certifi>=2022.12.7
 Requires-Dist: click==8.1.3
 Requires-Dist: ecs-logging==2.0.0
-Requires-Dist: elasticsearch8==8.6.2
-Requires-Dist: es-client==8.6.2
+Requires-Dist: elasticsearch8==8.7.0
+Requires-Dist: es-client==8.7.0
 Requires-Dist: pyyaml==6.0.0
 Requires-Dist: six>=1.16.0
 Requires-Dist: voluptuous>=0.13.1
 Provides-Extra: doc
 Requires-Dist: sphinx; extra == 'doc'
 Requires-Dist: sphinx-rtd-theme; extra == 'doc'
 Provides-Extra: test
```

