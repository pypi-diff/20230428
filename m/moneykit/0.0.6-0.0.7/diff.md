# Comparing `tmp/moneykit-0.0.6.tar.gz` & `tmp/moneykit-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moneykit-0.0.6.tar", max compression
+gzip compressed data, was "moneykit-0.0.7.tar", max compression
```

## Comparing `moneykit-0.0.6.tar` & `moneykit-0.0.7.tar`

### file list

```diff
@@ -1,252 +1,391 @@
--rw-r--r--   0        0        0      267 2023-04-27 15:31:27.000000 moneykit-0.0.6/README.md
--rw-r--r--   0        0        0    10496 2023-04-27 15:58:50.662047 moneykit-0.0.6/moneykit/__init__.py
--rw-r--r--   0        0        0      578 2023-04-27 15:31:40.451576 moneykit-0.0.6/moneykit/api/__init__.py
--rw-r--r--   0        0        0    23690 2023-04-27 15:31:41.269922 moneykit-0.0.6/moneykit/api/access_token_api.py
--rw-r--r--   0        0        0     8218 2023-04-27 15:31:41.265623 moneykit-0.0.6/moneykit/api/account_numbers_api.py
--rw-r--r--   0        0        0    32807 2023-04-27 15:31:41.274455 moneykit-0.0.6/moneykit/api/accounts_api.py
--rw-r--r--   0        0        0     9029 2023-04-27 15:31:41.276481 moneykit-0.0.6/moneykit/api/identity_api.py
--rw-r--r--   0        0        0    17337 2023-04-27 15:31:41.279397 moneykit-0.0.6/moneykit/api/institutions_api.py
--rw-r--r--   0        0        0    15712 2023-04-27 15:31:41.283839 moneykit-0.0.6/moneykit/api/link_session_api.py
--rw-r--r--   0        0        0    28982 2023-04-27 15:31:41.285087 moneykit-0.0.6/moneykit/api/links_api.py
--rw-r--r--   0        0        0    15610 2023-04-27 11:39:18.892259 moneykit-0.0.6/moneykit/api/money_link_api.py
--rw-r--r--   0        0        0     8788 2023-04-27 15:31:41.281592 moneykit-0.0.6/moneykit/api/products_api.py
--rw-r--r--   0        0        0    34884 2023-04-27 15:31:41.283803 moneykit-0.0.6/moneykit/api/transactions_api.py
--rw-r--r--   0        0        0    32254 2023-04-27 15:31:41.285304 moneykit-0.0.6/moneykit/api/users_api.py
--rw-r--r--   0        0        0    27824 2023-04-27 15:31:41.263924 moneykit-0.0.6/moneykit/api_client.py
--rw-r--r--   0        0        0    16781 2023-04-27 15:31:41.281491 moneykit-0.0.6/moneykit/configuration.py
--rw-r--r--   0        0        0     5100 2023-04-27 15:31:40.544955 moneykit-0.0.6/moneykit/exceptions.py
--rw-r--r--   0        0        0     9521 2023-04-27 15:31:40.543664 moneykit-0.0.6/moneykit/models/__init__.py
--rw-r--r--   0        0        0     3780 2023-04-27 15:31:41.266199 moneykit-0.0.6/moneykit/models/account_balances.py
--rw-r--r--   0        0        0     2888 2023-04-27 15:31:41.263245 moneykit-0.0.6/moneykit/models/account_group.py
--rw-r--r--   0        0        0     4250 2023-04-27 15:31:41.272420 moneykit-0.0.6/moneykit/models/account_identity.py
--rw-r--r--   0        0        0     2400 2023-04-27 15:31:41.278988 moneykit-0.0.6/moneykit/models/account_numbers.py
--rw-r--r--   0        0        0     3290 2023-04-27 15:31:41.266129 moneykit-0.0.6/moneykit/models/account_numbers_link_product.py
--rw-r--r--   0        0        0     2520 2023-04-27 15:31:41.264243 moneykit-0.0.6/moneykit/models/account_numbers_product_settings.py
--rw-r--r--   0        0        0      916 2023-04-27 15:31:41.282451 moneykit-0.0.6/moneykit/models/account_type.py
--rw-r--r--   0        0        0     4068 2023-04-27 15:31:41.270208 moneykit-0.0.6/moneykit/models/account_with_account_numbers.py
--rw-r--r--   0        0        0     2705 2023-04-27 15:31:41.264244 moneykit-0.0.6/moneykit/models/accounts_link_product.py
--rw-r--r--   0        0        0     2459 2023-04-27 15:31:41.262137 moneykit-0.0.6/moneykit/models/ach_number.py
--rw-r--r--   0        0        0     3720 2023-04-27 15:31:41.273910 moneykit-0.0.6/moneykit/models/address.py
--rw-r--r--   0        0        0     2950 2023-04-27 15:31:41.269608 moneykit-0.0.6/moneykit/models/api_client_out.py
--rw-r--r--   0        0        0     3148 2023-04-27 15:31:41.272921 moneykit-0.0.6/moneykit/models/api_error_auth_expired_access_token_response.py
--rw-r--r--   0        0        0     2939 2023-04-27 15:31:41.270460 moneykit-0.0.6/moneykit/models/api_error_auth_unauthorized_response.py
--rw-r--r--   0        0        0     3082 2023-04-27 15:31:41.267783 moneykit-0.0.6/moneykit/models/api_error_rate_limit_exceeded_response.py
--rw-r--r--   0        0        0     1824 2023-04-27 15:31:41.266792 moneykit-0.0.6/moneykit/models/app.py
--rw-r--r--   0        0        0     3751 2023-04-27 15:31:41.277275 moneykit-0.0.6/moneykit/models/app_api_public_accounts_account_out.py
--rw-r--r--   0        0        0     3232 2023-04-27 15:31:41.279696 moneykit-0.0.6/moneykit/models/app_api_public_users_transactions_account_out.py
--rw-r--r--   0        0        0     1897 2023-04-27 15:31:41.266633 moneykit-0.0.6/moneykit/models/bacs_number.py
--rw-r--r--   0        0        0     3942 2023-04-27 15:31:41.266844 moneykit-0.0.6/moneykit/models/balances.py
--rw-r--r--   0        0        0      518 2023-04-27 15:31:41.274787 moneykit-0.0.6/moneykit/models/country.py
--rw-r--r--   0        0        0     5363 2023-04-27 15:31:41.268951 moneykit-0.0.6/moneykit/models/create_link_session_body.py
--rw-r--r--   0        0        0     1943 2023-04-27 15:31:41.275461 moneykit-0.0.6/moneykit/models/create_link_session_response.py
--rw-r--r--   0        0        0     3569 2023-04-27 15:31:41.282180 moneykit-0.0.6/moneykit/models/currency.py
--rw-r--r--   0        0        0     1987 2023-04-27 15:31:41.264122 moneykit-0.0.6/moneykit/models/cursor.py
--rw-r--r--   0        0        0     2051 2023-04-27 15:31:41.277712 moneykit-0.0.6/moneykit/models/cursor_pagination.py
--rw-r--r--   0        0        0     1995 2023-04-27 15:31:41.273956 moneykit-0.0.6/moneykit/models/cursors.py
--rw-r--r--   0        0        0     1907 2023-04-27 15:31:41.274205 moneykit-0.0.6/moneykit/models/customer_app_out.py
--rw-r--r--   0        0        0     3533 2023-04-27 15:31:41.280839 moneykit-0.0.6/moneykit/models/customer_user.py
--rw-r--r--   0        0        0     2155 2023-04-27 15:31:41.265449 moneykit-0.0.6/moneykit/models/eft_number.py
--rw-r--r--   0        0        0     2030 2023-04-27 15:31:41.267190 moneykit-0.0.6/moneykit/models/email.py
--rw-r--r--   0        0        0     2978 2023-04-27 15:31:41.278463 moneykit-0.0.6/moneykit/models/email1.py
--rw-r--r--   0        0        0     1919 2023-04-27 15:31:41.269475 moneykit-0.0.6/moneykit/models/exchange_token_body.py
--rw-r--r--   0        0        0     2234 2023-04-27 15:31:41.269872 moneykit-0.0.6/moneykit/models/exchange_token_response.py
--rw-r--r--   0        0        0     2788 2023-04-27 15:31:41.262096 moneykit-0.0.6/moneykit/models/get_account_numbers_response.py
--rw-r--r--   0        0        0     2532 2023-04-27 15:31:41.271109 moneykit-0.0.6/moneykit/models/get_account_response.py
--rw-r--r--   0        0        0     2775 2023-04-27 15:31:41.262970 moneykit-0.0.6/moneykit/models/get_accounts_response.py
--rw-r--r--   0        0        0     3974 2023-04-27 15:31:41.273820 moneykit-0.0.6/moneykit/models/get_transactions_response.py
--rw-r--r--   0        0        0     3696 2023-04-27 15:31:41.262233 moneykit-0.0.6/moneykit/models/http_validation_error.py
--rw-r--r--   0        0        0     2352 2023-04-27 15:31:41.274319 moneykit-0.0.6/moneykit/models/identity.py
--rw-r--r--   0        0        0     3217 2023-04-27 15:31:41.266438 moneykit-0.0.6/moneykit/models/identity_link_product.py
--rw-r--r--   0        0        0     2472 2023-04-27 15:31:41.278092 moneykit-0.0.6/moneykit/models/identity_product_settings.py
--rw-r--r--   0        0        0     2748 2023-04-27 15:31:41.263031 moneykit-0.0.6/moneykit/models/identity_response.py
--rw-r--r--   0        0        0     3027 2023-04-27 15:31:41.276291 moneykit-0.0.6/moneykit/models/institution_error_not_found_response.py
--rw-r--r--   0        0        0     3375 2023-04-27 15:31:41.270373 moneykit-0.0.6/moneykit/models/institution_out.py
--rw-r--r--   0        0        0     1889 2023-04-27 15:31:41.275192 moneykit-0.0.6/moneykit/models/international_number.py
--rw-r--r--   0        0        0     1779 2023-04-27 15:31:41.261468 moneykit-0.0.6/moneykit/models/jwk_set.py
--rw-r--r--   0        0        0     4024 2023-04-27 15:31:41.275607 moneykit-0.0.6/moneykit/models/link.py
--rw-r--r--   0        0        0     4048 2023-04-27 15:31:41.282085 moneykit-0.0.6/moneykit/models/link1.py
--rw-r--r--   0        0        0     4050 2023-04-27 15:31:41.268989 moneykit-0.0.6/moneykit/models/link2.py
--rw-r--r--   0        0        0     4046 2023-04-27 15:31:41.276583 moneykit-0.0.6/moneykit/models/link3.py
--rw-r--r--   0        0        0     4050 2023-04-27 15:31:41.268301 moneykit-0.0.6/moneykit/models/link4.py
--rw-r--r--   0        0        0      724 2023-04-27 15:31:41.272137 moneykit-0.0.6/moneykit/models/link_error.py
--rw-r--r--   0        0        0     2885 2023-04-27 15:31:41.274663 moneykit-0.0.6/moneykit/models/link_error_bad_state_response.py
--rw-r--r--   0        0        0     2845 2023-04-27 15:31:41.263344 moneykit-0.0.6/moneykit/models/link_error_deleted_response.py
--rw-r--r--   0        0        0     2939 2023-04-27 15:31:41.266994 moneykit-0.0.6/moneykit/models/link_error_forbidden_action_response.py
--rw-r--r--   0        0        0     2899 2023-04-27 15:31:41.267289 moneykit-0.0.6/moneykit/models/link_error_not_found_response.py
--rw-r--r--   0        0        0     3071 2023-04-27 15:31:41.273383 moneykit-0.0.6/moneykit/models/link_error_unauthorized_access_response.py
--rw-r--r--   0        0        0     4076 2023-04-27 15:31:41.278288 moneykit-0.0.6/moneykit/models/link_out_common.py
--rw-r--r--   0        0        0     4578 2023-04-27 15:31:41.270181 moneykit-0.0.6/moneykit/models/link_out_full.py
--rw-r--r--   0        0        0      667 2023-04-27 15:31:41.263543 moneykit-0.0.6/moneykit/models/link_permission_scope.py
--rw-r--r--   0        0        0     2627 2023-04-27 15:31:41.278823 moneykit-0.0.6/moneykit/models/link_permissions.py
--rw-r--r--   0        0        0     3359 2023-04-27 15:31:41.275539 moneykit-0.0.6/moneykit/models/link_products.py
--rw-r--r--   0        0        0     3392 2023-04-27 15:31:41.280613 moneykit-0.0.6/moneykit/models/link_session_customer_user.py
--rw-r--r--   0        0        0     3000 2023-04-27 15:31:41.277053 moneykit-0.0.6/moneykit/models/link_session_customer_user_email.py
--rw-r--r--   0        0        0     3464 2023-04-27 15:31:41.262451 moneykit-0.0.6/moneykit/models/link_session_customer_user_phone.py
--rw-r--r--   0        0        0     3027 2023-04-27 15:31:41.264562 moneykit-0.0.6/moneykit/models/link_session_error_forbidden_config_response.py
--rw-r--r--   0        0        0     3027 2023-04-27 15:31:41.263456 moneykit-0.0.6/moneykit/models/link_session_error_invalid_token_exchange.py
--rw-r--r--   0        0        0      636 2023-04-27 15:31:41.262536 moneykit-0.0.6/moneykit/models/link_state.py
--rw-r--r--   0        0        0     4466 2023-04-27 15:31:41.269346 moneykit-0.0.6/moneykit/models/link_state_changed_webhook.py
--rw-r--r--   0        0        0     3767 2023-04-27 15:31:41.261474 moneykit-0.0.6/moneykit/models/location_inner.py
--rw-r--r--   0        0        0      534 2023-04-27 15:31:41.261925 moneykit-0.0.6/moneykit/models/money_kit_env.py
--rw-r--r--   0        0        0     2360 2023-04-27 15:31:41.268871 moneykit-0.0.6/moneykit/models/money_link_features.py
--rw-r--r--   0        0        0     2384 2023-04-27 15:31:41.270801 moneykit-0.0.6/moneykit/models/moneylink_features.py
--rw-r--r--   0        0        0     4104 2023-04-27 15:31:41.262022 moneykit-0.0.6/moneykit/models/numbers.py
--rw-r--r--   0        0        0     3805 2023-04-27 15:31:41.264663 moneykit-0.0.6/moneykit/models/owner.py
--rw-r--r--   0        0        0     2840 2023-04-27 15:31:41.271200 moneykit-0.0.6/moneykit/models/paged_institution_response.py
--rw-r--r--   0        0        0     3441 2023-04-27 15:31:41.275026 moneykit-0.0.6/moneykit/models/phone.py
--rw-r--r--   0        0        0     2262 2023-04-27 15:31:41.267674 moneykit-0.0.6/moneykit/models/phone_number.py
--rw-r--r--   0        0        0      562 2023-04-27 15:31:41.264072 moneykit-0.0.6/moneykit/models/phone_number_type.py
--rw-r--r--   0        0        0      625 2023-04-27 15:31:41.268749 moneykit-0.0.6/moneykit/models/product.py
--rw-r--r--   0        0        0     3364 2023-04-27 15:31:41.268405 moneykit-0.0.6/moneykit/models/products.py
--rw-r--r--   0        0        0     3105 2023-04-27 15:31:41.271633 moneykit-0.0.6/moneykit/models/products1.py
--rw-r--r--   0        0        0     3083 2023-04-27 15:31:41.282673 moneykit-0.0.6/moneykit/models/products_settings.py
--rw-r--r--   0        0        0      585 2023-04-27 15:31:41.271369 moneykit-0.0.6/moneykit/models/provider.py
--rw-r--r--   0        0        0     2011 2023-04-27 15:31:41.263456 moneykit-0.0.6/moneykit/models/refresh_products_body.py
--rw-r--r--   0        0        0     2616 2023-04-27 15:31:41.261332 moneykit-0.0.6/moneykit/models/requested_link_permission.py
--rw-r--r--   0        0        0     5403 2023-04-27 15:31:41.271378 moneykit-0.0.6/moneykit/models/response401_disconnect_links_id_delete.py
--rw-r--r--   0        0        0     4608 2023-04-27 15:31:41.264705 moneykit-0.0.6/moneykit/models/response401_exchange_token_link_session_exchange_token_post.py
--rw-r--r--   0        0        0     5515 2023-04-27 15:31:41.277124 moneykit-0.0.6/moneykit/models/response401_get_account_links_id_accounts_account_id_get.py
--rw-r--r--   0        0        0     5555 2023-04-27 15:31:41.278171 moneykit-0.0.6/moneykit/models/response401_get_account_numbers_links_id_accounts_numbers_get.py
--rw-r--r--   0        0        0     5451 2023-04-27 15:31:41.273521 moneykit-0.0.6/moneykit/models/response401_get_accounts_links_id_accounts_get.py
--rw-r--r--   0        0        0     5467 2023-04-27 15:31:41.264164 moneykit-0.0.6/moneykit/models/response401_get_identities_links_id_identity_get.py
--rw-r--r--   0        0        0     4616 2023-04-27 15:31:41.280562 moneykit-0.0.6/moneykit/models/response401_get_institution_institutions_institution_id_get.py
--rw-r--r--   0        0        0     4520 2023-04-27 15:31:41.266944 moneykit-0.0.6/moneykit/models/response401_get_institutions_institutions_get.py
--rw-r--r--   0        0        0     5355 2023-04-27 15:31:41.281671 moneykit-0.0.6/moneykit/models/response401_get_link_links_id_get.py
--rw-r--r--   0        0        0     5593 2023-04-27 15:31:41.274821 moneykit-0.0.6/moneykit/models/response401_get_transactions_diff_links_id_transactions_sync_get.py
--rw-r--r--   0        0        0     5515 2023-04-27 15:31:41.265815 moneykit-0.0.6/moneykit/models/response401_get_transactions_links_id_transactions_get.py
--rw-r--r--   0        0        0     4544 2023-04-27 15:31:41.277811 moneykit-0.0.6/moneykit/models/response401_get_user_accounts_users_id_accounts_get.py
--rw-r--r--   0        0        0     4496 2023-04-27 15:31:41.262190 moneykit-0.0.6/moneykit/models/response401_get_user_links_users_id_links_get.py
--rw-r--r--   0        0        0     4608 2023-04-27 15:31:41.279933 moneykit-0.0.6/moneykit/models/response401_get_user_transactions_users_id_transactions_get.py
--rw-r--r--   0        0        0     4568 2023-04-27 15:31:41.272230 moneykit-0.0.6/moneykit/models/response401_get_well_known_jwks_well_known_jwks_json_get.py
--rw-r--r--   0        0        0     4552 2023-04-27 15:31:41.279503 moneykit-0.0.6/moneykit/models/response401_instrospect_client_auth_introspect_get.py
--rw-r--r--   0        0        0     5491 2023-04-27 15:31:41.267952 moneykit-0.0.6/moneykit/models/response401_refresh_products_links_id_products_post.py
--rw-r--r--   0        0        0     5395 2023-04-27 15:31:41.272860 moneykit-0.0.6/moneykit/models/response401_update_link_links_id_patch.py
--rw-r--r--   0        0        0     4160 2023-04-27 15:31:41.265921 moneykit-0.0.6/moneykit/models/setting_overrides.py
--rw-r--r--   0        0        0     4169 2023-04-27 15:31:41.271871 moneykit-0.0.6/moneykit/models/settings.py
--rw-r--r--   0        0        0      532 2023-04-27 15:31:41.277234 moneykit-0.0.6/moneykit/models/supported_version.py
--rw-r--r--   0        0        0     2133 2023-04-27 15:31:41.266433 moneykit-0.0.6/moneykit/models/token.py
--rw-r--r--   0        0        0     5126 2023-04-27 15:31:41.276360 moneykit-0.0.6/moneykit/models/transaction.py
--rw-r--r--   0        0        0     3299 2023-04-27 15:31:41.273133 moneykit-0.0.6/moneykit/models/transaction_diff.py
--rw-r--r--   0        0        0     3253 2023-04-27 15:31:41.270149 moneykit-0.0.6/moneykit/models/transaction_sync_response.py
--rw-r--r--   0        0        0      526 2023-04-27 15:31:41.268502 moneykit-0.0.6/moneykit/models/transaction_type.py
--rw-r--r--   0        0        0      532 2023-04-27 15:31:41.271410 moneykit-0.0.6/moneykit/models/transaction_type_filter.py
--rw-r--r--   0        0        0     2818 2023-04-27 15:31:41.261339 moneykit-0.0.6/moneykit/models/transactions.py
--rw-r--r--   0        0        0     3320 2023-04-27 15:31:41.264452 moneykit-0.0.6/moneykit/models/transactions1.py
--rw-r--r--   0        0        0     3265 2023-04-27 15:31:41.265283 moneykit-0.0.6/moneykit/models/transactions_link_product.py
--rw-r--r--   0        0        0     2938 2023-04-27 15:31:41.274009 moneykit-0.0.6/moneykit/models/transactions_product_settings.py
--rw-r--r--   0        0        0     2529 2023-04-27 15:31:41.265379 moneykit-0.0.6/moneykit/models/update_link_body.py
--rw-r--r--   0        0        0     2485 2023-04-27 15:31:41.266502 moneykit-0.0.6/moneykit/models/user_accounts_out.py
--rw-r--r--   0        0        0     2444 2023-04-27 15:31:41.275951 moneykit-0.0.6/moneykit/models/user_links_out.py
--rw-r--r--   0        0        0     3730 2023-04-27 15:31:41.281239 moneykit-0.0.6/moneykit/models/user_transactions_paged_response.py
--rw-r--r--   0        0        0     2475 2023-04-27 15:31:41.273231 moneykit-0.0.6/moneykit/models/validation_error.py
--rw-r--r--   0        0        0      963 2023-04-27 15:32:15.096424 moneykit-0.0.6/moneykit/plaid_compatible/__init__.py
--rw-r--r--   0        0        0      227 2023-04-27 15:32:15.128739 moneykit-0.0.6/moneykit/plaid_compatible/api/__init__.py
--rw-r--r--   0        0        0    50030 2023-04-27 15:32:15.129474 moneykit-0.0.6/moneykit/plaid_compatible/api/plaid_api.py
--rw-r--r--   0        0        0    36839 2023-04-27 15:32:15.130349 moneykit-0.0.6/moneykit/plaid_compatible/api_client.py
--rw-r--r--   0        0        0      470 2023-04-27 15:32:15.095858 moneykit-0.0.6/moneykit/plaid_compatible/apis/__init__.py
--rw-r--r--   0        0        0    17735 2023-04-27 15:32:15.095649 moneykit-0.0.6/moneykit/plaid_compatible/configuration.py
--rw-r--r--   0        0        0     5093 2023-04-27 15:32:15.129747 moneykit-0.0.6/moneykit/plaid_compatible/exceptions.py
--rw-r--r--   0        0        0      348 2023-04-27 15:32:15.108804 moneykit-0.0.6/moneykit/plaid_compatible/model/__init__.py
--rw-r--r--   0        0        0    10890 2023-04-27 15:32:15.114848 moneykit-0.0.6/moneykit/plaid_compatible/model/account_balance.py
--rw-r--r--   0        0        0    10741 2023-04-27 15:32:15.111856 moneykit-0.0.6/moneykit/plaid_compatible/model/account_base.py
--rw-r--r--   0        0        0    11657 2023-04-27 15:32:15.106184 moneykit-0.0.6/moneykit/plaid_compatible/model/account_identity.py
--rw-r--r--   0        0        0    11414 2023-04-27 15:32:15.111248 moneykit-0.0.6/moneykit/plaid_compatible/model/account_subtype.py
--rw-r--r--   0        0        0     7191 2023-04-27 15:32:15.125685 moneykit-0.0.6/moneykit/plaid_compatible/model/account_type.py
--rw-r--r--   0        0        0     7674 2023-04-27 15:32:15.112197 moneykit-0.0.6/moneykit/plaid_compatible/model/accounts_get_request.py
--rw-r--r--   0        0        0     6636 2023-04-27 15:32:15.123182 moneykit-0.0.6/moneykit/plaid_compatible/model/accounts_get_request_options.py
--rw-r--r--   0        0        0     7447 2023-04-27 15:32:15.118764 moneykit-0.0.6/moneykit/plaid_compatible/model/accounts_get_response.py
--rw-r--r--   0        0        0     6925 2023-04-27 15:32:15.098822 moneykit-0.0.6/moneykit/plaid_compatible/model/address.py
--rw-r--r--   0        0        0     7501 2023-04-27 15:32:15.113361 moneykit-0.0.6/moneykit/plaid_compatible/model/address_data.py
--rw-r--r--   0        0        0     7793 2023-04-27 15:32:15.123493 moneykit-0.0.6/moneykit/plaid_compatible/model/auth_get_numbers.py
--rw-r--r--   0        0        0     7642 2023-04-27 15:32:15.122215 moneykit-0.0.6/moneykit/plaid_compatible/model/auth_get_request.py
--rw-r--r--   0        0        0     6715 2023-04-27 15:32:15.111534 moneykit-0.0.6/moneykit/plaid_compatible/model/auth_get_request_options.py
--rw-r--r--   0        0        0     7635 2023-04-27 15:32:15.127676 moneykit-0.0.6/moneykit/plaid_compatible/model/auth_get_response.py
--rw-r--r--   0        0        0     7265 2023-04-27 15:32:15.101156 moneykit-0.0.6/moneykit/plaid_compatible/model/counterparty_type.py
--rw-r--r--   0        0        0     6955 2023-04-27 15:32:15.123801 moneykit-0.0.6/moneykit/plaid_compatible/model/country_code.py
--rw-r--r--   0        0        0     7029 2023-04-27 15:32:15.101491 moneykit-0.0.6/moneykit/plaid_compatible/model/credit_account_subtype.py
--rw-r--r--   0        0        0     7070 2023-04-27 15:32:15.098118 moneykit-0.0.6/moneykit/plaid_compatible/model/credit_filter.py
--rw-r--r--   0        0        0     7417 2023-04-27 15:32:15.120721 moneykit-0.0.6/moneykit/plaid_compatible/model/depository_account_subtype.py
--rw-r--r--   0        0        0     7102 2023-04-27 15:32:15.122570 moneykit-0.0.6/moneykit/plaid_compatible/model/depository_filter.py
--rw-r--r--   0        0        0     6966 2023-04-27 15:32:15.116485 moneykit-0.0.6/moneykit/plaid_compatible/model/email.py
--rw-r--r--   0        0        0     6965 2023-04-27 15:32:15.127948 moneykit-0.0.6/moneykit/plaid_compatible/model/employment_source_type.py
--rw-r--r--   0        0        0     6724 2023-04-27 15:32:15.113087 moneykit-0.0.6/moneykit/plaid_compatible/model/http_validation_error.py
--rw-r--r--   0        0        0     9101 2023-04-27 15:32:15.116837 moneykit-0.0.6/moneykit/plaid_compatible/model/id_number_type.py
--rw-r--r--   0        0        0     7674 2023-04-27 15:32:15.119155 moneykit-0.0.6/moneykit/plaid_compatible/model/identity_get_request.py
--rw-r--r--   0        0        0     6723 2023-04-27 15:32:15.120335 moneykit-0.0.6/moneykit/plaid_compatible/model/identity_get_request_options.py
--rw-r--r--   0        0        0     7362 2023-04-27 15:32:15.117571 moneykit-0.0.6/moneykit/plaid_compatible/model/identity_get_response.py
--rw-r--r--   0        0        0     7111 2023-04-27 15:32:15.100566 moneykit-0.0.6/moneykit/plaid_compatible/model/income_verification_payroll_flow_type.py
--rw-r--r--   0        0        0     6981 2023-04-27 15:32:15.103155 moneykit-0.0.6/moneykit/plaid_compatible/model/income_verification_source_type.py
--rw-r--r--   0        0        0     9913 2023-04-27 15:32:15.125994 moneykit-0.0.6/moneykit/plaid_compatible/model/investment_account_subtype.py
--rw-r--r--   0        0        0     7102 2023-04-27 15:32:15.114235 moneykit-0.0.6/moneykit/plaid_compatible/model/investment_filter.py
--rw-r--r--   0        0        0    10420 2023-04-27 15:32:15.127395 moneykit-0.0.6/moneykit/plaid_compatible/model/item.py
--rw-r--r--   0        0        0     7717 2023-04-27 15:32:15.112476 moneykit-0.0.6/moneykit/plaid_compatible/model/item_error_webhook.py
--rw-r--r--   0        0        0     7265 2023-04-27 15:32:15.116194 moneykit-0.0.6/moneykit/plaid_compatible/model/item_get_request.py
--rw-r--r--   0        0        0     7287 2023-04-27 15:32:15.100216 moneykit-0.0.6/moneykit/plaid_compatible/model/item_get_response.py
--rw-r--r--   0        0        0     7331 2023-04-27 15:32:15.117188 moneykit-0.0.6/moneykit/plaid_compatible/model/item_public_token_exchange_request.py
--rw-r--r--   0        0        0     7235 2023-04-27 15:32:15.128231 moneykit-0.0.6/moneykit/plaid_compatible/model/item_public_token_exchange_response.py
--rw-r--r--   0        0        0     7271 2023-04-27 15:32:15.102124 moneykit-0.0.6/moneykit/plaid_compatible/model/item_remove_request.py
--rw-r--r--   0        0        0     6715 2023-04-27 15:32:15.124733 moneykit-0.0.6/moneykit/plaid_compatible/model/item_remove_response.py
--rw-r--r--   0        0        0     7362 2023-04-27 15:32:15.122888 moneykit-0.0.6/moneykit/plaid_compatible/model/item_status_investments.py
--rw-r--r--   0        0        0     6852 2023-04-27 15:32:15.113893 moneykit-0.0.6/moneykit/plaid_compatible/model/item_status_last_webhook.py
--rw-r--r--   0        0        0     7489 2023-04-27 15:32:15.121123 moneykit-0.0.6/moneykit/plaid_compatible/model/item_status_nullable.py
--rw-r--r--   0        0        0     7366 2023-04-27 15:32:15.104784 moneykit-0.0.6/moneykit/plaid_compatible/model/item_status_transactions.py
--rw-r--r--   0        0        0     7595 2023-04-27 15:32:15.126274 moneykit-0.0.6/moneykit/plaid_compatible/model/link_token_account_filters.py
--rw-r--r--   0        0        0     6644 2023-04-27 15:32:15.110857 moneykit-0.0.6/moneykit/plaid_compatible/model/link_token_create_institution_data.py
--rw-r--r--   0        0        0    21548 2023-04-27 15:32:15.125161 moneykit-0.0.6/moneykit/plaid_compatible/model/link_token_create_request.py
--rw-r--r--   0        0        0     8258 2023-04-27 15:32:15.099877 moneykit-0.0.6/moneykit/plaid_compatible/model/link_token_create_request_auth.py
--rw-r--r--   0        0        0     6733 2023-04-27 15:32:15.105787 moneykit-0.0.6/moneykit/plaid_compatible/model/link_token_create_request_deposit_switch.py
--rw-r--r--   0        0        0     7534 2023-04-27 15:32:15.106562 moneykit-0.0.6/moneykit/plaid_compatible/model/link_token_create_request_employment.py
--rw-r--r--   0        0        0     6722 2023-04-27 15:32:15.108289 moneykit-0.0.6/moneykit/plaid_compatible/model/link_token_create_request_employment_bank_income.py
--rw-r--r--   0        0        0     7661 2023-04-27 15:32:15.115600 moneykit-0.0.6/moneykit/plaid_compatible/model/link_token_create_request_identity_verification.py
--rw-r--r--   0        0        0    10586 2023-04-27 15:32:15.124133 moneykit-0.0.6/moneykit/plaid_compatible/model/link_token_create_request_income_verification.py
--rw-r--r--   0        0        0     7020 2023-04-27 15:32:15.097007 moneykit-0.0.6/moneykit/plaid_compatible/model/link_token_create_request_income_verification_bank_income.py
--rw-r--r--   0        0        0     7697 2023-04-27 15:32:15.107151 moneykit-0.0.6/moneykit/plaid_compatible/model/link_token_create_request_income_verification_payroll_income.py
--rw-r--r--   0        0        0     6937 2023-04-27 15:32:15.097783 moneykit-0.0.6/moneykit/plaid_compatible/model/link_token_create_request_payment_initiation.py
--rw-r--r--   0        0        0     6940 2023-04-27 15:32:15.114522 moneykit-0.0.6/moneykit/plaid_compatible/model/link_token_create_request_transfer.py
--rw-r--r--   0        0        0     6779 2023-04-27 15:32:15.104448 moneykit-0.0.6/moneykit/plaid_compatible/model/link_token_create_request_update.py
--rw-r--r--   0        0        0    11399 2023-04-27 15:32:15.098515 moneykit-0.0.6/moneykit/plaid_compatible/model/link_token_create_request_user.py
--rw-r--r--   0        0        0     6963 2023-04-27 15:32:15.126554 moneykit-0.0.6/moneykit/plaid_compatible/model/link_token_create_request_user_name.py
--rw-r--r--   0        0        0     8414 2023-04-27 15:32:15.104144 moneykit-0.0.6/moneykit/plaid_compatible/model/link_token_create_request_user_stated_income_source.py
--rw-r--r--   0        0        0     7615 2023-04-27 15:32:15.107454 moneykit-0.0.6/moneykit/plaid_compatible/model/link_token_create_response.py
--rw-r--r--   0        0        0     6616 2023-04-27 15:32:15.119981 moneykit-0.0.6/moneykit/plaid_compatible/model/link_token_eu_config.py
--rw-r--r--   0        0        0     6769 2023-04-27 15:32:15.127095 moneykit-0.0.6/moneykit/plaid_compatible/model/link_token_investments.py
--rw-r--r--   0        0        0     7573 2023-04-27 15:32:15.106855 moneykit-0.0.6/moneykit/plaid_compatible/model/loan_account_subtype.py
--rw-r--r--   0        0        0     7054 2023-04-27 15:32:15.109921 moneykit-0.0.6/moneykit/plaid_compatible/model/loan_filter.py
--rw-r--r--   0        0        0     7487 2023-04-27 15:32:15.113630 moneykit-0.0.6/moneykit/plaid_compatible/model/location.py
--rw-r--r--   0        0        0     7716 2023-04-27 15:32:15.109336 moneykit-0.0.6/moneykit/plaid_compatible/model/money_link_features.py
--rw-r--r--   0        0        0     8621 2023-04-27 15:32:15.124459 moneykit-0.0.6/moneykit/plaid_compatible/model/numbers_ach.py
--rw-r--r--   0        0        0     7019 2023-04-27 15:32:15.103444 moneykit-0.0.6/moneykit/plaid_compatible/model/numbers_bacs.py
--rw-r--r--   0        0        0     7225 2023-04-27 15:32:15.108613 moneykit-0.0.6/moneykit/plaid_compatible/model/numbers_eft.py
--rw-r--r--   0        0        0     7007 2023-04-27 15:32:15.112751 moneykit-0.0.6/moneykit/plaid_compatible/model/numbers_international.py
--rw-r--r--   0        0        0     8304 2023-04-27 15:32:15.110207 moneykit-0.0.6/moneykit/plaid_compatible/model/owner.py
--rw-r--r--   0        0        0     7593 2023-04-27 15:32:15.097403 moneykit-0.0.6/moneykit/plaid_compatible/model/payment_meta.py
--rw-r--r--   0        0        0     6930 2023-04-27 15:32:15.101817 moneykit-0.0.6/moneykit/plaid_compatible/model/personal_finance_category.py
--rw-r--r--   0        0        0     6934 2023-04-27 15:32:15.107717 moneykit-0.0.6/moneykit/plaid_compatible/model/phone_number.py
--rw-r--r--   0        0        0     9494 2023-04-27 15:32:15.128531 moneykit-0.0.6/moneykit/plaid_compatible/model/plaid_error.py
--rw-r--r--   0        0        0     8113 2023-04-27 15:32:15.099166 moneykit-0.0.6/moneykit/plaid_compatible/model/plaid_error_type.py
--rw-r--r--   0        0        0     7129 2023-04-27 15:32:15.109044 moneykit-0.0.6/moneykit/plaid_compatible/model/products.py
--rw-r--r--   0        0        0     6610 2023-04-27 15:32:15.099511 moneykit-0.0.6/moneykit/plaid_compatible/model/removed_transaction.py
--rw-r--r--   0        0        0    16756 2023-04-27 15:32:15.105222 moneykit-0.0.6/moneykit/plaid_compatible/model/transaction.py
--rw-r--r--   0        0        0     7632 2023-04-27 15:32:15.109657 moneykit-0.0.6/moneykit/plaid_compatible/model/transaction_code.py
--rw-r--r--   0        0        0     7510 2023-04-27 15:32:15.102816 moneykit-0.0.6/moneykit/plaid_compatible/model/transaction_counterparty.py
--rw-r--r--   0        0        0     8236 2023-04-27 15:32:15.117976 moneykit-0.0.6/moneykit/plaid_compatible/model/transactions_get_request.py
--rw-r--r--   0        0        0     9639 2023-04-27 15:32:15.115239 moneykit-0.0.6/moneykit/plaid_compatible/model/transactions_get_request_options.py
--rw-r--r--   0        0        0     8530 2023-04-27 15:32:15.121523 moneykit-0.0.6/moneykit/plaid_compatible/model/transactions_get_response.py
--rw-r--r--   0        0        0     7289 2023-04-27 15:32:15.126834 moneykit-0.0.6/moneykit/plaid_compatible/model/transactions_refresh_request.py
--rw-r--r--   0        0        0     6733 2023-04-27 15:32:15.100879 moneykit-0.0.6/moneykit/plaid_compatible/model/transactions_refresh_response.py
--rw-r--r--   0        0        0     8397 2023-04-27 15:32:15.118379 moneykit-0.0.6/moneykit/plaid_compatible/model/transactions_sync_request.py
--rw-r--r--   0        0        0     8427 2023-04-27 15:32:15.121895 moneykit-0.0.6/moneykit/plaid_compatible/model/transactions_sync_request_options.py
--rw-r--r--   0        0        0     8900 2023-04-27 15:32:15.110516 moneykit-0.0.6/moneykit/plaid_compatible/model/transactions_sync_response.py
--rw-r--r--   0        0        0     7916 2023-04-27 15:32:15.115910 moneykit-0.0.6/moneykit/plaid_compatible/model/user_address.py
--rw-r--r--   0        0        0     6950 2023-04-27 15:32:15.119582 moneykit-0.0.6/moneykit/plaid_compatible/model/user_id_number.py
--rw-r--r--   0        0        0     7625 2023-04-27 15:32:15.125418 moneykit-0.0.6/moneykit/plaid_compatible/model/user_stated_income_source_category.py
--rw-r--r--   0        0        0     7187 2023-04-27 15:32:15.103821 moneykit-0.0.6/moneykit/plaid_compatible/model/user_stated_income_source_frequency.py
--rw-r--r--   0        0        0     7027 2023-04-27 15:32:15.107982 moneykit-0.0.6/moneykit/plaid_compatible/model/user_stated_income_source_pay_type.py
--rw-r--r--   0        0        0     6793 2023-04-27 15:32:15.102418 moneykit-0.0.6/moneykit/plaid_compatible/model/validation_error.py
--rw-r--r--   0        0        0     7069 2023-04-27 15:32:15.105481 moneykit-0.0.6/moneykit/plaid_compatible/model/webhook_environment_values.py
--rw-r--r--   0        0        0    74795 2023-04-27 15:32:15.095156 moneykit-0.0.6/moneykit/plaid_compatible/model_utils.py
--rw-r--r--   0        0        0     8892 2023-04-27 15:32:15.096683 moneykit-0.0.6/moneykit/plaid_compatible/models/__init__.py
--rw-r--r--   0        0        0    12537 2023-04-27 15:32:15.096197 moneykit-0.0.6/moneykit/plaid_compatible/rest.py
--rw-r--r--   0        0        0    12478 2023-04-27 15:31:41.279569 moneykit-0.0.6/moneykit/rest.py
--rw-r--r--   0        0        0      935 2023-04-27 15:58:50.661421 moneykit-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1107 1970-01-01 00:00:00.000000 moneykit-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0    20273 2023-04-28 15:49:26.000000 moneykit-0.0.7/README.md
+-rw-r--r--   0        0        0      739 2023-04-28 15:51:49.450336 moneykit-0.0.7/moneykit/__init__.py
+-rw-r--r--   0        0        0    56712 2023-04-28 15:49:38.861106 moneykit-0.0.7/moneykit/api_client.py
+-rw-r--r--   0        0        0      215 2023-04-28 15:49:35.985342 moneykit-0.0.7/moneykit/apis/__init__.py
+-rw-r--r--   0        0        0     3789 2023-04-28 15:49:38.870097 moneykit-0.0.7/moneykit/apis/path_to_api.py
+-rw-r--r--   0        0        0      235 2023-04-28 15:49:26.000000 moneykit-0.0.7/moneykit/apis/paths/__init__.py
+-rw-r--r--   0        0        0      108 2023-04-28 15:49:21.000000 moneykit-0.0.7/moneykit/apis/paths/auth_introspect.py
+-rw-r--r--   0        0        0      101 2023-04-28 15:49:21.000000 moneykit-0.0.7/moneykit/apis/paths/auth_token.py
+-rw-r--r--   0        0        0      103 2023-04-28 15:49:23.000000 moneykit-0.0.7/moneykit/apis/paths/institutions.py
+-rw-r--r--   0        0        0      131 2023-04-28 15:49:23.000000 moneykit-0.0.7/moneykit/apis/paths/institutions_institution_id.py
+-rw-r--r--   0        0        0      146 2023-04-28 15:49:23.000000 moneykit-0.0.7/moneykit/apis/paths/institutions_institution_id_styling.py
+-rw-r--r--   0        0        0      105 2023-04-28 15:49:23.000000 moneykit-0.0.7/moneykit/apis/paths/link_session.py
+-rw-r--r--   0        0        0      133 2023-04-28 15:49:23.000000 moneykit-0.0.7/moneykit/apis/paths/link_session_exchange_token.py
+-rw-r--r--   0        0        0      239 2023-04-28 15:49:38.871155 moneykit-0.0.7/moneykit/apis/paths/links_id.py
+-rw-r--r--   0        0        0      111 2023-04-28 15:49:22.000000 moneykit-0.0.7/moneykit/apis/paths/links_id_accounts.py
+-rw-r--r--   0        0        0      131 2023-04-28 15:49:22.000000 moneykit-0.0.7/moneykit/apis/paths/links_id_accounts_account_id.py
+-rw-r--r--   0        0        0      126 2023-04-28 15:49:22.000000 moneykit-0.0.7/moneykit/apis/paths/links_id_accounts_numbers.py
+-rw-r--r--   0        0        0      111 2023-04-28 15:49:23.000000 moneykit-0.0.7/moneykit/apis/paths/links_id_identity.py
+-rw-r--r--   0        0        0      114 2023-04-28 15:49:24.000000 moneykit-0.0.7/moneykit/apis/paths/links_id_products.py
+-rw-r--r--   0        0        0      119 2023-04-28 15:49:25.000000 moneykit-0.0.7/moneykit/apis/paths/links_id_transactions.py
+-rw-r--r--   0        0        0      128 2023-04-28 15:49:25.000000 moneykit-0.0.7/moneykit/apis/paths/links_id_transactions_sync.py
+-rw-r--r--   0        0        0      111 2023-04-28 15:49:26.000000 moneykit-0.0.7/moneykit/apis/paths/users_id_accounts.py
+-rw-r--r--   0        0        0      105 2023-04-28 15:49:26.000000 moneykit-0.0.7/moneykit/apis/paths/users_id_links.py
+-rw-r--r--   0        0        0      119 2023-04-28 15:49:26.000000 moneykit-0.0.7/moneykit/apis/paths/users_id_transactions.py
+-rw-r--r--   0        0        0      116 2023-04-28 15:49:21.000000 moneykit-0.0.7/moneykit/apis/paths/well_known_jwks_json.py
+-rw-r--r--   0        0        0     1650 2023-04-28 15:49:38.870553 moneykit-0.0.7/moneykit/apis/tag_to_api.py
+-rw-r--r--   0        0        0      575 2023-04-28 15:49:26.000000 moneykit-0.0.7/moneykit/apis/tags/__init__.py
+-rw-r--r--   0        0        0      718 2023-04-28 15:49:38.864843 moneykit-0.0.7/moneykit/apis/tags/access_token_api.py
+-rw-r--r--   0        0        0      552 2023-04-28 15:49:35.998253 moneykit-0.0.7/moneykit/apis/tags/account_numbers_api.py
+-rw-r--r--   0        0        0      797 2023-04-28 15:49:38.865044 moneykit-0.0.7/moneykit/apis/tags/accounts_api.py
+-rw-r--r--   0        0        0      530 2023-04-28 15:49:36.002106 moneykit-0.0.7/moneykit/apis/tags/identity_api.py
+-rw-r--r--   0        0        0      743 2023-04-28 15:49:38.865347 moneykit-0.0.7/moneykit/apis/tags/institutions_api.py
+-rw-r--r--   0        0        0      630 2023-04-28 15:49:36.004372 moneykit-0.0.7/moneykit/apis/tags/link_session_api.py
+-rw-r--r--   0        0        0      722 2023-04-28 15:49:38.867992 moneykit-0.0.7/moneykit/apis/tags/links_api.py
+-rw-r--r--   0        0        0      535 2023-04-28 15:49:36.005215 moneykit-0.0.7/moneykit/apis/tags/products_api.py
+-rw-r--r--   0        0        0      743 2023-04-28 15:49:36.007058 moneykit-0.0.7/moneykit/apis/tags/transactions_api.py
+-rw-r--r--   0        0        0      706 2023-04-28 15:49:36.007188 moneykit-0.0.7/moneykit/apis/tags/users_api.py
+-rw-r--r--   0        0        0    18643 2023-04-28 15:49:38.843047 moneykit-0.0.7/moneykit/configuration.py
+-rw-r--r--   0        0        0     4490 2023-04-28 15:49:36.030900 moneykit-0.0.7/moneykit/exceptions.py
+-rw-r--r--   0        0        0      342 2023-04-28 15:49:26.000000 moneykit-0.0.7/moneykit/model/__init__.py
+-rw-r--r--   0        0        0    11454 2023-04-28 15:49:38.863988 moneykit-0.0.7/moneykit/model/account.py
+-rw-r--r--   0        0        0    11337 2023-04-28 15:49:38.871993 moneykit-0.0.7/moneykit/model/account.pyi
+-rw-r--r--   0        0        0     9362 2023-04-28 15:49:38.857098 moneykit-0.0.7/moneykit/model/account_balances.py
+-rw-r--r--   0        0        0     9265 2023-04-28 15:49:38.848070 moneykit-0.0.7/moneykit/model/account_balances.pyi
+-rw-r--r--   0        0        0     5097 2023-04-28 15:49:38.846266 moneykit-0.0.7/moneykit/model/account_group.py
+-rw-r--r--   0        0        0     5034 2023-04-28 15:49:38.869402 moneykit-0.0.7/moneykit/model/account_group.pyi
+-rw-r--r--   0        0        0    12821 2023-04-28 15:49:38.842983 moneykit-0.0.7/moneykit/model/account_identity.py
+-rw-r--r--   0        0        0    12684 2023-04-28 15:49:38.845722 moneykit-0.0.7/moneykit/model/account_identity.pyi
+-rw-r--r--   0        0        0     7878 2023-04-28 15:49:38.884406 moneykit-0.0.7/moneykit/model/account_numbers.py
+-rw-r--r--   0        0        0     7774 2023-04-28 15:49:38.844577 moneykit-0.0.7/moneykit/model/account_numbers.pyi
+-rw-r--r--   0        0        0     5932 2023-04-28 15:49:38.861586 moneykit-0.0.7/moneykit/model/account_numbers_link_product.py
+-rw-r--r--   0        0        0     5852 2023-04-28 15:49:38.876869 moneykit-0.0.7/moneykit/model/account_numbers_link_product.pyi
+-rw-r--r--   0        0        0     3467 2023-04-28 15:49:38.857710 moneykit-0.0.7/moneykit/model/account_numbers_product_settings.py
+-rw-r--r--   0        0        0     3409 2023-04-28 15:49:38.870271 moneykit-0.0.7/moneykit/model/account_numbers_product_settings.pyi
+-rw-r--r--   0        0        0     2418 2023-04-28 15:49:38.857288 moneykit-0.0.7/moneykit/model/account_type.py
+-rw-r--r--   0        0        0     1831 2023-04-28 15:49:38.846888 moneykit-0.0.7/moneykit/model/account_type.pyi
+-rw-r--r--   0        0        0    14837 2023-04-28 15:49:38.849741 moneykit-0.0.7/moneykit/model/account_with_account_numbers.py
+-rw-r--r--   0        0        0    14701 2023-04-28 15:49:38.862149 moneykit-0.0.7/moneykit/model/account_with_account_numbers.pyi
+-rw-r--r--   0        0        0     5109 2023-04-28 15:49:38.875074 moneykit-0.0.7/moneykit/model/accounts_link_product.py
+-rw-r--r--   0        0        0     5048 2023-04-28 15:49:38.844170 moneykit-0.0.7/moneykit/model/accounts_link_product.pyi
+-rw-r--r--   0        0        0     5023 2023-04-28 15:49:38.853103 moneykit-0.0.7/moneykit/model/ach_number.py
+-rw-r--r--   0        0        0     4974 2023-04-28 15:49:38.844034 moneykit-0.0.7/moneykit/model/ach_number.pyi
+-rw-r--r--   0        0        0     8379 2023-04-28 15:49:38.848713 moneykit-0.0.7/moneykit/model/address.py
+-rw-r--r--   0        0        0     8248 2023-04-28 15:49:38.862727 moneykit-0.0.7/moneykit/model/address.pyi
+-rw-r--r--   0        0        0     5259 2023-04-28 15:49:38.874767 moneykit-0.0.7/moneykit/model/api_error_auth_expired_access_token_response.py
+-rw-r--r--   0        0        0     4981 2023-04-28 15:49:38.842230 moneykit-0.0.7/moneykit/model/api_error_auth_expired_access_token_response.pyi
+-rw-r--r--   0        0        0     5291 2023-04-28 15:49:38.874043 moneykit-0.0.7/moneykit/model/api_error_auth_unauthorized_response.py
+-rw-r--r--   0        0        0     5030 2023-04-28 15:49:38.871035 moneykit-0.0.7/moneykit/model/api_error_auth_unauthorized_response.pyi
+-rw-r--r--   0        0        0     5225 2023-04-28 15:49:38.848183 moneykit-0.0.7/moneykit/model/api_error_rate_limit_exceeded_response.py
+-rw-r--r--   0        0        0     4959 2023-04-28 15:49:38.875463 moneykit-0.0.7/moneykit/model/api_error_rate_limit_exceeded_response.pyi
+-rw-r--r--   0        0        0     3626 2023-04-28 15:49:38.845453 moneykit-0.0.7/moneykit/model/bacs_number.py
+-rw-r--r--   0        0        0     3582 2023-04-28 15:49:38.847420 moneykit-0.0.7/moneykit/model/bacs_number.pyi
+-rw-r--r--   0        0        0     5566 2023-04-28 15:49:38.890149 moneykit-0.0.7/moneykit/model/basic_account_details.py
+-rw-r--r--   0        0        0     5484 2023-04-28 15:49:38.875544 moneykit-0.0.7/moneykit/model/basic_account_details.pyi
+-rw-r--r--   0        0        0     1162 2023-04-28 15:49:38.862461 moneykit-0.0.7/moneykit/model/country.py
+-rw-r--r--   0        0        0     1025 2023-04-28 15:49:38.860758 moneykit-0.0.7/moneykit/model/country.pyi
+-rw-r--r--   0        0        0    17582 2023-04-28 15:49:38.853450 moneykit-0.0.7/moneykit/model/create_link_session_request.py
+-rw-r--r--   0        0        0    17291 2023-04-28 15:49:38.856335 moneykit-0.0.7/moneykit/model/create_link_session_request.pyi
+-rw-r--r--   0        0        0     2943 2023-04-28 15:49:38.858622 moneykit-0.0.7/moneykit/model/create_link_session_response.py
+-rw-r--r--   0        0        0     2903 2023-04-28 15:49:38.848974 moneykit-0.0.7/moneykit/model/create_link_session_response.pyi
+-rw-r--r--   0        0        0    18827 2023-04-28 15:49:38.863236 moneykit-0.0.7/moneykit/model/currency.py
+-rw-r--r--   0        0        0    13878 2023-04-28 15:49:38.885098 moneykit-0.0.7/moneykit/model/currency.pyi
+-rw-r--r--   0        0        0     3163 2023-04-28 15:49:38.863873 moneykit-0.0.7/moneykit/model/cursor_pagination.py
+-rw-r--r--   0        0        0     3122 2023-04-28 15:49:38.864985 moneykit-0.0.7/moneykit/model/cursor_pagination.pyi
+-rw-r--r--   0        0        0     3473 2023-04-28 15:49:38.868796 moneykit-0.0.7/moneykit/model/customer_app.py
+-rw-r--r--   0        0        0     3415 2023-04-28 15:49:38.844814 moneykit-0.0.7/moneykit/model/customer_app.pyi
+-rw-r--r--   0        0        0     4489 2023-04-28 15:49:38.846541 moneykit-0.0.7/moneykit/model/eft_number.py
+-rw-r--r--   0        0        0     4427 2023-04-28 15:49:38.873254 moneykit-0.0.7/moneykit/model/eft_number.pyi
+-rw-r--r--   0        0        0     3449 2023-04-28 15:49:38.864519 moneykit-0.0.7/moneykit/model/email.py
+-rw-r--r--   0        0        0     3391 2023-04-28 15:49:38.858861 moneykit-0.0.7/moneykit/model/email.pyi
+-rw-r--r--   0        0        0     2933 2023-04-28 15:49:38.847602 moneykit-0.0.7/moneykit/model/exchange_token_request.py
+-rw-r--r--   0        0        0     2893 2023-04-28 15:49:38.853791 moneykit-0.0.7/moneykit/model/exchange_token_request.pyi
+-rw-r--r--   0        0        0     6194 2023-04-28 15:49:38.847814 moneykit-0.0.7/moneykit/model/exchange_token_response.py
+-rw-r--r--   0        0        0     6133 2023-04-28 15:49:38.874996 moneykit-0.0.7/moneykit/model/exchange_token_response.pyi
+-rw-r--r--   0        0        0     4350 2023-04-28 15:49:38.857821 moneykit-0.0.7/moneykit/model/generate_access_token_response.py
+-rw-r--r--   0        0        0     4274 2023-04-28 15:49:38.872872 moneykit-0.0.7/moneykit/model/generate_access_token_response.pyi
+-rw-r--r--   0        0        0     4468 2023-04-28 15:49:38.872579 moneykit-0.0.7/moneykit/model/get_account_numbers_response.py
+-rw-r--r--   0        0        0     4405 2023-04-28 15:49:38.860892 moneykit-0.0.7/moneykit/model/get_account_numbers_response.pyi
+-rw-r--r--   0        0        0     6175 2023-04-28 15:49:38.849501 moneykit-0.0.7/moneykit/model/get_account_response.py
+-rw-r--r--   0        0        0     6114 2023-04-28 15:49:38.864175 moneykit-0.0.7/moneykit/model/get_account_response.pyi
+-rw-r--r--   0        0        0     6991 2023-04-28 15:49:38.870178 moneykit-0.0.7/moneykit/model/get_accounts_response.py
+-rw-r--r--   0        0        0     6928 2023-04-28 15:49:38.848796 moneykit-0.0.7/moneykit/model/get_accounts_response.pyi
+-rw-r--r--   0        0        0     7164 2023-04-28 15:49:38.870334 moneykit-0.0.7/moneykit/model/get_institutions_response.py
+-rw-r--r--   0        0        0     7101 2023-04-28 15:49:38.847296 moneykit-0.0.7/moneykit/model/get_institutions_response.pyi
+-rw-r--r--   0        0        0    10245 2023-04-28 15:49:38.842506 moneykit-0.0.7/moneykit/model/get_transactions_response.py
+-rw-r--r--   0        0        0    10108 2023-04-28 15:49:38.852380 moneykit-0.0.7/moneykit/model/get_transactions_response.pyi
+-rw-r--r--   0        0        0     3894 2023-04-28 15:49:38.859527 moneykit-0.0.7/moneykit/model/get_user_accounts_response.py
+-rw-r--r--   0        0        0     3849 2023-04-28 15:49:38.863104 moneykit-0.0.7/moneykit/model/get_user_accounts_response.pyi
+-rw-r--r--   0        0        0     3874 2023-04-28 15:49:38.856994 moneykit-0.0.7/moneykit/model/get_user_links_response.py
+-rw-r--r--   0        0        0     3829 2023-04-28 15:49:38.868719 moneykit-0.0.7/moneykit/model/get_user_links_response.pyi
+-rw-r--r--   0        0        0     7425 2023-04-28 15:49:38.876937 moneykit-0.0.7/moneykit/model/get_user_transactions_response.py
+-rw-r--r--   0        0        0     7306 2023-04-28 15:49:38.857777 moneykit-0.0.7/moneykit/model/get_user_transactions_response.pyi
+-rw-r--r--   0        0        0     6893 2023-04-28 15:49:38.844031 moneykit-0.0.7/moneykit/model/http_validation_error.py
+-rw-r--r--   0        0        0     6594 2023-04-28 15:49:38.876894 moneykit-0.0.7/moneykit/model/http_validation_error.pyi
+-rw-r--r--   0        0        0     5871 2023-04-28 15:49:38.868027 moneykit-0.0.7/moneykit/model/identity_link_product.py
+-rw-r--r--   0        0        0     5791 2023-04-28 15:49:38.843512 moneykit-0.0.7/moneykit/model/identity_link_product.pyi
+-rw-r--r--   0        0        0     3455 2023-04-28 15:49:38.863639 moneykit-0.0.7/moneykit/model/identity_product_settings.py
+-rw-r--r--   0        0        0     3397 2023-04-28 15:49:38.844520 moneykit-0.0.7/moneykit/model/identity_product_settings.pyi
+-rw-r--r--   0        0        0     4332 2023-04-28 15:49:38.854955 moneykit-0.0.7/moneykit/model/identity_response.py
+-rw-r--r--   0        0        0     4269 2023-04-28 15:49:38.857231 moneykit-0.0.7/moneykit/model/identity_response.pyi
+-rw-r--r--   0        0        0    10361 2023-04-28 15:49:38.876789 moneykit-0.0.7/moneykit/model/institution.py
+-rw-r--r--   0        0        0    10223 2023-04-28 15:49:38.876694 moneykit-0.0.7/moneykit/model/institution.pyi
+-rw-r--r--   0        0        0     5215 2023-04-28 15:49:38.859530 moneykit-0.0.7/moneykit/model/institution_error_not_found_response.py
+-rw-r--r--   0        0        0     4953 2023-04-28 15:49:38.842659 moneykit-0.0.7/moneykit/model/institution_error_not_found_response.pyi
+-rw-r--r--   0        0        0     9656 2023-04-28 15:49:38.866599 moneykit-0.0.7/moneykit/model/institution_styling_response.py
+-rw-r--r--   0        0        0     9489 2023-04-28 15:49:38.870386 moneykit-0.0.7/moneykit/model/institution_styling_response.pyi
+-rw-r--r--   0        0        0     3388 2023-04-28 15:49:38.850598 moneykit-0.0.7/moneykit/model/international_number.py
+-rw-r--r--   0        0        0     3330 2023-04-28 15:49:38.851342 moneykit-0.0.7/moneykit/model/international_number.pyi
+-rw-r--r--   0        0        0     8829 2023-04-28 15:49:38.849859 moneykit-0.0.7/moneykit/model/introspect_client_response.py
+-rw-r--r--   0        0        0     8713 2023-04-28 15:49:38.854953 moneykit-0.0.7/moneykit/model/introspect_client_response.pyi
+-rw-r--r--   0        0        0     3841 2023-04-28 15:49:38.871930 moneykit-0.0.7/moneykit/model/jwk_set.py
+-rw-r--r--   0        0        0     3798 2023-04-28 15:49:38.872251 moneykit-0.0.7/moneykit/model/jwk_set.pyi
+-rw-r--r--   0        0        0    16329 2023-04-28 15:49:38.851937 moneykit-0.0.7/moneykit/model/link_common.py
+-rw-r--r--   0        0        0    16184 2023-04-28 15:49:38.860418 moneykit-0.0.7/moneykit/model/link_common.pyi
+-rw-r--r--   0        0        0     1836 2023-04-28 15:49:38.883224 moneykit-0.0.7/moneykit/model/link_error.py
+-rw-r--r--   0        0        0     1451 2023-04-28 15:49:38.883132 moneykit-0.0.7/moneykit/model/link_error.pyi
+-rw-r--r--   0        0        0     5991 2023-04-28 15:49:38.850815 moneykit-0.0.7/moneykit/model/link_error_bad_state_response.py
+-rw-r--r--   0        0        0     5754 2023-04-28 15:49:38.873482 moneykit-0.0.7/moneykit/model/link_error_bad_state_response.pyi
+-rw-r--r--   0        0        0     5191 2023-04-28 15:49:38.870956 moneykit-0.0.7/moneykit/model/link_error_deleted_response.py
+-rw-r--r--   0        0        0     4947 2023-04-28 15:49:38.871826 moneykit-0.0.7/moneykit/model/link_error_deleted_response.pyi
+-rw-r--r--   0        0        0     5291 2023-04-28 15:49:38.848910 moneykit-0.0.7/moneykit/model/link_error_forbidden_action_response.py
+-rw-r--r--   0        0        0     5030 2023-04-28 15:49:38.844260 moneykit-0.0.7/moneykit/model/link_error_forbidden_action_response.pyi
+-rw-r--r--   0        0        0     5173 2023-04-28 15:49:38.876847 moneykit-0.0.7/moneykit/model/link_error_not_found_response.py
+-rw-r--r--   0        0        0     4925 2023-04-28 15:49:38.867371 moneykit-0.0.7/moneykit/model/link_error_not_found_response.pyi
+-rw-r--r--   0        0        0     5233 2023-04-28 15:49:38.875835 moneykit-0.0.7/moneykit/model/link_error_unauthorized_access_response.py
+-rw-r--r--   0        0        0     4965 2023-04-28 15:49:38.856243 moneykit-0.0.7/moneykit/model/link_error_unauthorized_access_response.pyi
+-rw-r--r--   0        0        0     1461 2023-04-28 15:49:38.857705 moneykit-0.0.7/moneykit/model/link_permission_scope.py
+-rw-r--r--   0        0        0     1229 2023-04-28 15:49:38.849681 moneykit-0.0.7/moneykit/model/link_permission_scope.pyi
+-rw-r--r--   0        0        0     3654 2023-04-28 15:49:38.876008 moneykit-0.0.7/moneykit/model/link_permissions.py
+-rw-r--r--   0        0        0     3610 2023-04-28 15:49:38.849970 moneykit-0.0.7/moneykit/model/link_permissions.pyi
+-rw-r--r--   0        0        0     4930 2023-04-28 15:49:38.869484 moneykit-0.0.7/moneykit/model/link_products.py
+-rw-r--r--   0        0        0     4850 2023-04-28 15:49:38.872673 moneykit-0.0.7/moneykit/model/link_products.pyi
+-rw-r--r--   0        0        0    20792 2023-04-28 15:49:38.865384 moneykit-0.0.7/moneykit/model/link_response.py
+-rw-r--r--   0        0        0    20610 2023-04-28 15:49:38.854193 moneykit-0.0.7/moneykit/model/link_response.pyi
+-rw-r--r--   0        0        0     8548 2023-04-28 15:49:38.864114 moneykit-0.0.7/moneykit/model/link_session_customer_user.py
+-rw-r--r--   0        0        0     8207 2023-04-28 15:49:38.853342 moneykit-0.0.7/moneykit/model/link_session_customer_user.pyi
+-rw-r--r--   0        0        0     4714 2023-04-28 15:49:38.885139 moneykit-0.0.7/moneykit/model/link_session_customer_user_email.py
+-rw-r--r--   0        0        0     4391 2023-04-28 15:49:38.871697 moneykit-0.0.7/moneykit/model/link_session_customer_user_email.pyi
+-rw-r--r--   0        0        0     7373 2023-04-28 15:49:38.875226 moneykit-0.0.7/moneykit/model/link_session_customer_user_phone.py
+-rw-r--r--   0        0        0     7031 2023-04-28 15:49:38.849204 moneykit-0.0.7/moneykit/model/link_session_customer_user_phone.pyi
+-rw-r--r--   0        0        0     5337 2023-04-28 15:49:38.843058 moneykit-0.0.7/moneykit/model/link_session_error_forbidden_config_response.py
+-rw-r--r--   0        0        0     5060 2023-04-28 15:49:38.843869 moneykit-0.0.7/moneykit/model/link_session_error_forbidden_config_response.pyi
+-rw-r--r--   0        0        0     5355 2023-04-28 15:49:38.875143 moneykit-0.0.7/moneykit/model/link_session_error_invalid_token_exchange.py
+-rw-r--r--   0        0        0     5066 2023-04-28 15:49:38.854544 moneykit-0.0.7/moneykit/model/link_session_error_invalid_token_exchange.pyi
+-rw-r--r--   0        0        0    10704 2023-04-28 15:49:38.846163 moneykit-0.0.7/moneykit/model/link_session_setting_overrides.py
+-rw-r--r--   0        0        0    10536 2023-04-28 15:49:38.855581 moneykit-0.0.7/moneykit/model/link_session_setting_overrides.pyi
+-rw-r--r--   0        0        0     1528 2023-04-28 15:49:38.861355 moneykit-0.0.7/moneykit/model/link_state.py
+-rw-r--r--   0        0        0     1253 2023-04-28 15:49:38.855975 moneykit-0.0.7/moneykit/model/link_state.pyi
+-rw-r--r--   0        0        0    11804 2023-04-28 15:49:38.856327 moneykit-0.0.7/moneykit/model/link_state_changed_webhook.py
+-rw-r--r--   0        0        0    11152 2023-04-28 15:49:38.878419 moneykit-0.0.7/moneykit/model/link_state_changed_webhook.pyi
+-rw-r--r--   0        0        0     1124 2023-04-28 15:49:38.869035 moneykit-0.0.7/moneykit/model/money_kit_env.py
+-rw-r--r--   0        0        0      986 2023-04-28 15:49:38.858240 moneykit-0.0.7/moneykit/model/money_kit_env.pyi
+-rw-r--r--   0        0        0     3586 2023-04-28 15:49:38.857825 moneykit-0.0.7/moneykit/model/money_link_features.py
+-rw-r--r--   0        0        0     3542 2023-04-28 15:49:38.883021 moneykit-0.0.7/moneykit/model/money_link_features.pyi
+-rw-r--r--   0        0        0     8201 2023-04-28 15:49:38.845064 moneykit-0.0.7/moneykit/model/owner.py
+-rw-r--r--   0        0        0     8097 2023-04-28 15:49:38.858119 moneykit-0.0.7/moneykit/model/owner.pyi
+-rw-r--r--   0        0        0     6748 2023-04-28 15:49:38.846746 moneykit-0.0.7/moneykit/model/phone_number.py
+-rw-r--r--   0        0        0     6669 2023-04-28 15:49:38.871308 moneykit-0.0.7/moneykit/model/phone_number.pyi
+-rw-r--r--   0        0        0     1308 2023-04-28 15:49:38.845459 moneykit-0.0.7/moneykit/model/phone_number_type.py
+-rw-r--r--   0        0        0     1124 2023-04-28 15:49:38.841992 moneykit-0.0.7/moneykit/model/phone_number_type.pyi
+-rw-r--r--   0        0        0     1419 2023-04-28 15:49:38.857619 moneykit-0.0.7/moneykit/model/product.py
+-rw-r--r--   0        0        0     1187 2023-04-28 15:49:38.864482 moneykit-0.0.7/moneykit/model/product.pyi
+-rw-r--r--   0        0        0    12687 2023-04-28 15:49:38.874512 moneykit-0.0.7/moneykit/model/products_settings.py
+-rw-r--r--   0        0        0    12620 2023-04-28 15:49:38.865258 moneykit-0.0.7/moneykit/model/products_settings.pyi
+-rw-r--r--   0        0        0     1427 2023-04-28 15:49:38.880631 moneykit-0.0.7/moneykit/model/provider.py
+-rw-r--r--   0        0        0     1202 2023-04-28 15:49:38.858896 moneykit-0.0.7/moneykit/model/provider.pyi
+-rw-r--r--   0        0        0     3578 2023-04-28 15:49:38.850552 moneykit-0.0.7/moneykit/model/refresh_products_request.py
+-rw-r--r--   0        0        0     3493 2023-04-28 15:49:38.860318 moneykit-0.0.7/moneykit/model/refresh_products_request.pyi
+-rw-r--r--   0        0        0     6841 2023-04-28 15:49:38.863289 moneykit-0.0.7/moneykit/model/requested_link_permission.py
+-rw-r--r--   0        0        0     6762 2023-04-28 15:49:38.861173 moneykit-0.0.7/moneykit/model/requested_link_permission.pyi
+-rw-r--r--   0        0        0     1029 2023-04-28 15:49:38.868384 moneykit-0.0.7/moneykit/model/supported_version.py
+-rw-r--r--   0        0        0      919 2023-04-28 15:49:38.869762 moneykit-0.0.7/moneykit/model/supported_version.pyi
+-rw-r--r--   0        0        0    12832 2023-04-28 15:49:38.851265 moneykit-0.0.7/moneykit/model/transaction.py
+-rw-r--r--   0        0        0    12654 2023-04-28 15:49:38.874368 moneykit-0.0.7/moneykit/model/transaction.pyi
+-rw-r--r--   0        0        0     6744 2023-04-28 15:49:38.845377 moneykit-0.0.7/moneykit/model/transaction_diff.py
+-rw-r--r--   0        0        0     6660 2023-04-28 15:49:38.852229 moneykit-0.0.7/moneykit/model/transaction_diff.pyi
+-rw-r--r--   0        0        0    12987 2023-04-28 15:49:38.849460 moneykit-0.0.7/moneykit/model/transaction_sync_response.py
+-rw-r--r--   0        0        0    12887 2023-04-28 15:49:38.847540 moneykit-0.0.7/moneykit/model/transaction_sync_response.pyi
+-rw-r--r--   0        0        0     1104 2023-04-28 15:49:38.846444 moneykit-0.0.7/moneykit/model/transaction_type.py
+-rw-r--r--   0        0        0      978 2023-04-28 15:49:38.853683 moneykit-0.0.7/moneykit/model/transaction_type.pyi
+-rw-r--r--   0        0        0     1110 2023-04-28 15:49:38.847003 moneykit-0.0.7/moneykit/model/transaction_type_filter.py
+-rw-r--r--   0        0        0      984 2023-04-28 15:49:38.854148 moneykit-0.0.7/moneykit/model/transaction_type_filter.pyi
+-rw-r--r--   0        0        0     5911 2023-04-28 15:49:38.861215 moneykit-0.0.7/moneykit/model/transactions_link_product.py
+-rw-r--r--   0        0        0     5831 2023-04-28 15:49:38.858462 moneykit-0.0.7/moneykit/model/transactions_link_product.pyi
+-rw-r--r--   0        0        0     4128 2023-04-28 15:49:38.842721 moneykit-0.0.7/moneykit/model/transactions_product_settings.py
+-rw-r--r--   0        0        0     4052 2023-04-28 15:49:38.876650 moneykit-0.0.7/moneykit/model/transactions_product_settings.pyi
+-rw-r--r--   0        0        0     4719 2023-04-28 15:49:38.870730 moneykit-0.0.7/moneykit/model/update_link_request.py
+-rw-r--r--   0        0        0     4584 2023-04-28 15:49:38.880264 moneykit-0.0.7/moneykit/model/update_link_request.pyi
+-rw-r--r--   0        0        0     4612 2023-04-28 15:49:38.842923 moneykit-0.0.7/moneykit/model/user_accounts_out.py
+-rw-r--r--   0        0        0     4568 2023-04-28 15:49:38.843224 moneykit-0.0.7/moneykit/model/user_accounts_out.pyi
+-rw-r--r--   0        0        0     4606 2023-04-28 15:49:38.868095 moneykit-0.0.7/moneykit/model/user_links_out.py
+-rw-r--r--   0        0        0     4562 2023-04-28 15:49:38.846036 moneykit-0.0.7/moneykit/model/user_links_out.pyi
+-rw-r--r--   0        0        0     4704 2023-04-28 15:49:38.875348 moneykit-0.0.7/moneykit/model/user_transactions_paged_response.py
+-rw-r--r--   0        0        0     4660 2023-04-28 15:49:38.858534 moneykit-0.0.7/moneykit/model/user_transactions_paged_response.pyi
+-rw-r--r--   0        0        0     9395 2023-04-28 15:49:38.879410 moneykit-0.0.7/moneykit/model/validation_error.py
+-rw-r--r--   0        0        0     9315 2023-04-28 15:49:38.858855 moneykit-0.0.7/moneykit/model/validation_error.pyi
+-rw-r--r--   0        0        0     6451 2023-04-28 15:49:26.000000 moneykit-0.0.7/moneykit/models/__init__.py
+-rw-r--r--   0        0        0     1257 2023-04-28 15:49:26.000000 moneykit-0.0.7/moneykit/paths/__init__.py
+-rw-r--r--   0        0        0      306 2023-04-28 15:49:37.153985 moneykit-0.0.7/moneykit/paths/auth_introspect/__init__.py
+-rw-r--r--   0        0        0    13677 2023-04-28 15:49:38.865586 moneykit-0.0.7/moneykit/paths/auth_introspect/get.py
+-rw-r--r--   0        0        0    13392 2023-04-28 15:49:38.867277 moneykit-0.0.7/moneykit/paths/auth_introspect/get.pyi
+-rw-r--r--   0        0        0      296 2023-04-28 15:49:37.163270 moneykit-0.0.7/moneykit/paths/auth_token/__init__.py
+-rw-r--r--   0        0        0    17719 2023-04-28 15:49:38.852740 moneykit-0.0.7/moneykit/paths/auth_token/post.py
+-rw-r--r--   0        0        0    17426 2023-04-28 15:49:38.850488 moneykit-0.0.7/moneykit/paths/auth_token/post.pyi
+-rw-r--r--   0        0        0      300 2023-04-28 15:49:37.169646 moneykit-0.0.7/moneykit/paths/institutions/__init__.py
+-rw-r--r--   0        0        0    18697 2023-04-28 15:49:38.885876 moneykit-0.0.7/moneykit/paths/institutions/get.py
+-rw-r--r--   0        0        0    18300 2023-04-28 15:49:38.882833 moneykit-0.0.7/moneykit/paths/institutions/get.pyi
+-rw-r--r--   0        0        0      330 2023-04-28 15:49:37.170621 moneykit-0.0.7/moneykit/paths/institutions_institution_id/__init__.py
+-rw-r--r--   0        0        0    16873 2023-04-28 15:49:38.852041 moneykit-0.0.7/moneykit/paths/institutions_institution_id/get.py
+-rw-r--r--   0        0        0    16522 2023-04-28 15:49:38.843139 moneykit-0.0.7/moneykit/paths/institutions_institution_id/get.pyi
+-rw-r--r--   0        0        0      346 2023-04-28 15:49:37.208566 moneykit-0.0.7/moneykit/paths/institutions_institution_id_styling/__init__.py
+-rw-r--r--   0        0        0    17015 2023-04-28 15:49:38.866013 moneykit-0.0.7/moneykit/paths/institutions_institution_id_styling/get.py
+-rw-r--r--   0        0        0    16664 2023-04-28 15:49:38.868582 moneykit-0.0.7/moneykit/paths/institutions_institution_id_styling/get.pyi
+-rw-r--r--   0        0        0      299 2023-04-28 15:49:37.301033 moneykit-0.0.7/moneykit/paths/link_session/__init__.py
+-rw-r--r--   0        0        0    18397 2023-04-28 15:49:38.886452 moneykit-0.0.7/moneykit/paths/link_session/post.py
+-rw-r--r--   0        0        0    18052 2023-04-28 15:49:38.884474 moneykit-0.0.7/moneykit/paths/link_session/post.pyi
+-rw-r--r--   0        0        0      328 2023-04-28 15:49:37.308010 moneykit-0.0.7/moneykit/paths/link_session_exchange_token/__init__.py
+-rw-r--r--   0        0        0    18303 2023-04-28 15:49:38.882747 moneykit-0.0.7/moneykit/paths/link_session_exchange_token/post.py
+-rw-r--r--   0        0        0    17958 2023-04-28 15:49:38.873765 moneykit-0.0.7/moneykit/paths/link_session_exchange_token/post.pyi
+-rw-r--r--   0        0        0      292 2023-04-28 15:49:37.319367 moneykit-0.0.7/moneykit/paths/links_id/__init__.py
+-rw-r--r--   0        0        0    18419 2023-04-28 15:49:38.888536 moneykit-0.0.7/moneykit/paths/links_id/delete.py
+-rw-r--r--   0        0        0    17972 2023-04-28 15:49:38.882442 moneykit-0.0.7/moneykit/paths/links_id/delete.pyi
+-rw-r--r--   0        0        0    18631 2023-04-28 15:49:38.891122 moneykit-0.0.7/moneykit/paths/links_id/get.py
+-rw-r--r--   0        0        0    18184 2023-04-28 15:49:38.889189 moneykit-0.0.7/moneykit/paths/links_id/get.pyi
+-rw-r--r--   0        0        0    22888 2023-04-28 15:49:38.882591 moneykit-0.0.7/moneykit/paths/links_id/patch.py
+-rw-r--r--   0        0        0    22413 2023-04-28 15:49:38.880161 moneykit-0.0.7/moneykit/paths/links_id/patch.pyi
+-rw-r--r--   0        0        0      310 2023-04-28 15:49:37.463337 moneykit-0.0.7/moneykit/paths/links_id_accounts/__init__.py
+-rw-r--r--   0        0        0    21397 2023-04-28 15:49:38.867908 moneykit-0.0.7/moneykit/paths/links_id_accounts/get.py
+-rw-r--r--   0        0        0    20945 2023-04-28 15:49:38.864457 moneykit-0.0.7/moneykit/paths/links_id_accounts/get.pyi
+-rw-r--r--   0        0        0      332 2023-04-28 15:49:37.473607 moneykit-0.0.7/moneykit/paths/links_id_accounts_account_id/__init__.py
+-rw-r--r--   0        0        0    19061 2023-04-28 15:49:38.889317 moneykit-0.0.7/moneykit/paths/links_id_accounts_account_id/get.py
+-rw-r--r--   0        0        0    18614 2023-04-28 15:49:38.891563 moneykit-0.0.7/moneykit/paths/links_id_accounts_account_id/get.pyi
+-rw-r--r--   0        0        0      326 2023-04-28 15:49:37.487732 moneykit-0.0.7/moneykit/paths/links_id_accounts_numbers/__init__.py
+-rw-r--r--   0        0        0    18809 2023-04-28 15:49:38.887292 moneykit-0.0.7/moneykit/paths/links_id_accounts_numbers/get.py
+-rw-r--r--   0        0        0    18362 2023-04-28 15:49:38.890608 moneykit-0.0.7/moneykit/paths/links_id_accounts_numbers/get.pyi
+-rw-r--r--   0        0        0      310 2023-04-28 15:49:37.522917 moneykit-0.0.7/moneykit/paths/links_id_identity/__init__.py
+-rw-r--r--   0        0        0    21409 2023-04-28 15:49:38.887197 moneykit-0.0.7/moneykit/paths/links_id_identity/get.py
+-rw-r--r--   0        0        0    20957 2023-04-28 15:49:38.888401 moneykit-0.0.7/moneykit/paths/links_id_identity/get.pyi
+-rw-r--r--   0        0        0      310 2023-04-28 15:49:37.601093 moneykit-0.0.7/moneykit/paths/links_id_products/__init__.py
+-rw-r--r--   0        0        0    22935 2023-04-28 15:49:38.874500 moneykit-0.0.7/moneykit/paths/links_id_products/post.py
+-rw-r--r--   0        0        0    22460 2023-04-28 15:49:38.871628 moneykit-0.0.7/moneykit/paths/links_id_products/post.pyi
+-rw-r--r--   0        0        0      318 2023-04-28 15:49:37.657793 moneykit-0.0.7/moneykit/paths/links_id_transactions/__init__.py
+-rw-r--r--   0        0        0    23741 2023-04-28 15:49:38.847785 moneykit-0.0.7/moneykit/paths/links_id_transactions/get.py
+-rw-r--r--   0        0        0    23171 2023-04-28 15:49:38.854642 moneykit-0.0.7/moneykit/paths/links_id_transactions/get.pyi
+-rw-r--r--   0        0        0      328 2023-04-28 15:49:37.667606 moneykit-0.0.7/moneykit/paths/links_id_transactions_sync/__init__.py
+-rw-r--r--   0        0        0    21818 2023-04-28 15:49:38.860572 moneykit-0.0.7/moneykit/paths/links_id_transactions_sync/get.py
+-rw-r--r--   0        0        0    21293 2023-04-28 15:49:38.863297 moneykit-0.0.7/moneykit/paths/links_id_transactions_sync/get.pyi
+-rw-r--r--   0        0        0      310 2023-04-28 15:49:37.680528 moneykit-0.0.7/moneykit/paths/users_id_accounts/__init__.py
+-rw-r--r--   0        0        0    19316 2023-04-28 15:49:38.855071 moneykit-0.0.7/moneykit/paths/users_id_accounts/get.py
+-rw-r--r--   0        0        0    18938 2023-04-28 15:49:38.857945 moneykit-0.0.7/moneykit/paths/users_id_accounts/get.pyi
+-rw-r--r--   0        0        0      304 2023-04-28 15:49:37.700391 moneykit-0.0.7/moneykit/paths/users_id_links/__init__.py
+-rw-r--r--   0        0        0    15565 2023-04-28 15:49:38.845558 moneykit-0.0.7/moneykit/paths/users_id_links/get.py
+-rw-r--r--   0        0        0    15278 2023-04-28 15:49:38.847691 moneykit-0.0.7/moneykit/paths/users_id_links/get.pyi
+-rw-r--r--   0        0        0      318 2023-04-28 15:49:37.793076 moneykit-0.0.7/moneykit/paths/users_id_transactions/__init__.py
+-rw-r--r--   0        0        0    23515 2023-04-28 15:49:38.888644 moneykit-0.0.7/moneykit/paths/users_id_transactions/get.py
+-rw-r--r--   0        0        0    23015 2023-04-28 15:49:38.891074 moneykit-0.0.7/moneykit/paths/users_id_transactions/get.pyi
+-rw-r--r--   0        0        0      316 2023-04-28 15:49:37.853638 moneykit-0.0.7/moneykit/paths/well_known_jwks_json/__init__.py
+-rw-r--r--   0        0        0    13631 2023-04-28 15:49:38.877467 moneykit-0.0.7/moneykit/paths/well_known_jwks_json/get.py
+-rw-r--r--   0        0        0    13346 2023-04-28 15:49:38.884801 moneykit-0.0.7/moneykit/paths/well_known_jwks_json/get.pyi
+-rw-r--r--   0        0        0      963 2023-04-28 15:49:59.318396 moneykit-0.0.7/moneykit/plaid_compatible/__init__.py
+-rw-r--r--   0        0        0      227 2023-04-28 15:49:59.350279 moneykit-0.0.7/moneykit/plaid_compatible/api/__init__.py
+-rw-r--r--   0        0        0    50030 2023-04-28 15:49:59.351005 moneykit-0.0.7/moneykit/plaid_compatible/api/plaid_api.py
+-rw-r--r--   0        0        0    36839 2023-04-28 15:49:59.351886 moneykit-0.0.7/moneykit/plaid_compatible/api_client.py
+-rw-r--r--   0        0        0      470 2023-04-28 15:49:59.317734 moneykit-0.0.7/moneykit/plaid_compatible/apis/__init__.py
+-rw-r--r--   0        0        0    17735 2023-04-28 15:49:59.317518 moneykit-0.0.7/moneykit/plaid_compatible/configuration.py
+-rw-r--r--   0        0        0     5093 2023-04-28 15:49:59.351255 moneykit-0.0.7/moneykit/plaid_compatible/exceptions.py
+-rw-r--r--   0        0        0      348 2023-04-28 15:49:59.330811 moneykit-0.0.7/moneykit/plaid_compatible/model/__init__.py
+-rw-r--r--   0        0        0    10890 2023-04-28 15:49:59.337329 moneykit-0.0.7/moneykit/plaid_compatible/model/account_balance.py
+-rw-r--r--   0        0        0    10741 2023-04-28 15:49:59.333928 moneykit-0.0.7/moneykit/plaid_compatible/model/account_base.py
+-rw-r--r--   0        0        0    11657 2023-04-28 15:49:59.327765 moneykit-0.0.7/moneykit/plaid_compatible/model/account_identity.py
+-rw-r--r--   0        0        0    11414 2023-04-28 15:49:59.333260 moneykit-0.0.7/moneykit/plaid_compatible/model/account_subtype.py
+-rw-r--r--   0        0        0     7191 2023-04-28 15:49:59.347039 moneykit-0.0.7/moneykit/plaid_compatible/model/account_type.py
+-rw-r--r--   0        0        0     7674 2023-04-28 15:49:59.334337 moneykit-0.0.7/moneykit/plaid_compatible/model/accounts_get_request.py
+-rw-r--r--   0        0        0     6636 2023-04-28 15:49:59.344492 moneykit-0.0.7/moneykit/plaid_compatible/model/accounts_get_request_options.py
+-rw-r--r--   0        0        0     7447 2023-04-28 15:49:59.341074 moneykit-0.0.7/moneykit/plaid_compatible/model/accounts_get_response.py
+-rw-r--r--   0        0        0     6925 2023-04-28 15:49:59.320449 moneykit-0.0.7/moneykit/plaid_compatible/model/address.py
+-rw-r--r--   0        0        0     7501 2023-04-28 15:49:59.335694 moneykit-0.0.7/moneykit/plaid_compatible/model/address_data.py
+-rw-r--r--   0        0        0     7793 2023-04-28 15:49:59.344759 moneykit-0.0.7/moneykit/plaid_compatible/model/auth_get_numbers.py
+-rw-r--r--   0        0        0     7642 2023-04-28 15:49:59.343685 moneykit-0.0.7/moneykit/plaid_compatible/model/auth_get_request.py
+-rw-r--r--   0        0        0     6715 2023-04-28 15:49:59.333544 moneykit-0.0.7/moneykit/plaid_compatible/model/auth_get_request_options.py
+-rw-r--r--   0        0        0     7635 2023-04-28 15:49:59.349189 moneykit-0.0.7/moneykit/plaid_compatible/model/auth_get_response.py
+-rw-r--r--   0        0        0     7265 2023-04-28 15:49:59.322721 moneykit-0.0.7/moneykit/plaid_compatible/model/counterparty_type.py
+-rw-r--r--   0        0        0     6955 2023-04-28 15:49:59.345038 moneykit-0.0.7/moneykit/plaid_compatible/model/country_code.py
+-rw-r--r--   0        0        0     7029 2023-04-28 15:49:59.323051 moneykit-0.0.7/moneykit/plaid_compatible/model/credit_account_subtype.py
+-rw-r--r--   0        0        0     7070 2023-04-28 15:49:59.319828 moneykit-0.0.7/moneykit/plaid_compatible/model/credit_filter.py
+-rw-r--r--   0        0        0     7417 2023-04-28 15:49:59.342488 moneykit-0.0.7/moneykit/plaid_compatible/model/depository_account_subtype.py
+-rw-r--r--   0        0        0     7102 2023-04-28 15:49:59.343964 moneykit-0.0.7/moneykit/plaid_compatible/model/depository_filter.py
+-rw-r--r--   0        0        0     6966 2023-04-28 15:49:59.339302 moneykit-0.0.7/moneykit/plaid_compatible/model/email.py
+-rw-r--r--   0        0        0     6965 2023-04-28 15:49:59.349446 moneykit-0.0.7/moneykit/plaid_compatible/model/employment_source_type.py
+-rw-r--r--   0        0        0     6724 2023-04-28 15:49:59.335399 moneykit-0.0.7/moneykit/plaid_compatible/model/http_validation_error.py
+-rw-r--r--   0        0        0     9101 2023-04-28 15:49:59.339599 moneykit-0.0.7/moneykit/plaid_compatible/model/id_number_type.py
+-rw-r--r--   0        0        0     7674 2023-04-28 15:49:59.341343 moneykit-0.0.7/moneykit/plaid_compatible/model/identity_get_request.py
+-rw-r--r--   0        0        0     6723 2023-04-28 15:49:59.342215 moneykit-0.0.7/moneykit/plaid_compatible/model/identity_get_request_options.py
+-rw-r--r--   0        0        0     7362 2023-04-28 15:49:59.340156 moneykit-0.0.7/moneykit/plaid_compatible/model/identity_get_response.py
+-rw-r--r--   0        0        0     7111 2023-04-28 15:49:59.322049 moneykit-0.0.7/moneykit/plaid_compatible/model/income_verification_payroll_flow_type.py
+-rw-r--r--   0        0        0     6981 2023-04-28 15:49:59.324609 moneykit-0.0.7/moneykit/plaid_compatible/model/income_verification_source_type.py
+-rw-r--r--   0        0        0     9913 2023-04-28 15:49:59.347379 moneykit-0.0.7/moneykit/plaid_compatible/model/investment_account_subtype.py
+-rw-r--r--   0        0        0     7102 2023-04-28 15:49:59.336640 moneykit-0.0.7/moneykit/plaid_compatible/model/investment_filter.py
+-rw-r--r--   0        0        0    10420 2023-04-28 15:49:59.348916 moneykit-0.0.7/moneykit/plaid_compatible/model/item.py
+-rw-r--r--   0        0        0     7717 2023-04-28 15:49:59.334681 moneykit-0.0.7/moneykit/plaid_compatible/model/item_error_webhook.py
+-rw-r--r--   0        0        0     7265 2023-04-28 15:49:59.338969 moneykit-0.0.7/moneykit/plaid_compatible/model/item_get_request.py
+-rw-r--r--   0        0        0     7287 2023-04-28 15:49:59.321738 moneykit-0.0.7/moneykit/plaid_compatible/model/item_get_response.py
+-rw-r--r--   0        0        0     7331 2023-04-28 15:49:59.339889 moneykit-0.0.7/moneykit/plaid_compatible/model/item_public_token_exchange_request.py
+-rw-r--r--   0        0        0     7235 2023-04-28 15:49:59.349724 moneykit-0.0.7/moneykit/plaid_compatible/model/item_public_token_exchange_response.py
+-rw-r--r--   0        0        0     7271 2023-04-28 15:49:59.323736 moneykit-0.0.7/moneykit/plaid_compatible/model/item_remove_request.py
+-rw-r--r--   0        0        0     6715 2023-04-28 15:49:59.345931 moneykit-0.0.7/moneykit/plaid_compatible/model/item_remove_response.py
+-rw-r--r--   0        0        0     7362 2023-04-28 15:49:59.344235 moneykit-0.0.7/moneykit/plaid_compatible/model/item_status_investments.py
+-rw-r--r--   0        0        0     6852 2023-04-28 15:49:59.336334 moneykit-0.0.7/moneykit/plaid_compatible/model/item_status_last_webhook.py
+-rw-r--r--   0        0        0     7489 2023-04-28 15:49:59.342780 moneykit-0.0.7/moneykit/plaid_compatible/model/item_status_nullable.py
+-rw-r--r--   0        0        0     7366 2023-04-28 15:49:59.326197 moneykit-0.0.7/moneykit/plaid_compatible/model/item_status_transactions.py
+-rw-r--r--   0        0        0     7595 2023-04-28 15:49:59.347690 moneykit-0.0.7/moneykit/plaid_compatible/model/link_token_account_filters.py
+-rw-r--r--   0        0        0     6644 2023-04-28 15:49:59.332898 moneykit-0.0.7/moneykit/plaid_compatible/model/link_token_create_institution_data.py
+-rw-r--r--   0        0        0    21548 2023-04-28 15:49:59.346385 moneykit-0.0.7/moneykit/plaid_compatible/model/link_token_create_request.py
+-rw-r--r--   0        0        0     8258 2023-04-28 15:49:59.321400 moneykit-0.0.7/moneykit/plaid_compatible/model/link_token_create_request_auth.py
+-rw-r--r--   0        0        0     6733 2023-04-28 15:49:59.327345 moneykit-0.0.7/moneykit/plaid_compatible/model/link_token_create_request_deposit_switch.py
+-rw-r--r--   0        0        0     7534 2023-04-28 15:49:59.328059 moneykit-0.0.7/moneykit/plaid_compatible/model/link_token_create_request_employment.py
+-rw-r--r--   0        0        0     6722 2023-04-28 15:49:59.330230 moneykit-0.0.7/moneykit/plaid_compatible/model/link_token_create_request_employment_bank_income.py
+-rw-r--r--   0        0        0     7661 2023-04-28 15:49:59.338157 moneykit-0.0.7/moneykit/plaid_compatible/model/link_token_create_request_identity_verification.py
+-rw-r--r--   0        0        0    10586 2023-04-28 15:49:59.345389 moneykit-0.0.7/moneykit/plaid_compatible/model/link_token_create_request_income_verification.py
+-rw-r--r--   0        0        0     7020 2023-04-28 15:49:59.318959 moneykit-0.0.7/moneykit/plaid_compatible/model/link_token_create_request_income_verification_bank_income.py
+-rw-r--r--   0        0        0     7697 2023-04-28 15:49:59.328785 moneykit-0.0.7/moneykit/plaid_compatible/model/link_token_create_request_income_verification_payroll_income.py
+-rw-r--r--   0        0        0     6937 2023-04-28 15:49:59.319512 moneykit-0.0.7/moneykit/plaid_compatible/model/link_token_create_request_payment_initiation.py
+-rw-r--r--   0        0        0     6940 2023-04-28 15:49:59.336937 moneykit-0.0.7/moneykit/plaid_compatible/model/link_token_create_request_transfer.py
+-rw-r--r--   0        0        0     6779 2023-04-28 15:49:59.325850 moneykit-0.0.7/moneykit/plaid_compatible/model/link_token_create_request_update.py
+-rw-r--r--   0        0        0    11399 2023-04-28 15:49:59.320177 moneykit-0.0.7/moneykit/plaid_compatible/model/link_token_create_request_user.py
+-rw-r--r--   0        0        0     6963 2023-04-28 15:49:59.347994 moneykit-0.0.7/moneykit/plaid_compatible/model/link_token_create_request_user_name.py
+-rw-r--r--   0        0        0     8414 2023-04-28 15:49:59.325504 moneykit-0.0.7/moneykit/plaid_compatible/model/link_token_create_request_user_stated_income_source.py
+-rw-r--r--   0        0        0     7615 2023-04-28 15:49:59.329111 moneykit-0.0.7/moneykit/plaid_compatible/model/link_token_create_response.py
+-rw-r--r--   0        0        0     6616 2023-04-28 15:49:59.341936 moneykit-0.0.7/moneykit/plaid_compatible/model/link_token_eu_config.py
+-rw-r--r--   0        0        0     6769 2023-04-28 15:49:59.348583 moneykit-0.0.7/moneykit/plaid_compatible/model/link_token_investments.py
+-rw-r--r--   0        0        0     7573 2023-04-28 15:49:59.328430 moneykit-0.0.7/moneykit/plaid_compatible/model/loan_account_subtype.py
+-rw-r--r--   0        0        0     7054 2023-04-28 15:49:59.331999 moneykit-0.0.7/moneykit/plaid_compatible/model/loan_filter.py
+-rw-r--r--   0        0        0     7487 2023-04-28 15:49:59.336046 moneykit-0.0.7/moneykit/plaid_compatible/model/location.py
+-rw-r--r--   0        0        0     7716 2023-04-28 15:49:59.331379 moneykit-0.0.7/moneykit/plaid_compatible/model/money_link_features.py
+-rw-r--r--   0        0        0     8621 2023-04-28 15:49:59.345671 moneykit-0.0.7/moneykit/plaid_compatible/model/numbers_ach.py
+-rw-r--r--   0        0        0     7019 2023-04-28 15:49:59.324879 moneykit-0.0.7/moneykit/plaid_compatible/model/numbers_bacs.py
+-rw-r--r--   0        0        0     7225 2023-04-28 15:49:59.330536 moneykit-0.0.7/moneykit/plaid_compatible/model/numbers_eft.py
+-rw-r--r--   0        0        0     7007 2023-04-28 15:49:59.335068 moneykit-0.0.7/moneykit/plaid_compatible/model/numbers_international.py
+-rw-r--r--   0        0        0     8304 2023-04-28 15:49:59.332305 moneykit-0.0.7/moneykit/plaid_compatible/model/owner.py
+-rw-r--r--   0        0        0     7593 2023-04-28 15:49:59.319238 moneykit-0.0.7/moneykit/plaid_compatible/model/payment_meta.py
+-rw-r--r--   0        0        0     6930 2023-04-28 15:49:59.323415 moneykit-0.0.7/moneykit/plaid_compatible/model/personal_finance_category.py
+-rw-r--r--   0        0        0     6934 2023-04-28 15:49:59.329602 moneykit-0.0.7/moneykit/plaid_compatible/model/phone_number.py
+-rw-r--r--   0        0        0     9494 2023-04-28 15:49:59.350079 moneykit-0.0.7/moneykit/plaid_compatible/model/plaid_error.py
+-rw-r--r--   0        0        0     8113 2023-04-28 15:49:59.320767 moneykit-0.0.7/moneykit/plaid_compatible/model/plaid_error_type.py
+-rw-r--r--   0        0        0     7129 2023-04-28 15:49:59.331095 moneykit-0.0.7/moneykit/plaid_compatible/model/products.py
+-rw-r--r--   0        0        0     6610 2023-04-28 15:49:59.321063 moneykit-0.0.7/moneykit/plaid_compatible/model/removed_transaction.py
+-rw-r--r--   0        0        0    16756 2023-04-28 15:49:59.326595 moneykit-0.0.7/moneykit/plaid_compatible/model/transaction.py
+-rw-r--r--   0        0        0     7632 2023-04-28 15:49:59.331653 moneykit-0.0.7/moneykit/plaid_compatible/model/transaction_code.py
+-rw-r--r--   0        0        0     7510 2023-04-28 15:49:59.324333 moneykit-0.0.7/moneykit/plaid_compatible/model/transaction_counterparty.py
+-rw-r--r--   0        0        0     8236 2023-04-28 15:49:59.340437 moneykit-0.0.7/moneykit/plaid_compatible/model/transactions_get_request.py
+-rw-r--r--   0        0        0     9639 2023-04-28 15:49:59.337764 moneykit-0.0.7/moneykit/plaid_compatible/model/transactions_get_request_options.py
+-rw-r--r--   0        0        0     8530 2023-04-28 15:49:59.343129 moneykit-0.0.7/moneykit/plaid_compatible/model/transactions_get_response.py
+-rw-r--r--   0        0        0     7289 2023-04-28 15:49:59.348310 moneykit-0.0.7/moneykit/plaid_compatible/model/transactions_refresh_request.py
+-rw-r--r--   0        0        0     6733 2023-04-28 15:49:59.322394 moneykit-0.0.7/moneykit/plaid_compatible/model/transactions_refresh_response.py
+-rw-r--r--   0        0        0     8397 2023-04-28 15:49:59.340744 moneykit-0.0.7/moneykit/plaid_compatible/model/transactions_sync_request.py
+-rw-r--r--   0        0        0     8427 2023-04-28 15:49:59.343412 moneykit-0.0.7/moneykit/plaid_compatible/model/transactions_sync_request_options.py
+-rw-r--r--   0        0        0     8900 2023-04-28 15:49:59.332610 moneykit-0.0.7/moneykit/plaid_compatible/model/transactions_sync_response.py
+-rw-r--r--   0        0        0     7916 2023-04-28 15:49:59.338542 moneykit-0.0.7/moneykit/plaid_compatible/model/user_address.py
+-rw-r--r--   0        0        0     6950 2023-04-28 15:49:59.341621 moneykit-0.0.7/moneykit/plaid_compatible/model/user_id_number.py
+-rw-r--r--   0        0        0     7625 2023-04-28 15:49:59.346736 moneykit-0.0.7/moneykit/plaid_compatible/model/user_stated_income_source_category.py
+-rw-r--r--   0        0        0     7187 2023-04-28 15:49:59.325182 moneykit-0.0.7/moneykit/plaid_compatible/model/user_stated_income_source_frequency.py
+-rw-r--r--   0        0        0     7027 2023-04-28 15:49:59.329940 moneykit-0.0.7/moneykit/plaid_compatible/model/user_stated_income_source_pay_type.py
+-rw-r--r--   0        0        0     6793 2023-04-28 15:49:59.324040 moneykit-0.0.7/moneykit/plaid_compatible/model/validation_error.py
+-rw-r--r--   0        0        0     7069 2023-04-28 15:49:59.326993 moneykit-0.0.7/moneykit/plaid_compatible/model/webhook_environment_values.py
+-rw-r--r--   0        0        0    74795 2023-04-28 15:49:59.317075 moneykit-0.0.7/moneykit/plaid_compatible/model_utils.py
+-rw-r--r--   0        0        0     8892 2023-04-28 15:49:59.318683 moneykit-0.0.7/moneykit/plaid_compatible/models/__init__.py
+-rw-r--r--   0        0        0    12537 2023-04-28 15:49:59.318033 moneykit-0.0.7/moneykit/plaid_compatible/rest.py
+-rw-r--r--   0        0        0     9365 2023-04-28 15:49:38.880398 moneykit-0.0.7/moneykit/rest.py
+-rw-r--r--   0        0        0    99126 2023-04-28 15:49:38.877828 moneykit-0.0.7/moneykit/schemas.py
+-rw-r--r--   0        0        0      935 2023-04-28 15:51:49.449775 moneykit-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0    21113 1970-01-01 00:00:00.000000 moneykit-0.0.7/PKG-INFO
```

### Comparing `moneykit-0.0.6/moneykit/api/access_token_api.py` & `moneykit-0.0.7/moneykit/paths/users_id_transactions/get.pyi`

 * *Files 27% similar despite different names*

```diff
@@ -1,527 +1,669 @@
 # coding: utf-8
 
 """
-    MoneyKit API
 
-    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.0
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
+    Generated by: https://openapi-generator.tech
 """
 
