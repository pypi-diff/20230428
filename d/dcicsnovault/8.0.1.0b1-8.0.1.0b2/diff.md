# Comparing `tmp/dcicsnovault-8.0.1.0b1.tar.gz` & `tmp/dcicsnovault-8.0.1.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcicsnovault-8.0.1.0b1.tar", max compression
+gzip compressed data, was "dcicsnovault-8.0.1.0b2.tar", max compression
```

## Comparing `dcicsnovault-8.0.1.0b1.tar` & `dcicsnovault-8.0.1.0b2.tar`

### file list

```diff
@@ -1,153 +1,160 @@
--rw-r--r--   0        0        0     1135 2023-04-28 15:14:06.848052 dcicsnovault-8.0.1.0b1/LICENSE.txt
--rw-r--r--   0        0        0     6407 2023-04-28 15:14:06.848052 dcicsnovault-8.0.1.0b1/README.rst
--rw-r--r--   0        0        0     5597 2023-04-28 15:14:06.852052 dcicsnovault-8.0.1.0b1/pyproject.toml
--rw-r--r--   0        0        0     4586 2023-04-28 15:14:06.852052 dcicsnovault-8.0.1.0b1/snovault/__init__.py
--rw-r--r--   0        0        0     1942 2023-04-28 15:14:06.852052 dcicsnovault-8.0.1.0b1/snovault/aggregated_items.py
--rw-r--r--   0        0        0     8799 2023-04-28 15:14:06.852052 dcicsnovault-8.0.1.0b1/snovault/app.py
--rw-r--r--   0        0        0    11879 2023-04-28 15:14:06.852052 dcicsnovault-8.0.1.0b1/snovault/attachment.py
--rw-r--r--   0        0        0    25327 2023-04-28 15:14:06.852052 dcicsnovault-8.0.1.0b1/snovault/authentication.py
--rw-r--r--   0        0        0     4467 2023-04-28 15:14:06.852052 dcicsnovault-8.0.1.0b1/snovault/authorization.py
--rw-r--r--   0        0        0     6670 2023-04-28 15:14:06.852052 dcicsnovault-8.0.1.0b1/snovault/batchupgrade.py
--rw-r--r--   0        0        0     1902 2023-04-28 15:14:06.852052 dcicsnovault-8.0.1.0b1/snovault/cache.py
--rw-r--r--   0        0        0     6461 2023-04-28 15:14:06.852052 dcicsnovault-8.0.1.0b1/snovault/calculated.py
--rw-r--r--   0        0        0       10 2023-04-28 15:14:06.852052 dcicsnovault-8.0.1.0b1/snovault/commands/__init__.py
--rw-r--r--   0        0        0     3416 2023-04-28 15:14:06.852052 dcicsnovault-8.0.1.0b1/snovault/commands/check_rendering.py
--rw-r--r--   0        0        0     6813 2023-04-28 15:14:06.852052 dcicsnovault-8.0.1.0b1/snovault/commands/clear_db_es_contents.py
--rw-r--r--   0        0        0     3928 2023-04-28 15:14:06.852052 dcicsnovault-8.0.1.0b1/snovault/commands/create_mapping_on_deploy.py
--rw-r--r--   0        0        0     1608 2023-04-28 15:14:06.852052 dcicsnovault-8.0.1.0b1/snovault/commands/es_index_data.py
--rw-r--r--   0        0        0     1644 2023-04-28 15:14:06.852052 dcicsnovault-8.0.1.0b1/snovault/commands/jsonld_rdf.py
--rw-r--r--   0        0        0     6212 2023-04-28 15:14:06.852052 dcicsnovault-8.0.1.0b1/snovault/commands/load_access_keys.py
--rw-r--r--   0        0        0     2402 2023-04-28 15:14:06.852052 dcicsnovault-8.0.1.0b1/snovault/commands/load_data.py
--rw-r--r--   0        0        0     2188 2023-04-28 15:14:06.852052 dcicsnovault-8.0.1.0b1/snovault/commands/load_data_by_type.py
--rw-r--r--   0        0        0     4350 2023-04-28 15:14:06.852052 dcicsnovault-8.0.1.0b1/snovault/commands/profile.py
--rw-r--r--   0        0        0     3236 2023-04-28 15:14:06.852052 dcicsnovault-8.0.1.0b1/snovault/commands/purge_item_type.py
--rw-r--r--   0        0        0     1868 2023-04-28 15:14:06.852052 dcicsnovault-8.0.1.0b1/snovault/commands/run_upgrader_on_inserts.py
--rw-r--r--   0        0        0     8533 2023-04-28 15:14:06.852052 dcicsnovault-8.0.1.0b1/snovault/commands/update_inserts_from_server.py
--rw-r--r--   0        0        0      909 2023-04-28 15:14:06.852052 dcicsnovault-8.0.1.0b1/snovault/commands/wipe_test_indices.py
--rw-r--r--   0        0        0     4183 2023-04-28 15:14:06.852052 dcicsnovault-8.0.1.0b1/snovault/config.py
--rw-r--r--   0        0        0     6352 2023-04-28 15:14:06.852052 dcicsnovault-8.0.1.0b1/snovault/connection.py
--rw-r--r--   0        0        0    14798 2023-04-28 15:14:06.852052 dcicsnovault-8.0.1.0b1/snovault/crud_views.py
--rw-r--r--   0        0        0    15301 2023-04-28 15:14:06.852052 dcicsnovault-8.0.1.0b1/snovault/custom_embed.py
--rw-r--r--   0        0        0     7216 2023-04-28 15:14:06.852052 dcicsnovault-8.0.1.0b1/snovault/dev_servers.py
--rw-r--r--   0        0        0     4340 2023-04-28 15:14:06.852052 dcicsnovault-8.0.1.0b1/snovault/drs.py
--rw-r--r--   0        0        0     1829 2023-04-28 15:14:06.852052 dcicsnovault-8.0.1.0b1/snovault/edw_hash.py
--rw-r--r--   0        0        0     4282 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/elasticsearch/__init__.py
--rw-r--r--   0        0        0     4727 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/elasticsearch/cached_views.py
--rw-r--r--   0        0        0    61320 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/elasticsearch/create_mapping.py
--rw-r--r--   0        0        0     7939 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/elasticsearch/es_index_listener.py
--rw-r--r--   0        0        0    18572 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/elasticsearch/esstorage.py
--rw-r--r--   0        0        0    24405 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/elasticsearch/indexer.py
--rw-r--r--   0        0        0    31356 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/elasticsearch/indexer_queue.py
--rw-r--r--   0        0        0    20947 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/elasticsearch/indexer_utils.py
--rw-r--r--   0        0        0      349 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/elasticsearch/interfaces.py
--rw-r--r--   0        0        0    10190 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/elasticsearch/mpindexer.py
--rw-r--r--   0        0        0     8249 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/embed.py
--rw-r--r--   0        0        0     1061 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/etag.py
--rw-r--r--   0        0        0    10835 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/indexing_views.py
--rw-r--r--   0        0        0      774 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/interfaces.py
--rw-r--r--   0        0        0     2229 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/invalidation.py
--rw-r--r--   0        0        0     1639 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/json_renderer.py
--rw-r--r--   0        0        0     2292 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/jsongraph.py
--rw-r--r--   0        0        0     9713 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/jsonld_context.py
--rw-r--r--   0        0        0    30294 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/loadxl.py
--rw-r--r--   0        0        0     2425 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/memlimit.py
--rw-r--r--   0        0        0     1165 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/parallel.py
--rw-r--r--   0        0        0      846 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/predicates.py
--rw-r--r--   0        0        0       95 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/redis/README.rst
--rw-r--r--   0        0        0       90 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/redis/__init__.py
--rw-r--r--   0        0        0       16 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/redis/interfaces.py
--rw-r--r--   0        0        0     4106 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/redis/redis_connection.py
--rw-r--r--   0        0        0    22128 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/renderers.py
--rw-r--r--   0        0        0    11201 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/resource_views.py
--rw-r--r--   0        0        0    21863 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/resources.py
--rw-r--r--   0        0        0     3450 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/schema_graph.py
--rw-r--r--   0        0        0    14162 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/schema_utils.py
--rw-r--r--   0        0        0     4358 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/schema_views.py
--rw-r--r--   0        0        0     1855 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/schemas/access_key.json
--rw-r--r--   0        0        0     5098 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/schemas/filter_set.json
--rw-r--r--   0        0        0    18744 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/schemas/mixins.json
--rw-r--r--   0        0        0    19600 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/schemas/user.json
--rw-r--r--   0        0        0    20952 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/search/compound_search.py
--rw-r--r--   0        0        0    58595 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/search/lucene_builder.py
--rw-r--r--   0        0        0    62789 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/search/search.py
--rw-r--r--   0        0        0    17901 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/search/search_utils.py
--rw-r--r--   0        0        0     4541 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/server_defaults.py
--rw-r--r--   0        0        0      522 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/settings.py
--rw-r--r--   0        0        0     1498 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/standalone_dev.py
--rw-r--r--   0        0        0     4383 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/stats.py
--rw-r--r--   0        0        0    34834 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/storage.py
--rw-r--r--   0        0        0      330 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/test_schemas/AbstractItemTestSecondSubItem.json
--rw-r--r--   0        0        0      300 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/test_schemas/AbstractItemTestSubItem.json
--rw-r--r--   0        0        0     2467 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/test_schemas/EmbeddingTest.json
--rw-r--r--   0        0        0      446 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/test_schemas/NestedEmbeddingContainer.json
--rw-r--r--   0        0        0      883 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/test_schemas/NestedObjectLinkTarget.json
--rw-r--r--   0        0        0      473 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/test_schemas/TestingBiogroupSno.json
--rw-r--r--   0        0        0      968 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/test_schemas/TestingBiosampleSno.json
--rw-r--r--   0        0        0     1082 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/test_schemas/TestingBiosourceSno.json
--rw-r--r--   0        0        0      894 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/test_schemas/TestingCalculatedProperties.json
--rw-r--r--   0        0        0      276 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/test_schemas/TestingDependencies.json
--rw-r--r--   0        0        0      697 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/test_schemas/TestingDownload.json
--rw-r--r--   0        0        0      555 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/test_schemas/TestingIndividualSno.json
--rw-r--r--   0        0        0      730 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/test_schemas/TestingLinkAggregateSno.json
--rw-r--r--   0        0        0      697 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/test_schemas/TestingLinkSourceSno.json
--rw-r--r--   0        0        0      472 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/test_schemas/TestingLinkTargetElasticSearch.json
--rw-r--r--   0        0        0      292 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/test_schemas/TestingLinkTargetSno.json
--rw-r--r--   0        0        0      311 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/test_schemas/TestingMixins.json
--rw-r--r--   0        0        0      845 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/test_schemas/TestingNestedEnabled.json
--rw-r--r--   0        0        0     3721 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/test_schemas/TestingNoteSno.json
--rw-r--r--   0        0        0     1622 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/test_schemas/TestingPostPutPatchSno.json
--rw-r--r--   0        0        0      576 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/test_schemas/TestingServerDefault.json
--rw-r--r--   0        0        0     1215 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/test_schemas/mixins.json
--rw-r--r--   0        0        0        0 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/__init__.py
--rw-r--r--   0        0        0     2210 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/conftest.py
--rw-r--r--   0        0        0      100 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/conftest_settings.py
--rw-r--r--   0        0        0     3086 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/elasticsearch_fixture.py
--rw-r--r--   0        0        0     3921 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/postgresql_fixture.py
--rw-r--r--   0        0        0      852 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/pyramidfixtures.py
--rw-r--r--   0        0        0     3007 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/root.py
--rw-r--r--   0        0        0    17313 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/serverfixtures.py
--rw-r--r--   0        0        0    20332 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/test_attachment.py
--rw-r--r--   0        0        0     3937 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/test_authentication.py
--rw-r--r--   0        0        0     1370 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/test_calculated.py
--rw-r--r--   0        0        0    15979 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/test_clear_db_es_contents.py
--rw-r--r--   0        0        0     8984 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/test_create_mapping.py
--rw-r--r--   0        0        0     3173 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/test_drs.py
--rw-r--r--   0        0        0      528 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/test_edw_hash.py
--rw-r--r--   0        0        0     7493 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/test_embed_utils.py
--rw-r--r--   0        0        0     8823 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/test_embedding.py
--rw-r--r--   0        0        0    10024 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/test_es_permissions.py
--rw-r--r--   0        0        0   115140 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/test_indexing.py
--rw-r--r--   0        0        0    28258 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/test_invalidation_scope.py
--rw-r--r--   0        0        0     1808 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/test_key.py
--rw-r--r--   0        0        0     2458 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/test_link.py
--rw-r--r--   0        0        0     5316 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/test_logging.py
--rw-r--r--   0        0        0     1134 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/test_misc.py
--rw-r--r--   0        0        0      373 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/test_mixins.py
--rw-r--r--   0        0        0    13660 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/test_post_put_patch.py
--rw-r--r--   0        0        0     1570 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/test_postgresql_fixture.py
--rw-r--r--   0        0        0     1194 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/test_schemas.py
--rw-r--r--   0        0        0      952 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/test_serverfixtures.py
--rw-r--r--   0        0        0     4267 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/test_standalone_dev.py
--rw-r--r--   0        0        0     2211 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/test_stats.py
--rw-r--r--   0        0        0    13182 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/test_storage.py
--rw-r--r--   0        0        0     6782 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/test_types_access_key.py
--rw-r--r--   0        0        0     1291 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/test_upgrader.py
--rw-r--r--   0        0        0     6635 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/test_util.py
--rw-r--r--   0        0        0    18612 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/test_views.py
--rw-r--r--   0        0        0     4578 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/testappfixtures.py
--rw-r--r--   0        0        0      677 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/testing_upgrader.py
--rw-r--r--   0        0        0    34107 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/testing_views.py
--rw-r--r--   0        0        0     1342 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/toolfixtures.py
--rw-r--r--   0        0        0     4031 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tools.py
--rw-r--r--   0        0        0     1807 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/typedsheets.py
--rw-r--r--   0        0        0     7605 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/typeinfo.py
--rw-r--r--   0        0        0       70 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/types/__init__.py
--rw-r--r--   0        0        0     5101 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/types/access_key.py
--rw-r--r--   0        0        0    16288 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/types/base.py
--rw-r--r--   0        0        0      738 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/types/filter_set.py
--rw-r--r--   0        0        0     5536 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/types/user.py
--rw-r--r--   0        0        0     8124 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/upgrader.py
--rw-r--r--   0        0        0    51788 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/util.py
--rw-r--r--   0        0        0     5460 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/validation.py
--rw-r--r--   0        0        0     5718 2023-04-28 15:14:06.864052 dcicsnovault-8.0.1.0b1/snovault/validators.py
--rw-r--r--   0        0        0     9135 1970-01-01 00:00:00.000000 dcicsnovault-8.0.1.0b1/PKG-INFO
+-rw-r--r--   0        0        0     1135 2023-04-28 17:25:54.473943 dcicsnovault-8.0.1.0b2/LICENSE.txt
+-rw-r--r--   0        0        0     6407 2023-04-28 17:25:54.473943 dcicsnovault-8.0.1.0b2/README.rst
+-rw-r--r--   0        0        0     5506 2023-04-28 17:25:54.477943 dcicsnovault-8.0.1.0b2/pyproject.toml
+-rw-r--r--   0        0        0     4586 2023-04-28 17:25:54.477943 dcicsnovault-8.0.1.0b2/snovault/__init__.py
+-rw-r--r--   0        0        0     1942 2023-04-28 17:25:54.477943 dcicsnovault-8.0.1.0b2/snovault/aggregated_items.py
+-rw-r--r--   0        0        0     8799 2023-04-28 17:25:54.477943 dcicsnovault-8.0.1.0b2/snovault/app.py
+-rw-r--r--   0        0        0    11879 2023-04-28 17:25:54.477943 dcicsnovault-8.0.1.0b2/snovault/attachment.py
+-rw-r--r--   0        0        0    25327 2023-04-28 17:25:54.477943 dcicsnovault-8.0.1.0b2/snovault/authentication.py
+-rw-r--r--   0        0        0     4467 2023-04-28 17:25:54.477943 dcicsnovault-8.0.1.0b2/snovault/authorization.py
+-rw-r--r--   0        0        0     6670 2023-04-28 17:25:54.477943 dcicsnovault-8.0.1.0b2/snovault/batchupgrade.py
+-rw-r--r--   0        0        0     1902 2023-04-28 17:25:54.477943 dcicsnovault-8.0.1.0b2/snovault/cache.py
+-rw-r--r--   0        0        0     6461 2023-04-28 17:25:54.477943 dcicsnovault-8.0.1.0b2/snovault/calculated.py
+-rw-r--r--   0        0        0       10 2023-04-28 17:25:54.477943 dcicsnovault-8.0.1.0b2/snovault/commands/__init__.py
+-rw-r--r--   0        0        0     3416 2023-04-28 17:25:54.477943 dcicsnovault-8.0.1.0b2/snovault/commands/check_rendering.py
+-rw-r--r--   0        0        0     6813 2023-04-28 17:25:54.477943 dcicsnovault-8.0.1.0b2/snovault/commands/clear_db_es_contents.py
+-rw-r--r--   0        0        0     3928 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/commands/create_mapping_on_deploy.py
+-rw-r--r--   0        0        0     1608 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/commands/es_index_data.py
+-rw-r--r--   0        0        0     1644 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/commands/jsonld_rdf.py
+-rw-r--r--   0        0        0     5764 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/commands/list_db_tables.py
+-rw-r--r--   0        0        0     6212 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/commands/load_access_keys.py
+-rw-r--r--   0        0        0     2402 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/commands/load_data.py
+-rw-r--r--   0        0        0     2188 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/commands/load_data_by_type.py
+-rw-r--r--   0        0        0     5155 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/commands/prepare_template.py
+-rw-r--r--   0        0        0     4350 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/commands/profile.py
+-rw-r--r--   0        0        0     3236 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/commands/purge_item_type.py
+-rw-r--r--   0        0        0     1868 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/commands/run_upgrader_on_inserts.py
+-rw-r--r--   0        0        0     8533 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/commands/update_inserts_from_server.py
+-rw-r--r--   0        0        0      909 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/commands/wipe_test_indices.py
+-rw-r--r--   0        0        0     4183 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/config.py
+-rw-r--r--   0        0        0     6352 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/connection.py
+-rw-r--r--   0        0        0    14798 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/crud_views.py
+-rw-r--r--   0        0        0    15301 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/custom_embed.py
+-rw-r--r--   0        0        0     7228 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/dev_servers.py
+-rw-r--r--   0        0        0     4340 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/drs.py
+-rw-r--r--   0        0        0     1829 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/edw_hash.py
+-rw-r--r--   0        0        0     4282 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/elasticsearch/__init__.py
+-rw-r--r--   0        0        0     4727 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/elasticsearch/cached_views.py
+-rw-r--r--   0        0        0    61320 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/elasticsearch/create_mapping.py
+-rw-r--r--   0        0        0     7939 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/elasticsearch/es_index_listener.py
+-rw-r--r--   0        0        0    18572 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/elasticsearch/esstorage.py
+-rw-r--r--   0        0        0    24405 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/elasticsearch/indexer.py
+-rw-r--r--   0        0        0    31356 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/elasticsearch/indexer_queue.py
+-rw-r--r--   0        0        0    20947 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/elasticsearch/indexer_utils.py
+-rw-r--r--   0        0        0      349 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/elasticsearch/interfaces.py
+-rw-r--r--   0        0        0    10190 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/elasticsearch/mpindexer.py
+-rw-r--r--   0        0        0     8249 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/embed.py
+-rw-r--r--   0        0        0     1061 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/etag.py
+-rw-r--r--   0        0        0    10835 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/indexing_views.py
+-rw-r--r--   0        0        0      774 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/interfaces.py
+-rw-r--r--   0        0        0     2229 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/invalidation.py
+-rw-r--r--   0        0        0     1639 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/json_renderer.py
+-rw-r--r--   0        0        0     2292 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/jsongraph.py
+-rw-r--r--   0        0        0     9713 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/jsonld_context.py
+-rw-r--r--   0        0        0    30350 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/loadxl.py
+-rw-r--r--   0        0        0     2425 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/memlimit.py
+-rw-r--r--   0        0        0      895 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/nginx-dev.conf
+-rw-r--r--   0        0        0     1165 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/parallel.py
+-rw-r--r--   0        0        0      846 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/predicates.py
+-rw-r--r--   0        0        0     1095 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/project.py
+-rw-r--r--   0        0        0       95 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/redis/README.rst
+-rw-r--r--   0        0        0       90 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/redis/__init__.py
+-rw-r--r--   0        0        0       16 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/redis/interfaces.py
+-rw-r--r--   0        0        0     4106 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/redis/redis_connection.py
+-rw-r--r--   0        0        0    22128 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/renderers.py
+-rw-r--r--   0        0        0    11201 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/resource_views.py
+-rw-r--r--   0        0        0    21863 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/resources.py
+-rw-r--r--   0        0        0     3450 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/schema_graph.py
+-rw-r--r--   0        0        0    14547 2023-04-28 17:25:54.481943 dcicsnovault-8.0.1.0b2/snovault/schema_utils.py
+-rw-r--r--   0        0        0     4358 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/schema_views.py
+-rw-r--r--   0        0        0     1855 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/schemas/access_key.json
+-rw-r--r--   0        0        0     5098 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/schemas/filter_set.json
+-rw-r--r--   0        0        0    18744 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/schemas/mixins.json
+-rw-r--r--   0        0        0    19600 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/schemas/user.json
+-rw-r--r--   0        0        0    20952 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/search/compound_search.py
+-rw-r--r--   0        0        0    58595 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/search/lucene_builder.py
+-rw-r--r--   0        0        0    62789 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/search/search.py
+-rw-r--r--   0        0        0    17901 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/search/search_utils.py
+-rw-r--r--   0        0        0     4541 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/server_defaults.py
+-rw-r--r--   0        0        0      522 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/settings.py
+-rw-r--r--   0        0        0     1769 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/sqlalchemy_tools.py
+-rw-r--r--   0        0        0     1498 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/standalone_dev.py
+-rw-r--r--   0        0        0     4383 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/stats.py
+-rw-r--r--   0        0        0    34834 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/storage.py
+-rw-r--r--   0        0        0      330 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/test_schemas/AbstractItemTestSecondSubItem.json
+-rw-r--r--   0        0        0      300 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/test_schemas/AbstractItemTestSubItem.json
+-rw-r--r--   0        0        0     2467 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/test_schemas/EmbeddingTest.json
+-rw-r--r--   0        0        0      446 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/test_schemas/NestedEmbeddingContainer.json
+-rw-r--r--   0        0        0      883 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/test_schemas/NestedObjectLinkTarget.json
+-rw-r--r--   0        0        0      473 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/test_schemas/TestingBiogroupSno.json
+-rw-r--r--   0        0        0      968 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/test_schemas/TestingBiosampleSno.json
+-rw-r--r--   0        0        0     1082 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/test_schemas/TestingBiosourceSno.json
+-rw-r--r--   0        0        0      894 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/test_schemas/TestingCalculatedProperties.json
+-rw-r--r--   0        0        0      276 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/test_schemas/TestingDependencies.json
+-rw-r--r--   0        0        0      697 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/test_schemas/TestingDownload.json
+-rw-r--r--   0        0        0      555 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/test_schemas/TestingIndividualSno.json
+-rw-r--r--   0        0        0      730 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/test_schemas/TestingLinkAggregateSno.json
+-rw-r--r--   0        0        0      697 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/test_schemas/TestingLinkSourceSno.json
+-rw-r--r--   0        0        0      472 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/test_schemas/TestingLinkTargetElasticSearch.json
+-rw-r--r--   0        0        0      292 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/test_schemas/TestingLinkTargetSno.json
+-rw-r--r--   0        0        0      311 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/test_schemas/TestingMixins.json
+-rw-r--r--   0        0        0      845 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/test_schemas/TestingNestedEnabled.json
+-rw-r--r--   0        0        0     3721 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/test_schemas/TestingNoteSno.json
+-rw-r--r--   0        0        0     1622 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/test_schemas/TestingPostPutPatchSno.json
+-rw-r--r--   0        0        0      576 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/test_schemas/TestingServerDefault.json
+-rw-r--r--   0        0        0     1215 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/test_schemas/mixins.json
+-rw-r--r--   0        0        0        0 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/tests/__init__.py
+-rw-r--r--   0        0        0     2210 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/tests/conftest.py
+-rw-r--r--   0        0        0      100 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/tests/conftest_settings.py
+-rw-r--r--   0        0        0        0 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/tests/data/inserts/README.rst
+-rw-r--r--   0        0        0        0 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/tests/data/master-inserts/README.rst
+-rw-r--r--   0        0        0     3086 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/tests/elasticsearch_fixture.py
+-rw-r--r--   0        0        0     3921 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/tests/postgresql_fixture.py
+-rw-r--r--   0        0        0      852 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/tests/pyramidfixtures.py
+-rw-r--r--   0        0        0     3007 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/tests/root.py
+-rw-r--r--   0        0        0    17313 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/tests/serverfixtures.py
+-rw-r--r--   0        0        0    20332 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/tests/test_attachment.py
+-rw-r--r--   0        0        0     3937 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/tests/test_authentication.py
+-rw-r--r--   0        0        0     1370 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/tests/test_calculated.py
+-rw-r--r--   0        0        0    15979 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/tests/test_clear_db_es_contents.py
+-rw-r--r--   0        0        0     8984 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/tests/test_create_mapping.py
+-rw-r--r--   0        0        0     3173 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/tests/test_drs.py
+-rw-r--r--   0        0        0      528 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/tests/test_edw_hash.py
+-rw-r--r--   0        0        0     7493 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/tests/test_embed_utils.py
+-rw-r--r--   0        0        0     8823 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/tests/test_embedding.py
+-rw-r--r--   0        0        0    10024 2023-04-28 17:25:54.485942 dcicsnovault-8.0.1.0b2/snovault/tests/test_es_permissions.py
+-rw-r--r--   0        0        0   115140 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/tests/test_indexing.py
+-rw-r--r--   0        0        0    28258 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/tests/test_invalidation_scope.py
+-rw-r--r--   0        0        0     1808 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/tests/test_key.py
+-rw-r--r--   0        0        0     2458 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/tests/test_link.py
+-rw-r--r--   0        0        0     5316 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/tests/test_logging.py
+-rw-r--r--   0        0        0     1134 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/tests/test_misc.py
+-rw-r--r--   0        0        0      373 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/tests/test_mixins.py
+-rw-r--r--   0        0        0    13660 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/tests/test_post_put_patch.py
+-rw-r--r--   0        0        0     1570 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/tests/test_postgresql_fixture.py
+-rw-r--r--   0        0        0     1194 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/tests/test_schemas.py
+-rw-r--r--   0        0        0      952 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/tests/test_serverfixtures.py
+-rw-r--r--   0        0        0     4267 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/tests/test_standalone_dev.py
+-rw-r--r--   0        0        0     2211 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/tests/test_stats.py
+-rw-r--r--   0        0        0    13182 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/tests/test_storage.py
+-rw-r--r--   0        0        0     6782 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/tests/test_types_access_key.py
+-rw-r--r--   0        0        0     1291 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/tests/test_upgrader.py
+-rw-r--r--   0        0        0     6635 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/tests/test_util.py
+-rw-r--r--   0        0        0    18612 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/tests/test_views.py
+-rw-r--r--   0        0        0     4578 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/tests/testappfixtures.py
+-rw-r--r--   0        0        0      677 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/tests/testing_upgrader.py
+-rw-r--r--   0        0        0    34107 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/tests/testing_views.py
+-rw-r--r--   0        0        0     1342 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/tests/toolfixtures.py
+-rw-r--r--   0        0        0     4031 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/tools.py
+-rw-r--r--   0        0        0     1807 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/typedsheets.py
+-rw-r--r--   0        0        0     7605 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/typeinfo.py
+-rw-r--r--   0        0        0       70 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/types/__init__.py
+-rw-r--r--   0        0        0     5101 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/types/access_key.py
+-rw-r--r--   0        0        0    16288 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/types/base.py
+-rw-r--r--   0        0        0      738 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/types/filter_set.py
+-rw-r--r--   0        0        0     5536 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/types/user.py
+-rw-r--r--   0        0        0     8124 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/upgrader.py
+-rw-r--r--   0        0        0    51788 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/util.py
+-rw-r--r--   0        0        0     5460 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/validation.py
+-rw-r--r--   0        0        0     5718 2023-04-28 17:25:54.489943 dcicsnovault-8.0.1.0b2/snovault/validators.py
+-rw-r--r--   0        0        0     9182 1970-01-01 00:00:00.000000 dcicsnovault-8.0.1.0b2/PKG-INFO
```

### Comparing `dcicsnovault-8.0.1.0b1/LICENSE.txt` & `dcicsnovault-8.0.1.0b2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/README.rst` & `dcicsnovault-8.0.1.0b2/README.rst`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/pyproject.toml` & `dcicsnovault-8.0.1.0b2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dcicsnovault"
-version = "8.0.1.0b1"  # to become 8.1.0
+version = "8.0.1.0b2"  # to become 8.1.0
 description = "Storage support for 4DN Data Portals."
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/4dn-dcic/snovault"
 repository = "https://github.com/4dn-dcic/snovault"
 documentation = "https://github.com/4dn-dcic/snovault"
@@ -19,56 +19,56 @@
     'Development Status :: 4 - Beta',
 
     # Indicate who your project is intended for
     'Intended Audience :: Developers',
     'Intended Audience :: Science/Research',
     'Framework :: Pyramid',
 
-
     # Pick your license as you wish (should match "license" above)
     'License :: OSI Approved :: MIT License',
     'Topic :: Database :: Database Engines/Servers',
 
     # Specify the Python versions you support here. In particular, ensure
     # that you indicate whether you support Python 2, Python 3 or both.
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3.8',
+    'Programming Language :: Python :: 3.9',
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.10"
 aws_requests_auth = "^0.4.1"
-# TODO: This is a backport of Python's statistics library for versions earlier than Python 3.4,
-#       so may no longer be needed. Something to investigate later. -kmp 20-Feb-2020
-# "backports.statistics" = "0.1.0"
-botocore = ">=1.27.36"  # no particular version required, but this speeds up search
-boto3 = ">=1.24.36"  # no particular version required, but this speeds up search
+botocore = ">=1.19.119"  # no particular version required, but this speeds up search
+boto3 = ">=1.26.119"  # no particular version required, but this speeds up search
 elasticsearch = "7.13.4"  # versions >= 7.14.0 lock out AWS ES
 elasticsearch_dsl = "^7.4.0"
 dcicutils = "^7.0.0"
 future = ">=0.15.2,<1"
 html5lib = ">=1.1"  # experimental, should be OK now that we're not using moto server
 humanfriendly = "^1.44.9"
 jsonschema_serialize_fork = "^2.1.1"
 netaddr = ">=0.8.0,<1"
 passlib = "^1.7.4"
+pillow = "^9.5.0"
 psutil = "^5.9.0"
 psycopg2-binary = "^2.9.1"
 PyBrowserID = ">=0.10.0,<1"
+pyjwt = "^2.6.0"
 pyramid = "1.10.4"
 pyramid_localroles = ">=0.1,<1"
 pyramid-multiauth = ">=0.9.0,<1"
 pyramid-retry = "^1.0"
 pyramid-tm = "^2.5"
 pyramid-translogger = "^0.1"
 python-dateutil = "^2.8.2"
 python_magic = ">=0.4.27"
 pytz = ">=2021.3"
 rdflib = "^4.2.2"
 rdflib-jsonld = ">=0.5.0,<1.0.0"
+redis = "^4.5.1"
 rutter = ">=0.3,<1"
 simplejson = "^3.17.6"
 SPARQLWrapper = "^1.8.5"
 SQLAlchemy = "^1.4.41"  # portals pin 1.4.41, but we don't. should it matter? -kmp 6-Mar-2023
 # Our use of structlog is pretty vanilla, so we should be OK with changes across the 18-19 major version boundary.
 structlog = ">=19.2.0,<20"
 subprocess_middleware = ">=0.3,<1"
@@ -79,63 +79,70 @@
 WebOb = "^1.8.7"
 WebTest = "^2.0.35"
 WSGIProxy2 = "0.4.2"
 xlrd = "^1.0.0"
 "zope.deprecation" = "^4.4.0"
 "zope.interface" = ">=4.7.2,<6"
 "zope.sqlalchemy" = "1.6"
-pyjwt = "^2.6.0"
-pytest-redis = "^2.0.0"
-redis = "^4.5.1"
 
 [tool.poetry.dev-dependencies]
-botocore-stubs = ">=1.27.36"  # no particular version required, but this speeds up search
-boto3-stubs = ">=1.24.36"  # no particular version required, but this speeds up search
+botocore-stubs = ">=1.29.119"  # no particular version required, but this speeds up search
+boto3-stubs = ">=1.26.119"  # no particular version required, but this speeds up search
 coverage = ">=6.2"
 codacy-coverage = ">=1.3.11"
-coveralls = ">=3.3.1"
+# When we add coverage, this must be loaded manually in GA workflow for coverage because a dependency on 2to3
+# in its docopts dependency makes a problem for laoding it here in poetry. -kmp 25-Apr-2023
+# coveralls = ">=3.3.1"
 docutils = ">=0.16,<1"
 flake8 = ">=3.9.2"
 flaky = ">=3.7.0"
-# moto 2.0.0 (see https://github.com/spulec/moto/blob/master/CHANGELOG.md) has incompatibilities in how it needs
-# to be configured, so will require some adaptation. moto 1.3,14 will support python 3.8, but python 3.9 support
-# needs moto 2.2.5. If we do eventually upgrade, there are some tests in test_storage.py that may be possible to
-# simplify. -kmp 5-Feb-2022
-#
-# We tried 1.3.14 but it adds stuff we don't need (until Python 3.8) and it doesn't work as well.
-# See https://github.com/spulec/moto/blob/master/CHANGELOG.md
 moto = "^4.0.3"
+PasteDeploy = "1.5.2"
+plaster = "1.0"
+plaster-pastedeploy = "0.6"
 pipdeptree = ">=2.3.3"
-pip-licenses = "^3.5.3"
+# pip-licenses = ">=3.5.3"
 # Not even sure we need an explicit dependence on Pillow, though it might help keep from searching older versions.
 # -kmp 22-Feb-2022
 Pillow = ">=6.2.2"  # later version known to work - Will 11/17/20
 # Experimental upgrade to PyTest 4.5. It may be possible to upgrade further, but I think this is an improvement.
 # -kmp 11-May-2020
 pytest = "^7.2.2"
 pytest-cov = ">=2.2.1"
 # pytest_exact_fixtures = "^0.3"
 pytest-instafail = ">=0.3.0"
 # TODO: Investigate whether a major version upgrade is allowable for 'pytest-mock'.
 pytest-mock = ">=0.11.0"
+pytest-redis = "^2.0.0"
 # TODO: Investigate whether a major version upgrade is allowable for 'pytest-runner'.
 pytest-runner = ">=4.0"
 pytest-timeout = ">=1.0.0"
 # There was no version 4 of PyYAML. We upgraded today to PyYAML 5 per compatibility info in:
 # https://github.com/yaml/pyyaml/issues/265
 # We must have 5.1 to get the new yaml.safe_load method.
 # awscli appears to add its own restrictions, but our uses are pretty simple.
 # 5.2 had soe bugs that were probably only in Python 2, but we require 5.2 here just in case.
 # Any narrowing beyond that is just to help 'poetry lock' converge faster.
 # And we only need .safe_load in testing, so we're moving this to dev dependencies. -kmp 22-Feb-2022
 PyYAML = ">=5.1,<5.5"
 "repoze.debug" = ">=1.0.2"
-# Used only by moto, not explicitly by us.
-# responses = "^0.17.0"  # 0.17.0 is the last version compliant with Python 3.6
 wheel = ">=0.29.0"
 
 [tool.poetry.scripts]
+dev-servers = "snovault.dev_servers:main"
+list-db-tables = "snovault.commands.list_db_tables:main"
+prepare-local-dev = "snovault.commands.prepare_template:prepare_local_dev_main"
 wipe-test-indices = "snovault.commands.wipe_test_indices:main"
 
+[paste.app_factory]
+main = "snovault:main"
+
+[paste.composite_factory]
+indexer = "snovault.elasticsearch.es_index_listener:composite"
+# ingester = "encoded.ingestion_listener:composite"
+
+# [paste.filter_app_factory]
+# memlimit = "encoded.memlimit:filter_app"
+
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `dcicsnovault-8.0.1.0b1/snovault/__init__.py` & `dcicsnovault-8.0.1.0b2/snovault/__init__.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/aggregated_items.py` & `dcicsnovault-8.0.1.0b2/snovault/aggregated_items.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/app.py` & `dcicsnovault-8.0.1.0b2/snovault/app.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/attachment.py` & `dcicsnovault-8.0.1.0b2/snovault/attachment.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/authentication.py` & `dcicsnovault-8.0.1.0b2/snovault/authentication.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/authorization.py` & `dcicsnovault-8.0.1.0b2/snovault/authorization.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/batchupgrade.py` & `dcicsnovault-8.0.1.0b2/snovault/batchupgrade.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/cache.py` & `dcicsnovault-8.0.1.0b2/snovault/cache.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/calculated.py` & `dcicsnovault-8.0.1.0b2/snovault/calculated.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/commands/check_rendering.py` & `dcicsnovault-8.0.1.0b2/snovault/commands/check_rendering.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/commands/clear_db_es_contents.py` & `dcicsnovault-8.0.1.0b2/snovault/commands/clear_db_es_contents.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/commands/create_mapping_on_deploy.py` & `dcicsnovault-8.0.1.0b2/snovault/commands/create_mapping_on_deploy.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/commands/es_index_data.py` & `dcicsnovault-8.0.1.0b2/snovault/commands/es_index_data.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/commands/jsonld_rdf.py` & `dcicsnovault-8.0.1.0b2/snovault/commands/jsonld_rdf.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/commands/load_access_keys.py` & `dcicsnovault-8.0.1.0b2/snovault/commands/load_access_keys.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/commands/load_data.py` & `dcicsnovault-8.0.1.0b2/snovault/commands/load_data.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/commands/load_data_by_type.py` & `dcicsnovault-8.0.1.0b2/snovault/commands/load_data_by_type.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/commands/profile.py` & `dcicsnovault-8.0.1.0b2/snovault/commands/profile.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/commands/purge_item_type.py` & `dcicsnovault-8.0.1.0b2/snovault/commands/purge_item_type.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/commands/run_upgrader_on_inserts.py` & `dcicsnovault-8.0.1.0b2/snovault/commands/run_upgrader_on_inserts.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/commands/update_inserts_from_server.py` & `dcicsnovault-8.0.1.0b2/snovault/commands/update_inserts_from_server.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/commands/wipe_test_indices.py` & `dcicsnovault-8.0.1.0b2/snovault/commands/wipe_test_indices.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/config.py` & `dcicsnovault-8.0.1.0b2/snovault/config.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/connection.py` & `dcicsnovault-8.0.1.0b2/snovault/connection.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/crud_views.py` & `dcicsnovault-8.0.1.0b2/snovault/crud_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/custom_embed.py` & `dcicsnovault-8.0.1.0b2/snovault/custom_embed.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/dev_servers.py` & `dcicsnovault-8.0.1.0b2/snovault/dev_servers.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,30 +12,30 @@
 import os.path
 import select
 import shutil
 import subprocess
 import sys
 
 from dcicutils.misc_utils import PRINT
