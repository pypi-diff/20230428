# Comparing `tmp/pyfredapi-0.7.0.tar.gz` & `tmp/pyfredapi-0.7.1.tar.gz`

## Comparing `pyfredapi-0.7.0.tar` & `pyfredapi-0.7.1.tar`

### file list

```diff
@@ -1,164 +1,164 @@
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/.readthedocs.yml
--rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/RELEASE.md
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/mypy.ini
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/requirements.txt
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/sonar-project.properties
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tox.ini
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/.github/PULL_REQUEST_TEMPLATE/version_release.md
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/.github/workflows/build-pyfredapi.yml
--rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/.github/workflows/sonarcloud.yml
--rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/.github/workflows/test.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/.nojekyll
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/Makefile
--rw-r--r--   0        0        0     2456 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/conf.py
--rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/make.bat
--rw-r--r--   0        0        0     7860 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/requirements.txt
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/_templates/layout.html
--rw-r--r--   0        0        0     4919 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/CHANGELOG.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/CONTRIBUTING.rst
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/api.rst
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi._base.BaseApiParameters.rst
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi._base._get_api_key.rst
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi._base._get_request.rst
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.category.CategoryApiParameters.rst
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.category.get_category.rst
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.category.get_category_children.rst
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.category.get_category_related.rst
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.category.get_category_related_tags.rst
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.category.get_category_series.rst
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.category.get_category_tags.rst
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.maps.MapApiParameters.rst
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.maps.get_geoseries.rst
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.maps.get_geoseries_info.rst
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.maps.get_shape_files.rst
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.releases.ReleaseApiParameters.rst
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.releases.get_release.rst
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.releases.get_release_dates.rst
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.releases.get_release_related_tags.rst
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.releases.get_release_series.rst
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.releases.get_release_tables.rst
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.releases.get_releases.rst
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.releases.get_releases_dates.rst
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.series.SeriesApiParameters.rst
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.series.SeriesInfo.rst
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.series.SeriesSearchParameters.rst
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.series.get_series.rst
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.series.get_series_all_releases.rst
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.series.get_series_asof_date.rst
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.series.get_series_categories.rst
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.series.get_series_info.rst
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.series.get_series_initial_release.rst
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.series.get_series_releases.rst
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.series.get_series_tags.rst
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.series.get_series_updates.rst
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.series.get_series_vintagedates.rst
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.series.search_series.rst
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.series.search_series_related_tags.rst
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.series.search_series_tags.rst
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.series_collection.SeriesCollection.rst
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.series_collection.SeriesData.rst
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.sources.SourceApiParameters.rst
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.sources.get_source.rst
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.sources.get_source_release.rst
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.sources.get_sources.rst
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.tags.TagsApiParameters.rst
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.tags.get_related_tags.rst
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.tags.get_series_matching_tags.rst
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.tags.get_tags.rst
--rw-r--r--   0        0        0  7594465 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/tutorials/category.ipynb
--rw-r--r--   0        0        0    51427 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/tutorials/maps.ipynb
--rw-r--r--   0        0        0    33447 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/tutorials/series.ipynb
--rw-r--r--   0        0        0    24658 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/docs/tutorials/series_collection.ipynb
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/pyfredapi/__about__.py
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/pyfredapi/__init__.py
--rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/pyfredapi/_base.py
--rw-r--r--   0        0        0     8492 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/pyfredapi/category.py
--rw-r--r--   0        0        0     5824 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/pyfredapi/maps.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/pyfredapi/py.typed
--rw-r--r--   0        0        0     9651 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/pyfredapi/releases.py
--rw-r--r--   0        0        0    21037 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/pyfredapi/series.py
--rw-r--r--   0        0        0    15460 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/pyfredapi/series_collection.py
--rw-r--r--   0        0        0     3600 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/pyfredapi/sources.py
--rw-r--r--   0        0        0     4367 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/pyfredapi/tags.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/pyfredapi/exceptions/__init__.py
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/pyfredapi/exceptions/exceptions.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/pyfredapi/utils/__init__.py
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/pyfredapi/utils/_common_type_hints.py
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/pyfredapi/utils/_convert_to_pandas.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/pyfredapi/utils/enums.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/__init__.py
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/conftest.py
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/test_base.py
--rw-r--r--   0        0        0     3427 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/test_category.py
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/test_maps.py
--rw-r--r--   0        0        0     2902 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/test_release.py
--rw-r--r--   0        0        0     7245 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/test_series.py
--rw-r--r--   0        0        0     4174 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/test_series_collection.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/test_sources.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/test_tags.py
--rw-r--r--   0        0        0     4105 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_category/test_get_category.yaml
--rw-r--r--   0        0        0     3865 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_category/test_get_category_children.yaml
--rw-r--r--   0        0        0     3861 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_category/test_get_category_related.yaml
--rw-r--r--   0        0        0     8817 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_category/test_get_category_related_tags[json].yaml
--rw-r--r--   0        0        0     4421 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_category/test_get_category_related_tags[pandas].yaml
--rw-r--r--   0        0        0    20720 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_category/test_get_category_series.yaml
--rw-r--r--   0        0        0     8909 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_category/test_get_category_tags[json].yaml
--rw-r--r--   0        0        0     4467 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_category/test_get_category_tags[pandas].yaml
--rw-r--r--   0        0        0    23177 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_maps/test_get_geoseries[json].yaml
--rw-r--r--   0        0        0    11620 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_maps/test_get_geoseries[pandas].yaml
--rw-r--r--   0        0        0     4793 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_maps/test_get_geoseries_info.yaml
--rw-r--r--   0        0        0   128005 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_maps/test_get_shape_files.yaml
--rw-r--r--   0        0        0     4599 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_release/test_get_release.yaml
--rw-r--r--   0        0        0    34170 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_release/test_get_release_dates.yaml
--rw-r--r--   0        0        0     4581 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_release/test_get_release_related_tags.yaml
--rw-r--r--   0        0        0   122146 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_release/test_get_release_series.yaml
--rw-r--r--   0        0        0     4567 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_release/test_get_release_sources.yaml
--rw-r--r--   0        0        0     5060 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_release/test_get_release_tables.yaml
--rw-r--r--   0        0        0    28278 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_release/test_get_release_tags.yaml
--rw-r--r--   0        0        0   307432 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_release/test_get_releases.yaml
--rw-r--r--   0        0        0    69442 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_release/test_get_releases_dates.yaml
--rw-r--r--   0        0        0    29017 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_series/test_get_series[json].yaml
--rw-r--r--   0        0        0    14521 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_series/test_get_series[pandas].yaml
--rw-r--r--   0        0        0   241057 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_series/test_get_series_all_releases[json].yaml
--rw-r--r--   0        0        0   120541 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_series/test_get_series_all_releases[pandas].yaml
--rw-r--r--   0        0        0   219867 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_series/test_get_series_asof_date[json].yaml
--rw-r--r--   0        0        0   109946 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_series/test_get_series_asof_date[pandas].yaml
--rw-r--r--   0        0        0     4097 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_series/test_get_series_categories.yaml
--rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_series/test_get_series_info.yaml
--rw-r--r--   0        0        0    23366 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_series/test_get_series_initial_release[json].yaml
--rw-r--r--   0        0        0    11839 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_series/test_get_series_initial_release[pandas].yaml
--rw-r--r--   0        0        0     4757 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_series/test_get_series_releases.yaml
--rw-r--r--   0        0        0     7269 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_series/test_get_series_tags.yaml
--rw-r--r--   0        0        0   242266 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_series/test_get_series_updates.yaml
--rw-r--r--   0        0        0    15816 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_series/test_get_series_vintagedates.yaml
--rw-r--r--   0        0        0   198782 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_series/test_search_series[json].yaml
--rw-r--r--   0        0        0    99412 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_series/test_search_series[pandas].yaml
--rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_series/test_search_series_related_tags[json].yaml
--rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_series/test_search_series_related_tags[pandas].yaml
--rw-r--r--   0        0        0    55891 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_series/test_search_series_tags[json].yaml
--rw-r--r--   0        0        0    27958 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_series/test_search_series_tags[pandas].yaml
--rw-r--r--   0        0        0    35967 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_series_collection/test_add_series.yaml
--rw-r--r--   0        0        0    32455 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_series_collection/test_drop_series.yaml
--rw-r--r--   0        0        0    94151 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_series_collection/test_list_methods_diff.yaml
--rw-r--r--   0        0        0    46911 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_series_collection/test_remove_series.yaml
--rw-r--r--   0        0        0    17997 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_series_collection/test_rename_err.yaml
--rw-r--r--   0        0        0    18283 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_series_collection/test_rename_on_add[dict].yaml
--rw-r--r--   0        0        0    17997 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_series_collection/test_rename_on_add[func].yaml
--rw-r--r--   0        0        0    14483 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_series_collection/test_rename_partial.yaml
--rw-r--r--   0        0        0     4669 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_sources/test_get_source.yaml
--rw-r--r--   0        0        0    34693 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_sources/test_get_source_release.yaml
--rw-r--r--   0        0        0    37658 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_sources/test_get_sources.yaml
--rw-r--r--   0        0        0   156345 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_tags/test_get_related_tags.yaml
--rw-r--r--   0        0        0    12864 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_tags/test_get_tag_series.yaml
--rw-r--r--   0        0        0   151305 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/tests/vhs/test_tags/test_get_tags.yaml
--rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/LICENSE
--rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/README.md
--rw-r--r--   0        0        0     3969 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     7105 2020-02-02 00:00:00.000000 pyfredapi-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/.readthedocs.yml
+-rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/RELEASE.md
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/mypy.ini
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/requirements.txt
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/sonar-project.properties
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tox.ini
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/.github/PULL_REQUEST_TEMPLATE/version_release.md
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/.github/workflows/build-pyfredapi.yml
+-rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/.github/workflows/sonarcloud.yml
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/docs/.nojekyll
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/docs/Makefile
+-rw-r--r--   0        0        0     2456 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/docs/conf.py
+-rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/docs/make.bat
+-rw-r--r--   0        0        0     7960 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/docs/requirements.txt
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/docs/_templates/layout.html
+-rw-r--r--   0        0        0     5079 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/docs/references/CHANGELOG.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/docs/references/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/docs/references/api.rst
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/docs/references/_autosummary/pyfredapi._base.BaseApiParameters.rst
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/docs/references/_autosummary/pyfredapi._base._get_api_key.rst
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/docs/references/_autosummary/pyfredapi._base._get_request.rst
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/docs/references/_autosummary/pyfredapi.category.CategoryApiParameters.rst
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/docs/references/_autosummary/pyfredapi.category.get_category.rst
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/docs/references/_autosummary/pyfredapi.category.get_category_children.rst
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/docs/references/_autosummary/pyfredapi.category.get_category_related.rst
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/docs/references/_autosummary/pyfredapi.category.get_category_related_tags.rst
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/docs/references/_autosummary/pyfredapi.category.get_category_series.rst
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/docs/references/_autosummary/pyfredapi.category.get_category_tags.rst
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/docs/references/_autosummary/pyfredapi.maps.MapApiParameters.rst
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/docs/references/_autosummary/pyfredapi.maps.get_geoseries.rst
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/docs/references/_autosummary/pyfredapi.maps.get_geoseries_info.rst
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/docs/references/_autosummary/pyfredapi.maps.get_shape_files.rst
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/docs/references/_autosummary/pyfredapi.releases.ReleaseApiParameters.rst
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/docs/references/_autosummary/pyfredapi.releases.get_release.rst
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/docs/references/_autosummary/pyfredapi.releases.get_release_dates.rst
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/docs/references/_autosummary/pyfredapi.releases.get_release_related_tags.rst
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/docs/references/_autosummary/pyfredapi.releases.get_release_series.rst
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/docs/references/_autosummary/pyfredapi.releases.get_release_tables.rst
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/docs/references/_autosummary/pyfredapi.releases.get_releases.rst
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/docs/references/_autosummary/pyfredapi.releases.get_releases_dates.rst
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/docs/references/_autosummary/pyfredapi.series.SeriesApiParameters.rst
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/docs/references/_autosummary/pyfredapi.series.SeriesInfo.rst
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/docs/references/_autosummary/pyfredapi.series.SeriesSearchParameters.rst
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/docs/references/_autosummary/pyfredapi.series.get_series.rst
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/docs/references/_autosummary/pyfredapi.series.get_series_all_releases.rst
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/docs/references/_autosummary/pyfredapi.series.get_series_asof_date.rst
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/docs/references/_autosummary/pyfredapi.series.get_series_categories.rst
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/docs/references/_autosummary/pyfredapi.series.get_series_info.rst
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/docs/references/_autosummary/pyfredapi.series.get_series_initial_release.rst
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/docs/references/_autosummary/pyfredapi.series.get_series_releases.rst
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/docs/references/_autosummary/pyfredapi.series.get_series_tags.rst
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/docs/references/_autosummary/pyfredapi.series.get_series_updates.rst
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/docs/references/_autosummary/pyfredapi.series.get_series_vintagedates.rst
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/docs/references/_autosummary/pyfredapi.series.search_series.rst
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/docs/references/_autosummary/pyfredapi.series.search_series_related_tags.rst
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/docs/references/_autosummary/pyfredapi.series.search_series_tags.rst
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/docs/references/_autosummary/pyfredapi.series_collection.SeriesCollection.rst
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/docs/references/_autosummary/pyfredapi.series_collection.SeriesData.rst
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/docs/references/_autosummary/pyfredapi.sources.SourceApiParameters.rst
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/docs/references/_autosummary/pyfredapi.sources.get_source.rst
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/docs/references/_autosummary/pyfredapi.sources.get_source_release.rst
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/docs/references/_autosummary/pyfredapi.sources.get_sources.rst
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/docs/references/_autosummary/pyfredapi.tags.TagsApiParameters.rst
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/docs/references/_autosummary/pyfredapi.tags.get_related_tags.rst
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/docs/references/_autosummary/pyfredapi.tags.get_series_matching_tags.rst
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/docs/references/_autosummary/pyfredapi.tags.get_tags.rst
+-rw-r--r--   0        0        0  7594438 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/docs/tutorials/category.ipynb
+-rw-r--r--   0        0        0    51427 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/docs/tutorials/maps.ipynb
+-rw-r--r--   0        0        0    33447 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/docs/tutorials/series.ipynb
+-rw-r--r--   0        0        0    24658 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/docs/tutorials/series_collection.ipynb
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/pyfredapi/__about__.py
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/pyfredapi/__init__.py
+-rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/pyfredapi/_base.py
+-rw-r--r--   0        0        0     8492 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/pyfredapi/category.py
+-rw-r--r--   0        0        0     5824 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/pyfredapi/maps.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/pyfredapi/py.typed
+-rw-r--r--   0        0        0     9651 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/pyfredapi/releases.py
+-rw-r--r--   0        0        0    21037 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/pyfredapi/series.py
+-rw-r--r--   0        0        0    15462 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/pyfredapi/series_collection.py
+-rw-r--r--   0        0        0     3600 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/pyfredapi/sources.py
+-rw-r--r--   0        0        0     4367 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/pyfredapi/tags.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/pyfredapi/exceptions/__init__.py
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/pyfredapi/exceptions/exceptions.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/pyfredapi/utils/__init__.py
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/pyfredapi/utils/_common_type_hints.py
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/pyfredapi/utils/_convert_to_pandas.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/pyfredapi/utils/enums.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tests/__init__.py
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tests/conftest.py
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tests/test_base.py
+-rw-r--r--   0        0        0     3427 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tests/test_category.py
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tests/test_maps.py
+-rw-r--r--   0        0        0     2902 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tests/test_release.py
+-rw-r--r--   0        0        0     7245 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tests/test_series.py
+-rw-r--r--   0        0        0     4174 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tests/test_series_collection.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tests/test_sources.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tests/test_tags.py
+-rw-r--r--   0        0        0     4105 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tests/vhs/test_category/test_get_category.yaml
+-rw-r--r--   0        0        0     3865 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tests/vhs/test_category/test_get_category_children.yaml
+-rw-r--r--   0        0        0     3861 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tests/vhs/test_category/test_get_category_related.yaml
+-rw-r--r--   0        0        0     8817 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tests/vhs/test_category/test_get_category_related_tags[json].yaml
+-rw-r--r--   0        0        0     4421 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tests/vhs/test_category/test_get_category_related_tags[pandas].yaml
+-rw-r--r--   0        0        0    20720 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tests/vhs/test_category/test_get_category_series.yaml
+-rw-r--r--   0        0        0     8909 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tests/vhs/test_category/test_get_category_tags[json].yaml
+-rw-r--r--   0        0        0     4467 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tests/vhs/test_category/test_get_category_tags[pandas].yaml
+-rw-r--r--   0        0        0    23177 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tests/vhs/test_maps/test_get_geoseries[json].yaml
+-rw-r--r--   0        0        0    11620 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tests/vhs/test_maps/test_get_geoseries[pandas].yaml
+-rw-r--r--   0        0        0     4793 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tests/vhs/test_maps/test_get_geoseries_info.yaml
+-rw-r--r--   0        0        0   128005 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tests/vhs/test_maps/test_get_shape_files.yaml
+-rw-r--r--   0        0        0     4599 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tests/vhs/test_release/test_get_release.yaml
+-rw-r--r--   0        0        0    34170 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tests/vhs/test_release/test_get_release_dates.yaml
+-rw-r--r--   0        0        0     4581 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tests/vhs/test_release/test_get_release_related_tags.yaml
+-rw-r--r--   0        0        0   122146 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tests/vhs/test_release/test_get_release_series.yaml
+-rw-r--r--   0        0        0     4567 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tests/vhs/test_release/test_get_release_sources.yaml
+-rw-r--r--   0        0        0     5060 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tests/vhs/test_release/test_get_release_tables.yaml
+-rw-r--r--   0        0        0    28278 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tests/vhs/test_release/test_get_release_tags.yaml
+-rw-r--r--   0        0        0   307432 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tests/vhs/test_release/test_get_releases.yaml
+-rw-r--r--   0        0        0    69442 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tests/vhs/test_release/test_get_releases_dates.yaml
+-rw-r--r--   0        0        0    29017 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tests/vhs/test_series/test_get_series[json].yaml
+-rw-r--r--   0        0        0    14521 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tests/vhs/test_series/test_get_series[pandas].yaml
+-rw-r--r--   0        0        0   241057 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tests/vhs/test_series/test_get_series_all_releases[json].yaml
+-rw-r--r--   0        0        0   120541 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tests/vhs/test_series/test_get_series_all_releases[pandas].yaml
+-rw-r--r--   0        0        0   219867 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tests/vhs/test_series/test_get_series_asof_date[json].yaml
+-rw-r--r--   0        0        0   109946 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tests/vhs/test_series/test_get_series_asof_date[pandas].yaml
+-rw-r--r--   0        0        0     4097 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tests/vhs/test_series/test_get_series_categories.yaml
+-rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tests/vhs/test_series/test_get_series_info.yaml
+-rw-r--r--   0        0        0    23366 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tests/vhs/test_series/test_get_series_initial_release[json].yaml
+-rw-r--r--   0        0        0    11839 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tests/vhs/test_series/test_get_series_initial_release[pandas].yaml
+-rw-r--r--   0        0        0     4757 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tests/vhs/test_series/test_get_series_releases.yaml
+-rw-r--r--   0        0        0     7269 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tests/vhs/test_series/test_get_series_tags.yaml
+-rw-r--r--   0        0        0   242266 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tests/vhs/test_series/test_get_series_updates.yaml
+-rw-r--r--   0        0        0    15816 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tests/vhs/test_series/test_get_series_vintagedates.yaml
+-rw-r--r--   0        0        0   198782 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tests/vhs/test_series/test_search_series[json].yaml
+-rw-r--r--   0        0        0    99412 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tests/vhs/test_series/test_search_series[pandas].yaml
+-rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tests/vhs/test_series/test_search_series_related_tags[json].yaml
+-rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tests/vhs/test_series/test_search_series_related_tags[pandas].yaml
+-rw-r--r--   0        0        0    55891 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tests/vhs/test_series/test_search_series_tags[json].yaml
+-rw-r--r--   0        0        0    27958 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tests/vhs/test_series/test_search_series_tags[pandas].yaml
+-rw-r--r--   0        0        0    35967 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tests/vhs/test_series_collection/test_add_series.yaml
+-rw-r--r--   0        0        0    32455 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tests/vhs/test_series_collection/test_drop_series.yaml
+-rw-r--r--   0        0        0    94151 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tests/vhs/test_series_collection/test_list_methods_diff.yaml
+-rw-r--r--   0        0        0    46911 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tests/vhs/test_series_collection/test_remove_series.yaml
+-rw-r--r--   0        0        0    17997 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tests/vhs/test_series_collection/test_rename_err.yaml
+-rw-r--r--   0        0        0    18283 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tests/vhs/test_series_collection/test_rename_on_add[dict].yaml
+-rw-r--r--   0        0        0    17997 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tests/vhs/test_series_collection/test_rename_on_add[func].yaml
+-rw-r--r--   0        0        0    14483 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tests/vhs/test_series_collection/test_rename_partial.yaml
+-rw-r--r--   0        0        0     4669 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tests/vhs/test_sources/test_get_source.yaml
+-rw-r--r--   0        0        0    34693 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tests/vhs/test_sources/test_get_source_release.yaml
+-rw-r--r--   0        0        0    37658 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tests/vhs/test_sources/test_get_sources.yaml
+-rw-r--r--   0        0        0   156345 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tests/vhs/test_tags/test_get_related_tags.yaml
+-rw-r--r--   0        0        0    12864 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tests/vhs/test_tags/test_get_tag_series.yaml
+-rw-r--r--   0        0        0   151305 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/tests/vhs/test_tags/test_get_tags.yaml
+-rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/LICENSE
+-rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/README.md
+-rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     7205 2020-02-02 00:00:00.000000 pyfredapi-0.7.1/PKG-INFO
```