-
+import decimal  # noqa: F401
+import functools  # noqa: F401
+import io  # noqa: F401
 import re  # noqa: F401
-from typing import Any, Dict, Optional
-
-from pydantic import Field, StrictStr, constr, validate_arguments
-from typing_extensions import Annotated
-
-from moneykit.api_client import ApiClient
-from moneykit.exceptions import ApiTypeError, ApiValueError  # noqa: F401
-from moneykit.models.api_client_out import APIClientOut
-from moneykit.models.jwk_set import JWKSet
-from moneykit.models.token import Token
-
-
-class AccessTokenApi(object):
-    """NOTE: This class is auto generated by OpenAPI Generator
-    Ref: https://openapi-generator.tech
-
-    Do not edit the class manually.
-    """
-
-    def __init__(self, api_client=None):
-        if api_client is None:
-            api_client = ApiClient.get_default()
-        self.api_client = api_client
-
-    @validate_arguments
-    def generate_access_token(
-        self,
-        moneykit_version: Optional[Dict[str, Any]] = None,
-        grant_type: Annotated[
-            Optional[constr(strict=True)], Field(description="Token grant type. Only `client_credentials` supported.")
-        ] = None,
-        scope: Annotated[
-            Optional[StrictStr],
-            Field(
-                description="Actions to be allowed for this token, given as one or more strings separated by spaces.             If omitted, all actions allowed for your application will be granted to this token."
-            ),
-        ] = None,
-        client_id: Annotated[Optional[StrictStr], Field(description="Your application's MoneyKit client ID.")] = None,
-        client_secret: Annotated[
-            Optional[StrictStr], Field(description="Your application's MoneyKit client secret.")
-        ] = None,
-        **kwargs,
-    ) -> Token:  # noqa: E501
-        """/auth/token  # noqa: E501
-
-        Create a new short-lived access token by validating your `client_id` and `client_secret`.  The `access_token` is to be forwarded with all subsequent requests as `Authorization: Bearer {access_token}` HTTP header.  When the token expires you must regenerate your `access_token`.  The `client_id` and `client_secret` can be supplied as POST body parameters, or as a HTTP basic auth header.  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.generate_access_token(moneykit_version, grant_type, scope, client_id, client_secret, async_req=True)
-        >>> result = thread.get()
-
-        :param moneykit_version:
-        :type moneykit_version: SupportedVersion
-        :param grant_type: Token grant type. Only `client_credentials` supported.
-        :type grant_type: str
-        :param scope: Actions to be allowed for this token, given as one or more strings separated by spaces.             If omitted, all actions allowed for your application will be granted to this token.
-        :type scope: str
-        :param client_id: Your application's MoneyKit client ID.
-        :type client_id: str
-        :param client_secret: Your application's MoneyKit client secret.
-        :type client_secret: str
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: Token
-        """
-        kwargs["_return_http_data_only"] = True
-        return self.generate_access_token_with_http_info(
-            moneykit_version, grant_type, scope, client_id, client_secret, **kwargs
-        )  # noqa: E501
-
-    @validate_arguments
-    def generate_access_token_with_http_info(
-        self,
-        moneykit_version: Optional[Dict[str, Any]] = None,
-        grant_type: Annotated[
-            Optional[constr(strict=True)], Field(description="Token grant type. Only `client_credentials` supported.")
-        ] = None,
-        scope: Annotated[
-            Optional[StrictStr],
-            Field(
-                description="Actions to be allowed for this token, given as one or more strings separated by spaces.             If omitted, all actions allowed for your application will be granted to this token."
-            ),
-        ] = None,
-        client_id: Annotated[Optional[StrictStr], Field(description="Your application's MoneyKit client ID.")] = None,
-        client_secret: Annotated[
-            Optional[StrictStr], Field(description="Your application's MoneyKit client secret.")
-        ] = None,
-        **kwargs,
-    ):  # noqa: E501
-        """/auth/token  # noqa: E501
-
-        Create a new short-lived access token by validating your `client_id` and `client_secret`.  The `access_token` is to be forwarded with all subsequent requests as `Authorization: Bearer {access_token}` HTTP header.  When the token expires you must regenerate your `access_token`.  The `client_id` and `client_secret` can be supplied as POST body parameters, or as a HTTP basic auth header.  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.generate_access_token_with_http_info(moneykit_version, grant_type, scope, client_id, client_secret, async_req=True)
-        >>> result = thread.get()
-
-        :param moneykit_version:
-        :type moneykit_version: SupportedVersion
-        :param grant_type: Token grant type. Only `client_credentials` supported.
-        :type grant_type: str
-        :param scope: Actions to be allowed for this token, given as one or more strings separated by spaces.             If omitted, all actions allowed for your application will be granted to this token.
-        :type scope: str
-        :param client_id: Your application's MoneyKit client ID.
-        :type client_id: str
-        :param client_secret: Your application's MoneyKit client secret.
-        :type client_secret: str
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the authentication
-                              in the spec for a single request.
-        :type _request_auth: dict, optional
-        :type _content_type: string, optional: force content-type for the request
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: tuple(Token, status_code(int), headers(HTTPHeaderDict))
-        """
-
-        _params = locals()
+import typing  # noqa: F401
+import uuid  # noqa: F401
+from dataclasses import dataclass
+from datetime import date, datetime  # noqa: F401
+
+import frozendict  # noqa: F401
+import typing_extensions  # noqa: F401
+import urllib3
+from urllib3._collections import HTTPHeaderDict
+
+from moneykit import (
+    api_client,
+    exceptions,
+    schemas,  # noqa: F401
+)
+from moneykit.model.api_error_auth_expired_access_token_response import APIErrorAuthExpiredAccessTokenResponse
+from moneykit.model.api_error_auth_unauthorized_response import APIErrorAuthUnauthorizedResponse
+from moneykit.model.get_user_transactions_response import GetUserTransactionsResponse
+from moneykit.model.supported_version import SupportedVersion
+from moneykit.model.transaction_type_filter import TransactionTypeFilter
+
+# Query params
+
+class TransactionTypeSchema(schemas.ListBase, schemas.NoneBase, schemas.Schema, schemas.NoneTupleMixin):
+    class MetaOapg:
+        @staticmethod
+        def items() -> typing.Type["TransactionTypeFilter"]:
+            return TransactionTypeFilter
+    def __new__(
+        cls,
+        *_args: typing.Union[
+            list,
+            tuple,
+            None,
+        ],
+        _configuration: typing.Optional[schemas.Configuration] = None,
+    ) -> "TransactionTypeSchema":
+        return super().__new__(
+            cls,
+            *_args,
+            _configuration=_configuration,
+        )
 