-from pkg_resources import resource_filename
 from pyramid.paster import get_app, get_appsettings
 from pyramid.path import DottedNameResolver
 from .elasticsearch import create_mapping
+from .project import PROJECT_NAME, project_filename
 from .tests import elasticsearch_fixture, postgresql_fixture
 
 
 EPILOG = __doc__
 
 logger = logging.getLogger(__name__)
 
 
 def nginx_server_process(prefix='', echo=False):
     args = [
         os.path.join(prefix, 'nginx'),
-        '-c', resource_filename('encoded', 'nginx-dev.conf'),
+        '-c', project_filename('nginx-dev.conf'),
         '-g', 'daemon off;'
     ]
     process = subprocess.Popen(
         args,
         close_fds=True,
         stdout=subprocess.PIPE,
         stderr=subprocess.STDOUT,
@@ -100,26 +100,27 @@
     )
     parser.add_argument('--app-name', help="Pyramid app name in configfile")
     parser.add_argument('config_uri', help="path to configfile")
     parser.add_argument('--clear', action="store_true", help="Clear existing data")
     parser.add_argument('--init', action="store_true", help="Init database")
     parser.add_argument('--load', action="store_true", help="Load test set")
     parser.add_argument('--datadir', default='/tmp/snovault', help="path to datadir")