### Comparing `pyfredapi-0.7.0/.pre-commit-config.yaml` & `pyfredapi-0.7.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/CONTRIBUTING.md` & `pyfredapi-0.7.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/RELEASE.md` & `pyfredapi-0.7.1/RELEASE.md`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/requirements.txt` & `pyfredapi-0.7.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/tox.ini` & `pyfredapi-0.7.1/tox.ini`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/.github/ISSUE_TEMPLATE/bug.md` & `pyfredapi-0.7.1/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/.github/ISSUE_TEMPLATE/feature_request.md` & `pyfredapi-0.7.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md` & `pyfredapi-0.7.1/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/.github/workflows/build-pyfredapi.yml` & `pyfredapi-0.7.1/.github/workflows/build-pyfredapi.yml`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/.github/workflows/sonarcloud.yml` & `pyfredapi-0.7.1/.github/workflows/sonarcloud.yml`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/.github/workflows/test.yml` & `pyfredapi-0.7.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/docs/Makefile` & `pyfredapi-0.7.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/docs/conf.py` & `pyfredapi-0.7.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/docs/index.rst` & `pyfredapi-0.7.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/docs/make.bat` & `pyfredapi-0.7.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/docs/requirements.txt` & `pyfredapi-0.7.1/docs/requirements.txt`

 * *Files 4% similar despite different names*