-        _all_params = ["moneykit_version", "grant_type", "scope", "client_id", "client_secret"]
-        _all_params.extend(
-            [
-                "async_req",
-                "_return_http_data_only",
-                "_preload_content",
-                "_request_timeout",
-                "_request_auth",
-                "_content_type",
-                "_headers",
-            ]
+class CategorySchema(schemas.ListBase, schemas.NoneBase, schemas.Schema, schemas.NoneTupleMixin):
+    class MetaOapg:
+        items = schemas.StrSchema
+    def __new__(
+        cls,
+        *_args: typing.Union[
+            list,
+            tuple,
+            None,
+        ],
+        _configuration: typing.Optional[schemas.Configuration] = None,
+    ) -> "CategorySchema":
+        return super().__new__(
+            cls,
+            *_args,
+            _configuration=_configuration,
         )
 
-        # validate the arguments
-        for _key, _val in _params["kwargs"].items():
-            if _key not in _all_params:
-                raise ApiTypeError("Got an unexpected keyword argument '%s'" " to method generate_access_token" % _key)
-            _params[_key] = _val
-        del _params["kwargs"]
+class AccountIdSchema(schemas.ListBase, schemas.NoneBase, schemas.Schema, schemas.NoneTupleMixin):
+    class MetaOapg:
+        class items(schemas.StrSchema):
+            pass
+    def __new__(
+        cls,
+        *_args: typing.Union[
+            list,
+            tuple,
+            None,
+        ],
+        _configuration: typing.Optional[schemas.Configuration] = None,
+    ) -> "AccountIdSchema":
+        return super().__new__(
+            cls,
+            *_args,
+            _configuration=_configuration,
+        )
 
-        _collection_formats = {}
+class InstitutionIdSchema(schemas.ListBase, schemas.NoneBase, schemas.Schema, schemas.NoneTupleMixin):
+    class MetaOapg:
+        class items(schemas.StrSchema):
+            pass
+    def __new__(
+        cls,
+        *_args: typing.Union[
+            list,
+            tuple,
+            None,
+        ],
+        _configuration: typing.Optional[schemas.Configuration] = None,
+    ) -> "InstitutionIdSchema":
+        return super().__new__(
+            cls,
+            *_args,
+            _configuration=_configuration,
+        )
 
-        # process the path parameters
-        _path_params = {}
+class PageSchema(schemas.IntSchema):
+    pass
 
-        # process the query parameters
-        _query_params = []
-        # process the header parameters
-        _header_params = dict(_params.get("_headers", {}))
-        if _params["moneykit_version"]:
-            _header_params["moneykit-version"] = _params["moneykit_version"]
-
-        # process the form parameters
-        _form_params = []
-        _files = {}
-        if _params["grant_type"]:
-            _form_params.append(("grant_type", _params["grant_type"]))
-
-        if _params["scope"]:
-            _form_params.append(("scope", _params["scope"]))
-
-        if _params["client_id"]:
-            _form_params.append(("client_id", _params["client_id"]))
-
-        if _params["client_secret"]:
-            _form_params.append(("client_secret", _params["client_secret"]))
-
-        # process the body parameter
-        _body_params = None
-        # set the HTTP header `Accept`
-        _header_params["Accept"] = self.api_client.select_header_accept(["application/json"])  # noqa: E501
-
-        # set the HTTP header `Content-Type`
-        _content_types_list = _params.get(
-            "_content_type", self.api_client.select_header_content_type(["application/x-www-form-urlencoded"])
-        )
-        if _content_types_list:
-            _header_params["Content-Type"] = _content_types_list
-
-        # authentication setting
-        _auth_settings = ["HTTPBasic"]  # noqa: E501
-
-        _response_types_map = {
-            "201": "Token",
-            "400": "APIErrorAuthUnauthorizedResponse",
-            "401": "APIErrorAuthUnauthorizedResponse",
-        }
-
-        return self.api_client.call_api(
-            "/auth/token",
-            "POST",
-            _path_params,
-            _query_params,
-            _header_params,
-            body=_body_params,
-            post_params=_form_params,
-            files=_files,
-            response_types_map=_response_types_map,
-            auth_settings=_auth_settings,
-            async_req=_params.get("async_req"),
-            _return_http_data_only=_params.get("_return_http_data_only"),  # noqa: E501
-            _preload_content=_params.get("_preload_content", True),
-            _request_timeout=_params.get("_request_timeout"),
-            collection_formats=_collection_formats,
-            _request_auth=_params.get("_request_auth"),
-        )
-
-    @validate_arguments
-    def get_well_known_jwks(self, moneykit_version: Optional[Dict[str, Any]] = None, **kwargs) -> JWKSet:  # noqa: E501
-        """JSON Web Key Set  # noqa: E501
-
-        The JSON Web Key Set (JWKS) is a set of keys containing the public keys used to verify webhook JSON Web Tokens (JWT) issued by MoneyKit webhooks.  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.get_well_known_jwks(moneykit_version, async_req=True)
-        >>> result = thread.get()
-
-        :param moneykit_version:
-        :type moneykit_version: SupportedVersion
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: JWKSet
-        """
-        kwargs["_return_http_data_only"] = True
-        return self.get_well_known_jwks_with_http_info(moneykit_version, **kwargs)  # noqa: E501
+class SizeSchema(schemas.IntSchema):
+    pass
 
-    @validate_arguments
-    def get_well_known_jwks_with_http_info(
-        self, moneykit_version: Optional[Dict[str, Any]] = None, **kwargs
-    ):  # noqa: E501
-        """JSON Web Key Set  # noqa: E501
-
-        The JSON Web Key Set (JWKS) is a set of keys containing the public keys used to verify webhook JSON Web Tokens (JWT) issued by MoneyKit webhooks.  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.get_well_known_jwks_with_http_info(moneykit_version, async_req=True)
-        >>> result = thread.get()
-
-        :param moneykit_version:
-        :type moneykit_version: SupportedVersion
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the authentication
-                              in the spec for a single request.
-        :type _request_auth: dict, optional
-        :type _content_type: string, optional: force content-type for the request
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: tuple(JWKSet, status_code(int), headers(HTTPHeaderDict))
-        """
+class StartDateSchema(schemas.StrBase, schemas.NoneBase, schemas.Schema, schemas.NoneStrMixin):
+    def __new__(
+        cls,
+        *_args: typing.Union[
+            None,
+            str,
+        ],
+        _configuration: typing.Optional[schemas.Configuration] = None,
+    ) -> "StartDateSchema":
+        return super().__new__(
+            cls,
+            *_args,
+            _configuration=_configuration,
+        )
 
-        _params = locals()
+class EndDateSchema(schemas.StrBase, schemas.NoneBase, schemas.Schema, schemas.NoneStrMixin):
+    def __new__(
+        cls,
+        *_args: typing.Union[
+            None,
+            str,
+        ],
+        _configuration: typing.Optional[schemas.Configuration] = None,
+    ) -> "EndDateSchema":
+        return super().__new__(
+            cls,
+            *_args,
+            _configuration=_configuration,
+        )
 
-        _all_params = ["moneykit_version"]
-        _all_params.extend(
-            [
-                "async_req",
-                "_return_http_data_only",
-                "_preload_content",
-                "_request_timeout",
-                "_request_auth",
-                "_content_type",
-                "_headers",
+RequestRequiredQueryParams = typing_extensions.TypedDict("RequestRequiredQueryParams", {})
+RequestOptionalQueryParams = typing_extensions.TypedDict(
+    "RequestOptionalQueryParams",
+    {
+        "transaction_type": typing.Union[
+            TransactionTypeSchema,
+            list,
+            tuple,
+            None,
+        ],
+        "category": typing.Union[
+            CategorySchema,
+            list,
+            tuple,
+            None,
+        ],
+        "account_id": typing.Union[
+            AccountIdSchema,
+            list,
+            tuple,
+            None,
+        ],
+        "institution_id": typing.Union[
+            InstitutionIdSchema,
+            list,
+            tuple,
+            None,
+        ],
+        "page": typing.Union[
+            PageSchema,
+            decimal.Decimal,
+            int,
+        ],
+        "size": typing.Union[
+            SizeSchema,
+            decimal.Decimal,
+            int,
+        ],
+        "start_date": typing.Union[
+            StartDateSchema,
+            None,
+            str,
+        ],
+        "end_date": typing.Union[
+            EndDateSchema,
+            None,
+            str,
+        ],
+    },
+    total=False,
+)
+
+class RequestQueryParams(RequestRequiredQueryParams, RequestOptionalQueryParams):
+    pass
+
+request_query_transaction_type = api_client.QueryParameter(
+    name="transaction_type",
+    style=api_client.ParameterStyle.FORM,
+    schema=TransactionTypeSchema,
+    explode=True,
+)
+request_query_category = api_client.QueryParameter(
+    name="category",
+    style=api_client.ParameterStyle.FORM,
+    schema=CategorySchema,
+    explode=True,
+)
+request_query_account_id = api_client.QueryParameter(
+    name="account_id",
+    style=api_client.ParameterStyle.FORM,
+    schema=AccountIdSchema,
+    explode=True,
+)
+request_query_institution_id = api_client.QueryParameter(
+    name="institution_id",
+    style=api_client.ParameterStyle.FORM,
+    schema=InstitutionIdSchema,
+    explode=True,
+)
+request_query_page = api_client.QueryParameter(
+    name="page",
+    style=api_client.ParameterStyle.FORM,
+    schema=PageSchema,
+    explode=True,
+)
+request_query_size = api_client.QueryParameter(
+    name="size",
+    style=api_client.ParameterStyle.FORM,
+    schema=SizeSchema,
+    explode=True,
+)
+request_query_start_date = api_client.QueryParameter(
+    name="start_date",
+    style=api_client.ParameterStyle.FORM,
+    schema=StartDateSchema,
+    explode=True,
+)
+request_query_end_date = api_client.QueryParameter(
+    name="end_date",
+    style=api_client.ParameterStyle.FORM,
+    schema=EndDateSchema,
+    explode=True,
+)
+# Header params
+
+class MoneykitVersionSchema(
+    schemas.ComposedBase, schemas.DictBase, schemas.NoneBase, schemas.Schema, schemas.NoneFrozenDictMixin
+):
+    class MetaOapg:
+        @classmethod
+        @functools.lru_cache()
+        def all_of(cls):
+            # we need this here to make our import statements work
+            # we must store _composed_schemas in here so the code is only run
+            # when we invoke this method. If we kept this at the class
+            # level we would get an error because the class level
+            # code would be run when this module is imported, and these composed
+            # classes don't exist yet because their module has not finished
+            # loading
+            return [
+                SupportedVersion,
             ]
+    def __new__(
+        cls,
+        *_args: typing.Union[
+            dict,
+            frozendict.frozendict,
+            None,
+        ],
+        _configuration: typing.Optional[schemas.Configuration] = None,
+        **kwargs: typing.Union[
+            schemas.AnyTypeSchema,
+            dict,
+            frozendict.frozendict,
+            str,
+            date,
+            datetime,
+            uuid.UUID,
+            int,
+            float,
+            decimal.Decimal,
+            None,
+            list,
+            tuple,
+            bytes,
+        ],
+    ) -> "MoneykitVersionSchema":
+        return super().__new__(
+            cls,
+            *_args,
+            _configuration=_configuration,
+            **kwargs,
         )
 
-        # validate the arguments
-        for _key, _val in _params["kwargs"].items():
-            if _key not in _all_params:
-                raise ApiTypeError("Got an unexpected keyword argument '%s'" " to method get_well_known_jwks" % _key)
-            _params[_key] = _val
-        del _params["kwargs"]
+RequestRequiredHeaderParams = typing_extensions.TypedDict("RequestRequiredHeaderParams", {})
+RequestOptionalHeaderParams = typing_extensions.TypedDict(
+    "RequestOptionalHeaderParams",
+    {
+        "moneykit-version": typing.Union[
+            MoneykitVersionSchema,
+            dict,
+            frozendict.frozendict,
+            None,
+        ],
+    },
+    total=False,
+)
+
+class RequestHeaderParams(RequestRequiredHeaderParams, RequestOptionalHeaderParams):
+    pass
+
+request_header_moneykit_version = api_client.HeaderParameter(
+    name="moneykit-version",
+    style=api_client.ParameterStyle.SIMPLE,
+    schema=MoneykitVersionSchema,
+)
+# Path params
+IdSchema = schemas.StrSchema
+RequestRequiredPathParams = typing_extensions.TypedDict(
+    "RequestRequiredPathParams",
+    {
+        "id": typing.Union[
+            IdSchema,
+            str,
+        ],
+    },
+)
+RequestOptionalPathParams = typing_extensions.TypedDict("RequestOptionalPathParams", {}, total=False)
+
+class RequestPathParams(RequestRequiredPathParams, RequestOptionalPathParams):
+    pass
+
+request_path_id = api_client.PathParameter(
+    name="id",
+    style=api_client.ParameterStyle.SIMPLE,
+    schema=IdSchema,
+    required=True,
+)
+SchemaFor200ResponseBodyApplicationJson = GetUserTransactionsResponse
+
+@dataclass
+class ApiResponseFor200(api_client.ApiResponse):
+    response: urllib3.HTTPResponse
+    body: typing.Union[SchemaFor200ResponseBodyApplicationJson,]
+    headers: schemas.Unset = schemas.unset
+
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
+    content={
+        "application/json": api_client.MediaType(schema=SchemaFor200ResponseBodyApplicationJson),
+    },
+)
+
+class SchemaFor401ResponseBodyApplicationJson(
+    schemas.ComposedSchema,
+):
+    class MetaOapg:
+        @classmethod
+        @functools.lru_cache()
+        def any_of(cls):
+            # we need this here to make our import statements work
+            # we must store _composed_schemas in here so the code is only run
+            # when we invoke this method. If we kept this at the class
+            # level we would get an error because the class level
+            # code would be run when this module is imported, and these composed
+            # classes don't exist yet because their module has not finished
+            # loading
+            return [
+                APIErrorAuthExpiredAccessTokenResponse,
+                APIErrorAuthUnauthorizedResponse,
+            ]
+    def __new__(
+        cls,
+        *_args: typing.Union[
+            dict,
+            frozendict.frozendict,
+            str,
+            date,
+            datetime,
+            uuid.UUID,
+            int,
+            float,
+            decimal.Decimal,
+            bool,
+            None,
+            list,
+            tuple,
+            bytes,
+            io.FileIO,
+            io.BufferedReader,
+        ],
+        _configuration: typing.Optional[schemas.Configuration] = None,
+        **kwargs: typing.Union[
+            schemas.AnyTypeSchema,
+            dict,
+            frozendict.frozendict,
+            str,
+            date,
+            datetime,
+            uuid.UUID,
+            int,
+            float,
+            decimal.Decimal,
+            None,
+            list,
+            tuple,
+            bytes,
+        ],
+    ) -> "SchemaFor401ResponseBodyApplicationJson":
+        return super().__new__(
+            cls,
+            *_args,
+            _configuration=_configuration,
+            **kwargs,
+        )
 
-        _collection_formats = {}
+@dataclass
+class ApiResponseFor401(api_client.ApiResponse):
+    response: urllib3.HTTPResponse
+    body: typing.Union[SchemaFor401ResponseBodyApplicationJson,]
+    headers: schemas.Unset = schemas.unset
+
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
+    content={
+        "application/json": api_client.MediaType(schema=SchemaFor401ResponseBodyApplicationJson),
+    },
+)
+_all_accept_content_types = ("application/json",)
+
+class BaseApi(api_client.Api):
+    @typing.overload
+    def _get_user_transactions_oapg(
+        self,
+        query_params: RequestQueryParams = frozendict.frozendict(),
+        header_params: RequestHeaderParams = frozendict.frozendict(),
+        path_params: RequestPathParams = frozendict.frozendict(),
+        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        stream: bool = False,
+        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
+        skip_deserialization: typing_extensions.Literal[False] = ...,
+    ) -> typing.Union[ApiResponseFor200,]: ...
+    @typing.overload
+    def _get_user_transactions_oapg(
+        self,
+        skip_deserialization: typing_extensions.Literal[True],
+        query_params: RequestQueryParams = frozendict.frozendict(),
+        header_params: RequestHeaderParams = frozendict.frozendict(),
+        path_params: RequestPathParams = frozendict.frozendict(),
+        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        stream: bool = False,
+        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
+    ) -> api_client.ApiResponseWithoutDeserialization: ...
+    @typing.overload
+    def _get_user_transactions_oapg(
+        self,
+        query_params: RequestQueryParams = frozendict.frozendict(),
+        header_params: RequestHeaderParams = frozendict.frozendict(),
+        path_params: RequestPathParams = frozendict.frozendict(),
+        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        stream: bool = False,
+        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
+        skip_deserialization: bool = ...,
+    ) -> typing.Union[ApiResponseFor200, api_client.ApiResponseWithoutDeserialization,]: ...
+    def _get_user_transactions_oapg(
+        self,
+        query_params: RequestQueryParams = frozendict.frozendict(),
+        header_params: RequestHeaderParams = frozendict.frozendict(),
+        path_params: RequestPathParams = frozendict.frozendict(),
+        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        stream: bool = False,
+        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
+        skip_deserialization: bool = False,
+    ):
+        """
+        /users/{id}/transactions
+        :param skip_deserialization: If true then api_response.response will be set but
+            api_response.body and api_response.headers will not be deserialized into schema
+            class instances
+        """
+        self._verify_typed_dict_inputs_oapg(RequestQueryParams, query_params)
+        self._verify_typed_dict_inputs_oapg(RequestHeaderParams, header_params)
+        self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
+        used_path = path.value
 
-        # process the path parameters
         _path_params = {}
+        for parameter in (request_path_id,):
+            parameter_data = path_params.get(parameter.name, schemas.unset)
+            if parameter_data is schemas.unset:
+                continue
+            serialized_data = parameter.serialize(parameter_data)
+            _path_params.update(serialized_data)
+
+        for k, v in _path_params.items():
+            used_path = used_path.replace("{%s}" % k, v)
+
+        prefix_separator_iterator = None
+        for parameter in (
+            request_query_transaction_type,
+            request_query_category,
+            request_query_account_id,
+            request_query_institution_id,
+            request_query_page,
+            request_query_size,
+            request_query_start_date,
+            request_query_end_date,
+        ):
+            parameter_data = query_params.get(parameter.name, schemas.unset)
+            if parameter_data is schemas.unset:
+                continue
+            if prefix_separator_iterator is None:
+                prefix_separator_iterator = parameter.get_prefix_separator_iterator()
+            serialized_data = parameter.serialize(parameter_data, prefix_separator_iterator)
+            for serialized_value in serialized_data.values():
+                used_path += serialized_value
+
+        _headers = HTTPHeaderDict()
+        for parameter in (request_header_moneykit_version,):
+            parameter_data = header_params.get(parameter.name, schemas.unset)
+            if parameter_data is schemas.unset:
+                continue
+            serialized_data = parameter.serialize(parameter_data)
+            _headers.extend(serialized_data)
+        # TODO add cookie handling
+        if accept_content_types:
+            for accept_content_type in accept_content_types:
+                _headers.add("Accept", accept_content_type)
+
+        response = self.api_client.call_api(
+            resource_path=used_path,
+            method="get".upper(),
+            headers=_headers,
+            auth_settings=_auth,
+            stream=stream,
+            timeout=timeout,
+        )
 
-        # process the query parameters
-        _query_params = []
-        # process the header parameters
-        _header_params = dict(_params.get("_headers", {}))
-        if _params["moneykit_version"]:
-            _header_params["moneykit-version"] = _params["moneykit_version"]
-
-        # process the form parameters
-        _form_params = []
-        _files = {}
-        # process the body parameter
-        _body_params = None
-        # set the HTTP header `Accept`
-        _header_params["Accept"] = self.api_client.select_header_accept(["application/json"])  # noqa: E501
-
-        # authentication setting
-        _auth_settings = ["clientId", "OAuth2ClientCredentials", "clientSecret"]  # noqa: E501
-
-        _response_types_map = {
-            "200": "JWKSet",
-            "401": "Response401GetWellKnownJwksWellKnownJwksJsonGet",
-        }
-
-        return self.api_client.call_api(
-            "/.well-known/jwks.json",
-            "GET",
-            _path_params,
-            _query_params,
-            _header_params,
-            body=_body_params,
-            post_params=_form_params,
-            files=_files,
-            response_types_map=_response_types_map,
-            auth_settings=_auth_settings,
-            async_req=_params.get("async_req"),
-            _return_http_data_only=_params.get("_return_http_data_only"),  # noqa: E501
-            _preload_content=_params.get("_preload_content", True),
-            _request_timeout=_params.get("_request_timeout"),
-            collection_formats=_collection_formats,
-            _request_auth=_params.get("_request_auth"),
-        )
-
-    @validate_arguments
-    def instrospect_client(
-        self, moneykit_version: Optional[Dict[str, Any]] = None, **kwargs
-    ) -> APIClientOut:  # noqa: E501
-        """/auth/introspect  # noqa: E501
-
-        Get details about the client and application associated with your `access_token`.  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.instrospect_client(moneykit_version, async_req=True)
-        >>> result = thread.get()
-
-        :param moneykit_version:
-        :type moneykit_version: SupportedVersion
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: APIClientOut
-        """
-        kwargs["_return_http_data_only"] = True
-        return self.instrospect_client_with_http_info(moneykit_version, **kwargs)  # noqa: E501
+        if skip_deserialization:
+            api_response = api_client.ApiResponseWithoutDeserialization(response=response)
+        else:
+            response_for_status = _status_code_to_response.get(str(response.status))
+            if response_for_status:
+                api_response = response_for_status.deserialize(response, self.api_client.configuration)
+            else:
+                api_response = api_client.ApiResponseWithoutDeserialization(response=response)
+
+        if not 200 <= response.status <= 299:
+            raise exceptions.ApiException(status=response.status, reason=response.reason, api_response=api_response)
 
-    @validate_arguments
-    def instrospect_client_with_http_info(
-        self, moneykit_version: Optional[Dict[str, Any]] = None, **kwargs
-    ):  # noqa: E501
-        """/auth/introspect  # noqa: E501
-
-        Get details about the client and application associated with your `access_token`.  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.instrospect_client_with_http_info(moneykit_version, async_req=True)
-        >>> result = thread.get()
-
-        :param moneykit_version:
-        :type moneykit_version: SupportedVersion
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the authentication
-                              in the spec for a single request.
-        :type _request_auth: dict, optional
-        :type _content_type: string, optional: force content-type for the request
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: tuple(APIClientOut, status_code(int), headers(HTTPHeaderDict))
-        """
+        return api_response
 
-        _params = locals()
+class GetUserTransactions(BaseApi):
+    # this class is used by api classes that refer to endpoints with operationId fn names
 
-        _all_params = ["moneykit_version"]
-        _all_params.extend(
-            [
-                "async_req",
-                "_return_http_data_only",
-                "_preload_content",
-                "_request_timeout",
-                "_request_auth",
-                "_content_type",
-                "_headers",
-            ]
+    @typing.overload
+    def get_user_transactions(
+        self,
+        query_params: RequestQueryParams = frozendict.frozendict(),
+        header_params: RequestHeaderParams = frozendict.frozendict(),
+        path_params: RequestPathParams = frozendict.frozendict(),
+        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        stream: bool = False,
+        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
+        skip_deserialization: typing_extensions.Literal[False] = ...,
+    ) -> typing.Union[ApiResponseFor200,]: ...
+    @typing.overload
+    def get_user_transactions(
+        self,
+        skip_deserialization: typing_extensions.Literal[True],
+        query_params: RequestQueryParams = frozendict.frozendict(),
+        header_params: RequestHeaderParams = frozendict.frozendict(),
+        path_params: RequestPathParams = frozendict.frozendict(),
+        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        stream: bool = False,
+        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
+    ) -> api_client.ApiResponseWithoutDeserialization: ...
+    @typing.overload
+    def get_user_transactions(
+        self,
+        query_params: RequestQueryParams = frozendict.frozendict(),
+        header_params: RequestHeaderParams = frozendict.frozendict(),
+        path_params: RequestPathParams = frozendict.frozendict(),
+        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        stream: bool = False,
+        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
+        skip_deserialization: bool = ...,
+    ) -> typing.Union[ApiResponseFor200, api_client.ApiResponseWithoutDeserialization,]: ...
+    def get_user_transactions(
+        self,
+        query_params: RequestQueryParams = frozendict.frozendict(),
+        header_params: RequestHeaderParams = frozendict.frozendict(),
+        path_params: RequestPathParams = frozendict.frozendict(),
+        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        stream: bool = False,
+        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
+        skip_deserialization: bool = False,
+    ):
+        return self._get_user_transactions_oapg(
+            query_params=query_params,
+            header_params=header_params,
+            path_params=path_params,
+            accept_content_types=accept_content_types,
+            stream=stream,
+            timeout=timeout,
+            skip_deserialization=skip_deserialization,
         )
 
-        # validate the arguments
-        for _key, _val in _params["kwargs"].items():
-            if _key not in _all_params:
-                raise ApiTypeError("Got an unexpected keyword argument '%s'" " to method instrospect_client" % _key)
-            _params[_key] = _val
-        del _params["kwargs"]
-
-        _collection_formats = {}
-
-        # process the path parameters
-        _path_params = {}
+class ApiForget(BaseApi):
+    # this class is used by api classes that refer to endpoints by path and http method names
 
-        # process the query parameters
-        _query_params = []
-        # process the header parameters
-        _header_params = dict(_params.get("_headers", {}))
-        if _params["moneykit_version"]:
-            _header_params["moneykit-version"] = _params["moneykit_version"]
-
-        # process the form parameters
-        _form_params = []
-        _files = {}
-        # process the body parameter
-        _body_params = None
-        # set the HTTP header `Accept`
-        _header_params["Accept"] = self.api_client.select_header_accept(["application/json"])  # noqa: E501
-
-        # authentication setting
-        _auth_settings = ["clientId", "OAuth2ClientCredentials", "clientSecret"]  # noqa: E501
-
-        _response_types_map = {
-            "200": "APIClientOut",
-            "401": "Response401InstrospectClientAuthIntrospectGet",
-        }
-
-        return self.api_client.call_api(
-            "/auth/introspect",
-            "GET",
-            _path_params,
-            _query_params,
-            _header_params,
-            body=_body_params,
-            post_params=_form_params,
-            files=_files,
-            response_types_map=_response_types_map,
-            auth_settings=_auth_settings,
-            async_req=_params.get("async_req"),
-            _return_http_data_only=_params.get("_return_http_data_only"),  # noqa: E501
-            _preload_content=_params.get("_preload_content", True),
-            _request_timeout=_params.get("_request_timeout"),
-            collection_formats=_collection_formats,
-            _request_auth=_params.get("_request_auth"),
+    @typing.overload
+    def get(
+        self,
+        query_params: RequestQueryParams = frozendict.frozendict(),
+        header_params: RequestHeaderParams = frozendict.frozendict(),
+        path_params: RequestPathParams = frozendict.frozendict(),
+        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        stream: bool = False,
+        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
+        skip_deserialization: typing_extensions.Literal[False] = ...,
+    ) -> typing.Union[ApiResponseFor200,]: ...
+    @typing.overload
+    def get(
+        self,
+        skip_deserialization: typing_extensions.Literal[True],
+        query_params: RequestQueryParams = frozendict.frozendict(),
+        header_params: RequestHeaderParams = frozendict.frozendict(),
+        path_params: RequestPathParams = frozendict.frozendict(),
+        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        stream: bool = False,
+        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
+    ) -> api_client.ApiResponseWithoutDeserialization: ...
+    @typing.overload
+    def get(
+        self,
+        query_params: RequestQueryParams = frozendict.frozendict(),
+        header_params: RequestHeaderParams = frozendict.frozendict(),
+        path_params: RequestPathParams = frozendict.frozendict(),
+        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        stream: bool = False,
+        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
+        skip_deserialization: bool = ...,
+    ) -> typing.Union[ApiResponseFor200, api_client.ApiResponseWithoutDeserialization,]: ...
+    def get(
+        self,
+        query_params: RequestQueryParams = frozendict.frozendict(),
+        header_params: RequestHeaderParams = frozendict.frozendict(),
+        path_params: RequestPathParams = frozendict.frozendict(),
+        accept_content_types: typing.Tuple[str] = _all_accept_content_types,
+        stream: bool = False,
+        timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
+        skip_deserialization: bool = False,
+    ):
+        return self._get_user_transactions_oapg(
+            query_params=query_params,
+            header_params=header_params,
+            path_params=path_params,
+            accept_content_types=accept_content_types,
+            stream=stream,
+            timeout=timeout,
+            skip_deserialization=skip_deserialization,
         )
```

### Comparing `moneykit-0.0.6/moneykit/configuration.py` & `moneykit-0.0.7/moneykit/configuration.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,67 +2,93 @@
 
 """
     MoneyKit API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
+    Generated by: https://openapi-generator.tech
 """
 
-
 import copy
-import http.client as httplib
 import logging
 import multiprocessing
 import sys
+from http import client as http_client
 
 import urllib3
 
+from moneykit.exceptions import ApiValueError
+
 JSON_SCHEMA_VALIDATION_KEYWORDS = {
     "multipleOf",
     "maximum",
     "exclusiveMaximum",
     "minimum",
     "exclusiveMinimum",
     "maxLength",
     "minLength",
     "pattern",
     "maxItems",
     "minItems",
+    "uniqueItems",
+    "maxProperties",
+    "minProperties",
 }
 
 
 class Configuration(object):
-    """This class contains various settings of the API client.
+    """NOTE: This class is auto generated by OpenAPI Generator
 
-        :param host: Base url.
+        Ref: https://openapi-generator.tech
+        Do not edit the class manually.
+
+        :param host: Base url
         :param api_key: Dict to store API key(s).
           Each entry in the dict specifies an API key.
           The dict key is the name of the security scheme in the OAS specification.
           The dict value is the API key secret.
-        :param api_key_prefix: Dict to store API prefix (e.g. Bearer).
+        :param api_key_prefix: Dict to store API prefix (e.g. Bearer)
           The dict key is the name of the security scheme in the OAS specification.
           The dict value is an API key prefix when generating the auth data.
-        :param username: Username for HTTP basic authentication.
-        :param password: Password for HTTP basic authentication.
-        :param access_token: Access token.
+        :param username: Username for HTTP basic authentication
+        :param password: Password for HTTP basic authentication
+        :param discard_unknown_keys: Boolean value indicating whether to discard
+          unknown properties. A server may send a response that includes additional
+          properties that are not known by the client in the following scenarios:
+          1. The OpenAPI document is incomplete, i.e. it does not match the server
+             implementation.
+          2. The client was generated using an older version of the OpenAPI document
+             and the server has been upgraded since then.
+          If a schema in the OpenAPI document defines the additionalProperties attribute,
+          then all undeclared properties received by the server are injected into the
+          additional properties map. In that case, there are undeclared properties, and
+          nothing to discard.
+        :param disabled_client_side_validations (string): Comma-separated list of
+          JSON schema validation keywords to disable JSON schema structural validation
+          rules. The following keywords may be specified: multipleOf, maximum,
+          exclusiveMaximum, minimum, exclusiveMinimum, maxLength, minLength, pattern,
+          maxItems, minItems.
+          By default, the validation is performed for data generated locally by the client
+          and data received from the server, independent of any validation performed by
+          the server side. If the input data does not satisfy the JSON schema validation
+          rules specified in the OpenAPI document, an exception is raised.
+          If disabled_client_side_validations is set, structural validation is
+          disabled. This can be useful to troubleshoot data validation problem, such as
+          when the OpenAPI document validation rules do not match the actual API data
+          received by the server.
         :param server_index: Index to servers configuration.
         :param server_variables: Mapping with string values to replace variables in
           templated server configuration. The validation of enums is performed for
           variables with defined enum values before.
         :param server_operation_index: Mapping from operation ID to an index to server
           configuration.
         :param server_operation_variables: Mapping from operation ID to a mapping with
           string values to replace variables in templated server configuration.
           The validation of enums is performed for variables with defined enum values before.
-        :param ssl_ca_cert: str - the path to a file of concatenated CA certificates
-          in PEM format.
 
         :Example:
 
         API Key Authentication Example.
         Given the following security scheme in the OpenAPI specification:
           components:
             securitySchemes:
@@ -103,20 +129,21 @@
     def __init__(
         self,
         host=None,
         api_key=None,
         api_key_prefix=None,
         username=None,
         password=None,
-        access_token=None,
+        discard_unknown_keys=False,
+        disabled_client_side_validations="",
         server_index=None,
         server_variables=None,
         server_operation_index=None,
         server_operation_variables=None,
-        ssl_ca_cert=None,
+        access_token=None,
     ):
         """Constructor"""
         self._base_path = "https://production.moneykit.com" if host is None else host
         """Default Base url
         """
         self.server_index = 0 if server_index is None and host is None else server_index
         self.server_operation_index = server_operation_index or {}
@@ -145,17 +172,16 @@
         """
         self.username = username
         """Username for HTTP basic authentication
         """
         self.password = password
         """Password for HTTP basic authentication
         """
-        self.access_token = access_token
-        """Access token
-        """
+        self.discard_unknown_keys = discard_unknown_keys
+        self.disabled_client_side_validations = disabled_client_side_validations
         self.access_token = None
         """access token for OAuth/Bearer
         """
         self.logger = {}
         """Logging Settings
         """
         self.logger["package_logger"] = logging.getLogger("moneykit")
@@ -177,15 +203,15 @@
         """
 
         self.verify_ssl = True
         """SSL/TLS verification
            Set this to false to skip verifying SSL certificate when calling API
            from https server.
         """
-        self.ssl_ca_cert = ssl_ca_cert
+        self.ssl_ca_cert = None
         """Set this to customize the certificate file to verify the peer.
         """
         self.cert_file = None
         """client certificate file
         """
         self.key_file = None
         """client key file
@@ -213,25 +239,16 @@
         """
         self.retries = None
         """Adding retries to override urllib3 default value 3
         """
         # Enable client side validation
         self.client_side_validation = True
 
+        # Options to pass down to the underlying urllib3 socket
         self.socket_options = None
-        """Options to pass down to the underlying urllib3 socket
-        """
-
-        self.datetime_format = "%Y-%m-%dT%H:%M:%S.%f%z"
-        """datetime format
-        """
-
-        self.date_format = "%Y-%m-%d"
-        """date format
-        """
 
     def __deepcopy__(self, memo):
         cls = self.__class__
         result = cls.__new__(cls)
         memo[id(self)] = result
         for k, v in self.__dict__.items():
             if k not in ("logger", "logger_file_handler"):
@@ -241,49 +258,45 @@
         # use setters to configure loggers
         result.logger_file = self.logger_file
         result.debug = self.debug
         return result
 
     def __setattr__(self, name, value):
         object.__setattr__(self, name, value)
+        if name == "disabled_client_side_validations":
+            s = set(filter(None, value.split(",")))
+            for v in s:
+                if v not in JSON_SCHEMA_VALIDATION_KEYWORDS:
+                    raise ApiValueError("Invalid keyword: '{0}''".format(v))
+            self._disabled_client_side_validations = s
 
     @classmethod
     def set_default(cls, default):
         """Set default instance of configuration.
 
         It stores default configuration, which can be
         returned by get_default_copy method.
 
         :param default: object of Configuration
         """
-        cls._default = default
+        cls._default = copy.deepcopy(default)
 
     @classmethod
     def get_default_copy(cls):
-        """Deprecated. Please use `get_default` instead.
-
-        Deprecated. Please use `get_default` instead.
-
-        :return: The configuration object.
-        """
-        return cls.get_default()
-
-    @classmethod
-    def get_default(cls):
-        """Return the default configuration.
+        """Return new instance of configuration.
 
         This method returns newly created, based on default constructor,
         object of Configuration class or returns a copy of default
-        configuration.
+        configuration passed by the set_default method.
 
         :return: The configuration object.
         """
-        if cls._default is None:
-            cls._default = Configuration()
-        return cls._default
+        if cls._default is not None:
+            return copy.deepcopy(cls._default)
+        return Configuration()
 
     @property
     def logger_file(self):
         """The logger file.
 
         If the logger_file is None, then add stream handler and remove file
         handler. Otherwise, add file handler and remove stream handler.
@@ -329,23 +342,23 @@
         :type: bool
         """
         self.__debug = value
         if self.__debug:
             # if debug status is True, turn on debug logging
             for _, logger in self.logger.items():
                 logger.setLevel(logging.DEBUG)
-            # turn on httplib debug
-            httplib.HTTPConnection.debuglevel = 1
+            # turn on http_client debug
+            http_client.HTTPConnection.debuglevel = 1
         else:
             # if debug status is False, turn off debug logging,
             # setting log level to default `logging.WARNING`
             for _, logger in self.logger.items():
                 logger.setLevel(logging.WARNING)
-            # turn off httplib debug
-            httplib.HTTPConnection.debuglevel = 0
+            # turn off http_client debug
+            http_client.HTTPConnection.debuglevel = 0
 
     @property
     def logger_format(self):
         """The logger format.
 
         The logger_formatter will be updated when sets logger_format.
```

### Comparing `moneykit-0.0.6/moneykit/exceptions.py` & `moneykit-0.0.7/moneykit/plaid_compatible/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,26 @@
-# coding: utf-8
-
 """
     MoneyKit API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
+    Generated by: https://openapi-generator.tech
 """
 
 
+
 class OpenApiException(Exception):
     """The base exception class for all OpenAPIExceptions"""
 
 
 class ApiTypeError(OpenApiException, TypeError):
-    def __init__(self, msg, path_to_item=None, valid_classes=None, key_type=None):
-        """Raises an exception for TypeErrors
+    def __init__(self, msg, path_to_item=None, valid_classes=None,
+                 key_type=None):
+        """ Raises an exception for TypeErrors
 
         Args:
             msg (str): the exception message
 
         Keyword Args:
             path_to_item (list): a list of keys an indices to get to the
                                  current_item
@@ -95,54 +93,61 @@
         full_msg = msg
         if path_to_item:
             full_msg = "{0} at {1}".format(msg, render_path(path_to_item))
         super(ApiKeyError, self).__init__(full_msg)
 
 
 class ApiException(OpenApiException):
+
     def __init__(self, status=None, reason=None, http_resp=None):
         if http_resp:
             self.status = http_resp.status
             self.reason = http_resp.reason
             self.body = http_resp.data
             self.headers = http_resp.getheaders()
         else:
             self.status = status
             self.reason = reason
             self.body = None
             self.headers = None
 
     def __str__(self):
         """Custom error messages for exception"""
-        error_message = "({0})\n" "Reason: {1}\n".format(self.status, self.reason)
+        error_message = "({0})\n"\
+                        "Reason: {1}\n".format(self.status, self.reason)
         if self.headers:
-            error_message += "HTTP response headers: {0}\n".format(self.headers)
+            error_message += "HTTP response headers: {0}\n".format(
+                self.headers)
 
         if self.body:
             error_message += "HTTP response body: {0}\n".format(self.body)
 
         return error_message
 
 
 class NotFoundException(ApiException):
+
     def __init__(self, status=None, reason=None, http_resp=None):
         super(NotFoundException, self).__init__(status, reason, http_resp)
 
 
 class UnauthorizedException(ApiException):
+
     def __init__(self, status=None, reason=None, http_resp=None):
         super(UnauthorizedException, self).__init__(status, reason, http_resp)
 
 
 class ForbiddenException(ApiException):
+
     def __init__(self, status=None, reason=None, http_resp=None):
         super(ForbiddenException, self).__init__(status, reason, http_resp)
 
 
 class ServiceException(ApiException):
+
     def __init__(self, status=None, reason=None, http_resp=None):
         super(ServiceException, self).__init__(status, reason, http_resp)
 
 
 def render_path(path_to_item):
     """Returns a string representation of a path"""
     result = ""
```

### Comparing `moneykit-0.0.6/moneykit/models/account_with_account_numbers.py` & `moneykit-0.0.7/moneykit/model/identity_response.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,102 +2,161 @@
 
 """
     MoneyKit API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
+    Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import annotations
-
-import json
-import pprint
+import decimal  # noqa: F401
+import functools  # noqa: F401
+import io  # noqa: F401
 import re  # noqa: F401
-from typing import Optional
+import typing  # noqa: F401
+import uuid  # noqa: F401
+from datetime import date, datetime  # noqa: F401
 
-from pydantic import BaseModel, Field, StrictStr
+import frozendict  # noqa: F401
+import typing_extensions  # noqa: F401
 
-from moneykit.models.account_type import AccountType
-from moneykit.models.balances import Balances
-from moneykit.models.numbers import Numbers
+from moneykit import schemas  # noqa: F401
 
 
-class AccountWithAccountNumbers(BaseModel):
-    """
-    AccountWithAccountNumbers
+class IdentityResponse(schemas.DictSchema):
+    """NOTE: This class is auto generated by OpenAPI Generator.
+    Ref: https://openapi-generator.tech
+
+    Do not edit the class manually.
     """
 
-    account_id: StrictStr = Field(
-        ...,
-        description="MoneyKit's unique ID for the account.         <p>The `account_id` is distinct from the institution's account number.  For accounts that may change account         numbers from time to time, such as credit cards, MoneyKit attempts to keep the `account_id` constant.         However, if MoneyKit can't reconcile the new account data with the old data, the `account_id` may change.",
-    )
-    account_type: AccountType = ...
-    name: StrictStr = Field(
-        ...,
-        description="The account name, according to the institution.  Note that some institutions allow         the end user to nickname the account; in such cases this field may be the name assigned by the user",
-    )
-    account_mask: Optional[StrictStr] = Field(
-        None,
-        description="The last four characters (usually digits) of the account number.         Note that this mask may be non-unique between accounts.",
-    )
-    balances: Balances = ...
-    numbers: Numbers = ...
-    __properties = ["account_id", "account_type", "name", "account_mask", "balances", "numbers"]
-
-    class Config:
-        allow_population_by_field_name = True
-        validate_assignment = True
-
-    def to_str(self) -> str:
-        """Returns the string representation of the model using alias"""
-        return pprint.pformat(self.dict(by_alias=True))
-
-    def to_json(self) -> str:
-        """Returns the JSON representation of the model using alias"""
-        return json.dumps(self.to_dict())
-
-    @classmethod
-    def from_json(cls, json_str: str) -> AccountWithAccountNumbers:
-        """Create an instance of AccountWithAccountNumbers from a JSON string"""
-        return cls.from_dict(json.loads(json_str))
-
-    def to_dict(self):
-        """Returns the dictionary representation of the model using alias"""
-        _dict = self.dict(by_alias=True, exclude={}, exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of balances
-        if self.balances:
-            _dict["balances"] = self.balances.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of numbers
-        if self.numbers:
-            _dict["numbers"] = self.numbers.to_dict()
-        # set to None if account_mask (nullable) is None
-        # and __fields_set__ contains the field
-        if self.account_mask is None and "account_mask" in self.__fields_set__:
-            _dict["account_mask"] = None
-
-        return _dict
-
-    @classmethod
-    def from_dict(cls, obj: dict) -> AccountWithAccountNumbers:
-        """Create an instance of AccountWithAccountNumbers from a dict"""
-        if obj is None:
-            return None
-
-        if type(obj) is not dict:
-            return AccountWithAccountNumbers.parse_obj(obj)
-
-        _obj = AccountWithAccountNumbers.parse_obj(
-            {
-                "account_id": obj.get("account_id"),
-                "account_type": obj.get("account_type"),
-                "name": obj.get("name"),
-                "account_mask": obj.get("account_mask"),
-                "balances": Balances.from_dict(obj.get("balances")) if obj.get("balances") is not None else None,
-                "numbers": Numbers.from_dict(obj.get("numbers")) if obj.get("numbers") is not None else None,
+    class MetaOapg:
+        required = {
+            "link",
+            "accounts",
+        }
+
+        class properties:
+            class accounts(schemas.ListSchema):
+                class MetaOapg:
+                    @staticmethod
+                    def items() -> typing.Type["AccountIdentity"]:
+                        return AccountIdentity
+
+                def __new__(
+                    cls,
+                    _arg: typing.Union[typing.Tuple["AccountIdentity"], typing.List["AccountIdentity"]],
+                    _configuration: typing.Optional[schemas.Configuration] = None,
+                ) -> "accounts":
+                    return super().__new__(
+                        cls,
+                        _arg,
+                        _configuration=_configuration,
+                    )
+
+                def __getitem__(self, i: int) -> "AccountIdentity":
+                    return super().__getitem__(i)
+
+            @staticmethod
+            def link() -> typing.Type["LinkCommon"]:
+                return LinkCommon
+
+            __annotations__ = {
+                "accounts": accounts,
+                "link": link,
             }
+
+    link: "LinkCommon"
+    accounts: MetaOapg.properties.accounts
+
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["accounts"]) -> MetaOapg.properties.accounts:
+        ...
+
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["link"]) -> "LinkCommon":
+        ...
+
+    @typing.overload
+    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema:
+        ...
+
+    def __getitem__(
+        self,
+        name: typing.Union[
+            typing_extensions.Literal[
+                "accounts",
+                "link",
+            ],
+            str,
+        ],
+    ):
+        # dict_instance[name] accessor
+        return super().__getitem__(name)
+
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["accounts"]) -> MetaOapg.properties.accounts:
+        ...
+
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["link"]) -> "LinkCommon":
+        ...
+
+    @typing.overload
+    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]:
+        ...
+
+    def get_item_oapg(
+        self,
+        name: typing.Union[
+            typing_extensions.Literal[
+                "accounts",
+                "link",
+            ],
+            str,
+        ],
+    ):
+        return super().get_item_oapg(name)
+
+    def __new__(
+        cls,
+        *_args: typing.Union[
+            dict,
+            frozendict.frozendict,
+        ],
+        link: "LinkCommon",
+        accounts: typing.Union[
+            MetaOapg.properties.accounts,
+            list,
+            tuple,
+        ],
+        _configuration: typing.Optional[schemas.Configuration] = None,
+        **kwargs: typing.Union[
+            schemas.AnyTypeSchema,
+            dict,
+            frozendict.frozendict,
+            str,
+            date,
+            datetime,
+            uuid.UUID,
+            int,
+            float,
+            decimal.Decimal,
+            None,
+            list,
+            tuple,
+            bytes,
+        ],
+    ) -> "IdentityResponse":
+        return super().__new__(
+            cls,
+            *_args,
+            link=link,
+            accounts=accounts,
+            _configuration=_configuration,
+            **kwargs,
         )
-        return _obj
+
+
+from moneykit.model.account_identity import AccountIdentity
+from moneykit.model.link_common import LinkCommon
```

### Comparing `moneykit-0.0.6/moneykit/models/api_client_out.py` & `moneykit-0.0.7/moneykit/model/exchange_token_request.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,87 +2,106 @@
 
 """
     MoneyKit API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
+    Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import annotations
-
-import json
-import pprint
+import decimal  # noqa: F401
+import functools  # noqa: F401
+import io  # noqa: F401
 import re  # noqa: F401
-from datetime import datetime
-from typing import Optional
+import typing  # noqa: F401
+import uuid  # noqa: F401
+from datetime import date, datetime  # noqa: F401
 
-from pydantic import BaseModel, Field, StrictStr
+import frozendict  # noqa: F401
+import typing_extensions  # noqa: F401
 
-from moneykit.models.app import App
+from moneykit import schemas  # noqa: F401
 
 
-class APIClientOut(BaseModel):
-    """
-    MoneyKit API client for an application.
+class ExchangeTokenRequest(schemas.DictSchema):
+    """NOTE: This class is auto generated by OpenAPI Generator.
+    Ref: https://openapi-generator.tech
+
+    Do not edit the class manually.
     """
 
-    client_id: StrictStr = Field(..., description="Your application's MoneyKit client ID.")
-    client_name: StrictStr = Field(..., description="Friendly API client name for identification.")
-    scope: StrictStr = Field(..., description="Actions allowed by the client.")
-    app: App = ...
-    disabled_at: Optional[datetime] = Field(None, description="Set to timestamp if the client has been disabled.")
-    __properties = ["client_id", "client_name", "scope", "app", "disabled_at"]
-
-    class Config:
-        allow_population_by_field_name = True
-        validate_assignment = True
-
-    def to_str(self) -> str:
-        """Returns the string representation of the model using alias"""
-        return pprint.pformat(self.dict(by_alias=True))
-
-    def to_json(self) -> str:
-        """Returns the JSON representation of the model using alias"""
-        return json.dumps(self.to_dict())
-
-    @classmethod
-    def from_json(cls, json_str: str) -> APIClientOut:
-        """Create an instance of APIClientOut from a JSON string"""
-        return cls.from_dict(json.loads(json_str))
-
-    def to_dict(self):
-        """Returns the dictionary representation of the model using alias"""
-        _dict = self.dict(by_alias=True, exclude={}, exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of app
-        if self.app:
-            _dict["app"] = self.app.to_dict()
-        # set to None if disabled_at (nullable) is None
-        # and __fields_set__ contains the field
-        if self.disabled_at is None and "disabled_at" in self.__fields_set__:
-            _dict["disabled_at"] = None
-
-        return _dict
-
-    @classmethod
-    def from_dict(cls, obj: dict) -> APIClientOut:
-        """Create an instance of APIClientOut from a dict"""
-        if obj is None:
-            return None
-
-        if type(obj) is not dict:
-            return APIClientOut.parse_obj(obj)
-
-        _obj = APIClientOut.parse_obj(
-            {
-                "client_id": obj.get("client_id"),
-                "client_name": obj.get("client_name"),
-                "scope": obj.get("scope"),
-                "app": App.from_dict(obj.get("app")) if obj.get("app") is not None else None,
-                "disabled_at": obj.get("disabled_at"),
+    class MetaOapg:
+        required = {
+            "exchangeable_token",
+        }
+
+        class properties:
+            exchangeable_token = schemas.StrSchema
+            __annotations__ = {
+                "exchangeable_token": exchangeable_token,
             }
+
+    exchangeable_token: MetaOapg.properties.exchangeable_token
+
+    @typing.overload
+    def __getitem__(
+        self, name: typing_extensions.Literal["exchangeable_token"]
+    ) -> MetaOapg.properties.exchangeable_token:
+        ...
+
+    @typing.overload
+    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema:
+        ...
+
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["exchangeable_token",], str]):
+        # dict_instance[name] accessor
+        return super().__getitem__(name)
+
+    @typing.overload
+    def get_item_oapg(
+        self, name: typing_extensions.Literal["exchangeable_token"]
+    ) -> MetaOapg.properties.exchangeable_token:
+        ...
+
+    @typing.overload
+    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]:
+        ...
+
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["exchangeable_token",], str]):
+        return super().get_item_oapg(name)
+
+    def __new__(
+        cls,
+        *_args: typing.Union[
+            dict,
+            frozendict.frozendict,
+        ],
+        exchangeable_token: typing.Union[
+            MetaOapg.properties.exchangeable_token,
+            str,
+        ],
+        _configuration: typing.Optional[schemas.Configuration] = None,
+        **kwargs: typing.Union[
+            schemas.AnyTypeSchema,
+            dict,
+            frozendict.frozendict,
+            str,
+            date,
+            datetime,
+            uuid.UUID,
+            int,
+            float,
+            decimal.Decimal,
+            None,
+            list,
+            tuple,
+            bytes,
+        ],
+    ) -> "ExchangeTokenRequest":
+        return super().__new__(
+            cls,
+            *_args,
+            exchangeable_token=exchangeable_token,
+            _configuration=_configuration,
+            **kwargs,
         )
