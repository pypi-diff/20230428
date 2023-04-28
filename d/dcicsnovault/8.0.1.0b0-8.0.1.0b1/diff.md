# Comparing `tmp/dcicsnovault-8.0.1.0b0.tar.gz` & `tmp/dcicsnovault-8.0.1.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcicsnovault-8.0.1.0b0.tar", max compression
+gzip compressed data, was "dcicsnovault-8.0.1.0b1.tar", max compression
```

## Comparing `dcicsnovault-8.0.1.0b0.tar` & `dcicsnovault-8.0.1.0b1.tar`

### file list

```diff
@@ -1,154 +1,153 @@
--rw-r--r--   0        0        0     1135 2020-04-22 15:19:59.681690 dcicsnovault-8.0.1.0b0/LICENSE.txt
--rw-r--r--   0        0        0     6407 2023-02-08 18:10:49.791837 dcicsnovault-8.0.1.0b0/README.rst
--rw-r--r--   0        0        0     5597 2023-04-21 16:49:59.844602 dcicsnovault-8.0.1.0b0/pyproject.toml
--rw-r--r--   0        0        0     4586 2023-04-10 19:15:18.757135 dcicsnovault-8.0.1.0b0/snovault/__init__.py
--rw-r--r--   0        0        0     1942 2023-02-08 18:10:49.809612 dcicsnovault-8.0.1.0b0/snovault/aggregated_items.py
--rw-r--r--   0        0        0     8799 2023-04-10 19:15:16.606539 dcicsnovault-8.0.1.0b0/snovault/app.py
--rw-r--r--   0        0        0    11879 2023-02-08 18:10:49.815230 dcicsnovault-8.0.1.0b0/snovault/attachment.py
--rw-r--r--   0        0        0    25327 2023-04-10 19:15:18.762744 dcicsnovault-8.0.1.0b0/snovault/authentication.py
--rw-r--r--   0        0        0     4467 2023-04-10 19:15:18.769224 dcicsnovault-8.0.1.0b0/snovault/authorization.py
--rw-r--r--   0        0        0     6670 2023-02-08 18:10:49.815747 dcicsnovault-8.0.1.0b0/snovault/batchupgrade.py
--rw-r--r--   0        0        0     1902 2020-04-22 15:19:59.997364 dcicsnovault-8.0.1.0b0/snovault/cache.py
--rw-r--r--   0        0        0     6461 2020-10-21 18:02:06.878589 dcicsnovault-8.0.1.0b0/snovault/calculated.py
--rw-r--r--   0        0        0       10 2020-04-22 15:19:59.995285 dcicsnovault-8.0.1.0b0/snovault/commands/__init__.py
--rw-r--r--   0        0        0     3416 2020-09-15 14:05:58.054812 dcicsnovault-8.0.1.0b0/snovault/commands/check_rendering.py
--rw-r--r--   0        0        0     6813 2023-04-10 19:15:18.770085 dcicsnovault-8.0.1.0b0/snovault/commands/clear_db_es_contents.py
--rw-r--r--   0        0        0     3928 2023-04-12 19:00:53.363747 dcicsnovault-8.0.1.0b0/snovault/commands/create_mapping_on_deploy.py
--rw-r--r--   0        0        0     1608 2023-02-08 18:10:49.821555 dcicsnovault-8.0.1.0b0/snovault/commands/es_index_data.py
--rw-r--r--   0        0        0     1644 2020-04-22 15:19:59.991754 dcicsnovault-8.0.1.0b0/snovault/commands/jsonld_rdf.py
--rw-r--r--   0        0        0     6212 2023-04-10 19:15:18.783044 dcicsnovault-8.0.1.0b0/snovault/commands/load_access_keys.py
--rw-r--r--   0        0        0     2402 2023-04-12 18:12:36.164770 dcicsnovault-8.0.1.0b0/snovault/commands/load_data.py
--rw-r--r--   0        0        0     2188 2023-04-10 19:15:18.794707 dcicsnovault-8.0.1.0b0/snovault/commands/load_data_by_type.py
--rw-r--r--   0        0        0     4350 2023-02-08 18:10:49.822376 dcicsnovault-8.0.1.0b0/snovault/commands/profile.py
--rw-r--r--   0        0        0     3236 2023-04-10 19:15:18.800917 dcicsnovault-8.0.1.0b0/snovault/commands/purge_item_type.py
--rw-r--r--   0        0        0     1868 2023-04-10 19:15:18.806775 dcicsnovault-8.0.1.0b0/snovault/commands/run_upgrader_on_inserts.py
--rw-r--r--   0        0        0     8533 2023-04-10 19:15:18.813142 dcicsnovault-8.0.1.0b0/snovault/commands/update_inserts_from_server.py
--rw-r--r--   0        0        0      909 2023-02-08 18:10:49.823005 dcicsnovault-8.0.1.0b0/snovault/commands/wipe_test_indices.py
--rw-r--r--   0        0        0     4183 2023-02-08 18:10:49.823623 dcicsnovault-8.0.1.0b0/snovault/config.py
--rw-r--r--   0        0        0     6352 2023-02-08 18:10:49.824292 dcicsnovault-8.0.1.0b0/snovault/connection.py
--rw-r--r--   0        0        0    14798 2023-04-12 18:07:32.110006 dcicsnovault-8.0.1.0b0/snovault/crud_views.py
--rw-r--r--   0        0        0    15301 2023-04-10 19:15:18.825267 dcicsnovault-8.0.1.0b0/snovault/custom_embed.py
--rw-r--r--   0        0        0     7216 2023-04-10 19:15:18.827085 dcicsnovault-8.0.1.0b0/snovault/dev_servers.py
--rw-r--r--   0        0        0     4340 2023-04-13 14:12:36.718529 dcicsnovault-8.0.1.0b0/snovault/drs.py
--rw-r--r--   0        0        0     1829 2023-04-10 19:15:18.836570 dcicsnovault-8.0.1.0b0/snovault/edw_hash.py
--rw-r--r--   0        0        0     4282 2023-02-08 18:10:49.830617 dcicsnovault-8.0.1.0b0/snovault/elasticsearch/__init__.py
--rw-r--r--   0        0        0     4727 2023-02-08 18:10:49.835624 dcicsnovault-8.0.1.0b0/snovault/elasticsearch/cached_views.py
--rw-r--r--   0        0        0    61320 2023-04-07 15:35:45.681095 dcicsnovault-8.0.1.0b0/snovault/elasticsearch/create_mapping.py
--rw-r--r--   0        0        0     7939 2023-02-08 18:10:49.846547 dcicsnovault-8.0.1.0b0/snovault/elasticsearch/es_index_listener.py
--rw-r--r--   0        0        0    18572 2023-02-08 18:10:49.851730 dcicsnovault-8.0.1.0b0/snovault/elasticsearch/esstorage.py
--rw-r--r--   0        0        0    24405 2023-04-10 19:15:16.612559 dcicsnovault-8.0.1.0b0/snovault/elasticsearch/indexer.py
--rw-r--r--   0        0        0    31356 2023-02-08 18:10:49.863845 dcicsnovault-8.0.1.0b0/snovault/elasticsearch/indexer_queue.py
--rw-r--r--   0        0        0    20947 2023-02-08 18:10:49.871835 dcicsnovault-8.0.1.0b0/snovault/elasticsearch/indexer_utils.py
--rw-r--r--   0        0        0      349 2021-08-12 19:39:17.751212 dcicsnovault-8.0.1.0b0/snovault/elasticsearch/interfaces.py
--rw-r--r--   0        0        0    10190 2023-04-10 19:15:16.619476 dcicsnovault-8.0.1.0b0/snovault/elasticsearch/mpindexer.py
--rw-r--r--   0        0        0     8249 2021-08-12 19:39:17.757097 dcicsnovault-8.0.1.0b0/snovault/embed.py
--rw-r--r--   0        0        0     1061 2023-02-08 18:10:49.878124 dcicsnovault-8.0.1.0b0/snovault/etag.py
--rw-r--r--   0        0        0    10835 2023-02-08 18:10:49.886932 dcicsnovault-8.0.1.0b0/snovault/indexing_views.py
--rw-r--r--   0        0        0      774 2020-04-22 15:19:59.962133 dcicsnovault-8.0.1.0b0/snovault/interfaces.py
--rw-r--r--   0        0        0     2229 2023-02-08 18:10:49.892547 dcicsnovault-8.0.1.0b0/snovault/invalidation.py
--rw-r--r--   0        0        0     1639 2023-02-08 18:10:49.897621 dcicsnovault-8.0.1.0b0/snovault/json_renderer.py
--rw-r--r--   0        0        0     2292 2020-09-15 14:05:58.093412 dcicsnovault-8.0.1.0b0/snovault/jsongraph.py
--rw-r--r--   0        0        0     9713 2023-02-08 18:10:49.904627 dcicsnovault-8.0.1.0b0/snovault/jsonld_context.py
--rw-r--r--   0        0        0    30294 2023-04-10 19:15:18.843268 dcicsnovault-8.0.1.0b0/snovault/loadxl.py
--rw-r--r--   0        0        0     2425 2023-04-10 19:15:18.848768 dcicsnovault-8.0.1.0b0/snovault/memlimit.py
--rw-r--r--   0        0        0     1165 2023-04-10 19:15:18.854745 dcicsnovault-8.0.1.0b0/snovault/parallel.py
--rw-r--r--   0        0        0      846 2020-04-22 15:19:59.956023 dcicsnovault-8.0.1.0b0/snovault/predicates.py
--rw-r--r--   0        0        0       95 2023-04-10 19:15:16.625324 dcicsnovault-8.0.1.0b0/snovault/redis/README.rst
--rw-r--r--   0        0        0       90 2023-04-10 19:15:16.630313 dcicsnovault-8.0.1.0b0/snovault/redis/__init__.py
--rw-r--r--   0        0        0       16 2023-04-10 19:15:16.635178 dcicsnovault-8.0.1.0b0/snovault/redis/interfaces.py
--rw-r--r--   0        0        0     4106 2023-04-10 19:15:16.640462 dcicsnovault-8.0.1.0b0/snovault/redis/redis_connection.py
--rw-r--r--   0        0        0    22128 2023-04-10 19:15:18.861451 dcicsnovault-8.0.1.0b0/snovault/renderers.py
--rw-r--r--   0        0        0    11201 2023-02-08 18:10:49.914597 dcicsnovault-8.0.1.0b0/snovault/resource_views.py
--rw-r--r--   0        0        0    21863 2023-04-10 19:15:16.646344 dcicsnovault-8.0.1.0b0/snovault/resources.py
--rw-r--r--   0        0        0     3450 2023-02-08 18:10:49.920477 dcicsnovault-8.0.1.0b0/snovault/schema_graph.py
--rw-r--r--   0        0        0    14162 2023-04-10 19:15:18.867518 dcicsnovault-8.0.1.0b0/snovault/schema_utils.py
--rw-r--r--   0        0        0     4358 2023-04-10 19:15:18.873112 dcicsnovault-8.0.1.0b0/snovault/schema_views.py
--rw-r--r--   0        0        0     1855 2023-04-12 15:13:35.702783 dcicsnovault-8.0.1.0b0/snovault/schemas/access_key.json
--rw-r--r--   0        0        0     5098 2023-04-10 19:15:18.881989 dcicsnovault-8.0.1.0b0/snovault/schemas/filter_set.json
--rw-r--r--   0        0        0    18744 2023-04-10 19:15:18.887742 dcicsnovault-8.0.1.0b0/snovault/schemas/mixins.json
--rw-r--r--   0        0        0    19600 2023-04-10 19:15:18.893767 dcicsnovault-8.0.1.0b0/snovault/schemas/user.json
--rw-r--r--   0        0        0    20952 2023-04-10 19:15:18.900179 dcicsnovault-8.0.1.0b0/snovault/search/compound_search.py
--rw-r--r--   0        0        0    58595 2023-04-10 19:15:18.906948 dcicsnovault-8.0.1.0b0/snovault/search/lucene_builder.py
--rw-r--r--   0        0        0    62789 2023-04-10 19:15:18.913908 dcicsnovault-8.0.1.0b0/snovault/search/search.py
--rw-r--r--   0        0        0    17901 2023-04-10 19:15:18.923487 dcicsnovault-8.0.1.0b0/snovault/search/search_utils.py
--rw-r--r--   0        0        0     4541 2023-04-10 19:15:18.929481 dcicsnovault-8.0.1.0b0/snovault/server_defaults.py
--rw-r--r--   0        0        0      522 2023-02-08 18:10:49.926443 dcicsnovault-8.0.1.0b0/snovault/settings.py
--rw-r--r--   0        0        0     1498 2021-08-12 19:39:17.787731 dcicsnovault-8.0.1.0b0/snovault/standalone_dev.py
--rw-r--r--   0        0        0     4383 2023-02-08 18:10:49.931408 dcicsnovault-8.0.1.0b0/snovault/stats.py
--rw-r--r--   0        0        0    34834 2023-04-10 19:15:20.635570 dcicsnovault-8.0.1.0b0/snovault/storage.py
--rw-r--r--   0        0        0      330 2020-04-22 15:19:59.941685 dcicsnovault-8.0.1.0b0/snovault/test_schemas/AbstractItemTestSecondSubItem.json
--rw-r--r--   0        0        0      300 2020-04-22 15:19:59.940748 dcicsnovault-8.0.1.0b0/snovault/test_schemas/AbstractItemTestSubItem.json
--rw-r--r--   0        0        0     2467 2023-02-08 18:10:49.937350 dcicsnovault-8.0.1.0b0/snovault/test_schemas/EmbeddingTest.json
--rw-r--r--   0        0        0      446 2021-08-12 19:39:17.798764 dcicsnovault-8.0.1.0b0/snovault/test_schemas/NestedEmbeddingContainer.json
--rw-r--r--   0        0        0      883 2021-08-12 19:39:17.803883 dcicsnovault-8.0.1.0b0/snovault/test_schemas/NestedObjectLinkTarget.json
--rw-r--r--   0        0        0      473 2021-08-12 19:39:17.810025 dcicsnovault-8.0.1.0b0/snovault/test_schemas/TestingBiogroupSno.json
--rw-r--r--   0        0        0      968 2023-02-08 18:10:49.943722 dcicsnovault-8.0.1.0b0/snovault/test_schemas/TestingBiosampleSno.json
--rw-r--r--   0        0        0     1082 2021-08-12 19:39:17.820805 dcicsnovault-8.0.1.0b0/snovault/test_schemas/TestingBiosourceSno.json
--rw-r--r--   0        0        0      894 2020-09-25 18:48:35.851983 dcicsnovault-8.0.1.0b0/snovault/test_schemas/TestingCalculatedProperties.json
--rw-r--r--   0        0        0      276 2020-04-22 15:19:59.938605 dcicsnovault-8.0.1.0b0/snovault/test_schemas/TestingDependencies.json
--rw-r--r--   0        0        0      697 2023-04-10 19:15:18.936475 dcicsnovault-8.0.1.0b0/snovault/test_schemas/TestingDownload.json
--rw-r--r--   0        0        0      555 2021-08-12 19:39:17.826025 dcicsnovault-8.0.1.0b0/snovault/test_schemas/TestingIndividualSno.json
--rw-r--r--   0        0        0      730 2020-04-22 15:19:59.936694 dcicsnovault-8.0.1.0b0/snovault/test_schemas/TestingLinkAggregateSno.json
--rw-r--r--   0        0        0      697 2021-08-12 19:39:17.831918 dcicsnovault-8.0.1.0b0/snovault/test_schemas/TestingLinkSourceSno.json
--rw-r--r--   0        0        0      472 2021-08-12 19:39:17.838406 dcicsnovault-8.0.1.0b0/snovault/test_schemas/TestingLinkTargetElasticSearch.json
--rw-r--r--   0        0        0      292 2020-04-22 15:19:59.934939 dcicsnovault-8.0.1.0b0/snovault/test_schemas/TestingLinkTargetSno.json
--rw-r--r--   0        0        0      311 2023-04-10 18:54:40.455623 dcicsnovault-8.0.1.0b0/snovault/test_schemas/TestingMixins.json
--rw-r--r--   0        0        0      845 2021-08-12 19:39:18.009063 dcicsnovault-8.0.1.0b0/snovault/test_schemas/TestingNestedEnabled.json
--rw-r--r--   0        0        0     3721 2023-02-08 18:10:49.949847 dcicsnovault-8.0.1.0b0/snovault/test_schemas/TestingNoteSno.json
--rw-r--r--   0        0        0     1622 2021-08-12 19:39:17.850333 dcicsnovault-8.0.1.0b0/snovault/test_schemas/TestingPostPutPatchSno.json
--rw-r--r--   0        0        0      576 2020-04-22 15:19:59.932932 dcicsnovault-8.0.1.0b0/snovault/test_schemas/TestingServerDefault.json
--rw-r--r--   0        0        0     1215 2023-04-10 19:15:18.938054 dcicsnovault-8.0.1.0b0/snovault/test_schemas/mixins.json
--rw-r--r--   0        0        0        0 2023-03-31 18:39:46.436489 dcicsnovault-8.0.1.0b0/snovault/tests/__init__.py
--rw-r--r--   0        0        0     2210 2023-04-10 19:15:16.653133 dcicsnovault-8.0.1.0b0/snovault/tests/conftest.py
--rw-r--r--   0        0        0      100 2023-02-08 18:10:49.952678 dcicsnovault-8.0.1.0b0/snovault/tests/conftest_settings.py
--rw-r--r--   0        0        0     3086 2023-02-08 18:10:49.957620 dcicsnovault-8.0.1.0b0/snovault/tests/elasticsearch_fixture.py
--rw-r--r--   0        0        0     3921 2020-09-15 14:05:58.160270 dcicsnovault-8.0.1.0b0/snovault/tests/postgresql_fixture.py
--rw-r--r--   0        0        0      852 2023-04-10 19:15:16.658135 dcicsnovault-8.0.1.0b0/snovault/tests/pyramidfixtures.py
--rw-r--r--   0        0        0     3007 2020-09-15 14:05:58.161510 dcicsnovault-8.0.1.0b0/snovault/tests/root.py
--rw-r--r--   0        0        0    17313 2023-04-10 19:15:18.943657 dcicsnovault-8.0.1.0b0/snovault/tests/serverfixtures.py
--rw-r--r--   0        0        0    20332 2023-04-10 19:15:20.636889 dcicsnovault-8.0.1.0b0/snovault/tests/test_attachment.py
--rw-r--r--   0        0        0     3937 2023-04-12 18:08:29.011696 dcicsnovault-8.0.1.0b0/snovault/tests/test_authentication.py
--rw-r--r--   0        0        0     1370 2021-08-12 19:39:17.883512 dcicsnovault-8.0.1.0b0/snovault/tests/test_calculated.py
--rw-r--r--   0        0        0    15979 2023-04-10 19:15:18.956210 dcicsnovault-8.0.1.0b0/snovault/tests/test_clear_db_es_contents.py
--rw-r--r--   0        0        0     8984 2023-02-08 18:10:49.975775 dcicsnovault-8.0.1.0b0/snovault/tests/test_create_mapping.py
--rw-r--r--   0        0        0     3173 2023-04-13 14:15:18.241821 dcicsnovault-8.0.1.0b0/snovault/tests/test_drs.py
--rw-r--r--   0        0        0      528 2023-04-10 19:15:18.963682 dcicsnovault-8.0.1.0b0/snovault/tests/test_edw_hash.py
--rw-r--r--   0        0        0     7493 2023-04-10 19:17:54.481828 dcicsnovault-8.0.1.0b0/snovault/tests/test_embed_utils.py
--rw-r--r--   0        0        0     8823 2023-03-13 18:29:27.181151 dcicsnovault-8.0.1.0b0/snovault/tests/test_embedding.py
--rw-r--r--   0        0        0    10024 2020-04-22 15:19:59.916562 dcicsnovault-8.0.1.0b0/snovault/tests/test_es_permissions.py
--rw-r--r--   0        0        0   115140 2023-04-10 19:18:26.571266 dcicsnovault-8.0.1.0b0/snovault/tests/test_indexing.py
--rw-r--r--   0        0        0    28258 2023-02-08 18:10:49.984723 dcicsnovault-8.0.1.0b0/snovault/tests/test_invalidation_scope.py
--rw-r--r--   0        0        0     1808 2023-04-10 19:15:18.977778 dcicsnovault-8.0.1.0b0/snovault/tests/test_key.py
--rw-r--r--   0        0        0     2458 2020-04-22 15:19:59.908101 dcicsnovault-8.0.1.0b0/snovault/tests/test_link.py
--rw-r--r--   0        0        0     5316 2023-02-08 18:10:49.991255 dcicsnovault-8.0.1.0b0/snovault/tests/test_logging.py
--rw-r--r--   0        0        0     1134 2023-03-13 18:29:27.182699 dcicsnovault-8.0.1.0b0/snovault/tests/test_misc.py
--rw-r--r--   0        0        0      373 2020-09-25 18:48:35.895147 dcicsnovault-8.0.1.0b0/snovault/tests/test_mixins.py
--rw-r--r--   0        0        0    13660 2023-02-08 18:10:49.997635 dcicsnovault-8.0.1.0b0/snovault/tests/test_post_put_patch.py
--rw-r--r--   0        0        0     1570 2023-02-08 18:10:50.005697 dcicsnovault-8.0.1.0b0/snovault/tests/test_postgresql_fixture.py
--rw-r--r--   0        0        0     1194 2021-08-12 19:39:17.921857 dcicsnovault-8.0.1.0b0/snovault/tests/test_schemas.py
--rw-r--r--   0        0        0      952 2023-02-08 18:10:50.011548 dcicsnovault-8.0.1.0b0/snovault/tests/test_serverfixtures.py
--rw-r--r--   0        0        0     4267 2021-08-12 19:39:17.928403 dcicsnovault-8.0.1.0b0/snovault/tests/test_standalone_dev.py
--rw-r--r--   0        0        0     2211 2023-02-08 18:10:50.016544 dcicsnovault-8.0.1.0b0/snovault/tests/test_stats.py
--rw-r--r--   0        0        0    13182 2023-04-10 19:15:20.639545 dcicsnovault-8.0.1.0b0/snovault/tests/test_storage.py
--rw-r--r--   0        0        0     6782 2023-04-10 19:15:18.984951 dcicsnovault-8.0.1.0b0/snovault/tests/test_types_access_key.py
--rw-r--r--   0        0        0     1291 2020-04-22 15:19:59.901514 dcicsnovault-8.0.1.0b0/snovault/tests/test_upgrader.py
--rw-r--r--   0        0        0     6635 2023-02-08 18:10:50.017803 dcicsnovault-8.0.1.0b0/snovault/tests/test_util.py
--rw-r--r--   0        0        0    18612 2023-02-08 18:10:50.023759 dcicsnovault-8.0.1.0b0/snovault/tests/test_views.py
--rw-r--r--   0        0        0     4578 2023-04-10 19:15:18.986928 dcicsnovault-8.0.1.0b0/snovault/tests/testappfixtures.py
--rw-r--r--   0        0        0      677 2020-09-15 14:05:58.215585 dcicsnovault-8.0.1.0b0/snovault/tests/testing_upgrader.py
--rw-r--r--   0        0        0    34107 2023-04-13 14:14:38.777790 dcicsnovault-8.0.1.0b0/snovault/tests/testing_views.py
--rw-r--r--   0        0        0     1342 2020-09-15 14:05:58.228484 dcicsnovault-8.0.1.0b0/snovault/tests/toolfixtures.py
--rw-r--r--   0        0        0     4031 2023-04-07 15:35:45.690459 dcicsnovault-8.0.1.0b0/snovault/tools.py
--rw-r--r--   0        0        0     1807 2023-04-10 19:15:19.001310 dcicsnovault-8.0.1.0b0/snovault/typedsheets.py
--rw-r--r--   0        0        0     7605 2021-08-12 19:39:17.963916 dcicsnovault-8.0.1.0b0/snovault/typeinfo.py
--rw-r--r--   0        0        0       70 2023-04-10 19:15:19.007462 dcicsnovault-8.0.1.0b0/snovault/types/__init__.py
--rw-r--r--   0        0        0     5101 2023-04-10 19:15:19.012443 dcicsnovault-8.0.1.0b0/snovault/types/access_key.py
--rw-r--r--   0        0        0    16288 2023-04-10 19:15:19.017711 dcicsnovault-8.0.1.0b0/snovault/types/base.py
--rw-r--r--   0        0        0      738 2023-04-10 19:15:19.023321 dcicsnovault-8.0.1.0b0/snovault/types/filter_set.py
--rw-r--r--   0        0        0     5536 2023-04-10 19:15:19.028682 dcicsnovault-8.0.1.0b0/snovault/types/user.py
--rw-r--r--   0        0        0     8124 2023-02-08 18:10:50.037173 dcicsnovault-8.0.1.0b0/snovault/upgrader.py
--rw-r--r--   0        0        0    50126 2023-04-10 19:15:19.035305 dcicsnovault-8.0.1.0b0/snovault/util.py
--rw-r--r--   0        0        0     5460 2023-02-08 18:10:50.039101 dcicsnovault-8.0.1.0b0/snovault/validation.py
--rw-r--r--   0        0        0     5718 2023-02-08 18:10:50.044485 dcicsnovault-8.0.1.0b0/snovault/validators.py
--rw-r--r--   0        0        0     8848 1970-01-01 00:00:00.000000 dcicsnovault-8.0.1.0b0/setup.py
--rw-r--r--   0        0        0     9135 1970-01-01 00:00:00.000000 dcicsnovault-8.0.1.0b0/PKG-INFO
+-rw-r--r--   0        0        0     1135 2023-04-28 15:14:06.848052 dcicsnovault-8.0.1.0b1/LICENSE.txt
+-rw-r--r--   0        0        0     6407 2023-04-28 15:14:06.848052 dcicsnovault-8.0.1.0b1/README.rst
+-rw-r--r--   0        0        0     5597 2023-04-28 15:14:06.852052 dcicsnovault-8.0.1.0b1/pyproject.toml
+-rw-r--r--   0        0        0     4586 2023-04-28 15:14:06.852052 dcicsnovault-8.0.1.0b1/snovault/__init__.py
+-rw-r--r--   0        0        0     1942 2023-04-28 15:14:06.852052 dcicsnovault-8.0.1.0b1/snovault/aggregated_items.py
+-rw-r--r--   0        0        0     8799 2023-04-28 15:14:06.852052 dcicsnovault-8.0.1.0b1/snovault/app.py
+-rw-r--r--   0        0        0    11879 2023-04-28 15:14:06.852052 dcicsnovault-8.0.1.0b1/snovault/attachment.py
+-rw-r--r--   0        0        0    25327 2023-04-28 15:14:06.852052 dcicsnovault-8.0.1.0b1/snovault/authentication.py
+-rw-r--r--   0        0        0     4467 2023-04-28 15:14:06.852052 dcicsnovault-8.0.1.0b1/snovault/authorization.py
+-rw-r--r--   0        0        0     6670 2023-04-28 15:14:06.852052 dcicsnovault-8.0.1.0b1/snovault/batchupgrade.py
+-rw-r--r--   0        0        0     1902 2023-04-28 15:14:06.852052 dcicsnovault-8.0.1.0b1/snovault/cache.py
+-rw-r--r--   0        0        0     6461 2023-04-28 15:14:06.852052 dcicsnovault-8.0.1.0b1/snovault/calculated.py
+-rw-r--r--   0        0        0       10 2023-04-28 15:14:06.852052 dcicsnovault-8.0.1.0b1/snovault/commands/__init__.py
+-rw-r--r--   0        0        0     3416 2023-04-28 15:14:06.852052 dcicsnovault-8.0.1.0b1/snovault/commands/check_rendering.py
+-rw-r--r--   0        0        0     6813 2023-04-28 15:14:06.852052 dcicsnovault-8.0.1.0b1/snovault/commands/clear_db_es_contents.py
+-rw-r--r--   0        0        0     3928 2023-04-28 15:14:06.852052 dcicsnovault-8.0.1.0b1/snovault/commands/create_mapping_on_deploy.py
+-rw-r--r--   0        0        0     1608 2023-04-28 15:14:06.852052 dcicsnovault-8.0.1.0b1/snovault/commands/es_index_data.py
+-rw-r--r--   0        0        0     1644 2023-04-28 15:14:06.852052 dcicsnovault-8.0.1.0b1/snovault/commands/jsonld_rdf.py
+-rw-r--r--   0        0        0     6212 2023-04-28 15:14:06.852052 dcicsnovault-8.0.1.0b1/snovault/commands/load_access_keys.py
+-rw-r--r--   0        0        0     2402 2023-04-28 15:14:06.852052 dcicsnovault-8.0.1.0b1/snovault/commands/load_data.py
+-rw-r--r--   0        0        0     2188 2023-04-28 15:14:06.852052 dcicsnovault-8.0.1.0b1/snovault/commands/load_data_by_type.py
+-rw-r--r--   0        0        0     4350 2023-04-28 15:14:06.852052 dcicsnovault-8.0.1.0b1/snovault/commands/profile.py
+-rw-r--r--   0        0        0     3236 2023-04-28 15:14:06.852052 dcicsnovault-8.0.1.0b1/snovault/commands/purge_item_type.py
+-rw-r--r--   0        0        0     1868 2023-04-28 15:14:06.852052 dcicsnovault-8.0.1.0b1/snovault/commands/run_upgrader_on_inserts.py
+-rw-r--r--   0        0        0     8533 2023-04-28 15:14:06.852052 dcicsnovault-8.0.1.0b1/snovault/commands/update_inserts_from_server.py
+-rw-r--r--   0        0        0      909 2023-04-28 15:14:06.852052 dcicsnovault-8.0.1.0b1/snovault/commands/wipe_test_indices.py
+-rw-r--r--   0        0        0     4183 2023-04-28 15:14:06.852052 dcicsnovault-8.0.1.0b1/snovault/config.py
+-rw-r--r--   0        0        0     6352 2023-04-28 15:14:06.852052 dcicsnovault-8.0.1.0b1/snovault/connection.py
+-rw-r--r--   0        0        0    14798 2023-04-28 15:14:06.852052 dcicsnovault-8.0.1.0b1/snovault/crud_views.py
+-rw-r--r--   0        0        0    15301 2023-04-28 15:14:06.852052 dcicsnovault-8.0.1.0b1/snovault/custom_embed.py
+-rw-r--r--   0        0        0     7216 2023-04-28 15:14:06.852052 dcicsnovault-8.0.1.0b1/snovault/dev_servers.py
+-rw-r--r--   0        0        0     4340 2023-04-28 15:14:06.852052 dcicsnovault-8.0.1.0b1/snovault/drs.py
+-rw-r--r--   0        0        0     1829 2023-04-28 15:14:06.852052 dcicsnovault-8.0.1.0b1/snovault/edw_hash.py
+-rw-r--r--   0        0        0     4282 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/elasticsearch/__init__.py
+-rw-r--r--   0        0        0     4727 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/elasticsearch/cached_views.py
+-rw-r--r--   0        0        0    61320 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/elasticsearch/create_mapping.py
+-rw-r--r--   0        0        0     7939 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/elasticsearch/es_index_listener.py
+-rw-r--r--   0        0        0    18572 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/elasticsearch/esstorage.py
+-rw-r--r--   0        0        0    24405 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/elasticsearch/indexer.py
+-rw-r--r--   0        0        0    31356 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/elasticsearch/indexer_queue.py
+-rw-r--r--   0        0        0    20947 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/elasticsearch/indexer_utils.py
+-rw-r--r--   0        0        0      349 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/elasticsearch/interfaces.py
+-rw-r--r--   0        0        0    10190 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/elasticsearch/mpindexer.py
+-rw-r--r--   0        0        0     8249 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/embed.py
+-rw-r--r--   0        0        0     1061 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/etag.py
+-rw-r--r--   0        0        0    10835 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/indexing_views.py
+-rw-r--r--   0        0        0      774 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/interfaces.py
+-rw-r--r--   0        0        0     2229 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/invalidation.py
+-rw-r--r--   0        0        0     1639 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/json_renderer.py
+-rw-r--r--   0        0        0     2292 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/jsongraph.py
+-rw-r--r--   0        0        0     9713 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/jsonld_context.py
+-rw-r--r--   0        0        0    30294 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/loadxl.py
+-rw-r--r--   0        0        0     2425 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/memlimit.py
+-rw-r--r--   0        0        0     1165 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/parallel.py
+-rw-r--r--   0        0        0      846 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/predicates.py
+-rw-r--r--   0        0        0       95 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/redis/README.rst
+-rw-r--r--   0        0        0       90 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/redis/__init__.py
+-rw-r--r--   0        0        0       16 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/redis/interfaces.py
+-rw-r--r--   0        0        0     4106 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/redis/redis_connection.py
+-rw-r--r--   0        0        0    22128 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/renderers.py
+-rw-r--r--   0        0        0    11201 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/resource_views.py
+-rw-r--r--   0        0        0    21863 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/resources.py
+-rw-r--r--   0        0        0     3450 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/schema_graph.py
+-rw-r--r--   0        0        0    14162 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/schema_utils.py
+-rw-r--r--   0        0        0     4358 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/schema_views.py
+-rw-r--r--   0        0        0     1855 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/schemas/access_key.json
+-rw-r--r--   0        0        0     5098 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/schemas/filter_set.json
+-rw-r--r--   0        0        0    18744 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/schemas/mixins.json
+-rw-r--r--   0        0        0    19600 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/schemas/user.json
+-rw-r--r--   0        0        0    20952 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/search/compound_search.py
+-rw-r--r--   0        0        0    58595 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/search/lucene_builder.py
+-rw-r--r--   0        0        0    62789 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/search/search.py
+-rw-r--r--   0        0        0    17901 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/search/search_utils.py
+-rw-r--r--   0        0        0     4541 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/server_defaults.py
+-rw-r--r--   0        0        0      522 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/settings.py
+-rw-r--r--   0        0        0     1498 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/standalone_dev.py
+-rw-r--r--   0        0        0     4383 2023-04-28 15:14:06.856052 dcicsnovault-8.0.1.0b1/snovault/stats.py
+-rw-r--r--   0        0        0    34834 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/storage.py
+-rw-r--r--   0        0        0      330 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/test_schemas/AbstractItemTestSecondSubItem.json
+-rw-r--r--   0        0        0      300 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/test_schemas/AbstractItemTestSubItem.json
+-rw-r--r--   0        0        0     2467 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/test_schemas/EmbeddingTest.json
+-rw-r--r--   0        0        0      446 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/test_schemas/NestedEmbeddingContainer.json
+-rw-r--r--   0        0        0      883 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/test_schemas/NestedObjectLinkTarget.json
+-rw-r--r--   0        0        0      473 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/test_schemas/TestingBiogroupSno.json
+-rw-r--r--   0        0        0      968 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/test_schemas/TestingBiosampleSno.json
+-rw-r--r--   0        0        0     1082 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/test_schemas/TestingBiosourceSno.json
+-rw-r--r--   0        0        0      894 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/test_schemas/TestingCalculatedProperties.json
+-rw-r--r--   0        0        0      276 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/test_schemas/TestingDependencies.json
+-rw-r--r--   0        0        0      697 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/test_schemas/TestingDownload.json
+-rw-r--r--   0        0        0      555 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/test_schemas/TestingIndividualSno.json
+-rw-r--r--   0        0        0      730 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/test_schemas/TestingLinkAggregateSno.json
+-rw-r--r--   0        0        0      697 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/test_schemas/TestingLinkSourceSno.json
+-rw-r--r--   0        0        0      472 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/test_schemas/TestingLinkTargetElasticSearch.json
+-rw-r--r--   0        0        0      292 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/test_schemas/TestingLinkTargetSno.json
+-rw-r--r--   0        0        0      311 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/test_schemas/TestingMixins.json
+-rw-r--r--   0        0        0      845 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/test_schemas/TestingNestedEnabled.json
+-rw-r--r--   0        0        0     3721 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/test_schemas/TestingNoteSno.json
+-rw-r--r--   0        0        0     1622 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/test_schemas/TestingPostPutPatchSno.json
+-rw-r--r--   0        0        0      576 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/test_schemas/TestingServerDefault.json
+-rw-r--r--   0        0        0     1215 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/test_schemas/mixins.json
+-rw-r--r--   0        0        0        0 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/__init__.py
+-rw-r--r--   0        0        0     2210 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/conftest.py
+-rw-r--r--   0        0        0      100 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/conftest_settings.py
+-rw-r--r--   0        0        0     3086 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/elasticsearch_fixture.py
+-rw-r--r--   0        0        0     3921 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/postgresql_fixture.py
+-rw-r--r--   0        0        0      852 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/pyramidfixtures.py
+-rw-r--r--   0        0        0     3007 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/root.py
+-rw-r--r--   0        0        0    17313 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/serverfixtures.py
+-rw-r--r--   0        0        0    20332 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/test_attachment.py
+-rw-r--r--   0        0        0     3937 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/test_authentication.py
+-rw-r--r--   0        0        0     1370 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/test_calculated.py
+-rw-r--r--   0        0        0    15979 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/test_clear_db_es_contents.py
+-rw-r--r--   0        0        0     8984 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/test_create_mapping.py
+-rw-r--r--   0        0        0     3173 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/test_drs.py
+-rw-r--r--   0        0        0      528 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/test_edw_hash.py
+-rw-r--r--   0        0        0     7493 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/test_embed_utils.py
+-rw-r--r--   0        0        0     8823 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/test_embedding.py
+-rw-r--r--   0        0        0    10024 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/test_es_permissions.py
+-rw-r--r--   0        0        0   115140 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/test_indexing.py
+-rw-r--r--   0        0        0    28258 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/test_invalidation_scope.py
+-rw-r--r--   0        0        0     1808 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/test_key.py
+-rw-r--r--   0        0        0     2458 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/test_link.py
+-rw-r--r--   0        0        0     5316 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/test_logging.py
+-rw-r--r--   0        0        0     1134 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/test_misc.py
+-rw-r--r--   0        0        0      373 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/test_mixins.py
+-rw-r--r--   0        0        0    13660 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/test_post_put_patch.py
+-rw-r--r--   0        0        0     1570 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/test_postgresql_fixture.py
+-rw-r--r--   0        0        0     1194 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/test_schemas.py
+-rw-r--r--   0        0        0      952 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/test_serverfixtures.py
+-rw-r--r--   0        0        0     4267 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/test_standalone_dev.py
+-rw-r--r--   0        0        0     2211 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/test_stats.py
+-rw-r--r--   0        0        0    13182 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/test_storage.py
+-rw-r--r--   0        0        0     6782 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/test_types_access_key.py
+-rw-r--r--   0        0        0     1291 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/test_upgrader.py
+-rw-r--r--   0        0        0     6635 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/test_util.py
+-rw-r--r--   0        0        0    18612 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/test_views.py
+-rw-r--r--   0        0        0     4578 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/testappfixtures.py
+-rw-r--r--   0        0        0      677 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/testing_upgrader.py
+-rw-r--r--   0        0        0    34107 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/testing_views.py
+-rw-r--r--   0        0        0     1342 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tests/toolfixtures.py
+-rw-r--r--   0        0        0     4031 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/tools.py
+-rw-r--r--   0        0        0     1807 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/typedsheets.py
+-rw-r--r--   0        0        0     7605 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/typeinfo.py
+-rw-r--r--   0        0        0       70 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/types/__init__.py
+-rw-r--r--   0        0        0     5101 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/types/access_key.py
+-rw-r--r--   0        0        0    16288 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/types/base.py
+-rw-r--r--   0        0        0      738 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/types/filter_set.py
+-rw-r--r--   0        0        0     5536 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/types/user.py
+-rw-r--r--   0        0        0     8124 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/upgrader.py
+-rw-r--r--   0        0        0    51788 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/util.py
+-rw-r--r--   0        0        0     5460 2023-04-28 15:14:06.860052 dcicsnovault-8.0.1.0b1/snovault/validation.py
+-rw-r--r--   0        0        0     5718 2023-04-28 15:14:06.864052 dcicsnovault-8.0.1.0b1/snovault/validators.py
+-rw-r--r--   0        0        0     9135 1970-01-01 00:00:00.000000 dcicsnovault-8.0.1.0b1/PKG-INFO
```

### Comparing `dcicsnovault-8.0.1.0b0/LICENSE.txt` & `dcicsnovault-8.0.1.0b1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/README.rst` & `dcicsnovault-8.0.1.0b1/README.rst`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/pyproject.toml` & `dcicsnovault-8.0.1.0b1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dcicsnovault"
-version = "8.0.1.0b0"  # to become 8.1.0
+version = "8.0.1.0b1"  # to become 8.1.0
 description = "Storage support for 4DN Data Portals."
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/4dn-dcic/snovault"
 repository = "https://github.com/4dn-dcic/snovault"
 documentation = "https://github.com/4dn-dcic/snovault"
```