```diff
@@ -205,14 +205,15 @@
 numpy==1.24.2
     # via pandas
 packaging==23.1
     # via
     #   ipykernel
     #   jupyter-server
     #   nbconvert
+    #   plotly
     #   qtconsole
     #   qtpy
     #   sphinx
 pandas==1.5.3
     # via pyfredapi (pyproject.toml)
 pandocfilters==1.5.0
     # via nbconvert
@@ -220,14 +221,16 @@
     # via jedi
 pexpect==4.8.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
 platformdirs==3.2.0
     # via jupyter-core
+plotly==5.14.1
+    # via pyfredapi (pyproject.toml)
 pockets==0.9.1
     # via sphinxcontrib-napoleon
 prometheus-client==0.16.0
     # via
     #   jupyter-server
     #   nbclassic
     #   notebook
@@ -344,14 +347,16 @@
     # via pyfredapi (pyproject.toml)
 sphinxcontrib-qthelp==1.0.3
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.5
     # via sphinx
 stack-data==0.6.2
     # via ipython
+tenacity==8.2.2
+    # via plotly
 terminado==0.17.1
     # via
     #   jupyter-server
     #   jupyter-server-terminals
     #   nbclassic
     #   notebook
 text-unidecode==1.3
```

### Comparing `pyfredapi-0.7.0/docs/references/CHANGELOG.md` & `pyfredapi-0.7.1/docs/references/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # Changelog
 
 ## UNRELEASED
 