-        return _obj
```

### Comparing `moneykit-0.0.6/moneykit/models/country.py` & `moneykit-0.0.7/moneykit/apis/tags/access_token_api.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,29 +2,27 @@
 
 """
     MoneyKit API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
+    Generated by: https://openapi-generator.tech
 """
 
+from moneykit.paths.auth_introspect.get import InstrospectClient
+from moneykit.paths.auth_token.post import GenerateAccessToken
+from moneykit.paths.well_known_jwks_json.get import GetWellKnownJwks
 
-import re  # noqa: F401
 
-from aenum import Enum
+class AccessTokenApi(
+    GenerateAccessToken,
+    GetWellKnownJwks,
+    InstrospectClient,
+):
+    """NOTE: This class is auto generated by OpenAPI Generator
+    Ref: https://openapi-generator.tech
 
-
-class Country(str, Enum):
-    """
-    An enumeration.
+    Do not edit the class manually.
     """
 
-    """
-    allowed enum values
-    """
-    US = "US"
-    GB = "GB"
-    CA = "CA"
+    pass
```

### Comparing `moneykit-0.0.6/moneykit/models/link_error.py` & `moneykit-0.0.7/moneykit/apis/tags/account_numbers_api.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,33 +2,23 @@
 
 """
     MoneyKit API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