-    parser.add_argument('--no_ingest', action="store_true", default=False, help="Don't start the ingestion process.")
+    # parser.add_argument('--no_ingest', action="store_true", default=False, help="Don't start the ingestion process.")
     args = parser.parse_args()
 
     run(app_name=args.app_name, config_uri=args.config_uri, datadir=args.datadir,
-        clear=args.clear, init=args.init, load=args.load, ingest=not args.no_ingest)
+        # Ingestion is disabled. snovault has no such concept. -kmp 17-Feb-2023
+        clear=args.clear, init=args.init, load=args.load, ingest=False)  # ingest=not args.no_ingest
 
 
 def run(app_name, config_uri, datadir, clear=False, init=False, load=False, ingest=True):
 
     logging.basicConfig(format='')
     # Loading app will have configured from config file. Reconfigure here:
-    logging.getLogger('encoded').setLevel(logging.INFO)
+    logging.getLogger(PROJECT_NAME).setLevel(logging.INFO)
 
     # get the config and see if we want to connect to non-local servers
     # TODO: This variable seems to not get used? -kmp 25-Jul-2020
     config = get_appsettings(config_uri, app_name)
 
     datadir = os.path.abspath(datadir)
     pgdata = os.path.join(datadir, 'pgdata')
@@ -144,20 +145,19 @@
                 for line in process.stdout:
                     sys.stdout.write(line.decode('utf-8'))
             except IOError:
                 pass
             process.wait()
 
     processes = []