+## Version 0.7.1 - 2023-04-27
+
+### Fixed
+
+- Import error in `SeriesCollection` when `plotly` is not installed.
+- Updated dev dependencies to include `plotly`.
+
 ## Version 0.7.0 - 2023-04-27
 
 ### Changed
 
 - Refactor `SeriesCollection`'s internal structure to represent a sequence.
   - Updated `__init__` to handle adding the initial set of series.
   - `SeriesCollection` is now iterable, indexable, and sized.
```

### Comparing `pyfredapi-0.7.0/docs/references/api.rst` & `pyfredapi-0.7.1/docs/references/api.rst`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/docs/references/_autosummary/pyfredapi.series_collection.SeriesCollection.rst` & `pyfredapi-0.7.1/docs/references/_autosummary/pyfredapi.series_collection.SeriesCollection.rst`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/docs/tutorials/category.ipynb` & `pyfredapi-0.7.1/docs/tutorials/category.ipynb`

 * *Files 0% similar despite different names*

```diff
@@ -278,16 +278,16 @@
   {
    "cell_type": "code",
    "execution_count": 11,
    "metadata": {},
    "outputs": [],
    "source": [
     "long_df = unemployment_sc.merge_long()\n",
-    "min_date = min(long_df['date'].dt.date)\n",
-    "max_date = max(long_df['date'].dt.date)"
+    "min_date = min(long_df[\"date\"].dt.date)\n",
+    "max_date = max(long_df[\"date\"].dt.date)"
    ]
   },
   {
    "cell_type": "markdown",
    "metadata": {},
    "source": [
     "### Bar Chart"
@@ -364,17 +364,15 @@
    "source": [
     "bar_chart = px.bar(\n",
     "    long_df[long_df[\"date\"] == max(long_df[\"date\"])],\n",
     "    x=\"series\",\n",
     "    y=\"value\",\n",
     "    color=\"series\",\n",
     "    title=f\"U.S. Unemployment Rate, Seasonally Adjusted, {max_date}\",\n",
-    "    labels={\n",
-    "        \"value\": \"Unemployment Rate\"\n",
-    "    },\n",
+    "    labels={\"value\": \"Unemployment Rate\"},\n",
     "    color_discrete_sequence=px.colors.qualitative.Safe,\n",
     ")\n",
     "\n",
     "bar_chart.update_layout(showlegend=False)\n",
     "bar_chart.show(renderer=\"notebook\")"
    ]
   },
@@ -460,15 +458,15 @@
     "    x=\"date\",\n",
     "    y=\"value\",\n",
     "    color=\"series\",\n",
     "    title=f\"U.S. Unemployment Rate, Seasonally Adjusted, {min_date} - {max_date}\",\n",
     "    labels={\n",
     "        \"value\": \"Unemployment Rate\",\n",
     "        \"date\": \"Date\",\n",
-    "        \"series\": \"Unemployment Series\"\n",
+    "        \"series\": \"Unemployment Series\",\n",
     "    },\n",
     "    color_discrete_sequence=px.colors.qualitative.Safe,\n",
     ")\n",
     "\n",
     "time_series_plot.show(renderer=\"notebook\")"
    ]
   }