+    Generated by: https://openapi-generator.tech
 """
 
+from moneykit.paths.links_id_accounts_numbers.get import GetAccountNumbers
 
-import re  # noqa: F401
 
-from aenum import Enum
+class AccountNumbersApi(
+    GetAccountNumbers,
+):
+    """NOTE: This class is auto generated by OpenAPI Generator
+    Ref: https://openapi-generator.tech
 
-
-class LinkError(str, Enum):
-    """
-    An enumeration.
+    Do not edit the class manually.
     """
 
-    """
-    allowed enum values
-    """
-    SYSTEM_ERROR = "system_error"
-    PROVIDER_ERROR = "provider_error"
-    INSTITUTION_ERROR = "institution_error"
-    USER_ERROR = "user_error"
-    AUTH_EXPIRED = "auth_expired"
-    INCOMPLETE = "incomplete"
-    PAYMENT_ERROR = "payment_error"
+    pass
```

### Comparing `moneykit-0.0.6/moneykit/models/link_state.py` & `moneykit-0.0.7/moneykit/apis/tags/links_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,31 +2,29 @@
 
 """
     MoneyKit API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
+    Generated by: https://openapi-generator.tech
 """
 
+from moneykit.paths.links_id.delete import Disconnect
+from moneykit.paths.links_id.get import GetLink
+from moneykit.paths.links_id.patch import UpdateLink
+from moneykit.paths.users_id_links.get import GetUserLinks
 