### Comparing `dcicsnovault-8.0.1.0b0/snovault/__init__.py` & `dcicsnovault-8.0.1.0b1/snovault/__init__.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/aggregated_items.py` & `dcicsnovault-8.0.1.0b1/snovault/aggregated_items.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/app.py` & `dcicsnovault-8.0.1.0b1/snovault/app.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/attachment.py` & `dcicsnovault-8.0.1.0b1/snovault/attachment.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/authentication.py` & `dcicsnovault-8.0.1.0b1/snovault/authentication.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/authorization.py` & `dcicsnovault-8.0.1.0b1/snovault/authorization.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/batchupgrade.py` & `dcicsnovault-8.0.1.0b1/snovault/batchupgrade.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/cache.py` & `dcicsnovault-8.0.1.0b1/snovault/cache.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/calculated.py` & `dcicsnovault-8.0.1.0b1/snovault/calculated.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/commands/check_rendering.py` & `dcicsnovault-8.0.1.0b1/snovault/commands/check_rendering.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/commands/clear_db_es_contents.py` & `dcicsnovault-8.0.1.0b1/snovault/commands/clear_db_es_contents.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/commands/create_mapping_on_deploy.py` & `dcicsnovault-8.0.1.0b1/snovault/commands/create_mapping_on_deploy.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/commands/es_index_data.py` & `dcicsnovault-8.0.1.0b1/snovault/commands/es_index_data.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/commands/jsonld_rdf.py` & `dcicsnovault-8.0.1.0b1/snovault/commands/jsonld_rdf.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/commands/load_access_keys.py` & `dcicsnovault-8.0.1.0b1/snovault/commands/load_access_keys.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/commands/load_data.py` & `dcicsnovault-8.0.1.0b1/snovault/commands/load_data.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/commands/load_data_by_type.py` & `dcicsnovault-8.0.1.0b1/snovault/commands/load_data_by_type.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/commands/profile.py` & `dcicsnovault-8.0.1.0b1/snovault/commands/profile.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/commands/purge_item_type.py` & `dcicsnovault-8.0.1.0b1/snovault/commands/purge_item_type.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/commands/run_upgrader_on_inserts.py` & `dcicsnovault-8.0.1.0b1/snovault/commands/run_upgrader_on_inserts.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/commands/update_inserts_from_server.py` & `dcicsnovault-8.0.1.0b1/snovault/commands/update_inserts_from_server.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/commands/wipe_test_indices.py` & `dcicsnovault-8.0.1.0b1/snovault/commands/wipe_test_indices.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/config.py` & `dcicsnovault-8.0.1.0b1/snovault/config.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/connection.py` & `dcicsnovault-8.0.1.0b1/snovault/connection.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/crud_views.py` & `dcicsnovault-8.0.1.0b1/snovault/crud_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/custom_embed.py` & `dcicsnovault-8.0.1.0b1/snovault/custom_embed.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/dev_servers.py` & `dcicsnovault-8.0.1.0b1/snovault/dev_servers.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/drs.py` & `dcicsnovault-8.0.1.0b1/snovault/drs.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/edw_hash.py` & `dcicsnovault-8.0.1.0b1/snovault/edw_hash.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/elasticsearch/__init__.py` & `dcicsnovault-8.0.1.0b1/snovault/elasticsearch/__init__.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/elasticsearch/cached_views.py` & `dcicsnovault-8.0.1.0b1/snovault/elasticsearch/cached_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/elasticsearch/create_mapping.py` & `dcicsnovault-8.0.1.0b1/snovault/elasticsearch/create_mapping.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/elasticsearch/es_index_listener.py` & `dcicsnovault-8.0.1.0b1/snovault/elasticsearch/es_index_listener.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/elasticsearch/esstorage.py` & `dcicsnovault-8.0.1.0b1/snovault/elasticsearch/esstorage.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/elasticsearch/indexer.py` & `dcicsnovault-8.0.1.0b1/snovault/elasticsearch/indexer.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/elasticsearch/indexer_queue.py` & `dcicsnovault-8.0.1.0b1/snovault/elasticsearch/indexer_queue.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/elasticsearch/indexer_utils.py` & `dcicsnovault-8.0.1.0b1/snovault/elasticsearch/indexer_utils.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/elasticsearch/mpindexer.py` & `dcicsnovault-8.0.1.0b1/snovault/elasticsearch/mpindexer.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/embed.py` & `dcicsnovault-8.0.1.0b1/snovault/embed.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/etag.py` & `dcicsnovault-8.0.1.0b1/snovault/etag.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/indexing_views.py` & `dcicsnovault-8.0.1.0b1/snovault/indexing_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/interfaces.py` & `dcicsnovault-8.0.1.0b1/snovault/interfaces.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/invalidation.py` & `dcicsnovault-8.0.1.0b1/snovault/invalidation.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/json_renderer.py` & `dcicsnovault-8.0.1.0b1/snovault/json_renderer.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/jsongraph.py` & `dcicsnovault-8.0.1.0b1/snovault/jsongraph.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/jsonld_context.py` & `dcicsnovault-8.0.1.0b1/snovault/jsonld_context.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/loadxl.py` & `dcicsnovault-8.0.1.0b1/snovault/loadxl.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/memlimit.py` & `dcicsnovault-8.0.1.0b1/snovault/memlimit.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/parallel.py` & `dcicsnovault-8.0.1.0b1/snovault/parallel.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/predicates.py` & `dcicsnovault-8.0.1.0b1/snovault/predicates.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/redis/redis_connection.py` & `dcicsnovault-8.0.1.0b1/snovault/redis/redis_connection.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/renderers.py` & `dcicsnovault-8.0.1.0b1/snovault/renderers.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/resource_views.py` & `dcicsnovault-8.0.1.0b1/snovault/resource_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/resources.py` & `dcicsnovault-8.0.1.0b1/snovault/resources.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/schema_graph.py` & `dcicsnovault-8.0.1.0b1/snovault/schema_graph.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/schema_utils.py` & `dcicsnovault-8.0.1.0b1/snovault/schema_utils.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/schema_views.py` & `dcicsnovault-8.0.1.0b1/snovault/schema_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/schemas/access_key.json` & `dcicsnovault-8.0.1.0b1/snovault/schemas/access_key.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/schemas/filter_set.json` & `dcicsnovault-8.0.1.0b1/snovault/schemas/filter_set.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/schemas/mixins.json` & `dcicsnovault-8.0.1.0b1/snovault/schemas/mixins.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/schemas/user.json` & `dcicsnovault-8.0.1.0b1/snovault/schemas/user.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/search/compound_search.py` & `dcicsnovault-8.0.1.0b1/snovault/search/compound_search.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/search/lucene_builder.py` & `dcicsnovault-8.0.1.0b1/snovault/search/lucene_builder.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/search/search.py` & `dcicsnovault-8.0.1.0b1/snovault/search/search.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/search/search_utils.py` & `dcicsnovault-8.0.1.0b1/snovault/search/search_utils.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/server_defaults.py` & `dcicsnovault-8.0.1.0b1/snovault/server_defaults.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/settings.py` & `dcicsnovault-8.0.1.0b1/snovault/settings.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/standalone_dev.py` & `dcicsnovault-8.0.1.0b1/snovault/standalone_dev.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/stats.py` & `dcicsnovault-8.0.1.0b1/snovault/stats.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/storage.py` & `dcicsnovault-8.0.1.0b1/snovault/storage.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/test_schemas/EmbeddingTest.json` & `dcicsnovault-8.0.1.0b1/snovault/test_schemas/EmbeddingTest.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/test_schemas/NestedObjectLinkTarget.json` & `dcicsnovault-8.0.1.0b1/snovault/test_schemas/NestedObjectLinkTarget.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/test_schemas/TestingBiosampleSno.json` & `dcicsnovault-8.0.1.0b1/snovault/test_schemas/TestingBiosampleSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/test_schemas/TestingBiosourceSno.json` & `dcicsnovault-8.0.1.0b1/snovault/test_schemas/TestingBiosourceSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/test_schemas/TestingCalculatedProperties.json` & `dcicsnovault-8.0.1.0b1/snovault/test_schemas/TestingCalculatedProperties.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/test_schemas/TestingDownload.json` & `dcicsnovault-8.0.1.0b1/snovault/test_schemas/TestingDownload.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/test_schemas/TestingIndividualSno.json` & `dcicsnovault-8.0.1.0b1/snovault/test_schemas/TestingIndividualSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/test_schemas/TestingLinkAggregateSno.json` & `dcicsnovault-8.0.1.0b1/snovault/test_schemas/TestingLinkAggregateSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/test_schemas/TestingLinkSourceSno.json` & `dcicsnovault-8.0.1.0b1/snovault/test_schemas/TestingLinkSourceSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/test_schemas/TestingNestedEnabled.json` & `dcicsnovault-8.0.1.0b1/snovault/test_schemas/TestingNestedEnabled.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/test_schemas/TestingNoteSno.json` & `dcicsnovault-8.0.1.0b1/snovault/test_schemas/TestingNoteSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/test_schemas/TestingPostPutPatchSno.json` & `dcicsnovault-8.0.1.0b1/snovault/test_schemas/TestingPostPutPatchSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/test_schemas/TestingServerDefault.json` & `dcicsnovault-8.0.1.0b1/snovault/test_schemas/TestingServerDefault.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/test_schemas/mixins.json` & `dcicsnovault-8.0.1.0b1/snovault/test_schemas/mixins.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/tests/conftest.py` & `dcicsnovault-8.0.1.0b1/snovault/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/tests/elasticsearch_fixture.py` & `dcicsnovault-8.0.1.0b1/snovault/tests/elasticsearch_fixture.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/tests/postgresql_fixture.py` & `dcicsnovault-8.0.1.0b1/snovault/tests/postgresql_fixture.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/tests/pyramidfixtures.py` & `dcicsnovault-8.0.1.0b1/snovault/tests/pyramidfixtures.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/tests/root.py` & `dcicsnovault-8.0.1.0b1/snovault/tests/root.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/tests/serverfixtures.py` & `dcicsnovault-8.0.1.0b1/snovault/tests/serverfixtures.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/tests/test_attachment.py` & `dcicsnovault-8.0.1.0b1/snovault/tests/test_attachment.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/tests/test_authentication.py` & `dcicsnovault-8.0.1.0b1/snovault/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/tests/test_calculated.py` & `dcicsnovault-8.0.1.0b1/snovault/tests/test_calculated.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/tests/test_clear_db_es_contents.py` & `dcicsnovault-8.0.1.0b1/snovault/tests/test_clear_db_es_contents.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/tests/test_create_mapping.py` & `dcicsnovault-8.0.1.0b1/snovault/tests/test_create_mapping.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/tests/test_drs.py` & `dcicsnovault-8.0.1.0b1/snovault/tests/test_drs.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/tests/test_edw_hash.py` & `dcicsnovault-8.0.1.0b1/snovault/tests/test_edw_hash.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/tests/test_embed_utils.py` & `dcicsnovault-8.0.1.0b1/snovault/tests/test_embed_utils.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/tests/test_embedding.py` & `dcicsnovault-8.0.1.0b1/snovault/tests/test_embedding.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/tests/test_es_permissions.py` & `dcicsnovault-8.0.1.0b1/snovault/tests/test_es_permissions.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/tests/test_indexing.py` & `dcicsnovault-8.0.1.0b1/snovault/tests/test_indexing.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/tests/test_invalidation_scope.py` & `dcicsnovault-8.0.1.0b1/snovault/tests/test_invalidation_scope.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/tests/test_key.py` & `dcicsnovault-8.0.1.0b1/snovault/tests/test_key.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/tests/test_link.py` & `dcicsnovault-8.0.1.0b1/snovault/tests/test_link.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/tests/test_logging.py` & `dcicsnovault-8.0.1.0b1/snovault/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/tests/test_misc.py` & `dcicsnovault-8.0.1.0b1/snovault/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/tests/test_post_put_patch.py` & `dcicsnovault-8.0.1.0b1/snovault/tests/test_post_put_patch.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/tests/test_postgresql_fixture.py` & `dcicsnovault-8.0.1.0b1/snovault/tests/test_postgresql_fixture.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/tests/test_schemas.py` & `dcicsnovault-8.0.1.0b1/snovault/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/tests/test_serverfixtures.py` & `dcicsnovault-8.0.1.0b1/snovault/tests/test_serverfixtures.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/tests/test_standalone_dev.py` & `dcicsnovault-8.0.1.0b1/snovault/tests/test_standalone_dev.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/tests/test_stats.py` & `dcicsnovault-8.0.1.0b1/snovault/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/tests/test_storage.py` & `dcicsnovault-8.0.1.0b1/snovault/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/tests/test_types_access_key.py` & `dcicsnovault-8.0.1.0b1/snovault/tests/test_types_access_key.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/tests/test_upgrader.py` & `dcicsnovault-8.0.1.0b1/snovault/tests/test_upgrader.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/tests/test_util.py` & `dcicsnovault-8.0.1.0b1/snovault/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/tests/test_views.py` & `dcicsnovault-8.0.1.0b1/snovault/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/tests/testappfixtures.py` & `dcicsnovault-8.0.1.0b1/snovault/tests/testappfixtures.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/tests/testing_upgrader.py` & `dcicsnovault-8.0.1.0b1/snovault/tests/testing_upgrader.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/tests/testing_views.py` & `dcicsnovault-8.0.1.0b1/snovault/tests/testing_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/tests/toolfixtures.py` & `dcicsnovault-8.0.1.0b1/snovault/tests/toolfixtures.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/tools.py` & `dcicsnovault-8.0.1.0b1/snovault/tools.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/typedsheets.py` & `dcicsnovault-8.0.1.0b1/snovault/typedsheets.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/typeinfo.py` & `dcicsnovault-8.0.1.0b1/snovault/typeinfo.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/types/access_key.py` & `dcicsnovault-8.0.1.0b1/snovault/types/access_key.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/types/base.py` & `dcicsnovault-8.0.1.0b1/snovault/types/base.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/types/filter_set.py` & `dcicsnovault-8.0.1.0b1/snovault/types/filter_set.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/types/user.py` & `dcicsnovault-8.0.1.0b1/snovault/types/user.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/upgrader.py` & `dcicsnovault-8.0.1.0b1/snovault/upgrader.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/util.py` & `dcicsnovault-8.0.1.0b1/snovault/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,23 @@
 import datetime as datetime_module
 import functools
 import json
 import os
 import structlog
 import sys
 import re