```

### Comparing `pyfredapi-0.7.0/docs/tutorials/maps.ipynb` & `pyfredapi-0.7.1/docs/tutorials/maps.ipynb`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/docs/tutorials/series.ipynb` & `pyfredapi-0.7.1/docs/tutorials/series.ipynb`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/docs/tutorials/series_collection.ipynb` & `pyfredapi-0.7.1/docs/tutorials/series_collection.ipynb`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/pyfredapi/__init__.py` & `pyfredapi-0.7.1/pyfredapi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/pyfredapi/_base.py` & `pyfredapi-0.7.1/pyfredapi/_base.py`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/pyfredapi/category.py` & `pyfredapi-0.7.1/pyfredapi/category.py`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/pyfredapi/maps.py` & `pyfredapi-0.7.1/pyfredapi/maps.py`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/pyfredapi/releases.py` & `pyfredapi-0.7.1/pyfredapi/releases.py`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/pyfredapi/series.py` & `pyfredapi-0.7.1/pyfredapi/series.py`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/pyfredapi/series_collection.py` & `pyfredapi-0.7.1/pyfredapi/series_collection.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     data : pd.DataFrame
         Series data in a pandas dataframe.
     """
 
     info: SeriesInfo
     df: pd.DataFrame
 
-    def plot(self) -> Figure:
+    def plot(self) -> "Figure":
         """Create a `plotly <https://plotly.com/python/>`_ time series plot.
 
         Raises
         ------
         ValueError
             If data format is not a pandas dataframe.