-    app = get_app(config_uri, app_name)
-    settings = app.registry.settings
 
     # For now - required components
     postgres = postgresql_fixture.server_process(pgdata, echo=True)
     processes.append(postgres)
+
     es_server_url = config.get('elasticsearch.server', "localhost")
 
     if '127.0.0.1' in es_server_url or 'localhost' in es_server_url:
         # Bootup local ES server subprocess. Else assume connecting to remote ES cluster.
         elasticsearch = elasticsearch_fixture.server_process(esdata, echo=True)
         processes.append(elasticsearch)
     elif not config.get('indexer.namespace'):
@@ -168,28 +168,26 @@
         PRINT(
             'WARNING - elasticsearch.aws_auth is set to false.'
             ' Connection will fail if connecting to remote ES cluster on AWS.')
 
     nginx = nginx_server_process(echo=True)
     processes.append(nginx)
 
+    app = get_app(config_uri, app_name)
+    settings = app.registry.settings
+
     # Optional components
     if 'redis.server' in settings:
         redis = redis_server_process(echo=True)
         processes.append(redis)
 
     if ingest:
         ingestion_listener = ingestion_listener_process(config_uri, app_name)
         processes.append(ingestion_listener)
 
-    if init:
-        app = get_app(config_uri, app_name)
-    else:
-        app = None
-
     # clear queues and initialize indices before loading data. No indexing yet.
     # this is needed for items with properties stored in ES
     if init:
         create_mapping.run(app, skip_indexing=True, purge_queue=False)
 
     if init and load:
         load_test_data = app.registry.settings.get('load_test_data')