-import re  # noqa: F401
 
-from aenum import Enum
+class LinksApi(
+    Disconnect,
+    GetLink,
+    GetUserLinks,
+    UpdateLink,
+):
+    """NOTE: This class is auto generated by OpenAPI Generator
+    Ref: https://openapi-generator.tech
 
-
-class LinkState(str, Enum):
-    """
-    An enumeration.
+    Do not edit the class manually.
     """
 
-    """
-    allowed enum values
-    """
-    CONNECTING = "connecting"
-    AWAITING_TOKEN_EXCHANGE = "awaiting_token_exchange"
-    CONNECTED = "connected"
-    DELETED = "deleted"
-    ERROR = "error"
+    pass
```

### Comparing `moneykit-0.0.6/moneykit/models/money_kit_env.py` & `moneykit-0.0.7/moneykit/apis/tags/users_api.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,28 +2,27 @@
 
 """
     MoneyKit API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
+    Generated by: https://openapi-generator.tech
 """
 
+from moneykit.paths.users_id_accounts.get import GetUserAccounts
+from moneykit.paths.users_id_links.get import GetUserLinks
+from moneykit.paths.users_id_transactions.get import GetUserTransactions
 
-import re  # noqa: F401
 
-from aenum import Enum
+class UsersApi(
+    GetUserAccounts,
+    GetUserLinks,
+    GetUserTransactions,
+):
+    """NOTE: This class is auto generated by OpenAPI Generator
+    Ref: https://openapi-generator.tech
 