```

### Comparing `pyfredapi-0.7.0/pyfredapi/sources.py` & `pyfredapi-0.7.1/pyfredapi/sources.py`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/pyfredapi/tags.py` & `pyfredapi-0.7.1/pyfredapi/tags.py`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/pyfredapi/exceptions/exceptions.py` & `pyfredapi-0.7.1/pyfredapi/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/pyfredapi/utils/_convert_to_pandas.py` & `pyfredapi-0.7.1/pyfredapi/utils/_convert_to_pandas.py`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/tests/conftest.py` & `pyfredapi-0.7.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/tests/test_base.py` & `pyfredapi-0.7.1/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/tests/test_category.py` & `pyfredapi-0.7.1/tests/test_category.py`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/tests/test_maps.py` & `pyfredapi-0.7.1/tests/test_maps.py`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/tests/test_release.py` & `pyfredapi-0.7.1/tests/test_release.py`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/tests/test_series.py` & `pyfredapi-0.7.1/tests/test_series.py`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/tests/test_series_collection.py` & `pyfredapi-0.7.1/tests/test_series_collection.py`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/tests/test_sources.py` & `pyfredapi-0.7.1/tests/test_sources.py`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/tests/test_tags.py` & `pyfredapi-0.7.1/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/tests/vhs/test_category/test_get_category.yaml` & `pyfredapi-0.7.1/tests/vhs/test_category/test_get_category.yaml`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/tests/vhs/test_category/test_get_category_children.yaml` & `pyfredapi-0.7.1/tests/vhs/test_category/test_get_category_children.yaml`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/tests/vhs/test_category/test_get_category_related.yaml` & `pyfredapi-0.7.1/tests/vhs/test_category/test_get_category_related.yaml`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/tests/vhs/test_category/test_get_category_related_tags[json].yaml` & `pyfredapi-0.7.1/tests/vhs/test_category/test_get_category_related_tags[json].yaml`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/tests/vhs/test_category/test_get_category_related_tags[pandas].yaml` & `pyfredapi-0.7.1/tests/vhs/test_category/test_get_category_related_tags[pandas].yaml`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/tests/vhs/test_category/test_get_category_series.yaml` & `pyfredapi-0.7.1/tests/vhs/test_category/test_get_category_series.yaml`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/tests/vhs/test_category/test_get_category_tags[json].yaml` & `pyfredapi-0.7.1/tests/vhs/test_category/test_get_category_tags[json].yaml`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/tests/vhs/test_category/test_get_category_tags[pandas].yaml` & `pyfredapi-0.7.1/tests/vhs/test_category/test_get_category_tags[pandas].yaml`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/tests/vhs/test_maps/test_get_geoseries[json].yaml` & `pyfredapi-0.7.1/tests/vhs/test_maps/test_get_geoseries[json].yaml`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/tests/vhs/test_maps/test_get_geoseries[pandas].yaml` & `pyfredapi-0.7.1/tests/vhs/test_maps/test_get_geoseries[pandas].yaml`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/tests/vhs/test_maps/test_get_geoseries_info.yaml` & `pyfredapi-0.7.1/tests/vhs/test_maps/test_get_geoseries_info.yaml`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/tests/vhs/test_maps/test_get_shape_files.yaml` & `pyfredapi-0.7.1/tests/vhs/test_maps/test_get_shape_files.yaml`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/tests/vhs/test_release/test_get_release.yaml` & `pyfredapi-0.7.1/tests/vhs/test_release/test_get_release.yaml`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/tests/vhs/test_release/test_get_release_dates.yaml` & `pyfredapi-0.7.1/tests/vhs/test_release/test_get_release_dates.yaml`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/tests/vhs/test_release/test_get_release_related_tags.yaml` & `pyfredapi-0.7.1/tests/vhs/test_release/test_get_release_related_tags.yaml`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/tests/vhs/test_release/test_get_release_series.yaml` & `pyfredapi-0.7.1/tests/vhs/test_release/test_get_release_series.yaml`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/tests/vhs/test_release/test_get_release_sources.yaml` & `pyfredapi-0.7.1/tests/vhs/test_release/test_get_release_sources.yaml`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/tests/vhs/test_release/test_get_release_tables.yaml` & `pyfredapi-0.7.1/tests/vhs/test_release/test_get_release_tables.yaml`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/tests/vhs/test_release/test_get_release_tags.yaml` & `pyfredapi-0.7.1/tests/vhs/test_release/test_get_release_tags.yaml`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/tests/vhs/test_release/test_get_releases.yaml` & `pyfredapi-0.7.1/tests/vhs/test_release/test_get_releases.yaml`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/tests/vhs/test_release/test_get_releases_dates.yaml` & `pyfredapi-0.7.1/tests/vhs/test_release/test_get_releases_dates.yaml`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/tests/vhs/test_series/test_get_series[json].yaml` & `pyfredapi-0.7.1/tests/vhs/test_series/test_get_series[json].yaml`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/tests/vhs/test_series/test_get_series[pandas].yaml` & `pyfredapi-0.7.1/tests/vhs/test_series/test_get_series[pandas].yaml`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/tests/vhs/test_series/test_get_series_all_releases[json].yaml` & `pyfredapi-0.7.1/tests/vhs/test_series/test_get_series_all_releases[json].yaml`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/tests/vhs/test_series/test_get_series_all_releases[pandas].yaml` & `pyfredapi-0.7.1/tests/vhs/test_series/test_get_series_all_releases[pandas].yaml`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/tests/vhs/test_series/test_get_series_asof_date[json].yaml` & `pyfredapi-0.7.1/tests/vhs/test_series/test_get_series_asof_date[json].yaml`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/tests/vhs/test_series/test_get_series_asof_date[pandas].yaml` & `pyfredapi-0.7.1/tests/vhs/test_series/test_get_series_asof_date[pandas].yaml`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/tests/vhs/test_series/test_get_series_categories.yaml` & `pyfredapi-0.7.1/tests/vhs/test_series/test_get_series_categories.yaml`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/tests/vhs/test_series/test_get_series_info.yaml` & `pyfredapi-0.7.1/tests/vhs/test_series/test_get_series_info.yaml`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/tests/vhs/test_series/test_get_series_initial_release[json].yaml` & `pyfredapi-0.7.1/tests/vhs/test_series/test_get_series_initial_release[json].yaml`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/tests/vhs/test_series/test_get_series_initial_release[pandas].yaml` & `pyfredapi-0.7.1/tests/vhs/test_series/test_get_series_initial_release[pandas].yaml`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/tests/vhs/test_series/test_get_series_releases.yaml` & `pyfredapi-0.7.1/tests/vhs/test_series/test_get_series_releases.yaml`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/tests/vhs/test_series/test_get_series_tags.yaml` & `pyfredapi-0.7.1/tests/vhs/test_series/test_get_series_tags.yaml`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/tests/vhs/test_series/test_get_series_updates.yaml` & `pyfredapi-0.7.1/tests/vhs/test_series/test_get_series_updates.yaml`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/tests/vhs/test_series/test_get_series_vintagedates.yaml` & `pyfredapi-0.7.1/tests/vhs/test_series/test_get_series_vintagedates.yaml`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/tests/vhs/test_series/test_search_series[json].yaml` & `pyfredapi-0.7.1/tests/vhs/test_series/test_search_series[json].yaml`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/tests/vhs/test_series/test_search_series[pandas].yaml` & `pyfredapi-0.7.1/tests/vhs/test_series/test_search_series[pandas].yaml`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/tests/vhs/test_series/test_search_series_related_tags[json].yaml` & `pyfredapi-0.7.1/tests/vhs/test_series/test_search_series_related_tags[json].yaml`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/tests/vhs/test_series/test_search_series_related_tags[pandas].yaml` & `pyfredapi-0.7.1/tests/vhs/test_series/test_search_series_related_tags[pandas].yaml`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/tests/vhs/test_series/test_search_series_tags[json].yaml` & `pyfredapi-0.7.1/tests/vhs/test_series/test_search_series_tags[json].yaml`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/tests/vhs/test_series/test_search_series_tags[pandas].yaml` & `pyfredapi-0.7.1/tests/vhs/test_series/test_search_series_tags[pandas].yaml`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/tests/vhs/test_series_collection/test_add_series.yaml` & `pyfredapi-0.7.1/tests/vhs/test_series_collection/test_add_series.yaml`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/tests/vhs/test_series_collection/test_drop_series.yaml` & `pyfredapi-0.7.1/tests/vhs/test_series_collection/test_drop_series.yaml`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/tests/vhs/test_series_collection/test_list_methods_diff.yaml` & `pyfredapi-0.7.1/tests/vhs/test_series_collection/test_list_methods_diff.yaml`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/tests/vhs/test_series_collection/test_remove_series.yaml` & `pyfredapi-0.7.1/tests/vhs/test_series_collection/test_remove_series.yaml`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/tests/vhs/test_series_collection/test_rename_err.yaml` & `pyfredapi-0.7.1/tests/vhs/test_series_collection/test_rename_err.yaml`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/tests/vhs/test_series_collection/test_rename_on_add[dict].yaml` & `pyfredapi-0.7.1/tests/vhs/test_series_collection/test_rename_on_add[dict].yaml`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/tests/vhs/test_series_collection/test_rename_on_add[func].yaml` & `pyfredapi-0.7.1/tests/vhs/test_series_collection/test_rename_on_add[func].yaml`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/tests/vhs/test_series_collection/test_rename_partial.yaml` & `pyfredapi-0.7.1/tests/vhs/test_series_collection/test_rename_partial.yaml`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/tests/vhs/test_sources/test_get_source.yaml` & `pyfredapi-0.7.1/tests/vhs/test_sources/test_get_source.yaml`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/tests/vhs/test_sources/test_get_source_release.yaml` & `pyfredapi-0.7.1/tests/vhs/test_sources/test_get_source_release.yaml`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/tests/vhs/test_sources/test_get_sources.yaml` & `pyfredapi-0.7.1/tests/vhs/test_sources/test_get_sources.yaml`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/tests/vhs/test_tags/test_get_related_tags.yaml` & `pyfredapi-0.7.1/tests/vhs/test_tags/test_get_related_tags.yaml`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/tests/vhs/test_tags/test_get_tag_series.yaml` & `pyfredapi-0.7.1/tests/vhs/test_tags/test_get_tag_series.yaml`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/tests/vhs/test_tags/test_get_tags.yaml` & `pyfredapi-0.7.1/tests/vhs/test_tags/test_get_tags.yaml`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/.gitignore` & `pyfredapi-0.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/LICENSE` & `pyfredapi-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/README.md` & `pyfredapi-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `pyfredapi-0.7.0/pyproject.toml` & `pyfredapi-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 dynamic = ["version"]
 
 [project.optional-dependencies]
 plot = [
     "plotly>=5.0.0,<6.0.0",
 ]
 docs = [
+    "plotly>=5.0.0,<6.0.0",
     "jupyter==1.0.0",
     "Sphinx==6.1.3",
     "myst-parser==1.0.0",
     "nbsphinx==0.9.1",
     "sphinxcontrib-napoleon==0.7",
     "sphinx-copybutton==0.5.1",
     "sphinx-material==0.0.35",
@@ -75,14 +76,15 @@
     "coverage==7.2.2",
     "pytest-cov==4.0.0",
     "pytest-vcr==1.0.2",
 ]
 
 dev = [
     "pip-tools==6.13.0",
+    "pyfredapi[plot]",
     "pyfredapi[docs]",
     "pyfredapi[lint]",
     "pyfredapi[test]",
 ]
 
 [tool.hatch.version]
 path = "pyfredapi/__about__.py"
```

