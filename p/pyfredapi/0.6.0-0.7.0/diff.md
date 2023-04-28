# Comparing `tmp/pyfredapi-0.6.0.tar.gz` & `tmp/pyfredapi-0.7.0.tar.gz`

## Comparing `pyfredapi-0.6.0.tar` & `pyfredapi-0.7.0.tar`

### file list

```diff
@@ -1,158 +1,164 @@
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/.flake8
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/.readthedocs.yml
--rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/RELEASE.md
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/mypy.ini
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/requirements.txt
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/sonar-project.properties
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tox.ini
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/.github/PULL_REQUEST_TEMPLATE/version_release.md
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/.github/workflows/build-pyfredapi.yml
--rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/.github/workflows/sonarcloud.yml
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/.github/workflows/test.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/.nojekyll
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/Makefile
--rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/conf.py
--rw-r--r--   0        0        0     2489 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/make.bat
--rw-r--r--   0        0        0     7992 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/requirements.txt
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/_templates/layout.html
--rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/CHANGELOG.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/CONTRIBUTING.rst
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/api.rst
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.category.CategoryApiParameters.rst
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.category.get_category.rst
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.category.get_category_children.rst
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.category.get_category_related.rst
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.category.get_category_related_tags.rst
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.category.get_category_series.rst
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.category.get_category_tags.rst
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.maps.MapApiParameters.rst
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.maps.get_geoseries.rst
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.maps.get_geoseries_info.rst
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.maps.get_shape_files.rst
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.series.SeriesApiParameters.rst
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.series.SeriesInfo.rst
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.series.SeriesSearchParameters.rst
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.series.get_series.rst
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.series.get_series_all_releases.rst
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.series.get_series_asof_date.rst
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.series.get_series_categories.rst
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.series.get_series_info.rst
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.series.get_series_initial_release.rst
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.series.get_series_releases.rst
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.series.get_series_tags.rst
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.series.get_series_updates.rst
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.series.get_series_vintagedates.rst
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.series.search_series.rst
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.series.search_series_related_tags.rst
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.series.search_series_tags.rst
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.series_collection.SeriesCollection.rst
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.series_collection.SeriesData.rst
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.sources.SourceApiParameters.rst
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.sources.get_source.rst
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.sources.get_source_release.rst
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.sources.get_sources.rst
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.tags.TagsApiParameters.rst
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.tags.get_related_tags.rst
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.tags.get_series_matching_tags.rst
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.tags.get_tags.rst
--rw-r--r--   0        0        0    51352 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/tutorials/maps.ipynb
--rw-r--r--   0        0        0    26996 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/tutorials/series.ipynb
--rw-r--r--   0        0        0  3857297 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/docs/tutorials/series_collection.ipynb
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/pyfredapi/__about__.py
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/pyfredapi/__init__.py
--rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/pyfredapi/_base.py
--rw-r--r--   0        0        0     8441 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/pyfredapi/category.py
--rw-r--r--   0        0        0     5794 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/pyfredapi/maps.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/pyfredapi/py.typed
--rw-r--r--   0        0        0     9561 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/pyfredapi/releases.py
--rw-r--r--   0        0        0    20891 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/pyfredapi/series.py
--rw-r--r--   0        0        0    13493 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/pyfredapi/series_collection.py
--rw-r--r--   0        0        0     3570 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/pyfredapi/sources.py
--rw-r--r--   0        0        0     4337 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/pyfredapi/tags.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/pyfredapi/exceptions/__init__.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/pyfredapi/exceptions/exceptions.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/pyfredapi/utils/__init__.py
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/pyfredapi/utils/_common_type_hints.py
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/pyfredapi/utils/_convert_to_pandas.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/pyfredapi/utils/enums.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/__init__.py
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/conftest.py
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/test_base.py
--rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/test_category.py
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/test_maps.py
--rw-r--r--   0        0        0     2902 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/test_release.py
--rw-r--r--   0        0        0     7245 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/test_series.py
--rw-r--r--   0        0        0     4515 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/test_series_collection.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/test_sources.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/test_tags.py
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_category/test_get_category.yaml
--rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_category/test_get_category_children.yaml
--rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_category/test_get_category_related.yaml
--rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_category/test_get_category_related_tags[json].yaml
--rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_category/test_get_category_related_tags[pandas].yaml
--rw-r--r--   0        0        0    10367 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_category/test_get_category_series.yaml
--rw-r--r--   0        0        0     4353 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_category/test_get_category_tags[json].yaml
--rw-r--r--   0        0        0     4353 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_category/test_get_category_tags[pandas].yaml
--rw-r--r--   0        0        0    11038 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_maps/test_get_geoseries[json].yaml
--rw-r--r--   0        0        0    11181 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_maps/test_get_geoseries[pandas].yaml
--rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_maps/test_get_geoseries_info.yaml
--rw-r--r--   0        0        0    64017 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_maps/test_get_shape_files.yaml
--rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_release/test_get_release.yaml
--rw-r--r--   0        0        0    16989 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_release/test_get_release_dates.yaml
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_release/test_get_release_related_tags.yaml
--rw-r--r--   0        0        0    60220 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_release/test_get_release_series.yaml
--rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_release/test_get_release_sources.yaml
--rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_release/test_get_release_tables.yaml
--rw-r--r--   0        0        0    14156 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_release/test_get_release_tags.yaml
--rw-r--r--   0        0        0   153657 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_release/test_get_releases.yaml
--rw-r--r--   0        0        0    35336 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_release/test_get_releases_dates.yaml
--rw-r--r--   0        0        0    16234 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series/test_get_series[json].yaml
--rw-r--r--   0        0        0    16234 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series/test_get_series[pandas].yaml
--rw-r--r--   0        0        0   121930 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series/test_get_series_all_releases[json].yaml
--rw-r--r--   0        0        0   121930 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series/test_get_series_all_releases[pandas].yaml
--rw-r--r--   0        0        0   111804 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series/test_get_series_asof_date[json].yaml
--rw-r--r--   0        0        0   111807 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series/test_get_series_asof_date[pandas].yaml
--rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series/test_get_series_categories.yaml
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series/test_get_series_info.yaml
--rw-r--r--   0        0        0    13320 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series/test_get_series_initial_release[json].yaml
--rw-r--r--   0        0        0    13320 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series/test_get_series_initial_release[pandas].yaml
--rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series/test_get_series_releases.yaml
--rw-r--r--   0        0        0     3650 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series/test_get_series_tags.yaml
--rw-r--r--   0        0        0   137616 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series/test_get_series_updates.yaml
--rw-r--r--   0        0        0     7814 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series/test_get_series_vintagedates.yaml
--rw-r--r--   0        0        0    98930 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series/test_search_series[json].yaml
--rw-r--r--   0        0        0    99086 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series/test_search_series[pandas].yaml
--rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series/test_search_series_related_tags[json].yaml
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series/test_search_series_related_tags[pandas].yaml
--rw-r--r--   0        0        0    27622 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series/test_search_series_tags[json].yaml
--rw-r--r--   0        0        0    27627 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series/test_search_series_tags[pandas].yaml
--rw-r--r--   0        0        0    17912 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series_collection/test_add_series.yaml
--rw-r--r--   0        0        0    17911 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series_collection/test_keep_realtime_cols.yaml
--rw-r--r--   0        0        0    64575 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series_collection/test_list_methods_diff.yaml
--rw-r--r--   0        0        0    17910 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series_collection/test_list_methods_same.yaml
--rw-r--r--   0        0        0    32224 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series_collection/test_merge_asof.yaml
--rw-r--r--   0        0        0    32224 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series_collection/test_merge_long.yaml
--rw-r--r--   0        0        0    32224 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series_collection/test_merge_wide.yaml
--rw-r--r--   0        0        0    17910 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series_collection/test_rename_after_add[dict].yaml
--rw-r--r--   0        0        0    17910 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series_collection/test_rename_after_add[func].yaml
--rw-r--r--   0        0        0    17910 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series_collection/test_rename_err.yaml
--rw-r--r--   0        0        0    17910 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series_collection/test_rename_on_add[dict].yaml
--rw-r--r--   0        0        0    17910 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series_collection/test_rename_on_add[func].yaml
--rw-r--r--   0        0        0    32224 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_series_collection/test_rename_partial.yaml
--rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_sources/test_get_source.yaml
--rw-r--r--   0        0        0    17356 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_sources/test_get_source_release.yaml
--rw-r--r--   0        0        0    18851 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_sources/test_get_sources.yaml
--rw-r--r--   0        0        0    77768 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_tags/test_get_related_tags.yaml
--rw-r--r--   0        0        0     6478 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_tags/test_get_tag_series.yaml
--rw-r--r--   0        0        0    75282 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/tests/vhs/test_tags/test_get_tags.yaml
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/LICENSE
--rw-r--r--   0        0        0     4532 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/README.md
--rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     7141 2020-02-02 00:00:00.000000 pyfredapi-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/.readthedocs.yml
+-rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/RELEASE.md
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/mypy.ini
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/requirements.txt
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/sonar-project.properties
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tox.ini
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/.github/PULL_REQUEST_TEMPLATE/version_release.md
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/.github/workflows/build-pyfredapi.yml
+-rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/.github/workflows/sonarcloud.yml
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/.nojekyll
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/Makefile
+-rw-r--r--   0        0        0     2456 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/conf.py
+-rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/make.bat
+-rw-r--r--   0        0        0     7860 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/requirements.txt
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/_templates/layout.html
+-rw-r--r--   0        0        0     4919 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/CHANGELOG.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/api.rst
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi._base.BaseApiParameters.rst
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi._base._get_api_key.rst
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi._base._get_request.rst
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.category.CategoryApiParameters.rst
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.category.get_category.rst
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.category.get_category_children.rst
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.category.get_category_related.rst
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.category.get_category_related_tags.rst
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.category.get_category_series.rst
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.category.get_category_tags.rst
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.maps.MapApiParameters.rst
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.maps.get_geoseries.rst
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.maps.get_geoseries_info.rst
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.maps.get_shape_files.rst
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.releases.ReleaseApiParameters.rst
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.releases.get_release.rst
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.releases.get_release_dates.rst
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.releases.get_release_related_tags.rst
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.releases.get_release_series.rst
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.releases.get_release_tables.rst
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.releases.get_releases.rst
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.releases.get_releases_dates.rst
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.series.SeriesApiParameters.rst
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.series.SeriesInfo.rst
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.series.SeriesSearchParameters.rst
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.series.get_series.rst
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.series.get_series_all_releases.rst
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.series.get_series_asof_date.rst
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.series.get_series_categories.rst
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.series.get_series_info.rst
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.series.get_series_initial_release.rst
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.series.get_series_releases.rst
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.series.get_series_tags.rst
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.series.get_series_updates.rst
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.series.get_series_vintagedates.rst
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.series.search_series.rst
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.series.search_series_related_tags.rst
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.series.search_series_tags.rst
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.series_collection.SeriesCollection.rst
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.series_collection.SeriesData.rst
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.sources.SourceApiParameters.rst
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.sources.get_source.rst
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.sources.get_source_release.rst
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.sources.get_sources.rst
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.tags.TagsApiParameters.rst
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.tags.get_related_tags.rst
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.tags.get_series_matching_tags.rst
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.tags.get_tags.rst
+-rw-r--r--   0        0        0  7594465 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/tutorials/category.ipynb
+-rw-r--r--   0        0        0    51427 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/tutorials/maps.ipynb
+-rw-r--r--   0        0        0    33447 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/tutorials/series.ipynb
+-rw-r--r--   0        0        0    24658 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/tutorials/series_collection.ipynb
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/pyfredapi/__about__.py
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/pyfredapi/__init__.py
+-rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/pyfredapi/_base.py
+-rw-r--r--   0        0        0     8492 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/pyfredapi/category.py
+-rw-r--r--   0        0        0     5824 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/pyfredapi/maps.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/pyfredapi/py.typed
+-rw-r--r--   0        0        0     9651 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/pyfredapi/releases.py
+-rw-r--r--   0        0        0    21037 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/pyfredapi/series.py
+-rw-r--r--   0        0        0    15460 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/pyfredapi/series_collection.py
+-rw-r--r--   0        0        0     3600 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/pyfredapi/sources.py
+-rw-r--r--   0        0        0     4367 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/pyfredapi/tags.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/pyfredapi/exceptions/__init__.py
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/pyfredapi/exceptions/exceptions.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/pyfredapi/utils/__init__.py
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/pyfredapi/utils/_common_type_hints.py
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/pyfredapi/utils/_convert_to_pandas.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/pyfredapi/utils/enums.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/__init__.py
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/conftest.py
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/test_base.py
+-rw-r--r--   0        0        0     3427 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/test_category.py
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/test_maps.py
+-rw-r--r--   0        0        0     2902 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/test_release.py
+-rw-r--r--   0        0        0     7245 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/test_series.py
+-rw-r--r--   0        0        0     4174 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/test_series_collection.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/test_sources.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/test_tags.py
+-rw-r--r--   0        0        0     4105 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_category/test_get_category.yaml
+-rw-r--r--   0        0        0     3865 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_category/test_get_category_children.yaml
+-rw-r--r--   0        0        0     3861 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_category/test_get_category_related.yaml
+-rw-r--r--   0        0        0     8817 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_category/test_get_category_related_tags[json].yaml
+-rw-r--r--   0        0        0     4421 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_category/test_get_category_related_tags[pandas].yaml
+-rw-r--r--   0        0        0    20720 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_category/test_get_category_series.yaml
+-rw-r--r--   0        0        0     8909 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_category/test_get_category_tags[json].yaml
+-rw-r--r--   0        0        0     4467 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_category/test_get_category_tags[pandas].yaml
+-rw-r--r--   0        0        0    23177 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_maps/test_get_geoseries[json].yaml
+-rw-r--r--   0        0        0    11620 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_maps/test_get_geoseries[pandas].yaml
+-rw-r--r--   0        0        0     4793 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_maps/test_get_geoseries_info.yaml
+-rw-r--r--   0        0        0   128005 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_maps/test_get_shape_files.yaml
+-rw-r--r--   0        0        0     4599 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_release/test_get_release.yaml
+-rw-r--r--   0        0        0    34170 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_release/test_get_release_dates.yaml
+-rw-r--r--   0        0        0     4581 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_release/test_get_release_related_tags.yaml
+-rw-r--r--   0        0        0   122146 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_release/test_get_release_series.yaml
+-rw-r--r--   0        0        0     4567 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_release/test_get_release_sources.yaml
+-rw-r--r--   0        0        0     5060 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_release/test_get_release_tables.yaml
+-rw-r--r--   0        0        0    28278 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_release/test_get_release_tags.yaml
+-rw-r--r--   0        0        0   307432 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_release/test_get_releases.yaml
+-rw-r--r--   0        0        0    69442 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_release/test_get_releases_dates.yaml
+-rw-r--r--   0        0        0    29017 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_series/test_get_series[json].yaml
+-rw-r--r--   0        0        0    14521 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_series/test_get_series[pandas].yaml
+-rw-r--r--   0        0        0   241057 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_series/test_get_series_all_releases[json].yaml
+-rw-r--r--   0        0        0   120541 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_series/test_get_series_all_releases[pandas].yaml
+-rw-r--r--   0        0        0   219867 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_series/test_get_series_asof_date[json].yaml
+-rw-r--r--   0        0        0   109946 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_series/test_get_series_asof_date[pandas].yaml
+-rw-r--r--   0        0        0     4097 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_series/test_get_series_categories.yaml
+-rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_series/test_get_series_info.yaml
+-rw-r--r--   0        0        0    23366 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_series/test_get_series_initial_release[json].yaml
+-rw-r--r--   0        0        0    11839 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_series/test_get_series_initial_release[pandas].yaml
+-rw-r--r--   0        0        0     4757 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_series/test_get_series_releases.yaml
+-rw-r--r--   0        0        0     7269 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_series/test_get_series_tags.yaml
+-rw-r--r--   0        0        0   242266 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_series/test_get_series_updates.yaml
+-rw-r--r--   0        0        0    15816 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_series/test_get_series_vintagedates.yaml
+-rw-r--r--   0        0        0   198782 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_series/test_search_series[json].yaml
+-rw-r--r--   0        0        0    99412 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_series/test_search_series[pandas].yaml
+-rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_series/test_search_series_related_tags[json].yaml
+-rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_series/test_search_series_related_tags[pandas].yaml
+-rw-r--r--   0        0        0    55891 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_series/test_search_series_tags[json].yaml
+-rw-r--r--   0        0        0    27958 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_series/test_search_series_tags[pandas].yaml
+-rw-r--r--   0        0        0    35967 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_series_collection/test_add_series.yaml
+-rw-r--r--   0        0        0    32455 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_series_collection/test_drop_series.yaml
+-rw-r--r--   0        0        0    94151 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_series_collection/test_list_methods_diff.yaml
+-rw-r--r--   0        0        0    46911 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_series_collection/test_remove_series.yaml
+-rw-r--r--   0        0        0    17997 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_series_collection/test_rename_err.yaml
+-rw-r--r--   0        0        0    18283 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_series_collection/test_rename_on_add[dict].yaml
+-rw-r--r--   0        0        0    17997 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_series_collection/test_rename_on_add[func].yaml
+-rw-r--r--   0        0        0    14483 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_series_collection/test_rename_partial.yaml
+-rw-r--r--   0        0        0     4669 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_sources/test_get_source.yaml
+-rw-r--r--   0        0        0    34693 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_sources/test_get_source_release.yaml
+-rw-r--r--   0        0        0    37658 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_sources/test_get_sources.yaml
+-rw-r--r--   0        0        0   156345 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_tags/test_get_related_tags.yaml
+-rw-r--r--   0        0        0    12864 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_tags/test_get_tag_series.yaml
+-rw-r--r--   0        0        0   151305 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_tags/test_get_tags.yaml
+-rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/LICENSE
+-rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/README.md
+-rw-r--r--   0        0        0     3969 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     7105 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/PKG-INFO
```

### Comparing `pyfredapi-0.6.0/.pre-commit-config.yaml` & `pyfredapi-0.7.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.6.0/CONTRIBUTING.md` & `pyfredapi-0.7.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.6.0/RELEASE.md` & `pyfredapi-0.7.0/RELEASE.md`

 * *Files 6% similar despite different names*

```diff
@@ -2,48 +2,57 @@
 
 This document describes the process for preparing new version of the `pyfredapi` package.
 
 ## Pre-release PR Checklist
 
 Preform these tasks before opening a PR for the `main` branch.
 
+- [ ] Bump the version number. `pyfredapi` follow [semantic versioning](https://semver.org/spec/v2.0.0.html), and uses [hatch](https://hatch.pypa.io/latest/) to manage the version number.
+    - Determine if this is a major, minor, or patch release based on the UNRELEASED section in changelog
+    - Use [hatch to bump the package version number](https://hatch.pypa.io/latest/version/#updating)
 - [ ] Update the `CHANGELOG.md` file with the changes for the new release. Follow the [keepachangelog](https://keepachangelog.com/en/1.0.0/) guidelines.
 - [ ] Check that no updates are needed in `CONTRIBUTING.md`
 - [ ] Check that no updates are needed in `README.md`
 - [ ] Update the requirements.txt
     ```bash
     pip-compile -o requirements.txt pyproject.toml  --resolver=backtracking
     ```
-- [ ] Determine if this a major, minor, or patch release and use [hatch to bump the package version number](https://hatch.pypa.io/latest/version/#updating)
+- [ ] Run unit tests and make fresh vcr cassettes
+    ```bash
+    pytest tests/ --vcr-record=all --runslow
+    ```
 - [ ] Make sure the `pyfredapi` package builds locally
     ```bash
     hatch build
     ```
 
 ### Prepare the documentation
 
-When the PR is merged, the Read The Docs build will be triggered and the documentation will be updated. It is important to be sure the documentation is correct before merging into the main branch.
+When a PR is merged into, the Read The Docs build will be triggered and the documentation will be updated. It is important to be sure the documentation is correct before merging into the main branch.
 
 - [ ] Update documentation dependencies for Read The Docs
     ```bash
     pip-compile --extra docs -o docs/requirements.txt pyproject.toml  --resolver=backtracking
     ```
 - [ ] Test that the documentation builds locally
     ```bash
-    make clean -C docs/
-    make html -C docs/
+    make clean html -C docs/
     open docs/_build/html/index.html
     ```
 - [ ] Review the documentation site
 
+## Open a PR
+
 When a PR is opened for the main branch, the GitHub actions pipeline will the test suite and lint the code.
 
 - [ ] Check that the CI/CD pipeline tasks have passed
+- [ ] Give the PR a descriptive title
+- [ ] Add a description of the changes
 
-# Post PR merge tasks
+## Post PR merge tasks
 
 The package is published to PyPi via GitHub actions pipeline. The pipeline is triggered when a new version release is created in GitHub. Use the GitHub UI to create a new release.
 
 - [ ] Title the tag `pyfredapi-v<version>`. The tag is used to trigger the GitHub actions pipeline to publish the package to PyPi.
 - [ ] Title the release `pyfredapi v<version>`
 - [ ] Add the changelog release notes to the release description
 - [ ] Publish the release
```

### Comparing `pyfredapi-0.6.0/requirements.txt` & `pyfredapi-0.7.0/requirements.txt`

 * *Files 18% similar despite different names*

```diff
@@ -14,19 +14,15 @@
     # via requests
 markdown-it-py==2.2.0
     # via rich
 mdurl==0.1.2
     # via markdown-it-py
 numpy==1.24.2
     # via pandas
-packaging==23.1
-    # via plotly
-pandas==2.0.0
-    # via pyfredapi (pyproject.toml)
-plotly==5.14.1
+pandas==1.5.3
     # via pyfredapi (pyproject.toml)
 pydantic==1.10.7
     # via pyfredapi (pyproject.toml)
 pygments==2.15.1
     # via rich
 python-dateutil==2.8.2
     # via pandas
@@ -34,15 +30,11 @@
     # via pandas
 requests==2.28.2
     # via pyfredapi (pyproject.toml)
 rich==13.3.4
     # via pyfredapi (pyproject.toml)
 six==1.16.0
     # via python-dateutil
-tenacity==8.2.2
-    # via plotly
 typing-extensions==4.5.0
     # via pydantic
-tzdata==2023.3
-    # via pandas
 urllib3==1.26.15
     # via requests
```

### Comparing `pyfredapi-0.6.0/tox.ini` & `pyfredapi-0.7.0/tox.ini`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.6.0/.github/ISSUE_TEMPLATE/bug.md` & `pyfredapi-0.7.0/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.6.0/.github/ISSUE_TEMPLATE/feature_request.md` & `pyfredapi-0.7.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.6.0/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md` & `pyfredapi-0.7.0/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.6.0/.github/workflows/build-pyfredapi.yml` & `pyfredapi-0.7.0/.github/workflows/build-pyfredapi.yml`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.6.0/.github/workflows/sonarcloud.yml` & `pyfredapi-0.7.0/.github/workflows/sonarcloud.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 name: SonarCloud
 
 on:
-  push:
-    branches:
-      - main
   pull_request:
     types:
       - opened
       - synchronize
       - reopened
 
 jobs:
```

### Comparing `pyfredapi-0.6.0/.github/workflows/test.yml` & `pyfredapi-0.7.0/.github/workflows/test.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 name: test
 
 on:
+  push:
+    branches:
+      - main
   pull_request:
     types: [opened, synchronize, reopened]
     branches:
       - main
 
 jobs:
   lint:
```

### Comparing `pyfredapi-0.6.0/docs/Makefile` & `pyfredapi-0.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.6.0/docs/conf.py` & `pyfredapi-0.7.0/docs/conf.py`

 * *Files 10% similar despite different names*

```diff
@@ -64,21 +64,14 @@
 }
 html_theme_options = {
     "base_url": "https://pyfredapi.readthedocs.io/en/latest/",
     "repo_url": "https://github.com/gw-moore/pyfredapi/",
     "repo_name": project,
     "repo_type": "github",
     "nav_title": f"{project} v{release}",
-    # "nav_links": [
-    #     {
-    #         "href": "index",
-    #         "title": project,
-    #         "internal": True,
-    #     }
-    # ],
     "color_primary": "indigo",
     "color_accent": "blue",
     "globaltoc_depth": 2,
     "master_doc": True,
     "heroes": {
         "index": "Python library to make retrieving data from FRED easy",
     },
```

### Comparing `pyfredapi-0.6.0/docs/index.rst` & `pyfredapi-0.7.0/docs/index.rst`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 
 :code:`pyfreadpi` can be installed via pip.
 
 .. code-block:: bash
 
    pip install pyfredapi
 
+   # install with plotting dependencies
+   pip install 'pyfredapi[plot]'
+
 FRED API Key
 ------------
 
 Before you can use :code:`pyfredapi` you must have an API key to the FRED API web service. You can `apply for one <https://fred.stlouisfed.org/docs/api/api_key.html>`_ for free on the FRED website.
 
 You can set your API key in two ways:
 
@@ -50,23 +53,24 @@
 .. code-block:: python
 
    import pyfreadpi as pf
 
    # api key set as environment variable
    pf.get_series_info(series_id="GDP")
 
-   # api key passed to initializer
-   pf.get_series_info(series_id="GDP", api_key="my_api_key"")
+   # api key passed to function
+   pf.get_series_info(series_id="GDP", api_key="my_api_key")
 
 .. toctree::
    :caption: Tutorials
    :maxdepth: 1
 
    FRED Series <tutorials/series.ipynb>
    Series Collection <tutorials/series_collection.ipynb>
+   FRED Categories <tutorials/category.ipynb>
    FRED Maps <tutorials/maps.ipynb>
 
 .. toctree::
    :caption: Reference
    :maxdepth: 1
 
    API <references/api>
```

### Comparing `pyfredapi-0.6.0/docs/make.bat` & `pyfredapi-0.7.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.6.0/docs/requirements.txt` & `pyfredapi-0.7.0/docs/requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -205,32 +205,29 @@
 numpy==1.24.2
     # via pandas
 packaging==23.1
     # via
     #   ipykernel
     #   jupyter-server
     #   nbconvert
-    #   plotly
     #   qtconsole
     #   qtpy
     #   sphinx
-pandas==2.0.0
+pandas==1.5.3
     # via pyfredapi (pyproject.toml)
 pandocfilters==1.5.0
     # via nbconvert
 parso==0.8.3
     # via jedi
 pexpect==4.8.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
 platformdirs==3.2.0
     # via jupyter-core
-plotly==5.14.1
-    # via pyfredapi (pyproject.toml)
 pockets==0.9.1
     # via sphinxcontrib-napoleon
 prometheus-client==0.16.0
     # via
     #   jupyter-server
     #   nbclassic
     #   notebook
@@ -347,16 +344,14 @@
     # via pyfredapi (pyproject.toml)
 sphinxcontrib-qthelp==1.0.3
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.5
     # via sphinx
 stack-data==0.6.2
     # via ipython
-tenacity==8.2.2
-    # via plotly
 terminado==0.17.1
     # via
     #   jupyter-server
     #   jupyter-server-terminals
     #   nbclassic
     #   notebook
 text-unidecode==1.3
@@ -388,16 +383,14 @@
     #   nbconvert
     #   nbformat
     #   nbsphinx
     #   notebook
     #   qtconsole
 typing-extensions==4.5.0
     # via pydantic
-tzdata==2023.3
-    # via pandas
 unidecode==1.3.6
     # via python-slugify
 uri-template==1.2.0
     # via jsonschema
 urllib3==1.26.15
     # via requests
 wcwidth==0.2.6
```

### Comparing `pyfredapi-0.6.0/docs/references/CHANGELOG.md` & `pyfredapi-0.7.0/docs/references/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,38 @@
 # Changelog
 
+## UNRELEASED
+
+## Version 0.7.0 - 2023-04-27
+
+### Changed
+
+- Refactor `SeriesCollection`'s internal structure to represent a sequence.
+  - Updated `__init__` to handle adding the initial set of series.
+  - `SeriesCollection` is now iterable, indexable, and sized.
+  - Renamed `add_series()` to `add()`.
+  - Renamed `drop_series()` to `remove()`.
+- Updated the docstring for `api_key` parameter.
+- When data is converted to a pandas dataframe, the `created` attribute will be cast a date-type column.
+- Added `sleep` parameter to `SeriesCollection.add_series`. Defaults to 0.1 seconds.
+- Added upper bound to dependency versions.
+- Made `plotly` an optional dependency.
+
+### Removed
+
+- Unnecessary type ignore comments.
+- .flake8 config file.
+
 ## Version 0.6.0 - 2023-04-22
 
 ### Changed
 
 - Switched to the [Hatch](https://github.com/pypa/hatch) build tool.
 - Bumped copyright year to 2023.
-- Renamed APIKeyNotFoundError exception to APIKeyNotFound.
+- Renamed `APIKeyNotFoundError` exception to `APIKeyNotFound`.
 - Updated the bug report github issue template.
 
 ## Version 0.5.4 - 2022-04-16
 
 ### Changed
 
 - Loosened the dependency package versions to >= latest major version.
@@ -127,15 +149,15 @@
 - Install instructions.
 - pydantic dependency.
 - `FredSeries.get_series_releases` endpoint.
 - Removed `series_id` from `SeriesArgs`.
 
 ## Version 0.1.0 - 2022-09-25
 
-**Note:** This version has been deleted from pypi.
+**Note:** This version has been deleted from Python Package Index.
 
 Initial release of `pyfredapi` package.
 
 ### Added
 
 - `FredApi` class.
 - `FredCategory` class.
```

### Comparing `pyfredapi-0.6.0/docs/references/api.rst` & `pyfredapi-0.7.0/docs/references/api.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,21 @@
 pyfredapi: Public API Reference
 ================================
 
+Base Module
+------------------------------
+.. currentmodule:: pyfredapi._base
+.. autosummary::
+    :toctree: _autosummary
+    :nosignatures:
+
+    _get_api_key
+    _get_request
+    BaseApiParameters
+
 FRED Categories
 ------------------------------
 .. currentmodule:: pyfredapi.category
 .. autosummary::
     :toctree: _autosummary
     :nosignatures:
 
@@ -24,14 +35,30 @@
     :nosignatures:
 
     get_geoseries
     get_geoseries_info
     get_shape_files
     MapApiParameters
 
+FRED Releases
+------------------------------
+.. currentmodule:: pyfredapi.releases
+.. autosummary::
+    :toctree: _autosummary
+    :nosignatures:
+
+    get_releases
+    get_releases_dates
+    get_release
+    get_release_dates
+    get_release_series
+    get_release_related_tags
+    get_release_tables
+    ReleaseApiParameters
+
 FRED Series
 ------------------------------
 .. currentmodule:: pyfredapi.series
 .. autosummary::
     :toctree: _autosummary
     :nosignatures:
 
@@ -48,14 +75,24 @@
     search_series
     search_series_related_tags
     search_series_tags
     SeriesApiParameters
     SeriesInfo
     SeriesSearchParameters
 
+Series Collection
+------------------------------
+.. currentmodule:: pyfredapi.series_collection
+.. autosummary::
+    :toctree: _autosummary
+    :nosignatures:
+
+    SeriesCollection
+    SeriesData
+
 FRED Sources
 ------------------------------
 .. currentmodule:: pyfredapi.sources
 .. autosummary::
     :toctree: _autosummary
     :nosignatures:
 
@@ -71,17 +108,7 @@
     :toctree: _autosummary
     :nosignatures:
 
     get_tags
     get_related_tags
     get_series_matching_tags
     TagsApiParameters
-
-Series Collection
-------------------------------
-.. currentmodule:: pyfredapi.series_collection
-.. autosummary::
-    :toctree: _autosummary
-    :nosignatures:
-
-    SeriesCollection
-    SeriesData
```

### Comparing `pyfredapi-0.6.0/docs/references/_autosummary/pyfredapi.series_collection.SeriesCollection.rst` & `pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.series_collection.SeriesCollection.rst`

 * *Files 10% similar despite different names*

```diff
@@ -10,27 +10,25 @@
 
    
    .. rubric:: Methods
 
    .. autosummary::
    
       ~SeriesCollection.__init__
-      ~SeriesCollection.add_series
-      ~SeriesCollection.drop_series
-      ~SeriesCollection.extract_series
+      ~SeriesCollection.add
       ~SeriesCollection.list_end_date
       ~SeriesCollection.list_frequency
       ~SeriesCollection.list_seasonality
       ~SeriesCollection.list_series
       ~SeriesCollection.list_start_date
       ~SeriesCollection.list_units
       ~SeriesCollection.merge_asof
       ~SeriesCollection.merge_long
       ~SeriesCollection.merge_wide
-      ~SeriesCollection.plot
+      ~SeriesCollection.remove
       ~SeriesCollection.rename_series
```

### Comparing `pyfredapi-0.6.0/docs/tutorials/maps.ipynb` & `pyfredapi-0.7.0/docs/tutorials/maps.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9856024750230479%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(0, 'import pyfredapi as pf\\n'), (2, 'from rich.pretty "*

 * *            "import pprint')], delete: [4, 3, 2, 0]}}, 4: {'outputs': {0: {'data': {'text/html': "*

 * *            '{insert: [(8, \'    <span style="color: #808000; text-decoration-color: '*

 * *            '#808000">max_date</span>=<span style="color: #008000; text-decoration-color: '*

 * *            '#008000">\\\'2022-01-01\\\'</span>\\n\')], delete: [8]}, \'text/plain\': {insert: '*

 * *            '[(8, "    \\x1b[33mmax_date\ […]*

```diff
@@ -7,25 +7,32 @@
             "source": [
                 "# FRED Maps\n",
                 "\n",
                 "This documentation serves as a quick start guide to `FredMaps`. The FRED Maps API enables developers to pull regional data or shape files."
             ]
         },
         {
+            "attachments": {},
+            "cell_type": "markdown",
+            "id": "692df619",
+            "metadata": {},
+            "source": [
+                "## Setup"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": 1,
             "id": "d82ae970",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from pyfredapi import FredMaps\n",
+                "import pyfredapi as pf\n",
                 "from rich import print\n",
-                "from rich.pretty import pprint\n",
-                "\n",
-                "client = FredMaps()"
+                "from rich.pretty import pprint"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "e43484be",
             "metadata": {},
             "source": [
@@ -45,37 +52,37 @@
                             "    <span style=\"color: #808000; text-decoration-color: #808000\">title</span>=<span style=\"color: #008000; text-decoration-color: #008000\">'Per Capita Personal Income'</span>,\n",
                             "    <span style=\"color: #808000; text-decoration-color: #808000\">region_type</span>=<span style=\"color: #008000; text-decoration-color: #008000\">'state'</span>,\n",
                             "    <span style=\"color: #808000; text-decoration-color: #808000\">series_group</span>=<span style=\"color: #008000; text-decoration-color: #008000\">'882'</span>,\n",
                             "    <span style=\"color: #808000; text-decoration-color: #808000\">season</span>=<span style=\"color: #008000; text-decoration-color: #008000\">'NSA'</span>,\n",
                             "    <span style=\"color: #808000; text-decoration-color: #808000\">units</span>=<span style=\"color: #008000; text-decoration-color: #008000\">'Dollars'</span>,\n",
                             "    <span style=\"color: #808000; text-decoration-color: #808000\">frequency</span>=<span style=\"color: #008000; text-decoration-color: #008000\">'Annual'</span>,\n",
                             "    <span style=\"color: #808000; text-decoration-color: #808000\">min_date</span>=<span style=\"color: #008000; text-decoration-color: #008000\">'1929-01-01'</span>,\n",
-                            "    <span style=\"color: #808000; text-decoration-color: #808000\">max_date</span>=<span style=\"color: #008000; text-decoration-color: #008000\">'2021-01-01'</span>\n",
+                            "    <span style=\"color: #808000; text-decoration-color: #808000\">max_date</span>=<span style=\"color: #008000; text-decoration-color: #008000\">'2022-01-01'</span>\n",
                             "<span style=\"font-weight: bold\">)</span>\n",
                             "</pre>\n"
                         ],
                         "text/plain": [
                             "\u001b[1;35mGeoseriesInfo\u001b[0m\u001b[1m(\u001b[0m\n",
                             "    \u001b[33mtitle\u001b[0m=\u001b[32m'Per Capita Personal Income'\u001b[0m,\n",
                             "    \u001b[33mregion_type\u001b[0m=\u001b[32m'state'\u001b[0m,\n",
                             "    \u001b[33mseries_group\u001b[0m=\u001b[32m'882'\u001b[0m,\n",
                             "    \u001b[33mseason\u001b[0m=\u001b[32m'NSA'\u001b[0m,\n",
                             "    \u001b[33munits\u001b[0m=\u001b[32m'Dollars'\u001b[0m,\n",
                             "    \u001b[33mfrequency\u001b[0m=\u001b[32m'Annual'\u001b[0m,\n",
                             "    \u001b[33mmin_date\u001b[0m=\u001b[32m'1929-01-01'\u001b[0m,\n",
-                            "    \u001b[33mmax_date\u001b[0m=\u001b[32m'2021-01-01'\u001b[0m\n",
+                            "    \u001b[33mmax_date\u001b[0m=\u001b[32m'2022-01-01'\u001b[0m\n",
                             "\u001b[1m)\u001b[0m\n"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
-                "info = client.get_geoseries_info(series_id=\"WIPCPI\")\n",
+                "info = pf.get_geoseries_info(series_id=\"WIPCPI\")\n",
                 "print(info)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "adee8bff",
             "metadata": {},
@@ -90,15 +97,15 @@
         {
             "cell_type": "code",
             "execution_count": 3,
             "id": "ba7d2935",
             "metadata": {},
             "outputs": [],
             "source": [
-                "geoseries_data = client.get_geoseries(\n",
+                "geoseries_data = pf.get_geoseries(\n",
                 "    series_id=\"WIPCPI\",\n",
                 "    start_date=\"2010-01-01\",\n",
                 "    end_date=\"2021-01-01\",\n",
                 ")"
             ]
         },
         {
@@ -232,15 +239,15 @@
         {
             "cell_type": "code",
             "execution_count": 6,
             "id": "f36c83c6",
             "metadata": {},
             "outputs": [],
             "source": [
-                "bea_shape_files = client.get_shape_files(shape=\"bea\")"
+                "bea_shape_files = pf.get_shape_files(shape=\"bea\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 7,
             "id": "23f730d1",
             "metadata": {},
@@ -430,15 +437,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.1"
+            "version": "3.11.2"
         },
         "vscode": {
             "interpreter": {
                 "hash": "9f8da5f516a0f7b58441e46157a772613635e3a9b5450eafa77dccb7c363b35a"
             }
         }
     },
```

### Comparing `pyfredapi-0.6.0/docs/tutorials/series.ipynb` & `pyfredapi-0.7.0/docs/tutorials/series_collection.ipynb`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7560090071323445%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '# Series Collection\\n'), (2, 'Often users of the FRED "*

 * *            'API will want analyze multiple economic series. This can be done with `FredSeries` '*

 * *            'alone, but can be tedious and cumbersome. `pyfredapi` offers the `SeriesCollection` '*

 * *            'class to streamline the process of collecting and munging data for plotting and '*

 * *            "analysis.\\n'), (4, 'A `SeriesCollection` object is a set of `SeriesData` objects. "*

 * *            "`SeriesCo […]*

```diff
@@ -1,727 +1,566 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "id": "7cbad414",
             "metadata": {},
             "source": [
-                "# FRED Series\n",
+                "# Series Collection\n",
                 "\n",
-                "This documentation serves as an introduction to requesting series data from the FRED API with `pyfredapi`.\n",
+                "Often users of the FRED API will want analyze multiple economic series. This can be done with `FredSeries` alone, but can be tedious and cumbersome. `pyfredapi` offers the `SeriesCollection` class to streamline the process of collecting and munging data for plotting and analysis.\n",
                 "\n",
-                "The primary use case of the FRED web service is to pull economic series data for analysis or reporting. The `pyfredapi.series` module aims to make it easy to get series metadata and data from [FRED](https://fred.stlouisfed.org/) or [ALFRED](https://alfred.stlouisfed.org/)."
+                "A `SeriesCollection` object is a set of `SeriesData` objects. `SeriesCollection` provide helpful methods to:\n",
+                "\n",
+                "* List the metadata (frequency, seasonality, units, etc.) of the series in the collection\n",
+                "* Merge series dataframes into a long dataframe\n",
+                "* Merge series dataframes into a wide dataframe by index\n",
+                "* Merge series dataframes into a wide dataframe by date"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
-            "id": "0e08721a",
             "metadata": {},
             "source": [
                 "## Setup\n",
                 "\n",
-                "Import and create an instance of `FredSeries`"
+                "Import pyfredapi"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
-            "id": "41acbef2",
             "metadata": {},
             "outputs": [],
             "source": [
                 "import pyfredapi as pf\n",
-                "from rich import print as rprint"
+                "from rich.pretty import pprint"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
-            "id": "736e6209",
             "metadata": {},
             "source": [
-                "## Series info\n",
-                "\n",
-                "Before looking at series data, it is helpful to understand the `pyfredapi`'s `get_series_info` function and `SeriesInfo` object. Each series published by FRED has associated metadata such as\n",
-                "\n",
-                "- the start and end dates\n",
-                "- the publish frequency\n",
-                "- the units\n",
-                "\n",
-                "You can query a series' information directly with `get_series_info`. The `get_series_info` function returns a `SeriesInfo` object that contains all the metadata for the given series.\n",
+                "## Create a SeriesCollection\n",
                 "\n",
-                "In the below example, we request information on the U.S. GDP. From the result, we can see that the GDP series is\n",
+                "Create an instance of `SeriesCollection`,\n",
                 "\n",
-                "* Published quarterly\n",
-                "* The latest data available is 2022-04-01\n",
-                "* Reported in Billions of Dollars\n",
-                "* Seasonally Adjusted Annual Rate"
+                "Add data to the collection with `add_series()`. By default the column for the series values will be renamed to the series id."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
-            "id": "06d9ea55",
             "metadata": {},
             "outputs": [
                 {
-                    "data": {
-                        "text/html": [
-                            "<pre style=\"white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,'DejaVu Sans Mono',consolas,'Courier New',monospace\"><span style=\"color: #800080; text-decoration-color: #800080; font-weight: bold\">SeriesInfo</span><span style=\"font-weight: bold\">(</span>\n",
-                            "    <span style=\"color: #808000; text-decoration-color: #808000\">id</span>=<span style=\"color: #008000; text-decoration-color: #008000\">'GDP'</span>,\n",
-                            "    <span style=\"color: #808000; text-decoration-color: #808000\">realtime_start</span>=<span style=\"color: #008000; text-decoration-color: #008000\">'2022-10-26'</span>,\n",
-                            "    <span style=\"color: #808000; text-decoration-color: #808000\">realtime_end</span>=<span style=\"color: #008000; text-decoration-color: #008000\">'2022-10-26'</span>,\n",
-                            "    <span style=\"color: #808000; text-decoration-color: #808000\">title</span>=<span style=\"color: #008000; text-decoration-color: #008000\">'Gross Domestic Product'</span>,\n",
-                            "    <span style=\"color: #808000; text-decoration-color: #808000\">observation_start</span>=<span style=\"color: #008000; text-decoration-color: #008000\">'1947-01-01'</span>,\n",
-                            "    <span style=\"color: #808000; text-decoration-color: #808000\">observation_end</span>=<span style=\"color: #008000; text-decoration-color: #008000\">'2022-04-01'</span>,\n",
-                            "    <span style=\"color: #808000; text-decoration-color: #808000\">frequency</span>=<span style=\"color: #008000; text-decoration-color: #008000\">'Quarterly'</span>,\n",
-                            "    <span style=\"color: #808000; text-decoration-color: #808000\">frequency_short</span>=<span style=\"color: #008000; text-decoration-color: #008000\">'Q'</span>,\n",
-                            "    <span style=\"color: #808000; text-decoration-color: #808000\">units</span>=<span style=\"color: #008000; text-decoration-color: #008000\">'Billions of Dollars'</span>,\n",
-                            "    <span style=\"color: #808000; text-decoration-color: #808000\">units_short</span>=<span style=\"color: #008000; text-decoration-color: #008000\">'Bil. of $'</span>,\n",
-                            "    <span style=\"color: #808000; text-decoration-color: #808000\">seasonal_adjustment</span>=<span style=\"color: #008000; text-decoration-color: #008000\">'Seasonally Adjusted Annual Rate'</span>,\n",
-                            "    <span style=\"color: #808000; text-decoration-color: #808000\">seasonal_adjustment_short</span>=<span style=\"color: #008000; text-decoration-color: #008000\">'SAAR'</span>,\n",
-                            "    <span style=\"color: #808000; text-decoration-color: #808000\">last_updated</span>=<span style=\"color: #008000; text-decoration-color: #008000\">'2022-09-29 07:46:02-05'</span>,\n",
-                            "    <span style=\"color: #808000; text-decoration-color: #808000\">popularity</span>=<span style=\"color: #008080; text-decoration-color: #008080; font-weight: bold\">93</span>,\n",
-                            "    <span style=\"color: #808000; text-decoration-color: #808000\">notes</span>=<span style=\"color: #008000; text-decoration-color: #008000\">'BEA Account Code: A191RC\\n\\nGross domestic product (GDP), the featured measure of U.S. output, is the </span>\n",
-                            "<span style=\"color: #008000; text-decoration-color: #008000\">market value of the goods and services produced by labor and property located in the United States.For more </span>\n",
-                            "<span style=\"color: #008000; text-decoration-color: #008000\">information, see the Guide to the National Income and Product Accounts of the United States (NIPA) and the Bureau </span>\n",
-                            "<span style=\"color: #008000; text-decoration-color: #008000\">of Economic Analysis (http://www.bea.gov/national/pdf/nipaguid.pdf).'</span>\n",
-                            "<span style=\"font-weight: bold\">)</span>\n",
-                            "</pre>\n"
-                        ],
-                        "text/plain": [
-                            "\u001b[1;35mSeriesInfo\u001b[0m\u001b[1m(\u001b[0m\n",
-                            "    \u001b[33mid\u001b[0m=\u001b[32m'GDP'\u001b[0m,\n",
-                            "    \u001b[33mrealtime_start\u001b[0m=\u001b[32m'2022-10-26'\u001b[0m,\n",
-                            "    \u001b[33mrealtime_end\u001b[0m=\u001b[32m'2022-10-26'\u001b[0m,\n",
-                            "    \u001b[33mtitle\u001b[0m=\u001b[32m'Gross Domestic Product'\u001b[0m,\n",
-                            "    \u001b[33mobservation_start\u001b[0m=\u001b[32m'1947-01-01'\u001b[0m,\n",
-                            "    \u001b[33mobservation_end\u001b[0m=\u001b[32m'2022-04-01'\u001b[0m,\n",
-                            "    \u001b[33mfrequency\u001b[0m=\u001b[32m'Quarterly'\u001b[0m,\n",
-                            "    \u001b[33mfrequency_short\u001b[0m=\u001b[32m'Q'\u001b[0m,\n",
-                            "    \u001b[33munits\u001b[0m=\u001b[32m'Billions of Dollars'\u001b[0m,\n",
-                            "    \u001b[33munits_short\u001b[0m=\u001b[32m'Bil. of $'\u001b[0m,\n",
-                            "    \u001b[33mseasonal_adjustment\u001b[0m=\u001b[32m'Seasonally Adjusted Annual Rate'\u001b[0m,\n",
-                            "    \u001b[33mseasonal_adjustment_short\u001b[0m=\u001b[32m'SAAR'\u001b[0m,\n",
-                            "    \u001b[33mlast_updated\u001b[0m=\u001b[32m'2022-09-29 07:46:02-05'\u001b[0m,\n",
-                            "    \u001b[33mpopularity\u001b[0m=\u001b[1;36m93\u001b[0m,\n",
-                            "    \u001b[33mnotes\u001b[0m=\u001b[32m'BEA Account Code: A191RC\\n\\nGross domestic product \u001b[0m\u001b[32m(\u001b[0m\u001b[32mGDP\u001b[0m\u001b[32m)\u001b[0m\u001b[32m, the featured measure of U.S. output, is the \u001b[0m\n",
-                            "\u001b[32mmarket value of the goods and services produced by labor and property located in the United States.For more \u001b[0m\n",
-                            "\u001b[32minformation, see the Guide to the National Income and Product Accounts of the United States \u001b[0m\u001b[32m(\u001b[0m\u001b[32mNIPA\u001b[0m\u001b[32m)\u001b[0m\u001b[32m and the Bureau \u001b[0m\n",
-                            "\u001b[32mof Economic Analysis \u001b[0m\u001b[32m(\u001b[0m\u001b[32mhttp://www.bea.gov/national/pdf/nipaguid.pdf\u001b[0m\u001b[32m)\u001b[0m\u001b[32m.'\u001b[0m\n",
-                            "\u001b[1m)\u001b[0m\n"
-                        ]
-                    },
-                    "metadata": {},
-                    "output_type": "display_data"
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Requesting series GDP...\n"
+                    ]
                 }
             ],
             "source": [
-                "gdp_info = pf.get_series_info(series_id=\"GDP\")\n",
-                "\n",
-                "# Using rich to pretty print the SeriesInfo\n",
-                "rprint(gdp_info)"
+                "sc = pf.SeriesCollection(series_ids=[\"GDP\"])"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
-            "id": "6809519b",
             "metadata": {},
             "source": [
-                "`SeriesInfo` also provides a useful method to open the FRED webpage for the series. Call `open_url` on the info object and a new browser tab will open."
+                "## Collect additional series\n",
+                "\n",
+                "Add more series to a `SeriesCollection` object with `add()`."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
-            "id": "9b14d963",
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Requesting series SP500...\n"
+                    ]
+                }
+            ],
             "source": [
-                "gdp_info.open_url()"
+                "sc.add(series_ids=[\"SP500\"])"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
-            "id": "6a74c86d",
             "metadata": {},
             "source": [
-                "## Pull data\n",
+                "### Remove series\n",
                 "\n",
-                "The `get_series` function gets the latest data available for a given series and returns either a pandas dataframe of a dictionary."
+                "Remove series from the collection with `remove()`."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
-            "id": "db9e0762",
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "gdp_df = pf.get_series(series_id=\"GDP\")"
+                "sc.remove(\"SP500\")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
-            "id": "5e015cdb",
+            "execution_count": null,
             "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "text/html": [
-                            "<div>\n",
-                            "<style scoped>\n",
-                            "    .dataframe tbody tr th:only-of-type {\n",
-                            "        vertical-align: middle;\n",
-                            "    }\n",
-                            "\n",
-                            "    .dataframe tbody tr th {\n",
-                            "        vertical-align: top;\n",
-                            "    }\n",
-                            "\n",
-                            "    .dataframe thead th {\n",
-                            "        text-align: right;\n",
-                            "    }\n",
-                            "</style>\n",
-                            "<table border=\"1\" class=\"dataframe\">\n",
-                            "  <thead>\n",
-                            "    <tr style=\"text-align: right;\">\n",
-                            "      <th></th>\n",
-                            "      <th>realtime_start</th>\n",
-                            "      <th>realtime_end</th>\n",
-                            "      <th>date</th>\n",
-                            "      <th>value</th>\n",
-                            "    </tr>\n",
-                            "  </thead>\n",
-                            "  <tbody>\n",
-                            "    <tr>\n",
-                            "      <th>301</th>\n",
-                            "      <td>2022-10-26</td>\n",
-                            "      <td>2022-10-26</td>\n",
-                            "      <td>2021-04-01</td>\n",
-                            "      <td>23046.934</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>302</th>\n",
-                            "      <td>2022-10-26</td>\n",
-                            "      <td>2022-10-26</td>\n",
-                            "      <td>2021-07-01</td>\n",
-                            "      <td>23550.420</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>303</th>\n",
-                            "      <td>2022-10-26</td>\n",
-                            "      <td>2022-10-26</td>\n",
-                            "      <td>2021-10-01</td>\n",
-                            "      <td>24349.121</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>304</th>\n",
-                            "      <td>2022-10-26</td>\n",
-                            "      <td>2022-10-26</td>\n",
-                            "      <td>2022-01-01</td>\n",
-                            "      <td>24740.480</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>305</th>\n",
-                            "      <td>2022-10-26</td>\n",
-                            "      <td>2022-10-26</td>\n",
-                            "      <td>2022-04-01</td>\n",
-                            "      <td>25248.476</td>\n",
-                            "    </tr>\n",
-                            "  </tbody>\n",
-                            "</table>\n",
-                            "</div>"
-                        ],
-                        "text/plain": [
-                            "    realtime_start realtime_end       date      value\n",
-                            "301     2022-10-26   2022-10-26 2021-04-01  23046.934\n",
-                            "302     2022-10-26   2022-10-26 2021-07-01  23550.420\n",
-                            "303     2022-10-26   2022-10-26 2021-10-01  24349.121\n",
-                            "304     2022-10-26   2022-10-26 2022-01-01  24740.480\n",
-                            "305     2022-10-26   2022-10-26 2022-04-01  25248.476"
-                        ]
-                    },
-                    "execution_count": 5,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
+            "outputs": [],
             "source": [
-                "gdp_df.tail()"
+                "del sc[\"SP500\"]"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "5a02f5d1",
             "metadata": {},
             "source": [
-                "When the data is returned as a pandas dataframe, the correct data type will be inferred and applied to each column"
+                "## Plot Series\n",
+                "\n",
+                "The `plot` method builds a [plotly](https://plotly.com/python/) time series plot of the data."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
-            "id": "9f292ec7",
+            "execution_count": null,
             "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "text/plain": [
-                            "realtime_start            object\n",
-                            "realtime_end              object\n",
-                            "date              datetime64[ns]\n",
-                            "value                    float64\n",
-                            "dtype: object"
-                        ]
-                    },
-                    "execution_count": 6,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
+            "outputs": [],
             "source": [
-                "gdp_df.dtypes"
+                "fig = sc.GDP.plot()\n",
+                "fig.show(renderer=\"notebook\")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
-            "id": "ae55d33c",
             "metadata": {},
             "source": [
-                "## Data revisions\n",
+                "## Accessing the data\n",
                 "\n",
-                "Many economic series are often revised as more complete information is made available. Every time a new version of a data series is released, FRED displays the latest version, and the replaced version is archived in [ALFRED](https://alfred.stlouisfed.org/). ALFRED stores all the previous versions of data so that it possible to understand, \"what was known when?\".\n",
+                "The `SeriesCollection` is composed of `SeriesData` objects. You can access the `SeriesData` by attribute. Each series_id added to the collection will be an attribute that returns the `SeriesData` object for that series.\n",
                 "\n",
-                "`pyfredapi` provides functions to access data from ALFRED:\n",
+                "`SeriesData` is has two attributes.\n",
                 "\n",
-                "* `get_series_all_releases` - get data for all releases\n",
-                "* `get_series_initial_release` - get data for the initial release\n",
-                "* `get_series_asof_date` - get data released on or before a specific date"
+                "* `info` - The series metadata.\n",
+                "* `df` - Series observations in a pandas dataframe."
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "52fc3f6c",
             "metadata": {},
             "source": [
-                "### Get all releases\n",
-                "\n",
-                "`get_series_all_releases` returns all the observations for each release of an economic series. In the example below, a request is made for all the releases of Gross Domestic Product. We can see that the GDP estimates for Q2 2022 has been revised 3 times. The first release was on 2022-07-28. Since then, two revisions have been released on 2022-08-25 and 2022-09-29.\n",
-                "\n",
-                "The realtime columns indicates the time period that the data was known to be true. For more information, see the [FRED docs](https://fred.stlouisfed.org/docs/api/fred/realtime_period.html) on realtime periods."
+                "### Access via attribute"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
-            "id": "5c1e9ca9",
+            "execution_count": 8,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "text/html": [
-                            "<div>\n",
-                            "<style scoped>\n",
-                            "    .dataframe tbody tr th:only-of-type {\n",
-                            "        vertical-align: middle;\n",
-                            "    }\n",
-                            "\n",
-                            "    .dataframe tbody tr th {\n",
-                            "        vertical-align: top;\n",
-                            "    }\n",
-                            "\n",
-                            "    .dataframe thead th {\n",
-                            "        text-align: right;\n",
-                            "    }\n",
-                            "</style>\n",
-                            "<table border=\"1\" class=\"dataframe\">\n",
-                            "  <thead>\n",
-                            "    <tr style=\"text-align: right;\">\n",
-                            "      <th></th>\n",
-                            "      <th>realtime_start</th>\n",
-                            "      <th>realtime_end</th>\n",
-                            "      <th>date</th>\n",
-                            "      <th>value</th>\n",
-                            "    </tr>\n",
-                            "  </thead>\n",
-                            "  <tbody>\n",
-                            "    <tr>\n",
-                            "      <th>3093</th>\n",
-                            "      <td>2022-06-29</td>\n",
-                            "      <td>2022-09-28</td>\n",
-                            "      <td>2022-01-01</td>\n",
-                            "      <td>24386.734</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>3094</th>\n",
-                            "      <td>2022-09-29</td>\n",
-                            "      <td>9999-12-31</td>\n",
-                            "      <td>2022-01-01</td>\n",
-                            "      <td>24740.480</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>3095</th>\n",
-                            "      <td>2022-07-28</td>\n",
-                            "      <td>2022-08-24</td>\n",
-                            "      <td>2022-04-01</td>\n",
-                            "      <td>24851.809</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>3096</th>\n",
-                            "      <td>2022-08-25</td>\n",
-                            "      <td>2022-09-28</td>\n",
-                            "      <td>2022-04-01</td>\n",
-                            "      <td>24882.878</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>3097</th>\n",
-                            "      <td>2022-09-29</td>\n",
-                            "      <td>9999-12-31</td>\n",
-                            "      <td>2022-04-01</td>\n",
-                            "      <td>25248.476</td>\n",
-                            "    </tr>\n",
-                            "  </tbody>\n",
-                            "</table>\n",
-                            "</div>"
-                        ],
                         "text/plain": [
-                            "     realtime_start realtime_end       date      value\n",
-                            "3093     2022-06-29   2022-09-28 2022-01-01  24386.734\n",
-                            "3094     2022-09-29   9999-12-31 2022-01-01  24740.480\n",
-                            "3095     2022-07-28   2022-08-24 2022-04-01  24851.809\n",
-                            "3096     2022-08-25   2022-09-28 2022-04-01  24882.878\n",
-                            "3097     2022-09-29   9999-12-31 2022-04-01  25248.476"
+                            "True"
                         ]
                     },
-                    "execution_count": 7,
+                    "execution_count": 8,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "gdp_all_releases_df = pf.get_series_all_releases(\"GDP\")\n",
-                "gdp_all_releases_df.tail()"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "a471bce2",
-            "metadata": {},
-            "source": [
-                "### Get initial release\n",
-                "\n",
-                "`get_series_initial_release` return only the first release of the series. Below we see that only first estimate of Q2 2022 GDP released on 2022-07-28 is included in the dataframe."
+                "sc.GDP == sc[\"GDP\"]"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
-            "id": "72a6b101",
+            "execution_count": 6,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div>\n",
-                            "<style scoped>\n",
-                            "    .dataframe tbody tr th:only-of-type {\n",
-                            "        vertical-align: middle;\n",
-                            "    }\n",
-                            "\n",
-                            "    .dataframe tbody tr th {\n",
-                            "        vertical-align: top;\n",
-                            "    }\n",
-                            "\n",
-                            "    .dataframe thead th {\n",
-                            "        text-align: right;\n",
-                            "    }\n",
-                            "</style>\n",
-                            "<table border=\"1\" class=\"dataframe\">\n",
-                            "  <thead>\n",
-                            "    <tr style=\"text-align: right;\">\n",
-                            "      <th></th>\n",
-                            "      <th>realtime_start</th>\n",
-                            "      <th>realtime_end</th>\n",
-                            "      <th>date</th>\n",
-                            "      <th>value</th>\n",
-                            "    </tr>\n",
-                            "  </thead>\n",
-                            "  <tbody>\n",
-                            "    <tr>\n",
-                            "      <th>118</th>\n",
-                            "      <td>2021-07-29</td>\n",
-                            "      <td>2021-08-25</td>\n",
-                            "      <td>2021-04-01</td>\n",
-                            "      <td>22722.581</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>119</th>\n",
-                            "      <td>2021-10-28</td>\n",
-                            "      <td>2021-11-23</td>\n",
-                            "      <td>2021-07-01</td>\n",
-                            "      <td>23173.496</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>120</th>\n",
-                            "      <td>2022-01-27</td>\n",
-                            "      <td>2022-02-23</td>\n",
-                            "      <td>2021-10-01</td>\n",
-                            "      <td>23992.355</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>121</th>\n",
-                            "      <td>2022-04-28</td>\n",
-                            "      <td>2022-05-25</td>\n",
-                            "      <td>2022-01-01</td>\n",
-                            "      <td>24382.683</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>122</th>\n",
-                            "      <td>2022-07-28</td>\n",
-                            "      <td>2022-08-24</td>\n",
-                            "      <td>2022-04-01</td>\n",
-                            "      <td>24851.809</td>\n",
-                            "    </tr>\n",
-                            "  </tbody>\n",
-                            "</table>\n",
-                            "</div>"
+                            "<pre style=\"white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,'DejaVu Sans Mono',consolas,'Courier New',monospace\"><span style=\"color: #800080; text-decoration-color: #800080; font-weight: bold\">SeriesInfo</span><span style=\"font-weight: bold\">(</span>\n",
+                            "<span style=\"color: #7fbf7f; text-decoration-color: #7fbf7f\">\u2502   </span><span style=\"color: #808000; text-decoration-color: #808000\">id</span>=<span style=\"color: #008000; text-decoration-color: #008000\">'GDP'</span>,\n",
+                            "<span style=\"color: #7fbf7f; text-decoration-color: #7fbf7f\">\u2502   </span><span style=\"color: #808000; text-decoration-color: #808000\">realtime_start</span>=<span style=\"color: #008000; text-decoration-color: #008000\">'2023-04-27'</span>,\n",
+                            "<span style=\"color: #7fbf7f; text-decoration-color: #7fbf7f\">\u2502   </span><span style=\"color: #808000; text-decoration-color: #808000\">realtime_end</span>=<span style=\"color: #008000; text-decoration-color: #008000\">'2023-04-27'</span>,\n",
+                            "<span style=\"color: #7fbf7f; text-decoration-color: #7fbf7f\">\u2502   </span><span style=\"color: #808000; text-decoration-color: #808000\">title</span>=<span style=\"color: #008000; text-decoration-color: #008000\">'Gross Domestic Product'</span>,\n",
+                            "<span style=\"color: #7fbf7f; text-decoration-color: #7fbf7f\">\u2502   </span><span style=\"color: #808000; text-decoration-color: #808000\">observation_start</span>=<span style=\"color: #008000; text-decoration-color: #008000\">'1947-01-01'</span>,\n",
+                            "<span style=\"color: #7fbf7f; text-decoration-color: #7fbf7f\">\u2502   </span><span style=\"color: #808000; text-decoration-color: #808000\">observation_end</span>=<span style=\"color: #008000; text-decoration-color: #008000\">'2023-01-01'</span>,\n",
+                            "<span style=\"color: #7fbf7f; text-decoration-color: #7fbf7f\">\u2502   </span><span style=\"color: #808000; text-decoration-color: #808000\">frequency</span>=<span style=\"color: #008000; text-decoration-color: #008000\">'Quarterly'</span>,\n",
+                            "<span style=\"color: #7fbf7f; text-decoration-color: #7fbf7f\">\u2502   </span><span style=\"color: #808000; text-decoration-color: #808000\">frequency_short</span>=<span style=\"color: #008000; text-decoration-color: #008000\">'Q'</span>,\n",
+                            "<span style=\"color: #7fbf7f; text-decoration-color: #7fbf7f\">\u2502   </span><span style=\"color: #808000; text-decoration-color: #808000\">units</span>=<span style=\"color: #008000; text-decoration-color: #008000\">'Billions of Dollars'</span>,\n",
+                            "<span style=\"color: #7fbf7f; text-decoration-color: #7fbf7f\">\u2502   </span><span style=\"color: #808000; text-decoration-color: #808000\">units_short</span>=<span style=\"color: #008000; text-decoration-color: #008000\">'Bil. of $'</span>,\n",
+                            "<span style=\"color: #7fbf7f; text-decoration-color: #7fbf7f\">\u2502   </span><span style=\"color: #808000; text-decoration-color: #808000\">seasonal_adjustment</span>=<span style=\"color: #008000; text-decoration-color: #008000\">'Seasonally Adjusted Annual Rate'</span>,\n",
+                            "<span style=\"color: #7fbf7f; text-decoration-color: #7fbf7f\">\u2502   </span><span style=\"color: #808000; text-decoration-color: #808000\">seasonal_adjustment_short</span>=<span style=\"color: #008000; text-decoration-color: #008000\">'SAAR'</span>,\n",
+                            "<span style=\"color: #7fbf7f; text-decoration-color: #7fbf7f\">\u2502   </span><span style=\"color: #808000; text-decoration-color: #808000\">last_updated</span>=<span style=\"color: #008000; text-decoration-color: #008000\">'2023-04-27 07:53:02-05'</span>,\n",
+                            "<span style=\"color: #7fbf7f; text-decoration-color: #7fbf7f\">\u2502   </span><span style=\"color: #808000; text-decoration-color: #808000\">popularity</span>=<span style=\"color: #008080; text-decoration-color: #008080; font-weight: bold\">93</span>,\n",
+                            "<span style=\"color: #7fbf7f; text-decoration-color: #7fbf7f\">\u2502   </span><span style=\"color: #808000; text-decoration-color: #808000\">notes</span>=<span style=\"color: #008000; text-decoration-color: #008000\">'BEA Account Code: A191RC\\n\\nGross domestic product (GDP), the featured measure of U.S. output, is the market value of the goods and services produced by labor and property located in the United States.For more information, see the Guide to the National Income and Product Accounts of the United States (NIPA) and the Bureau of Economic Analysis (http://www.bea.gov/national/pdf/nipaguid.pdf).'</span>\n",
+                            "<span style=\"font-weight: bold\">)</span>\n",
+                            "</pre>\n"
                         ],
                         "text/plain": [
-                            "    realtime_start realtime_end       date      value\n",
-                            "118     2021-07-29   2021-08-25 2021-04-01  22722.581\n",
-                            "119     2021-10-28   2021-11-23 2021-07-01  23173.496\n",
-                            "120     2022-01-27   2022-02-23 2021-10-01  23992.355\n",
-                            "121     2022-04-28   2022-05-25 2022-01-01  24382.683\n",
-                            "122     2022-07-28   2022-08-24 2022-04-01  24851.809"
+                            "\u001b[1;35mSeriesInfo\u001b[0m\u001b[1m(\u001b[0m\n",
+                            "\u001b[2;32m\u2502   \u001b[0m\u001b[33mid\u001b[0m=\u001b[32m'GDP'\u001b[0m,\n",
+                            "\u001b[2;32m\u2502   \u001b[0m\u001b[33mrealtime_start\u001b[0m=\u001b[32m'2023-04-27'\u001b[0m,\n",
+                            "\u001b[2;32m\u2502   \u001b[0m\u001b[33mrealtime_end\u001b[0m=\u001b[32m'2023-04-27'\u001b[0m,\n",
+                            "\u001b[2;32m\u2502   \u001b[0m\u001b[33mtitle\u001b[0m=\u001b[32m'Gross Domestic Product'\u001b[0m,\n",
+                            "\u001b[2;32m\u2502   \u001b[0m\u001b[33mobservation_start\u001b[0m=\u001b[32m'1947-01-01'\u001b[0m,\n",
+                            "\u001b[2;32m\u2502   \u001b[0m\u001b[33mobservation_end\u001b[0m=\u001b[32m'2023-01-01'\u001b[0m,\n",
+                            "\u001b[2;32m\u2502   \u001b[0m\u001b[33mfrequency\u001b[0m=\u001b[32m'Quarterly'\u001b[0m,\n",
+                            "\u001b[2;32m\u2502   \u001b[0m\u001b[33mfrequency_short\u001b[0m=\u001b[32m'Q'\u001b[0m,\n",
+                            "\u001b[2;32m\u2502   \u001b[0m\u001b[33munits\u001b[0m=\u001b[32m'Billions of Dollars'\u001b[0m,\n",
+                            "\u001b[2;32m\u2502   \u001b[0m\u001b[33munits_short\u001b[0m=\u001b[32m'Bil. of $'\u001b[0m,\n",
+                            "\u001b[2;32m\u2502   \u001b[0m\u001b[33mseasonal_adjustment\u001b[0m=\u001b[32m'Seasonally Adjusted Annual Rate'\u001b[0m,\n",
+                            "\u001b[2;32m\u2502   \u001b[0m\u001b[33mseasonal_adjustment_short\u001b[0m=\u001b[32m'SAAR'\u001b[0m,\n",
+                            "\u001b[2;32m\u2502   \u001b[0m\u001b[33mlast_updated\u001b[0m=\u001b[32m'2023-04-27 07:53:02-05'\u001b[0m,\n",
+                            "\u001b[2;32m\u2502   \u001b[0m\u001b[33mpopularity\u001b[0m=\u001b[1;36m93\u001b[0m,\n",
+                            "\u001b[2;32m\u2502   \u001b[0m\u001b[33mnotes\u001b[0m=\u001b[32m'BEA Account Code: A191RC\\n\\nGross domestic product \u001b[0m\u001b[32m(\u001b[0m\u001b[32mGDP\u001b[0m\u001b[32m)\u001b[0m\u001b[32m, the featured measure of U.S. output, is the market value of the goods and services produced by labor and property located in the United States.For more information, see the Guide to the National Income and Product Accounts of the United States \u001b[0m\u001b[32m(\u001b[0m\u001b[32mNIPA\u001b[0m\u001b[32m)\u001b[0m\u001b[32m and the Bureau of Economic Analysis \u001b[0m\u001b[32m(\u001b[0m\u001b[32mhttp://www.bea.gov/national/pdf/nipaguid.pdf\u001b[0m\u001b[32m)\u001b[0m\u001b[32m.'\u001b[0m\n",
+                            "\u001b[1m)\u001b[0m\n"
                         ]
                     },
-                    "execution_count": 8,
                     "metadata": {},
-                    "output_type": "execute_result"
+                    "output_type": "display_data"
                 }
             ],
             "source": [
-                "gdp_initial_release_df = pf.get_series_initial_release(\"GDP\")\n",
-                "gdp_initial_release_df.tail()"
+                "pprint(sc.GDP.info)"
             ]
         },
         {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "sc.GDP.df.tail()"
+            ]
+        },
+        {
+            "attachments": {},
             "cell_type": "markdown",
-            "id": "4912f5a0",
             "metadata": {},
             "source": [
-                "### Get releases as-of date\n",
-                "\n",
-                "`get_series_asof_date` returns all releases of a series made on or before a given date. This is helpful if you want limit your analysis window to only the data know on or before a given date.\n",
-                "\n",
-                "For example, suppose we want the GDP estimates available on or before 2022-09-01. We can use `get_series_asof_date` with the date `2022-09-01`. The response includes the Q2 2022 estimates for 2022-07-28 and 2022-08-25, but not 2022-09-29 since that is after 2022-09-01."
+                "## Access via bracket notation"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
-            "id": "2d9d8131",
+            "execution_count": 7,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div>\n",
-                            "<style scoped>\n",
-                            "    .dataframe tbody tr th:only-of-type {\n",
-                            "        vertical-align: middle;\n",
-                            "    }\n",
-                            "\n",
-                            "    .dataframe tbody tr th {\n",
-                            "        vertical-align: top;\n",
-                            "    }\n",
-                            "\n",
-                            "    .dataframe thead th {\n",
-                            "        text-align: right;\n",
-                            "    }\n",
-                            "</style>\n",
-                            "<table border=\"1\" class=\"dataframe\">\n",
-                            "  <thead>\n",
-                            "    <tr style=\"text-align: right;\">\n",
-                            "      <th></th>\n",
-                            "      <th>realtime_start</th>\n",
-                            "      <th>realtime_end</th>\n",
-                            "      <th>date</th>\n",
-                            "      <th>value</th>\n",
-                            "    </tr>\n",
-                            "  </thead>\n",
-                            "  <tbody>\n",
-                            "    <tr>\n",
-                            "      <th>3071</th>\n",
-                            "      <td>2022-04-28</td>\n",
-                            "      <td>2022-05-25</td>\n",
-                            "      <td>2022-01-01</td>\n",
-                            "      <td>24382.683</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>3072</th>\n",
-                            "      <td>2022-05-26</td>\n",
-                            "      <td>2022-06-28</td>\n",
-                            "      <td>2022-01-01</td>\n",
-                            "      <td>24384.289</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>3073</th>\n",
-                            "      <td>2022-06-29</td>\n",
-                            "      <td>2022-09-01</td>\n",
-                            "      <td>2022-01-01</td>\n",
-                            "      <td>24386.734</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>3074</th>\n",
-                            "      <td>2022-07-28</td>\n",
-                            "      <td>2022-08-24</td>\n",
-                            "      <td>2022-04-01</td>\n",
-                            "      <td>24851.809</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>3075</th>\n",
-                            "      <td>2022-08-25</td>\n",
-                            "      <td>2022-09-01</td>\n",
-                            "      <td>2022-04-01</td>\n",
-                            "      <td>24882.878</td>\n",
-                            "    </tr>\n",
-                            "  </tbody>\n",
-                            "</table>\n",
-                            "</div>"
+                            "<pre style=\"white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,'DejaVu Sans Mono',consolas,'Courier New',monospace\"><span style=\"color: #800080; text-decoration-color: #800080; font-weight: bold\">SeriesInfo</span><span style=\"font-weight: bold\">(</span>\n",
+                            "<span style=\"color: #7fbf7f; text-decoration-color: #7fbf7f\">\u2502   </span><span style=\"color: #808000; text-decoration-color: #808000\">id</span>=<span style=\"color: #008000; text-decoration-color: #008000\">'GDP'</span>,\n",
+                            "<span style=\"color: #7fbf7f; text-decoration-color: #7fbf7f\">\u2502   </span><span style=\"color: #808000; text-decoration-color: #808000\">realtime_start</span>=<span style=\"color: #008000; text-decoration-color: #008000\">'2023-04-27'</span>,\n",
+                            "<span style=\"color: #7fbf7f; text-decoration-color: #7fbf7f\">\u2502   </span><span style=\"color: #808000; text-decoration-color: #808000\">realtime_end</span>=<span style=\"color: #008000; text-decoration-color: #008000\">'2023-04-27'</span>,\n",
+                            "<span style=\"color: #7fbf7f; text-decoration-color: #7fbf7f\">\u2502   </span><span style=\"color: #808000; text-decoration-color: #808000\">title</span>=<span style=\"color: #008000; text-decoration-color: #008000\">'Gross Domestic Product'</span>,\n",
+                            "<span style=\"color: #7fbf7f; text-decoration-color: #7fbf7f\">\u2502   </span><span style=\"color: #808000; text-decoration-color: #808000\">observation_start</span>=<span style=\"color: #008000; text-decoration-color: #008000\">'1947-01-01'</span>,\n",
+                            "<span style=\"color: #7fbf7f; text-decoration-color: #7fbf7f\">\u2502   </span><span style=\"color: #808000; text-decoration-color: #808000\">observation_end</span>=<span style=\"color: #008000; text-decoration-color: #008000\">'2023-01-01'</span>,\n",
+                            "<span style=\"color: #7fbf7f; text-decoration-color: #7fbf7f\">\u2502   </span><span style=\"color: #808000; text-decoration-color: #808000\">frequency</span>=<span style=\"color: #008000; text-decoration-color: #008000\">'Quarterly'</span>,\n",
+                            "<span style=\"color: #7fbf7f; text-decoration-color: #7fbf7f\">\u2502   </span><span style=\"color: #808000; text-decoration-color: #808000\">frequency_short</span>=<span style=\"color: #008000; text-decoration-color: #008000\">'Q'</span>,\n",
+                            "<span style=\"color: #7fbf7f; text-decoration-color: #7fbf7f\">\u2502   </span><span style=\"color: #808000; text-decoration-color: #808000\">units</span>=<span style=\"color: #008000; text-decoration-color: #008000\">'Billions of Dollars'</span>,\n",
+                            "<span style=\"color: #7fbf7f; text-decoration-color: #7fbf7f\">\u2502   </span><span style=\"color: #808000; text-decoration-color: #808000\">units_short</span>=<span style=\"color: #008000; text-decoration-color: #008000\">'Bil. of $'</span>,\n",
+                            "<span style=\"color: #7fbf7f; text-decoration-color: #7fbf7f\">\u2502   </span><span style=\"color: #808000; text-decoration-color: #808000\">seasonal_adjustment</span>=<span style=\"color: #008000; text-decoration-color: #008000\">'Seasonally Adjusted Annual Rate'</span>,\n",
+                            "<span style=\"color: #7fbf7f; text-decoration-color: #7fbf7f\">\u2502   </span><span style=\"color: #808000; text-decoration-color: #808000\">seasonal_adjustment_short</span>=<span style=\"color: #008000; text-decoration-color: #008000\">'SAAR'</span>,\n",
+                            "<span style=\"color: #7fbf7f; text-decoration-color: #7fbf7f\">\u2502   </span><span style=\"color: #808000; text-decoration-color: #808000\">last_updated</span>=<span style=\"color: #008000; text-decoration-color: #008000\">'2023-04-27 07:53:02-05'</span>,\n",
+                            "<span style=\"color: #7fbf7f; text-decoration-color: #7fbf7f\">\u2502   </span><span style=\"color: #808000; text-decoration-color: #808000\">popularity</span>=<span style=\"color: #008080; text-decoration-color: #008080; font-weight: bold\">93</span>,\n",
+                            "<span style=\"color: #7fbf7f; text-decoration-color: #7fbf7f\">\u2502   </span><span style=\"color: #808000; text-decoration-color: #808000\">notes</span>=<span style=\"color: #008000; text-decoration-color: #008000\">'BEA Account Code: A191RC\\n\\nGross domestic product (GDP), the featured measure of U.S. output, is the market value of the goods and services produced by labor and property located in the United States.For more information, see the Guide to the National Income and Product Accounts of the United States (NIPA) and the Bureau of Economic Analysis (http://www.bea.gov/national/pdf/nipaguid.pdf).'</span>\n",
+                            "<span style=\"font-weight: bold\">)</span>\n",
+                            "</pre>\n"
                         ],
                         "text/plain": [
-                            "     realtime_start realtime_end       date      value\n",
-                            "3071     2022-04-28   2022-05-25 2022-01-01  24382.683\n",
-                            "3072     2022-05-26   2022-06-28 2022-01-01  24384.289\n",
-                            "3073     2022-06-29   2022-09-01 2022-01-01  24386.734\n",
-                            "3074     2022-07-28   2022-08-24 2022-04-01  24851.809\n",
-                            "3075     2022-08-25   2022-09-01 2022-04-01  24882.878"
+                            "\u001b[1;35mSeriesInfo\u001b[0m\u001b[1m(\u001b[0m\n",
+                            "\u001b[2;32m\u2502   \u001b[0m\u001b[33mid\u001b[0m=\u001b[32m'GDP'\u001b[0m,\n",
+                            "\u001b[2;32m\u2502   \u001b[0m\u001b[33mrealtime_start\u001b[0m=\u001b[32m'2023-04-27'\u001b[0m,\n",
+                            "\u001b[2;32m\u2502   \u001b[0m\u001b[33mrealtime_end\u001b[0m=\u001b[32m'2023-04-27'\u001b[0m,\n",
+                            "\u001b[2;32m\u2502   \u001b[0m\u001b[33mtitle\u001b[0m=\u001b[32m'Gross Domestic Product'\u001b[0m,\n",
+                            "\u001b[2;32m\u2502   \u001b[0m\u001b[33mobservation_start\u001b[0m=\u001b[32m'1947-01-01'\u001b[0m,\n",
+                            "\u001b[2;32m\u2502   \u001b[0m\u001b[33mobservation_end\u001b[0m=\u001b[32m'2023-01-01'\u001b[0m,\n",
+                            "\u001b[2;32m\u2502   \u001b[0m\u001b[33mfrequency\u001b[0m=\u001b[32m'Quarterly'\u001b[0m,\n",
+                            "\u001b[2;32m\u2502   \u001b[0m\u001b[33mfrequency_short\u001b[0m=\u001b[32m'Q'\u001b[0m,\n",
+                            "\u001b[2;32m\u2502   \u001b[0m\u001b[33munits\u001b[0m=\u001b[32m'Billions of Dollars'\u001b[0m,\n",
+                            "\u001b[2;32m\u2502   \u001b[0m\u001b[33munits_short\u001b[0m=\u001b[32m'Bil. of $'\u001b[0m,\n",
+                            "\u001b[2;32m\u2502   \u001b[0m\u001b[33mseasonal_adjustment\u001b[0m=\u001b[32m'Seasonally Adjusted Annual Rate'\u001b[0m,\n",
+                            "\u001b[2;32m\u2502   \u001b[0m\u001b[33mseasonal_adjustment_short\u001b[0m=\u001b[32m'SAAR'\u001b[0m,\n",
+                            "\u001b[2;32m\u2502   \u001b[0m\u001b[33mlast_updated\u001b[0m=\u001b[32m'2023-04-27 07:53:02-05'\u001b[0m,\n",
+                            "\u001b[2;32m\u2502   \u001b[0m\u001b[33mpopularity\u001b[0m=\u001b[1;36m93\u001b[0m,\n",
+                            "\u001b[2;32m\u2502   \u001b[0m\u001b[33mnotes\u001b[0m=\u001b[32m'BEA Account Code: A191RC\\n\\nGross domestic product \u001b[0m\u001b[32m(\u001b[0m\u001b[32mGDP\u001b[0m\u001b[32m)\u001b[0m\u001b[32m, the featured measure of U.S. output, is the market value of the goods and services produced by labor and property located in the United States.For more information, see the Guide to the National Income and Product Accounts of the United States \u001b[0m\u001b[32m(\u001b[0m\u001b[32mNIPA\u001b[0m\u001b[32m)\u001b[0m\u001b[32m and the Bureau of Economic Analysis \u001b[0m\u001b[32m(\u001b[0m\u001b[32mhttp://www.bea.gov/national/pdf/nipaguid.pdf\u001b[0m\u001b[32m)\u001b[0m\u001b[32m.'\u001b[0m\n",
+                            "\u001b[1m)\u001b[0m\n"
                         ]
                     },
-                    "execution_count": 9,
                     "metadata": {},
-                    "output_type": "execute_result"
+                    "output_type": "display_data"
                 }
             ],
             "source": [
-                "gdp_090122_df = pf.get_series_asof_date(\"GDP\", date=\"2022-09-01\")\n",
-                "gdp_090122_df.tail()"
+                "pprint(sc[\"GDP\"].info)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "72dcdc06",
             "metadata": {},
             "source": [
-                "## Additional Parameters\n",
+                "## Rename series in the collection"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "### Rename on add\n",
                 "\n",
-                "You can pass additional arguments to the FRED API via `**kwargs`. The FRED API endpoint supports many parameters to customize your query. See the [FRED API docs](https://fred.stlouisfed.org/docs/api/fred/) for details."
+                "You can rename the series when adding them to the collection. Renaming can be done with a dictionary mapping the series id to the new name, or with a function which parses the series title into the new name."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
-            "id": "24dc9d3e",
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "extra_parameters = {\n",
-                "    \"observation_start\": \"2020-01-01\",\n",
-                "    \"observation_end\": \"2020-12-31\",\n",
+                "# Rename with a dictionary\n",
+                "new_names = {\n",
+                "    \"CPIAUCSL\": \"cpi_all_items\",\n",
+                "    \"CPILFESL\": \"cpi_all_items_less_food_and_energy\",\n",
                 "}\n",
                 "\n",
-                "gdp_df = pf.get_series(series_id=\"GDP\", **extra_parameters)"
+                "cpi_sc = pf.SeriesCollection(series_ids=[\"CPIAUCSL\", \"CPILFESL\"], rename=new_names)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
-            "id": "a6232cb6",
+            "execution_count": null,
             "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "text/html": [
-                            "<div>\n",
-                            "<style scoped>\n",
-                            "    .dataframe tbody tr th:only-of-type {\n",
-                            "        vertical-align: middle;\n",
-                            "    }\n",
-                            "\n",
-                            "    .dataframe tbody tr th {\n",
-                            "        vertical-align: top;\n",
-                            "    }\n",
-                            "\n",
-                            "    .dataframe thead th {\n",
-                            "        text-align: right;\n",
-                            "    }\n",
-                            "</style>\n",
-                            "<table border=\"1\" class=\"dataframe\">\n",
-                            "  <thead>\n",
-                            "    <tr style=\"text-align: right;\">\n",
-                            "      <th></th>\n",
-                            "      <th>realtime_start</th>\n",
-                            "      <th>realtime_end</th>\n",
-                            "      <th>date</th>\n",
-                            "      <th>value</th>\n",
-                            "    </tr>\n",
-                            "  </thead>\n",
-                            "  <tbody>\n",
-                            "    <tr>\n",
-                            "      <th>0</th>\n",
-                            "      <td>2022-10-26</td>\n",
-                            "      <td>2022-10-26</td>\n",
-                            "      <td>2020-01-01</td>\n",
-                            "      <td>21538.032</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>1</th>\n",
-                            "      <td>2022-10-26</td>\n",
-                            "      <td>2022-10-26</td>\n",
-                            "      <td>2020-04-01</td>\n",
-                            "      <td>19636.731</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>2</th>\n",
-                            "      <td>2022-10-26</td>\n",
-                            "      <td>2022-10-26</td>\n",
-                            "      <td>2020-07-01</td>\n",
-                            "      <td>21362.428</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>3</th>\n",
-                            "      <td>2022-10-26</td>\n",
-                            "      <td>2022-10-26</td>\n",
-                            "      <td>2020-10-01</td>\n",
-                            "      <td>21704.706</td>\n",
-                            "    </tr>\n",
-                            "  </tbody>\n",
-                            "</table>\n",
-                            "</div>"
-                        ],
-                        "text/plain": [
-                            "  realtime_start realtime_end       date      value\n",
-                            "0     2022-10-26   2022-10-26 2020-01-01  21538.032\n",
-                            "1     2022-10-26   2022-10-26 2020-04-01  19636.731\n",
-                            "2     2022-10-26   2022-10-26 2020-07-01  21362.428\n",
-                            "3     2022-10-26   2022-10-26 2020-10-01  21704.706"
-                        ]
-                    },
-                    "execution_count": 11,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
+            "outputs": [],
+            "source": [
+                "cpi_sc.CPIAUCSL.df.head()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "cpi_sc.CPILFESL.df.head()"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "### Rename after add\n",
+                "\n",
+                "You can rename series in the collection with the `rename_series` method. Works the same way as renaming on add."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "def parse_cpi_title(title: str) -> str:\n",
+                "    \"\"\"Parse CPI series title into a readable label.\"\"\"\n",
+                "    return (\n",
+                "        title.lower()\n",
+                "        .replace(\"consumer price index\", \"CPI \")\n",
+                "        .replace(\" for all urban consumers: \", \"\")\n",
+                "        .replace(\" in u.s. city average\", \"\")\n",
+                "        .title()\n",
+                "    )\n",
+                "\n",
+                "\n",
+                "cpi_sc.rename_series(rename=parse_cpi_title)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "cpi_sc.CPIAUCSL.df.head()"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## List metadata\n",
+                "\n",
+                "`SeriesCollection` has a number of list methods to print out the metadata of the series in the collection."
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "### Series in the collection"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "cpi_sc.list_series()"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "### Frequency"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "cpi_sc.list_frequency()"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "### Seasonality"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "cpi_sc.list_seasonality()"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "### Units"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "cpi_sc.list_units()"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "### Dates"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "cpi_sc.list_end_date()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "cpi_sc.list_start_date()"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## Merge data\n",
+                "\n",
+                "`SeriesCollection` supports merging the data into long and wide formats. By default the series ID will be used as the column name or observation label."
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "### Merge long\n",
+                "\n",
+                "Merge the series in the collection into a long pandas dataframe."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "cpi_long = cpi_sc.merge_long()\n",
+                "cpi_long"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "### Merge as-of\n",
+                "\n",
+                "Merge the series in the collection into a wide pandas dataframe based on nearest date. Must define a base series. The base series defines the set of dates to serve of the basis of joining."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "cpi_asof = cpi_sc.merge_asof(base_series_id=\"CPIAUCSL\")\n",
+                "cpi_asof.tail()"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "### Merge wide\n",
+                "\n",
+                "Merge the series in the collection into a wide pandas dataframe. Only works if all the series in the collection share the same date index."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
             "source": [
-                "gdp_df"
+                "cpi_wide = cpi_sc.merge_wide()\n",
+                "cpi_wide.tail()"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3.10.1 ('.venv': poetry)",
             "language": "python",
@@ -733,18 +572,19 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.1"
+            "version": "3.11.2"
         },
+        "orig_nbformat": 4,
         "vscode": {
             "interpreter": {
                 "hash": "9f8da5f516a0f7b58441e46157a772613635e3a9b5450eafa77dccb7c363b35a"
             }
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 5
+    "nbformat_minor": 2
 }
```

### Comparing `pyfredapi-0.6.0/pyfredapi/__init__.py` & `pyfredapi-0.7.0/pyfredapi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.6.0/pyfredapi/_base.py` & `pyfredapi-0.7.0/pyfredapi/_base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,12 @@
-"""The _base module contains the base functions used pyfredapi modules."""
+"""The _base module contains the get request functions used in the pyfredapi modules.
+
+The _base module is not intended to be used directly by the user. It is used by the other
+functions in pyfredapi.
+"""
 
 from functools import lru_cache
 from http import HTTPStatus
 from os import environ
 from typing import Any, Dict, Optional, Union
 
 import requests
@@ -21,15 +25,29 @@
 
     class Config:
         extra = Extra.forbid
 
 
 @lru_cache
 def _get_api_key(api_key: Optional[str] = None) -> str:
-    """Get FRED_API_KEY from the environment."""
+    """Get FRED_API_KEY from the environment.
+
+    api_key : str | None
+        FRED API key. Defaults to None. If None, will check for FRED_API_KEY in the environment.
+
+    Returns
+    -------
+    str
+        The FRED API key.
+
+    Raises
+    ------
+    APIKeyNotFound
+        If the api_key is None and FRED_API_KEY is not in the environment.
+    """
     if api_key is None:
         api_key = environ.get("FRED_API_KEY", None)
 
     if api_key is None:
         raise APIKeyNotFound()
     elif not api_key.isalnum() or len(api_key) != 32:
         raise InvalidAPIKey()
@@ -47,25 +65,30 @@
     """Make a get request to a FRED web service endpoint and return the response as Json.
 
     Base get request that child class methods utilize.
 
     Parameters
     ----------
     endpoint : str
-        The FRED endpoint to hit.
-    api_key : str | None
-        FRED API key. Defaults to None. If None, will search for FRED_API_KEY in the environment.
-    params : Dict[str, Any] | None
+        The FRED API endpoint.
+    api_key : str | None, optional
+        FRED API key. Defaults to None. If None, will check for FRED_API_KEY in the environment.
+    params : Dict[str, Any] | None, optional
         Dictionary of query parameters. Defaults to None.
     base_url : str, optional
         Base fred url. Defaults to https://api.stlouisfed.org/fred.
 
     Returns
     -------
     A dictionary representing the json response.
+
+    Raises
+    ------
+    FredAPIRequestError
+        If the request fails.
     """
     api_key = _get_api_key(api_key)
     _base_params = BaseApiParameters(api_key=api_key)
 
     if not params:
         params = {}
     try:
```

### Comparing `pyfredapi-0.6.0/pyfredapi/category.py` & `pyfredapi-0.7.0/pyfredapi/category.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 ) -> JsonType:
     """Get category by ID. https://fred.stlouisfed.org/docs/api/fred/category.html.
 
     Parameters
     ----------
     category_id : str | None
         Category id of interest.
-    api_key : str | None
+    api_key : str | None, optional
         FRED API key. Defaults to None. If None, will search for FRED_API_KEY in environment variables.
     **kwargs: Dict[str, str], optional
         Additional parameters to FRED API ``category/`` endpoint. Refer to the FRED documentation for a list of all possible parameters.
 
     Returns
     -------
     dict
@@ -92,15 +92,15 @@
 ) -> JsonType:
     """Get category children by category ID. https://fred.stlouisfed.org/docs/api/fred/category_children.html.
 
     Parameters
     ----------
     category_id : str | None
         Category id of interest.
-    api_key : str | None
+    api_key : str | None, optional
         FRED API key. Defaults to None. If None, will search for FRED_API_KEY in environment variables.
     **kwargs : dict, optional
         Additional parameters to FRED API ``category/children`` endpoint. Refer to the FRED documentation for a list of all possible parameters.
 
     Returns
     -------
     dict
@@ -124,15 +124,15 @@
 ) -> JsonType:
     """Get related categories by category ID. https://fred.stlouisfed.org/docs/api/fred/category_related.html.
 
     Parameters
     ----------
     category_id : str
         Category id of interest.
-    api_key : str | None
+    api_key : str | None, optional
         FRED API key. Defaults to None. If None, will search for FRED_API_KEY in environment variables.
     **kwargs : dict, optional
         Additional parameters to FRED API ``category/children`` endpoint. Refer to the FRED documentation for a list of all possible parameters.
 
 
     Returns
     -------
@@ -144,25 +144,23 @@
         api_key=api_key,
         endpoint="category/related",
         params=frozendict(params.dict(exclude_none=True)),
     )
 
 
 def get_category_series(
-    category_id: int,
-    api_key: ApiKeyType = None,
-    **kwargs: KwargsType,
+    category_id: int, api_key: ApiKeyType = None, **kwargs: KwargsType
 ) -> Dict[str, SeriesInfo]:
     """Get the series info for each series in a category by category ID. https://fred.stlouisfed.org/docs/api/fred/category_series.html.
 
     Parameters
     ----------
     category_id : str
         Category id of interest.
-    api_key : str | None
+    api_key : str | None, optional
         FRED API key. Defaults to None. If None, will search for FRED_API_KEY in environment variables.
     **kwargs : dict, optional
         Additional parameters to FRED API ``category/children`` endpoint. Refer to the FRED documentation for a list of all possible parameters.
 
     Returns
     -------
     dict
@@ -186,15 +184,15 @@
 ) -> JsonOrPdType:
     """Get the FRED tags for a category by category ID. https://fred.stlouisfed.org/docs/api/fred/category_tags.html.
 
     Parameters
     ----------
     category_id : str | None
         Category id of interest.
-    api_key : str | None
+    api_key : str | None, optional
         FRED API key. Defaults to None. If None, will search for FRED_API_KEY in environment variables.
     return_format : str | ReturnFormat
         Define how to return the response. Must be either 'json' or 'pandas'.
     **kwargs : dict, optional
         Additional parameters to FRED API ``category/children`` endpoint. Refer to the FRED documentation for a list of all possible parameters.
 
     Returns
@@ -224,15 +222,15 @@
 ) -> JsonOrPdType:
     """Get the related FRED tags for a category by category ID. https://fred.stlouisfed.org/docs/api/fred/category_related_tags.html.
 
     Parameters
     ----------
     category_id : str | None
         Category id of interest.
-    api_key : str | None
+    api_key : str | None, optional
         FRED API key. Defaults to None. If None, will search for FRED_API_KEY in environment variables.
     return_format : str | ReturnFormat
         Define how to return the response. Must be either 'json' or 'pandas'.
     **kwargs : dict, optional
         Additional parameters to FRED API ``category/children`` endpoint. Refer to the FRED documentation for a list of all possible parameters.
 
     Returns
```

### Comparing `pyfredapi-0.6.0/pyfredapi/maps.py` & `pyfredapi-0.7.0/pyfredapi/maps.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 def get_geoseries_info(series_id: str, api_key: ApiKeyType = None) -> GeoseriesInfo:
     """Request the metadata for a given geo series id. https://fred.stlouisfed.org/docs/api/geofred/series_group.html.
 
     Parameters
     ----------
     series_id : str
         Series id of interest.
-    api_key : str | None
+    api_key : str | None, optional
         FRED API key. Defaults to None. If None, will search for FRED_API_KEY in environment variables.
 
     Returns
     -------
     GeoseriesInfo
         An instance of GeoseriesInfo.
     """
@@ -108,15 +108,15 @@
 ) -> JsonType:
     """Request shape files from FRED in Well-known text (WKT) format.
 
     Parameters
     ----------
     shape : One of "bea", "msa", "frb", "necta", "state", "country", "county", "censusregion", "censusdivision"
         Define the shape of Well-known text (WKT) data.
-    api_key : str | None
+    api_key : str | None, optional
         FRED API key. Defaults to None. If None, will search for FRED_API_KEY in environment variables.
 
     Returns
     -------
     dict
         Dictionary representing the json response.
     """
@@ -141,15 +141,15 @@
     For example, you can request Per Capita Personal Income by State (series_id: WIPCPI) over a specific time period.
     https://fred.stlouisfed.org/docs/api/geofred/series_data.html.
 
     Parameters
     ----------
     series_id : str
         Series id of interest. Not all series that are in FRED have geographical data.
-    api_key : str | None
+    api_key : str | None, optional
         FRED API key. Defaults to None. If None, will search for FRED_API_KEY in environment variables.
     start_date : str, optional
         Define start date. YYYY-MM-DD formatted string.
     end_date : str, optional
         Define the end date. YYYY-MM-DD formatted string.
     return_format : Literal[json, pandas] | ReturnFormat
         Define how to return the response. Must be either 'json' or 'pandas'. Defaults to 'pandas'.
```

### Comparing `pyfredapi-0.6.0/pyfredapi/releases.py` & `pyfredapi-0.7.0/pyfredapi/releases.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
 
 def get_releases(api_key: ApiKeyType = None, **kwargs: KwargsType) -> JsonType:
     """Get all releases of economic data. https://fred.stlouisfed.org/docs/api/fred/releases.html.
 
     Parameters
     ----------
-    api_key : str | None
+    api_key : str | None, optional
         FRED API key. Defaults to None. If None, will search for FRED_API_KEY in environment variables.
     **kwargs : dict, optional
         Additional parameters to FRED API ``releases/`` endpoint. Refer to the FRED documentation for a list of all possible parameters.
 
     Returns
     -------
     Dictionary representing the Json response
@@ -66,15 +66,15 @@
 
 
 def get_releases_dates(api_key: ApiKeyType = None, **kwargs: KwargsType) -> JsonType:
     """Get release dates for all releases of economic data. https://fred.stlouisfed.org/docs/api/fred/releases_dates.html.
 
     Parameters
     ----------
-    api_key : str | None
+    api_key : str | None, optional
         FRED API key. Defaults to None. If None, will search for FRED_API_KEY in environment variables.
     **kwargs : dict, optional
         Additional parameters to FRED API ``releases/dates`` endpoint. Refer to the FRED documentation for a list of all possible parameters.
 
     Returns
     -------
     Dictionary representing the Json response
@@ -92,15 +92,15 @@
 ) -> JsonType:
     """Get a release of economic data. https://fred.stlouisfed.org/docs/api/fred/release.html.
 
     Parameters
     ----------
     release_id : int
         Release id of interest.
-    api_key : str | None
+    api_key : str | None, optional
         FRED API key. Defaults to None. If None, will search for FRED_API_KEY in environment variables.
     **kwargs : dict, optional
         Additional parameters to FRED API ``release/`` endpoint. Refer to the FRED documentation for a list of all possible parameters.
 
     Returns
     -------
     Dictionary representing the Json response.
@@ -122,15 +122,15 @@
 ) -> JsonType:
     """Get release dates for a release of economic data. https://fred.stlouisfed.org/docs/api/fred/release_dates.html.
 
     Parameters
     ----------
     release_id : int
         Release id of interest.
-    api_key : str | None
+    api_key : str | None, optional
         FRED API key. Defaults to None. If None, will search for FRED_API_KEY in environment variables.
     **kwargs : dict, optional
         Additional parameters to FRED API ``release/dates/`` endpoint. Refer to the FRED documentation for a list of all possible parameters.
 
     Returns
     -------
     Dictionary representing the Json response.
@@ -148,15 +148,15 @@
 ) -> JsonType:
     """Get the series on a release of economic data. https://fred.stlouisfed.org/docs/api/fred/release_series.html.
 
     Parameters
     ----------
     release_id : int
         Release id of interest.
-    api_key : str | None
+    api_key : str | None, optional
         FRED API key. Defaults to None. If None, will search for FRED_API_KEY in environment variables.
     **kwargs : dict, optional
         Additional parameters to FRED API release/release_series/ endpoint. Refer to the FRED documentation for a list of all possible parameters.
 
     Returns
     -------
     Dictionary representing the Json response.
@@ -174,15 +174,15 @@
 ) -> JsonType:
     """Get the sources for a release of economic data. https://fred.stlouisfed.org/docs/api/fred/release_sources.html.
 
     Parameters
     ----------
     release_id : int
         Release id of interest.
-    api_key : str | None
+    api_key : str | None, optional
         FRED API key. Defaults to None. If None, will search for FRED_API_KEY in environment variables.
     **kwargs : dict, optional
         Additional parameters to FRED API ``release/sources/`` endpoint. Refer to the FRED documentation for a list of all possible parameters.
 
     Returns
     -------
     Dictionary representing the Json response.
@@ -200,15 +200,15 @@
 ) -> JsonType:
     """Get the FRED tags for a release. https://fred.stlouisfed.org/docs/api/fred/release_tags.html.
 
     Parameters
     ----------
     release_id : int
         Release id of interest.
-    api_key : str | None
+    api_key : str | None, optional
         FRED API key. Defaults to None. If None, will search for FRED_API_KEY in environment variables.
     **kwargs : dict, optional
         Additional parameters to FRED API ``release/tags/`` endpoint. Refer to the FRED documentation for a list of all possible parameters.
 
     Returns
     -------
     Dictionary representing the Json response.
@@ -228,15 +228,15 @@
 
     Parameters
     ----------
     release_id : int
         Release id of interest.
     tag_names : str
         A semicolon delimited list of tag names that series match all of. See the related request fred/release/tags.
-    api_key : str | None
+    api_key : str | None, optional
         FRED API key. Defaults to None. If None, will search for FRED_API_KEY in environment variables.
     **kwargs : dict, optional
         Additional parameters to FRED API ``release/related_tags/`` endpoint. Refer to the FRED documentation for a list of all possible parameters.
 
     Returns
     -------
     Dictionary representing the Json response.
@@ -254,15 +254,15 @@
 ) -> JsonType:
     """Get release table trees for a given release. https://fred.stlouisfed.org/docs/api/fred/release_tables.html.
 
     Parameters
     ----------
     release_id : int
         Release id of interest.
-    api_key : str | None
+    api_key : str | None, optional
         FRED API key. Defaults to None. If None, will search for FRED_API_KEY in environment variables.
     **kwargs : dict, optional
         Additional parameters to FRED API ``release/tables/`` endpoint. Refer to the FRED documentation for a list of all possible parameters.
 
     Returns
     -------
     Dictionary representing the Json response.
```

### Comparing `pyfredapi-0.6.0/pyfredapi/series.py` & `pyfredapi-0.7.0/pyfredapi/series.py`

 * *Files 7% similar despite different names*

```diff
@@ -145,15 +145,15 @@
 ) -> SeriesInfo:
     """Get an economic data series information by ID. https://fred.stlouisfed.org/docs/api/fred/series.html.
 
     Parameters
     ----------
     series_id : str
         Series id of interest.
-    api_key : str | None
+    api_key : str | None, optional
         FRED API key. Defaults to None. If None, will search for FRED_API_KEY in environment variables.
     **kwargs : dict, optional
         Additional parameters to FRED API ``series/`` endpoint. Refer to the FRED documentation for a list of all possible parameters.
 
     Returns
     -------
     SeriesInfo
@@ -173,15 +173,15 @@
 ) -> JsonType:
     """Get the categories for an economic data series by ID. https://fred.stlouisfed.org/docs/api/fred/series_categories.html.
 
     Parameters
     ----------
     series_id : str
         Series id of interest.
-    api_key : str | None
+    api_key : str | None, optional
         FRED API key. Defaults to None. If None, will search for FRED_API_KEY in environment variables.
     **kwargs : dict, optional
         Additional parameters to FRED API ``series/categories`` endpoint. Refer to the FRED documentation for a list of all possible parameters.
 
     Returns
     -------
     dict
@@ -203,15 +203,15 @@
 ) -> JsonOrPdType:
     """Get the observations or data values for an economic data series by ID. https://fred.stlouisfed.org/docs/api/fred/series_observations.html.
 
     Parameters
     ----------
     series_id : str
         Series id of interest.
-    api_key : str | None
+    api_key : str | None, optional
         FRED API key. Defaults to None. If None, will search for FRED_API_KEY in environment variables.
     return_format : Literal[json, pandas] | ReturnFormat, optional
         Define how to return the response. Must be either 'json' or 'pandas'. Defaults to 'pandas'.
     **kwargs : dict, optional
         Additional parameters to FRED API ``series/observations`` endpoint. Refer to the FRED documentation for a list of all possible parameters.
 
     Returns
@@ -239,15 +239,15 @@
 ) -> JsonType:
     """Get the FRED release for an economic data series by ID. https://fred.stlouisfed.org/docs/api/fred/series_release.html.
 
     Parameters
     ----------
     series_id : str
         Series id of interest.
-    api_key : str | None
+    api_key : str | None, optional
         FRED API key. Defaults to None. If None, will search for FRED_API_KEY in environment variables.
     **kwargs : dict, optional
         Additional parameters to FRED API ``series/releases`` endpoint. Refer to the FRED documentation for a list of all possible parameters.
 
     Returns
     -------
     dict
@@ -266,15 +266,15 @@
 ) -> JsonType:
     """Get the FRED tags for an economic data series by ID. https://fred.stlouisfed.org/docs/api/fred/series_tags.html.
 
     Parameters
     ----------
     series_id : str
         Series id of interest.
-    api_key : str | None
+    api_key : str | None, optional
         FRED API key. Defaults to None. If None, will search for FRED_API_KEY in environment variables.
     **kwargs : dict, optional
         Additional parameters to FRED API ``series/tags`` endpoint. Refer to the FRED documentation for a list of all possible parameters.
 
     Returns
     -------
     dict
@@ -293,15 +293,15 @@
 ) -> JsonType:
     """Get the FRED updates for an economic data series by ID. https://fred.stlouisfed.org/docs/api/fred/series_updates.html.
 
     Parameters
     ----------
     series_id : str
         Series id of interest.
-    api_key : str | None
+    api_key : str | None, optional
         FRED API key. Defaults to None. If None, will search for FRED_API_KEY in environment variables.
     **kwargs : dict, optional
         Additional parameters to FRED API ``series/updates`` endpoint. Refer to the FRED documentation for a list of all possible parameters.
 
     Returns
     -------
     dict
@@ -322,15 +322,15 @@
 
     Vintage dates are the release dates for a series excluding release dates when the data did not change. https://fred.stlouisfed.org/docs/api/fred/series_vintagesdates.html.
 
     Parameters
     ----------
     series_id : str
         Series id of interest.
-    api_key : str | None
+    api_key : str | None, optional
         FRED API key. Defaults to None. If None, will search for FRED_API_KEY in environment variables.
     **kwargs : dict, optional
         Additional parameters to FRED API ``series/vintagedates`` endpoint. Refer to the FRED documentation for a list of all possible parameters.
 
     Returns
     -------
     List[str]
@@ -353,15 +353,15 @@
 ) -> JsonOrPdType:
     """Get the observations or data values for all releases an economic data series by ID.
 
     Parameters
     ----------
     series_id : str
         Series id of interest.
-    api_key : str | None
+    api_key : str | None, optional
         FRED API key. Defaults to None. If None, will search for FRED_API_KEY in environment variables.
     return_format : Literal["json", "pandas"] | ReturnFormat, optional
         In what format to return the response. Must be either 'json' or 'pandas'. Defaults to 'pandas'.
     **kwargs : dict, optional
         Additional parameters to FRED API ``series/observation`` endpoint. Refer to the FRED documentation for a list of all possible parameters.
 
     Returns
@@ -399,15 +399,15 @@
 
     Includes only the the initial release of the series and excludes all revisions.
 
     Parameters
     ----------
     series_id : str
         Series id of interest.
-    api_key : str | None
+    api_key : str | None, optional
         FRED API key. Defaults to None. If None, will search for FRED_API_KEY in environment variables.
     return_format : Literal["json", "pandas"] | ReturnFormat, optional
         In what format to return the response. Must be either 'json' or 'pandas'. Defaults to 'pandas'.
     **kwargs : dict, optional
         Additional parameters to FRED API ``series/observation`` endpoint. Refer to the FRED documentation for a list of all possible parameters.
 
     Returns
@@ -447,15 +447,15 @@
 
     Parameters
     ----------
     series_id : str
         Series id of interest.
     date : str
         Include only data revisions made on or before this date.
-    api_key : str | None
+    api_key : str | None, optional
         FRED API key. Defaults to None. If None, will search for FRED_API_KEY in environment variables.
     return_format : Literal["json", "pandas"] | ReturnFormat, optional
         In what format to return the response. Must be either 'json' or 'pandas'. Defaults to 'pandas'.
     **kwargs : dict, optional
         Additional parameters to FRED API ``series/observation`` endpoint. Refer to the FRED documentation for a list of all possible parameters.
 
     Returns
@@ -490,15 +490,15 @@
 ) -> JsonOrPdType:
     """Get economic data series that match search text. `FRED docs <https://fred.stlouisfed.org/docs/api/fred/series_search.html>`_.
 
     Parameters
     ----------
     search_text : str
         The text to match against.
-    api_key : str | None
+    api_key : str | None, optional, optional
         FRED API key. Defaults to None. If None, will search for FRED_API_KEY in environment variables.
     search_type : Literal["full_text", "series_id"]
         Defines which type of search to preform. One of the following strings: 'full_text', 'series_id'.
         Parameter docs: https://fred.stlouisfed.org/docs/api/fred/series_search.html#search_type.
     return_format : : Literal["json", "pandas"] | ReturnFormat, optional
         In what format to return the response. Must be either 'json' or 'pandas'. Defaults to 'pandas'.
     **kwargs : dict, optional
@@ -535,15 +535,15 @@
 ) -> JsonOrPdType:
     """Get the FRED tags for a series search. https://fred.stlouisfed.org/docs/api/fred/release_related_tags.html.
 
     Parameters
     ----------
     search_text : str
         The text to match against.
-    api_key : str | None
+    api_key : str | None, optional, optional
         FRED API key. Defaults to None. If None, will search for FRED_API_KEY in environment variables.
     return_format : : Literal["json", "pandas"] | ReturnFormat, optional
         In what format to return the response. Must be either 'json' or 'pandas'. Defaults to 'pandas'.
     **kwargs : dict, optional
         Additional parameters to FRED API ``series/observation`` endpoint. Refer to the FRED documentation for a list of all possible parameters.
 
     Returns
@@ -562,15 +562,15 @@
                 "series_search_text": search_text,
                 **params.dict(exclude_none=True),
             }
         ),
     )
 
     if return_format == ReturnFormat.pandas:
-        return pd.DataFrame.from_dict(response["tags"])
+        return _convert_to_pandas(response["tags"])
     return response
 
 
 def search_series_related_tags(
     search_text: str,
     tag_names: str,
     api_key: ApiKeyType = None,
@@ -581,15 +581,15 @@
 
     Parameters
     ----------
     search_text : str
         The text to match against.
     tag_names : str
         A semicolon delimited list of tag names that series match all of.
-    api_key : str | None
+    api_key : str | None, optional
         FRED API key. Defaults to None. If None, will search for FRED_API_KEY in environment variables.
     return_format : : Literal["json", "pandas"] | ReturnFormat, optional
         In what format to return the response. Must be either 'json' or 'pandas'. Defaults to 'pandas'.
     **kwargs : dict, optional
         Additional parameters to FRED API ``series/observation`` endpoint. Refer to the FRED documentation for a list of all possible parameters.
 
     Returns
```

### Comparing `pyfredapi-0.6.0/pyfredapi/series_collection.py` & `pyfredapi-0.7.0/pyfredapi/series_collection.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 """The series_collection module contains the SeriesCollection implementation.
 
 SeriesCollection is meant to make handling multiple series easier. Often users of the FRED API will want analyze multiple economic series. This can be done with `FredSeries` alone, but can be tedious and cumbersome.
 `pyfredapi` offers the `SeriesCollection` class to streamline the process of collecting and munging the data for plotting and analysis.
 """
 
+import time
 from dataclasses import dataclass
 from typing import Callable, Dict, List, Union
 
 import pandas as pd
-import plotly.express as px
-from plotly.graph_objects import Figure
 from rich.console import Console
 
 from pyfredapi._base import _get_api_key
 from pyfredapi.series import SeriesInfo, get_series, get_series_info
 
+try:
+    import plotly.express as px
+    from plotly.graph_objects import Figure
+except ImportError:
+    pass
+
 console = Console()
 
 
 date_cols = ["date", "realtime_start", "realtime_end"]
 
 
 @dataclass
@@ -59,31 +64,36 @@
         def format_title(title, start_date: str, end_date: str, subtitle=None):
             title = f"{title}, {start_date} - {end_date}"
             if not subtitle:
                 return title
             subtitle = f"<sup>{subtitle}</sup>"
             return f"{title}<br>{subtitle}"
 
-        fig = px.line(
-            data_frame=self.df,
-            x="date",
-            y=value_col,
-            title=format_title(
-                title=self.info.title,
-                start_date=self.info.observation_start,
-                end_date=self.info.observation_end,
-                subtitle=f"{self.info.seasonal_adjustment}, {self.info.units}",
-            ),
-            color_discrete_sequence=px.colors.qualitative.Safe,
-            labels=dict(
-                value=f"{self.info.id}",
-                date="Date",
-                variable="Series",
-            ),
-        )
+        try:
+            fig = px.line(
+                data_frame=self.df,
+                x="date",
+                y=value_col,
+                title=format_title(
+                    title=self.info.title,
+                    start_date=self.info.observation_start,
+                    end_date=self.info.observation_end,
+                    subtitle=f"{self.info.seasonal_adjustment}, {self.info.units}",
+                ),
+                color_discrete_sequence=px.colors.qualitative.Safe,
+                labels=dict(
+                    value=f"{self.info.id}",
+                    date="Date",
+                    variable="Series",
+                ),
+            )
+        except NameError as e:
+            raise ImportError(
+                "Plotly is required to create plots. You can install pyfredapi with plotly with `pip install 'pyfredapi[plot]`"
+            ) from e
 
         fig.update_layout(showlegend=False)
 
         return fig
 
 
 def _rename_series(
@@ -104,116 +114,178 @@
     if series_name is None or rename is None:
         series_name = series_data.info.id
 
     return series_name
 
 
 class SeriesCollection:
-    """A collection of pyfredapi.SeriesData objects.
+    """A collection of `pyfredapi.SeriesData` objects.
 
     Useful when you need to collect and manage multiple economic series. Provides methods
     for listing metadata, collecting data, and merging data together in long or wide formats.
     """
 
-    def __init__(self, api_key: Union[str, None] = None):
-        """Create instance of SeriesCollection.
+    def __init__(
+        self,
+        series_id: Union[List[str], str, None] = None,
+        api_key: Union[str, None] = None,
+        rename: Union[Dict[str, str], Callable[[str], str], None] = None,
+        drop_realtime: bool = True,
+        sleep: float = 0.1,
+        **kwargs,
+    ):
+        """Create an instance of SeriesCollection.
 
         Parameters
         ----------
-        api_key : str | None
+        series_id : List[str] | str | None, optional
+            List of series IDs to add to collection.
+        api_key : str | None, optional
             FRED API key. Defaults to None. If None, will search for FRED_API_KEY in environment variables.
+        drop_realtime : bool, optional
+            Indicates if you want to drop the realtime columns.
+        rename : Union[Dict[str, str], Callable[[str], str], None], optional
+            Label to give series. Defaults to series ID.
+        sleep : float, optional
+            Time to sleep between requests. Defaults to 0.1.
+        **kwargs : dict, optional
+            Additional parameters to FRED API `series/` endpoint.
+            Refer to the FRED documentation for a list of all possible parameters.
         """
+        self._data: List[SeriesData] = []
+        self.sleep = sleep
+        self.rename = rename
+        self.drop_realtime = drop_realtime
         if api_key is None:
             self.api_key = _get_api_key()
-        self.data: Dict[str, SeriesData] = {}
+
+        if isinstance(series_id, str):
+            series_id = [series_id]
+        if series_id is None:
+            series_id = []
+
+        for sid in series_id:
+            time.sleep(sleep)
+            if sid in self._data:
+                print(f"Already have {sid}")
+                continue
+
+            print(f"Requesting series {sid}...")
+
+            series_info = get_series_info(series_id=sid)
+            series_df = get_series(series_id=sid, api_key=self.api_key, **kwargs)
+            assert isinstance(series_df, pd.DataFrame)  # noqa: S101
+
+            series_data = SeriesData(info=series_info, df=series_df)
+
+            if drop_realtime:
+                series_data.df.drop(
+                    ["realtime_start", "realtime_end"], inplace=True, axis=1
+                )
+            if rename:
+                series_name = _rename_series(series_data, rename)
+            else:
+                series_name = series_data.info.id
+
+            series_data.df.rename(columns={"value": series_name}, inplace=True)
+            self._data.append(series_data)
+            setattr(self, sid, series_data)
+
+    def __getitem__(self, key):
+        return [s for s in self._data if s.info.id == key].pop()
+
+    def __delitem__(self, key):
+        self.remove(key)
+
+    def __iter__(self):
+        for series_info in self._data:
+            yield series_info
+
+    def __len__(self):
+        return len(self._data)
+
+    def __rich_repr__(self):
+        yield self._data
 
     def rename_series(self, rename):
         """Rename series columns."""
-        for series_id, series_data in self.data.items():
+        for series_data in self._data:
             series_name = _rename_series(series_data=series_data, rename=rename)
 
             orig_col_name = [
-                c
-                for c in self.data[series_id].df.columns.tolist()
-                if c not in date_cols
+                c for c in series_data.df.columns.tolist() if c not in date_cols
             ].pop()
 
-            self.data[series_id].df.rename(columns={orig_col_name: series_name}, inplace=True)  # type: ignore
+            series_data.df.rename(columns={orig_col_name: series_name}, inplace=True)
 
-    def add_series(
-        self,
-        series_ids: Union[str, List[str]],
-        drop_realtime: bool = True,
-        rename: Union[Dict[str, str], Callable[[str], str], None] = None,
-        **kwargs,
-    ) -> None:
-        """Add series to class instance.
+    def add(self, series_ids: Union[str, List[str]], **kwargs) -> None:
+        """Add series to the collection.
 
         A request to the FRED api will be made for the series. The data will
         be formatted as as pandas dataframe.
 
         After adding a series, you can access it via an attribute or
         in the responses dict.
 
         Parameters
         ----------
         series_ids : Union[str, List[str]]
             Series to add to collection.
-        drop_realtime : bool
-            Indicates if you want to drop the realtime columns.
-        rename : Union[Dict[str, str], Callable[[str], str], None]
-            Label to give series. Defaults to series ID.
         **kwargs : dict, optional
-            Additional parameters to FRED API series/ endpoint. Refer to the FRED documentation for a list of all possible parameters.
+            Additional parameters to FRED API `series/` endpoint.
+            Refer to the FRED documentation for a list of all possible parameters.
         """
         if isinstance(series_ids, str):
             series_ids = [series_ids]
 
         for series_id in series_ids:
-            if series_id in self.data:
+            time.sleep(self.sleep)
+            if series_id in self._data:
                 print(f"Already have {series_id}")
                 continue
 
             print(f"Requesting series {series_id}...")
 
+            info = get_series_info(series_id=series_id)
             df = get_series(series_id=series_id, api_key=self.api_key, **kwargs)
             assert isinstance(df, pd.DataFrame)  # noqa: S101
 
-            series_data = SeriesData(info=get_series_info(series_id=series_id), df=df)
+            series_data = SeriesData(info=info, df=df)
 
-            if drop_realtime:
+            if self.drop_realtime:
                 series_data.df.drop(
                     ["realtime_start", "realtime_end"], inplace=True, axis=1
                 )
-            if rename:
-                series_name = _rename_series(series_data, rename)
+            if self.rename:
+                series_name = _rename_series(series_data, self.rename)
             else:
                 series_name = series_data.info.id
 
             series_data.df.rename(columns={"value": series_name}, inplace=True)
-            self.data[series_id] = series_data
+            self._data.append(series_data)
             setattr(self, series_id, series_data)
 
-    def drop_series(self, series_ids: Union[str, List[str]]) -> None:
-        """Drop series from collection.
+    def remove(self, series_ids: Union[str, List[str]]) -> None:
+        """Remove series from collection.
 
         Parameters
         ----------
         series_ids : Union[str, List[str]]
             Series ids to remove from collection.
         """
         if isinstance(series_ids, str):
             series_ids = [series_ids]
 
         for series_id in series_ids:
             try:
-                del self.data[series_id]
-            except KeyError:
-                raise ValueError from KeyError(f"No series '{series_id}' in collection")
+                series_info = [s for s in self._data if s.info.id == series_id].pop()
+            except IndexError as e:
+                raise ValueError(f"No series '{series_id}' in collection") from e
 
+            self._data.remove(series_info)
             delattr(self, series_id)
             print(f"Removed series {series_id}")
 
     def merge_long(self, col_name: Union[str, None] = None) -> pd.DataFrame:
         """Merge the series in the collection into a long pandas dataframe.
 
         Parameters
@@ -226,15 +298,15 @@
         pd.DataFrame
             Long pandas dataframe.
         """
         if col_name is None:
             col_name = "series"
 
         long_df_prep = []
-        for series in list(self.data.values()):
+        for series in self._data:
             series_name = [
                 c for c in series.df.columns.tolist() if c not in date_cols
             ].pop()
             long_df = series.df.copy()
             long_df = long_df.rename(columns={series_name: "value"})
             long_df[col_name] = series_name
             long_df_prep.append(long_df)
@@ -245,137 +317,121 @@
         """Merge the series in the collection into a wide pandas dataframe. Only works if all the series in the collection share the same date index.
 
         Returns
         -------
         pd.DataFrame
             Wide pandas dataframe.
         """
-        wide_df_prep = [
-            series.df.copy().set_index("date") for series in list(self.data.values())  # type: ignore
-        ]
+        wide_df_prep = [series.df.copy().set_index("date") for series in self._data]
         wide_df = pd.concat(wide_df_prep, axis=1)
         return wide_df.reset_index()
 
-    def merge_asof(
-        self,
-        base_series_id: str,
-    ) -> pd.DataFrame:
+    def merge_asof(self, base_series_id: str) -> pd.DataFrame:
         """Merge the series in the collection into a wide pandas dataframe based on nearest date.
 
         Uses pandas `merge_asof` methods to merge the data based on nearest date.
 
         Parameters
         ----------
         base_series_id: str
             Series ID of the series to serve of the basis for joining.
 
         Returns
         -------
         pd.DataFrame
             Wide pandas dataframe.
         """
-        base_df = self.data[base_series_id].df.copy()
-        for series_data in list(self.data.values()):
+        base_series = [
+            series_info
+            for series_info in self._data
+            if series_info.info.id == base_series_id
+        ].pop()
+        base_df = base_series.df.copy()
+        for series_data in self._data:
             if base_series_id == series_data.info.id:
                 continue
             df = series_data.df.copy()
-            base_df = pd.merge_asof(left=base_df, right=df, on="date")  # type: ignore
+            base_df = pd.merge_asof(left=base_df, right=df, on="date")
 
-        return base_df  # type: ignore
+        return base_df
 
     def list_series(self) -> None:
         """List the series' id and title."""
-        for series_data in list(self.data.values()):
+        for series_data in self._data:
             console.print(f"{series_data.info.id}: {series_data.info.title}")
 
     def list_seasonality(self) -> None:
         """List the series' seasonality."""
         seasonal_adjustments = [
-            series_data.info.seasonal_adjustment
-            for series_data in list(self.data.values())
+            series_data.info.seasonal_adjustment for series_data in self._data
         ]
         distinct_seasonality = set(seasonal_adjustments)
 
         if len(distinct_seasonality) == 1:
             print(f"All series are {distinct_seasonality.pop()}")
             return
 
         for season in distinct_seasonality:
             console.rule(f"[bold red]Series that are {season}")
-            for series_data in list(self.data.values()):
+            for series_data in self._data:
                 if series_data.info.seasonal_adjustment == season:
                     console.print(f"{series_data.info.id}: {series_data.info.title}")
 
     def list_frequency(self) -> None:
         """List the series' frequency."""
-        frequencies = [
-            series_data.info.frequency for series_data in list(self.data.values())
-        ]
+        frequencies = [series_data.info.frequency for series_data in self._data]
         distinct_freq = set(frequencies)
 
         if len(distinct_freq) == 1:
             print(f"All series are {distinct_freq.pop()}")
             return
 
         for freq in distinct_freq:
             console.rule(f"[bold red]Series that are published {freq}")
-            for series_data in list(self.data.values()):
+            for series_data in self._data:
                 if series_data.info.frequency == freq:
                     console.print(f"{series_data.info.id}: {series_data.info.title}")
 
     def list_units(self) -> None:
         """List the series' measurement units."""
-        units = [series_data.info.units for series_data in list(self.data.values())]
+        units = [series_data.info.units for series_data in self._data]
         distinct_units = set(units)
 
         if len(distinct_units) == 1:
             print(f"All series are that are measured in {distinct_units.pop()}")
             return
 
         for unit in distinct_units:
             console.rule(f"[bold red]Series that are measured in {unit}")
-            for series_data in list(self.data.values()):
+            for series_data in self._data:
                 if series_data.info.units == unit:
                     console.print(f"{series_data.info.id}: {series_data.info.title}")
 
     def list_end_date(self) -> None:
         """List the series' latest date."""
-        end_dates = [
-            series_data.info.observation_end for series_data in list(self.data.values())
-        ]
+        end_dates = [series_data.info.observation_end for series_data in self._data]
         distinct_end_dates = set(end_dates)
 
         if len(distinct_end_dates) == 1:
             print(f"All series end on {distinct_end_dates.pop()}")
             return
 
         for date in distinct_end_dates:
             console.rule(f"[bold red]Series that end on {date}")
-            for series_data in list(self.data.values()):
+            for series_data in self._data:
                 if series_data.info.observation_end == date:
                     console.print(f"{series_data.info.id}: {series_data.info.title}")
 
     def list_start_date(self) -> None:
         """List the series' earliest date."""
-        start_dates = [
-            series_data.info.observation_start
-            for series_data in list(self.data.values())
-        ]
+        start_dates = [series_data.info.observation_start for series_data in self._data]
         distinct_start_dates = set(start_dates)
 
         if len(distinct_start_dates) == 1:
             print(f"All series start on {distinct_start_dates.pop()}")
             return
 
         for date in distinct_start_dates:
             console.rule(f"[bold red]Series that start on {date}")
-            for series_data in list(self.data.values()):
+            for series_data in self._data:
                 if series_data.info.observation_start == date:
                     console.print(f"{series_data.info.id}: {series_data.info.title}")
-
-    def plot(self):
-        """Make a basic plotly time series plot with all series in the collection."""
-        raise NotImplementedError
-
-    def extract_series(self):
-        """Return a new instance of SeriesCollection, with a subset of data from this instance."""
-        raise NotImplementedError
```

### Comparing `pyfredapi-0.6.0/pyfredapi/sources.py` & `pyfredapi-0.7.0/pyfredapi/sources.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 
 def get_sources(api_key: ApiKeyType = None, **kwargs: KwargsType) -> JsonType:
     """Get all sources of economic data. https://fred.stlouisfed.org/docs/api/fred/sources.html.
 
     Parameters
     ----------
-    api_key : str | None
+    api_key : str | None, optional
         FRED API key. Defaults to None. If None, will search for FRED_API_KEY in environment variables.
     **kwargs : dict, optional
         Additional parameters to FRED API ``sources/`` endpoint. Refer to the FRED documentation for a list of all possible parameters.
 
     Returns
     -------
     Dictionary representing the Json response
@@ -56,15 +56,15 @@
 ) -> JsonType:
     """Get a source of economic data. https://fred.stlouisfed.org/docs/api/fred/source.html.
 
     Parameters
     ----------
     source_id : int
         Source id of interest.
-    api_key : str | None
+    api_key : str | None, optional
         FRED API key. Defaults to None. If None, will search for FRED_API_KEY in environment variables.
     **kwargs : dict, optional
         Additional parameters to FRED API ``source/`` endpoint. Refer to the FRED documentation for a list of all possible parameters.
 
     Returns
     -------
     Dictionary representing the Json response
@@ -82,15 +82,15 @@
 ):
     """Get the releases for a source. https://fred.stlouisfed.org/docs/api/fred/source.html.
 
     Parameters
     ----------
     source_id : int
         Source id of interest.
-    api_key : str | None
+    api_key : str | None, optional
         FRED API key. Defaults to None. If None, will search for FRED_API_KEY in environment variables.
     **kwargs : dict, optional
         Additional parameters to FRED API ``source/releases`` endpoint.
         Refer to the FRED documentation for a list of all possible parameters.
 
     Returns
     -------
```

### Comparing `pyfredapi-0.6.0/pyfredapi/tags.py` & `pyfredapi-0.7.0/pyfredapi/tags.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
 
 def get_tags(api_key: ApiKeyType = None, **kwargs: KwargsType) -> JsonType:
     """Get FRED tags. https://fred.stlouisfed.org/docs/api/fred/tags.html.
 
     Parameters
     ----------
-    api_key : str | None
+    api_key : str | None, optional
         FRED API key. Defaults to None. If None, will search for FRED_API_KEY in environment variables.
     **kwargs : dict, optional
         Additional parameters to FRED API ``tags/`` endpoint. Refer to the FRED documentation for a list of all possible parameters.
 
     Returns
     -------
     dict
@@ -71,15 +71,15 @@
 ) -> JsonType:
     """Get related FRED tags for one or more FRED tags. https://fred.stlouisfed.org/docs/api/fred/related_tags.html.
 
     Parameters
     ----------
     tag_names : str
         A semicolon delimited list of tag names that series match all of.
-    api_key : str | None
+    api_key : str | None, optional
         FRED API key. Defaults to None. If None, will search for FRED_API_KEY in the environment.
     **kwargs : dict, optional
         Additional parameters to FRED API ``related_tags/`` endpoint. Refer to the FRED documentation for a list of all possible parameters.
 
     Returns
     -------
     dict
@@ -101,15 +101,15 @@
 ) -> JsonType:
     """Get the series matching all tags in the tag_names parameter. https://fred.stlouisfed.org/docs/api/fred/tags_series.html.
 
     Parameters
     ----------
     tag_names : str
         A semicolon delimited list of tag names that series match all of.
-    api_key : str | None
+    api_key : str | None, optional
         FRED API key. Defaults to None. If None, will search for FRED_API_KEY in environment variables.
     **kwargs : dict, optional
         Additional parameters to FRED API ``tags/series`` endpoint. Refer to the FRED documentation for a list of all possible parameters.
 
     Returns
     -------
     dict
```

### Comparing `pyfredapi-0.6.0/pyfredapi/exceptions/exceptions.py` & `pyfredapi-0.7.0/pyfredapi/exceptions/exceptions.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,19 +15,18 @@
         """Error raised when the API Key is invalid."""
         super().__init__(
             "API key must be a 32 character lower-cased alpha-numeric string."
         )
 
 
 class APIKeyNotFound(BaseFredAPIError):
-    """Error raised when FRED_API_KEY not found in the environment."""
-
     def __init__(self):
+        """Error raised when FRED_API_KEY not found in the environment."""
         super().__init__(
-            """API key not found. Either set a FRED_API_KEY environment variable or pass your API key to the api_key parameter"""
+            """API key not found. Either set a FRED_API_KEY environment variable or pass your API key to the `api_key` parameter."""
         )
 
 
 class FredAPIRequestError(BaseFredAPIError):
     def __init__(self, message, status_code):
         """Error raised when a request to the FRED API fails."""
         super().__init__(message)
```

### Comparing `pyfredapi-0.6.0/pyfredapi/utils/_convert_to_pandas.py` & `pyfredapi-0.7.0/pyfredapi/utils/_convert_to_pandas.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # ! The minimum date pandas accepts is 1677-09-21
 # ! The maximum date pandas accepts is 2262-04-11
 # ! code snippet for converting to valid date:
 # for c in date_cols:
 #     df.loc[(df[c] < "1677-09-21"), c] = "1677-09-21"
 #     df.loc[(df[c] > "2262-04-11"), c] = "2262-04-11"
 
-FRED_DATE_COLS = ["date"]
+FRED_DATE_COLS = ["date", "created"]
 FRED_NUM_COLS = ["value"]
 
 
 def _convert_to_pandas(data: dict) -> pd.DataFrame:
     """Convert a FRED response dictionary to a pandas dataframe.
 
     Parameters
```

### Comparing `pyfredapi-0.6.0/tests/test_base.py` & `pyfredapi-0.7.0/tests/test_base.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,10 +21,8 @@
     with mock.patch.dict(os.environ, {}, clear=True):
         with pytest.raises(APIKeyNotFound):
             _ = _get_api_key()
 
 
 def test_fredapi_request_err():
     with pytest.raises(FredAPIRequestError):
-        _get_request(
-            endpoint="not-a-real-endpoint",
-        )
+        _get_request(endpoint="not-a-real-endpoint")
```

### Comparing `pyfredapi-0.6.0/tests/test_category.py` & `pyfredapi-0.7.0/tests/test_category.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     get_category_children,
     get_category_related,
     get_category_related_tags,
     get_category_series,
     get_category_tags,
 )
 from pyfredapi.series import SeriesInfo
+from pyfredapi.utils import _convert_to_pandas
 
 from .conftest import get_request as category_request
 
 category_params = {
     "category_id": 125,
 }
 
@@ -85,15 +86,15 @@
 
     if return_type == "json":
         assert isinstance(actual, dict)
         assert "tags" in actual
         assert expected == actual
     elif return_type == "pandas":
         assert isinstance(actual, pd.DataFrame)
-        pd.testing.assert_frame_equal(pd.DataFrame.from_dict(expected["tags"]), actual)
+        pd.testing.assert_frame_equal(_convert_to_pandas(expected["tags"]), actual)
 
 
 @pytest.mark.vcr()
 @pytest.mark.parametrize("return_type", ["json", "pandas"])
 def test_get_category_related_tags(return_type):
     actual = get_category_related_tags(
         category_id=category_params["category_id"],
@@ -108,8 +109,8 @@
 
     if return_type == "json":
         assert isinstance(actual, dict)
         assert "tags" in actual
         assert expected == actual
     elif return_type == "pandas":
         assert isinstance(actual, pd.DataFrame)
-        pd.testing.assert_frame_equal(pd.DataFrame.from_dict(expected["tags"]), actual)
+        pd.testing.assert_frame_equal(_convert_to_pandas(expected["tags"]), actual)
```

### Comparing `pyfredapi-0.6.0/tests/test_maps.py` & `pyfredapi-0.7.0/tests/test_maps.py`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.6.0/tests/test_release.py` & `pyfredapi-0.7.0/tests/test_release.py`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.6.0/tests/test_series.py` & `pyfredapi-0.7.0/tests/test_series.py`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.6.0/tests/test_series_collection.py` & `pyfredapi-0.7.0/tests/test_series_collection.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,39 +8,38 @@
     sc = SeriesCollection()
     assert isinstance(sc, SeriesCollection)
 
 
 @pytest.mark.vcr()
 def test_add_series():
     sc = SeriesCollection()
-    sc.add_series("CPIAUCSL")
+    sc.add("CPIAUCSL")
     assert hasattr(sc, "CPIAUCSL")
     assert isinstance(sc.CPIAUCSL, SeriesData)
-    assert isinstance(sc.data["CPIAUCSL"], SeriesData)
 
 
-def test_drop_series():
-    sc = SeriesCollection()
-    sc.CPIAUCSL = None
-    sc.data = {"CPIAUCSL": None}
+@pytest.mark.vcr()
+def test_remove_series():
+    sc = SeriesCollection(series_id=["CPIAUCSL", "CPILFESL"])
     assert hasattr(sc, "CPIAUCSL")
-    sc.drop_series("CPIAUCSL")
+    assert hasattr(sc, "CPILFESL")
+    sc.remove("CPIAUCSL")
     assert not hasattr(sc, "CPIAUCSL")
+    assert hasattr(sc, "CPILFESL")
 
 
 def test_drop_series_err():
     with pytest.raises(ValueError):
         sc = SeriesCollection()
-        sc.drop_series("foobar")
+        sc.remove("foobar")
 
 
 @pytest.mark.vcr()
 def test_keep_realtime_cols():
-    sc = SeriesCollection()
-    sc.add_series("CPIAUCSL", drop_realtime=False)
+    sc = SeriesCollection(series_id="CPIAUCSL", drop_realtime=False)
     df_cols = set(sc.CPIAUCSL.df.columns.to_list())
     assert set(("date", "CPIAUCSL", "realtime_start", "realtime_end")) == df_cols
 
 
 def parse_cpi_title(title: str) -> str:
     """Parse CPI series title into a readable label."""
     return (
@@ -54,112 +53,95 @@
 
 
 @pytest.mark.vcr()
 @pytest.mark.parametrize(
     "rename", [{"CPIAUCSL": "cpi_all_items"}, parse_cpi_title], ids=["dict", "func"]
 )
 def test_rename_on_add(rename):
-    sc = SeriesCollection()
-    sc.add_series("CPIAUCSL", rename=rename)
+    sc = SeriesCollection(series_id="CPIAUCSL", rename=rename)
     df_cols = set(sc.CPIAUCSL.df.columns.to_list())
     assert set(("date", "cpi_all_items")) == df_cols
 
 
 @pytest.mark.vcr()
 def test_rename_err():
     with pytest.raises(TypeError):
-        sc = SeriesCollection()
-        sc.add_series("CPIAUCSL", rename="foobar")
+        sc = SeriesCollection(rename="foobar")
+        sc.add("CPIAUCSL")
 
 
 @pytest.mark.vcr()
 @pytest.mark.parametrize(
     "rename", [{"CPIAUCSL": "cpi_all_items"}, parse_cpi_title], ids=["dict", "func"]
 )
 def test_rename_after_add(rename):
     sc = SeriesCollection()
-    sc.add_series("CPIAUCSL")
+    sc.add("CPIAUCSL")
     sc.rename_series(rename=rename)
     df_cols = set(sc.CPIAUCSL.df.columns.to_list())
     assert set(("date", "cpi_all_items")) == df_cols
 
 
 @pytest.mark.vcr()
 def test_rename_partial():
     rename = {"CPIAUCSL": "cpi_all_items"}
-    sc = SeriesCollection()
-    sc.add_series(["CPIAUCSL", "CPILFESL"])
+    sc = SeriesCollection(series_id=["CPIAUCSL", "CPILFESL"])
     sc.rename_series(rename=rename)
     assert set(("date", "cpi_all_items")) == set(sc.CPIAUCSL.df.columns.to_list())
     assert set(("date", "CPILFESL")) == set(sc.CPILFESL.df.columns.to_list())
 
 
 @pytest.mark.vcr()
 def test_merge_long():
     series = ["CPIAUCSL", "CPILFESL"]
-    sc = SeriesCollection()
-    sc.add_series(series)
+    sc = SeriesCollection(series_id=series)
     long_df = sc.merge_long()
     assert isinstance(long_df, pd.DataFrame)
     cols = set(long_df.columns.to_list())
     assert set(("date", "value", "series")) == cols
     assert set(series) == set(long_df.series.tolist())
 
 
 @pytest.mark.vcr()
 def test_merge_asof():
     series = ["CPIAUCSL", "CPILFESL"]
-    sc = SeriesCollection()
-    sc.add_series(series)
+    sc = SeriesCollection(series_id=series)
     asof_df = sc.merge_asof(base_series_id="CPIAUCSL")
     assert isinstance(asof_df, pd.DataFrame)
     cols = set(asof_df.columns.to_list())
     assert set(["date"] + series) == cols
     assert set(series) == set([c for c in asof_df.columns.tolist() if c != "date"])
 
 
 @pytest.mark.vcr()
 def test_merge_wide():
     series = ["CPIAUCSL", "CPILFESL"]
-    sc = SeriesCollection()
-    sc.add_series(series)
+    sc = SeriesCollection(series_id=series)
     wide_df = sc.merge_wide()
     assert isinstance(wide_df, pd.DataFrame)
     cols = set(wide_df.columns.to_list())
     assert set(["date"] + series) == cols
     assert set(series) == set([c for c in wide_df.columns.tolist() if c != "date"])
 
 
 @pytest.mark.vcr()
 def test_list_methods_same():
     sc = SeriesCollection()
-    sc.add_series("CPIAUCSL")
+    sc.add("CPIAUCSL")
     sc.list_series()
     sc.list_end_date()
     sc.list_frequency()
     sc.list_seasonality()
     sc.list_start_date()
     sc.list_units()
 
 
 @pytest.mark.vcr()
 def test_list_methods_diff():
     sc = SeriesCollection()
-    sc.add_series(["CPIAUCSL", "WGS10YR"])
+    sc.add(["CPIAUCSL", "WGS10YR"])
     sc.list_series()
     sc.list_end_date()
     sc.list_frequency()
     sc.list_seasonality()
     sc.list_start_date()
     sc.list_units()
-
-
-def test_plot():
-    with pytest.raises(NotImplementedError):
-        sc = SeriesCollection()
-        sc.plot()
-
-
-def test_extract_series():
-    with pytest.raises(NotImplementedError):
-        sc = SeriesCollection()
-        sc.extract_series()
```

### Comparing `pyfredapi-0.6.0/tests/test_sources.py` & `pyfredapi-0.7.0/tests/test_sources.py`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.6.0/tests/test_tags.py` & `pyfredapi-0.7.0/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.6.0/tests/vhs/test_category/test_get_category.yaml` & `pyfredapi-0.7.0/tests/vhs/test_series/test_get_series_categories.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -5,86 +5,174 @@
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python-requests/2.28.1
+      - python-requests/2.28.2
     method: GET
-    uri: https://api.stlouisfed.org/fred/category?category_id=125&file_type=json
+    uri: https://api.stlouisfed.org/fred/series/categories?file_type=json&series_id=GDP
   response:
     body:
       string: !!binary |
-        H4sIAAAAAAAEA6pWSk4sSU3PL8pMLVayiq5WykxRsjI0MtVRykvMTVWyUgopSkxJVXBKzEnMS05V
-        0lEqSCxKzSuJBysDzLg2thYA+F23z0EAAAA=
+        H4sIAAAAAAAEA6pWSk4sSU3PL8pMLVayiq5WykxRsjI0MNNRykvMTVWyUnJ3CYjRd/cLUNJRKkgs
+        Ss0riQerAMyiNrYWAAMe5nI8AAAA
     headers:
       Accept-Ranges:
       - bytes
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Length:
-      - '83'
+      - '78'
       Content-Type:
       - application/json; charset=UTF-8
       Date:
-      - Fri, 21 Oct 2022 14:44:09 GMT
+      - Thu, 27 Apr 2023 14:58:48 GMT
       ETag:
-      - W/"48e42f7425269d17f8a0c22b919840a3-gzip"
+      - W/"2bf4093f7eb3c38e2ac8850d83df83bc-gzip"
       Expires:
-      - Sat, 22 Oct 2022 14:44:09 GMT
+      - Fri, 28 Apr 2023 14:58:48 GMT
       Vary:
       - Accept-Encoding
       x-rate-limit-limit:
       - '120'
       x-rate-limit-remaining:
+      - '75'
+    status:
+      code: 200
+      message: OK
+- request:
+    body: null
+    headers:
+      Accept:
+      - '*/*'
+      Accept-Encoding:
+      - gzip, deflate
+      Connection:
+      - keep-alive
+      User-Agent:
+      - python-requests/2.28.2
+    method: GET
+    uri: https://api.stlouisfed.org/fred/series/categories?file_type=json&series_id=GDP
+  response:
+    body:
+      string: !!binary |
+        H4sIAAAAAAAEA6pWSk4sSU3PL8pMLVayiq5WykxRsjI0MNNRykvMTVWyUnJ3CYjRd/cLUNJRKkgs
+        Ss0riQerAMyiNrYWAAMe5nI8AAAA
+    headers:
+      Accept-Ranges:
+      - bytes
+      Connection:
+      - keep-alive
+      Content-Encoding:
+      - gzip
+      Content-Length:
+      - '78'
+      Content-Type:
+      - application/json; charset=UTF-8
+      Date:
+      - Thu, 27 Apr 2023 14:58:49 GMT
+      ETag:
+      - W/"2bf4093f7eb3c38e2ac8850d83df83bc-gzip"
+      Expires:
+      - Fri, 28 Apr 2023 14:58:49 GMT
+      Vary:
+      - Accept-Encoding
+      x-rate-limit-limit:
       - '120'
+      x-rate-limit-remaining:
+      - '73'
+    status:
+      code: 200
+      message: OK
+- request:
+    body: null
+    headers:
+      Accept:
+      - '*/*'
+      Accept-Encoding:
+      - gzip, deflate
+      Connection:
+      - keep-alive
+      User-Agent:
+      - python-requests/2.28.2
+    method: GET
+    uri: https://api.stlouisfed.org/fred/series/categories?file_type=json&series_id=GDP
+  response:
+    body:
+      string: !!binary |
+        H4sIAAAAAAAEA6pWSk4sSU3PL8pMLVayiq5WykxRsjI0MNNRykvMTVWyUnJ3CYjRd/cLUNJRKkgs
+        Ss0riQerAMyiNrYWAAMe5nI8AAAA
+    headers:
+      Accept-Ranges:
+      - bytes
+      Connection:
+      - keep-alive
+      Content-Encoding:
+      - gzip
+      Content-Length:
+      - '78'
+      Content-Type:
+      - application/json; charset=UTF-8
+      Date:
+      - Fri, 28 Apr 2023 01:29:14 GMT
+      ETag:
+      - W/"2bf4093f7eb3c38e2ac8850d83df83bc-gzip"
+      Expires:
+      - Sat, 29 Apr 2023 01:29:14 GMT
+      Vary:
+      - Accept-Encoding
+      x-rate-limit-limit:
+      - '120'
+      x-rate-limit-remaining:
+      - '93'
     status:
       code: 200
       message: OK
 - request:
     body: null
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python-requests/2.28.1
+      - python-requests/2.28.2
     method: GET
-    uri: https://api.stlouisfed.org/fred/category?category_id=125&file_type=json
+    uri: https://api.stlouisfed.org/fred/series/categories?file_type=json&series_id=GDP
   response:
     body:
       string: !!binary |
-        H4sIAAAAAAAEA6pWSk4sSU3PL8pMLVayiq5WykxRsjI0MtVRykvMTVWyUgopSkxJVXBKzEnMS05V
-        0lEqSCxKzSuJBysDzLg2thYA+F23z0EAAAA=
+        H4sIAAAAAAAEA6pWSk4sSU3PL8pMLVayiq5WykxRsjI0MNNRykvMTVWyUnJ3CYjRd/cLUNJRKkgs
+        Ss0riQerAMyiNrYWAAMe5nI8AAAA
     headers:
       Accept-Ranges:
       - bytes
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Length:
-      - '83'
+      - '78'
       Content-Type:
       - application/json; charset=UTF-8
       Date:
-      - Fri, 21 Oct 2022 14:44:10 GMT
+      - Fri, 28 Apr 2023 01:29:15 GMT
       ETag:
-      - W/"48e42f7425269d17f8a0c22b919840a3-gzip"
+      - W/"2bf4093f7eb3c38e2ac8850d83df83bc-gzip"
       Expires:
-      - Sat, 22 Oct 2022 14:44:10 GMT
+      - Sat, 29 Apr 2023 01:29:15 GMT
       Vary:
       - Accept-Encoding
       x-rate-limit-limit:
       - '120'
       x-rate-limit-remaining:
-      - '119'
+      - '91'
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `pyfredapi-0.6.0/tests/vhs/test_category/test_get_category_children.yaml` & `pyfredapi-0.7.0/tests/vhs/test_category/test_get_category_related.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -5,17 +5,17 @@
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python-requests/2.28.1
+      - python-requests/2.28.2
     method: GET
-    uri: https://api.stlouisfed.org/fred/category/children?category_id=125&file_type=json
+    uri: https://api.stlouisfed.org/fred/category/related?category_id=125&file_type=json
   response:
     body:
       string: !!binary |
         H4sIAAAAAAAEA6tWSk4sSU3PL8pMLVayio6tBQDFInZ5EQAAAA==
     headers:
       Accept-Ranges:
       - bytes
@@ -24,41 +24,41 @@
       Content-Encoding:
       - gzip
       Content-Length:
       - '37'
       Content-Type:
       - application/json; charset=UTF-8
       Date:
-      - Fri, 21 Oct 2022 14:44:10 GMT
+      - Thu, 27 Apr 2023 14:58:22 GMT
       ETag:
-      - W/"487d2beefe344a5cb73afd2f7a8dc8a2-gzip"
+      - W/"73f19c6fbc6ebeb7065dc4e99bdbc326-gzip"
       Expires:
-      - Sat, 22 Oct 2022 14:44:10 GMT
+      - Fri, 28 Apr 2023 14:58:22 GMT
       Vary:
       - Accept-Encoding
       x-rate-limit-limit:
       - '120'
       x-rate-limit-remaining:
-      - '118'
+      - '114'
     status:
       code: 200
       message: OK
 - request:
     body: null
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python-requests/2.28.1
+      - python-requests/2.28.2
     method: GET
-    uri: https://api.stlouisfed.org/fred/category/children?category_id=125&file_type=json
+    uri: https://api.stlouisfed.org/fred/category/related?category_id=125&file_type=json
   response:
     body:
       string: !!binary |
         H4sIAAAAAAAEA6tWSk4sSU3PL8pMLVayio6tBQDFInZ5EQAAAA==
     headers:
       Accept-Ranges:
       - bytes
@@ -67,22 +67,108 @@
       Content-Encoding:
       - gzip
       Content-Length:
       - '37'
       Content-Type:
       - application/json; charset=UTF-8
       Date:
-      - Fri, 21 Oct 2022 14:44:11 GMT
+      - Thu, 27 Apr 2023 14:58:22 GMT
       ETag:
-      - W/"487d2beefe344a5cb73afd2f7a8dc8a2-gzip"
+      - W/"73f19c6fbc6ebeb7065dc4e99bdbc326-gzip"
       Expires:
-      - Sat, 22 Oct 2022 14:44:11 GMT
+      - Fri, 28 Apr 2023 14:58:22 GMT
       Vary:
       - Accept-Encoding
       x-rate-limit-limit:
       - '120'
       x-rate-limit-remaining:
-      - '116'
+      - '112'
+    status:
+      code: 200
+      message: OK
+- request:
+    body: null
+    headers:
+      Accept:
+      - '*/*'
+      Accept-Encoding:
+      - gzip, deflate
+      Connection:
+      - keep-alive
+      User-Agent:
+      - python-requests/2.28.2
+    method: GET
+    uri: https://api.stlouisfed.org/fred/category/related?category_id=125&file_type=json
+  response:
+    body:
+      string: !!binary |
+        H4sIAAAAAAAEA6tWSk4sSU3PL8pMLVayio6tBQDFInZ5EQAAAA==
+    headers:
+      Accept-Ranges:
+      - bytes
+      Connection:
+      - keep-alive
+      Content-Encoding:
+      - gzip
+      Content-Length:
+      - '37'
+      Content-Type:
+      - application/json; charset=UTF-8
+      Date:
+      - Fri, 28 Apr 2023 01:28:51 GMT
+      ETag:
+      - W/"73f19c6fbc6ebeb7065dc4e99bdbc326-gzip"
+      Expires:
+      - Sat, 29 Apr 2023 01:28:51 GMT
+      Vary:
+      - Accept-Encoding
+      x-rate-limit-limit:
+      - '120'
+      x-rate-limit-remaining:
+      - '114'
+    status:
+      code: 200
+      message: OK
+- request:
+    body: null
+    headers:
+      Accept:
+      - '*/*'
+      Accept-Encoding:
+      - gzip, deflate
+      Connection:
+      - keep-alive
+      User-Agent:
+      - python-requests/2.28.2
+    method: GET
+    uri: https://api.stlouisfed.org/fred/category/related?category_id=125&file_type=json
+  response:
+    body:
+      string: !!binary |
+        H4sIAAAAAAAEA6tWSk4sSU3PL8pMLVayio6tBQDFInZ5EQAAAA==
+    headers:
+      Accept-Ranges:
+      - bytes
+      Connection:
+      - keep-alive
+      Content-Encoding:
+      - gzip
+      Content-Length:
+      - '37'
+      Content-Type:
+      - application/json; charset=UTF-8
+      Date:
+      - Fri, 28 Apr 2023 01:28:51 GMT
+      ETag:
+      - W/"73f19c6fbc6ebeb7065dc4e99bdbc326-gzip"
+      Expires:
+      - Sat, 29 Apr 2023 01:28:51 GMT
+      Vary:
+      - Accept-Encoding
+      x-rate-limit-limit:
+      - '120'
+      x-rate-limit-remaining:
+      - '112'
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `pyfredapi-0.6.0/tests/vhs/test_category/test_get_category_related.yaml` & `pyfredapi-0.7.0/tests/vhs/test_category/test_get_category.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -5,84 +5,174 @@
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python-requests/2.28.1
+      - python-requests/2.28.2
     method: GET
-    uri: https://api.stlouisfed.org/fred/category/related?category_id=125&file_type=json
+    uri: https://api.stlouisfed.org/fred/category?category_id=125&file_type=json
   response:
     body:
       string: !!binary |
-        H4sIAAAAAAAEA6tWSk4sSU3PL8pMLVayio6tBQDFInZ5EQAAAA==
+        H4sIAAAAAAAEA6pWSk4sSU3PL8pMLVayiq5WykxRsjI0MtVRykvMTVWyUgopSkxJVXBKzEnMS05V
+        0lEqSCxKzSuJBysDzLg2thYA+F23z0EAAAA=
     headers:
       Accept-Ranges:
       - bytes
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Length:
-      - '37'
+      - '83'
       Content-Type:
       - application/json; charset=UTF-8
       Date:
-      - Fri, 21 Oct 2022 14:44:11 GMT
+      - Thu, 27 Apr 2023 14:58:19 GMT
       ETag:
-      - W/"15aa78a4e02c437d1e91beed156f55fc-gzip"
+      - W/"11c3a5982195af3895aca973f7e42ddc-gzip"
       Expires:
-      - Sat, 22 Oct 2022 14:44:11 GMT
+      - Fri, 28 Apr 2023 14:58:19 GMT
       Vary:
       - Accept-Encoding
       x-rate-limit-limit:
       - '120'
       x-rate-limit-remaining:
-      - '114'
+      - '120'
+    status:
+      code: 200
+      message: OK
+- request:
+    body: null
+    headers:
+      Accept:
+      - '*/*'
+      Accept-Encoding:
+      - gzip, deflate
+      Connection:
+      - keep-alive
+      User-Agent:
+      - python-requests/2.28.2
+    method: GET
+    uri: https://api.stlouisfed.org/fred/category?category_id=125&file_type=json
+  response:
+    body:
+      string: !!binary |
+        H4sIAAAAAAAEA6pWSk4sSU3PL8pMLVayiq5WykxRsjI0MtVRykvMTVWyUgopSkxJVXBKzEnMS05V
+        0lEqSCxKzSuJBysDzLg2thYA+F23z0EAAAA=
+    headers:
+      Accept-Ranges:
+      - bytes
+      Connection:
+      - keep-alive
+      Content-Encoding:
+      - gzip
+      Content-Length:
+      - '83'
+      Content-Type:
+      - application/json; charset=UTF-8
+      Date:
+      - Thu, 27 Apr 2023 14:58:19 GMT
+      ETag:
+      - W/"11c3a5982195af3895aca973f7e42ddc-gzip"
+      Expires:
+      - Fri, 28 Apr 2023 14:58:19 GMT
+      Vary:
+      - Accept-Encoding
+      x-rate-limit-limit:
+      - '120'
+      x-rate-limit-remaining:
+      - '119'
+    status:
+      code: 200
+      message: OK
+- request:
+    body: null
+    headers:
+      Accept:
+      - '*/*'
+      Accept-Encoding:
+      - gzip, deflate
+      Connection:
+      - keep-alive
+      User-Agent:
+      - python-requests/2.28.2
+    method: GET
+    uri: https://api.stlouisfed.org/fred/category?category_id=125&file_type=json
+  response:
+    body:
+      string: !!binary |
+        H4sIAAAAAAAEA6pWSk4sSU3PL8pMLVayiq5WykxRsjI0MtVRykvMTVWyUgopSkxJVXBKzEnMS05V
+        0lEqSCxKzSuJBysDzLg2thYA+F23z0EAAAA=
+    headers:
+      Accept-Ranges:
+      - bytes
+      Connection:
+      - keep-alive
+      Content-Encoding:
+      - gzip
+      Content-Length:
+      - '83'
+      Content-Type:
+      - application/json; charset=UTF-8
+      Date:
+      - Fri, 28 Apr 2023 01:28:49 GMT
+      ETag:
+      - W/"11c3a5982195af3895aca973f7e42ddc-gzip"
+      Expires:
+      - Sat, 29 Apr 2023 01:28:49 GMT
+      Vary:
+      - Accept-Encoding
+      x-rate-limit-limit:
+      - '120'
+      x-rate-limit-remaining:
+      - '120'
     status:
       code: 200
       message: OK
 - request:
     body: null
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python-requests/2.28.1
+      - python-requests/2.28.2
     method: GET
-    uri: https://api.stlouisfed.org/fred/category/related?category_id=125&file_type=json
+    uri: https://api.stlouisfed.org/fred/category?category_id=125&file_type=json
   response:
     body:
       string: !!binary |
-        H4sIAAAAAAAEA6tWSk4sSU3PL8pMLVayio6tBQDFInZ5EQAAAA==
+        H4sIAAAAAAAEA6pWSk4sSU3PL8pMLVayiq5WykxRsjI0MtVRykvMTVWyUgopSkxJVXBKzEnMS05V
+        0lEqSCxKzSuJBysDzLg2thYA+F23z0EAAAA=
     headers:
       Accept-Ranges:
       - bytes
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Length:
-      - '37'
+      - '83'
       Content-Type:
       - application/json; charset=UTF-8
       Date:
-      - Fri, 21 Oct 2022 14:44:12 GMT
+      - Fri, 28 Apr 2023 01:28:49 GMT
       ETag:
-      - W/"15aa78a4e02c437d1e91beed156f55fc-gzip"
+      - W/"11c3a5982195af3895aca973f7e42ddc-gzip"
       Expires:
-      - Sat, 22 Oct 2022 14:44:12 GMT
+      - Sat, 29 Apr 2023 01:28:49 GMT
       Vary:
       - Accept-Encoding
       x-rate-limit-limit:
       - '120'
       x-rate-limit-remaining:
-      - '112'
+      - '119'
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `pyfredapi-0.6.0/tests/vhs/test_category/test_get_category_related_tags[json].yaml` & `pyfredapi-0.7.0/tests/vhs/test_category/test_get_category_tags[pandas].yaml`

 * *Files 26% similar despite different names*

```diff
@@ -5,112 +5,114 @@
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python-requests/2.28.1
+      - python-requests/2.28.2
     method: GET
-    uri: https://api.stlouisfed.org/fred/category/related_tags?category_id=125&file_type=json&tag_names=balance
+    uri: https://api.stlouisfed.org/fred/category/tags?category_id=125&file_type=json
   response:
     body:
       string: !!binary |
-        H4sIAAAAAAAEA6pWKkpNzCnJzE2NLy5JLCpRslIyMjAy0jU00DUyVNJByKbmpaDL5RelpBbFJ1Uq
-        WSkVpxZlphbHJ+eX5pUo6SgV5xeVxIOllayUUlKLk5V0lCByVkbGOkr5aWnFqSVKVgY6SjmZuZkl
+        H4sIAAAAAAAEA6pWKkpNzCnJzE2NLy5JLCpRslIyMjAy1jUw0TUyV9JByKbmpaDL5RelpBbFJ1Uq
+        WSkVpxZlphbHJ+eX5pUo6SgV5xeVxIOllayUUlKLk5V0lCByVkZmOkr5aWnFqSVKVgY6SjmZuZkl
         SlaGBgYGOkolienFSlbR1Up5ibmpSlZKeYklmfl5SjpK6UX5pQXxmSAXpKfmg2zIyy9JLVayUgIZ
-        XJSaWJIKkjMyMDTSNTDSNTJXMDSwMrSwMrTUNTBT0lEqyC8ozUksyiypVLKytNRBda6VsUmtDtzO
+        XJSaWJIKkjMyMDTSNTDSNTJXMDSwMrSwMrTUNTBT0lEqyC8ozUksyiypVLKytNRBda6ViUmtDtzO
         gtKknMxkhZT83MTMPCuF5MwSsCMUilILS1OLQfagOCcZ5DWoY/JKc3J0lJKRnWOha2ika2iuYGRs
         ZWxsZWhMsnNKixMx/K+kowS1USk0L7MkNUUhuCSxJLVYIT9NwTE3tSgzGaQHxR2Eg8UQFAEo0Yga
-        LkmpIEORIqK4CMnrSk6lRamJpSAXuCbn5+XnZiYrOOYl5lQWZxaTHkXmFhhRZIQURXnoYVKcmgiy
-        BRYofvklCsGpicX5eYk5OZUKjilZpdCIozxMjJDTSmFpYlFJalFOJWoUpRWlFiLFEen+tzBB97+h
-        BZL/E/PyShNzqG0nRpgbIod5SmZxcn5eSWZeaWoKqs3pqaAcCgt70j1rZobhWWSLi1OLyjKTU0Hx
-        i5T4KLYUv28z85Lzc1Op7E+McsfQAClSCaRpqqRnC0xfIzshKb8An5edEnMS85JTQXk8ILEyNzWv
-        BBQpKFnKWNfAUNfIQsHQxApUAGMp7kzM0WPbDCkQ0vPzU0CGUjGmzQ3wWVicmpyfl5JYhJaDKU1e
-        xhgBjezLkqLEFConLlNTfL5MTs0rLkULV9Ti2xmmAiU6Cdca5hiJGrl8TC4tKkrNK1FITIZU/ig1
-        J6VhbGKI7mVkq3Pz80oyqF4wW2IEM7KdyYkFmSWJObTxLqjdhFo9I5eSmXllqcUloDyJLweTXjhj
-        pitkW3NTi5IzEvNSMotJSs7GuoaGuobGCoZmVgYWVsaGmI0iI4xSAtnaAkTpQ8WCwhgjKaPYWZSZ
-        S/ViwhSjbALMqDa2FgC66DHakwsAAA==
+        LkmpIEORIqK4CMnrSk6lRamJpSAXuCbn5+XnZiYrOOYl5lQWZxaTHkXm5hhRZIQURUmJOYl5yano
+        4QJKKLBwId1OUwN0O43NkOzMQ4+H4tREkM9gFvrllygEpyYW5+cl5uRUKjimZJVCEwuJ8YCZPI0s
+        kNxRWJpYVJJalFOJ6vu0otRCpGRBuvctTNC9b4ScK1Iyi5Pz80oy80pTU1BtTk+lLNzNMC02QPIv
+        gWCnSpBbYJQIhshRn5iXV5qYg+prysPbFD28DZHDOym/ANVC1GB2guQAUHYLSKzMTc0rAaVFlJRm
+        rGtgqGtkoWBoYgUqC7GUPCbGGE5AzmWZecn5uVTOZGZmeK0sTi0qy0xOBfkFqaBB9TrpSdsMozQx
+        RPZnXiqoPqGifaYYyQk5A5cUJaZQOVRNMSIS2cLkxILMksQchcRkSA2MUn1RGraGGGGLnHOSU/OK
+        S9FiE7XacIapQEm7hGsrcwv0hIRsb3p+fgqatZR61Ayvhbn5eSUZVC+TLTGKRmRPFqcm5+elJBah
+        1QSUetQYo2BCtjS5tKgoNa+ENonJGKN0QC4SC4oyc6nuWxOM9ItsZUlRYl5xWmoRldOSEUZaQrY0
+        M68stbgEVKbjqwFILwYxSwnkUjA3tSg5IzEvJbOYpMLJWNfQUNfQWMHQzMrAwsrYELN9a2SEnlOR
+        rS1A1F5ULIGNMQIYMKPa2FoAH/Z0DOsMAAA=
     headers:
       Accept-Ranges:
       - bytes
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Length:
-      - '820'
+      - '881'
       Content-Type:
       - application/json; charset=UTF-8
       Date:
-      - Fri, 21 Oct 2022 14:44:16 GMT
+      - Thu, 27 Apr 2023 14:58:27 GMT
       ETag:
-      - W/"2f74c8636f7555be1f398932a625b6ff-gzip-gzip"
+      - W/"1434349e173e654f7ba0bc90e775198c-gzip-gzip"
       Expires:
-      - Sat, 22 Oct 2022 14:44:16 GMT
+      - Fri, 28 Apr 2023 14:58:27 GMT
       Vary:
       - Accept-Encoding
       x-rate-limit-limit:
       - '120'
       x-rate-limit-remaining:
-      - '102'
+      - '104'
     status:
       code: 200
       message: OK
 - request:
     body: null
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python-requests/2.28.1
+      - python-requests/2.28.2
     method: GET
-    uri: https://api.stlouisfed.org/fred/category/related_tags?category_id=125&file_type=json&tag_names=balance
+    uri: https://api.stlouisfed.org/fred/category/tags?category_id=125&file_type=json
   response:
     body:
       string: !!binary |
-        H4sIAAAAAAAEA6pWKkpNzCnJzE2NLy5JLCpRslIyMjAy0jU00DUyVNJByKbmpaDL5RelpBbFJ1Uq
-        WSkVpxZlphbHJ+eX5pUo6SgV5xeVxIOllayUUlKLk5V0lCByVkbGOkr5aWnFqSVKVgY6SjmZuZkl
+        H4sIAAAAAAAEA6pWKkpNzCnJzE2NLy5JLCpRslIyMjAy1jUw0TUyV9JByKbmpaDL5RelpBbFJ1Uq
+        WSkVpxZlphbHJ+eX5pUo6SgV5xeVxIOllayUUlKLk5V0lCByVkZmOkr5aWnFqSVKVgY6SjmZuZkl
         SlaGBgYGOkolienFSlbR1Up5ibmpSlZKeYklmfl5SjpK6UX5pQXxmSAXpKfmg2zIyy9JLVayUgIZ
-        XJSaWJIKkjMyMDTSNTDSNTJXMDSwMrSwMrTUNTBT0lEqyC8ozUksyiypVLKytNRBda6VsUmtDtzO
+        XJSaWJIKkjMyMDTSNTDSNTJXMDSwMrSwMrTUNTBT0lEqyC8ozUksyiypVLKytNRBda6ViUmtDtzO
         gtKknMxkhZT83MTMPCuF5MwSsCMUilILS1OLQfagOCcZ5DWoY/JKc3J0lJKRnWOha2ika2iuYGRs
         ZWxsZWhMsnNKixMx/K+kowS1USk0L7MkNUUhuCSxJLVYIT9NwTE3tSgzGaQHxR2Eg8UQFAEo0Yga
-        LkmpIEORIqK4CMnrSk6lRamJpSAXuCbn5+XnZiYrOOYl5lQWZxaTHkXmFhhRZIQURXnoYVKcmgiy
-        BRYofvklCsGpicX5eYk5OZUKjilZpdCIozxMjJDTSmFpYlFJalFOJWoUpRWlFiLFEen+tzBB97+h
-        BZL/E/PyShNzqG0nRpgbIod5SmZxcn5eSWZeaWoKqs3pqaAcCgt70j1rZobhWWSLi1OLyjKTU0Hx
-        i5T4KLYUv28z85Lzc1Op7E+McsfQAClSCaRpqqRnC0xfIzshKb8An5edEnMS85JTQXk8ILEyNzWv
-        BBQpKFnKWNfAUNfIQsHQxApUAGMp7kzM0WPbDCkQ0vPzU0CGUjGmzQ3wWVicmpyfl5JYhJaDKU1e
-        xhgBjezLkqLEFConLlNTfL5MTs0rLkULV9Ti2xmmAiU6Cdca5hiJGrl8TC4tKkrNK1FITIZU/ig1
-        J6VhbGKI7mVkq3Pz80oyqF4wW2IEM7KdyYkFmSWJObTxLqjdhFo9I5eSmXllqcUloDyJLweTXjhj
-        pitkW3NTi5IzEvNSMotJSs7GuoaGuobGCoZmVgYWVsaGmI0iI4xSAtnaAkTpQ8WCwhgjKaPYWZSZ
-        S/ViwhSjbALMqDa2FgC66DHakwsAAA==
+        LkmpIEORIqK4CMnrSk6lRamJpSAXuCbn5+XnZiYrOOYl5lQWZxaTHkXm5hhRZIQURUmJOYl5yano
+        4QJKKLBwId1OUwN0O43NkOzMQ4+H4tREkM9gFvrllygEpyYW5+cl5uRUKjimZJVCEwuJ8YCZPI0s
+        kNxRWJpYVJJalFOJ6vu0otRCpGRBuvctTNC9b4ScK1Iyi5Pz80oy80pTU1BtTk+lLNzNMC02QPIv
+        gWCnSpBbYJQIhshRn5iXV5qYg+prysPbFD28DZHDOym/ANVC1GB2guQAUHYLSKzMTc0rAaVFlJRm
+        rGtgqGtkoWBoYgUqC7GUPCbGGE5AzmWZecn5uVTOZGZmeK0sTi0qy0xOBfkFqaBB9TrpSdsMozQx
+        RPZnXiqoPqGifaYYyQk5A5cUJaZQOVRNMSIS2cLkxILMksQchcRkSA2MUn1RGraGGGGLnHOSU/OK
+        S9FiE7XacIapQEm7hGsrcwv0hIRsb3p+fgqatZR61Ayvhbn5eSUZVC+TLTGKRmRPFqcm5+elJBah
+        1QSUetQYo2BCtjS5tKgoNa+ENonJGKN0QC4SC4oyc6nuWxOM9ItsZUlRYl5xWmoRldOSEUZaQrY0
+        M68stbgEVKbjqwFILwYxSwnkUjA3tSg5IzEvJbOYpMLJWNfQUNfQWMHQzMrAwsrYELN9a2SEnlOR
+        rS1A1F5ULIGNMQIYMKPa2FoAH/Z0DOsMAAA=
     headers:
       Accept-Ranges:
       - bytes
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Length:
-      - '820'
+      - '881'
       Content-Type:
       - application/json; charset=UTF-8
       Date:
-      - Fri, 21 Oct 2022 14:44:16 GMT
+      - Fri, 28 Apr 2023 01:28:55 GMT
       ETag:
-      - W/"2f74c8636f7555be1f398932a625b6ff-gzip-gzip"
+      - W/"1434349e173e654f7ba0bc90e775198c-gzip-gzip"
       Expires:
-      - Sat, 22 Oct 2022 14:44:16 GMT
+      - Sat, 29 Apr 2023 01:28:55 GMT
       Vary:
       - Accept-Encoding
       x-rate-limit-limit:
       - '120'
       x-rate-limit-remaining:
-      - '101'
+      - '104'
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `pyfredapi-0.6.0/tests/vhs/test_category/test_get_category_tags[json].yaml` & `pyfredapi-0.7.0/tests/vhs/test_release/test_get_release_related_tags.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -5,112 +5,178 @@
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python-requests/2.28.1
+      - python-requests/2.28.2
     method: GET
-    uri: https://api.stlouisfed.org/fred/category/tags?category_id=125&file_type=json
+    uri: https://api.stlouisfed.org/fred/release/related_tags?file_type=json&release_id=10&tag_names=sa%3Bforeign
   response:
     body:
       string: !!binary |
-        H4sIAAAAAAAEA6pWKkpNzCnJzE2NLy5JLCpRslIyMjAy0jU00DUyVNJByKbmpaDL5RelpBbFJ1Uq
-        WSkVpxZlphbHJ+eX5pUo6SgV5xeVxIOllayUUlKLk5V0lCByVkYmOkr5aWnFqSVKVgY6SjmZuZkl
-        SlaGBgYGOkolienFSlbR1Up5ibmpSlZKSamJSjpK6UX5pQXxmSDri4tAJuXll6QWK1kpOZUWpSaW
-        KuSnKbgm5+fl52YmKzjmJeZUFmcWg+wrSk0sSQXpMjIwNNI1MNI1MlcwNLAytLAytNQ1MFPSUSrI
-        LyjNSSzKLKlUsjK30EH1hZWpUa0O3Cl5iSWZ+XmorklPzQd5FuYc0u20tMRrZ0FpUk5mskJKfm5i
-        Zp6VQnJmCdgRCkWphaWpxSC/oQROMlLY5JXm5OgoJSMHgYWuoZGuobmCkbGVsbGVoTFmEBBwTmkx
-        Wmykp+Yr6SjBvB+al1mSmqIQXJJYkloMihTH3NSizGSQHhR3EI4KQ1BaQElRqHGRlJiTmJecih4Z
-        oNiBOYb0uDDBiH8TC6T4LyxNLCpJLcqpRLU1rSi1ECkMSLfWwgQ9CRijJDv0MC9OTQQlbpg//fJL
-        FIJTE4vz8xJzcioVHFOySqEJg/IwNzZA8j8Bd1DFDRYYUWCEHBYpmcXJ+XklmXmlqSmosZCeSlnc
-        m5mhR4IRit9Ti8oyk1NB4Y5UFlFsKaZvkS1NzMsrTcxB9SflqQ3DTkPkRJ6en59CZV+aG6AHraEZ
-        UrJKyi9A9SJqqDpBcjqoNAlIrMxNzSsBOQ8laRvrGhjqGlkoGJpYgQp3LMWaiTmGE0yQnJCZl5yf
-        S+XCxAyjYEcO5uTEgsySxByFxGRInYhSiqMGAOkFipExum+Rwzu5tKgoNa+ENlabGOKzujg1OT8v
-        JbEIrQSl1L/GGEka2b8lRYkpVI5bU1N8vsxNLUrOSMxLySwmyVpjXUNDXUNjBUMzKwMLK2NDzMrZ
-        CCMVIyfivFRQS4SapRNGvkW2Ljk1r7gUlBWRbERtmznDVKBkVsJ1vzlGzkGuAnLz80oyqF4HW2LE
-        KLKdBUWZuVRPtaYYwYtsZUlRYl5xWmoRWghTnFWM0FMuYEa1sbUAcg9Y6AIMAAA=
+        H4sIAAAAAAAEA6pWKkpNzCnJzE2NLy5JLCpRslIyMjAy1jUw0TUyV9JByKbmpaDL5RelpBbFJ1Uq
+        WSkVpxZlphbHJ+eX5pUo6SgV5xeVxIOllayUUlKLk5V0lCByVgY6SvlpacWpJUogJmA5mbmZJUpW
+        hgYGBjpKJYnpxUpW0bG1ADvPSoCVAAAA
     headers:
       Accept-Ranges:
       - bytes
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Length:
-      - '845'
+      - '138'
       Content-Type:
       - application/json; charset=UTF-8
       Date:
-      - Fri, 21 Oct 2022 14:44:13 GMT
+      - Thu, 27 Apr 2023 14:58:44 GMT
       ETag:
-      - W/"c21027dd6c9bfd3018524a28a083b372-gzip-gzip"
+      - W/"b7b91a6326279f8fa135842f24cc2308-gzip-gzip"
       Expires:
-      - Sat, 22 Oct 2022 14:44:13 GMT
+      - Fri, 28 Apr 2023 14:58:44 GMT
       Vary:
       - Accept-Encoding
       x-rate-limit-limit:
       - '120'
       x-rate-limit-remaining:
-      - '106'
+      - '80'
     status:
       code: 200
       message: OK
 - request:
     body: null
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python-requests/2.28.1
+      - python-requests/2.28.2
     method: GET
-    uri: https://api.stlouisfed.org/fred/category/tags?category_id=125&file_type=json
+    uri: https://api.stlouisfed.org/fred/release/related_tags?file_type=json&release_id=10&tag_names=sa%3Bforeign
   response:
     body:
       string: !!binary |
-        H4sIAAAAAAAEA6pWKkpNzCnJzE2NLy5JLCpRslIyMjAy0jU00DUyVNJByKbmpaDL5RelpBbFJ1Uq
-        WSkVpxZlphbHJ+eX5pUo6SgV5xeVxIOllayUUlKLk5V0lCByVkYmOkr5aWnFqSVKVgY6SjmZuZkl
-        SlaGBgYGOkolienFSlbR1Up5ibmpSlZKSamJSjpK6UX5pQXxmSDri4tAJuXll6QWK1kpOZUWpSaW
-        KuSnKbgm5+fl52YmKzjmJeZUFmcWg+wrSk0sSQXpMjIwNNI1MNI1MlcwNLAytLAytNQ1MFPSUSrI
-        LyjNSSzKLKlUsjK30EH1hZWpUa0O3Cl5iSWZ+XmorklPzQd5FuYc0u20tMRrZ0FpUk5mskJKfm5i
-        Zp6VQnJmCdgRCkWphaWpxSC/oQROMlLY5JXm5OgoJSMHgYWuoZGuobmCkbGVsbGVoTFmEBBwTmkx
-        Wmykp+Yr6SjBvB+al1mSmqIQXJJYkloMihTH3NSizGSQHhR3EI4KQ1BaQElRqHGRlJiTmJecih4Z
-        oNiBOYb0uDDBiH8TC6T4LyxNLCpJLcqpRLU1rSi1ECkMSLfWwgQ9CRijJDv0MC9OTQQlbpg//fJL
-        FIJTE4vz8xJzcioVHFOySqEJg/IwNzZA8j8Bd1DFDRYYUWCEHBYpmcXJ+XklmXmlqSmosZCeSlnc
-        m5mhR4IRit9Ti8oyk1NB4Y5UFlFsKaZvkS1NzMsrTcxB9SflqQ3DTkPkRJ6en59CZV+aG6AHraEZ
-        UrJKyi9A9SJqqDpBcjqoNAlIrMxNzSsBOQ8laRvrGhjqGlkoGJpYgQp3LMWaiTmGE0yQnJCZl5yf
-        S+XCxAyjYEcO5uTEgsySxByFxGRInYhSiqMGAOkFipExum+Rwzu5tKgoNa+ENlabGOKzujg1OT8v
-        JbEIrQSl1L/GGEka2b8lRYkpVI5bU1N8vsxNLUrOSMxLySwmyVpjXUNDXUNjBUMzKwMLK2NDzMrZ
-        CCMVIyfivFRQS4SapRNGvkW2Ljk1r7gUlBWRbERtmznDVKBkVsJ1vzlGzkGuAnLz80oyqF4HW2LE
-        KLKdBUWZuVRPtaYYwYtsZUlRYl5xWmoRWghTnFWM0FMuYEa1sbUAcg9Y6AIMAAA=
+        H4sIAAAAAAAEA6pWKkpNzCnJzE2NLy5JLCpRslIyMjAy1jUw0TUyV9JByKbmpaDL5RelpBbFJ1Uq
+        WSkVpxZlphbHJ+eX5pUo6SgV5xeVxIOllayUUlKLk5V0lCByVgY6SvlpacWpJUogJmA5mbmZJUpW
+        hgYGBjpKJYnpxUpW0bG1ADvPSoCVAAAA
     headers:
       Accept-Ranges:
       - bytes
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Length:
-      - '845'
+      - '138'
       Content-Type:
       - application/json; charset=UTF-8
       Date:
-      - Fri, 21 Oct 2022 14:44:14 GMT
+      - Thu, 27 Apr 2023 14:58:45 GMT
       ETag:
-      - W/"c21027dd6c9bfd3018524a28a083b372-gzip-gzip"
+      - W/"b7b91a6326279f8fa135842f24cc2308-gzip-gzip"
       Expires:
-      - Sat, 22 Oct 2022 14:44:14 GMT
+      - Fri, 28 Apr 2023 14:58:45 GMT
       Vary:
       - Accept-Encoding
       x-rate-limit-limit:
       - '120'
       x-rate-limit-remaining:
-      - '105'
+      - '79'
+    status:
+      code: 200
+      message: OK
+- request:
+    body: null
+    headers:
+      Accept:
+      - '*/*'
+      Accept-Encoding:
+      - gzip, deflate
+      Connection:
+      - keep-alive
+      User-Agent:
+      - python-requests/2.28.2
+    method: GET
+    uri: https://api.stlouisfed.org/fred/release/related_tags?file_type=json&release_id=10&tag_names=sa%3Bforeign
+  response:
+    body:
+      string: !!binary |
+        H4sIAAAAAAAEA6pWKkpNzCnJzE2NLy5JLCpRslIyMjAy1jUw0TUyV9JByKbmpaDL5RelpBbFJ1Uq
+        WSkVpxZlphbHJ+eX5pUo6SgV5xeVxIOllayUUlKLk5V0lCByVgY6SvlpacWpJUogJmA5mbmZJUpW
+        hgYGBjpKJYnpxUpW0bG1ADvPSoCVAAAA
+    headers:
+      Accept-Ranges:
+      - bytes
+      Connection:
+      - keep-alive
+      Content-Encoding:
+      - gzip
+      Content-Length:
+      - '138'
+      Content-Type:
+      - application/json; charset=UTF-8
+      Date:
+      - Fri, 28 Apr 2023 01:29:11 GMT
+      ETag:
+      - W/"b7b91a6326279f8fa135842f24cc2308-gzip-gzip"
+      Expires:
+      - Sat, 29 Apr 2023 01:29:11 GMT
+      Vary:
+      - Accept-Encoding
+      x-rate-limit-limit:
+      - '120'
+      x-rate-limit-remaining:
+      - '98'
+    status:
+      code: 200
+      message: OK
+- request:
+    body: null
+    headers:
+      Accept:
+      - '*/*'
+      Accept-Encoding:
+      - gzip, deflate
+      Connection:
+      - keep-alive
+      User-Agent:
+      - python-requests/2.28.2
+    method: GET
+    uri: https://api.stlouisfed.org/fred/release/related_tags?file_type=json&release_id=10&tag_names=sa%3Bforeign
+  response:
+    body:
+      string: !!binary |
+        H4sIAAAAAAAEA6pWKkpNzCnJzE2NLy5JLCpRslIyMjAy1jUw0TUyV9JByKbmpaDL5RelpBbFJ1Uq
+        WSkVpxZlphbHJ+eX5pUo6SgV5xeVxIOllayUUlKLk5V0lCByVgY6SvlpacWpJUogJmA5mbmZJUpW
+        hgYGBjpKJYnpxUpW0bG1ADvPSoCVAAAA
+    headers:
+      Accept-Ranges:
+      - bytes
+      Connection:
+      - keep-alive
+      Content-Encoding:
+      - gzip
+      Content-Length:
+      - '138'
+      Content-Type:
+      - application/json; charset=UTF-8
+      Date:
+      - Fri, 28 Apr 2023 01:29:11 GMT
+      ETag:
+      - W/"b7b91a6326279f8fa135842f24cc2308-gzip-gzip"
+      Expires:
+      - Sat, 29 Apr 2023 01:29:11 GMT
+      Vary:
+      - Accept-Encoding
+      x-rate-limit-limit:
+      - '120'
+      x-rate-limit-remaining:
+      - '97'
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `pyfredapi-0.6.0/tests/vhs/test_category/test_get_category_tags[pandas].yaml` & `pyfredapi-0.7.0/tests/vhs/test_category/test_get_category_related_tags[pandas].yaml`

 * *Files 26% similar despite different names*

```diff
@@ -5,112 +5,112 @@
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python-requests/2.28.1
+      - python-requests/2.28.2
     method: GET
-    uri: https://api.stlouisfed.org/fred/category/tags?category_id=125&file_type=json
+    uri: https://api.stlouisfed.org/fred/category/related_tags?category_id=125&file_type=json&tag_names=balance
   response:
     body:
       string: !!binary |
-        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
+        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
     headers:
       Accept-Ranges:
       - bytes
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Length:
-      - '845'
+      - '850'
       Content-Type:
       - application/json; charset=UTF-8
       Date:
-      - Fri, 21 Oct 2022 14:44:15 GMT
+      - Thu, 27 Apr 2023 14:58:29 GMT
       ETag:
-      - W/"c21027dd6c9bfd3018524a28a083b372-gzip-gzip"
+      - W/"d30ca904f26ed64f4b3363fa50266ac9-gzip-gzip"
       Expires:
-      - Sat, 22 Oct 2022 14:44:14 GMT
+      - Fri, 28 Apr 2023 14:58:29 GMT
       Vary:
       - Accept-Encoding
       x-rate-limit-limit:
       - '120'
       x-rate-limit-remaining:
-      - '104'
+      - '101'
     status:
       code: 200
       message: OK
 - request:
     body: null
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python-requests/2.28.1
+      - python-requests/2.28.2
     method: GET
-    uri: https://api.stlouisfed.org/fred/category/tags?category_id=125&file_type=json
+    uri: https://api.stlouisfed.org/fred/category/related_tags?category_id=125&file_type=json&tag_names=balance
   response:
     body:
       string: !!binary |
-        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
+        H4sIAAAAAAAEA6pWKkpNzCnJzE2NLy5JLCpRslIyMjAy1jUw0TUyV9JByKbmpaDL5RelpBbFJ1Uq
+        WSkVpxZlphbHJ+eX5pUo6SgV5xeVxIOllayUUlKLk5V0lCByVkbGOkr5aWnFqSVKVgY6SjmZuZkl
+        SlaGBgYGOkolienFSlbR1Up5ibmpSlZKeYklmfl5SjpK6UX5pQXxmSAXpKfmg2zIyy9JLVayUgIZ
+        XJSaWJIKkjMyMDTSNTDSNTJXMDSwMrSwMrTUNTBT0lEqyC8ozUksyiypVLKytNRBda6ViUGtDtzO
+        gtKknMxkhZT83MTMPCuF5MwSsCMUilILS1OLQfagOCcZ5DWoY/JKc3J0lJKRnWOha2ika2iuYGRs
+        ZWxsZWhMsnNKixMx/K+kowS1USk0L7MkNUUhuCSxJLVYIT9NwTE3tSgzGaQHxR2Eg8UQFAEo0Yga
+        LkmpIEORIqK4CMnrSk6lRamJpSAXuCbn5+XnZiYrOOYl5lQWZxaTHkXm5uhRZGyGFEWFpYlFJalF
+        OZWoIZNWlFqIFDSkW2thgm6tkQmStXnoUVGcmgjyHCwu/PJLFIJTE4vz8xJzcioVHFOySqHphcSo
+        wEyhRkZI7kjPz08B2YsUF+mpoFwCcwjpPjezQPe5oQWSjQQ8ThVPW2BkSxQnpGQWJ+fnlWTmlaam
+        oEY7xX7HiHVD5FgvTi0qy0xOpXaAY6RwFEuT8gvwedIpMScxLzkVlNsCEitzU/NKQM5DSWXGugaG
+        ukYWCoYmVqCiEEvBY2KMEefI5WBJUWJKKj5HkJ7KTPHbmJiXV5qYg2ol5XnaFN2XyAk7OTWvuBQU
+        dkh5CbVcc4apQAldwsWpOUaOQrY3My85P5fKoWtmhs+nufl5JRlULzEtMfIOsi+TS4uKUvNKFBKT
+        IXU/SsVJabY1xvAuchWRmVeWWlwCyhmo6YlSWzGTMHJZUVCUmZtYhFYtUWqlCUZRgWxlcmJBZkli
+        Dm3C2BDDauR6KCM1MSUnMy9VIS0zvbSIpNRsrGtoqGtoqWBobGVqamWKpXTCDGhkq3NTi5IzEvNS
+        MovJsNZYwdDMysDCytgQszVmZISeiZCtLUAUtkgFBqURbIxRVABmVBtbCwDrnCAXmQsAAA==
     headers:
       Accept-Ranges:
       - bytes
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Length:
-      - '845'
+      - '850'
       Content-Type:
       - application/json; charset=UTF-8
       Date:
-      - Fri, 21 Oct 2022 14:44:15 GMT
+      - Fri, 28 Apr 2023 01:28:57 GMT
       ETag:
-      - W/"c21027dd6c9bfd3018524a28a083b372-gzip-gzip"
+      - W/"d30ca904f26ed64f4b3363fa50266ac9-gzip-gzip"
       Expires:
-      - Sat, 22 Oct 2022 14:44:15 GMT
+      - Sat, 29 Apr 2023 01:28:57 GMT
       Vary:
       - Accept-Encoding
       x-rate-limit-limit:
       - '120'
       x-rate-limit-remaining:
-      - '103'
+      - '101'
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `pyfredapi-0.6.0/tests/vhs/test_maps/test_get_geoseries[json].yaml` & `pyfredapi-0.7.0/tests/vhs/test_tags/test_get_tag_series.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -5,222 +5,274 @@
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python-requests/2.28.1
+      - python-requests/2.28.2
     method: GET
-    uri: https://api.stlouisfed.org/geofred//series/data?date=2021-01-01&file_type=json&series_id=WIPCPI&start_date=2019-01-01
+    uri: https://api.stlouisfed.org/fred/tags/series?file_type=json&tag_names=slovenia%3Bfood%3Boecd
   response:
     body:
       string: !!binary |
-        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
+        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
     headers:
       Accept-Ranges:
       - bytes
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Length:
-      - '2653'
+      - '1539'
       Content-Type:
       - application/json; charset=UTF-8
       Date:
-      - Fri, 21 Oct 2022 14:56:36 GMT
+      - Thu, 27 Apr 2023 14:59:31 GMT
       ETag:
-      - '"451f11741b1c9cd7948aa4f18627d3a0-gzip"'
+      - W/"d92191e7ee0c444ac0417190d1ea07da-gzip-gzip"
       Expires:
-      - Fri, 21 Oct 2022 15:06:35 GMT
+      - Thu, 27 Apr 2023 15:09:31 GMT
       Vary:
       - Accept-Encoding
       x-rate-limit-limit:
       - '120'
       x-rate-limit-remaining:
-      - '120'
+      - '88'
     status:
       code: 200
       message: OK
 - request:
     body: null
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python-requests/2.28.1
+      - python-requests/2.28.2
     method: GET
-    uri: https://api.stlouisfed.org/geofred//series/group?file_type=json&series_id=WIPCPI
+    uri: https://api.stlouisfed.org/fred/tags/series?file_type=json&tag_names=slovenia%3Bfood%3Boecd
   response:
     body:
       string: !!binary |
-        H4sIAAAAAAAEA6pWKk4tykwtjk8vyi8tULKqVirJLMlJVbJSCkgtUnBOLMgsSVQISC0qzs9LzFHw
-        zEvOz01V0lEqSk3PzM+LL6ksACktLkksAYmiGqVkYWGkpKNUnJpYnJ+nZKXkF+yopKNUmpdZUqxk
-        peSSn5OTWFSspKOUVpRaWJqal1ypZKXkmJdXmpijpKOUm5kXnwIy1UrJ0NLIUtfAUNfAECSeWAET
-        NzIwAgmCxAGrrQUA1qmJWsgAAAA=
+        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
     headers:
       Accept-Ranges:
       - bytes
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Length:
-      - '191'
+      - '1539'
       Content-Type:
       - application/json; charset=UTF-8
       Date:
-      - Fri, 21 Oct 2022 14:56:36 GMT
+      - Thu, 27 Apr 2023 14:59:32 GMT
       ETag:
-      - '"153c7c9bf9aea8ceb7e89963b1a4d947-gzip"'
+      - W/"d92191e7ee0c444ac0417190d1ea07da-gzip-gzip"
       Expires:
-      - Sat, 22 Oct 2022 14:54:33 GMT
+      - Thu, 27 Apr 2023 15:09:32 GMT
       Vary:
       - Accept-Encoding
       x-rate-limit-limit:
       - '120'
       x-rate-limit-remaining:
+      - '87'
+    status:
+      code: 200
+      message: OK
+- request:
+    body: null
+    headers:
+      Accept:
+      - '*/*'
+      Accept-Encoding:
+      - gzip, deflate
+      Connection:
+      - keep-alive
+      User-Agent:
+      - python-requests/2.28.2
+    method: GET
+    uri: https://api.stlouisfed.org/fred/tags/series?file_type=json&tag_names=slovenia%3Bfood%3Boecd
+  response:
+    body:
+      string: !!binary |
+        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
+    headers:
+      Accept-Ranges:
+      - bytes
+      Connection:
+      - keep-alive
+      Content-Encoding:
+      - gzip
+      Content-Length:
+      - '1539'
+      Content-Type:
+      - application/json; charset=UTF-8
+      Date:
+      - Fri, 28 Apr 2023 01:29:58 GMT
+      ETag:
+      - '"e695ae7936c5fb535fa5fa697c4f7844-gzip"'
+      Expires:
+      - Fri, 28 Apr 2023 01:39:58 GMT
+      Vary:
+      - Accept-Encoding
+      x-rate-limit-limit:
       - '120'
+      x-rate-limit-remaining:
+      - '36'
     status:
       code: 200
       message: OK
 - request:
     body: null
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python-requests/2.28.1
+      - python-requests/2.28.2
     method: GET
-    uri: https://api.stlouisfed.org/geofred//series/data?date=2021-01-01&file_type=json&return_format=json&series_id=WIPCPI&start_date=2019-01-01
+    uri: https://api.stlouisfed.org/fred/tags/series?file_type=json&tag_names=slovenia%3Bfood%3Boecd
   response:
     body:
       string: !!binary |
-        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
+        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
     headers:
       Accept-Ranges:
       - bytes
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Length:
-      - '2653'
+      - '1539'
       Content-Type:
       - application/json; charset=UTF-8
       Date:
-      - Fri, 21 Oct 2022 14:56:37 GMT
+      - Fri, 28 Apr 2023 01:29:58 GMT
       ETag:
-      - '"d2af875f8d7f5833202594add3184f4c-gzip"'
+      - W/"e695ae7936c5fb535fa5fa697c4f7844-gzip-gzip"
       Expires:
-      - Fri, 21 Oct 2022 15:06:36 GMT
+      - Fri, 28 Apr 2023 01:39:58 GMT
       Vary:
       - Accept-Encoding
       x-rate-limit-limit:
       - '120'
       x-rate-limit-remaining:
-      - '119'
+      - '35'
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `pyfredapi-0.6.0/tests/vhs/test_maps/test_get_geoseries_info.yaml` & `pyfredapi-0.7.0/tests/vhs/test_series/test_search_series_related_tags[pandas].yaml`

 * *Files 21% similar despite different names*

```diff
@@ -5,90 +5,88 @@
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python-requests/2.28.1
+      - python-requests/2.28.2
     method: GET
-    uri: https://api.stlouisfed.org/geofred//series/group?file_type=json&series_id=WIPCPI
+    uri: https://api.stlouisfed.org/fred/series/search/related_tags?file_type=json&series_search_text=monetary%2Bservice%2Bindex&tag_names=30-year%3Bfrb
   response:
     body:
       string: !!binary |
-        H4sIAAAAAAAEA6pWKk4tykwtjk8vyi8tULKqVirJLMlJVbJSCkgtUnBOLMgsSVQISC0qzs9LzFHw
-        zEvOz01V0lEqSk3PzM+LL6ksACktLkksAYmiGqVkYWGkpKNUnJpYnJ+nZKXkF+yopKNUmpdZUqxk
-        peSSn5OTWFSspKOUVpRaWJqal1ypZKXkmJdXmpijpKOUm5kXnwIy1UrJ0NLIUtfAUNfAECSeWAET
-        NzIwAgmCxAGrrQUA1qmJWsgAAAA=
+        H4sIAAAAAAAEA6pWKkpNzCnJzE2NLy5JLCpRslIyMjAy1jUw0TUyV9JByKbmpaDL5RelpBbFJ1Uq
+        WSkVpxZlphbHJ+eX5pUo6SgV5xeVxIOllayUUlKLk5V0lCByVgY6SvlpacWpJUogJmA5mbmZJUpW
+        hgYGBjpKJYnpxUpW0bG1ADvPSoCVAAAA
     headers:
       Accept-Ranges:
       - bytes
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Length:
-      - '191'
+      - '138'
       Content-Type:
       - application/json; charset=UTF-8
       Date:
-      - Fri, 21 Oct 2022 14:56:34 GMT
+      - Thu, 27 Apr 2023 14:59:11 GMT
       ETag:
-      - '"153c7c9bf9aea8ceb7e89963b1a4d947-gzip"'
+      - W/"54d0e6d98b0491cc5f504bc7603102fb-gzip-gzip"
       Expires:
-      - Sat, 22 Oct 2022 14:54:33 GMT
+      - Fri, 28 Apr 2023 14:59:11 GMT
       Vary:
       - Accept-Encoding
       x-rate-limit-limit:
       - '120'
       x-rate-limit-remaining:
-      - '120'
+      - '107'
     status:
       code: 200
       message: OK
 - request:
     body: null
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python-requests/2.28.1
+      - python-requests/2.28.2
     method: GET
-    uri: https://api.stlouisfed.org/geofred//series/group?file_type=json&series_id=WIPCPI
+    uri: https://api.stlouisfed.org/fred/series/search/related_tags?file_type=json&series_search_text=monetary%2Bservice%2Bindex&tag_names=30-year%3Bfrb
   response:
     body:
       string: !!binary |
-        H4sIAAAAAAAEA6pWKk4tykwtjk8vyi8tULKqVirJLMlJVbJSCkgtUnBOLMgsSVQISC0qzs9LzFHw
-        zEvOz01V0lEqSk3PzM+LL6ksACktLkksAYmiGqVkYWGkpKNUnJpYnJ+nZKXkF+yopKNUmpdZUqxk
-        peSSn5OTWFSspKOUVpRaWJqal1ypZKXkmJdXmpijpKOUm5kXnwIy1UrJ0NLIUtfAUNfAECSeWAET
-        NzIwAgmCxAGrrQUA1qmJWsgAAAA=
+        H4sIAAAAAAAEA6pWKkpNzCnJzE2NLy5JLCpRslIyMjAy1jUw0TUyV9JByKbmpaDL5RelpBbFJ1Uq
+        WSkVpxZlphbHJ+eX5pUo6SgV5xeVxIOllayUUlKLk5V0lCByVgY6SvlpacWpJUogJmA5mbmZJUpW
+        hgYGBjpKJYnpxUpW0bG1ADvPSoCVAAAA
     headers:
       Accept-Ranges:
       - bytes
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Length:
-      - '191'
+      - '138'
       Content-Type:
       - application/json; charset=UTF-8
       Date:
-      - Fri, 21 Oct 2022 14:56:34 GMT
+      - Fri, 28 Apr 2023 01:29:37 GMT
       ETag:
-      - '"153c7c9bf9aea8ceb7e89963b1a4d947-gzip"'
+      - W/"54d0e6d98b0491cc5f504bc7603102fb-gzip-gzip"
       Expires:
-      - Sat, 22 Oct 2022 14:54:33 GMT
+      - Sat, 29 Apr 2023 01:29:37 GMT
       Vary:
       - Accept-Encoding
       x-rate-limit-limit:
       - '120'
       x-rate-limit-remaining:
-      - '120'
+      - '55'
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `pyfredapi-0.6.0/tests/vhs/test_maps/test_get_shape_files.yaml` & `pyfredapi-0.7.0/tests/vhs/test_maps/test_get_shape_files.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -5,15 +5,15 @@
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python-requests/2.28.1
+      - python-requests/2.28.2
     method: GET
     uri: https://api.stlouisfed.org/geofred//shapes/file?file_type=json&shape=bea
   response:
     body:
       string: !!binary |
         H4sIAAAAAAAEA6pWKqksSFWyUnJLTSwpLUp1zs/JSU0uyczPU9JRykvMBUkVlySWpMYnpSbGF6Wm
         Q2SSi4qVrOB6wep0lAqK8gtSi0oyU8FyYEErpdKiPKv89GSrlNQ0q+SiYit/d2crQz1jK+egYAsT
@@ -389,39 +389,39 @@
       Content-Encoding:
       - gzip
       Content-Length:
       - '20855'
       Content-Type:
       - application/json; charset=UTF-8
       Date:
-      - Fri, 21 Oct 2022 14:56:35 GMT
+      - Thu, 27 Apr 2023 14:58:31 GMT
       ETag:
-      - '"3cf7ebfdeb72821584cb68136171432a-gzip"'
+      - '"f960410b9b1a32174c4bbd501d22578b-gzip"'
       Expires:
-      - Sat, 22 Oct 2022 14:54:35 GMT
+      - Fri, 28 Apr 2023 14:55:10 GMT
       Vary:
       - Accept-Encoding
       x-rate-limit-limit:
       - '120'
       x-rate-limit-remaining:
-      - '119'
+      - '99'
     status:
       code: 200
       message: OK
 - request:
     body: null
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python-requests/2.28.1
+      - python-requests/2.28.2
     method: GET
     uri: https://api.stlouisfed.org/geofred//shapes/file?file_type=json&shape=bea
   response:
     body:
       string: !!binary |
         H4sIAAAAAAAEA6pWKqksSFWyUnJLTSwpLUp1zs/JSU0uyczPU9JRykvMBUkVlySWpMYnpSbGF6Wm
         Q2SSi4qVrOB6wep0lAqK8gtSi0oyU8FyYEErpdKiPKv89GSrlNQ0q+SiYit/d2crQz1jK+egYAsT
@@ -797,22 +797,838 @@
       Content-Encoding:
       - gzip
       Content-Length:
       - '20855'
       Content-Type:
       - application/json; charset=UTF-8
       Date:
-      - Fri, 21 Oct 2022 14:56:35 GMT
+      - Thu, 27 Apr 2023 14:58:32 GMT
       ETag:
-      - '"3cf7ebfdeb72821584cb68136171432a-gzip"'
+      - '"f960410b9b1a32174c4bbd501d22578b-gzip"'
       Expires:
-      - Sat, 22 Oct 2022 14:54:35 GMT
+      - Fri, 28 Apr 2023 14:55:10 GMT
       Vary:
       - Accept-Encoding
       x-rate-limit-limit:
       - '120'
       x-rate-limit-remaining:
-      - '119'
+      - '99'
+    status:
+      code: 200
+      message: OK
+- request:
+    body: null
+    headers:
+      Accept:
+      - '*/*'
+      Accept-Encoding:
+      - gzip, deflate
+      Connection:
+      - keep-alive
+      User-Agent:
+      - python-requests/2.28.2
+    method: GET
+    uri: https://api.stlouisfed.org/geofred//shapes/file?file_type=json&shape=bea
+  response:
+    body:
+      string: !!binary |
+        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
+    headers:
+      Accept-Ranges:
+      - bytes
+      Connection:
+      - keep-alive
+      Content-Encoding:
+      - gzip
+      Content-Length:
+      - '20855'
+      Content-Type:
+      - application/json; charset=UTF-8
+      Date:
+      - Fri, 28 Apr 2023 01:28:59 GMT
+      ETag:
+      - '"f960410b9b1a32174c4bbd501d22578b-gzip"'
+      Expires:
+      - Fri, 28 Apr 2023 14:55:10 GMT
+      Vary:
+      - Accept-Encoding
+      x-rate-limit-limit:
+      - '120'
+      x-rate-limit-remaining:
+      - '99'
+    status:
+      code: 200
+      message: OK
+- request:
+    body: null
+    headers:
+      Accept:
+      - '*/*'
+      Accept-Encoding:
+      - gzip, deflate
+      Connection:
+      - keep-alive
+      User-Agent:
+      - python-requests/2.28.2
+    method: GET
+    uri: https://api.stlouisfed.org/geofred//shapes/file?file_type=json&shape=bea
+  response:
+    body:
+      string: !!binary |
+        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
+    headers:
+      Accept-Ranges:
+      - bytes
+      Connection:
+      - keep-alive
+      Content-Encoding:
+      - gzip
+      Content-Length:
+      - '20855'
+      Content-Type:
+      - application/json; charset=UTF-8
+      Date:
+      - Fri, 28 Apr 2023 01:28:59 GMT
+      ETag:
+      - '"f960410b9b1a32174c4bbd501d22578b-gzip"'
+      Expires:
+      - Fri, 28 Apr 2023 14:55:10 GMT
+      Vary:
+      - Accept-Encoding
+      x-rate-limit-limit:
+      - '120'
+      x-rate-limit-remaining:
+      - '99'
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `pyfredapi-0.6.0/tests/vhs/test_release/test_get_release.yaml` & `pyfredapi-0.7.0/tests/vhs/test_release/test_get_release.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -5,88 +5,178 @@
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python-requests/2.28.1
+      - python-requests/2.28.2
     method: GET
     uri: https://api.stlouisfed.org/fred/release?file_type=json&release_id=10
   response:
     body:
       string: !!binary |
-        H4sIAAAAAAAEA6pWKkpNzCnJzE2NLy5JLCpRslIyMjAy0jU00DUyVNJByKbmpWDK5aQmFqcWK1lF
+        H4sIAAAAAAAEA6pWKkpNzCnJzE2NLy5JLCpRslIyMjAy1jUw0TUyV9JByKbmpWDK5aQmFqcWK1lF
         VytlpihZGRogaSDZuLzE3FQlKyXn/Lzi0tzUIoWAoszkVAXPvJTUCiUdpYKi1OLi+KJUsJWAKVmV
-        FJWm6ijlZOZlK1kpZZSUFFjF6Mfol5eX6yXlFOul55fF6CcXZMboK9XG1gIAp19d9OQAAAA=
+        FJWm6ijlZOZlK1kpZZSUFFjF6Mfol5eX6yXlFOul55fF6CcXZMboK9XG1gIAITa72eQAAAA=
     headers:
       Accept-Ranges:
       - bytes
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Length:
       - '167'
       Content-Type:
       - application/json; charset=UTF-8
       Date:
-      - Fri, 21 Oct 2022 15:13:19 GMT
+      - Thu, 27 Apr 2023 14:58:37 GMT
       ETag:
-      - '"a15c79d85d6e5c112405473d801a8586-gzip"'
+      - W/"58c7be1fd24b4cbd94fa10c22b905ad8-gzip-gzip"
       Expires:
-      - Sat, 22 Oct 2022 15:13:19 GMT
+      - Fri, 28 Apr 2023 14:58:37 GMT
       Vary:
       - Accept-Encoding
       x-rate-limit-limit:
       - '120'
       x-rate-limit-remaining:
-      - '116'
+      - '96'
     status:
       code: 200
       message: OK
 - request:
     body: null
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python-requests/2.28.1
+      - python-requests/2.28.2
     method: GET
     uri: https://api.stlouisfed.org/fred/release?file_type=json&release_id=10
   response:
     body:
       string: !!binary |
-        H4sIAAAAAAAEA6pWKkpNzCnJzE2NLy5JLCpRslIyMjAy0jU00DUyVNJByKbmpWDK5aQmFqcWK1lF
+        H4sIAAAAAAAEA6pWKkpNzCnJzE2NLy5JLCpRslIyMjAy1jUw0TUyV9JByKbmpWDK5aQmFqcWK1lF
         VytlpihZGRogaSDZuLzE3FQlKyXn/Lzi0tzUIoWAoszkVAXPvJTUCiUdpYKi1OLi+KJUsJWAKVmV
-        FJWm6ijlZOZlK1kpZZSUFFjF6Mfol5eX6yXlFOul55fF6CcXZMboK9XG1gIAp19d9OQAAAA=
+        FJWm6ijlZOZlK1kpZZSUFFjF6Mfol5eX6yXlFOul55fF6CcXZMboK9XG1gIAITa72eQAAAA=
     headers:
       Accept-Ranges:
       - bytes
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Length:
       - '167'
       Content-Type:
       - application/json; charset=UTF-8
       Date:
-      - Fri, 21 Oct 2022 15:13:19 GMT
+      - Thu, 27 Apr 2023 14:58:38 GMT
       ETag:
-      - W/"a15c79d85d6e5c112405473d801a8586-gzip-gzip"
+      - W/"58c7be1fd24b4cbd94fa10c22b905ad8-gzip-gzip"
       Expires:
-      - Sat, 22 Oct 2022 15:13:19 GMT
+      - Fri, 28 Apr 2023 14:58:38 GMT
       Vary:
       - Accept-Encoding
       x-rate-limit-limit:
       - '120'
       x-rate-limit-remaining:
-      - '115'
+      - '95'
+    status:
+      code: 200
+      message: OK
+- request:
+    body: null
+    headers:
+      Accept:
+      - '*/*'
+      Accept-Encoding:
+      - gzip, deflate
+      Connection:
+      - keep-alive
+      User-Agent:
+      - python-requests/2.28.2
+    method: GET
+    uri: https://api.stlouisfed.org/fred/release?file_type=json&release_id=10
+  response:
+    body:
+      string: !!binary |
+        H4sIAAAAAAAEA6pWKkpNzCnJzE2NLy5JLCpRslIyMjAy1jUw0TUyV9JByKbmpWDK5aQmFqcWK1lF
+        VytlpihZGRogaSDZuLzE3FQlKyXn/Lzi0tzUIoWAoszkVAXPvJTUCiUdpYKi1OLi+KJUsJWAKVmV
+        FJWm6ijlZOZlK1kpZZSUFFjF6Mfol5eX6yXlFOul55fF6CcXZMboK9XG1gIAITa72eQAAAA=
+    headers:
+      Accept-Ranges:
+      - bytes
+      Connection:
+      - keep-alive
+      Content-Encoding:
+      - gzip
+      Content-Length:
+      - '167'
+      Content-Type:
+      - application/json; charset=UTF-8
+      Date:
+      - Fri, 28 Apr 2023 01:29:05 GMT
+      ETag:
+      - W/"58c7be1fd24b4cbd94fa10c22b905ad8-gzip-gzip"
+      Expires:
+      - Sat, 29 Apr 2023 01:29:05 GMT
+      Vary:
+      - Accept-Encoding
+      x-rate-limit-limit:
+      - '120'
+      x-rate-limit-remaining:
+      - '114'
+    status:
+      code: 200
+      message: OK
+- request:
+    body: null
+    headers:
+      Accept:
+      - '*/*'
+      Accept-Encoding:
+      - gzip, deflate
+      Connection:
+      - keep-alive
+      User-Agent:
+      - python-requests/2.28.2
+    method: GET
+    uri: https://api.stlouisfed.org/fred/release?file_type=json&release_id=10
+  response:
+    body:
+      string: !!binary |
+        H4sIAAAAAAAEA6pWKkpNzCnJzE2NLy5JLCpRslIyMjAy1jUw0TUyV9JByKbmpWDK5aQmFqcWK1lF
+        VytlpihZGRogaSDZuLzE3FQlKyXn/Lzi0tzUIoWAoszkVAXPvJTUCiUdpYKi1OLi+KJUsJWAKVmV
+        FJWm6ijlZOZlK1kpZZSUFFjF6Mfol5eX6yXlFOul55fF6CcXZMboK9XG1gIAITa72eQAAAA=
+    headers:
+      Accept-Ranges:
+      - bytes
+      Connection:
+      - keep-alive
+      Content-Encoding:
+      - gzip
+      Content-Length:
+      - '167'
+      Content-Type:
+      - application/json; charset=UTF-8
+      Date:
+      - Fri, 28 Apr 2023 01:29:05 GMT
+      ETag:
+      - W/"58c7be1fd24b4cbd94fa10c22b905ad8-gzip-gzip"
+      Expires:
+      - Sat, 29 Apr 2023 01:29:05 GMT
+      Vary:
+      - Accept-Encoding
+      x-rate-limit-limit:
+      - '120'
+      x-rate-limit-remaining:
+      - '113'
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `pyfredapi-0.6.0/tests/vhs/test_release/test_get_release_dates.yaml` & `pyfredapi-0.7.0/tests/vhs/test_release/test_get_release_dates.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -5,23 +5,23 @@
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python-requests/2.28.1
+      - python-requests/2.28.2
     method: GET
     uri: https://api.stlouisfed.org/fred/release/dates?file_type=json&release_id=10
   response:
     body:
       string: !!binary |
         H4sIAAAAAAAEA6pWKkpNzCnJzE2NLy5JLCpRslIyNDc30zUw1zUwUdJByKbmpShZKVlaWlrqGhrp
-        Ghsq6SjlF6WkFsUnVSpZKRWl5qQmFqfGpySWpCrpKBXnF5XEg6WVrJQSi5OVdJSS80vzSpSsLA0M
-        dZTy09KKU0uUrAx0lHIyczNLlKwMDQwMDEC2IYwpVrKKBrkOIpKZAlKkowS2wErJ0NLEUtfAWNfI
+        Ghsq6SjlF6WkFsUnVSpZKRWl5qQmFqfGpySWpCrpKBXnF5XEg6WVrJQSi5OVdJSS80vzSpSsLA0s
+        dJTy09KKU0uUrAx0lHIyczNLlKwMDQwMDEC2IYwpVrKKBrkOIpKZAlKkowS2wErJ0NLEUtfAWNfI
         RKlWh4AqE10jI8KqTHWNjAmrMiPKRnOibLTQNTIjbKOlrpEFQVWGBkSpMiRKlRFBVaYGugaGBF0P
         UmVEMLxAqox1jUzx+xGkinA8glSZ6hoZEDbLjCgbCccjyEYLgikHpMqSmJAAxSOBFG1qoGtoqGtk
         SdCPhkaE3WUIjkdCYW8IymkGBPKQKVgVofwIUmVCOIYMdQ0I50eQWWa6RuYEQsIQVJYRymkgsywI
         x5ChroGlrpEhQRtB8Ug4VEHxSKDMMTUElbYEbTQiKh6NdA2MCOdaI1BsE2MjEfnRCByPhFKOka6B
         ma4hoRRtBI5HQrnDSNfAgnAMGYHikQgbQfFI2EZQPBJKE0ageCRoozEoHg0J1AqmxuB4JJTujcHx
         SIRZRMSjMVHxaAyKR0K1KMj1RJSrxuB4JML1loRLOWNdUDwSqEVNjcHlKqFcawyKR4J+NAHFI6FW
         h6kJOB4J+dEEHI+EUqGJrgER8WgCjkdCadUEHI+Ecq0JOD8SKr9MwPFIqEY2AeVHgnWHCTgeCYcX
@@ -99,61 +99,61 @@
         IqL9BVlnRSiGIKNkhFWB4pFAr8kQMkpGKB4h66wIxSNRo2SG4PEvQiMPUFVE2EhEjQxZjUWozQQZ
         JcO7x8DIAOQuwqsGQKoIj4CDVFno4l8dCbGRiPYXZJQM7woXsFmg1jbhUAXlWkJmQUbJCIUXePyL
         0NiQIWT8iwgbTQiHF2T8i1CtYAEeESHC9eYE1hcaGYBcDxq2wrfSEqKK0CpXsCpQrsW75hSiypBw
         Cxky/kXIj5DxL0I2WoJGtgimVYgqQvEIGf8iwl2ghgeBULXUNQBN/hBWBSrCCKsCDSMTVkXEiIgl
         eM0WYT+CYptQWoWs2SIcqqBcSyAejSDjXwTKQpAqI4I5DaqKgLtAqoyJMotwbIPMAk3P4Y8hkCoz
         Xfy7LYwMQKoIl9EgVaBsRNhGUCQRVAWKbcLhBSqjCaQcIwPwiAiBlGMEGf8iZCN4/MuAQEsBZJYR
         4VCF7Ocjwl2ER0RANhIR25CVXUTYaE5wDAZkI+EaGaSKcI1sBNnPRzjsQbFN2PWgvE1IFWT8i1DK
-        AY9sEYxtsCqCeQgy/kWEu0DdPgK5AzL+Raj8gox/EWEjEbEN2fVHhFmE620jUNYApy/AYmsBr00b
-        WV2GAAA=
+        AY9sEYxtsCqCeQgy/kWEu0DdPgK5AzL+Raj8gox/EWEjEbEN2fVHhFmE620jUNYgnL5AhSrhPARZ
+        /0Uo5UDGvwjFNnj9F8F4hKgiVCuAV4kRassZQca/ADNSqo2tBQCrib/1Z4cAAA==
     headers:
       Accept-Ranges:
       - bytes
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Length:
-      - '5078'
+      - '5119'
       Content-Type:
       - application/json; charset=UTF-8
       Date:
-      - Fri, 21 Oct 2022 15:13:20 GMT
+      - Thu, 27 Apr 2023 14:58:39 GMT
       ETag:
-      - W/"93eb06d45a975a24b291d8e44d890361-gzip-gzip"
+      - W/"1631795f5b0095a13f80c438488748cd-gzip-gzip"
       Expires:
-      - Fri, 21 Oct 2022 15:23:20 GMT
+      - Thu, 27 Apr 2023 15:08:38 GMT
       Vary:
       - Accept-Encoding
       x-rate-limit-limit:
       - '120'
       x-rate-limit-remaining:
-      - '114'
+      - '94'
     status:
       code: 200
       message: OK
 - request:
     body: null
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python-requests/2.28.1
+      - python-requests/2.28.2
     method: GET
     uri: https://api.stlouisfed.org/fred/release/dates?file_type=json&release_id=10
   response:
     body:
       string: !!binary |
         H4sIAAAAAAAEA6pWKkpNzCnJzE2NLy5JLCpRslIyNDc30zUw1zUwUdJByKbmpShZKVlaWlrqGhrp
-        Ghsq6SjlF6WkFsUnVSpZKRWl5qQmFqfGpySWpCrpKBXnF5XEg6WVrJQSi5OVdJSS80vzSpSsLA0M
-        dZTy09KKU0uUrAx0lHIyczNLlKwMDQwMDEC2IYwpVrKKBrkOIpKZAlKkowS2wErJ0NLEUtfAWNfI
+        Ghsq6SjlF6WkFsUnVSpZKRWl5qQmFqfGpySWpCrpKBXnF5XEg6WVrJQSi5OVdJSS80vzSpSsLA0s
+        dJTy09KKU0uUrAx0lHIyczNLlKwMDQwMDEC2IYwpVrKKBrkOIpKZAlKkowS2wErJ0NLEUtfAWNfI
         RKlWh4AqE10jI8KqTHWNjAmrMiPKRnOibLTQNTIjbKOlrpEFQVWGBkSpMiRKlRFBVaYGugaGBF0P
         UmVEMLxAqox1jUzx+xGkinA8glSZ6hoZEDbLjCgbCccjyEYLgikHpMqSmJAAxSOBFG1qoGtoqGtk
         SdCPhkaE3WUIjkdCYW8IymkGBPKQKVgVofwIUmVCOIYMdQ0I50eQWWa6RuYEQsIQVJYRymkgsywI
         x5ChroGlrpEhQRtB8Ug4VEHxSKDMMTUElbYEbTQiKh6NdA2MCOdaI1BsE2MjEfnRCByPhFKOka6B
         ma4hoRRtBI5HQrnDSNfAgnAMGYHikQgbQfFI2EZQPBJKE0ageCRoozEoHg0J1AqmxuB4JJTujcHx
         SIRZRMSjMVHxaAyKR0K1KMj1RJSrxuB4JML1loRLOWNdUDwSqEVNjcHlKqFcawyKR4J+NAHFI6FW
         h6kJOB4J+dEEHI+EUqGJrgER8WgCjkdCadUEHI+Ecq0JOD8SKr9MwPFIqEY2AeVHgnWHCTgeCYcX
@@ -231,36 +231,300 @@
         IqL9BVlnRSiGIKNkhFWB4pFAr8kQMkpGKB4h66wIxSNRo2SG4PEvQiMPUFVE2EhEjQxZjUWozQQZ
         JcO7x8DIAOQuwqsGQKoIj4CDVFno4l8dCbGRiPYXZJQM7woXsFmg1jbhUAXlWkJmQUbJCIUXePyL
         0NiQIWT8iwgbTQiHF2T8i1CtYAEeESHC9eYE1hcaGYBcDxq2wrfSEqKK0CpXsCpQrsW75hSiypBw
         Cxky/kXIj5DxL0I2WoJGtgimVYgqQvEIGf8iwl2ghgeBULXUNQBN/hBWBSrCCKsCDSMTVkXEiIgl
         eM0WYT+CYptQWoWs2SIcqqBcSyAejSDjXwTKQpAqI4I5DaqKgLtAqoyJMotwbIPMAk3P4Y8hkCoz
         Xfy7LYwMQKoIl9EgVaBsRNhGUCQRVAWKbcLhBSqjCaQcIwPwiAiBlGMEGf8iZCN4/MuAQEsBZJYR
         4VCF7Ocjwl2ER0RANhIR25CVXUTYaE5wDAZkI+EaGaSKcI1sBNnPRzjsQbFN2PWgvE1IFWT8i1DK
-        AY9sEYxtsCqCeQgy/kWEu0DdPgK5AzL+Raj8gox/EWEjEbEN2fVHhFmE620jUNYApy/AYmsBr00b
-        WV2GAAA=
+        AY9sEYxtsCqCeQgy/kWEu0DdPgK5AzL+Raj8gox/EWEjEbEN2fVHhFmE620jUNYgnL5AhSrhPARZ
+        /0Uo5UDGvwjFNnj9F8F4hKgiVCuAV4kRassZQca/ADNSqo2tBQCrib/1Z4cAAA==
     headers:
       Accept-Ranges:
       - bytes
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Length:
-      - '5078'
+      - '5119'
       Content-Type:
       - application/json; charset=UTF-8
       Date:
-      - Fri, 21 Oct 2022 15:13:20 GMT
+      - Thu, 27 Apr 2023 14:58:39 GMT
       ETag:
-      - W/"93eb06d45a975a24b291d8e44d890361-gzip-gzip"
+      - W/"1631795f5b0095a13f80c438488748cd-gzip-gzip"
       Expires:
-      - Fri, 21 Oct 2022 15:23:20 GMT
+      - Thu, 27 Apr 2023 15:08:39 GMT
+      Vary:
+      - Accept-Encoding
+      x-rate-limit-limit:
+      - '120'
+      x-rate-limit-remaining:
+      - '92'
+    status:
+      code: 200
+      message: OK
+- request:
+    body: null
+    headers:
+      Accept:
+      - '*/*'
+      Accept-Encoding:
+      - gzip, deflate
+      Connection:
+      - keep-alive
+      User-Agent:
+      - python-requests/2.28.2
+    method: GET
+    uri: https://api.stlouisfed.org/fred/release/dates?file_type=json&release_id=10
+  response:
+    body:
+      string: !!binary |
+        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
+    headers:
+      Accept-Ranges:
+      - bytes
+      Connection:
+      - keep-alive
+      Content-Encoding:
+      - gzip
+      Content-Length:
+      - '5119'
+      Content-Type:
+      - application/json; charset=UTF-8
+      Date:
+      - Fri, 28 Apr 2023 01:29:06 GMT
+      ETag:
+      - '"baae1875bb0c801377071f0409c1f366-gzip"'
+      Expires:
+      - Fri, 28 Apr 2023 01:39:06 GMT
       Vary:
       - Accept-Encoding
       x-rate-limit-limit:
       - '120'
       x-rate-limit-remaining:
       - '112'
     status:
       code: 200
       message: OK
+- request:
+    body: null
+    headers:
+      Accept:
+      - '*/*'
+      Accept-Encoding:
+      - gzip, deflate
+      Connection:
+      - keep-alive
+      User-Agent:
+      - python-requests/2.28.2
+    method: GET
+    uri: https://api.stlouisfed.org/fred/release/dates?file_type=json&release_id=10
+  response:
+    body:
+      string: !!binary |
+        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
+    headers:
+      Accept-Ranges:
+      - bytes
+      Connection:
+      - keep-alive
+      Content-Encoding:
+      - gzip
+      Content-Length:
+      - '5119'
+      Content-Type:
+      - application/json; charset=UTF-8
+      Date:
+      - Fri, 28 Apr 2023 01:29:07 GMT
+      ETag:
+      - W/"baae1875bb0c801377071f0409c1f366-gzip-gzip"
+      Expires:
+      - Fri, 28 Apr 2023 01:39:06 GMT
+      Vary:
+      - Accept-Encoding
+      x-rate-limit-limit:
+      - '120'
+      x-rate-limit-remaining:
+      - '110'
+    status:
+      code: 200
+      message: OK
 version: 1
```

### Comparing `pyfredapi-0.6.0/tests/vhs/test_release/test_get_release_sources.yaml` & `pyfredapi-0.7.0/tests/vhs/test_release/test_get_release_sources.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -5,88 +5,178 @@
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python-requests/2.28.1
+      - python-requests/2.28.2
     method: GET
     uri: https://api.stlouisfed.org/fred/release/sources?file_type=json&release_id=10
   response:
     body:
       string: !!binary |
-        H4sIAAAAAAAEA6pWKkpNzCnJzE2NLy5JLCpRslIyMjAy0jU00DUyVNJByKbmpaDLFeeXFiWnFitZ
+        H4sIAAAAAAAEA6pWKkpNzCnJzE2NLy5JLCpRslIyMjAy1jUw0TUyV9JByKbmpaDLFeeXFiWnFitZ
         RVcrZaYoWRkZIakn2TTA8hJzU5WslEL1gvUUnEqLUhNLFfLTFHwSk/KLFIJLEksyi0syk4uVdJRy
-        MvOylayUMkpKCoqtYvRj9MvLy/WScor10vPLYvSVamNrAYt1tSfVAAAA
+        MvOylayUMkpKCoqtYvRj9MvLy/WScor10vPLYvSVamNrAV+oHQTVAAAA
     headers:
       Accept-Ranges:
       - bytes
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Length:
       - '156'
       Content-Type:
       - application/json; charset=UTF-8
       Date:
-      - Fri, 21 Oct 2022 15:15:01 GMT
+      - Thu, 27 Apr 2023 14:58:41 GMT
       ETag:
-      - '"222ae02222ef6412ad99b94f9695cc94-gzip"'
+      - W/"10494880d8d7a0e8d1a1912b3e61b973-gzip-gzip"
       Expires:
-      - Sat, 22 Oct 2022 15:15:01 GMT
+      - Fri, 28 Apr 2023 14:58:41 GMT
       Vary:
       - Accept-Encoding
       x-rate-limit-limit:
       - '120'
       x-rate-limit-remaining:
+      - '86'
+    status:
+      code: 200
+      message: OK
+- request:
+    body: null
+    headers:
+      Accept:
+      - '*/*'
+      Accept-Encoding:
+      - gzip, deflate
+      Connection:
+      - keep-alive
+      User-Agent:
+      - python-requests/2.28.2
+    method: GET
+    uri: https://api.stlouisfed.org/fred/release/sources?file_type=json&release_id=10
+  response:
+    body:
+      string: !!binary |
+        H4sIAAAAAAAEA6pWKkpNzCnJzE2NLy5JLCpRslIyMjAy1jUw0TUyV9JByKbmpaDLFeeXFiWnFitZ
+        RVcrZaYoWRkZIakn2TTA8hJzU5WslEL1gvUUnEqLUhNLFfLTFHwSk/KLFIJLEksyi0syk4uVdJRy
+        MvOylayUMkpKCoqtYvRj9MvLy/WScor10vPLYvSVamNrAV+oHQTVAAAA
+    headers:
+      Accept-Ranges:
+      - bytes
+      Connection:
+      - keep-alive
+      Content-Encoding:
+      - gzip
+      Content-Length:
+      - '156'
+      Content-Type:
+      - application/json; charset=UTF-8
+      Date:
+      - Thu, 27 Apr 2023 14:58:42 GMT
+      ETag:
+      - W/"10494880d8d7a0e8d1a1912b3e61b973-gzip-gzip"
+      Expires:
+      - Fri, 28 Apr 2023 14:58:42 GMT
+      Vary:
+      - Accept-Encoding
+      x-rate-limit-limit:
       - '120'
+      x-rate-limit-remaining:
+      - '84'
+    status:
+      code: 200
+      message: OK
+- request:
+    body: null
+    headers:
+      Accept:
+      - '*/*'
+      Accept-Encoding:
+      - gzip, deflate
+      Connection:
+      - keep-alive
+      User-Agent:
+      - python-requests/2.28.2
+    method: GET
+    uri: https://api.stlouisfed.org/fred/release/sources?file_type=json&release_id=10
+  response:
+    body:
+      string: !!binary |
+        H4sIAAAAAAAEA6pWKkpNzCnJzE2NLy5JLCpRslIyMjAy1jUw0TUyV9JByKbmpaDLFeeXFiWnFitZ
+        RVcrZaYoWRkZIakn2TTA8hJzU5WslEL1gvUUnEqLUhNLFfLTFHwSk/KLFIJLEksyi0syk4uVdJRy
+        MvOylayUMkpKCoqtYvRj9MvLy/WScor10vPLYvSVamNrAV+oHQTVAAAA
+    headers:
+      Accept-Ranges:
+      - bytes
+      Connection:
+      - keep-alive
+      Content-Encoding:
+      - gzip
+      Content-Length:
+      - '156'
+      Content-Type:
+      - application/json; charset=UTF-8
+      Date:
+      - Fri, 28 Apr 2023 01:29:09 GMT
+      ETag:
+      - W/"10494880d8d7a0e8d1a1912b3e61b973-gzip-gzip"
+      Expires:
+      - Sat, 29 Apr 2023 01:29:09 GMT
+      Vary:
+      - Accept-Encoding
+      x-rate-limit-limit:
+      - '120'
+      x-rate-limit-remaining:
+      - '104'
     status:
       code: 200
       message: OK
 - request:
     body: null
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python-requests/2.28.1
+      - python-requests/2.28.2
     method: GET
     uri: https://api.stlouisfed.org/fred/release/sources?file_type=json&release_id=10
   response:
     body:
       string: !!binary |
-        H4sIAAAAAAAEA6pWKkpNzCnJzE2NLy5JLCpRslIyMjAy0jU00DUyVNJByKbmpaDLFeeXFiWnFitZ
+        H4sIAAAAAAAEA6pWKkpNzCnJzE2NLy5JLCpRslIyMjAy1jUw0TUyV9JByKbmpaDLFeeXFiWnFitZ
         RVcrZaYoWRkZIakn2TTA8hJzU5WslEL1gvUUnEqLUhNLFfLTFHwSk/KLFIJLEksyi0syk4uVdJRy
-        MvOylayUMkpKCoqtYvRj9MvLy/WScor10vPLYvSVamNrAYt1tSfVAAAA
+        MvOylayUMkpKCoqtYvRj9MvLy/WScor10vPLYvSVamNrAV+oHQTVAAAA
     headers:
       Accept-Ranges:
       - bytes
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Length:
       - '156'
       Content-Type:
       - application/json; charset=UTF-8
       Date:
-      - Fri, 21 Oct 2022 15:15:02 GMT
+      - Fri, 28 Apr 2023 01:29:09 GMT
       ETag:
-      - W/"222ae02222ef6412ad99b94f9695cc94-gzip-gzip"
+      - W/"10494880d8d7a0e8d1a1912b3e61b973-gzip-gzip"
       Expires:
-      - Sat, 22 Oct 2022 15:15:02 GMT
+      - Sat, 29 Apr 2023 01:29:09 GMT
       Vary:
       - Accept-Encoding
       x-rate-limit-limit:
       - '120'
       x-rate-limit-remaining:
-      - '118'
+      - '102'
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `pyfredapi-0.6.0/tests/vhs/test_release/test_get_release_tables.yaml` & `pyfredapi-0.7.0/tests/vhs/test_release/test_get_release_tables.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -5,15 +5,15 @@
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python-requests/2.28.1
+      - python-requests/2.28.2
     method: GET
     uri: https://api.stlouisfed.org/fred/release/tables?file_type=json&release_id=10
   response:
     body:
       string: !!binary |
         H4sIAAAAAAAEA6pWKkrNSU0sTo3PTFGyUjI0UNJRSs1JzU3NKylWsqpWMjYxsTAEMaCCYGVgQR0U
         nYYGOkrFqUWZqcVgFXmlOTk6SgWJRal5JUgCOZl5qUpWEMmSyoJUJSul4tTkksz8PCUdpbzEXJCA
@@ -28,39 +28,39 @@
       Content-Encoding:
       - gzip
       Content-Length:
       - '235'
       Content-Type:
       - application/json; charset=UTF-8
       Date:
-      - Fri, 21 Oct 2022 15:15:02 GMT
+      - Thu, 27 Apr 2023 14:58:46 GMT
       ETag:
-      - '"3859ca83e63a083196ab4d648b611413-gzip"'
+      - W/"41a552fce265eaa06652862f2265d36a-gzip-gzip"
       Expires:
-      - Fri, 21 Oct 2022 15:25:02 GMT
+      - Thu, 27 Apr 2023 15:08:46 GMT
       Vary:
       - Accept-Encoding
       x-rate-limit-limit:
       - '120'
       x-rate-limit-remaining:
-      - '116'
+      - '78'
     status:
       code: 200
       message: OK
 - request:
     body: null
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python-requests/2.28.1
+      - python-requests/2.28.2
     method: GET
     uri: https://api.stlouisfed.org/fred/release/tables?file_type=json&release_id=10
   response:
     body:
       string: !!binary |
         H4sIAAAAAAAEA6pWKkrNSU0sTo3PTFGyUjI0UNJRSs1JzU3NKylWsqpWMjYxsTAEMaCCYGVgQR0U
         nYYGOkrFqUWZqcVgFXmlOTk6SgWJRal5JUgCOZl5qUpWEMmSyoJUJSul4tTkksz8PCUdpbzEXJCA
@@ -75,22 +75,116 @@
       Content-Encoding:
       - gzip
       Content-Length:
       - '235'
       Content-Type:
       - application/json; charset=UTF-8
       Date:
-      - Fri, 21 Oct 2022 15:15:03 GMT
+      - Thu, 27 Apr 2023 14:58:46 GMT
       ETag:
-      - W/"3859ca83e63a083196ab4d648b611413-gzip-gzip"
+      - W/"41a552fce265eaa06652862f2265d36a-gzip-gzip"
       Expires:
-      - Fri, 21 Oct 2022 15:25:02 GMT
+      - Thu, 27 Apr 2023 15:08:46 GMT
       Vary:
       - Accept-Encoding
       x-rate-limit-limit:
       - '120'
       x-rate-limit-remaining:
-      - '115'
+      - '77'
+    status:
+      code: 200
+      message: OK
+- request:
+    body: null
+    headers:
+      Accept:
+      - '*/*'
+      Accept-Encoding:
+      - gzip, deflate
+      Connection:
+      - keep-alive
+      User-Agent:
+      - python-requests/2.28.2
+    method: GET
+    uri: https://api.stlouisfed.org/fred/release/tables?file_type=json&release_id=10
+  response:
+    body:
+      string: !!binary |
+        H4sIAAAAAAAEA6pWKkrNSU0sTo3PTFGyUjI0UNJRSs1JzU3NKylWsqpWMjYxsTAEMaCCYGVgQR0U
+        nYYGOkrFqUWZqcVgFXmlOTk6SgWJRal5JUgCOZl5qUpWEMmSyoJUJSul4tTkksz8PCUdpbzEXJCA
+        c35ecWluapFCQFFmcqqCZ15KaoVCUqWCa0VBal5KZklpUaqCc2JJanp+UaWSjlJOallqjpKVEsjh
+        yRmZOSlFqXlKVtGxtTpKxmbmhkYYbgcJ0tXtwQWpyZmJOQqO6elFqemJJWA/ZSanFuNzPWC1tQDh
+        cBummgEAAA==
+    headers:
+      Accept-Ranges:
+      - bytes
+      Connection:
+      - keep-alive
+      Content-Encoding:
+      - gzip
+      Content-Length:
+      - '235'
+      Content-Type:
+      - application/json; charset=UTF-8
+      Date:
+      - Fri, 28 Apr 2023 01:29:12 GMT
+      ETag:
+      - '"3f2ee28961b077794aa9225a89111994-gzip"'
+      Expires:
+      - Fri, 28 Apr 2023 01:39:12 GMT
+      Vary:
+      - Accept-Encoding
+      x-rate-limit-limit:
+      - '120'
+      x-rate-limit-remaining:
+      - '96'
+    status:
+      code: 200
+      message: OK
+- request:
+    body: null
+    headers:
+      Accept:
+      - '*/*'
+      Accept-Encoding:
+      - gzip, deflate
+      Connection:
+      - keep-alive
+      User-Agent:
+      - python-requests/2.28.2
+    method: GET
+    uri: https://api.stlouisfed.org/fred/release/tables?file_type=json&release_id=10
+  response:
+    body:
+      string: !!binary |
+        H4sIAAAAAAAEA6pWKkrNSU0sTo3PTFGyUjI0UNJRSs1JzU3NKylWsqpWMjYxsTAEMaCCYGVgQR0U
+        nYYGOkrFqUWZqcVgFXmlOTk6SgWJRal5JUgCOZl5qUpWEMmSyoJUJSul4tTkksz8PCUdpbzEXJCA
+        c35ecWluapFCQFFmcqqCZ15KaoVCUqWCa0VBal5KZklpUaqCc2JJanp+UaWSjlJOallqjpKVEsjh
+        yRmZOSlFqXlKVtGxtTpKxmbmhkYYbgcJ0tXtwQWpyZmJOQqO6elFqemJJWA/ZSanFuNzPWC1tQDh
+        cBummgEAAA==
+    headers:
+      Accept-Ranges:
+      - bytes
+      Connection:
+      - keep-alive
+      Content-Encoding:
+      - gzip
+      Content-Length:
+      - '235'
+      Content-Type:
+      - application/json; charset=UTF-8
+      Date:
+      - Fri, 28 Apr 2023 01:29:12 GMT
+      ETag:
+      - W/"3f2ee28961b077794aa9225a89111994-gzip-gzip"
+      Expires:
+      - Fri, 28 Apr 2023 01:39:12 GMT
+      Vary:
+      - Accept-Encoding
+      x-rate-limit-limit:
+      - '120'
+      x-rate-limit-remaining:
+      - '95'
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `pyfredapi-0.6.0/tests/vhs/test_series/test_get_series_all_releases[json].yaml` & `pyfredapi-0.7.0/tests/vhs/test_series/test_get_series_all_releases[pandas].yaml`

 * *Files 2% similar despite different names*

```diff
@@ -5,24 +5,24 @@
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python-requests/2.28.1
+      - python-requests/2.28.2
     method: GET
     uri: https://api.stlouisfed.org/fred/series/observations?file_type=json&realtime_end=9999-12-31&realtime_start=1776-07-04&series_id=GDP
   response:
     body:
       string: !!binary |
         H4sIAAAAAAAEA6pWKkpNzCnJzE2NLy5JLCpRslIyNDc30zUw1zUwUdJByKbmpShZKVlaWlrqGhrp
         Ghsq6SjlJxWnFpUllmTm5yE0mxkY6BoY6hqgK8CivzQvs6RYyUopJzMPZFppSUFpSXxJZUGqkpWh
         jlJaZk4qlKeUVZwPVlKUkloUn1SpZIVid0piSaqSjlJxflFJfD5IiZKVUmJxspKOUnJ+aV6JkpWx
-        gaWFjlJ+WlpxaomSlYGOUk5mbmaJkpWhAQigeKRYySoaW5hYWhqB/G1khBkmhpaWZiAvG1oo6SiB
+        oYGpjlJ+WlpxaomSlYGOUk5mbmaJkpWhAQigeKRYySoaW5hYWhqB/G1khBkmhpaWZiAvG1oo6SiB
         3WKlZGhpAhYDB0NZYk5pKihgLS31zJVqdbCbD1ZvaInVfHNdA1NdAzMC5uvhNBui3xyr2Za6hga6
         RiA5fG43MjTQM8FpPsQMkP/hqQlLfOMzH7fbyQh3E0jyg4W7kYE5dcMdzXzcbicj3NHMNjK00DOl
         ZrijmY/b7WSEuzlauBua61nidDsZ6R3NfNxuJyPc0cw2MrLQM8PpdjLSO5r5uN1OergbgkpcJR0l
         eHo3MtIzwul20sMd3Xzcbic93NHNNjI20rPA6XbSwx3dfNxuJzXcQRGKlt6NzKhYzmCaj9vtpIY7
         ptlGxubklO9GBqDq3kTXCLVuwjQfh9vh+kH1D1rdYWRgYAyqcw1AdSKi7sA0G+R2HGUkzAxDA8y6
         z8jA0BjUzjEGyREyH0d+gpsBau5guN/QHFy3EgobIxNjPUPsad7IAGoG1vAxtAC5n2DYg8w3wJGp
         jAyghmCxAKWxhzeAQB4ww908ICNroVVTRsYGeIpjUos0UNsWNeviSJ6GlpZkZC10t5sY4KkGcRZp
@@ -705,115 +705,64 @@
         zAz1DPCMkBmC2wygtIPVDow4x2WHKTl7S7E3E0HlC8gapMVERkYGxhZ6Rka444PEZiJWO4wNjcm6
         wtrIAGScBdpABkgMrfowMjI3MtIzxX0cLUgPtFmANTowqnPM2+mNjMyNQU0fvEUJzuocEoyoRTtW
         O0wM9CzxNEsg5mCpBrH3BkH+Rg8rYwMTMz1L3HM4RuC7irGv/wbJoZ8EArIDvWg3NjQ31jPBvc4H
         ag6u7IFZ1YKLN9RBBmNDC3M9AxPczUQ8N+1DizKM+MDwh5GBkZ6xCe7uBxnxgWGHqamBHh5vgC+Y
         xX77OsgbRpilFUapa2xpaaRnjHuNNtQc7NGBuDkduUTEsMPEwMBCz8Qcd3SAzcHRaocEI3p0YLPD
         SM8Cz0IGiDmkZA9MO4xNQAMAOMdEQWGFa7c9SM4UvbgCxx9q0jUxtjDSM8OzkwR8MbcRaCwPs7gy
         AtcsqGGF3Q4TPSPcR7SA3GqGq6aFhCMxdoBa7dTLHtj8YW5ioId7SBTkDWhlijWoLNAHAIxAYxJo
-        0WFhaqhngaejBrlNGXsDDkdQoZe6JhYWRnoW5lQbPgb5G90OUyMTUBYEzEypNrYWAB4R3V0fmAQA
+        0WFhaqhngaejBrlNGXsDDkdQoZe6JhYWRnoW5lQbPgb5G90OUyMTUBbEV5mDOlFYp6KMjMCdKFDW
+        QWRzzKtdjUzNzIwJJCtDnGOJRuDOD2onCqsdlhZ4TrMBORV6AjRalOOoBLFZYW5krGeJexOUEfhe
+        Nhw5EHJpKagPhxxUGCWJmaGxEd4hOIg5xtgOowPZbwzJnQTsMDHRszTFHeXGoD4MtlIXZ1hh84e5
+        niWe9THgG7uw1VA47ACHLWoWBMzMxMxUz8LMVKk2thYAqbiVfdqaBAA=
     headers:
       Accept-Ranges:
       - bytes
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Length:
-      - '39615'
+      - '39770'
       Content-Type:
       - application/json; charset=UTF-8
       Date:
-      - Fri, 21 Oct 2022 14:44:51 GMT
+      - Thu, 27 Apr 2023 14:58:59 GMT
       Expires:
-      - Fri, 21 Oct 2022 14:45:51 GMT
+      - Thu, 27 Apr 2023 14:59:58 GMT
       Last-Modified:
-      - Thu, 29 Sep 2022 12:46:02 GMT
+      - Thu, 27 Apr 2023 12:53:02 GMT
       Vary:
       - Accept-Encoding
       x-rate-limit-limit:
       - '120'
       x-rate-limit-remaining:
-      - '73'
+      - '52'
     status:
       code: 200
       message: OK
 - request:
     body: null
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python-requests/2.28.1
-    method: GET
-    uri: https://api.stlouisfed.org/fred/series?file_type=json&series_id=GDP
-  response:
-    body:
-      string: !!binary |
-        H4sIAAAAAAAEA6pWKkpNzCnJzE2NLy5JLCpRslIyMjAy0jU00DUyVNJByKbmpaDLFacWZaYWFytZ
-        RVcrZYJk3V0CkLWQbGBJZklOqpKVkntRfnGxgkt+bmpxSWayQkBRfkppcomSjlJ+UnFqUVliSWZ+
-        Hty5hpYm5roGhroGIOciK0BysYEJRDqtKLWwNDUvuVLJSimwNLGoJLUop1JJRwkuHl+ckQ8OhEAl
-        HaXSvMySYiUrJafMnJzM/Lxihfw0BZf8nJzEomKYLFy9U2aOHkheRUlHqTg1sTg/LzEnPjElq7S4
-        JDc1DxSswVDRnEoFR7B4aoqCY15eaWKOQlBiSSp2fXDzgx0dg5R0lHISi0viSwtSEktSQQEOjioD
-        S10jSwUDcysTMysDI10DUyUdpYL8gtKcxKLMkkolK0tjHaW8/JJUsFdcHRUck5PzS/NKFJzzU1Kt
-        FBwNLQ2DnGPyYvIgoZ4CC/UCSKgraLi7BGjqKJRkpCqkpSaWlBalpijkpiYWlxalgjwcqhesp5Bf
-        WlJQWqKjkFkMVpebWJSdWqJQlphTClYD0puen59SrJCYl6IAisLM5NRiBYgNqSkKSZUKOYlJ+UVg
-        6YKi/ILUopJKhZz8ZJA3FTLzwIaG5mWWpKYoBJcklqQW67nlFynk5helKmTmpeUX5YKThI5CcWoq
-        WK17aWZKqkJJPpjjB5ZMzFHwzEvOz00FWwJNUrCwAEctyJUoliho+HkGOGqCNYAknUqLUhNLQZ52
-        Tc7Py8/NTFZwzEvMqSzOLFbQyCgpKbCK0Y/RLy8v10tKTdRLzy+L0c+D2g1YjH5BSlqMfl5mQWJ6
-        aWaKXkFKmqaeUm1sLQCTEdb/gAMAAA==
-    headers:
-      Accept-Ranges:
-      - bytes
-      Connection:
-      - keep-alive
-      Content-Encoding:
-      - gzip
-      Content-Length:
-      - '649'
-      Content-Type:
-      - application/json; charset=UTF-8
-      Date:
-      - Fri, 21 Oct 2022 14:44:52 GMT
-      Expires:
-      - Fri, 21 Oct 2022 14:45:52 GMT
-      Last-Modified:
-      - Thu, 29 Sep 2022 12:46:02 GMT
-      Vary:
-      - Accept-Encoding
-      x-rate-limit-limit:
-      - '120'
-      x-rate-limit-remaining:
-      - '72'
-    status:
-      code: 200
-      message: OK
-- request:
-    body: null
-    headers:
-      Accept:
-      - '*/*'
-      Accept-Encoding:
-      - gzip, deflate
-      Connection:
-      - keep-alive
-      User-Agent:
-      - python-requests/2.28.1
+      - python-requests/2.28.2
     method: GET
     uri: https://api.stlouisfed.org/fred/series/observations?file_type=json&realtime_end=9999-12-31&realtime_start=1776-07-04&series_id=GDP
   response:
     body:
       string: !!binary |
         H4sIAAAAAAAEA6pWKkpNzCnJzE2NLy5JLCpRslIyNDc30zUw1zUwUdJByKbmpShZKVlaWlrqGhrp
         Ghsq6SjlJxWnFpUllmTm5yE0mxkY6BoY6hqgK8CivzQvs6RYyUopJzMPZFppSUFpSXxJZUGqkpWh
         jlJaZk4qlKeUVZwPVlKUkloUn1SpZIVid0piSaqSjlJxflFJfD5IiZKVUmJxspKOUnJ+aV6JkpWx
-        gaWFjlJ+WlpxaomSlYGOUk5mbmaJkpWhAQigeKRYySoaW5hYWhqB/G1khBkmhpaWZiAvG1oo6SiB
+        oYGpjlJ+WlpxaomSlYGOUk5mbmaJkpWhAQigeKRYySoaW5hYWhqB/G1khBkmhpaWZiAvG1oo6SiB
         3WKlZGhpAhYDB0NZYk5pKihgLS31zJVqdbCbD1ZvaInVfHNdA1NdAzMC5uvhNBui3xyr2Za6hga6
         RiA5fG43MjTQM8FpPsQMkP/hqQlLfOMzH7fbyQh3E0jyg4W7kYE5dcMdzXzcbicj3NHMNjK00DOl
         ZrijmY/b7WSEuzlauBua61nidDsZ6R3NfNxuJyPc0cw2MrLQM8PpdjLSO5r5uN1OergbgkpcJR0l
         eHo3MtIzwul20sMd3Xzcbic93NHNNjI20rPA6XbSwx3dfNxuJzXcQRGKlt6NzKhYzmCaj9vtpIY7
         ptlGxubklO9GBqDq3kTXCLVuwjQfh9vh+kH1D1rdYWRgYAyqcw1AdSKi7sA0G+R2HGUkzAxDA8y6
         z8jA0BjUzjEGyREyH0d+gpsBau5guN/QHFy3EgobIxNjPUPsad7IAGoG1vAxtAC5n2DYg8w3wJGp
         jAyghmCxAKWxhzeAQB4ww908ICNroVVTRsYGeIpjUos0UNsWNeviSJ6GlpZkZC10t5sY4KkGcRZp
@@ -1496,35 +1445,38 @@
         zAz1DPCMkBmC2wygtIPVDow4x2WHKTl7S7E3E0HlC8gapMVERkYGxhZ6Rka444PEZiJWO4wNjcm6
         wtrIAGScBdpABkgMrfowMjI3MtIzxX0cLUgPtFmANTowqnPM2+mNjMyNQU0fvEUJzuocEoyoRTtW
         O0wM9CzxNEsg5mCpBrH3BkH+Rg8rYwMTMz1L3HM4RuC7irGv/wbJoZ8EArIDvWg3NjQ31jPBvc4H
         ag6u7IFZ1YKLN9RBBmNDC3M9AxPczUQ8N+1DizKM+MDwh5GBkZ6xCe7uBxnxgWGHqamBHh5vgC+Y
         xX77OsgbRpilFUapa2xpaaRnjHuNNtQc7NGBuDkduUTEsMPEwMBCz8Qcd3SAzcHRaocEI3p0YLPD
         SM8Cz0IGiDmkZA9MO4xNQAMAOMdEQWGFa7c9SM4UvbgCxx9q0jUxtjDSM8OzkwR8MbcRaCwPs7gy
         AtcsqGGF3Q4TPSPcR7SA3GqGq6aFhCMxdoBa7dTLHtj8YW5ioId7SBTkDWhlijWoLNAHAIxAYxJo
-        0WFhaqhngaejBrlNGXsDDkdQoZe6JhYWRnoW5lQbPgb5G90OUyMTUBYEzEypNrYWAB4R3V0fmAQA
+        0WFhaqhngaejBrlNGXsDDkdQoZe6JhYWRnoW5lQbPgb5G90OUyMTUBbEV5mDOlFYp6KMjMCdKFDW
+        QWRzzKtdjUzNzIwJJCtDnGOJRuDOD2onCqsdlhZ4TrMBORV6AjRalOOoBLFZYW5krGeJexOUEfhe
+        Nhw5EHJpKagPhxxUGCWJmaGxEd4hOIg5xtgOowPZbwzJnQTsMDHRszTFHeXGoD4MtlIXZ1hh84e5
+        niWe9THgG7uw1VA47ACHLWoWBMzMxMxUz8LMVKk2thYAqbiVfdqaBAA=
     headers:
       Accept-Ranges:
       - bytes
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Length:
-      - '39615'
+      - '39770'
       Content-Type:
       - application/json; charset=UTF-8
       Date:
-      - Fri, 21 Oct 2022 14:44:52 GMT
+      - Fri, 28 Apr 2023 01:29:26 GMT
       Expires:
-      - Fri, 21 Oct 2022 14:45:52 GMT
+      - Fri, 28 Apr 2023 01:30:25 GMT
       Last-Modified:
-      - Thu, 29 Sep 2022 12:46:02 GMT
+      - Thu, 27 Apr 2023 12:53:02 GMT
       Vary:
       - Accept-Encoding
       x-rate-limit-limit:
       - '120'
       x-rate-limit-remaining:
-      - '71'
+      - '70'
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `pyfredapi-0.6.0/tests/vhs/test_series/test_get_series_all_releases[pandas].yaml` & `pyfredapi-0.7.0/tests/vhs/test_series/test_get_series_all_releases[json].yaml`

 * *Files 24% similar despite different names*

```diff
@@ -5,24 +5,24 @@
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python-requests/2.28.1
+      - python-requests/2.28.2
     method: GET
     uri: https://api.stlouisfed.org/fred/series/observations?file_type=json&realtime_end=9999-12-31&realtime_start=1776-07-04&series_id=GDP
   response:
     body:
       string: !!binary |
         H4sIAAAAAAAEA6pWKkpNzCnJzE2NLy5JLCpRslIyNDc30zUw1zUwUdJByKbmpShZKVlaWlrqGhrp
         Ghsq6SjlJxWnFpUllmTm5yE0mxkY6BoY6hqgK8CivzQvs6RYyUopJzMPZFppSUFpSXxJZUGqkpWh
         jlJaZk4qlKeUVZwPVlKUkloUn1SpZIVid0piSaqSjlJxflFJfD5IiZKVUmJxspKOUnJ+aV6JkpWx
-        gaWFjlJ+WlpxaomSlYGOUk5mbmaJkpWhAQigeKRYySoaW5hYWhqB/G1khBkmhpaWZiAvG1oo6SiB
+        oYGpjlJ+WlpxaomSlYGOUk5mbmaJkpWhAQigeKRYySoaW5hYWhqB/G1khBkmhpaWZiAvG1oo6SiB
         3WKlZGhpAhYDB0NZYk5pKihgLS31zJVqdbCbD1ZvaInVfHNdA1NdAzMC5uvhNBui3xyr2Za6hga6
         RiA5fG43MjTQM8FpPsQMkP/hqQlLfOMzH7fbyQh3E0jyg4W7kYE5dcMdzXzcbicj3NHMNjK00DOl
         ZrijmY/b7WSEuzlauBua61nidDsZ6R3NfNxuJyPc0cw2MrLQM8PpdjLSO5r5uN1OergbgkpcJR0l
         eHo3MtIzwul20sMd3Xzcbic93NHNNjI20rPA6XbSwx3dfNxuJzXcQRGKlt6NzKhYzmCaj9vtpIY7
         ptlGxubklO9GBqDq3kTXCLVuwjQfh9vh+kH1D1rdYWRgYAyqcw1AdSKi7sA0G+R2HGUkzAxDA8y6
         z8jA0BjUzjEGyREyH0d+gpsBau5guN/QHFy3EgobIxNjPUPsad7IAGoG1vAxtAC5n2DYg8w3wJGp
         jAyghmCxAKWxhzeAQB4ww908ICNroVVTRsYGeIpjUos0UNsWNeviSJ6GlpZkZC10t5sY4KkGcRZp
@@ -705,115 +705,1544 @@
         zAz1DPCMkBmC2wygtIPVDow4x2WHKTl7S7E3E0HlC8gapMVERkYGxhZ6Rka444PEZiJWO4wNjcm6
         wtrIAGScBdpABkgMrfowMjI3MtIzxX0cLUgPtFmANTowqnPM2+mNjMyNQU0fvEUJzuocEoyoRTtW
         O0wM9CzxNEsg5mCpBrH3BkH+Rg8rYwMTMz1L3HM4RuC7irGv/wbJoZ8EArIDvWg3NjQ31jPBvc4H
         ag6u7IFZ1YKLN9RBBmNDC3M9AxPczUQ8N+1DizKM+MDwh5GBkZ6xCe7uBxnxgWGHqamBHh5vgC+Y
         xX77OsgbRpilFUapa2xpaaRnjHuNNtQc7NGBuDkduUTEsMPEwMBCz8Qcd3SAzcHRaocEI3p0YLPD
         SM8Cz0IGiDmkZA9MO4xNQAMAOMdEQWGFa7c9SM4UvbgCxx9q0jUxtjDSM8OzkwR8MbcRaCwPs7gy
         AtcsqGGF3Q4TPSPcR7SA3GqGq6aFhCMxdoBa7dTLHtj8YW5ioId7SBTkDWhlijWoLNAHAIxAYxJo
-        0WFhaqhngaejBrlNGXsDDkdQoZe6JhYWRnoW5lQbPgb5G90OUyMTUBYEzEypNrYWAB4R3V0fmAQA
+        0WFhaqhngaejBrlNGXsDDkdQoZe6JhYWRnoW5lQbPgb5G90OUyMTUBbEV5mDOlFYp6KMjMCdKFDW
+        QWRzzKtdjUzNzIwJJCtDnGOJRuDOD2onCqsdlhZ4TrMBORV6AjRalOOoBLFZYW5krGeJexOUEfhe
+        Nhw5EHJpKagPhxxUGCWJmaGxEd4hOIg5xtgOowPZbwzJnQTsMDHRszTFHeXGoD4MtlIXZ1hh84e5
+        niWe9THgG7uw1VA47ACHLWoWBMzMxMxUz8LMVKk2thYAqbiVfdqaBAA=
     headers:
       Accept-Ranges:
       - bytes
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Length:
-      - '39615'
+      - '39770'
       Content-Type:
       - application/json; charset=UTF-8
       Date:
-      - Fri, 21 Oct 2022 14:44:53 GMT
+      - Thu, 27 Apr 2023 14:58:57 GMT
       Expires:
-      - Fri, 21 Oct 2022 14:45:53 GMT
+      - Thu, 27 Apr 2023 14:59:57 GMT
       Last-Modified:
-      - Thu, 29 Sep 2022 12:46:02 GMT
+      - Thu, 27 Apr 2023 12:53:02 GMT
       Vary:
       - Accept-Encoding
       x-rate-limit-limit:
       - '120'
       x-rate-limit-remaining:
-      - '70'
+      - '54'
     status:
       code: 200
       message: OK
 - request:
     body: null
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python-requests/2.28.1
+      - python-requests/2.28.2
     method: GET
-    uri: https://api.stlouisfed.org/fred/series?file_type=json&series_id=GDP
+    uri: https://api.stlouisfed.org/fred/series/observations?file_type=json&realtime_end=9999-12-31&realtime_start=1776-07-04&series_id=GDP
   response:
     body:
       string: !!binary |
-        H4sIAAAAAAAEA6pWKkpNzCnJzE2NLy5JLCpRslIyMjAy0jU00DUyVNJByKbmpaDLFacWZaYWFytZ
-        RVcrZYJk3V0CkLWQbGBJZklOqpKVkntRfnGxgkt+bmpxSWayQkBRfkppcomSjlJ+UnFqUVliSWZ+
-        Hty5hpYm5roGhroGIOciK0BysYEJRDqtKLWwNDUvuVLJSimwNLGoJLUop1JJRwkuHl+ckQ8OhEAl
-        HaXSvMySYiUrJafMnJzM/Lxihfw0BZf8nJzEomKYLFy9U2aOHkheRUlHqTg1sTg/LzEnPjElq7S4
-        JDc1DxSswVDRnEoFR7B4aoqCY15eaWKOQlBiSSp2fXDzgx0dg5R0lHISi0viSwtSEktSQQEOjioD
-        S10jSwUDcysTMysDI10DUyUdpYL8gtKcxKLMkkolK0tjHaW8/JJUsFdcHRUck5PzS/NKFJzzU1Kt
-        FBwNLQ2DnGPyYvIgoZ4CC/UCSKgraLi7BGjqKJRkpCqkpSaWlBalpijkpiYWlxalgjwcqhesp5Bf
-        WlJQWqKjkFkMVpebWJSdWqJQlphTClYD0puen59SrJCYl6IAisLM5NRiBYgNqSkKSZUKOYlJ+UVg
-        6YKi/ILUopJKhZz8ZJA3FTLzwIaG5mWWpKYoBJcklqQW67nlFynk5helKmTmpeUX5YKThI5CcWoq
-        WK17aWZKqkJJPpjjB5ZMzFHwzEvOz00FWwJNUrCwAEctyJUoliho+HkGOGqCNYAknUqLUhNLQZ52
-        Tc7Py8/NTFZwzEvMqSzOLFbQyCgpKbCK0Y/RLy8v10tKTdRLzy+L0c+D2g1YjH5BSlqMfl5mQWJ6
-        aWaKXkFKmqaeUm1sLQCTEdb/gAMAAA==
+        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
+    headers:
+      Accept-Ranges:
+      - bytes
+      Connection:
+      - keep-alive
+      Content-Encoding:
+      - gzip
+      Content-Length:
+      - '39770'
+      Content-Type:
+      - application/json; charset=UTF-8
+      Date:
+      - Thu, 27 Apr 2023 14:58:58 GMT
+      Expires:
+      - Thu, 27 Apr 2023 14:59:58 GMT
+      Last-Modified:
+      - Thu, 27 Apr 2023 12:53:02 GMT
+      Vary:
+      - Accept-Encoding
+      x-rate-limit-limit:
+      - '120'
+      x-rate-limit-remaining:
+      - '53'
+    status:
+      code: 200
+      message: OK
+- request:
+    body: null
+    headers:
+      Accept:
+      - '*/*'
+      Accept-Encoding:
+      - gzip, deflate
+      Connection:
+      - keep-alive
+      User-Agent:
+      - python-requests/2.28.2
+    method: GET
+    uri: https://api.stlouisfed.org/fred/series/observations?file_type=json&realtime_end=9999-12-31&realtime_start=1776-07-04&series_id=GDP
+  response:
+    body:
+      string: !!binary |
+        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
     headers:
       Accept-Ranges:
       - bytes
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Length:
-      - '649'
+      - '39770'
       Content-Type:
       - application/json; charset=UTF-8
       Date:
-      - Fri, 21 Oct 2022 14:44:53 GMT
+      - Fri, 28 Apr 2023 01:29:24 GMT
       Expires:
-      - Fri, 21 Oct 2022 14:45:53 GMT
+      - Fri, 28 Apr 2023 01:30:24 GMT
       Last-Modified:
-      - Thu, 29 Sep 2022 12:46:02 GMT
+      - Thu, 27 Apr 2023 12:53:02 GMT
       Vary:
       - Accept-Encoding
       x-rate-limit-limit:
       - '120'
       x-rate-limit-remaining:
-      - '69'
+      - '72'
     status:
       code: 200
       message: OK
 - request:
     body: null
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python-requests/2.28.1
+      - python-requests/2.28.2
     method: GET
     uri: https://api.stlouisfed.org/fred/series/observations?file_type=json&realtime_end=9999-12-31&realtime_start=1776-07-04&series_id=GDP
   response:
     body:
       string: !!binary |
         H4sIAAAAAAAEA6pWKkpNzCnJzE2NLy5JLCpRslIyNDc30zUw1zUwUdJByKbmpShZKVlaWlrqGhrp
         Ghsq6SjlJxWnFpUllmTm5yE0mxkY6BoY6hqgK8CivzQvs6RYyUopJzMPZFppSUFpSXxJZUGqkpWh
         jlJaZk4qlKeUVZwPVlKUkloUn1SpZIVid0piSaqSjlJxflFJfD5IiZKVUmJxspKOUnJ+aV6JkpWx
-        gaWFjlJ+WlpxaomSlYGOUk5mbmaJkpWhAQigeKRYySoaW5hYWhqB/G1khBkmhpaWZiAvG1oo6SiB
+        oYGpjlJ+WlpxaomSlYGOUk5mbmaJkpWhAQigeKRYySoaW5hYWhqB/G1khBkmhpaWZiAvG1oo6SiB
         3WKlZGhpAhYDB0NZYk5pKihgLS31zJVqdbCbD1ZvaInVfHNdA1NdAzMC5uvhNBui3xyr2Za6hga6
         RiA5fG43MjTQM8FpPsQMkP/hqQlLfOMzH7fbyQh3E0jyg4W7kYE5dcMdzXzcbicj3NHMNjK00DOl
         ZrijmY/b7WSEuzlauBua61nidDsZ6R3NfNxuJyPc0cw2MrLQM8PpdjLSO5r5uN1OergbgkpcJR0l
         eHo3MtIzwul20sMd3Xzcbic93NHNNjI20rPA6XbSwx3dfNxuJzXcQRGKlt6NzKhYzmCaj9vtpIY7
         ptlGxubklO9GBqDq3kTXCLVuwjQfh9vh+kH1D1rdYWRgYAyqcw1AdSKi7sA0G+R2HGUkzAxDA8y6
         z8jA0BjUzjEGyREyH0d+gpsBau5guN/QHFy3EgobIxNjPUPsad7IAGoG1vAxtAC5n2DYg8w3wJGp
         jAyghmCxAKWxhzeAQB4ww908ICNroVVTRsYGeIpjUos0UNsWNeviSJ6GlpZkZC10t5sY4KkGcRZp
@@ -1496,35 +2925,38 @@
         zAz1DPCMkBmC2wygtIPVDow4x2WHKTl7S7E3E0HlC8gapMVERkYGxhZ6Rka444PEZiJWO4wNjcm6
         wtrIAGScBdpABkgMrfowMjI3MtIzxX0cLUgPtFmANTowqnPM2+mNjMyNQU0fvEUJzuocEoyoRTtW
         O0wM9CzxNEsg5mCpBrH3BkH+Rg8rYwMTMz1L3HM4RuC7irGv/wbJoZ8EArIDvWg3NjQ31jPBvc4H
         ag6u7IFZ1YKLN9RBBmNDC3M9AxPczUQ8N+1DizKM+MDwh5GBkZ6xCe7uBxnxgWGHqamBHh5vgC+Y
         xX77OsgbRpilFUapa2xpaaRnjHuNNtQc7NGBuDkduUTEsMPEwMBCz8Qcd3SAzcHRaocEI3p0YLPD
         SM8Cz0IGiDmkZA9MO4xNQAMAOMdEQWGFa7c9SM4UvbgCxx9q0jUxtjDSM8OzkwR8MbcRaCwPs7gy
         AtcsqGGF3Q4TPSPcR7SA3GqGq6aFhCMxdoBa7dTLHtj8YW5ioId7SBTkDWhlijWoLNAHAIxAYxJo
-        0WFhaqhngaejBrlNGXsDDkdQoZe6JhYWRnoW5lQbPgb5G90OUyMTUBYEzEypNrYWAB4R3V0fmAQA
+        0WFhaqhngaejBrlNGXsDDkdQoZe6JhYWRnoW5lQbPgb5G90OUyMTUBbEV5mDOlFYp6KMjMCdKFDW
+        QWRzzKtdjUzNzIwJJCtDnGOJRuDOD2onCqsdlhZ4TrMBORV6AjRalOOoBLFZYW5krGeJexOUEfhe
+        Nhw5EHJpKagPhxxUGCWJmaGxEd4hOIg5xtgOowPZbwzJnQTsMDHRszTFHeXGoD4MtlIXZ1hh84e5
+        niWe9THgG7uw1VA47ACHLWoWBMzMxMxUz8LMVKk2thYAqbiVfdqaBAA=
     headers:
       Accept-Ranges:
       - bytes
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Length:
-      - '39615'
+      - '39770'
       Content-Type:
       - application/json; charset=UTF-8
       Date:
-      - Fri, 21 Oct 2022 14:44:54 GMT
+      - Fri, 28 Apr 2023 01:29:24 GMT
       Expires:
-      - Fri, 21 Oct 2022 14:45:54 GMT
+      - Fri, 28 Apr 2023 01:30:24 GMT
       Last-Modified:
-      - Thu, 29 Sep 2022 12:46:02 GMT
+      - Thu, 27 Apr 2023 12:53:02 GMT
       Vary:
       - Accept-Encoding
       x-rate-limit-limit:
       - '120'
       x-rate-limit-remaining:
-      - '68'
+      - '71'
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `pyfredapi-0.6.0/tests/vhs/test_series/test_get_series_asof_date[json].yaml` & `pyfredapi-0.7.0/tests/vhs/test_series/test_get_series_asof_date[pandas].yaml`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python-requests/2.28.1
+      - python-requests/2.28.2
     method: GET
     uri: https://api.stlouisfed.org/fred/series/observations?file_type=json&realtime_end=2019-01-01&realtime_start=1776-07-04&series_id=GDP
   response:
     body:
       string: !!binary |
         H4sIAAAAAAAEA6pWKkpNzCnJzE2NLy5JLCpRslIyNDc30zUw1zUwUdJByKbmpShZKRkZGFrqGhjq
         Ghgq6SjlJxWnFpUllmTm5yE0mxkYYFUA0W9paWmpa2ikawzSX5qXWVKsZKWUk5kHMq20pKC0JL6k
@@ -659,93 +659,39 @@
       Content-Encoding:
       - gzip
       Content-Length:
       - '36214'
       Content-Type:
       - application/json; charset=UTF-8
       Date:
-      - Fri, 21 Oct 2022 14:44:58 GMT
+      - Thu, 27 Apr 2023 14:59:04 GMT
       Expires:
-      - Fri, 21 Oct 2022 14:45:58 GMT
+      - Thu, 27 Apr 2023 15:00:04 GMT
       Last-Modified:
       - Mon, 07 Jan 2019 18:40:19 GMT
       Vary:
       - Accept-Encoding
       x-rate-limit-limit:
       - '120'
       x-rate-limit-remaining:
-      - '61'
+      - '116'
     status:
       code: 200
       message: OK
 - request:
     body: null
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python-requests/2.28.1
-    method: GET
-    uri: https://api.stlouisfed.org/fred/series?file_type=json&series_id=GDP
-  response:
-    body:
-      string: !!binary |
-        H4sIAAAAAAAEA6pWKkpNzCnJzE2NLy5JLCpRslIyMjAy0jU00DUyVNJByKbmpaDLFacWZaYWFytZ
-        RVcrZYJk3V0CkLWQbGBJZklOqpKVkntRfnGxgkt+bmpxSWayQkBRfkppcomSjlJ+UnFqUVliSWZ+
-        Hty5hpYm5roGhroGIOciK0BysYEJRDqtKLWwNDUvuVLJSimwNLGoJLUop1JJRwkuHl+ckQ8OhEAl
-        HaXSvMySYiUrJafMnJzM/Lxihfw0BZf8nJzEomKYLFy9U2aOHkheRUlHqTg1sTg/LzEnPjElq7S4
-        JDc1DxSswVDRnEoFR7B4aoqCY15eaWKOQlBiSSp2fXDzgx0dg5R0lHISi0viSwtSEktSQQEOjioD
-        S10jSwUDcysTMysDI10DUyUdpYL8gtKcxKLMkkolK0tjHaW8/JJUsFdcHRUck5PzS/NKFJzzU1Kt
-        FBwNLQ2DnGPyYvIgoZ4CC/UCSKgraLi7BGjqKJRkpCqkpSaWlBalpijkpiYWlxalgjwcqhesp5Bf
-        WlJQWqKjkFkMVpebWJSdWqJQlphTClYD0puen59SrJCYl6IAisLM5NRiBYgNqSkKSZUKOYlJ+UVg
-        6YKi/ILUopJKhZz8ZJA3FTLzwIaG5mWWpKYoBJcklqQW67nlFynk5helKmTmpeUX5YKThI5CcWoq
-        WK17aWZKqkJJPpjjB5ZMzFHwzEvOz00FWwJNUrCwAEctyJUoliho+HkGOGqCNYAknUqLUhNLQZ52
-        Tc7Py8/NTFZwzEvMqSzOLFbQyCgpKbCK0Y/RLy8v10tKTdRLzy+L0c+D2g1YjH5BSlqMfl5mQWJ6
-        aWaKXkFKmqaeUm1sLQCTEdb/gAMAAA==
-    headers:
-      Accept-Ranges:
-      - bytes
-      Connection:
-      - keep-alive
-      Content-Encoding:
-      - gzip
-      Content-Length:
-      - '649'
-      Content-Type:
-      - application/json; charset=UTF-8
-      Date:
-      - Fri, 21 Oct 2022 14:44:59 GMT
-      Expires:
-      - Fri, 21 Oct 2022 14:45:59 GMT
-      Last-Modified:
-      - Thu, 29 Sep 2022 12:46:02 GMT
-      Vary:
-      - Accept-Encoding
-      x-rate-limit-limit:
-      - '120'
-      x-rate-limit-remaining:
-      - '60'
-    status:
-      code: 200
-      message: OK
-- request:
-    body: null
-    headers:
-      Accept:
-      - '*/*'
-      Accept-Encoding:
-      - gzip, deflate
-      Connection:
-      - keep-alive
-      User-Agent:
-      - python-requests/2.28.1
+      - python-requests/2.28.2
     method: GET
     uri: https://api.stlouisfed.org/fred/series/observations?file_type=json&realtime_end=2019-01-01&realtime_start=1776-07-04&series_id=GDP
   response:
     body:
       string: !!binary |
         H4sIAAAAAAAEA6pWKkpNzCnJzE2NLy5JLCpRslIyNDc30zUw1zUwUdJByKbmpShZKRkZGFrqGhjq
         Ghgq6SjlJxWnFpUllmTm5yE0mxkYYFUA0W9paWmpa2ikawzSX5qXWVKsZKWUk5kHMq20pKC0JL6k
@@ -1391,22 +1337,22 @@
       Content-Encoding:
       - gzip
       Content-Length:
       - '36214'
       Content-Type:
       - application/json; charset=UTF-8
       Date:
-      - Fri, 21 Oct 2022 14:44:59 GMT
+      - Fri, 28 Apr 2023 01:29:31 GMT
       Expires:
-      - Fri, 21 Oct 2022 14:45:59 GMT
+      - Fri, 28 Apr 2023 01:30:31 GMT
       Last-Modified:
       - Mon, 07 Jan 2019 18:40:19 GMT
       Vary:
       - Accept-Encoding
       x-rate-limit-limit:
       - '120'
       x-rate-limit-remaining:
-      - '59'
+      - '64'
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `pyfredapi-0.6.0/tests/vhs/test_series/test_get_series_asof_date[pandas].yaml` & `pyfredapi-0.7.0/tests/vhs/test_series/test_get_series_asof_date[json].yaml`

 * *Files 25% similar despite different names*

```diff
@@ -5,15 +5,15 @@
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python-requests/2.28.1
+      - python-requests/2.28.2
     method: GET
     uri: https://api.stlouisfed.org/fred/series/observations?file_type=json&realtime_end=2019-01-01&realtime_start=1776-07-04&series_id=GDP
   response:
     body:
       string: !!binary |
         H4sIAAAAAAAEA6pWKkpNzCnJzE2NLy5JLCpRslIyNDc30zUw1zUwUdJByKbmpShZKRkZGFrqGhjq
         Ghgq6SjlJxWnFpUllmTm5yE0mxkYYFUA0W9paWmpa2ikawzSX5qXWVKsZKWUk5kHMq20pKC0JL6k
@@ -659,93 +659,1395 @@
       Content-Encoding:
       - gzip
       Content-Length:
       - '36214'
       Content-Type:
       - application/json; charset=UTF-8
       Date:
-      - Fri, 21 Oct 2022 14:45:00 GMT
+      - Thu, 27 Apr 2023 14:59:02 GMT
       Expires:
-      - Fri, 21 Oct 2022 14:46:00 GMT
+      - Thu, 27 Apr 2023 15:00:02 GMT
       Last-Modified:
       - Mon, 07 Jan 2019 18:40:19 GMT
       Vary:
       - Accept-Encoding
       x-rate-limit-limit:
       - '120'
       x-rate-limit-remaining:
+      - '118'
+    status:
+      code: 200
+      message: OK
+- request:
+    body: null
+    headers:
+      Accept:
+      - '*/*'
+      Accept-Encoding:
+      - gzip, deflate
+      Connection:
+      - keep-alive
+      User-Agent:
+      - python-requests/2.28.2
+    method: GET
+    uri: https://api.stlouisfed.org/fred/series/observations?file_type=json&realtime_end=2019-01-01&realtime_start=1776-07-04&series_id=GDP
+  response:
+    body:
+      string: !!binary |
+        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
+        s9AzMjBRqo2tBQA7ARwprUsEAA==
+    headers:
+      Accept-Ranges:
+      - bytes
+      Connection:
+      - keep-alive
+      Content-Encoding:
+      - gzip
+      Content-Length:
+      - '36214'
+      Content-Type:
+      - application/json; charset=UTF-8
+      Date:
+      - Thu, 27 Apr 2023 14:59:03 GMT
+      Expires:
+      - Thu, 27 Apr 2023 15:00:02 GMT
+      Last-Modified:
+      - Mon, 07 Jan 2019 18:40:19 GMT
+      Vary:
+      - Accept-Encoding
+      x-rate-limit-limit:
       - '120'
+      x-rate-limit-remaining:
+      - '117'
     status:
       code: 200
       message: OK
 - request:
     body: null
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python-requests/2.28.1
+      - python-requests/2.28.2
     method: GET
-    uri: https://api.stlouisfed.org/fred/series?file_type=json&series_id=GDP
+    uri: https://api.stlouisfed.org/fred/series/observations?file_type=json&realtime_end=2019-01-01&realtime_start=1776-07-04&series_id=GDP
   response:
     body:
       string: !!binary |
-        H4sIAAAAAAAEA6pWKkpNzCnJzE2NLy5JLCpRslIyMjAy0jU00DUyVNJByKbmpaDLFacWZaYWFytZ
-        RVcrZYJk3V0CkLWQbGBJZklOqpKVkntRfnGxgkt+bmpxSWayQkBRfkppcomSjlJ+UnFqUVliSWZ+
-        Hty5hpYm5roGhroGIOciK0BysYEJRDqtKLWwNDUvuVLJSimwNLGoJLUop1JJRwkuHl+ckQ8OhEAl
-        HaXSvMySYiUrJafMnJzM/Lxihfw0BZf8nJzEomKYLFy9U2aOHkheRUlHqTg1sTg/LzEnPjElq7S4
-        JDc1DxSswVDRnEoFR7B4aoqCY15eaWKOQlBiSSp2fXDzgx0dg5R0lHISi0viSwtSEktSQQEOjioD
-        S10jSwUDcysTMysDI10DUyUdpYL8gtKcxKLMkkolK0tjHaW8/JJUsFdcHRUck5PzS/NKFJzzU1Kt
-        FBwNLQ2DnGPyYvIgoZ4CC/UCSKgraLi7BGjqKJRkpCqkpSaWlBalpijkpiYWlxalgjwcqhesp5Bf
-        WlJQWqKjkFkMVpebWJSdWqJQlphTClYD0puen59SrJCYl6IAisLM5NRiBYgNqSkKSZUKOYlJ+UVg
-        6YKi/ILUopJKhZz8ZJA3FTLzwIaG5mWWpKYoBJcklqQW67nlFynk5helKmTmpeUX5YKThI5CcWoq
-        WK17aWZKqkJJPpjjB5ZMzFHwzEvOz00FWwJNUrCwAEctyJUoliho+HkGOGqCNYAknUqLUhNLQZ52
-        Tc7Py8/NTFZwzEvMqSzOLFbQyCgpKbCK0Y/RLy8v10tKTdRLzy+L0c+D2g1YjH5BSlqMfl5mQWJ6
-        aWaKXkFKmqaeUm1sLQCTEdb/gAMAAA==
+        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
+        s9AzMjBRqo2tBQA7ARwprUsEAA==
     headers:
       Accept-Ranges:
       - bytes
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Length:
-      - '649'
+      - '36214'
       Content-Type:
       - application/json; charset=UTF-8
       Date:
-      - Fri, 21 Oct 2022 14:45:01 GMT
+      - Fri, 28 Apr 2023 01:29:29 GMT
       Expires:
-      - Fri, 21 Oct 2022 14:46:01 GMT
+      - Fri, 28 Apr 2023 01:30:29 GMT
       Last-Modified:
-      - Thu, 29 Sep 2022 12:46:02 GMT
+      - Mon, 07 Jan 2019 18:40:19 GMT
       Vary:
       - Accept-Encoding
       x-rate-limit-limit:
       - '120'
       x-rate-limit-remaining:
-      - '119'
+      - '66'
     status:
       code: 200
       message: OK
 - request:
     body: null
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python-requests/2.28.1
+      - python-requests/2.28.2
     method: GET
     uri: https://api.stlouisfed.org/fred/series/observations?file_type=json&realtime_end=2019-01-01&realtime_start=1776-07-04&series_id=GDP
   response:
     body:
       string: !!binary |
         H4sIAAAAAAAEA6pWKkpNzCnJzE2NLy5JLCpRslIyNDc30zUw1zUwUdJByKbmpShZKRkZGFrqGhjq
         Ghgq6SjlJxWnFpUllmTm5yE0mxkYYFUA0W9paWmpa2ikawzSX5qXWVKsZKWUk5kHMq20pKC0JL6k
@@ -1391,22 +2693,22 @@
       Content-Encoding:
       - gzip
       Content-Length:
       - '36214'
       Content-Type:
       - application/json; charset=UTF-8
       Date:
-      - Fri, 21 Oct 2022 14:45:01 GMT
+      - Fri, 28 Apr 2023 01:29:30 GMT
       Expires:
-      - Fri, 21 Oct 2022 14:46:01 GMT
+      - Fri, 28 Apr 2023 01:30:30 GMT
       Last-Modified:
       - Mon, 07 Jan 2019 18:40:19 GMT
       Vary:
       - Accept-Encoding
       x-rate-limit-limit:
       - '120'
       x-rate-limit-remaining:
-      - '118'
+      - '65'
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `pyfredapi-0.6.0/tests/vhs/test_series/test_get_series_initial_release[json].yaml` & `pyfredapi-0.7.0/tests/vhs/test_series/test_get_series_initial_release[pandas].yaml`

 * *Files 18% similar despite different names*

```diff
@@ -5,24 +5,24 @@
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python-requests/2.28.1
+      - python-requests/2.28.2
     method: GET
     uri: https://api.stlouisfed.org/fred/series/observations?file_type=json&output_type=4&realtime_start=1776-07-04&series_id=GDP
   response:
     body:
       string: !!binary |
         H4sIAAAAAAAEA6pWKkpNzCnJzE2NLy5JLCpRslIyNDc30zUw1zUwUdJByKbmpShZKVlaWlrqGhrp
         Ghsq6SjlJxWnFpUllmTm5yE0mxkY6BoY6hqgK8CivzQvs6RYyUopJzMPZFppSUFpSXxJZUGqkpWJ
         jlJaZk4qlKeUVZwPVlKUkloUn1SpZIVid0piSaqSjlJxflFJfD5IiZKVUmJxspKOUnJ+aV6JkpWh
-        kbGOUn5aWnFqiZKVgY5STmZuJkjYAARQ/FGsZBWNLUgsLY1AvjKyxAwSQ7Ccka6RuZKOEtgpVkqG
+        kZmOUn5aWnFqiZKVgY5STmZuJkjYAARQ/FGsZBWNLUgsLY1AvjKyxAwSQ7Ccka6RuZKOEtgpVkqG
         lpaGuoaggFDSUSpLzClNVbJSMjU3NtMzU6rVwWmBia6RBS4LTCFyCAvADgIHM9wCCwNLPWN8Fpjr
         GhvgssBC18gMxQdGugYmkHhEWGBpjNcHhgaQYICnKUisg4PI0FDXCJSiUHxgjmaBpZm5niFOHxiD
         4wB7EBnrGhjpGpmi+QA9DswMzAz1LPFZYKKLI5KNdQ1MIb5D+ADsIJQ4MDM0tdCzwGeBOR4LLCDx
         g2IBWhyYGRmY4fUBKA5wBZGhIRYL0OLAzNjSDE8qAjkHkhQxI9kEHAcgy5F9gBEHpoYGeILIBJTs
         cOQDE3AcoCZTsINQ48DMwFLPBGccmIAKNxyRbKJrYIGeisAOQrPAAl8+MAFlfZw+AOUDUDGCCCKw
         g1AtMDc3xRPJpuB8ACpvMOPAFEscgB2EaoGFpSGejGaKJw5MQXEALkYQPgA7CNUCSwsj/D4wx5WK
         TMFxgBpEYAehWGBuYGiIJxWZguMAexCZgYLPEDWZmoISBaoFhobGekY4U5EZOJyNsZamZqDgAxuG
@@ -66,116 +66,63 @@
         HgK7CcUOIwMTUE1ngGMhi5GBIXg6GGdYgdpNqDURuKePZoeZqaWegRGOdXVGBoaQ3jPIrZjxYalr
         YAzJNYi8B3YTmh0WloZ6xma44wPck8XhD0jfGjU+MPvWRoYGZkZ6Zpa4SylwXxa3HRitJ7CbUP1h
         aGxsrmdhiWOJIDiscI5zGFqCyynUWhXsJjQ7TI1M9SwMccaHEah7gKMFBZJDn5EA2QvSgpQHjQzN
         jU30jMxwpl2QOSY4evEgOdS1lEYGIDG0OsPI0NTYXM8SZwMEpAVX5Q2SQ+9kg8RALTUkbxhamhhY
         6Jmb4gsq0DAsKOlgJF0jA3B0oDSjQHagFVdGhoag5qwxjkUuRgZGIH9DOkCYdhiCO3jodqBXHEaG
         JuaWeqa4syDIDpzRAZm6RklWIPUgZyGFlZGRgYmFngWe+AB3bbE3REDmoXe2QWJo8WFkZG5kpGdq
         gTMLGkG621iLEpCcoa4RSnMKZAd6fBgbmhvrmVjiTrrg7i32ot0I0uFGtwMjPowtLY30jE1xxzl4
-        whh7RQuyA70qB4mhx4eJsYWRnpkFzklskB5cazpAcuhrOkBi6PEBmImFqaGehYGlUm1sLRcXFwAZ
-        bKGfLzAAAA==
+        whh7RQuyA70qB4mhx4eJsYWRnpkFzklskB5cazpAcuhrOkBi6PFhYmFqqGdhgDt/QLrdoCoCM+0a
+        gfMHKO/Ai3aQHejxYWpmZqxnZIHbDnDHG3uxawSZyEYZ6jICuwm1SDQzNDbSMzHFWeyCzME+BIKy
+        5QHhD7Cb0OwAzMTMVM/CzFSpNraWi4sLAPX5MHxbMQAA
     headers:
       Accept-Ranges:
       - bytes
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Length:
-      - '3199'
+      - '3282'
       Content-Type:
       - application/json; charset=UTF-8
       Date:
-      - Fri, 21 Oct 2022 14:44:55 GMT
+      - Thu, 27 Apr 2023 14:59:01 GMT
       Expires:
-      - Fri, 21 Oct 2022 14:45:55 GMT
+      - Thu, 27 Apr 2023 15:00:01 GMT
       Last-Modified:
-      - Thu, 29 Sep 2022 12:46:02 GMT
+      - Thu, 27 Apr 2023 12:53:02 GMT
       Vary:
       - Accept-Encoding
       x-rate-limit-limit:
       - '120'
       x-rate-limit-remaining:
-      - '67'
+      - '119'
     status:
       code: 200
       message: OK
 - request:
     body: null
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python-requests/2.28.1
-    method: GET
-    uri: https://api.stlouisfed.org/fred/series?file_type=json&series_id=GDP
-  response:
-    body:
-      string: !!binary |
-        H4sIAAAAAAAEA6pWKkpNzCnJzE2NLy5JLCpRslIyMjAy0jU00DUyVNJByKbmpaDLFacWZaYWFytZ
-        RVcrZYJk3V0CkLWQbGBJZklOqpKVkntRfnGxgkt+bmpxSWayQkBRfkppcomSjlJ+UnFqUVliSWZ+
-        Hty5hpYm5roGhroGIOciK0BysYEJRDqtKLWwNDUvuVLJSimwNLGoJLUop1JJRwkuHl+ckQ8OhEAl
-        HaXSvMySYiUrJafMnJzM/Lxihfw0BZf8nJzEomKYLFy9U2aOHkheRUlHqTg1sTg/LzEnPjElq7S4
-        JDc1DxSswVDRnEoFR7B4aoqCY15eaWKOQlBiSSp2fXDzgx0dg5R0lHISi0viSwtSEktSQQEOjioD
-        S10jSwUDcysTMysDI10DUyUdpYL8gtKcxKLMkkolK0tjHaW8/JJUsFdcHRUck5PzS/NKFJzzU1Kt
-        FBwNLQ2DnGPyYvIgoZ4CC/UCSKgraLi7BGjqKJRkpCqkpSaWlBalpijkpiYWlxalgjwcqhesp5Bf
-        WlJQWqKjkFkMVpebWJSdWqJQlphTClYD0puen59SrJCYl6IAisLM5NRiBYgNqSkKSZUKOYlJ+UVg
-        6YKi/ILUopJKhZz8ZJA3FTLzwIaG5mWWpKYoBJcklqQW67nlFynk5helKmTmpeUX5YKThI5CcWoq
-        WK17aWZKqkJJPpjjB5ZMzFHwzEvOz00FWwJNUrCwAEctyJUoliho+HkGOGqCNYAknUqLUhNLQZ52
-        Tc7Py8/NTFZwzEvMqSzOLFbQyCgpKbCK0Y/RLy8v10tKTdRLzy+L0c+D2g1YjH5BSlqMfl5mQWJ6
-        aWaKXkFKmqaeUm1sLQCTEdb/gAMAAA==
-    headers:
-      Accept-Ranges:
-      - bytes
-      Connection:
-      - keep-alive
-      Content-Encoding:
-      - gzip
-      Content-Length:
-      - '649'
-      Content-Type:
-      - application/json; charset=UTF-8
-      Date:
-      - Fri, 21 Oct 2022 14:44:55 GMT
-      Expires:
-      - Fri, 21 Oct 2022 14:45:55 GMT
-      Last-Modified:
-      - Thu, 29 Sep 2022 12:46:02 GMT
-      Vary:
-      - Accept-Encoding
-      x-rate-limit-limit:
-      - '120'
-      x-rate-limit-remaining:
-      - '66'
-    status:
-      code: 200
-      message: OK
-- request:
-    body: null
-    headers:
-      Accept:
-      - '*/*'
-      Accept-Encoding:
-      - gzip, deflate
-      Connection:
-      - keep-alive
-      User-Agent:
-      - python-requests/2.28.1
+      - python-requests/2.28.2
     method: GET
     uri: https://api.stlouisfed.org/fred/series/observations?file_type=json&output_type=4&realtime_start=1776-07-04&series_id=GDP
   response:
     body:
       string: !!binary |
         H4sIAAAAAAAEA6pWKkpNzCnJzE2NLy5JLCpRslIyNDc30zUw1zUwUdJByKbmpShZKVlaWlrqGhrp
         Ghsq6SjlJxWnFpUllmTm5yE0mxkY6BoY6hqgK8CivzQvs6RYyUopJzMPZFppSUFpSXxJZUGqkpWJ
         jlJaZk4qlKeUVZwPVlKUkloUn1SpZIVid0piSaqSjlJxflFJfD5IiZKVUmJxspKOUnJ+aV6JkpWh
-        kbGOUn5aWnFqiZKVgY5STmZuJkjYAARQ/FGsZBWNLUgsLY1AvjKyxAwSQ7Ccka6RuZKOEtgpVkqG
+        kZmOUn5aWnFqiZKVgY5STmZuJkjYAARQ/FGsZBWNLUgsLY1AvjKyxAwSQ7Ccka6RuZKOEtgpVkqG
         lpaGuoaggFDSUSpLzClNVbJSMjU3NtMzU6rVwWmBia6RBS4LTCFyCAvADgIHM9wCCwNLPWN8Fpjr
         GhvgssBC18gMxQdGugYmkHhEWGBpjNcHhgaQYICnKUisg4PI0FDXCJSiUHxgjmaBpZm5niFOHxiD
         4wB7EBnrGhjpGpmi+QA9DswMzAz1LPFZYKKLI5KNdQ1MIb5D+ADsIJQ4MDM0tdCzwGeBOR4LLCDx
         g2IBWhyYGRmY4fUBKA5wBZGhIRYL0OLAzNjSDE8qAjkHkhQxI9kEHAcgy5F9gBEHpoYGeILIBJTs
         cOQDE3AcoCZTsINQ48DMwFLPBGccmIAKNxyRbKJrYIGeisAOQrPAAl8+MAFlfZw+AOUDUDGCCCKw
         g1AtMDc3xRPJpuB8ACpvMOPAFEscgB2EaoGFpSGejGaKJw5MQXEALkYQPgA7CNUCSwsj/D4wx5WK
         TMFxgBpEYAehWGBuYGiIJxWZguMAexCZgYLPEDWZmoISBaoFhobGekY4U5EZOJyNsZamZqDgAxuG
@@ -219,36 +166,40 @@
         HgK7CcUOIwMTUE1ngGMhi5GBIXg6GGdYgdpNqDURuKePZoeZqaWegRGOdXVGBoaQ3jPIrZjxYalr
         YAzJNYi8B3YTmh0WloZ6xma44wPck8XhD0jfGjU+MPvWRoYGZkZ6Zpa4SylwXxa3HRitJ7CbUP1h
         aGxsrmdhiWOJIDiscI5zGFqCyynUWhXsJjQ7TI1M9SwMccaHEah7gKMFBZJDn5EA2QvSgpQHjQzN
         jU30jMxwpl2QOSY4evEgOdS1lEYGIDG0OsPI0NTYXM8SZwMEpAVX5Q2SQ+9kg8RALTUkbxhamhhY
         6Jmb4gsq0DAsKOlgJF0jA3B0oDSjQHagFVdGhoag5qwxjkUuRgZGIH9DOkCYdhiCO3jodqBXHEaG
         JuaWeqa4syDIDpzRAZm6RklWIPUgZyGFlZGRgYmFngWe+AB3bbE3REDmoXe2QWJo8WFkZG5kpGdq
         gTMLGkG621iLEpCcoa4RSnMKZAd6fBgbmhvrmVjiTrrg7i32ot0I0uFGtwMjPowtLY30jE1xxzl4
-        whh7RQuyA70qB4mhx4eJsYWRnpkFzklskB5cazpAcuhrOkBi6PEBmImFqaGehYGlUm1sLRcXFwAZ
-        bKGfLzAAAA==
+        whh7RQuyA70qB4mhx4eJsYWRnpkFzklskB5cazpAcuhrOkBi6PFhYmFqqGdhgDt/QLrdoCoCM+0a
+        gfMHKO/Ai3aQHejxYWpmZqxnZIHbDnDHG3uxawSZyEYZ6jICuwm1SDQzNDbSMzHFWeyCzME+BIKy
+        5QHhD7Cb0OwAzMTMVM/CzFSpNraWi4sLAPX5MHxbMQAA
     headers:
       Accept-Ranges:
       - bytes
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Length:
-      - '3199'
+      - '3282'
       Content-Type:
       - application/json; charset=UTF-8
       Date:
-      - Fri, 21 Oct 2022 14:44:56 GMT
+      - Fri, 28 Apr 2023 01:29:28 GMT
       Expires:
-      - Fri, 21 Oct 2022 14:45:56 GMT
+      - Fri, 28 Apr 2023 01:30:28 GMT
       Last-Modified:
-      - Thu, 29 Sep 2022 12:46:02 GMT
+      - Thu, 27 Apr 2023 12:53:02 GMT
+      Set-Cookie:
+      - cookiesession1=678A3E1FBAD4F66142727BC12B30073B;Expires=Sat, 27 Apr 2024 01:29:25
+        GMT;Path=/;Secure;HttpOnly
       Vary:
       - Accept-Encoding
       x-rate-limit-limit:
       - '120'
       x-rate-limit-remaining:
-      - '65'
+      - '67'
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `pyfredapi-0.6.0/tests/vhs/test_series/test_get_series_initial_release[pandas].yaml` & `pyfredapi-0.7.0/tests/vhs/test_series/test_get_series_initial_release[json].yaml`

 * *Files 27% similar despite different names*

```diff
@@ -5,24 +5,24 @@
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python-requests/2.28.1
+      - python-requests/2.28.2
     method: GET
     uri: https://api.stlouisfed.org/fred/series/observations?file_type=json&output_type=4&realtime_start=1776-07-04&series_id=GDP
   response:
     body:
       string: !!binary |
         H4sIAAAAAAAEA6pWKkpNzCnJzE2NLy5JLCpRslIyNDc30zUw1zUwUdJByKbmpShZKVlaWlrqGhrp
         Ghsq6SjlJxWnFpUllmTm5yE0mxkY6BoY6hqgK8CivzQvs6RYyUopJzMPZFppSUFpSXxJZUGqkpWJ
         jlJaZk4qlKeUVZwPVlKUkloUn1SpZIVid0piSaqSjlJxflFJfD5IiZKVUmJxspKOUnJ+aV6JkpWh
-        kbGOUn5aWnFqiZKVgY5STmZuJkjYAARQ/FGsZBWNLUgsLY1AvjKyxAwSQ7Ccka6RuZKOEtgpVkqG
+        kZmOUn5aWnFqiZKVgY5STmZuJkjYAARQ/FGsZBWNLUgsLY1AvjKyxAwSQ7Ccka6RuZKOEtgpVkqG
         lpaGuoaggFDSUSpLzClNVbJSMjU3NtMzU6rVwWmBia6RBS4LTCFyCAvADgIHM9wCCwNLPWN8Fpjr
         GhvgssBC18gMxQdGugYmkHhEWGBpjNcHhgaQYICnKUisg4PI0FDXCJSiUHxgjmaBpZm5niFOHxiD
         4wB7EBnrGhjpGpmi+QA9DswMzAz1LPFZYKKLI5KNdQ1MIb5D+ADsIJQ4MDM0tdCzwGeBOR4LLCDx
         g2IBWhyYGRmY4fUBKA5wBZGhIRYL0OLAzNjSDE8qAjkHkhQxI9kEHAcgy5F9gBEHpoYGeILIBJTs
         cOQDE3AcoCZTsINQ48DMwFLPBGccmIAKNxyRbKJrYIGeisAOQrPAAl8+MAFlfZw+AOUDUDGCCCKw
         g1AtMDc3xRPJpuB8ACpvMOPAFEscgB2EaoGFpSGejGaKJw5MQXEALkYQPgA7CNUCSwsj/D4wx5WK
         TMFxgBpEYAehWGBuYGiIJxWZguMAexCZgYLPEDWZmoISBaoFhobGekY4U5EZOJyNsZamZqDgAxuG
@@ -66,116 +66,263 @@
         HgK7CcUOIwMTUE1ngGMhi5GBIXg6GGdYgdpNqDURuKePZoeZqaWegRGOdXVGBoaQ3jPIrZjxYalr
         YAzJNYi8B3YTmh0WloZ6xma44wPck8XhD0jfGjU+MPvWRoYGZkZ6Zpa4SylwXxa3HRitJ7CbUP1h
         aGxsrmdhiWOJIDiscI5zGFqCyynUWhXsJjQ7TI1M9SwMccaHEah7gKMFBZJDn5EA2QvSgpQHjQzN
         jU30jMxwpl2QOSY4evEgOdS1lEYGIDG0OsPI0NTYXM8SZwMEpAVX5Q2SQ+9kg8RALTUkbxhamhhY
         6Jmb4gsq0DAsKOlgJF0jA3B0oDSjQHagFVdGhoag5qwxjkUuRgZGIH9DOkCYdhiCO3jodqBXHEaG
         JuaWeqa4syDIDpzRAZm6RklWIPUgZyGFlZGRgYmFngWe+AB3bbE3REDmoXe2QWJo8WFkZG5kpGdq
         gTMLGkG621iLEpCcoa4RSnMKZAd6fBgbmhvrmVjiTrrg7i32ot0I0uFGtwMjPowtLY30jE1xxzl4
-        whh7RQuyA70qB4mhx4eJsYWRnpkFzklskB5cazpAcuhrOkBi6PEBmImFqaGehYGlUm1sLRcXFwAZ
-        bKGfLzAAAA==
+        whh7RQuyA70qB4mhx4eJsYWRnpkFzklskB5cazpAcuhrOkBi6PFhYmFqqGdhgDt/QLrdoCoCM+0a
+        gfMHKO/Ai3aQHejxYWpmZqxnZIHbDnDHG3uxawSZyEYZ6jICuwm1SDQzNDbSMzHFWeyCzME+BIKy
+        5QHhD7Cb0OwAzMTMVM/CzFSpNraWi4sLAPX5MHxbMQAA
     headers:
       Accept-Ranges:
       - bytes
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Length:
-      - '3199'
+      - '3282'
       Content-Type:
       - application/json; charset=UTF-8
       Date:
-      - Fri, 21 Oct 2022 14:44:56 GMT
+      - Thu, 27 Apr 2023 14:59:00 GMT
       Expires:
-      - Fri, 21 Oct 2022 14:45:56 GMT
+      - Thu, 27 Apr 2023 15:00:00 GMT
       Last-Modified:
-      - Thu, 29 Sep 2022 12:46:02 GMT
+      - Thu, 27 Apr 2023 12:53:02 GMT
       Vary:
       - Accept-Encoding
       x-rate-limit-limit:
       - '120'
       x-rate-limit-remaining:
-      - '64'
+      - '51'
     status:
       code: 200
       message: OK
 - request:
     body: null
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python-requests/2.28.1
+      - python-requests/2.28.2
     method: GET
-    uri: https://api.stlouisfed.org/fred/series?file_type=json&series_id=GDP
+    uri: https://api.stlouisfed.org/fred/series/observations?file_type=json&output_type=4&realtime_start=1776-07-04&series_id=GDP
+  response:
+    body:
+      string: !!binary |
+        H4sIAAAAAAAEA6pWKkpNzCnJzE2NLy5JLCpRslIyNDc30zUw1zUwUdJByKbmpShZKVlaWlrqGhrp
+        Ghsq6SjlJxWnFpUllmTm5yE0mxkY6BoY6hqgK8CivzQvs6RYyUopJzMPZFppSUFpSXxJZUGqkpWJ
+        jlJaZk4qlKeUVZwPVlKUkloUn1SpZIVid0piSaqSjlJxflFJfD5IiZKVUmJxspKOUnJ+aV6JkpWh
+        kZmOUn5aWnFqiZKVgY5STmZuJkjYAARQ/FGsZBWNLUgsLY1AvjKyxAwSQ7Ccka6RuZKOEtgpVkqG
+        lpaGuoaggFDSUSpLzClNVbJSMjU3NtMzU6rVwWmBia6RBS4LTCFyCAvADgIHM9wCCwNLPWN8Fpjr
+        GhvgssBC18gMxQdGugYmkHhEWGBpjNcHhgaQYICnKUisg4PI0FDXCJSiUHxgjmaBpZm5niFOHxiD
+        4wB7EBnrGhjpGpmi+QA9DswMzAz1LPFZYKKLI5KNdQ1MIb5D+ADsIJQ4MDM0tdCzwGeBOR4LLCDx
+        g2IBWhyYGRmY4fUBKA5wBZGhIRYL0OLAzNjSDE8qAjkHkhQxI9kEHAcgy5F9gBEHpoYGeILIBJTs
+        cOQDE3AcoCZTsINQ48DMwFLPBGccmIAKNxyRbKJrYIGeisAOQrPAAl8+MAFlfZw+AOUDUDGCCCKw
+        g1AtMDc3xRPJpuB8ACpvMOPAFEscgB2EaoGFpSGejGaKJw5MQXEALkYQPgA7CNUCSwsj/D4wx5WK
+        TMFxgBpEYAehWGBuYGiIJxWZguMAexCZgYLPEDWZmoISBaoFhobGekY4U5EZOJyNsZamZqDgAxuG
+        HETo+cDc2MQCTxyYgcLZwAiXBaaQYgRhAdhXYEthxbW5ibGBnjk+H1hAil/MVGQGjgPUIEL4Cm6B
+        qTF+HxgaQMobbBaA8gFqToa0OkANB7gFZoa4K0xQuQVpiGAabw6OHVD0IwcQRgyYGxviCSBQEwiX
+        +81BsQMuRBAWgB2EGgMWZmZ6BjhjwByU6MBNKaw+sECvbsAOQrHAwsDABE8uMAflApwWgGIAtcIE
+        OwjVAkO8QQRKQLiCyAIcB6hRDHYQqgVGJoZ6pjiDyAKUlcClDWYQWYDjADWSwQ5CtcDY2AhPPrbA
+        EwcW4FyA6gOwg1AtMCEQRLhzgYUuKA5AhQgiFYEdhGqBqZEZniCyBBVn4KSIGUSW4DhAjWQLUKJA
+        tcDM3AhPKrLEEweW4DhADSKwg1AtsDAwx1MbWILiALcPMGpksIPQLLA0xtNosQR5GUeNbIklDsAO
+        QrHA0sgcZ6vIyADS58FmAUTOCL3pC3YQqgUm5jibvhBDTCDFAVokQ+RMUSyAiEE7YbCy1NLM0hxX
+        PoBowF4jQ+QssFgAankh9W8sLY3NccUB2BBQyxSUW7H5AJQPkKobsHpQHxS5NjA0MDDDGctGBuBe
+        J9YKASKH2kUD24BeIRgaGBqZ4iqwIabgjAVDcE5A6uFA1KPFgqGBkQnOtiNEhzmueDYEF0eooWQI
+        ypsoCcnQwMjQHFcvDWwDqDwChStmPBiC8wJS0wusHjMejEzM9XA0LIwMDMA9U2xlNkQOIx4wu8qG
+        BkZGhnj8AO6agrurmH4wAscDUpkKsRUjHkClNo7OMkSHOa60ZIQlHsAuQosHYzNLXIUe2Abc8WAE
+        jgekYhusHjMeTCzMcLUgjQwMwL1THPEA6S6DciO05gHbgJkfTM2N8ORpY1DqA3e6MeMB0l9GTa1g
+        F6GFEqhYwtHIg/gBZzwYg+MB1Q9gF6HZYG6Or1wyBtUNOEMJVC6h5mljUGWFaoOhgbEFrg6nkQF4
+        FAVrIwkiZ4Qy8AL2M0Y8GBqZ4Kt+wF1UbBUoxAZTdBtAJTek6Q+rHQwNTUzMcbUBIKZgHzyCyKEO
+        HkHEQJYgVQ+GhmYmOIenwDpA9QOo7MFMSybg/ACSQ6RWzF6zoaGFgTGuhpKRgQG4l4qjkoZ0m1Fj
+        GrPbbGgIGqDC0aCH2IB9DA8iZ4oytAARQy+XjAwtjPCUreB+Ko6YBnecwSkZEUqYHWdDI2NzMzwN
+        AUjPGZRvMePBFEs8gF2Emh+MTC0s8ZTe4J4qeLgU0wZItxo1T4NdhGaDubEpnnIJ3FXFEdPgfjXy
+        SKSRgQHYRag2GBsYGeApvcF9Vdw2WKD0ziE2oOcHY0NLY7w2gPIDKCSwhRKoXALFESKmwS5C84Ox
+        gQWeUAL3V7H1Do0MQFUNRj1tBiop0WwwsTDHk5bAHVYcMQ3uQaOlVrCL0GwwMzbCk5bAPVbcNmDE
+        A9hFaDaYm+IcbAOHBO562hycH1DjAewiNBssjczw5GlwnxUcEpgxDelEg1IBIqYxO9GGJgYWOMdU
+        jQwMwJ1W3Dagzi1A1KOXSyaGFqZ4Yhrca8WRliDdaFQ/gF2EGkomRqY4u7lgN4HiAcv0BUQOdXYB
+        LAZKxKB2LryOMzExssTjB0tQRxpHKEE60kj9XLANGPW0iZGZCZ7UCu644ii9IT1p1LQEdhFaKBmY
+        m+Kp48A9VxzxYAluL6H6AewiNBsMTSzxtATAXVecfgCVS6htb7CL0GwwNsA55mNkAA5USPmJkR9A
+        cqjTPEYGBmAXodlgYmaMu0UGMsUER4sMJGeG1tkFiWHkBzMDQ/w24GovgUxDby+BxNDrBxNTSzy9
+        LEMDUGmMPR5Acoa6RqCxY3ipAbIBVLwit8hMzI0NcOcHQ5CXsQ7SGxmA5FAHNcDxBrIENcdZmBvg
+        CSVw7xV7LQqyAb29BBIDOQrZD6YGBmb4bcA+4QbxA+rQEkQMPR5MDQyMcecHQ3DvFXsNBJIz1DUC
+        hQgiHgwx+w+mhpYWuEsNQ3B/GocNRuABPpRSA2Qr2tSzoamRpQnulgDIBlzjGiA5U0heQfgB7CLU
+        HGdqYoZzPsbIAGQKrnENkJwFJJ2h2IARD6aWeOppQyNwfgCVbkWwFQ2Q2Wew7aByCTWUjLDEA2ja
+        Dee4hiG494q9fgDJobeXIC5CCyULI0vc40sgU0wgfTVMP0D60yh9IJB69PxgZmCIL0+De6/Y6weQ
+        aRjxgKU/bWZmjK9sNQa1iQxAtT02P4AiG6WXBbIVvVwyszDFM4JlCEoYkBSJaQNkChpkOyItgXv4
+        qPFgbmhghLsWBdmAs36AzEGjpiWwi9BtMMHTBwLZgLN+gExCo/oB3MNHswGUp3GnVnDvFUdqhfSn
+        UeMBS3/a3NTYVA/HRLqRgSG4P43DBkh/GpQbEfEAdhGaH8wNDXC3jEE2YF+PAbEdvd0KUo+eH8xB
+        NuDssYN04IwHcH8aPMqI8AOW/rS5hYkBnrQE7r3iqKch/WmU9hLERaihZGFgjHOWz8jAENx7xWED
+        pD+NMpJoCHYRmg2GRhZ4WgJ4+tMg29HHl0Bi6PFgARrRxbG0B+IHnPU0ZDIa1Q9gF6H5wcQYX6kB
+        7r3iaGuYgcossBwiprH0py3MTA3xhBKoGMMxdm+IMSEN9jNGe8nCwgxPPw5kCq7xJZAcRnsJ7CLU
+        ULI0MDDH0xIA917BIYFZtpqD+w+oNRCW/rSlEb7eriG494qjNYOlPw3yF8gbyG0+SxNLUz0Tc5yj
+        xobgHjU452L6AkuPGuImtHAyN7bQs7DAXb6Ce7A4/AGZmUYNKbCb0OywNDPVMzbC6w+crSZIrxq1
+        HgK7CcUOIwMTUE1ngGMhi5GBIXg6GGdYgdpNqDURuKePZoeZqaWegRGOdXVGBoaQ3jPIrZjxYalr
+        YAzJNYi8B3YTmh0WloZ6xma44wPck8XhD0jfGjU+MPvWRoYGZkZ6Zpa4SylwXxa3HRitJ7CbUP1h
+        aGxsrmdhiWOJIDiscI5zGFqCyynUWhXsJjQ7TI1M9SwMccaHEah7gKMFBZJDn5EA2QvSgpQHjQzN
+        jU30jMxwpl2QOSY4evEgOdS1lEYGIDG0OsPI0NTYXM8SZwMEpAVX5Q2SQ+9kg8RALTUkbxhamhhY
+        6Jmb4gsq0DAsKOlgJF0jA3B0oDSjQHagFVdGhoag5qwxjkUuRgZGIH9DOkCYdhiCO3jodqBXHEaG
+        JuaWeqa4syDIDpzRAZm6RklWIPUgZyGFlZGRgYmFngWe+AB3bbE3REDmoXe2QWJo8WFkZG5kpGdq
+        gTMLGkG621iLEpCcoa4RSnMKZAd6fBgbmhvrmVjiTrrg7i32ot0I0uFGtwMjPowtLY30jE1xxzl4
+        whh7RQuyA70qB4mhx4eJsYWRnpkFzklskB5cazpAcuhrOkBi6PFhYmFqqGdhgDt/QLrdoCoCM+0a
+        gfMHKO/Ai3aQHejxYWpmZqxnZIHbDnDHG3uxawSZyEYZ6jICuwm1SDQzNDbSMzHFWeyCzME+BIKy
+        5QHhD7Cb0OwAzMTMVM/CzFSpNraWi4sLAPX5MHxbMQAA
+    headers:
+      Accept-Ranges:
+      - bytes
+      Connection:
+      - keep-alive
+      Content-Encoding:
+      - gzip
+      Content-Length:
+      - '3282'
+      Content-Type:
+      - application/json; charset=UTF-8
+      Date:
+      - Thu, 27 Apr 2023 14:59:00 GMT
+      Expires:
+      - Thu, 27 Apr 2023 15:00:00 GMT
+      Last-Modified:
+      - Thu, 27 Apr 2023 12:53:02 GMT
+      Vary:
+      - Accept-Encoding
+      x-rate-limit-limit:
+      - '120'
+      x-rate-limit-remaining:
+      - '120'
+    status:
+      code: 200
+      message: OK
+- request:
+    body: null
+    headers:
+      Accept:
+      - '*/*'
+      Accept-Encoding:
+      - gzip, deflate
+      Connection:
+      - keep-alive
+      User-Agent:
+      - python-requests/2.28.2
+    method: GET
+    uri: https://api.stlouisfed.org/fred/series/observations?file_type=json&output_type=4&realtime_start=1776-07-04&series_id=GDP
   response:
     body:
       string: !!binary |
-        H4sIAAAAAAAEA6pWKkpNzCnJzE2NLy5JLCpRslIyMjAy0jU00DUyVNJByKbmpaDLFacWZaYWFytZ
-        RVcrZYJk3V0CkLWQbGBJZklOqpKVkntRfnGxgkt+bmpxSWayQkBRfkppcomSjlJ+UnFqUVliSWZ+
-        Hty5hpYm5roGhroGIOciK0BysYEJRDqtKLWwNDUvuVLJSimwNLGoJLUop1JJRwkuHl+ckQ8OhEAl
-        HaXSvMySYiUrJafMnJzM/Lxihfw0BZf8nJzEomKYLFy9U2aOHkheRUlHqTg1sTg/LzEnPjElq7S4
-        JDc1DxSswVDRnEoFR7B4aoqCY15eaWKOQlBiSSp2fXDzgx0dg5R0lHISi0viSwtSEktSQQEOjioD
-        S10jSwUDcysTMysDI10DUyUdpYL8gtKcxKLMkkolK0tjHaW8/JJUsFdcHRUck5PzS/NKFJzzU1Kt
-        FBwNLQ2DnGPyYvIgoZ4CC/UCSKgraLi7BGjqKJRkpCqkpSaWlBalpijkpiYWlxalgjwcqhesp5Bf
-        WlJQWqKjkFkMVpebWJSdWqJQlphTClYD0puen59SrJCYl6IAisLM5NRiBYgNqSkKSZUKOYlJ+UVg
-        6YKi/ILUopJKhZz8ZJA3FTLzwIaG5mWWpKYoBJcklqQW67nlFynk5helKmTmpeUX5YKThI5CcWoq
-        WK17aWZKqkJJPpjjB5ZMzFHwzEvOz00FWwJNUrCwAEctyJUoliho+HkGOGqCNYAknUqLUhNLQZ52
-        Tc7Py8/NTFZwzEvMqSzOLFbQyCgpKbCK0Y/RLy8v10tKTdRLzy+L0c+D2g1YjH5BSlqMfl5mQWJ6
-        aWaKXkFKmqaeUm1sLQCTEdb/gAMAAA==
+        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
     headers:
       Accept-Ranges:
       - bytes
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Length:
-      - '649'
+      - '3282'
       Content-Type:
       - application/json; charset=UTF-8
       Date:
-      - Fri, 21 Oct 2022 14:44:57 GMT
+      - Fri, 28 Apr 2023 01:29:27 GMT
       Expires:
-      - Fri, 21 Oct 2022 14:45:57 GMT
+      - Fri, 28 Apr 2023 01:30:27 GMT
       Last-Modified:
-      - Thu, 29 Sep 2022 12:46:02 GMT
+      - Thu, 27 Apr 2023 12:53:02 GMT
       Vary:
       - Accept-Encoding
       x-rate-limit-limit:
       - '120'
       x-rate-limit-remaining:
-      - '63'
+      - '69'
     status:
       code: 200
       message: OK
 - request:
     body: null
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python-requests/2.28.1
+      - python-requests/2.28.2
     method: GET
     uri: https://api.stlouisfed.org/fred/series/observations?file_type=json&output_type=4&realtime_start=1776-07-04&series_id=GDP
   response:
     body:
       string: !!binary |
         H4sIAAAAAAAEA6pWKkpNzCnJzE2NLy5JLCpRslIyNDc30zUw1zUwUdJByKbmpShZKVlaWlrqGhrp
         Ghsq6SjlJxWnFpUllmTm5yE0mxkY6BoY6hqgK8CivzQvs6RYyUopJzMPZFppSUFpSXxJZUGqkpWJ
         jlJaZk4qlKeUVZwPVlKUkloUn1SpZIVid0piSaqSjlJxflFJfD5IiZKVUmJxspKOUnJ+aV6JkpWh
-        kbGOUn5aWnFqiZKVgY5STmZuJkjYAARQ/FGsZBWNLUgsLY1AvjKyxAwSQ7Ccka6RuZKOEtgpVkqG
+        kZmOUn5aWnFqiZKVgY5STmZuJkjYAARQ/FGsZBWNLUgsLY1AvjKyxAwSQ7Ccka6RuZKOEtgpVkqG
         lpaGuoaggFDSUSpLzClNVbJSMjU3NtMzU6rVwWmBia6RBS4LTCFyCAvADgIHM9wCCwNLPWN8Fpjr
         GhvgssBC18gMxQdGugYmkHhEWGBpjNcHhgaQYICnKUisg4PI0FDXCJSiUHxgjmaBpZm5niFOHxiD
         4wB7EBnrGhjpGpmi+QA9DswMzAz1LPFZYKKLI5KNdQ1MIb5D+ADsIJQ4MDM0tdCzwGeBOR4LLCDx
         g2IBWhyYGRmY4fUBKA5wBZGhIRYL0OLAzNjSDE8qAjkHkhQxI9kEHAcgy5F9gBEHpoYGeILIBJTs
         cOQDE3AcoCZTsINQ48DMwFLPBGccmIAKNxyRbKJrYIGeisAOQrPAAl8+MAFlfZw+AOUDUDGCCCKw
         g1AtMDc3xRPJpuB8ACpvMOPAFEscgB2EaoGFpSGejGaKJw5MQXEALkYQPgA7CNUCSwsj/D4wx5WK
         TMFxgBpEYAehWGBuYGiIJxWZguMAexCZgYLPEDWZmoISBaoFhobGekY4U5EZOJyNsZamZqDgAxuG
@@ -219,36 +366,37 @@
         HgK7CcUOIwMTUE1ngGMhi5GBIXg6GGdYgdpNqDURuKePZoeZqaWegRGOdXVGBoaQ3jPIrZjxYalr
         YAzJNYi8B3YTmh0WloZ6xma44wPck8XhD0jfGjU+MPvWRoYGZkZ6Zpa4SylwXxa3HRitJ7CbUP1h
         aGxsrmdhiWOJIDiscI5zGFqCyynUWhXsJjQ7TI1M9SwMccaHEah7gKMFBZJDn5EA2QvSgpQHjQzN
         jU30jMxwpl2QOSY4evEgOdS1lEYGIDG0OsPI0NTYXM8SZwMEpAVX5Q2SQ+9kg8RALTUkbxhamhhY
         6Jmb4gsq0DAsKOlgJF0jA3B0oDSjQHagFVdGhoag5qwxjkUuRgZGIH9DOkCYdhiCO3jodqBXHEaG
         JuaWeqa4syDIDpzRAZm6RklWIPUgZyGFlZGRgYmFngWe+AB3bbE3REDmoXe2QWJo8WFkZG5kpGdq
         gTMLGkG621iLEpCcoa4RSnMKZAd6fBgbmhvrmVjiTrrg7i32ot0I0uFGtwMjPowtLY30jE1xxzl4
-        whh7RQuyA70qB4mhx4eJsYWRnpkFzklskB5cazpAcuhrOkBi6PEBmImFqaGehYGlUm1sLRcXFwAZ
-        bKGfLzAAAA==
+        whh7RQuyA70qB4mhx4eJsYWRnpkFzklskB5cazpAcuhrOkBi6PFhYmFqqGdhgDt/QLrdoCoCM+0a
+        gfMHKO/Ai3aQHejxYWpmZqxnZIHbDnDHG3uxawSZyEYZ6jICuwm1SDQzNDbSMzHFWeyCzME+BIKy
+        5QHhD7Cb0OwAzMTMVM/CzFSpNraWi4sLAPX5MHxbMQAA
     headers:
       Accept-Ranges:
       - bytes
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Length:
-      - '3199'
+      - '3282'
       Content-Type:
       - application/json; charset=UTF-8
       Date:
-      - Fri, 21 Oct 2022 14:44:58 GMT
+      - Fri, 28 Apr 2023 01:29:27 GMT
       Expires:
-      - Fri, 21 Oct 2022 14:45:57 GMT
+      - Fri, 28 Apr 2023 01:30:27 GMT
       Last-Modified:
-      - Thu, 29 Sep 2022 12:46:02 GMT
+      - Thu, 27 Apr 2023 12:53:02 GMT
       Vary:
       - Accept-Encoding
       x-rate-limit-limit:
       - '120'
       x-rate-limit-remaining:
-      - '62'
+      - '68'
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `pyfredapi-0.6.0/tests/vhs/test_series_collection/test_merge_asof.yaml` & `pyfredapi-0.7.0/tests/vhs/test_series_collection/test_drop_series.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -5,504 +5,507 @@
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python-requests/2.28.1
+      - python-requests/2.29.0
     method: GET
     uri: https://api.stlouisfed.org/fred/series/observations?file_type=json&series_id=CPIAUCSL
   response:
     body:
       string: !!binary |
-        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
+        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
     headers:
       Accept-Ranges:
       - bytes
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Length:
-      - '8718'
+      - '8776'
       Content-Type:
       - application/json; charset=UTF-8
       Date:
-      - Fri, 21 Oct 2022 15:13:40 GMT
+      - Thu, 27 Apr 2023 15:01:37 GMT
       Expires:
-      - Fri, 21 Oct 2022 15:14:40 GMT
+      - Thu, 27 Apr 2023 15:02:37 GMT
       Last-Modified:
-      - Thu, 13 Oct 2022 12:37:02 GMT
+      - Wed, 12 Apr 2023 16:11:01 GMT
       Vary:
       - Accept-Encoding
       x-rate-limit-limit:
       - '120'
       x-rate-limit-remaining:
-      - '80'
+      - '116'
     status:
       code: 200
       message: OK
 - request:
     body: null
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python-requests/2.28.1
+      - python-requests/2.29.0
     method: GET
     uri: https://api.stlouisfed.org/fred/series?file_type=json&series_id=CPIAUCSL
   response:
     body:
       string: !!binary |
-        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
+        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
-        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
-        l1GSq6lUG1sLABtQtSScDAAA
+        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
+        XE2l2thaAPvCGzucDAAA
     headers:
       Accept-Ranges:
       - bytes
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Length:
-      - '2070'
+      - '2067'
       Content-Type:
       - application/json; charset=UTF-8
       Date:
-      - Fri, 21 Oct 2022 15:13:41 GMT
+      - Thu, 27 Apr 2023 15:01:37 GMT
       Expires:
-      - Fri, 21 Oct 2022 15:14:41 GMT
+      - Thu, 27 Apr 2023 15:02:37 GMT
       Last-Modified:
-      - Thu, 13 Oct 2022 12:37:02 GMT
+      - Wed, 12 Apr 2023 16:11:01 GMT
       Vary:
       - Accept-Encoding
       x-rate-limit-limit:
       - '120'
       x-rate-limit-remaining:
-      - '79'
+      - '115'
     status:
       code: 200
       message: OK
 - request:
     body: null
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python-requests/2.28.1
+      - python-requests/2.29.0
     method: GET
     uri: https://api.stlouisfed.org/fred/series/observations?file_type=json&series_id=CPILFESL
   response:
     body:
       string: !!binary |
-        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
+        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
+        +QHkDaSSz9jAVM8IVD8AFlsLAFl1uPlTKwEA
     headers:
       Accept-Ranges:
       - bytes
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Length:
-      - '7629'
+      - '7722'
       Content-Type:
       - application/json; charset=UTF-8
       Date:
-      - Fri, 21 Oct 2022 15:13:41 GMT
+      - Thu, 27 Apr 2023 15:01:38 GMT
       Expires:
-      - Fri, 21 Oct 2022 15:14:41 GMT
+      - Thu, 27 Apr 2023 15:02:38 GMT
       Last-Modified:
-      - Thu, 13 Oct 2022 12:37:21 GMT
+      - Wed, 12 Apr 2023 16:09:03 GMT
       Vary:
       - Accept-Encoding
       x-rate-limit-limit:
       - '120'
       x-rate-limit-remaining:
-      - '78'
+      - '114'
     status:
       code: 200
       message: OK
 - request:
     body: null
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
       User-Agent:
-      - python-requests/2.28.1
+      - python-requests/2.29.0
     method: GET
     uri: https://api.stlouisfed.org/fred/series?file_type=json&series_id=CPILFESL
   response:
     body:
       string: !!binary |
-        H4sIAAAAAAAEA6pWKkpNzCnJzE2NLy5JLCpRslIyMjAy0jU00DUyVNJByKbmpaDLFacWZaYWFytZ
+        H4sIAAAAAAAEA6pWKkpNzCnJzE2NLy5JLCpRslIyMjAy1jUw0TUyV9JByKbmpaDLFacWZaYWFytZ
         RVcrZYJknQM8fdxcg32Q9ZFsaklmSU6qkpWSc35ecWluapFCQFFmcqqCZ15KaoVCWn6RgmNOjkJo
         UVJingJMSbEVWNCzJDW3WMEntbhYwS0/P0UhMS9FwTUvtSi9UiEzTyFUL1hPwTmzpFLBsSy1KDE9
-        VUlHKT+pOLWoLLEkMz8P7n1DS1NzXQNDXQOQ95EVIIWAgSVEOq0otbA0NS+5UslKyTc/ryQjp1JJ
-        RwkuGl+ckQ8OUl8lHaXSvMySYiUrJYhHDC0tjHQNLS1MbA0NDGCycPXY1RSnJhbn5yXmxCemZJUW
-        l+Sm5oGiKxgqmlOp4AgWT01R0lHCohZuerCjko5STmJxSXxpQUpiSSoo6mCRbmisYGBuZWxuZWSo
-        a2CqpKNUkF9QmpNYlFlSqWRlYayjlJdfkgryRkhGqkIMFSJJDRpFMUoKmcUKiXkKienpRanpiSWp
-        CvlpCgWguC9WKEjMTFFIqlQoBUd7MjRlFIOTQ6JCSWVBZnJijkJSYnF2aglIW3p+fkqxjkJqRXJO
-        aUpmXrpCWn4+JD2kgtODnkJIRmaxQm5qYnFpUSooIHUUsvPyy/MUEovBvipKVXAO8NSBOKo8MyU1
-        p1KhtDgV7IjU5Py8/NzM4pJihaTU5MTS4lR04xUyEstSFcpSiyoVyvJzEksyc1IVCsA+AVmcquBU
-        WpSaWApyqE9iUn6RQnBJYklmcUlmcrFCSmpaZl4qKCBSYM4rVijJAAVGWmZyZmIO2F3gpJ2bX5Sq
-        kJmXll+UC07BCsmJeQpJIMeU5qWAUjxIm5tjoIJGRklJQbFVjH6Mfnl5uV5STrFeen5ZjH5yQWaM
-        fmFpajEo/RfrJual6CbmFZenFhXrZZTkairkF0FMAcVLUUlmck4qTqPyC0qTYvQz8nNj9AtS0sBG
-        A5aRn6tXkJKmqadUG1sLAF2PIiFnBAAA
+        VUlHKT+pOLWoLLEkMz8P7n1DS1NzXQNDXQNDNAXIIWAMkU4rSi0sTc1LrlSyUvLNzyvJyKlU0lGC
+        i8YXZ+SDg9RXSUepNC+zpFjJSgniEUNLCyNdQ0sLE1tDAwOYLFw9djXFqYnF+XmJOfGJKVmlxSW5
+        qXmg6AqGiuZUKjiCxVNTlHSUsKiFmx7sqKSjlJNYXBJfWpCSWJIKijpYpBsaKRgaWhlYWhkY6xqY
+        KukoFeQXlOYkFmWWVCpZWRjpKOXll6SCvBGSkaoQQ4VIUoNGUYySQmaxQmKeQmJ6elFqemJJqkJ+
+        mkIBKO6LFQoSM1MUkioVSsHRngxNGcXg5JCoUFJZkJmcmKOQlFicnVoC0paen59SrKOQWpGcU5qS
+        mZeukJafD0kPqeD0oKcQkpFZrJCbmlhcWpQKCkgdhey8/PI8hcRisK+KUhWcAzx1II4qz0xJzalU
+        KC1OBTsiNTk/Lz83s7ikWCEpNTmxtDgV3XiFjMSyVIWy1KJKhbL8nMSSzJxUhQKwT0AWpyo4lRal
+        JpaCHOqTmJRfpBBckliSWVySmVyskJKalpmXCgqIFJjzihVKMkCBkZaZnJmYA3YXOGnn5helKmTm
+        peUX5YJTsEJyYp5CEsgxpXkpoBQP0ubmGKigkVFSUlBsFaMfo19eXq6XlFOsl55fFqOfXJAZo19Y
+        mloMSv/Fuol5KbqJecXlqUXFehkluZoK+UUQU0DxUlSSmZyTitOo/ILSpBj9jPzcGP2ClDSw0YBl
+        5OfqFaSkaeop1cbWAgDYo9lOZwQAAA==
     headers:
       Accept-Ranges:
       - bytes
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Length:
-      - '765'
+      - '763'
       Content-Type:
       - application/json; charset=UTF-8
       Date:
-      - Fri, 21 Oct 2022 15:13:42 GMT
+      - Thu, 27 Apr 2023 15:01:38 GMT
       Expires:
-      - Fri, 21 Oct 2022 15:14:42 GMT
+      - Thu, 27 Apr 2023 15:02:38 GMT
       Last-Modified:
-      - Thu, 13 Oct 2022 12:37:21 GMT
+      - Wed, 12 Apr 2023 16:09:03 GMT
       Vary:
       - Accept-Encoding
       x-rate-limit-limit:
       - '120'
       x-rate-limit-remaining:
-      - '77'
+      - '113'
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `pyfredapi-0.6.0/.gitignore` & `pyfredapi-0.7.0/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -130,10 +130,11 @@
 .ruff_cache/
 
 # Pyre type checker
 .pyre/
 
 # IDE
 .vscode/
+.idea/
 
 # docs in development
 dev_docs/
```

### Comparing `pyfredapi-0.6.0/LICENSE` & `pyfredapi-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.6.0/README.md` & `pyfredapi-0.7.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,44 +1,47 @@
 # pyfredapi - Python library for the Federal Reserve Economic Data (FRED) API
 
 <div align="center">
 
 
 | | |
-| --- | --- |
+| :--- | :--- |
 | CI/CD | [![CI - Test](https://github.com/gw-moore/pyfredapi/actions/workflows/test.yml/badge.svg)](https://github.com/gw-moore/pyfredapi/actions/workflows/test.yml)|
 | Docs | [![Documentation Status](https://readthedocs.org/projects/pyfredapi/badge/?version=latest)](https://pyfredapi.readthedocs.io/en/latest/?badge=latest) |
 | Package | [![PyPi Version](https://img.shields.io/pypi/v/pyfredapi.svg)](https://pypi.python.org/pypi/pyfredapi/) [![Supported Python Versions](https://img.shields.io/pypi/pyversions/pyfredapi)](https://pypi.python.org/pypi/pyfredapi) [![PyPI - Downloads](https://img.shields.io/pypi/dm/pyfredapi.svg?color=blue&label=Downloads)](https://pypi.org/project/pyfredapi/) |
-| Meta | [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch) [![linting - Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v0.json)](https://github.com/charliermarsh/ruff) [![code style - Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![types - Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://github.com/python/mypy) [![License - MIT](https://img.shields.io/badge/license-MIT-9400d3.svg)](https://spdx.org/licenses/) [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=gw-moore_pyfredapi&metric=alert_status)](https://sonarcloud.io/dashboard?id=gw-moore_pyfredapi) [![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=gw-moore_pyfredapi&metric=security_rating)](https://sonarcloud.io/dashboard?id=gw-moore_pyfredapi) [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=gw-moore_pyfredapi&metric=reliability_rating)](https://sonarcloud.io/dashboard?id=gw-moore_pyfredapi) [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=gw-moore_pyfredapi&metric=reliability_rating)](https://sonarcloud.io/dashboard?id=gw-moore_pyfredapi) |
+| Meta | [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch) [![linting - Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v0.json)](https://github.com/charliermarsh/ruff) [![code style - Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![types - Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://github.com/python/mypy) [![License - MIT](https://img.shields.io/badge/license-MIT-9400d3.svg)](https://spdx.org/licenses/) [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=gw-moore_pyfredapi&metric=alert_status)](https://sonarcloud.io/dashboard?id=gw-moore_pyfredapi) [![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=gw-moore_pyfredapi&metric=security_rating)](https://sonarcloud.io/dashboard?id=gw-moore_pyfredapi) [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=gw-moore_pyfredapi&metric=reliability_rating)](https://sonarcloud.io/dashboard?id=gw-moore_pyfredapi) |
 
 </div>
 
 -----
 
-`pyfredapi` is a full featured Python library that makes it is easy to retrieve data from the [Federal Reserve Economic Data](https://fred.stlouisfed.org/docs/api/fred/) (FRED) API web service. `pyfredapi` covers all the FRED api endpoints, and can retrieve data from [FRED](https://fred.stlouisfed.org/) and [ALFRED](https://alfred.stlouisfed.org).Data can be returned as a [pandas](https://pandas.pydata.org/) dataframe or json. Requests to the FRED API can be customized according to the parameters made available by the web service endpoints.
+`pyfredapi` is a full featured Python library that makes it is easy to retrieve data from the [Federal Reserve Economic Data](https://fred.stlouisfed.org/docs/api/fred/) (FRED) API web service. `pyfredapi` covers all the FRED api endpoints, and can retrieve data from [FRED](https://fred.stlouisfed.org/) and [ALFRED](https://alfred.stlouisfed.org). Data can be returned as a [pandas](https://pandas.pydata.org/) dataframe or json. Requests to the FRED API can be customized according to the parameters made available by the web service endpoints.
 
 ## Documentation
 
 The [documentation](https://pyfredapi.readthedocs.io/en/latest/) is made with [Sphinx](https://www.sphinx-doc.org/en/master/) and hosted on [Read the Docs](https://readthedocs.org/).
 
 ## Installation
 
 ```bash
 pip install pyfredapi
+
+# install with plotting dependencies
+pip install 'pyfredapi[plot]'
 ```
 
 ## Quick Start
 
 ### FRED API Key
 
 Before using `pyfredapi` and must have an API key to the FRED API web service. You can apply for [one for free](https://fred.stlouisfed.org/docs/api/api_key.html) on the FRED website.
 
 You can set your API key in two ways:
 
-* set your API key to the environment variable :code:`FRED_API_KEY`
+* set your API key to the environment variable `FRED_API_KEY`
 * pass it to the `api_key` parameter of the request function
 
 You can set the API key as an environment variable by adding the following line to your `~/.zshrc`, `~/.bashrc` file:
 
 ```bash
 export FRED_API_KEY="your_api_key"
 ```
```

### Comparing `pyfredapi-0.6.0/pyproject.toml` & `pyfredapi-0.7.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 authors = [
     { name = "Greg Moore", email =  "gwmoore.career@gmail.com" }
 ]
 readme = "README.md"
 license = "MIT"
 requires-python = ">=3.8"
 keywords = [
-    "fred",
     "federal reserve",
+    "fred",
     "economic data",
     "economic indicators",
     "economic statistics",
     "economic time series",
     "economic data api",
     "economic data api client",
     "economics",
@@ -31,24 +31,26 @@
     "Intended Audience :: Science/Research",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
-    "requests>=2.0.0",
-    "pandas>=1.0.0",
-    "pydantic>=1.0.0",
-    "rich>=13.0.0",
-    "plotly>=5.0.0",
-    "frozendict >=2.0.0"
+    "requests>=2.0.0,<3.0.0",
+    "pandas>=1.0.0,<2.0.0",
+    "pydantic>=1.0.0,<2.0.0",
+    "rich>=13.0.0,<14.0.0",
+    "frozendict>=2.0.0,<3.0.0",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
+plot = [
+    "plotly>=5.0.0,<6.0.0",
+]
 docs = [
     "jupyter==1.0.0",
     "Sphinx==6.1.3",
     "myst-parser==1.0.0",
     "nbsphinx==0.9.1",
     "sphinxcontrib-napoleon==0.7",
     "sphinx-copybutton==0.5.1",
@@ -104,32 +106,30 @@
     | _build
     | buck-out
     | build
     | dist
 )/
 '''
 
-[tool.isort]
-profile = "black"
-
 [tool.ruff]
 select = [
     "E",  # pycodestyle
     "F",  # Pyflakes
     "I",  # isort
     "D",  # pydocstyle
     "S",  # flake8-bandit
     "B",  # flake8-bugbear
 ]
 ignore = [
     "E501", # Line too long
     "D106", # Missing docstring in public nested class
     "D101", # Missing docstring in public class
     "D203", # 1 blank line required before class docstring
-    "D213"  # Multi-line docstring summary should start at the second line
+    "D213", # Multi-line docstring summary should start at the second line
+    "D105"  # Missing docstring in magic method
 ]
 
 # Allow autofix for all enabled rules (when `--fix`) is provided.
 fixable = ["A", "B", "C", "D", "E", "F", "G", "I", "N", "Q", "S", "T", "W", "ANN", "ARG", "BLE", "COM", "DJ", "DTZ", "EM", "ERA", "EXE", "FBT", "ICN", "INP", "ISC", "NPY", "PD", "PGH", "PIE", "PL", "PT", "PTH", "PYI", "RET", "RSE", "RUF", "SIM", "SLF", "TCH", "TID", "TRY", "UP", "YTT"]
 unfixable = []
 
 # Exclude a variety of commonly ignored directories.
@@ -162,14 +162,13 @@
 # Allow unused variables when underscore-prefixed.
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
 
 # Assume Python 3.11
 target-version = "py311"
 
 [tool.ruff.mccabe]
-# Unlike Flake8, default to a complexity level of 10.
 max-complexity = 10
 
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["E402", "D105", "F401", "D205"]
 "tests/*" = ["S101", "D103", "D100"]
 "exceptions.py" = ["D101", "D105", "D107"]
```

### Comparing `pyfredapi-0.6.0/PKG-INFO` & `pyfredapi-0.7.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfredapi
-Version: 0.6.0
+Version: 0.7.0
 Summary: A full featured API client for the FRED API web service.
 Project-URL: Homepage, https://pyfredapi.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/gw-moore/pyfredapi
 Author-email: Greg Moore <gwmoore.career@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: economic data,economic data api,economic data api client,economic indicators,economic statistics,economic time series,economics,federal reserve,fred
@@ -15,20 +15,19 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
-Requires-Dist: frozendict>=2.0.0
-Requires-Dist: pandas>=1.0.0
-Requires-Dist: plotly>=5.0.0
-Requires-Dist: pydantic>=1.0.0
-Requires-Dist: requests>=2.0.0
-Requires-Dist: rich>=13.0.0
+Requires-Dist: frozendict<3.0.0,>=2.0.0
+Requires-Dist: pandas<2.0.0,>=1.0.0
+Requires-Dist: pydantic<2.0.0,>=1.0.0
+Requires-Dist: requests<3.0.0,>=2.0.0
+Requires-Dist: rich<14.0.0,>=13.0.0
 Provides-Extra: dev
 Requires-Dist: pip-tools==6.13.0; extra == 'dev'
 Requires-Dist: pyfredapi[docs]; extra == 'dev'
 Requires-Dist: pyfredapi[lint]; extra == 'dev'
 Requires-Dist: pyfredapi[test]; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: autodoc-pydantic==1.8.0; extra == 'docs'
@@ -44,59 +43,64 @@
 Requires-Dist: mypy==1.1.1; extra == 'lint'
 Requires-Dist: pandas-stubs==1.5.3.230321; extra == 'lint'
 Requires-Dist: pre-commit==3.2.1; extra == 'lint'
 Requires-Dist: ruff==0.0.260; extra == 'lint'
 Requires-Dist: types-frozendict==2.0.9; extra == 'lint'
 Requires-Dist: types-requests==2.28.11.17; extra == 'lint'
 Requires-Dist: types-setuptools==67.6.0.6; extra == 'lint'
+Provides-Extra: plot
+Requires-Dist: plotly<6.0.0,>=5.0.0; extra == 'plot'
 Provides-Extra: test
 Requires-Dist: coverage==7.2.2; extra == 'test'
 Requires-Dist: pytest-cov==4.0.0; extra == 'test'
 Requires-Dist: pytest-vcr==1.0.2; extra == 'test'
 Requires-Dist: pytest==7.2.2; extra == 'test'
 Requires-Dist: tox==4.4.8; extra == 'test'
 Description-Content-Type: text/markdown
 
 # pyfredapi - Python library for the Federal Reserve Economic Data (FRED) API
 
 <div align="center">
 
 
 | | |
-| --- | --- |
+| :--- | :--- |
 | CI/CD | [![CI - Test](https://github.com/gw-moore/pyfredapi/actions/workflows/test.yml/badge.svg)](https://github.com/gw-moore/pyfredapi/actions/workflows/test.yml)|
 | Docs | [![Documentation Status](https://readthedocs.org/projects/pyfredapi/badge/?version=latest)](https://pyfredapi.readthedocs.io/en/latest/?badge=latest) |
 | Package | [![PyPi Version](https://img.shields.io/pypi/v/pyfredapi.svg)](https://pypi.python.org/pypi/pyfredapi/) [![Supported Python Versions](https://img.shields.io/pypi/pyversions/pyfredapi)](https://pypi.python.org/pypi/pyfredapi) [![PyPI - Downloads](https://img.shields.io/pypi/dm/pyfredapi.svg?color=blue&label=Downloads)](https://pypi.org/project/pyfredapi/) |
-| Meta | [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch) [![linting - Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v0.json)](https://github.com/charliermarsh/ruff) [![code style - Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![types - Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://github.com/python/mypy) [![License - MIT](https://img.shields.io/badge/license-MIT-9400d3.svg)](https://spdx.org/licenses/) [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=gw-moore_pyfredapi&metric=alert_status)](https://sonarcloud.io/dashboard?id=gw-moore_pyfredapi) [![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=gw-moore_pyfredapi&metric=security_rating)](https://sonarcloud.io/dashboard?id=gw-moore_pyfredapi) [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=gw-moore_pyfredapi&metric=reliability_rating)](https://sonarcloud.io/dashboard?id=gw-moore_pyfredapi) [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=gw-moore_pyfredapi&metric=reliability_rating)](https://sonarcloud.io/dashboard?id=gw-moore_pyfredapi) |
+| Meta | [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch) [![linting - Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v0.json)](https://github.com/charliermarsh/ruff) [![code style - Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![types - Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://github.com/python/mypy) [![License - MIT](https://img.shields.io/badge/license-MIT-9400d3.svg)](https://spdx.org/licenses/) [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=gw-moore_pyfredapi&metric=alert_status)](https://sonarcloud.io/dashboard?id=gw-moore_pyfredapi) [![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=gw-moore_pyfredapi&metric=security_rating)](https://sonarcloud.io/dashboard?id=gw-moore_pyfredapi) [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=gw-moore_pyfredapi&metric=reliability_rating)](https://sonarcloud.io/dashboard?id=gw-moore_pyfredapi) |
 
 </div>
 
 -----
 
-`pyfredapi` is a full featured Python library that makes it is easy to retrieve data from the [Federal Reserve Economic Data](https://fred.stlouisfed.org/docs/api/fred/) (FRED) API web service. `pyfredapi` covers all the FRED api endpoints, and can retrieve data from [FRED](https://fred.stlouisfed.org/) and [ALFRED](https://alfred.stlouisfed.org).Data can be returned as a [pandas](https://pandas.pydata.org/) dataframe or json. Requests to the FRED API can be customized according to the parameters made available by the web service endpoints.
+`pyfredapi` is a full featured Python library that makes it is easy to retrieve data from the [Federal Reserve Economic Data](https://fred.stlouisfed.org/docs/api/fred/) (FRED) API web service. `pyfredapi` covers all the FRED api endpoints, and can retrieve data from [FRED](https://fred.stlouisfed.org/) and [ALFRED](https://alfred.stlouisfed.org). Data can be returned as a [pandas](https://pandas.pydata.org/) dataframe or json. Requests to the FRED API can be customized according to the parameters made available by the web service endpoints.
 
 ## Documentation
 
 The [documentation](https://pyfredapi.readthedocs.io/en/latest/) is made with [Sphinx](https://www.sphinx-doc.org/en/master/) and hosted on [Read the Docs](https://readthedocs.org/).
 
 ## Installation
 
 ```bash
 pip install pyfredapi
+
+# install with plotting dependencies
+pip install 'pyfredapi[plot]'
 ```
 
 ## Quick Start
 
 ### FRED API Key
 
 Before using `pyfredapi` and must have an API key to the FRED API web service. You can apply for [one for free](https://fred.stlouisfed.org/docs/api/api_key.html) on the FRED website.
 
 You can set your API key in two ways:
 
-* set your API key to the environment variable :code:`FRED_API_KEY`
+* set your API key to the environment variable `FRED_API_KEY`
 * pass it to the `api_key` parameter of the request function
 
 You can set the API key as an environment variable by adding the following line to your `~/.zshrc`, `~/.bashrc` file:
 
 ```bash
 export FRED_API_KEY="your_api_key"
 ```
```