-
-class MoneyKitEnv(str, Enum):
-    """
-    An enumeration.
+    Do not edit the class manually.
     """
 
-    """
-    allowed enum values
-    """
-    PRODUCTION = "production"
-    SANDBOX = "sandbox"
+    pass
```

### Comparing `moneykit-0.0.6/moneykit/models/numbers.py` & `moneykit-0.0.7/moneykit/model/get_user_accounts_response.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,110 +2,134 @@
 
 """
     MoneyKit API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
+    Generated by: https://openapi-generator.tech
 """
 
-
-from __future__ import annotations
-
-import json
-import pprint
+import decimal  # noqa: F401
+import functools  # noqa: F401
+import io  # noqa: F401
 import re  # noqa: F401
+import typing  # noqa: F401
+import uuid  # noqa: F401
+from datetime import date, datetime  # noqa: F401
 
-from pydantic import BaseModel, Field, conlist
+import frozendict  # noqa: F401
+import typing_extensions  # noqa: F401
 
-from moneykit.models.ach_number import AchNumber
-from moneykit.models.bacs_number import BacsNumber
-from moneykit.models.eft_number import EftNumber
-from moneykit.models.international_number import InternationalNumber
+from moneykit import schemas  # noqa: F401
 
 
-class Numbers(BaseModel):
-    """
-    The various types of account numbers.
+class GetUserAccountsResponse(schemas.DictSchema):
+    """NOTE: This class is auto generated by OpenAPI Generator.
+    Ref: https://openapi-generator.tech
+
+    Do not edit the class manually.
     """
 
-    ach: conlist(AchNumber) = Field(..., description="List of ACH account numbers.")
-    bacs: conlist(BacsNumber) = Field(..., description="List of BACS account numbers.")
-    eft: conlist(EftNumber) = Field(..., description="List of EFT account numbers.")
-    international: conlist(InternationalNumber) = Field(..., description="List of international account numbers.")
-    __properties = ["ach", "bacs", "eft", "international"]
-
-    class Config:
-        allow_population_by_field_name = True
-        validate_assignment = True
-
-    def to_str(self) -> str:
-        """Returns the string representation of the model using alias"""
-        return pprint.pformat(self.dict(by_alias=True))
-
-    def to_json(self) -> str:
-        """Returns the JSON representation of the model using alias"""
-        return json.dumps(self.to_dict())
-
-    @classmethod
-    def from_json(cls, json_str: str) -> Numbers:
-        """Create an instance of Numbers from a JSON string"""
-        return cls.from_dict(json.loads(json_str))
-
-    def to_dict(self):
-        """Returns the dictionary representation of the model using alias"""
-        _dict = self.dict(by_alias=True, exclude={}, exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of each item in ach (list)
-        _items = []
-        if self.ach:
-            for _item in self.ach:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict["ach"] = _items
-        # override the default output from pydantic by calling `to_dict()` of each item in bacs (list)
-        _items = []
-        if self.bacs:
-            for _item in self.bacs:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict["bacs"] = _items
-        # override the default output from pydantic by calling `to_dict()` of each item in eft (list)
-        _items = []
-        if self.eft:
-            for _item in self.eft:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict["eft"] = _items
-        # override the default output from pydantic by calling `to_dict()` of each item in international (list)
-        _items = []
-        if self.international:
-            for _item in self.international:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict["international"] = _items
-        return _dict
-
-    @classmethod
-    def from_dict(cls, obj: dict) -> Numbers:
-        """Create an instance of Numbers from a dict"""
-        if obj is None:
-            return None
-
-        if type(obj) is not dict:
-            return Numbers.parse_obj(obj)
-
-        _obj = Numbers.parse_obj(
-            {
-                "ach": [AchNumber.from_dict(_item) for _item in obj.get("ach")] if obj.get("ach") is not None else None,
-                "bacs": [BacsNumber.from_dict(_item) for _item in obj.get("bacs")]
-                if obj.get("bacs") is not None
-                else None,
-                "eft": [EftNumber.from_dict(_item) for _item in obj.get("eft")] if obj.get("eft") is not None else None,
-                "international": [InternationalNumber.from_dict(_item) for _item in obj.get("international")]
-                if obj.get("international") is not None
-                else None,
+    class MetaOapg:
+        required = {
+            "links",
+        }
+
+        class properties:
+            class links(schemas.DictSchema):
+                class MetaOapg:
+                    @staticmethod
+                    def additional_properties() -> typing.Type["AccountGroup"]:
+                        return AccountGroup
+
+                def __getitem__(self, name: typing.Union[str,]) -> "AccountGroup":
+                    # dict_instance[name] accessor
+                    return super().__getitem__(name)
+
+                def get_item_oapg(self, name: typing.Union[str,]) -> "AccountGroup":
+                    return super().get_item_oapg(name)
+
+                def __new__(
+                    cls,
+                    *_args: typing.Union[
+                        dict,
+                        frozendict.frozendict,
+                    ],
+                    _configuration: typing.Optional[schemas.Configuration] = None,
+                    **kwargs: "AccountGroup",
+                ) -> "links":
+                    return super().__new__(
+                        cls,
+                        *_args,
+                        _configuration=_configuration,
+                        **kwargs,
+                    )
+
+            __annotations__ = {
+                "links": links,
             }
+
+    links: MetaOapg.properties.links
+
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["links"]) -> MetaOapg.properties.links:
+        ...
+
+    @typing.overload
+    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema:
+        ...
+
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["links",], str]):
+        # dict_instance[name] accessor
+        return super().__getitem__(name)
+
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["links"]) -> MetaOapg.properties.links:
+        ...
+
+    @typing.overload
+    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]:
+        ...
+
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["links",], str]):
+        return super().get_item_oapg(name)
+
+    def __new__(
+        cls,
+        *_args: typing.Union[
+            dict,
+            frozendict.frozendict,
+        ],
+        links: typing.Union[
+            MetaOapg.properties.links,
+            dict,
+            frozendict.frozendict,
+        ],
+        _configuration: typing.Optional[schemas.Configuration] = None,
+        **kwargs: typing.Union[
+            schemas.AnyTypeSchema,
+            dict,
+            frozendict.frozendict,
+            str,
+            date,
+            datetime,
+            uuid.UUID,
+            int,
+            float,
+            decimal.Decimal,
+            None,
+            list,
+            tuple,
+            bytes,
+        ],
+    ) -> "GetUserAccountsResponse":
+        return super().__new__(
+            cls,
+            *_args,
+            links=links,
+            _configuration=_configuration,
+            **kwargs,
         )
-        return _obj
+
+
+from moneykit.model.account_group import AccountGroup
```

### Comparing `moneykit-0.0.6/moneykit/models/phone_number_type.py` & `moneykit-0.0.7/moneykit/apis/tags/link_session_api.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,30 +2,25 @@
 
 """
     MoneyKit API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