+import boto3
 
+from botocore.client import Config
 from copy import copy
 from datetime import datetime, timedelta
 from pyramid.httpexceptions import HTTPForbidden
 from pyramid.threadlocal import manager as threadlocal_manager
+from dcicutils.secrets_utils import assume_identity
+from dcicutils.ecs_utils import ECSUtils
 
 from .interfaces import CONNECTION, STORAGE, TYPES
 from .settings import Settings
 
 
 log = structlog.getLogger(__name__)
 
@@ -1179,7 +1183,44 @@
             elif isinstance(path_condition, compiled_regexp_class):
                 if path_condition.match(request.path):
                     return True
             else:
                 raise NotImplementedError(f"Unrecognized path_condition: {path_condition}")
 
     return False
+
+
+def check_user_is_logged_in(request):
+    """ Raises HTTPForbidden if the request did not come from a logged in user. """
+    for principal in request.effective_principals:
+        if principal.startswith('userid.') or principal == 'group.admin':  # allow if logged in OR has admin
+            break
+    else:
+        raise HTTPForbidden(title="Not logged in.")
+
+
+def make_s3_client():
+    s3_client_extra_args = {}
+    if 'IDENTITY' in os.environ:
+        identity = assume_identity()
+        s3_client_extra_args['aws_access_key_id'] = key_id = identity.get('S3_AWS_ACCESS_KEY_ID')
+        s3_client_extra_args['aws_secret_access_key'] = identity.get('S3_AWS_SECRET_ACCESS_KEY')
+        s3_client_extra_args['region_name'] = ECSUtils.REGION
+        log.warning(f"make_s3_client using S3 entity ID {key_id[:10]} arguments in `boto3 client creation call.")
+        if 'ENCODED_S3_ENCRYPT_KEY_ID' in identity:
+            # This setting is required when testing locally and encrypted buckets need to be accessed.
+            s3_client_extra_args['config'] = Config(signature_version='s3v4')
+    else:
+        log.warning(f'make_s3_client called with no identity')
+
+    s3_client = boto3.client('s3', **s3_client_extra_args)
+    return s3_client
+
+
+def build_s3_presigned_get_url(*, params):
+    """ Helper function that builds a presigned URL. """
+    s3_client = make_s3_client()
+    return s3_client.generate_presigned_url(
+        ClientMethod='get_object',
+        Params=params,
+        ExpiresIn=36 * 60 * 60
+    )
```

### Comparing `dcicsnovault-8.0.1.0b0/snovault/validation.py` & `dcicsnovault-8.0.1.0b1/snovault/validation.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/snovault/validators.py` & `dcicsnovault-8.0.1.0b1/snovault/validators.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.0b0/PKG-INFO` & `dcicsnovault-8.0.1.0b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcicsnovault
-Version: 8.0.1.0b0
+Version: 8.0.1.0b1
 Summary: Storage support for 4DN Data Portals.
 Home-page: https://github.com/4dn-dcic/snovault
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.8.1,<3.10
 Classifier: Development Status :: 4 - Beta
```