```

### Comparing `dcicsnovault-8.0.1.0b1/snovault/drs.py` & `dcicsnovault-8.0.1.0b2/snovault/drs.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/edw_hash.py` & `dcicsnovault-8.0.1.0b2/snovault/edw_hash.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/elasticsearch/__init__.py` & `dcicsnovault-8.0.1.0b2/snovault/elasticsearch/__init__.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/elasticsearch/cached_views.py` & `dcicsnovault-8.0.1.0b2/snovault/elasticsearch/cached_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/elasticsearch/create_mapping.py` & `dcicsnovault-8.0.1.0b2/snovault/elasticsearch/create_mapping.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/elasticsearch/es_index_listener.py` & `dcicsnovault-8.0.1.0b2/snovault/elasticsearch/es_index_listener.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/elasticsearch/esstorage.py` & `dcicsnovault-8.0.1.0b2/snovault/elasticsearch/esstorage.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/elasticsearch/indexer.py` & `dcicsnovault-8.0.1.0b2/snovault/elasticsearch/indexer.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/elasticsearch/indexer_queue.py` & `dcicsnovault-8.0.1.0b2/snovault/elasticsearch/indexer_queue.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/elasticsearch/indexer_utils.py` & `dcicsnovault-8.0.1.0b2/snovault/elasticsearch/indexer_utils.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/elasticsearch/mpindexer.py` & `dcicsnovault-8.0.1.0b2/snovault/elasticsearch/mpindexer.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/embed.py` & `dcicsnovault-8.0.1.0b2/snovault/embed.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/etag.py` & `dcicsnovault-8.0.1.0b2/snovault/etag.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/indexing_views.py` & `dcicsnovault-8.0.1.0b2/snovault/indexing_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/interfaces.py` & `dcicsnovault-8.0.1.0b2/snovault/interfaces.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/invalidation.py` & `dcicsnovault-8.0.1.0b2/snovault/invalidation.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/json_renderer.py` & `dcicsnovault-8.0.1.0b2/snovault/json_renderer.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/jsongraph.py` & `dcicsnovault-8.0.1.0b2/snovault/jsongraph.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/jsonld_context.py` & `dcicsnovault-8.0.1.0b2/snovault/jsonld_context.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/loadxl.py` & `dcicsnovault-8.0.1.0b2/snovault/loadxl.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,22 +8,23 @@
 import os
 import structlog
 import webtest
 import traceback
 import uuid
 
 from base64 import b64encode