+    Generated by: https://openapi-generator.tech
 """
 
+from moneykit.paths.link_session.post import CreateLinkSession
+from moneykit.paths.link_session_exchange_token.post import ExchangeToken
 
-import re  # noqa: F401
 
-from aenum import Enum
+class LinkSessionApi(
+    CreateLinkSession,
+    ExchangeToken,
+):
+    """NOTE: This class is auto generated by OpenAPI Generator
+    Ref: https://openapi-generator.tech
 
-
-class PhoneNumberType(str, Enum):
-    """
-    An enumeration.
+    Do not edit the class manually.
     """
 
-    """
-    allowed enum values
-    """
-    HOME = "home"
-    WORK = "work"
-    MOBILE = "mobile"
-    OTHER = "other"
+    pass
```

### Comparing `moneykit-0.0.6/moneykit/models/provider.py` & `moneykit-0.0.7/moneykit/apis/tags/identity_api.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,31 +2,23 @@
 
 """
     MoneyKit API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
+    Generated by: https://openapi-generator.tech
 """
 
+from moneykit.paths.links_id_identity.get import GetIdentities
 
-import re  # noqa: F401
 
-from aenum import Enum
+class IdentityApi(
+    GetIdentities,
+):
+    """NOTE: This class is auto generated by OpenAPI Generator
+    Ref: https://openapi-generator.tech
 
-
-class Provider(str, Enum):
-    """
-    An enumeration.
+    Do not edit the class manually.
     """
 
-    """
-    allowed enum values
-    """
-    MONEYKIT = "moneykit"
-    FINICITY = "finicity"
-    PLAID = "plaid"
-    YODLEE = "yodlee"
-    MX = "mx"
+    pass
```

### Comparing `moneykit-0.0.6/moneykit/models/token.py` & `moneykit-0.0.7/moneykit/model/create_link_session_response.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,71 +2,106 @@
 
 """
     MoneyKit API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
+    Generated by: https://openapi-generator.tech
 """
 
+import decimal  # noqa: F401
+import functools  # noqa: F401
+import io  # noqa: F401
+import re  # noqa: F401
+import typing  # noqa: F401
+import uuid  # noqa: F401
+from datetime import date, datetime  # noqa: F401
 
-from __future__ import annotations
+import frozendict  # noqa: F401
+import typing_extensions  # noqa: F401
 
-import json
-import pprint
-import re  # noqa: F401
+from moneykit import schemas  # noqa: F401
 
-from pydantic import BaseModel, Field, StrictInt, StrictStr
 
+class CreateLinkSessionResponse(schemas.DictSchema):
+    """NOTE: This class is auto generated by OpenAPI Generator.
+    Ref: https://openapi-generator.tech
 
-class Token(BaseModel):
-    """
-    MoneyKit API access token.
+    Do not edit the class manually.
     """
 
-    access_token: StrictStr = Field(..., description="Short-lived access token.")
-    token_type: StrictStr = Field(..., description='Always "bearer".')
-    expires_in: StrictInt = Field(..., description="How long until `access_token` expires in seconds.")
-    __properties = ["access_token", "token_type", "expires_in"]
-
-    class Config:
-        allow_population_by_field_name = True
-        validate_assignment = True
-
-    def to_str(self) -> str:
-        """Returns the string representation of the model using alias"""
-        return pprint.pformat(self.dict(by_alias=True))
-
-    def to_json(self) -> str:
-        """Returns the JSON representation of the model using alias"""
-        return json.dumps(self.to_dict())
-
-    @classmethod
-    def from_json(cls, json_str: str) -> Token:
-        """Create an instance of Token from a JSON string"""
-        return cls.from_dict(json.loads(json_str))
-
-    def to_dict(self):
-        """Returns the dictionary representation of the model using alias"""
-        _dict = self.dict(by_alias=True, exclude={}, exclude_none=True)
-        return _dict
-
-    @classmethod
-    def from_dict(cls, obj: dict) -> Token:
-        """Create an instance of Token from a dict"""
-        if obj is None:
-            return None
-
-        if type(obj) is not dict:
-            return Token.parse_obj(obj)
-
-        _obj = Token.parse_obj(
-            {
-                "access_token": obj.get("access_token"),
-                "token_type": obj.get("token_type"),
-                "expires_in": obj.get("expires_in"),
+    class MetaOapg:
+        required = {
+            "link_session_token",
+        }
+
+        class properties:
+            link_session_token = schemas.StrSchema
+            __annotations__ = {
+                "link_session_token": link_session_token,
             }
+
+    link_session_token: MetaOapg.properties.link_session_token
+
+    @typing.overload
+    def __getitem__(
+        self, name: typing_extensions.Literal["link_session_token"]
+    ) -> MetaOapg.properties.link_session_token:
+        ...
+
+    @typing.overload
+    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema:
+        ...
+
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["link_session_token",], str]):
+        # dict_instance[name] accessor
+        return super().__getitem__(name)
+
+    @typing.overload
+    def get_item_oapg(
+        self, name: typing_extensions.Literal["link_session_token"]
+    ) -> MetaOapg.properties.link_session_token:
+        ...
+
+    @typing.overload
+    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]:
+        ...
+
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["link_session_token",], str]):
+        return super().get_item_oapg(name)
+
+    def __new__(
+        cls,
+        *_args: typing.Union[
+            dict,
+            frozendict.frozendict,
+        ],
+        link_session_token: typing.Union[
+            MetaOapg.properties.link_session_token,
+            str,
+        ],
+        _configuration: typing.Optional[schemas.Configuration] = None,
+        **kwargs: typing.Union[
+            schemas.AnyTypeSchema,
+            dict,
+            frozendict.frozendict,
+            str,
+            date,
+            datetime,
+            uuid.UUID,
+            int,
+            float,
+            decimal.Decimal,
+            None,
+            list,
+            tuple,
+            bytes,
+        ],
+    ) -> "CreateLinkSessionResponse":
+        return super().__new__(
+            cls,
+            *_args,
+            link_session_token=link_session_token,
+            _configuration=_configuration,
+            **kwargs,
         )
-        return _obj
```

### Comparing `moneykit-0.0.6/moneykit/models/transaction_type.py` & `moneykit-0.0.7/moneykit/model/transaction_type_filter.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,28 +2,46 @@
 
 """
     MoneyKit API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
-    Generated by OpenAPI Generator (https://openapi-generator.tech)
-
-    Do not edit the class manually.
+    Generated by: https://openapi-generator.tech
 """
 
-
+import decimal  # noqa: F401
+import functools  # noqa: F401
+import io  # noqa: F401
 import re  # noqa: F401
+import typing  # noqa: F401
+import uuid  # noqa: F401
+from datetime import date, datetime  # noqa: F401
 
-from aenum import Enum
+import frozendict  # noqa: F401
+import typing_extensions  # noqa: F401
 
+from moneykit import schemas  # noqa: F401
+
+
+class TransactionTypeFilter(schemas.EnumBase, schemas.StrSchema):
+    """NOTE: This class is auto generated by OpenAPI Generator.
+    Ref: https://openapi-generator.tech
+
+    Do not edit the class manually.
 
-class TransactionType(str, Enum):
-    """
     An enumeration.
     """
 
-    """
-    allowed enum values
-    """
-    CREDIT = "credit"
-    DEBIT = "debit"
+    class MetaOapg:
+        enum_value_to_name = {
+            "credit": "CREDIT",
+            "debit": "DEBIT",
+        }
+
+    @schemas.classproperty
+    def CREDIT(cls):
+        return cls("credit")
+
+    @schemas.classproperty
+    def DEBIT(cls):
+        return cls("debit")
```

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/__init__.py` & `moneykit-0.0.7/moneykit/plaid_compatible/__init__.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/api/plaid_api.py` & `moneykit-0.0.7/moneykit/plaid_compatible/api/plaid_api.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/api_client.py` & `moneykit-0.0.7/moneykit/plaid_compatible/api_client.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/configuration.py` & `moneykit-0.0.7/moneykit/plaid_compatible/configuration.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/exceptions.py` & `moneykit-0.0.7/moneykit/exceptions.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,30 @@
+# coding: utf-8
+
 """
     MoneyKit API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
+import dataclasses
+import typing
 
+from urllib3._collections import HTTPHeaderDict
 
 
 class OpenApiException(Exception):
     """The base exception class for all OpenAPIExceptions"""
 
 
 class ApiTypeError(OpenApiException, TypeError):
-    def __init__(self, msg, path_to_item=None, valid_classes=None,
-                 key_type=None):
-        """ Raises an exception for TypeErrors
+    def __init__(self, msg, path_to_item=None, valid_classes=None, key_type=None):
+        """Raises an exception for TypeErrors
 
         Args:
             msg (str): the exception message
 
         Keyword Args:
             path_to_item (list): a list of keys an indices to get to the
                                  current_item
@@ -92,66 +96,47 @@
         self.path_to_item = path_to_item
         full_msg = msg
         if path_to_item:
             full_msg = "{0} at {1}".format(msg, render_path(path_to_item))
         super(ApiKeyError, self).__init__(full_msg)
 
 
-class ApiException(OpenApiException):
+T = typing.TypeVar("T")
+
 
-    def __init__(self, status=None, reason=None, http_resp=None):
-        if http_resp:
-            self.status = http_resp.status
-            self.reason = http_resp.reason
-            self.body = http_resp.data
-            self.headers = http_resp.getheaders()
-        else:
-            self.status = status
-            self.reason = reason
-            self.body = None
-            self.headers = None
+@dataclasses.dataclass
+class ApiException(OpenApiException, typing.Generic[T]):
+    status: int
+    reason: str
+    api_response: typing.Optional[T] = None
+
+    @property
+    def body(self) -> typing.Union[str, bytes, None]:
+        if not self.api_response:
+            return None
+        return self.api_response.response.data
+
+    @property
+    def headers(self) -> typing.Optional[HTTPHeaderDict]:
+        if not self.api_response:
+            return None
+        return self.api_response.response.getheaders()
 
     def __str__(self):
         """Custom error messages for exception"""
-        error_message = "({0})\n"\
-                        "Reason: {1}\n".format(self.status, self.reason)
+        error_message = "({0})\n" "Reason: {1}\n".format(self.status, self.reason)
         if self.headers:
-            error_message += "HTTP response headers: {0}\n".format(
-                self.headers)
+            error_message += "HTTP response headers: {0}\n".format(self.headers)
 
         if self.body:
             error_message += "HTTP response body: {0}\n".format(self.body)
 
         return error_message
 
 
-class NotFoundException(ApiException):
-
-    def __init__(self, status=None, reason=None, http_resp=None):
-        super(NotFoundException, self).__init__(status, reason, http_resp)
-
-
-class UnauthorizedException(ApiException):
-
-    def __init__(self, status=None, reason=None, http_resp=None):
-        super(UnauthorizedException, self).__init__(status, reason, http_resp)
-
-
-class ForbiddenException(ApiException):
-
-    def __init__(self, status=None, reason=None, http_resp=None):
-        super(ForbiddenException, self).__init__(status, reason, http_resp)
-
-
-class ServiceException(ApiException):
-
-    def __init__(self, status=None, reason=None, http_resp=None):
-        super(ServiceException, self).__init__(status, reason, http_resp)
-
-
 def render_path(path_to_item):
     """Returns a string representation of a path"""
     result = ""
     for pth in path_to_item:
         if isinstance(pth, int):
             result += "[{0}]".format(pth)
         else:
```

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/account_balance.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/account_balance.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/account_base.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/account_base.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/account_identity.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/account_identity.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/account_subtype.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/account_subtype.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/account_type.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/account_type.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/accounts_get_request.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/accounts_get_request.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/accounts_get_request_options.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/accounts_get_request_options.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/accounts_get_response.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/accounts_get_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/address.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/address.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/address_data.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/address_data.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/auth_get_numbers.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/auth_get_numbers.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/auth_get_request.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/auth_get_request.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/auth_get_request_options.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/auth_get_request_options.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/auth_get_response.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/auth_get_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/counterparty_type.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/counterparty_type.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/country_code.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/country_code.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/credit_account_subtype.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/credit_account_subtype.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/credit_filter.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/credit_filter.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/depository_account_subtype.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/depository_account_subtype.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/depository_filter.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/depository_filter.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/email.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/email.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/employment_source_type.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/employment_source_type.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/http_validation_error.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/id_number_type.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/id_number_type.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/identity_get_request.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/identity_get_request.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/identity_get_request_options.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/identity_get_request_options.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/identity_get_response.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/identity_get_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/income_verification_payroll_flow_type.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/income_verification_payroll_flow_type.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/income_verification_source_type.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/income_verification_source_type.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/investment_account_subtype.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/investment_account_subtype.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/investment_filter.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/investment_filter.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/item.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/item.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/item_error_webhook.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/item_error_webhook.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/item_get_request.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/item_get_request.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/item_get_response.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/item_get_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/item_public_token_exchange_request.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/item_public_token_exchange_request.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/item_public_token_exchange_response.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/item_public_token_exchange_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/item_remove_request.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/item_remove_request.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/item_remove_response.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/item_remove_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/item_status_investments.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/item_status_investments.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/item_status_last_webhook.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/item_status_last_webhook.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/item_status_nullable.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/item_status_nullable.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/item_status_transactions.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/item_status_transactions.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/link_token_account_filters.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/link_token_account_filters.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/link_token_create_institution_data.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/link_token_create_institution_data.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/link_token_create_request.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/link_token_create_request.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/link_token_create_request_auth.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/link_token_create_request_auth.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/link_token_create_request_deposit_switch.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/link_token_create_request_deposit_switch.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/link_token_create_request_employment.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/link_token_create_request_employment.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/link_token_create_request_employment_bank_income.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/link_token_create_request_employment_bank_income.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/link_token_create_request_identity_verification.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/link_token_create_request_identity_verification.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/link_token_create_request_income_verification.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/link_token_create_request_income_verification.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/link_token_create_request_income_verification_bank_income.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/link_token_create_request_income_verification_bank_income.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/link_token_create_request_income_verification_payroll_income.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/link_token_create_request_income_verification_payroll_income.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/link_token_create_request_payment_initiation.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/link_token_create_request_payment_initiation.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/link_token_create_request_transfer.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/link_token_create_request_transfer.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/link_token_create_request_update.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/link_token_create_request_update.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/link_token_create_request_user.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/link_token_create_request_user.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/link_token_create_request_user_name.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/link_token_create_request_user_name.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/link_token_create_request_user_stated_income_source.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/link_token_create_request_user_stated_income_source.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/link_token_create_response.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/link_token_create_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/link_token_eu_config.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/link_token_eu_config.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/link_token_investments.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/link_token_investments.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/loan_account_subtype.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/loan_account_subtype.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/loan_filter.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/loan_filter.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/location.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/location.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/money_link_features.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/money_link_features.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/numbers_ach.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/numbers_ach.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/numbers_bacs.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/numbers_bacs.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/numbers_eft.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/numbers_eft.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/numbers_international.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/numbers_international.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/owner.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/owner.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/payment_meta.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/payment_meta.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/personal_finance_category.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/personal_finance_category.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/phone_number.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/phone_number.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/plaid_error.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/plaid_error.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/plaid_error_type.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/plaid_error_type.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/products.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/products.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/removed_transaction.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/removed_transaction.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/transaction.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/transaction.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/transaction_code.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/transaction_code.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/transaction_counterparty.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/transaction_counterparty.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/transactions_get_request.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/transactions_get_request.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/transactions_get_request_options.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/transactions_get_request_options.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/transactions_get_response.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/transactions_get_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/transactions_refresh_request.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/transactions_refresh_request.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/transactions_refresh_response.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/transactions_refresh_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/transactions_sync_request.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/transactions_sync_request.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/transactions_sync_request_options.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/transactions_sync_request_options.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/transactions_sync_response.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/transactions_sync_response.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/user_address.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/user_address.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/user_id_number.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/user_id_number.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/user_stated_income_source_category.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/user_stated_income_source_category.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/user_stated_income_source_frequency.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/user_stated_income_source_frequency.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/user_stated_income_source_pay_type.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/user_stated_income_source_pay_type.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/validation_error.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/validation_error.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model/webhook_environment_values.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model/webhook_environment_values.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/model_utils.py` & `moneykit-0.0.7/moneykit/plaid_compatible/model_utils.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/models/__init__.py` & `moneykit-0.0.7/moneykit/plaid_compatible/models/__init__.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/moneykit/plaid_compatible/rest.py` & `moneykit-0.0.7/moneykit/plaid_compatible/rest.py`

 * *Files identical despite different names*

### Comparing `moneykit-0.0.6/pyproject.toml` & `moneykit-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "moneykit"
-version = "0.0.6"
+version = "0.0.7"
 description = "MoneyKit API SDK"
 authors = ["MoneyKit"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/moneykit/moneykit-python"
 keywords = ["OpenAPI", "OpenAPI-Generator", "MoneyKit"]
```