### Comparing `pyfredapi-0.7.0/PKG-INFO` & `pyfredapi-0.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfredapi
-Version: 0.7.0
+Version: 0.7.1
 Summary: A full featured API client for the FRED API web service.
 Project-URL: Homepage, https://pyfredapi.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/gw-moore/pyfredapi
 Author-email: Greg Moore <gwmoore.career@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: economic data,economic data api,economic data api client,economic indicators,economic statistics,economic time series,economics,federal reserve,fred
@@ -24,20 +24,22 @@
 Requires-Dist: pydantic<2.0.0,>=1.0.0
 Requires-Dist: requests<3.0.0,>=2.0.0
 Requires-Dist: rich<14.0.0,>=13.0.0
 Provides-Extra: dev
 Requires-Dist: pip-tools==6.13.0; extra == 'dev'
 Requires-Dist: pyfredapi[docs]; extra == 'dev'
 Requires-Dist: pyfredapi[lint]; extra == 'dev'
+Requires-Dist: pyfredapi[plot]; extra == 'dev'
 Requires-Dist: pyfredapi[test]; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: autodoc-pydantic==1.8.0; extra == 'docs'
 Requires-Dist: jupyter==1.0.0; extra == 'docs'
 Requires-Dist: myst-parser==1.0.0; extra == 'docs'
 Requires-Dist: nbsphinx==0.9.1; extra == 'docs'
+Requires-Dist: plotly<6.0.0,>=5.0.0; extra == 'docs'
 Requires-Dist: sphinx-copybutton==0.5.1; extra == 'docs'
 Requires-Dist: sphinx-material==0.0.35; extra == 'docs'
 Requires-Dist: sphinx==6.1.3; extra == 'docs'
 Requires-Dist: sphinxcontrib-napoleon==0.7; extra == 'docs'
 Provides-Extra: lint
 Requires-Dist: black[jupyter]==23.3.0; extra == 'lint'
 Requires-Dist: mypy==1.1.1; extra == 'lint'
```