-from dcicutils.misc_utils import ignored
+from dcicutils.misc_utils import ignored, environ_bool
 from dcicutils.secrets_utils import assume_identity
 from PIL import Image
-from pkg_resources import resource_filename
 from pyramid.paster import get_app
 from pyramid.response import Response
 from pyramid.view import view_config
 from snovault.util import debug_log
+
+from .project import project_filename
 from .server_defaults import add_last_modified
 
 
 text = type(u'')
 logger = structlog.getLogger(__name__)
 
 
@@ -112,15 +113,15 @@
     fdn_dir = request.json.get('fdn_dir')
     overwrite = request.json.get('overwrite', False)
     itype = request.json.get('itype')
     iter_resp = request.json.get('iter_response', False)
     inserts = None
     from_json = False
     if fdn_dir:
-        inserts = resource_filename('encoded', 'tests/data/' + fdn_dir + '/')
+        inserts = project_filename('tests/data/' + fdn_dir + '/')
     elif local_path:
         inserts = local_path
     elif store:
         inserts = store
         from_json = True
     # if we want to iterate over the response to keep the connection alive
     # this directly calls load_all_gen, instead of load_all
@@ -282,14 +283,17 @@
     # gen.caught is None for success and an error message on failure
     if gen.caught is None:
         return None
     else:
         return Exception(gen.caught)
 
 
