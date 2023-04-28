# Comparing `tmp/sink_pypi-0.2.4.tar.gz` & `tmp/sink_pypi-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sink_pypi-0.2.4.tar", max compression
+gzip compressed data, was "sink_pypi-0.2.5.tar", max compression
```

## Comparing `sink_pypi-0.2.4.tar` & `sink_pypi-0.2.5.tar`

### file list

```diff
@@ -1,190 +1,190 @@
--rw-r--r--   0        0        0    11334 2023-04-27 10:18:25.106682 sink_pypi-0.2.4/LICENSE
--rw-r--r--   0        0        0     8243 2023-04-27 10:18:25.106682 sink_pypi-0.2.4/README.md
--rw-r--r--   0        0        0     1894 2023-04-27 10:18:25.106682 sink_pypi-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     1968 2023-04-27 10:18:25.106682 sink_pypi-0.2.4/src/sink/__init__.py
--rw-r--r--   0        0        0    45503 2023-04-27 10:18:25.106682 sink_pypi-0.2.4/src/sink/_base_client.py
--rw-r--r--   0        0        0     3889 2023-04-27 10:18:25.106682 sink_pypi-0.2.4/src/sink/_base_exceptions.py
--rw-r--r--   0        0        0    34399 2023-04-27 10:18:25.106682 sink_pypi-0.2.4/src/sink/_client.py
--rw-r--r--   0        0        0       92 2023-04-27 10:18:25.106682 sink_pypi-0.2.4/src/sink/_constants.py
--rw-r--r--   0        0        0     1285 2023-04-27 10:18:25.106682 sink_pypi-0.2.4/src/sink/_exceptions.py
--rw-r--r--   0        0        0     7343 2023-04-27 10:18:25.106682 sink_pypi-0.2.4/src/sink/_models.py
--rw-r--r--   0        0        0     4781 2023-04-27 10:18:25.106682 sink_pypi-0.2.4/src/sink/_qs.py
--rw-r--r--   0        0        0      866 2023-04-27 10:18:25.106682 sink_pypi-0.2.4/src/sink/_resource.py
--rw-r--r--   0        0        0     3975 2023-04-27 10:18:25.106682 sink_pypi-0.2.4/src/sink/_types.py
--rw-r--r--   0        0        0     1277 2023-04-27 10:18:25.106682 sink_pypi-0.2.4/src/sink/_utils/__init__.py
--rw-r--r--   0        0        0     6701 2023-04-27 10:18:25.106682 sink_pypi-0.2.4/src/sink/_utils/_transform.py
--rw-r--r--   0        0        0     9411 2023-04-27 10:18:25.106682 sink_pypi-0.2.4/src/sink/_utils/_utils.py
--rw-r--r--   0        0        0      123 2023-04-27 10:18:25.106682 sink_pypi-0.2.4/src/sink/_version.py
--rw-r--r--   0        0        0      312 2023-04-27 10:18:25.106682 sink_pypi-0.2.4/src/sink/_wrappers.py
--rw-r--r--   0        0        0     9832 2023-04-27 10:18:25.106682 sink_pypi-0.2.4/src/sink/pagination.py
--rw-r--r--   0        0        0        0 2023-04-27 10:18:25.106682 sink_pypi-0.2.4/src/sink/py.typed
--rw-r--r--   0        0        0     2265 2023-04-27 10:18:25.106682 sink_pypi-0.2.4/src/sink/resources/__init__.py
--rw-r--r--   0        0        0    32928 2023-04-27 10:18:25.106682 sink_pypi-0.2.4/src/sink/resources/body_params.py
--rw-r--r--   0        0        0    51067 2023-04-27 10:18:25.106682 sink_pypi-0.2.4/src/sink/resources/cards.py
--rw-r--r--   0        0        0      243 2023-04-27 10:18:25.106682 sink_pypi-0.2.4/src/sink/resources/company/__init__.py
--rw-r--r--   0        0        0      739 2023-04-27 10:18:25.106682 sink_pypi-0.2.4/src/sink/resources/company/company.py
--rw-r--r--   0        0        0     2135 2023-04-27 10:18:25.106682 sink_pypi-0.2.4/src/sink/resources/company/payments.py
--rw-r--r--   0        0        0      295 2023-04-27 10:18:25.106682 sink_pypi-0.2.4/src/sink/resources/config_tools.py
--rw-r--r--   0        0        0      396 2023-04-27 10:18:25.106682 sink_pypi-0.2.4/src/sink/resources/decorator_tests/__init__.py
--rw-r--r--   0        0        0     2906 2023-04-27 10:18:25.106682 sink_pypi-0.2.4/src/sink/resources/decorator_tests/decorator_tests.py
--rw-r--r--   0        0        0     2421 2023-04-27 10:18:25.106682 sink_pypi-0.2.4/src/sink/resources/decorator_tests/keep_this_resource.py
--rw-r--r--   0        0        0     2255 2023-04-27 10:18:25.106682 sink_pypi-0.2.4/src/sink/resources/decorator_tests/languages.py
--rw-r--r--   0        0        0      238 2023-04-27 10:18:25.106682 sink_pypi-0.2.4/src/sink/resources/deeply_nested/__init__.py
--rw-r--r--   0        0        0      732 2023-04-27 10:18:25.106682 sink_pypi-0.2.4/src/sink/resources/deeply_nested/deeply_nested.py
--rw-r--r--   0        0        0      218 2023-04-27 10:18:25.106682 sink_pypi-0.2.4/src/sink/resources/deeply_nested/level_one/__init__.py
--rw-r--r--   0        0        0     2558 2023-04-27 10:18:25.106682 sink_pypi-0.2.4/src/sink/resources/deeply_nested/level_one/level_one.py
--rw-r--r--   0        0        0      228 2023-04-27 10:18:25.106682 sink_pypi-0.2.4/src/sink/resources/deeply_nested/level_one/level_two/__init__.py
--rw-r--r--   0        0        0     2117 2023-04-27 10:18:25.106682 sink_pypi-0.2.4/src/sink/resources/deeply_nested/level_one/level_two/level_three.py
--rw-r--r--   0        0        0     2585 2023-04-27 10:18:25.106682 sink_pypi-0.2.4/src/sink/resources/deeply_nested/level_one/level_two/level_two.py
--rw-r--r--   0        0        0     5962 2023-04-27 10:18:25.106682 sink_pypi-0.2.4/src/sink/resources/envelopes.py
--rw-r--r--   0        0        0     4021 2023-04-27 10:18:25.106682 sink_pypi-0.2.4/src/sink/resources/header_params.py
--rw-r--r--   0        0        0      191 2023-04-27 10:18:25.106682 sink_pypi-0.2.4/src/sink/resources/names/__init__.py
--rw-r--r--   0        0        0     2719 2023-04-27 10:18:25.106682 sink_pypi-0.2.4/src/sink/resources/names/names.py
--rw-r--r--   0        0        0     3757 2023-04-27 10:18:25.106682 sink_pypi-0.2.4/src/sink/resources/names/params.py
--rw-r--r--   0        0        0      891 2023-04-27 10:18:25.106682 sink_pypi-0.2.4/src/sink/resources/pagination_tests/__init__.py
--rw-r--r--   0        0        0     3886 2023-04-27 10:18:25.106682 sink_pypi-0.2.4/src/sink/resources/pagination_tests/concrete.py
--rw-r--r--   0        0        0     3674 2023-04-27 10:18:25.106682 sink_pypi-0.2.4/src/sink/resources/pagination_tests/cursor.py
--rw-r--r--   0        0        0     3738 2023-04-27 10:18:25.106682 sink_pypi-0.2.4/src/sink/resources/pagination_tests/cursor_url.py
--rw-r--r--   0        0        0     3592 2023-04-27 10:18:25.106682 sink_pypi-0.2.4/src/sink/resources/pagination_tests/fake_pages.py
--rw-r--r--   0        0        0     3360 2023-04-27 10:18:25.106682 sink_pypi-0.2.4/src/sink/resources/pagination_tests/hypermedia.py
--rw-r--r--   0        0        0     3424 2023-04-27 10:18:25.106682 sink_pypi-0.2.4/src/sink/resources/pagination_tests/hypermedia_raw.py
--rw-r--r--   0        0        0     3674 2023-04-27 10:18:25.106682 sink_pypi-0.2.4/src/sink/resources/pagination_tests/offset.py
--rw-r--r--   0        0        0     3769 2023-04-27 10:18:25.106682 sink_pypi-0.2.4/src/sink/resources/pagination_tests/page_number.py
--rw-r--r--   0        0        0     2124 2023-04-27 10:18:25.106682 sink_pypi-0.2.4/src/sink/resources/pagination_tests/pagination_tests.py
--rw-r--r--   0        0        0      191 2023-04-27 10:18:25.106682 sink_pypi-0.2.4/src/sink/resources/parent/__init__.py
--rw-r--r--   0        0        0     2128 2023-04-27 10:18:25.106682 sink_pypi-0.2.4/src/sink/resources/parent/child.py
--rw-r--r--   0        0        0      670 2023-04-27 10:18:25.106682 sink_pypi-0.2.4/src/sink/resources/parent/parent.py
--rw-r--r--   0        0        0     4621 2023-04-27 10:18:25.106682 sink_pypi-0.2.4/src/sink/resources/path_params.py
--rw-r--r--   0        0        0    21560 2023-04-27 10:18:25.106682 sink_pypi-0.2.4/src/sink/resources/query_params.py
--rw-r--r--   0        0        0      516 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/resources/resource_refs/__init__.py
--rw-r--r--   0        0        0     4008 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/resources/resource_refs/paginated_model_first_ref.py
--rw-r--r--   0        0        0     4017 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/resources/resource_refs/paginated_model_second_ref.py
--rw-r--r--   0        0        0     1286 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/resources/resource_refs/resource_refs.py
--rw-r--r--   0        0        0     2380 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/resources/resources.py
--rw-r--r--   0        0        0    24645 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/resources/responses.py
--rw-r--r--   0        0        0     2774 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/resources/sta_563.py
--rw-r--r--   0        0        0     7658 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/resources/sta_569.py
--rw-r--r--   0        0        0     6292 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/resources/sta_606.py
--rw-r--r--   0        0        0     5493 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/resources/sta_613.py
--rw-r--r--   0        0        0     2285 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/resources/sta_630.py
--rw-r--r--   0        0        0     1955 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/resources/testing.py
--rw-r--r--   0        0        0     2136 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/resources/tests.py
--rw-r--r--   0        0        0      528 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/resources/types/__init__.py
--rw-r--r--   0        0        0      268 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/resources/types/maps.py
--rw-r--r--   0        0        0     2431 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/resources/types/objects.py
--rw-r--r--   0        0        0     3977 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/resources/types/read_only_params.py
--rw-r--r--   0        0        0    14218 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/resources/types/types.py
--rw-r--r--   0        0        0     2290 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/resources/types/write_only_responses.py
--rw-r--r--   0        0        0     2406 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/resources/widgets.py
--rw-r--r--   0        0        0     6744 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/__init__.py
--rw-r--r--   0        0        0      830 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/address.py
--rw-r--r--   0        0        0      249 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/api_status.py
--rw-r--r--   0        0        0      124 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/api_status_alias.py
--rw-r--r--   0        0        0      264 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/body_param_read_only_properties_params.py
--rw-r--r--   0        0        0      577 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/body_param_top_level_any_of_params.py
--rw-r--r--   0        0        0      511 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/body_param_top_level_any_of_response.py
--rw-r--r--   0        0        0      577 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/body_param_top_level_one_of_params.py
--rw-r--r--   0        0        0      511 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/body_param_top_level_one_of_response.py
--rw-r--r--   0        0        0      543 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/body_param_union_overlapping_prop_params.py
--rw-r--r--   0        0        0      210 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/body_param_union_overlapping_prop_response.py
--rw-r--r--   0        0        0      346 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/body_param_with_model_property_params.py
--rw-r--r--   0        0        0     4177 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/card.py
--rw-r--r--   0        0        0      102 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/card_alias.py
--rw-r--r--   0        0        0     4493 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/card_create_aliased_params.py
--rw-r--r--   0        0        0     4458 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/card_create_params.py
--rw-r--r--   0        0        0     1112 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/card_list_params.py
--rw-r--r--   0        0        0     1151 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/card_provision_foo_params.py
--rw-r--r--   0        0        0      201 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/card_provision_foo_response.py
--rw-r--r--   0        0        0     1210 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/card_reissue_params.py
--rw-r--r--   0        0        0     2245 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/card_update_params.py
--rw-r--r--   0        0        0      192 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/company/__init__.py
--rw-r--r--   0        0        0      152 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/company/company.py
--rw-r--r--   0        0        0      170 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/company/company_payment.py
--rw-r--r--   0        0        0      122 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/custom_api_status_message.py
--rw-r--r--   0        0        0      190 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/decorator_test_keep_me_response.py
--rw-r--r--   0        0        0      238 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/decorator_tests/__init__.py
--rw-r--r--   0        0        0      213 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/decorator_tests/keep_this_resource_keep_this_method_response.py
--rw-r--r--   0        0        0      146 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/deeply_nested/__init__.py
--rw-r--r--   0        0        0      146 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/deeply_nested/level_one/__init__.py
--rw-r--r--   0        0        0      146 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/deeply_nested/level_one/level_two/__init__.py
--rw-r--r--   0        0        0      257 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/deeply_nested/level_one/level_two/model_level_3.py
--rw-r--r--   0        0        0      256 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/deeply_nested/level_one/model_level_2.py
--rw-r--r--   0        0        0      255 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/deeply_nested/model_level_1.py
--rw-r--r--   0        0        0      182 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/delete_empty_object_response.py
--rw-r--r--   0        0        0      235 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/envelope_inline_response_response.py
--rw-r--r--   0        0        0     1548 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/funding_account.py
--rw-r--r--   0        0        0      301 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/github_user.py
--rw-r--r--   0        0        0      485 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/github_user_preferences.py
--rw-r--r--   0        0        0      255 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/header_param_client_argument_params.py
--rw-r--r--   0        0        0      190 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/my_model.py
--rw-r--r--   0        0        0      285 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/name_response_shadows_pydantic_response.py
--rw-r--r--   0        0        0      190 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/names/__init__.py
--rw-r--r--   0        0        0      282 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/names/param_options_param_params.py
--rw-r--r--   0        0        0      285 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/object_with_any_of_null_property.py
--rw-r--r--   0        0        0      284 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/object_with_one_of_null_property.py
--rw-r--r--   0        0        0      797 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/pagination_tests/__init__.py
--rw-r--r--   0        0        0      251 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/pagination_tests/concrete_list_params.py
--rw-r--r--   0        0        0      244 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/pagination_tests/cursor_list_params.py
--rw-r--r--   0        0        0      250 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/pagination_tests/cursor_url_list_params.py
--rw-r--r--   0        0        0      264 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/pagination_tests/fake_page_list_params.py
--rw-r--r--   0        0        0      234 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/pagination_tests/hypermedia_list_params.py
--rw-r--r--   0        0        0      240 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/pagination_tests/hypermedia_raw_list_params.py
--rw-r--r--   0        0        0      213 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/pagination_tests/my_concrete_page_item.py
--rw-r--r--   0        0        0      244 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/pagination_tests/offset_list_params.py
--rw-r--r--   0        0        0      254 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/pagination_tests/page_number_list_params.py
--rw-r--r--   0        0        0      205 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/parent/__init__.py
--rw-r--r--   0        0        0      195 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/parent/child_inlined_response_response.py
--rw-r--r--   0        0        0      186 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/path_param_multiple_response.py
--rw-r--r--   0        0        0      186 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/path_param_singular_response.py
--rw-r--r--   0        0        0      286 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/query_param_any_of_params.py
--rw-r--r--   0        0        0      316 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/query_param_array_params.py
--rw-r--r--   0        0        0      575 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/query_param_enum_params.py
--rw-r--r--   0        0        0      445 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/query_param_object_params.py
--rw-r--r--   0        0        0      286 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/query_param_one_of_params.py
--rw-r--r--   0        0        0      328 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/query_param_primitives_params.py
--rw-r--r--   0        0        0      351 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/resource_refs/__init__.py
--rw-r--r--   0        0        0      276 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/resource_refs/paginated_model_first_ref_list_params.py
--rw-r--r--   0        0        0      278 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/resource_refs/paginated_model_second_ref_list_params.py
--rw-r--r--   0        0        0      268 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/response_additional_properties_nested_model_reference_response.py
--rw-r--r--   0        0        0      188 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/response_additional_properties_response.py
--rw-r--r--   0        0        0      253 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/response_allof_simple_response.py
--rw-r--r--   0        0        0      231 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/response_array_response_response.py
--rw-r--r--   0        0        0      252 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/response_missing_required_response.py
--rw-r--r--   0        0        0      200 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/response_object_no_properties_response.py
--rw-r--r--   0        0        0      336 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/response_object_with_additional_properties_prop_response.py
--rw-r--r--   0        0        0      138 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/response_string_response_response.py
--rw-r--r--   0        0        0      164 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/root_response.py
--rw-r--r--   0        0        0      366 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/shared/__init__.py
--rw-r--r--   0        0        0      314 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/shared/currency.py
--rw-r--r--   0        0        0      272 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/shared/object_with_child_ref.py
--rw-r--r--   0        0        0     1534 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/shared/shipping_address.py
--rw-r--r--   0        0        0      322 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/shared/simple_object.py
--rw-r--r--   0        0        0      164 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/shared/simple_object_alias.py
--rw-r--r--   0        0        0      366 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/shared_params/__init__.py
--rw-r--r--   0        0        0      314 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/shared_params/currency.py
--rw-r--r--   0        0        0      323 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/shared_params/object_with_child_ref.py
--rw-r--r--   0        0        0     1565 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/shared_params/shipping_address.py
--rw-r--r--   0        0        0      362 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/shared_params/simple_object.py
--rw-r--r--   0        0        0      164 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/shared_params/simple_object_alias.py
--rw-r--r--   0        0        0      243 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/simple_allof.py
--rw-r--r--   0        0        0      192 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/sta_563_post_empty_object_response.py
--rw-r--r--   0        0        0      273 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/sta_569_one_entry_params.py
--rw-r--r--   0        0        0      221 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/sta_569_one_entry_response.py
--rw-r--r--   0        0        0      269 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/sta_569_one_entry_with_null_params.py
--rw-r--r--   0        0        0      237 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/sta_569_one_entry_with_null_response.py
--rw-r--r--   0        0        0      235 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/sta_606_with_shared_params_params.py
--rw-r--r--   0        0        0      202 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/sta_613_global_with_standard_response.py
--rw-r--r--   0        0        0      186 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/sta_613_only_global_response.py
--rw-r--r--   0        0        0      782 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/type_dates_params.py
--rw-r--r--   0        0        0      409 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/type_dates_response.py
--rw-r--r--   0        0        0      897 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/type_datetimes_params.py
--rw-r--r--   0        0        0      461 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/type_datetimes_response.py
--rw-r--r--   0        0        0      401 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/type_enums_params.py
--rw-r--r--   0        0        0      444 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/type_enums_response.py
--rw-r--r--   0        0        0      570 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/types/__init__.py
--rw-r--r--   0        0        0      542 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/types/object_mixed_known_and_unknown_response.py
--rw-r--r--   0        0        0      317 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/types/read_only_param_simple_params.py
--rw-r--r--   0        0        0      170 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/types/read_only_param_simple_response.py
--rw-r--r--   0        0        0      367 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/types/write_only_response_simple_response.py
--rw-r--r--   0        0        0      196 2023-04-27 10:18:25.110682 sink_pypi-0.2.4/src/sink/types/widget.py
--rw-r--r--   0        0        0     9187 1970-01-01 00:00:00.000000 sink_pypi-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0    11334 2023-04-28 13:09:40.787740 sink_pypi-0.2.5/LICENSE
+-rw-r--r--   0        0        0     8243 2023-04-28 13:09:40.787740 sink_pypi-0.2.5/README.md
+-rw-r--r--   0        0        0     1894 2023-04-28 13:09:40.787740 sink_pypi-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     1968 2023-04-28 13:09:40.787740 sink_pypi-0.2.5/src/sink/__init__.py
+-rw-r--r--   0        0        0    45503 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/_base_client.py
+-rw-r--r--   0        0        0     3889 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/_base_exceptions.py
+-rw-r--r--   0        0        0    34399 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/_client.py
+-rw-r--r--   0        0        0       92 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/_constants.py
+-rw-r--r--   0        0        0     1285 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/_exceptions.py
+-rw-r--r--   0        0        0     7343 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/_models.py
+-rw-r--r--   0        0        0     4781 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/_qs.py
+-rw-r--r--   0        0        0      866 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/_resource.py
+-rw-r--r--   0        0        0     3975 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/_types.py
+-rw-r--r--   0        0        0     1277 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/_utils/__init__.py
+-rw-r--r--   0        0        0     6701 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/_utils/_transform.py
+-rw-r--r--   0        0        0     9411 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/_utils/_utils.py
+-rw-r--r--   0        0        0      123 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/_version.py
+-rw-r--r--   0        0        0      312 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/_wrappers.py
+-rw-r--r--   0        0        0     9832 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/pagination.py
+-rw-r--r--   0        0        0        0 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/py.typed
+-rw-r--r--   0        0        0     2265 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/resources/__init__.py
+-rw-r--r--   0        0        0    32928 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/resources/body_params.py
+-rw-r--r--   0        0        0    51067 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/resources/cards.py
+-rw-r--r--   0        0        0      243 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/resources/company/__init__.py
+-rw-r--r--   0        0        0      739 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/resources/company/company.py
+-rw-r--r--   0        0        0     2135 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/resources/company/payments.py
+-rw-r--r--   0        0        0      295 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/resources/config_tools.py
+-rw-r--r--   0        0        0      396 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/resources/decorator_tests/__init__.py
+-rw-r--r--   0        0        0     2906 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/resources/decorator_tests/decorator_tests.py
+-rw-r--r--   0        0        0     2421 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/resources/decorator_tests/keep_this_resource.py
+-rw-r--r--   0        0        0     2255 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/resources/decorator_tests/languages.py
+-rw-r--r--   0        0        0      238 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/resources/deeply_nested/__init__.py
+-rw-r--r--   0        0        0      732 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/resources/deeply_nested/deeply_nested.py
+-rw-r--r--   0        0        0      218 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/resources/deeply_nested/level_one/__init__.py
+-rw-r--r--   0        0        0     2558 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/resources/deeply_nested/level_one/level_one.py
+-rw-r--r--   0        0        0      228 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/resources/deeply_nested/level_one/level_two/__init__.py
+-rw-r--r--   0        0        0     2117 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/resources/deeply_nested/level_one/level_two/level_three.py
+-rw-r--r--   0        0        0     2585 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/resources/deeply_nested/level_one/level_two/level_two.py
+-rw-r--r--   0        0        0     5962 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/resources/envelopes.py
+-rw-r--r--   0        0        0     4021 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/resources/header_params.py
+-rw-r--r--   0        0        0      191 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/resources/names/__init__.py
+-rw-r--r--   0        0        0     2719 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/resources/names/names.py
+-rw-r--r--   0        0        0     3757 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/resources/names/params.py
+-rw-r--r--   0        0        0      891 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/resources/pagination_tests/__init__.py
+-rw-r--r--   0        0        0     3886 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/resources/pagination_tests/concrete.py
+-rw-r--r--   0        0        0     3674 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/resources/pagination_tests/cursor.py
+-rw-r--r--   0        0        0     3738 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/resources/pagination_tests/cursor_url.py
+-rw-r--r--   0        0        0     3592 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/resources/pagination_tests/fake_pages.py
+-rw-r--r--   0        0        0     3360 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/resources/pagination_tests/hypermedia.py
+-rw-r--r--   0        0        0     3424 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/resources/pagination_tests/hypermedia_raw.py
+-rw-r--r--   0        0        0     3674 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/resources/pagination_tests/offset.py
+-rw-r--r--   0        0        0     3769 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/resources/pagination_tests/page_number.py
+-rw-r--r--   0        0        0     2124 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/resources/pagination_tests/pagination_tests.py
+-rw-r--r--   0        0        0      191 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/resources/parent/__init__.py
+-rw-r--r--   0        0        0     2128 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/resources/parent/child.py
+-rw-r--r--   0        0        0      670 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/resources/parent/parent.py
+-rw-r--r--   0        0        0     4621 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/resources/path_params.py
+-rw-r--r--   0        0        0    21560 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/resources/query_params.py
+-rw-r--r--   0        0        0      516 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/resources/resource_refs/__init__.py
+-rw-r--r--   0        0        0     4008 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/resources/resource_refs/paginated_model_first_ref.py
+-rw-r--r--   0        0        0     4017 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/resources/resource_refs/paginated_model_second_ref.py
+-rw-r--r--   0        0        0     1286 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/resources/resource_refs/resource_refs.py
+-rw-r--r--   0        0        0     2380 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/resources/resources.py
+-rw-r--r--   0        0        0    24645 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/resources/responses.py
+-rw-r--r--   0        0        0     2774 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/resources/sta_563.py
+-rw-r--r--   0        0        0     7658 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/resources/sta_569.py
+-rw-r--r--   0        0        0     6292 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/resources/sta_606.py
+-rw-r--r--   0        0        0     5493 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/resources/sta_613.py
+-rw-r--r--   0        0        0     2285 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/resources/sta_630.py
+-rw-r--r--   0        0        0     1955 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/resources/testing.py
+-rw-r--r--   0        0        0     2136 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/resources/tests.py
+-rw-r--r--   0        0        0      528 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/resources/types/__init__.py
+-rw-r--r--   0        0        0      268 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/resources/types/maps.py
+-rw-r--r--   0        0        0     2431 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/resources/types/objects.py
+-rw-r--r--   0        0        0     3977 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/resources/types/read_only_params.py
+-rw-r--r--   0        0        0    14218 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/resources/types/types.py
+-rw-r--r--   0        0        0     2290 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/resources/types/write_only_responses.py
+-rw-r--r--   0        0        0     2406 2023-04-28 13:09:40.791740 sink_pypi-0.2.5/src/sink/resources/widgets.py
+-rw-r--r--   0        0        0     6744 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/__init__.py
+-rw-r--r--   0        0        0      830 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/address.py
+-rw-r--r--   0        0        0      249 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/api_status.py
+-rw-r--r--   0        0        0      124 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/api_status_alias.py
+-rw-r--r--   0        0        0      264 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/body_param_read_only_properties_params.py
+-rw-r--r--   0        0        0      577 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/body_param_top_level_any_of_params.py
+-rw-r--r--   0        0        0      511 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/body_param_top_level_any_of_response.py
+-rw-r--r--   0        0        0      577 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/body_param_top_level_one_of_params.py
+-rw-r--r--   0        0        0      511 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/body_param_top_level_one_of_response.py
+-rw-r--r--   0        0        0      543 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/body_param_union_overlapping_prop_params.py
+-rw-r--r--   0        0        0      210 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/body_param_union_overlapping_prop_response.py
+-rw-r--r--   0        0        0      346 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/body_param_with_model_property_params.py
+-rw-r--r--   0        0        0     4177 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/card.py
+-rw-r--r--   0        0        0      102 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/card_alias.py
+-rw-r--r--   0        0        0     4493 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/card_create_aliased_params.py
+-rw-r--r--   0        0        0     4458 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/card_create_params.py
+-rw-r--r--   0        0        0     1112 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/card_list_params.py
+-rw-r--r--   0        0        0     1151 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/card_provision_foo_params.py
+-rw-r--r--   0        0        0      201 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/card_provision_foo_response.py
+-rw-r--r--   0        0        0     1210 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/card_reissue_params.py
+-rw-r--r--   0        0        0     2245 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/card_update_params.py
+-rw-r--r--   0        0        0      192 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/company/__init__.py
+-rw-r--r--   0        0        0      152 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/company/company.py
+-rw-r--r--   0        0        0      170 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/company/company_payment.py
+-rw-r--r--   0        0        0      122 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/custom_api_status_message.py
+-rw-r--r--   0        0        0      190 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/decorator_test_keep_me_response.py
+-rw-r--r--   0        0        0      238 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/decorator_tests/__init__.py
+-rw-r--r--   0        0        0      213 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/decorator_tests/keep_this_resource_keep_this_method_response.py
+-rw-r--r--   0        0        0      146 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/deeply_nested/__init__.py
+-rw-r--r--   0        0        0      146 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/deeply_nested/level_one/__init__.py
+-rw-r--r--   0        0        0      146 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/deeply_nested/level_one/level_two/__init__.py
+-rw-r--r--   0        0        0      257 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/deeply_nested/level_one/level_two/model_level_3.py
+-rw-r--r--   0        0        0      256 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/deeply_nested/level_one/model_level_2.py
+-rw-r--r--   0        0        0      255 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/deeply_nested/model_level_1.py
+-rw-r--r--   0        0        0      182 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/delete_empty_object_response.py
+-rw-r--r--   0        0        0      235 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/envelope_inline_response_response.py
+-rw-r--r--   0        0        0     1548 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/funding_account.py
+-rw-r--r--   0        0        0      301 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/github_user.py
+-rw-r--r--   0        0        0      485 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/github_user_preferences.py
+-rw-r--r--   0        0        0      255 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/header_param_client_argument_params.py
+-rw-r--r--   0        0        0      190 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/my_model.py
+-rw-r--r--   0        0        0      285 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/name_response_shadows_pydantic_response.py
+-rw-r--r--   0        0        0      190 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/names/__init__.py
+-rw-r--r--   0        0        0      282 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/names/param_options_param_params.py
+-rw-r--r--   0        0        0      285 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/object_with_any_of_null_property.py
+-rw-r--r--   0        0        0      284 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/object_with_one_of_null_property.py
+-rw-r--r--   0        0        0      797 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/pagination_tests/__init__.py
+-rw-r--r--   0        0        0      251 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/pagination_tests/concrete_list_params.py
+-rw-r--r--   0        0        0      244 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/pagination_tests/cursor_list_params.py
+-rw-r--r--   0        0        0      250 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/pagination_tests/cursor_url_list_params.py
+-rw-r--r--   0        0        0      264 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/pagination_tests/fake_page_list_params.py
+-rw-r--r--   0        0        0      234 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/pagination_tests/hypermedia_list_params.py
+-rw-r--r--   0        0        0      240 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/pagination_tests/hypermedia_raw_list_params.py
+-rw-r--r--   0        0        0      213 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/pagination_tests/my_concrete_page_item.py
+-rw-r--r--   0        0        0      244 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/pagination_tests/offset_list_params.py
+-rw-r--r--   0        0        0      254 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/pagination_tests/page_number_list_params.py
+-rw-r--r--   0        0        0      205 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/parent/__init__.py
+-rw-r--r--   0        0        0      195 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/parent/child_inlined_response_response.py
+-rw-r--r--   0        0        0      186 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/path_param_multiple_response.py
+-rw-r--r--   0        0        0      186 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/path_param_singular_response.py
+-rw-r--r--   0        0        0      286 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/query_param_any_of_params.py
+-rw-r--r--   0        0        0      316 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/query_param_array_params.py
+-rw-r--r--   0        0        0      575 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/query_param_enum_params.py
+-rw-r--r--   0        0        0      445 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/query_param_object_params.py
+-rw-r--r--   0        0        0      286 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/query_param_one_of_params.py
+-rw-r--r--   0        0        0      328 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/query_param_primitives_params.py
+-rw-r--r--   0        0        0      351 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/resource_refs/__init__.py
+-rw-r--r--   0        0        0      276 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/resource_refs/paginated_model_first_ref_list_params.py
+-rw-r--r--   0        0        0      278 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/resource_refs/paginated_model_second_ref_list_params.py
+-rw-r--r--   0        0        0      268 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/response_additional_properties_nested_model_reference_response.py
+-rw-r--r--   0        0        0      188 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/response_additional_properties_response.py
+-rw-r--r--   0        0        0      253 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/response_allof_simple_response.py
+-rw-r--r--   0        0        0      231 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/response_array_response_response.py
+-rw-r--r--   0        0        0      252 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/response_missing_required_response.py
+-rw-r--r--   0        0        0      200 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/response_object_no_properties_response.py
+-rw-r--r--   0        0        0      336 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/response_object_with_additional_properties_prop_response.py
+-rw-r--r--   0        0        0      138 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/response_string_response_response.py
+-rw-r--r--   0        0        0      164 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/root_response.py
+-rw-r--r--   0        0        0      366 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/shared/__init__.py
+-rw-r--r--   0        0        0      314 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/shared/currency.py
+-rw-r--r--   0        0        0      272 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/shared/object_with_child_ref.py
+-rw-r--r--   0        0        0     1534 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/shared/shipping_address.py
+-rw-r--r--   0        0        0      322 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/shared/simple_object.py
+-rw-r--r--   0        0        0      164 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/shared/simple_object_alias.py
+-rw-r--r--   0        0        0      366 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/shared_params/__init__.py
+-rw-r--r--   0        0        0      314 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/shared_params/currency.py
+-rw-r--r--   0        0        0      323 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/shared_params/object_with_child_ref.py
+-rw-r--r--   0        0        0     1565 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/shared_params/shipping_address.py
+-rw-r--r--   0        0        0      362 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/shared_params/simple_object.py
+-rw-r--r--   0        0        0      164 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/shared_params/simple_object_alias.py
+-rw-r--r--   0        0        0      243 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/simple_allof.py
+-rw-r--r--   0        0        0      192 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/sta_563_post_empty_object_response.py
+-rw-r--r--   0        0        0      273 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/sta_569_one_entry_params.py
+-rw-r--r--   0        0        0      221 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/sta_569_one_entry_response.py
+-rw-r--r--   0        0        0      269 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/sta_569_one_entry_with_null_params.py
+-rw-r--r--   0        0        0      237 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/sta_569_one_entry_with_null_response.py
+-rw-r--r--   0        0        0      235 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/sta_606_with_shared_params_params.py
+-rw-r--r--   0        0        0      202 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/sta_613_global_with_standard_response.py
+-rw-r--r--   0        0        0      186 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/sta_613_only_global_response.py
+-rw-r--r--   0        0        0      782 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/type_dates_params.py
+-rw-r--r--   0        0        0      409 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/type_dates_response.py
+-rw-r--r--   0        0        0      897 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/type_datetimes_params.py
+-rw-r--r--   0        0        0      461 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/type_datetimes_response.py
+-rw-r--r--   0        0        0      401 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/type_enums_params.py
+-rw-r--r--   0        0        0      444 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/type_enums_response.py
+-rw-r--r--   0        0        0      570 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/types/__init__.py
+-rw-r--r--   0        0        0      542 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/types/object_mixed_known_and_unknown_response.py
+-rw-r--r--   0        0        0      317 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/types/read_only_param_simple_params.py
+-rw-r--r--   0        0        0      170 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/types/read_only_param_simple_response.py
+-rw-r--r--   0        0        0      367 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/types/write_only_response_simple_response.py
+-rw-r--r--   0        0        0      196 2023-04-28 13:09:40.795740 sink_pypi-0.2.5/src/sink/types/widget.py
+-rw-r--r--   0        0        0     9187 1970-01-01 00:00:00.000000 sink_pypi-0.2.5/PKG-INFO
```

### Comparing `sink_pypi-0.2.4/LICENSE` & `sink_pypi-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/README.md` & `sink_pypi-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/pyproject.toml` & `sink_pypi-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sink-pypi"
-version = "0.2.4"
+version = "0.2.5"
 description = "Client library for the sink API"
 readme = "README.md"
 authors = ["Sink <dev@stainlessapi.com>"]
 license = "Apache-2.0"
 repository = "https://github.com/stainless-sdks/sink-python-public"
 packages = [
   { include = "sink", from = "src" }
```

### Comparing `sink_pypi-0.2.4/src/sink/__init__.py` & `sink_pypi-0.2.5/src/sink/__init__.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/_base_client.py` & `sink_pypi-0.2.5/src/sink/_base_client.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/_base_exceptions.py` & `sink_pypi-0.2.5/src/sink/_base_exceptions.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/_client.py` & `sink_pypi-0.2.5/src/sink/_client.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/_exceptions.py` & `sink_pypi-0.2.5/src/sink/_exceptions.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/_models.py` & `sink_pypi-0.2.5/src/sink/_models.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/_qs.py` & `sink_pypi-0.2.5/src/sink/_qs.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/_resource.py` & `sink_pypi-0.2.5/src/sink/_resource.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/_types.py` & `sink_pypi-0.2.5/src/sink/_types.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/_utils/__init__.py` & `sink_pypi-0.2.5/src/sink/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/_utils/_transform.py` & `sink_pypi-0.2.5/src/sink/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/_utils/_utils.py` & `sink_pypi-0.2.5/src/sink/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/pagination.py` & `sink_pypi-0.2.5/src/sink/pagination.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/resources/__init__.py` & `sink_pypi-0.2.5/src/sink/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/resources/body_params.py` & `sink_pypi-0.2.5/src/sink/resources/body_params.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/resources/cards.py` & `sink_pypi-0.2.5/src/sink/resources/cards.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/resources/company/company.py` & `sink_pypi-0.2.5/src/sink/resources/company/company.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/resources/company/payments.py` & `sink_pypi-0.2.5/src/sink/resources/company/payments.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/resources/decorator_tests/decorator_tests.py` & `sink_pypi-0.2.5/src/sink/resources/decorator_tests/decorator_tests.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/resources/decorator_tests/keep_this_resource.py` & `sink_pypi-0.2.5/src/sink/resources/decorator_tests/keep_this_resource.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/resources/decorator_tests/languages.py` & `sink_pypi-0.2.5/src/sink/resources/decorator_tests/languages.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/resources/deeply_nested/deeply_nested.py` & `sink_pypi-0.2.5/src/sink/resources/deeply_nested/deeply_nested.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/resources/deeply_nested/level_one/level_one.py` & `sink_pypi-0.2.5/src/sink/resources/deeply_nested/level_one/level_one.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/resources/deeply_nested/level_one/level_two/level_three.py` & `sink_pypi-0.2.5/src/sink/resources/deeply_nested/level_one/level_two/level_three.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/resources/deeply_nested/level_one/level_two/level_two.py` & `sink_pypi-0.2.5/src/sink/resources/deeply_nested/level_one/level_two/level_two.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/resources/envelopes.py` & `sink_pypi-0.2.5/src/sink/resources/envelopes.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/resources/header_params.py` & `sink_pypi-0.2.5/src/sink/resources/header_params.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/resources/names/names.py` & `sink_pypi-0.2.5/src/sink/resources/names/names.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/resources/names/params.py` & `sink_pypi-0.2.5/src/sink/resources/names/params.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/resources/pagination_tests/__init__.py` & `sink_pypi-0.2.5/src/sink/resources/pagination_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/resources/pagination_tests/concrete.py` & `sink_pypi-0.2.5/src/sink/resources/pagination_tests/concrete.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/resources/pagination_tests/cursor.py` & `sink_pypi-0.2.5/src/sink/resources/pagination_tests/cursor.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/resources/pagination_tests/cursor_url.py` & `sink_pypi-0.2.5/src/sink/resources/pagination_tests/cursor_url.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/resources/pagination_tests/fake_pages.py` & `sink_pypi-0.2.5/src/sink/resources/pagination_tests/fake_pages.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/resources/pagination_tests/hypermedia.py` & `sink_pypi-0.2.5/src/sink/resources/pagination_tests/hypermedia.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/resources/pagination_tests/hypermedia_raw.py` & `sink_pypi-0.2.5/src/sink/resources/pagination_tests/hypermedia_raw.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/resources/pagination_tests/offset.py` & `sink_pypi-0.2.5/src/sink/resources/pagination_tests/offset.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/resources/pagination_tests/page_number.py` & `sink_pypi-0.2.5/src/sink/resources/pagination_tests/page_number.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/resources/pagination_tests/pagination_tests.py` & `sink_pypi-0.2.5/src/sink/resources/pagination_tests/pagination_tests.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/resources/parent/child.py` & `sink_pypi-0.2.5/src/sink/resources/parent/child.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/resources/parent/parent.py` & `sink_pypi-0.2.5/src/sink/resources/parent/parent.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/resources/path_params.py` & `sink_pypi-0.2.5/src/sink/resources/path_params.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/resources/query_params.py` & `sink_pypi-0.2.5/src/sink/resources/query_params.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/resources/resource_refs/__init__.py` & `sink_pypi-0.2.5/src/sink/resources/resource_refs/__init__.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/resources/resource_refs/paginated_model_first_ref.py` & `sink_pypi-0.2.5/src/sink/resources/resource_refs/paginated_model_first_ref.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/resources/resource_refs/paginated_model_second_ref.py` & `sink_pypi-0.2.5/src/sink/resources/resource_refs/paginated_model_second_ref.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/resources/resource_refs/resource_refs.py` & `sink_pypi-0.2.5/src/sink/resources/resource_refs/resource_refs.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/resources/resources.py` & `sink_pypi-0.2.5/src/sink/resources/resources.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/resources/responses.py` & `sink_pypi-0.2.5/src/sink/resources/responses.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/resources/sta_563.py` & `sink_pypi-0.2.5/src/sink/resources/sta_563.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/resources/sta_569.py` & `sink_pypi-0.2.5/src/sink/resources/sta_569.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/resources/sta_606.py` & `sink_pypi-0.2.5/src/sink/resources/sta_606.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/resources/sta_613.py` & `sink_pypi-0.2.5/src/sink/resources/sta_613.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/resources/sta_630.py` & `sink_pypi-0.2.5/src/sink/resources/sta_630.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/resources/testing.py` & `sink_pypi-0.2.5/src/sink/resources/testing.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/resources/tests.py` & `sink_pypi-0.2.5/src/sink/resources/tests.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/resources/types/__init__.py` & `sink_pypi-0.2.5/src/sink/resources/types/__init__.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/resources/types/objects.py` & `sink_pypi-0.2.5/src/sink/resources/types/objects.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/resources/types/read_only_params.py` & `sink_pypi-0.2.5/src/sink/resources/types/read_only_params.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/resources/types/types.py` & `sink_pypi-0.2.5/src/sink/resources/types/types.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/resources/types/write_only_responses.py` & `sink_pypi-0.2.5/src/sink/resources/types/write_only_responses.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/resources/widgets.py` & `sink_pypi-0.2.5/src/sink/resources/widgets.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/types/__init__.py` & `sink_pypi-0.2.5/src/sink/types/__init__.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/types/address.py` & `sink_pypi-0.2.5/src/sink/types/address.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/types/body_param_top_level_any_of_params.py` & `sink_pypi-0.2.5/src/sink/types/body_param_top_level_any_of_params.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/types/body_param_top_level_one_of_params.py` & `sink_pypi-0.2.5/src/sink/types/body_param_top_level_one_of_params.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/types/body_param_union_overlapping_prop_params.py` & `sink_pypi-0.2.5/src/sink/types/body_param_union_overlapping_prop_params.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/types/card.py` & `sink_pypi-0.2.5/src/sink/types/card.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/types/card_create_aliased_params.py` & `sink_pypi-0.2.5/src/sink/types/card_create_aliased_params.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/types/card_create_params.py` & `sink_pypi-0.2.5/src/sink/types/card_create_params.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/types/card_list_params.py` & `sink_pypi-0.2.5/src/sink/types/card_list_params.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/types/card_provision_foo_params.py` & `sink_pypi-0.2.5/src/sink/types/card_provision_foo_params.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/types/card_reissue_params.py` & `sink_pypi-0.2.5/src/sink/types/card_reissue_params.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/types/card_update_params.py` & `sink_pypi-0.2.5/src/sink/types/card_update_params.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/types/funding_account.py` & `sink_pypi-0.2.5/src/sink/types/funding_account.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/types/pagination_tests/__init__.py` & `sink_pypi-0.2.5/src/sink/types/pagination_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/types/query_param_enum_params.py` & `sink_pypi-0.2.5/src/sink/types/query_param_enum_params.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/types/shared/shipping_address.py` & `sink_pypi-0.2.5/src/sink/types/shared/shipping_address.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/types/shared_params/shipping_address.py` & `sink_pypi-0.2.5/src/sink/types/shared_params/shipping_address.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/types/type_dates_params.py` & `sink_pypi-0.2.5/src/sink/types/type_dates_params.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/types/type_datetimes_params.py` & `sink_pypi-0.2.5/src/sink/types/type_datetimes_params.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/types/types/__init__.py` & `sink_pypi-0.2.5/src/sink/types/types/__init__.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/src/sink/types/types/object_mixed_known_and_unknown_response.py` & `sink_pypi-0.2.5/src/sink/types/types/object_mixed_known_and_unknown_response.py`

 * *Files identical despite different names*

### Comparing `sink_pypi-0.2.4/PKG-INFO` & `sink_pypi-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sink-pypi
-Version: 0.2.4
+Version: 0.2.5
 Summary: Client library for the sink API
 Home-page: https://github.com/stainless-sdks/sink-python-public
 License: Apache-2.0
 Author: Sink
 Author-email: dev@stainlessapi.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