+LOADXL_ALLOW_NONE = environ_bool("LOADXL_ALLOW_NONE", default=True)
+
+
 def load_all_gen(testapp, inserts, docsdir, overwrite=True, itype=None, from_json=False,
                  patch_only=False, post_only=False, skip_types=None):
     """
     Generator function that yields bytes information about each item POSTed/PATCHed.
     Is the base functionality of load_all function.
 
     convert data to store format dictionary (same format expected from from_json=True),
@@ -351,14 +355,16 @@
         if isinstance(itype, list):
             store = {i: store[i] for i in itype if i in store}
         else:
             store = {itype: store.get(itype, [])}
     # clear empty values
     store = {k: v for k, v in store.items() if v is not None}
     if not store:
+        if LOADXL_ALLOW_NONE:
+            return
         if from_json:
             err_msg = 'No items found in input "store" json'
         else:
             err_msg = 'No items found in %s' % inserts
         if itype:
             err_msg += ' for item type(s) %s' % itype
         # import pdb; pdb.set_trace()
@@ -507,30 +513,30 @@
     environ = {
         'HTTP_ACCEPT': 'application/json',
         'REMOTE_USER': 'TEST',
     }
     testapp = webtest.TestApp(app, environ)
     # load master-inserts by default
     if indir != 'master-inserts' and use_master_inserts:
-        master_inserts = resource_filename('encoded', 'tests/data/master-inserts/')
+        master_inserts = project_filename('tests/data/master-inserts/')
         master_res = load_all(testapp, master_inserts, [], skip_types=skip_types)
         if master_res:  # None if successful
             print(LOAD_ERROR_MESSAGE)
             logger.error('load_data: failed to load from %s' % master_inserts, error=master_res)
             return master_res
 
     if not indir.endswith('/'):
         indir += '/'
-    inserts = resource_filename('encoded', 'tests/data/' + indir)
+    inserts = project_filename('tests/data/' + indir)
     if docsdir is None:
         docsdir = []
     else:
         if not docsdir.endswith('/'):
             docsdir += '/'
-        docsdir = [resource_filename('encoded', 'tests/data/' + docsdir)]
+        docsdir = [project_filename('tests/data/' + docsdir)]
     res = load_all(testapp, inserts, docsdir, overwrite=overwrite)
     if res:  # None if successful
         print(LOAD_ERROR_MESSAGE)
         logger.error('load_data: failed to load from %s' % docsdir, error=res)
         return res
     return None  # unnecessary, but makes it more clear that no error was encountered
 
@@ -558,15 +564,15 @@
 
     test_insert_dirs = [
         'temp-local-inserts',
         'demo_inserts'
     ]
 
     for test_insert_dir in test_insert_dirs:
-        chk_dir = resource_filename('encoded', "tests/data/" + test_insert_dir)
+        chk_dir = project_filename("tests/data/" + test_insert_dir)
         for (dirpath, dirnames, filenames) in os.walk(chk_dir):
             if any([fn for fn in filenames if fn.endswith('.json') or fn.endswith('.json.gz')]):
                 logger.info('Loading inserts from "{}" directory.'.format(test_insert_dir))
                 return load_data(app, docsdir='documents', indir=test_insert_dir, use_master_inserts=True,
                                  overwrite=overwrite)
 
     # Default to 'inserts' if no temp inserts found.
@@ -701,15 +707,15 @@
         'HTTP_ACCEPT': 'application/json',
         'REMOTE_USER': 'TEST',
     }
     testapp = webtest.TestApp(app, environ)
 
     if not indir.endswith('/'):
         indir += '/'
-    inserts = resource_filename('encoded', 'tests/data/' + indir)
+    inserts = project_filename('tests/data/' + indir)
 
     res = load_all(testapp, inserts, docsdir=[], overwrite=overwrite, itype=itype)
     if res:  # None if successful
         print(LOAD_ERROR_MESSAGE)
         logger.error('load_data_by_type: failed to load from %s' % indir, error=res)
         return res
     return None  # unnecessary, but makes it more clear that no error was encountered
```

### Comparing `dcicsnovault-8.0.1.0b1/snovault/memlimit.py` & `dcicsnovault-8.0.1.0b2/snovault/memlimit.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/parallel.py` & `dcicsnovault-8.0.1.0b2/snovault/parallel.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/predicates.py` & `dcicsnovault-8.0.1.0b2/snovault/predicates.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/redis/redis_connection.py` & `dcicsnovault-8.0.1.0b2/snovault/redis/redis_connection.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/renderers.py` & `dcicsnovault-8.0.1.0b2/snovault/renderers.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/resource_views.py` & `dcicsnovault-8.0.1.0b2/snovault/resource_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/resources.py` & `dcicsnovault-8.0.1.0b2/snovault/resources.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/schema_graph.py` & `dcicsnovault-8.0.1.0b2/snovault/schema_graph.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/schema_utils.py` & `dcicsnovault-8.0.1.0b2/snovault/schema_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,22 @@
 # to avoid a circularity. No files should refer upward to "." for imports. -kmp 9-Jun-2020
 from .resources import Item, COLLECTIONS
 
 
 SERVER_DEFAULTS = {}
 
 
+# TODO: Shouldn't this return func? Otherwise this:
+#           @server_default
+#           def foo(instance, subschema):
+#               return ...something...
+#       does (approximately):
+#           SERVER_DEFAULTS['foo'] = lambda(instance, subschema): ...something...
+#           server_default = None
+#       It feels like the function should still get defined. -kmp 17-Feb-2023
 def server_default(func):
     SERVER_DEFAULTS[func.__name__] = func
 
 
 class NoRemoteResolver(RefResolver):
     def resolve_remote(self, uri):
         raise ValueError('Resolution disallowed for: %s' % uri)
```

### Comparing `dcicsnovault-8.0.1.0b1/snovault/schema_views.py` & `dcicsnovault-8.0.1.0b2/snovault/schema_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/schemas/access_key.json` & `dcicsnovault-8.0.1.0b2/snovault/schemas/access_key.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/schemas/filter_set.json` & `dcicsnovault-8.0.1.0b2/snovault/schemas/filter_set.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/schemas/mixins.json` & `dcicsnovault-8.0.1.0b2/snovault/schemas/mixins.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/schemas/user.json` & `dcicsnovault-8.0.1.0b2/snovault/schemas/user.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/search/compound_search.py` & `dcicsnovault-8.0.1.0b2/snovault/search/compound_search.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/search/lucene_builder.py` & `dcicsnovault-8.0.1.0b2/snovault/search/lucene_builder.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/search/search.py` & `dcicsnovault-8.0.1.0b2/snovault/search/search.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/search/search_utils.py` & `dcicsnovault-8.0.1.0b2/snovault/search/search_utils.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/server_defaults.py` & `dcicsnovault-8.0.1.0b2/snovault/server_defaults.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/settings.py` & `dcicsnovault-8.0.1.0b2/snovault/settings.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/standalone_dev.py` & `dcicsnovault-8.0.1.0b2/snovault/standalone_dev.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/stats.py` & `dcicsnovault-8.0.1.0b2/snovault/stats.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/storage.py` & `dcicsnovault-8.0.1.0b2/snovault/storage.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/test_schemas/EmbeddingTest.json` & `dcicsnovault-8.0.1.0b2/snovault/test_schemas/EmbeddingTest.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/test_schemas/NestedObjectLinkTarget.json` & `dcicsnovault-8.0.1.0b2/snovault/test_schemas/NestedObjectLinkTarget.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/test_schemas/TestingBiosampleSno.json` & `dcicsnovault-8.0.1.0b2/snovault/test_schemas/TestingBiosampleSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/test_schemas/TestingBiosourceSno.json` & `dcicsnovault-8.0.1.0b2/snovault/test_schemas/TestingBiosourceSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/test_schemas/TestingCalculatedProperties.json` & `dcicsnovault-8.0.1.0b2/snovault/test_schemas/TestingCalculatedProperties.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/test_schemas/TestingDownload.json` & `dcicsnovault-8.0.1.0b2/snovault/test_schemas/TestingDownload.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/test_schemas/TestingIndividualSno.json` & `dcicsnovault-8.0.1.0b2/snovault/test_schemas/TestingIndividualSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/test_schemas/TestingLinkAggregateSno.json` & `dcicsnovault-8.0.1.0b2/snovault/test_schemas/TestingLinkAggregateSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/test_schemas/TestingLinkSourceSno.json` & `dcicsnovault-8.0.1.0b2/snovault/test_schemas/TestingLinkSourceSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/test_schemas/TestingNestedEnabled.json` & `dcicsnovault-8.0.1.0b2/snovault/test_schemas/TestingNestedEnabled.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/test_schemas/TestingNoteSno.json` & `dcicsnovault-8.0.1.0b2/snovault/test_schemas/TestingNoteSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/test_schemas/TestingPostPutPatchSno.json` & `dcicsnovault-8.0.1.0b2/snovault/test_schemas/TestingPostPutPatchSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/test_schemas/TestingServerDefault.json` & `dcicsnovault-8.0.1.0b2/snovault/test_schemas/TestingServerDefault.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/test_schemas/mixins.json` & `dcicsnovault-8.0.1.0b2/snovault/test_schemas/mixins.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/tests/conftest.py` & `dcicsnovault-8.0.1.0b2/snovault/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/tests/elasticsearch_fixture.py` & `dcicsnovault-8.0.1.0b2/snovault/tests/elasticsearch_fixture.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/tests/postgresql_fixture.py` & `dcicsnovault-8.0.1.0b2/snovault/tests/postgresql_fixture.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/tests/pyramidfixtures.py` & `dcicsnovault-8.0.1.0b2/snovault/tests/pyramidfixtures.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/tests/root.py` & `dcicsnovault-8.0.1.0b2/snovault/tests/root.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/tests/serverfixtures.py` & `dcicsnovault-8.0.1.0b2/snovault/tests/serverfixtures.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/tests/test_attachment.py` & `dcicsnovault-8.0.1.0b2/snovault/tests/test_attachment.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/tests/test_authentication.py` & `dcicsnovault-8.0.1.0b2/snovault/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/tests/test_calculated.py` & `dcicsnovault-8.0.1.0b2/snovault/tests/test_calculated.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/tests/test_clear_db_es_contents.py` & `dcicsnovault-8.0.1.0b2/snovault/tests/test_clear_db_es_contents.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/tests/test_create_mapping.py` & `dcicsnovault-8.0.1.0b2/snovault/tests/test_create_mapping.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/tests/test_drs.py` & `dcicsnovault-8.0.1.0b2/snovault/tests/test_drs.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/tests/test_edw_hash.py` & `dcicsnovault-8.0.1.0b2/snovault/tests/test_edw_hash.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/tests/test_embed_utils.py` & `dcicsnovault-8.0.1.0b2/snovault/tests/test_embed_utils.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/tests/test_embedding.py` & `dcicsnovault-8.0.1.0b2/snovault/tests/test_embedding.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/tests/test_es_permissions.py` & `dcicsnovault-8.0.1.0b2/snovault/tests/test_es_permissions.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/tests/test_indexing.py` & `dcicsnovault-8.0.1.0b2/snovault/tests/test_indexing.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/tests/test_invalidation_scope.py` & `dcicsnovault-8.0.1.0b2/snovault/tests/test_invalidation_scope.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/tests/test_key.py` & `dcicsnovault-8.0.1.0b2/snovault/tests/test_key.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/tests/test_link.py` & `dcicsnovault-8.0.1.0b2/snovault/tests/test_link.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/tests/test_logging.py` & `dcicsnovault-8.0.1.0b2/snovault/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/tests/test_misc.py` & `dcicsnovault-8.0.1.0b2/snovault/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/tests/test_post_put_patch.py` & `dcicsnovault-8.0.1.0b2/snovault/tests/test_post_put_patch.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/tests/test_postgresql_fixture.py` & `dcicsnovault-8.0.1.0b2/snovault/tests/test_postgresql_fixture.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/tests/test_schemas.py` & `dcicsnovault-8.0.1.0b2/snovault/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/tests/test_serverfixtures.py` & `dcicsnovault-8.0.1.0b2/snovault/tests/test_serverfixtures.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/tests/test_standalone_dev.py` & `dcicsnovault-8.0.1.0b2/snovault/tests/test_standalone_dev.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/tests/test_stats.py` & `dcicsnovault-8.0.1.0b2/snovault/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/tests/test_storage.py` & `dcicsnovault-8.0.1.0b2/snovault/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/tests/test_types_access_key.py` & `dcicsnovault-8.0.1.0b2/snovault/tests/test_types_access_key.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/tests/test_upgrader.py` & `dcicsnovault-8.0.1.0b2/snovault/tests/test_upgrader.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/tests/test_util.py` & `dcicsnovault-8.0.1.0b2/snovault/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/tests/test_views.py` & `dcicsnovault-8.0.1.0b2/snovault/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/tests/testappfixtures.py` & `dcicsnovault-8.0.1.0b2/snovault/tests/testappfixtures.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/tests/testing_upgrader.py` & `dcicsnovault-8.0.1.0b2/snovault/tests/testing_upgrader.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/tests/testing_views.py` & `dcicsnovault-8.0.1.0b2/snovault/tests/testing_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/tests/toolfixtures.py` & `dcicsnovault-8.0.1.0b2/snovault/tests/toolfixtures.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/tools.py` & `dcicsnovault-8.0.1.0b2/snovault/tools.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/typedsheets.py` & `dcicsnovault-8.0.1.0b2/snovault/typedsheets.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/typeinfo.py` & `dcicsnovault-8.0.1.0b2/snovault/typeinfo.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/types/access_key.py` & `dcicsnovault-8.0.1.0b2/snovault/types/access_key.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/types/base.py` & `dcicsnovault-8.0.1.0b2/snovault/types/base.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/types/filter_set.py` & `dcicsnovault-8.0.1.0b2/snovault/types/filter_set.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/types/user.py` & `dcicsnovault-8.0.1.0b2/snovault/types/user.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/upgrader.py` & `dcicsnovault-8.0.1.0b2/snovault/upgrader.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/util.py` & `dcicsnovault-8.0.1.0b2/snovault/util.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/validation.py` & `dcicsnovault-8.0.1.0b2/snovault/validation.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/snovault/validators.py` & `dcicsnovault-8.0.1.0b2/snovault/validators.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b1/PKG-INFO` & `dcicsnovault-8.0.1.0b2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcicsnovault
-Version: 8.0.1.0b1
+Version: 8.0.1.0b2
 Summary: Storage support for 4DN Data Portals.
 Home-page: https://github.com/4dn-dcic/snovault
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.8.1,<3.10
 Classifier: Development Status :: 4 - Beta
@@ -12,43 +12,44 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Database :: Database Engines/Servers
 Requires-Dist: PyBrowserID (>=0.10.0,<1)
 Requires-Dist: SPARQLWrapper (>=1.8.5,<2.0.0)
 Requires-Dist: SQLAlchemy (>=1.4.41,<2.0.0)
 Requires-Dist: WSGIProxy2 (==0.4.2)
 Requires-Dist: WebOb (>=1.8.7,<2.0.0)
 Requires-Dist: WebTest (>=2.0.35,<3.0.0)
 Requires-Dist: aws_requests_auth (>=0.4.1,<0.5.0)
-Requires-Dist: boto3 (>=1.24.36)
-Requires-Dist: botocore (>=1.27.36)
+Requires-Dist: boto3 (>=1.26.119)
+Requires-Dist: botocore (>=1.19.119)
 Requires-Dist: dcicutils (>=7.0.0,<8.0.0)
 Requires-Dist: elasticsearch (==7.13.4)
 Requires-Dist: elasticsearch_dsl (>=7.4.0,<8.0.0)
 Requires-Dist: future (>=0.15.2,<1)
 Requires-Dist: html5lib (>=1.1)
 Requires-Dist: humanfriendly (>=1.44.9,<2.0.0)
 Requires-Dist: jsonschema_serialize_fork (>=2.1.1,<3.0.0)
 Requires-Dist: netaddr (>=0.8.0,<1)
 Requires-Dist: passlib (>=1.7.4,<2.0.0)
+Requires-Dist: pillow (>=9.5.0,<10.0.0)
 Requires-Dist: psutil (>=5.9.0,<6.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.1,<3.0.0)
 Requires-Dist: pyjwt (>=2.6.0,<3.0.0)
 Requires-Dist: pyramid (==1.10.4)
 Requires-Dist: pyramid-multiauth (>=0.9.0,<1)
 Requires-Dist: pyramid-retry (>=1.0,<2.0)
 Requires-Dist: pyramid-tm (>=2.5,<3.0)
 Requires-Dist: pyramid-translogger (>=0.1,<0.2)
 Requires-Dist: pyramid_localroles (>=0.1,<1)
-Requires-Dist: pytest-redis (>=2.0.0,<3.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: python_magic (>=0.4.27)
 Requires-Dist: pytz (>=2021.3)
 Requires-Dist: rdflib (>=4.2.2,<5.0.0)
 Requires-Dist: rdflib-jsonld (>=0.5.0,<1.0.0)
 Requires-Dist: redis (>=4.5.1,<5.0.0)
 Requires-Dist: rutter (>=0.3,<1)
```

