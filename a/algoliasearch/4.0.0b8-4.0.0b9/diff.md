# Comparing `tmp/algoliasearch-4.0.0b8.tar.gz` & `tmp/algoliasearch-4.0.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "algoliasearch-4.0.0b8.tar", max compression
+gzip compressed data, was "algoliasearch-4.0.0b9.tar", max compression
```

## Comparing `algoliasearch-4.0.0b8.tar` & `algoliasearch-4.0.0b9.tar`

### file list

```diff
@@ -1,548 +1,551 @@
--rw-r--r--   0        0        0     1071 2024-02-29 16:26:22.677463 algoliasearch-4.0.0b8/LICENSE
--rw-r--r--   0        0        0     3718 2024-02-29 16:26:22.677463 algoliasearch-4.0.0b8/README.md
--rw-r--r--   0        0        0     5988 2024-02-29 16:26:22.677463 algoliasearch-4.0.0b8/algoliasearch/.openapi-generator/FILES
--rw-r--r--   0        0        0        5 2024-02-29 16:26:22.677463 algoliasearch-4.0.0b8/algoliasearch/.openapi-generator/VERSION
--rw-r--r--   0        0        0     1040 2024-02-29 16:26:22.677463 algoliasearch-4.0.0b8/algoliasearch/.openapi-generator-ignore
--rw-r--r--   0        0        0      270 2024-02-29 16:26:22.677463 algoliasearch-4.0.0b8/algoliasearch/__init__.py
--rw-r--r--   0        0        0      270 2024-02-29 16:26:22.677463 algoliasearch-4.0.0b8/algoliasearch/abtesting/__init__.py
--rw-r--r--   0        0        0    30767 2024-02-29 16:26:22.677463 algoliasearch-4.0.0b8/algoliasearch/abtesting/client.py
--rw-r--r--   0        0        0     1547 2024-02-29 16:26:22.677463 algoliasearch-4.0.0b8/algoliasearch/abtesting/config.py
--rw-r--r--   0        0        0      270 2024-02-29 16:26:22.677463 algoliasearch-4.0.0b8/algoliasearch/abtesting/models/__init__.py
--rw-r--r--   0        0        0     7051 2024-02-29 16:26:22.677463 algoliasearch-4.0.0b8/algoliasearch/abtesting/models/ab_test.py
--rw-r--r--   0        0        0     2267 2024-02-29 16:26:22.677463 algoliasearch-4.0.0b8/algoliasearch/abtesting/models/ab_test_response.py
--rw-r--r--   0        0        0     2165 2024-02-29 16:26:22.677463 algoliasearch-4.0.0b8/algoliasearch/abtesting/models/ab_tests_variant.py
--rw-r--r--   0        0        0     2375 2024-02-29 16:26:22.677463 algoliasearch-4.0.0b8/algoliasearch/abtesting/models/ab_tests_variant_search_params.py
--rw-r--r--   0        0        0     2653 2024-02-29 16:26:22.677463 algoliasearch-4.0.0b8/algoliasearch/abtesting/models/add_ab_tests_request.py
--rw-r--r--   0        0        0     3359 2024-02-29 16:26:22.677463 algoliasearch-4.0.0b8/algoliasearch/abtesting/models/add_ab_tests_variant.py
--rw-r--r--   0        0        0     2470 2024-02-29 16:26:22.677463 algoliasearch-4.0.0b8/algoliasearch/abtesting/models/currencies_value.py
--rw-r--r--   0        0        0     2029 2024-02-29 16:26:22.677463 algoliasearch-4.0.0b8/algoliasearch/abtesting/models/custom_search_params.py
--rw-r--r--   0        0        0     2376 2024-02-29 16:26:22.677463 algoliasearch-4.0.0b8/algoliasearch/abtesting/models/error_base.py
--rw-r--r--   0        0        0     2627 2024-02-29 16:26:22.677463 algoliasearch-4.0.0b8/algoliasearch/abtesting/models/filter_effects.py
--rw-r--r--   0        0        0     2281 2024-02-29 16:26:22.677463 algoliasearch-4.0.0b8/algoliasearch/abtesting/models/filter_effects_empty_search.py
--rw-r--r--   0        0        0     2266 2024-02-29 16:26:22.677463 algoliasearch-4.0.0b8/algoliasearch/abtesting/models/filter_effects_outliers.py
--rw-r--r--   0        0        0     2659 2024-02-29 16:26:22.677463 algoliasearch-4.0.0b8/algoliasearch/abtesting/models/list_ab_tests_response.py
--rw-r--r--   0        0        0     9910 2024-02-29 16:26:22.677463 algoliasearch-4.0.0b8/algoliasearch/abtesting/models/variant.py
--rw-r--r--   0        0        0      270 2024-02-29 16:26:22.677463 algoliasearch-4.0.0b8/algoliasearch/analytics/__init__.py
--rw-r--r--   0        0        0   129977 2024-02-29 16:26:22.677463 algoliasearch-4.0.0b8/algoliasearch/analytics/client.py
--rw-r--r--   0        0        0     1547 2024-02-29 16:26:22.677463 algoliasearch-4.0.0b8/algoliasearch/analytics/config.py
--rw-r--r--   0        0        0      270 2024-02-29 16:26:22.677463 algoliasearch-4.0.0b8/algoliasearch/analytics/models/__init__.py
--rw-r--r--   0        0        0     2208 2024-02-29 16:26:22.677463 algoliasearch-4.0.0b8/algoliasearch/analytics/models/average_click_event.py
--rw-r--r--   0        0        0     2154 2024-02-29 16:26:22.677463 algoliasearch-4.0.0b8/algoliasearch/analytics/models/click_position.py
--rw-r--r--   0        0        0     3004 2024-02-29 16:26:22.677463 algoliasearch-4.0.0b8/algoliasearch/analytics/models/click_through_rate_event.py
--rw-r--r--   0        0        0     3020 2024-02-29 16:26:22.677463 algoliasearch-4.0.0b8/algoliasearch/analytics/models/conversion_rate_event.py
--rw-r--r--   0        0        0      608 2024-02-29 16:26:22.677463 algoliasearch-4.0.0b8/algoliasearch/analytics/models/direction.py
--rw-r--r--   0        0        0     2376 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/analytics/models/error_base.py
--rw-r--r--   0        0        0     2662 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/analytics/models/get_average_click_position_response.py
--rw-r--r--   0        0        0     2357 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/analytics/models/get_click_positions_response.py
--rw-r--r--   0        0        0     3454 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/analytics/models/get_click_through_rate_response.py
--rw-r--r--   0        0        0     3452 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/analytics/models/get_conversation_rate_response.py
--rw-r--r--   0        0        0     2967 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/analytics/models/get_no_click_rate_response.py
--rw-r--r--   0        0        0     2986 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/analytics/models/get_no_results_rate_response.py
--rw-r--r--   0        0        0     2385 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/analytics/models/get_searches_count_response.py
--rw-r--r--   0        0        0     2317 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/analytics/models/get_searches_no_clicks_response.py
--rw-r--r--   0        0        0     2346 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/analytics/models/get_searches_no_results_response.py
--rw-r--r--   0        0        0     1871 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/analytics/models/get_status_response.py
--rw-r--r--   0        0        0     2259 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/analytics/models/get_top_countries_response.py
--rw-r--r--   0        0        0     1899 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/analytics/models/get_top_filter_attribute.py
--rw-r--r--   0        0        0     2396 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/analytics/models/get_top_filter_attributes_response.py
--rw-r--r--   0        0        0     2168 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/analytics/models/get_top_filter_for_attribute.py
--rw-r--r--   0        0        0     2398 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/analytics/models/get_top_filter_for_attribute_response.py
--rw-r--r--   0        0        0     2400 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/analytics/models/get_top_filters_no_results_response.py
--rw-r--r--   0        0        0     2059 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/analytics/models/get_top_filters_no_results_value.py
--rw-r--r--   0        0        0     2510 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/analytics/models/get_top_filters_no_results_values.py
--rw-r--r--   0        0        0     3397 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/analytics/models/get_top_hits_response.py
--rw-r--r--   0        0        0     3495 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/analytics/models/get_top_searches_response.py
--rw-r--r--   0        0        0     2318 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/analytics/models/get_users_count_response.py
--rw-r--r--   0        0        0     2580 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/analytics/models/no_click_rate_event.py
--rw-r--r--   0        0        0     2590 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/analytics/models/no_results_rate_event.py
--rw-r--r--   0        0        0      879 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/analytics/models/order_by.py
--rw-r--r--   0        0        0     1882 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/analytics/models/search_event.py
--rw-r--r--   0        0        0     2102 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/analytics/models/search_no_click_event.py
--rw-r--r--   0        0        0     2087 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/analytics/models/search_no_result_event.py
--rw-r--r--   0        0        0     1842 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/analytics/models/top_country.py
--rw-r--r--   0        0        0     1788 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/analytics/models/top_hit.py
--rw-r--r--   0        0        0     3597 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/analytics/models/top_hit_with_analytics.py
--rw-r--r--   0        0        0     2138 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/analytics/models/top_hits_response.py
--rw-r--r--   0        0        0     2282 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/analytics/models/top_hits_response_with_analytics.py
--rw-r--r--   0        0        0     2134 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/analytics/models/top_search.py
--rw-r--r--   0        0        0     4192 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/analytics/models/top_search_with_analytics.py
--rw-r--r--   0        0        0     2258 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/analytics/models/top_searches_response.py
--rw-r--r--   0        0        0     2421 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/analytics/models/top_searches_response_with_analytics.py
--rw-r--r--   0        0        0     1886 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/analytics/models/user_with_date.py
--rw-r--r--   0        0        0      270 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/http/__init__.py
--rw-r--r--   0        0        0     2770 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/http/api_response.py
--rw-r--r--   0        0        0     1062 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/http/base_config.py
--rw-r--r--   0        0        0     4756 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/http/exceptions.py
--rw-r--r--   0        0        0     1228 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/http/helpers.py
--rw-r--r--   0        0        0     1244 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/http/hosts.py
--rw-r--r--   0        0        0     2945 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/http/request_options.py
--rw-r--r--   0        0        0     1461 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/http/retry.py
--rw-r--r--   0        0        0     1811 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/http/serializer.py
--rw-r--r--   0        0        0     5911 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/http/transporter.py
--rw-r--r--   0        0        0      497 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/http/user_agent.py
--rw-r--r--   0        0        0      104 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/http/verb.py
--rw-r--r--   0        0        0      270 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/ingestion/__init__.py
--rw-r--r--   0        0        0   124701 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/ingestion/client.py
--rw-r--r--   0        0        0     1409 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/ingestion/config.py
--rw-r--r--   0        0        0      270 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/__init__.py
--rw-r--r--   0        0        0      676 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/action_type.py
--rw-r--r--   0        0        0     1962 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/auth_algolia.py
--rw-r--r--   0        0        0     2070 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/auth_algolia_partial.py
--rw-r--r--   0        0        0     1702 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/auth_api_key.py
--rw-r--r--   0        0        0     1750 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/auth_api_key_partial.py
--rw-r--r--   0        0        0     1809 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/auth_basic.py
--rw-r--r--   0        0        0     1874 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/auth_basic_partial.py
--rw-r--r--   0        0        0     2071 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/auth_google_service_account.py
--rw-r--r--   0        0        0     2184 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/auth_google_service_account_partial.py
--rw-r--r--   0        0        0     4409 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/auth_input.py
--rw-r--r--   0        0        0     4852 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/auth_input_partial.py
--rw-r--r--   0        0        0     2031 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/auth_o_auth.py
--rw-r--r--   0        0        0     2148 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/auth_o_auth_partial.py
--rw-r--r--   0        0        0     3306 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/authentication.py
--rw-r--r--   0        0        0     2684 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/authentication_create.py
--rw-r--r--   0        0        0     2264 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/authentication_create_response.py
--rw-r--r--   0        0        0     1868 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/authentication_search.py
--rw-r--r--   0        0        0      765 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/authentication_sort_keys.py
--rw-r--r--   0        0        0      798 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/authentication_type.py
--rw-r--r--   0        0        0     2787 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/authentication_update.py
--rw-r--r--   0        0        0     2267 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/authentication_update_response.py
--rw-r--r--   0        0        0     2063 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/big_commerce_channel.py
--rw-r--r--   0        0        0     1908 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/big_commerce_metafield.py
--rw-r--r--   0        0        0      631 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/big_query_data_type.py
--rw-r--r--   0        0        0     2955 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/commercetools_custom_fields.py
--rw-r--r--   0        0        0     1797 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/delete_response.py
--rw-r--r--   0        0        0     3095 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/destination.py
--rw-r--r--   0        0        0     2535 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/destination_create.py
--rw-r--r--   0        0        0     2237 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/destination_create_response.py
--rw-r--r--   0        0        0     2703 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/destination_index_name.py
--rw-r--r--   0        0        0     1838 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/destination_index_prefix.py
--rw-r--r--   0        0        0     3382 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/destination_input.py
--rw-r--r--   0        0        0     1841 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/destination_search.py
--rw-r--r--   0        0        0      720 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/destination_sort_keys.py
--rw-r--r--   0        0        0      725 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/destination_type.py
--rw-r--r--   0        0        0     2609 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/destination_update.py
--rw-r--r--   0        0        0     2240 2024-02-29 16:26:22.681463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/destination_update_response.py
--rw-r--r--   0        0        0      667 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/docker_image_type.py
--rw-r--r--   0        0        0      660 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/docker_registry.py
--rw-r--r--   0        0        0     1944 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/docker_source_discover.py
--rw-r--r--   0        0        0     1718 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/docker_source_streams.py
--rw-r--r--   0        0        0     2376 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/error_base.py
--rw-r--r--   0        0        0     2905 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/event.py
--rw-r--r--   0        0        0      682 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/event_sort_keys.py
--rw-r--r--   0        0        0      728 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/event_status.py
--rw-r--r--   0        0        0      660 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/event_type.py
--rw-r--r--   0        0        0     2647 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/list_authentications_response.py
--rw-r--r--   0        0        0     2582 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/list_destinations_response.py
--rw-r--r--   0        0        0     2744 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/list_events_response.py
--rw-r--r--   0        0        0     2469 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/list_sources_response.py
--rw-r--r--   0        0        0     2462 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/list_tasks_response.py
--rw-r--r--   0        0        0      697 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/mapping_type_csv.py
--rw-r--r--   0        0        0      611 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/method_type.py
--rw-r--r--   0        0        0     2134 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/on_demand_date_utils_input.py
--rw-r--r--   0        0        0     2066 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/on_demand_trigger.py
--rw-r--r--   0        0        0     1826 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/on_demand_trigger_input.py
--rw-r--r--   0        0        0      671 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/on_demand_trigger_type.py
--rw-r--r--   0        0        0      630 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/order_keys.py
--rw-r--r--   0        0        0     2036 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/pagination.py
--rw-r--r--   0        0        0      686 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/platform.py
--rw-r--r--   0        0        0      645 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/platform_none.py
--rw-r--r--   0        0        0     3187 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/platform_with_none.py
--rw-r--r--   0        0        0      685 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/record_type.py
--rw-r--r--   0        0        0     4007 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/run.py
--rw-r--r--   0        0        0     2710 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/run_list_response.py
--rw-r--r--   0        0        0      655 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/run_outcome.py
--rw-r--r--   0        0        0     2040 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/run_progress.py
--rw-r--r--   0        0        0      810 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/run_reason_code.py
--rw-r--r--   0        0        0     1999 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/run_response.py
--rw-r--r--   0        0        0      682 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/run_sort_keys.py
--rw-r--r--   0        0        0      692 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/run_status.py
--rw-r--r--   0        0        0      640 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/run_type.py
--rw-r--r--   0        0        0     1978 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/schedule_date_utils_input.py
--rw-r--r--   0        0        0     2472 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/schedule_trigger.py
--rw-r--r--   0        0        0     1994 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/schedule_trigger_input.py
--rw-r--r--   0        0        0      669 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/schedule_trigger_type.py
--rw-r--r--   0        0        0     2876 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/source.py
--rw-r--r--   0        0        0     3755 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/source_big_commerce.py
--rw-r--r--   0        0        0     3154 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/source_big_query.py
--rw-r--r--   0        0        0     3161 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/source_commercetools.py
--rw-r--r--   0        0        0     2388 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/source_create.py
--rw-r--r--   0        0        0     2067 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/source_create_response.py
--rw-r--r--   0        0        0     2908 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/source_csv.py
--rw-r--r--   0        0        0     2468 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/source_docker.py
--rw-r--r--   0        0        0     4991 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/source_input.py
--rw-r--r--   0        0        0     2208 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/source_json.py
--rw-r--r--   0        0        0     1737 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/source_search.py
--rw-r--r--   0        0        0      705 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/source_sort_keys.py
--rw-r--r--   0        0        0      727 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/source_type.py
--rw-r--r--   0        0        0     2319 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/source_update.py
--rw-r--r--   0        0        0     3190 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/source_update_commercetools.py
--rw-r--r--   0        0        0     2360 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/source_update_docker.py
--rw-r--r--   0        0        0     4665 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/source_update_input.py
--rw-r--r--   0        0        0     2070 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/source_update_response.py
--rw-r--r--   0        0        0     1842 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/subscription_trigger.py
--rw-r--r--   0        0        0      696 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/subscription_trigger_type.py
--rw-r--r--   0        0        0     3713 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/task.py
--rw-r--r--   0        0        0     3337 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/task_create.py
--rw-r--r--   0        0        0     1971 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/task_create_response.py
--rw-r--r--   0        0        0     3805 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/task_create_trigger.py
--rw-r--r--   0        0        0     3387 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/task_input.py
--rw-r--r--   0        0        0     1721 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/task_search.py
--rw-r--r--   0        0        0      741 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/task_sort_keys.py
--rw-r--r--   0        0        0     3114 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/task_update.py
--rw-r--r--   0        0        0     1972 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/task_update_response.py
--rw-r--r--   0        0        0     3689 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/trigger.py
--rw-r--r--   0        0        0      929 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/trigger_type.py
--rw-r--r--   0        0        0     1835 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/trigger_update_input.py
--rw-r--r--   0        0        0     2158 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/ingestion/models/window.py
--rw-r--r--   0        0        0      270 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/insights/__init__.py
--rw-r--r--   0        0        0    22116 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/insights/client.py
--rw-r--r--   0        0        0     1541 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/insights/config.py
--rw-r--r--   0        0        0      270 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/insights/models/__init__.py
--rw-r--r--   0        0        0      617 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/insights/models/add_to_cart_event.py
--rw-r--r--   0        0        0     6815 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/insights/models/added_to_cart_object_ids.py
--rw-r--r--   0        0        0     7492 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/insights/models/added_to_cart_object_ids_after_search.py
--rw-r--r--   0        0        0      597 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/insights/models/click_event.py
--rw-r--r--   0        0        0     5013 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/insights/models/clicked_filters.py
--rw-r--r--   0        0        0     5218 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/insights/models/clicked_object_ids.py
--rw-r--r--   0        0        0     6196 2024-02-29 16:26:22.685463 algoliasearch-4.0.0b8/algoliasearch/insights/models/clicked_object_ids_after_search.py
--rw-r--r--   0        0        0      622 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/insights/models/conversion_event.py
--rw-r--r--   0        0        0     4972 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/insights/models/converted_filters.py
--rw-r--r--   0        0        0     5251 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/insights/models/converted_object_ids.py
--rw-r--r--   0        0        0     6007 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/insights/models/converted_object_ids_after_search.py
--rw-r--r--   0        0        0     3286 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/insights/models/discount.py
--rw-r--r--   0        0        0     2376 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/insights/models/error_base.py
--rw-r--r--   0        0        0     8136 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/insights/models/events_items.py
--rw-r--r--   0        0        0     2024 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/insights/models/events_response.py
--rw-r--r--   0        0        0     2494 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/insights/models/insights_events.py
--rw-r--r--   0        0        0     2624 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/insights/models/object_data.py
--rw-r--r--   0        0        0     3425 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/insights/models/object_data_after_search.py
--rw-r--r--   0        0        0     3282 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/insights/models/price.py
--rw-r--r--   0        0        0      612 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/insights/models/purchase_event.py
--rw-r--r--   0        0        0     6780 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/insights/models/purchased_object_ids.py
--rw-r--r--   0        0        0     6759 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/insights/models/purchased_object_ids_after_search.py
--rw-r--r--   0        0        0     3262 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/insights/models/value.py
--rw-r--r--   0        0        0      592 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/insights/models/view_event.py
--rw-r--r--   0        0        0     5069 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/insights/models/viewed_filters.py
--rw-r--r--   0        0        0     5008 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/insights/models/viewed_object_ids.py
--rw-r--r--   0        0        0      270 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/monitoring/__init__.py
--rw-r--r--   0        0        0    38131 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/monitoring/client.py
--rw-r--r--   0        0        0     1085 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/monitoring/config.py
--rw-r--r--   0        0        0      270 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/monitoring/models/__init__.py
--rw-r--r--   0        0        0     2376 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/monitoring/models/error_base.py
--rw-r--r--   0        0        0     1752 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/monitoring/models/get_inventory403_response.py
--rw-r--r--   0        0        0     1924 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/monitoring/models/incident.py
--rw-r--r--   0        0        0     2182 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/monitoring/models/incidents_inner.py
--rw-r--r--   0        0        0     2526 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/monitoring/models/incidents_response.py
--rw-r--r--   0        0        0     2109 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/monitoring/models/indexing_time_response.py
--rw-r--r--   0        0        0     2538 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/monitoring/models/indexing_time_response_metrics.py
--rw-r--r--   0        0        0     2124 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/monitoring/models/infrastructure_response.py
--rw-r--r--   0        0        0     6267 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/monitoring/models/infrastructure_response_metrics.py
--rw-r--r--   0        0        0     2168 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/monitoring/models/inventory_response.py
--rw-r--r--   0        0        0     2068 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/monitoring/models/latency_response.py
--rw-r--r--   0        0        0     2510 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/monitoring/models/latency_response_metrics.py
--rw-r--r--   0        0        0      762 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/monitoring/models/metric.py
--rw-r--r--   0        0        0      659 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/monitoring/models/period.py
--rw-r--r--   0        0        0     1943 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/monitoring/models/probes_metric.py
--rw-r--r--   0        0        0      817 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/monitoring/models/region.py
--rw-r--r--   0        0        0     2886 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/monitoring/models/server.py
--rw-r--r--   0        0        0      613 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/monitoring/models/server_status.py
--rw-r--r--   0        0        0      735 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/monitoring/models/status.py
--rw-r--r--   0        0        0     1831 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/monitoring/models/status_response.py
--rw-r--r--   0        0        0     1922 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/monitoring/models/time_inner.py
--rw-r--r--   0        0        0      583 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/monitoring/models/type.py
--rw-r--r--   0        0        0      270 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/personalization/__init__.py
--rw-r--r--   0        0        0    28661 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/personalization/client.py
--rw-r--r--   0        0        0     1432 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/personalization/config.py
--rw-r--r--   0        0        0      270 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/personalization/models/__init__.py
--rw-r--r--   0        0        0     2227 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/personalization/models/delete_user_profile_response.py
--rw-r--r--   0        0        0     2376 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/personalization/models/error_base.py
--rw-r--r--   0        0        0     2109 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/personalization/models/event_scoring.py
--rw-r--r--   0        0        0     1906 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/personalization/models/facet_scoring.py
--rw-r--r--   0        0        0     2233 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/personalization/models/get_user_token_response.py
--rw-r--r--   0        0        0     3371 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/personalization/models/personalization_strategy_params.py
--rw-r--r--   0        0        0     1844 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/personalization/models/set_personalization_strategy_response.py
--rw-r--r--   0        0        0        0 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/py.typed
--rw-r--r--   0        0        0      270 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/query_suggestions/__init__.py
--rw-r--r--   0        0        0    34436 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/query_suggestions/client.py
--rw-r--r--   0        0        0     1436 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/query_suggestions/config.py
--rw-r--r--   0        0        0      270 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/query_suggestions/models/__init__.py
--rw-r--r--   0        0        0     2637 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/query_suggestions/models/base_query_suggestions_configuration_response.py
--rw-r--r--   0        0        0     1904 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/query_suggestions/models/base_query_suggestions_configuration_with_index.py
--rw-r--r--   0        0        0     1963 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/query_suggestions/models/base_response.py
--rw-r--r--   0        0        0     2376 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/query_suggestions/models/error_base.py
--rw-r--r--   0        0        0     1926 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/query_suggestions/models/facet.py
--rw-r--r--   0        0        0     3150 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/query_suggestions/models/get_config_status200_response.py
--rw-r--r--   0        0        0     2642 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/query_suggestions/models/get_log_file200_response.py
--rw-r--r--   0        0        0     3301 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/query_suggestions/models/languages.py
--rw-r--r--   0        0        0      903 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/query_suggestions/models/log_level.py
--rw-r--r--   0        0        0     3796 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/query_suggestions/models/query_suggestions_configuration.py
--rw-r--r--   0        0        0     4825 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/query_suggestions/models/query_suggestions_configuration_response.py
--rw-r--r--   0        0        0     3986 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/query_suggestions/models/query_suggestions_configuration_with_index.py
--rw-r--r--   0        0        0     5389 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/query_suggestions/models/source_index.py
--rw-r--r--   0        0        0      270 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/recommend/__init__.py
--rw-r--r--   0        0        0    37789 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/recommend/client.py
--rw-r--r--   0        0        0     1638 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/recommend/config.py
--rw-r--r--   0        0        0      270 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/__init__.py
--rw-r--r--   0        0        0      679 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/advanced_syntax_features.py
--rw-r--r--   0        0        0      728 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/alternatives_as_exact.py
--rw-r--r--   0        0        0      827 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/anchoring.py
--rw-r--r--   0        0        0     3944 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/around_precision.py
--rw-r--r--   0        0        0     1875 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/around_precision_from_value_inner.py
--rw-r--r--   0        0        0     3398 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/around_radius.py
--rw-r--r--   0        0        0      608 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/around_radius_all.py
--rw-r--r--   0        0        0     2350 2024-02-29 16:26:22.689463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/automatic_facet_filter.py
--rw-r--r--   0        0        0     3519 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/automatic_facet_filters.py
--rw-r--r--   0        0        0     2592 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/base_recommend_request.py
--rw-r--r--   0        0        0     3020 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/base_recommendations_query.py
--rw-r--r--   0        0        0     2974 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/base_recommended_for_you_query.py
--rw-r--r--   0        0        0     1981 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/base_recommended_for_you_query_parameters.py
--rw-r--r--   0        0        0    14304 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/base_search_params.py
--rw-r--r--   0        0        0    14197 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/base_search_params_without_query.py
--rw-r--r--   0        0        0    11592 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/base_search_response.py
--rw-r--r--   0        0        0     2023 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/base_trending_facets_query.py
--rw-r--r--   0        0        0     3252 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/base_trending_items_query.py
--rw-r--r--   0        0        0     2381 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/condition.py
--rw-r--r--   0        0        0     4232 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/consequence.py
--rw-r--r--   0        0        0     1813 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/consequence_hide.py
--rw-r--r--   0        0        0    33338 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/consequence_params.py
--rw-r--r--   0        0        0     3437 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/consequence_query.py
--rw-r--r--   0        0        0     2367 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/consequence_query_object.py
--rw-r--r--   0        0        0     2240 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/deleted_at_response.py
--rw-r--r--   0        0        0     3396 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/distinct.py
--rw-r--r--   0        0        0     2190 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/edit.py
--rw-r--r--   0        0        0      622 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/edit_type.py
--rw-r--r--   0        0        0     2376 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/error_base.py
--rw-r--r--   0        0        0      926 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/exact_on_single_word_query.py
--rw-r--r--   0        0        0     3981 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/exhaustive.py
--rw-r--r--   0        0        0     3408 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/facet_filters.py
--rw-r--r--   0        0        0     2657 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/facet_ordering.py
--rw-r--r--   0        0        0     1796 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/facets.py
--rw-r--r--   0        0        0     2386 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/facets_stats.py
--rw-r--r--   0        0        0     1786 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/get_recommend_task_response.py
--rw-r--r--   0        0        0     2404 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/get_recommendations_params.py
--rw-r--r--   0        0        0     2321 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/get_recommendations_response.py
--rw-r--r--   0        0        0     4159 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/highlight_result.py
--rw-r--r--   0        0        0     2567 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/highlight_result_option.py
--rw-r--r--   0        0        0     4005 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/ignore_plurals.py
--rw-r--r--   0        0        0    19465 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/index_settings_as_search_params.py
--rw-r--r--   0        0        0      685 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/match_level.py
--rw-r--r--   0        0        0     2293 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/matched_geo_location.py
--rw-r--r--   0        0        0     3199 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/mixed_search_filters.py
--rw-r--r--   0        0        0      677 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/mode.py
--rw-r--r--   0        0        0     3416 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/numeric_filters.py
--rw-r--r--   0        0        0     3603 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/optional_filters.py
--rw-r--r--   0        0        0     3692 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/params.py
--rw-r--r--   0        0        0     2235 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/personalization.py
--rw-r--r--   0        0        0     3255 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/promote.py
--rw-r--r--   0        0        0     2153 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/promote_object_id.py
--rw-r--r--   0        0        0     2175 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/promote_object_ids.py
--rw-r--r--   0        0        0      846 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/query_type.py
--rw-r--r--   0        0        0     5053 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/ranking_info.py
--rw-r--r--   0        0        0     3555 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/re_ranking_apply_filter.py
--rw-r--r--   0        0        0     5201 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/recommend_hit.py
--rw-r--r--   0        0        0      776 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/recommend_models.py
--rw-r--r--   0        0        0      702 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/recommendation_models.py
--rw-r--r--   0        0        0     3251 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/recommendations_hit.py
--rw-r--r--   0        0        0     2557 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/recommendations_hits.py
--rw-r--r--   0        0        0     3880 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/recommendations_query.py
--rw-r--r--   0        0        0     4383 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/recommendations_request.py
--rw-r--r--   0        0        0    10919 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/recommendations_results.py
--rw-r--r--   0        0        0      677 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/recommended_for_you_model.py
--rw-r--r--   0        0        0     3845 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/recommended_for_you_query.py
--rw-r--r--   0        0        0    32016 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/recommended_for_you_query_parameters.py
--rw-r--r--   0        0        0     2374 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/redirect.py
--rw-r--r--   0        0        0     2607 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/redirect_rule_index_metadata.py
--rw-r--r--   0        0        0     1796 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/redirect_rule_index_metadata_data.py
--rw-r--r--   0        0        0     3937 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/remove_stop_words.py
--rw-r--r--   0        0        0      924 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/remove_words_if_no_results.py
--rw-r--r--   0        0        0     2511 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/rendering_content.py
--rw-r--r--   0        0        0     3881 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/rule_response.py
--rw-r--r--   0        0        0     1929 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/rule_response_metadata.py
--rw-r--r--   0        0        0    31992 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/search_params_object.py
--rw-r--r--   0        0        0     1806 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/search_params_query.py
--rw-r--r--   0        0        0     3111 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/search_recommend_rules_params.py
--rw-r--r--   0        0        0     2717 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/search_recommend_rules_response.py
--rw-r--r--   0        0        0     2290 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/semantic_search.py
--rw-r--r--   0        0        0     4237 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/snippet_result.py
--rw-r--r--   0        0        0     2075 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/snippet_result_option.py
--rw-r--r--   0        0        0      792 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/sort_remaining_by.py
--rw-r--r--   0        0        0     3395 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/tag_filters.py
--rw-r--r--   0        0        0      698 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/task_status.py
--rw-r--r--   0        0        0     2294 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/trending_facet_hit.py
--rw-r--r--   0        0        0      653 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/trending_facets_model.py
--rw-r--r--   0        0        0     2930 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/trending_facets_query.py
--rw-r--r--   0        0        0      648 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/trending_items_model.py
--rw-r--r--   0        0        0     4112 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/trending_items_query.py
--rw-r--r--   0        0        0     3378 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/typo_tolerance.py
--rw-r--r--   0        0        0      636 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/typo_tolerance_enum.py
--rw-r--r--   0        0        0     2026 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/recommend/models/value.py
--rw-r--r--   0        0        0      270 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/search/__init__.py
--rw-r--r--   0        0        0   214867 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/search/client.py
--rw-r--r--   0        0        0     1632 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/search/config.py
--rw-r--r--   0        0        0      270 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/search/models/__init__.py
--rw-r--r--   0        0        0     1856 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/search/models/acl.py
--rw-r--r--   0        0        0      833 2024-02-29 16:26:22.693463 algoliasearch-4.0.0b8/algoliasearch/search/models/action.py
--rw-r--r--   0        0        0     1960 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/add_api_key_response.py
--rw-r--r--   0        0        0      679 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/advanced_syntax_features.py
--rw-r--r--   0        0        0      728 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/alternatives_as_exact.py
--rw-r--r--   0        0        0      827 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/anchoring.py
--rw-r--r--   0        0        0     5481 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/api_key.py
--rw-r--r--   0        0        0      652 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/api_key_operation.py
--rw-r--r--   0        0        0     3941 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/around_precision.py
--rw-r--r--   0        0        0     1875 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/around_precision_from_value_inner.py
--rw-r--r--   0        0        0     3395 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/around_radius.py
--rw-r--r--   0        0        0      608 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/around_radius_all.py
--rw-r--r--   0        0        0     1759 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/assign_user_id_params.py
--rw-r--r--   0        0        0     3317 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/attribute_to_update.py
--rw-r--r--   0        0        0     2350 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/automatic_facet_filter.py
--rw-r--r--   0        0        0     3516 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/automatic_facet_filters.py
--rw-r--r--   0        0        0     2044 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/base_get_api_key_response.py
--rw-r--r--   0        0        0     8818 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/base_index_settings.py
--rw-r--r--   0        0        0    14286 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/base_search_params.py
--rw-r--r--   0        0        0    14179 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/base_search_params_without_query.py
--rw-r--r--   0        0        0    11580 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/base_search_response.py
--rw-r--r--   0        0        0     1902 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/batch_assign_user_ids_params.py
--rw-r--r--   0        0        0     2836 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/batch_dictionary_entries_params.py
--rw-r--r--   0        0        0     2184 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/batch_dictionary_entries_request.py
--rw-r--r--   0        0        0     2228 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/batch_params.py
--rw-r--r--   0        0        0     1892 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/batch_request.py
--rw-r--r--   0        0        0     2158 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/batch_response.py
--rw-r--r--   0        0        0     2190 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/batch_write_params.py
--rw-r--r--   0        0        0     3299 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/browse_params.py
--rw-r--r--   0        0        0    32333 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/browse_params_object.py
--rw-r--r--   0        0        0    11120 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/browse_response.py
--rw-r--r--   0        0        0     2141 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/built_in_operation.py
--rw-r--r--   0        0        0      815 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/built_in_operation_type.py
--rw-r--r--   0        0        0     2378 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/condition.py
--rw-r--r--   0        0        0     4223 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/consequence.py
--rw-r--r--   0        0        0     1813 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/consequence_hide.py
--rw-r--r--   0        0        0    33266 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/consequence_params.py
--rw-r--r--   0        0        0     3425 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/consequence_query.py
--rw-r--r--   0        0        0     2364 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/consequence_query_object.py
--rw-r--r--   0        0        0     1879 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/created_at_response.py
--rw-r--r--   0        0        0     2014 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/cursor.py
--rw-r--r--   0        0        0     1876 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/delete_api_key_response.py
--rw-r--r--   0        0        0     4903 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/delete_by_params.py
--rw-r--r--   0        0        0     1876 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/delete_source_response.py
--rw-r--r--   0        0        0     2240 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/deleted_at_response.py
--rw-r--r--   0        0        0      656 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/dictionary_action.py
--rw-r--r--   0        0        0     4691 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/dictionary_entry.py
--rw-r--r--   0        0        0      721 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/dictionary_entry_state.py
--rw-r--r--   0        0        0     2049 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/dictionary_language.py
--rw-r--r--   0        0        0     2282 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/dictionary_settings_params.py
--rw-r--r--   0        0        0      669 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/dictionary_type.py
--rw-r--r--   0        0        0     3396 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/distinct.py
--rw-r--r--   0        0        0     2187 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/edit.py
--rw-r--r--   0        0        0      622 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/edit_type.py
--rw-r--r--   0        0        0     2376 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/error_base.py
--rw-r--r--   0        0        0      926 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/exact_on_single_word_query.py
--rw-r--r--   0        0        0     3981 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/exhaustive.py
--rw-r--r--   0        0        0     3405 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/facet_filters.py
--rw-r--r--   0        0        0     2343 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/facet_hits.py
--rw-r--r--   0        0        0     2651 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/facet_ordering.py
--rw-r--r--   0        0        0     1796 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/facets.py
--rw-r--r--   0        0        0     2386 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/facets_stats.py
--rw-r--r--   0        0        0     3925 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/fetched_index.py
--rw-r--r--   0        0        0     5876 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/get_api_key_response.py
--rw-r--r--   0        0        0     2251 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/get_dictionary_settings_response.py
--rw-r--r--   0        0        0     2082 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/get_logs_response.py
--rw-r--r--   0        0        0     2213 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/get_objects_params.py
--rw-r--r--   0        0        0     2355 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/get_objects_request.py
--rw-r--r--   0        0        0     1763 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/get_objects_response.py
--rw-r--r--   0        0        0     1747 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/get_task_response.py
--rw-r--r--   0        0        0     1987 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/get_top_user_ids_response.py
--rw-r--r--   0        0        0     2124 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/has_pending_mappings_response.py
--rw-r--r--   0        0        0     4156 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/highlight_result.py
--rw-r--r--   0        0        0     2564 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/highlight_result_option.py
--rw-r--r--   0        0        0     4880 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/hit.py
--rw-r--r--   0        0        0     4005 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/ignore_plurals.py
--rw-r--r--   0        0        0    26249 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/index_settings.py
--rw-r--r--   0        0        0    19417 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/index_settings_as_search_params.py
--rw-r--r--   0        0        0     3244 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/languages.py
--rw-r--r--   0        0        0     2235 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/list_api_keys_response.py
--rw-r--r--   0        0        0     1912 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/list_clusters_response.py
--rw-r--r--   0        0        0     2415 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/list_indices_response.py
--rw-r--r--   0        0        0     2186 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/list_user_ids_response.py
--rw-r--r--   0        0        0     4460 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/log.py
--rw-r--r--   0        0        0     2153 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/log_query.py
--rw-r--r--   0        0        0      644 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/log_type.py
--rw-r--r--   0        0        0      685 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/match_level.py
--rw-r--r--   0        0        0     2293 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/matched_geo_location.py
--rw-r--r--   0        0        0     3199 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/mixed_search_filters.py
--rw-r--r--   0        0        0      677 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/mode.py
--rw-r--r--   0        0        0     2151 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/multiple_batch_request.py
--rw-r--r--   0        0        0     2006 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/multiple_batch_response.py
--rw-r--r--   0        0        0     3413 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/numeric_filters.py
--rw-r--r--   0        0        0     2398 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/operation_index_params.py
--rw-r--r--   0        0        0      649 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/operation_type.py
--rw-r--r--   0        0        0     3600 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/optional_filters.py
--rw-r--r--   0        0        0     3683 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/params.py
--rw-r--r--   0        0        0     2235 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/personalization.py
--rw-r--r--   0        0        0     3249 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/promote.py
--rw-r--r--   0        0        0     2153 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/promote_object_id.py
--rw-r--r--   0        0        0     2175 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/promote_object_ids.py
--rw-r--r--   0        0        0      846 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/query_type.py
--rw-r--r--   0        0        0     5047 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/ranking_info.py
--rw-r--r--   0        0        0     3552 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/re_ranking_apply_filter.py
--rw-r--r--   0        0        0     2371 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/redirect.py
--rw-r--r--   0        0        0     2604 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/redirect_rule_index_metadata.py
--rw-r--r--   0        0        0     1796 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/redirect_rule_index_metadata_data.py
--rw-r--r--   0        0        0     3937 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/remove_stop_words.py
--rw-r--r--   0        0        0     1876 2024-02-29 16:26:22.697463 algoliasearch-4.0.0b8/algoliasearch/search/models/remove_user_id_response.py
--rw-r--r--   0        0        0      924 2024-02-29 16:26:22.701463 algoliasearch-4.0.0b8/algoliasearch/search/models/remove_words_if_no_results.py
--rw-r--r--   0        0        0     2508 2024-02-29 16:26:22.701463 algoliasearch-4.0.0b8/algoliasearch/search/models/rendering_content.py
--rw-r--r--   0        0        0     1887 2024-02-29 16:26:22.701463 algoliasearch-4.0.0b8/algoliasearch/search/models/replace_source_response.py
--rw-r--r--   0        0        0     4129 2024-02-29 16:26:22.701463 algoliasearch-4.0.0b8/algoliasearch/search/models/rule.py
--rw-r--r--   0        0        0     2402 2024-02-29 16:26:22.701463 algoliasearch-4.0.0b8/algoliasearch/search/models/save_object_response.py
--rw-r--r--   0        0        0     2395 2024-02-29 16:26:22.701463 algoliasearch-4.0.0b8/algoliasearch/search/models/save_synonym_response.py
--rw-r--r--   0        0        0      646 2024-02-29 16:26:22.701463 algoliasearch-4.0.0b8/algoliasearch/search/models/scope_type.py
--rw-r--r--   0        0        0     2613 2024-02-29 16:26:22.701463 algoliasearch-4.0.0b8/algoliasearch/search/models/search_dictionary_entries_params.py
--rw-r--r--   0        0        0     2542 2024-02-29 16:26:22.701463 algoliasearch-4.0.0b8/algoliasearch/search/models/search_for_facet_values_request.py
--rw-r--r--   0        0        0     2832 2024-02-29 16:26:22.701463 algoliasearch-4.0.0b8/algoliasearch/search/models/search_for_facet_values_response.py
--rw-r--r--   0        0        0    32686 2024-02-29 16:26:22.701463 algoliasearch-4.0.0b8/algoliasearch/search/models/search_for_facets.py
--rw-r--r--   0        0        0     2727 2024-02-29 16:26:22.701463 algoliasearch-4.0.0b8/algoliasearch/search/models/search_for_facets_options.py
--rw-r--r--   0        0        0    32384 2024-02-29 16:26:22.701463 algoliasearch-4.0.0b8/algoliasearch/search/models/search_for_hits.py
--rw-r--r--   0        0        0     1973 2024-02-29 16:26:22.701463 algoliasearch-4.0.0b8/algoliasearch/search/models/search_for_hits_options.py
--rw-r--r--   0        0        0     3039 2024-02-29 16:26:22.701463 algoliasearch-4.0.0b8/algoliasearch/search/models/search_hits.py
--rw-r--r--   0        0        0     2370 2024-02-29 16:26:22.701463 algoliasearch-4.0.0b8/algoliasearch/search/models/search_method_params.py
--rw-r--r--   0        0        0     3299 2024-02-29 16:26:22.701463 algoliasearch-4.0.0b8/algoliasearch/search/models/search_params.py
--rw-r--r--   0        0        0    31926 2024-02-29 16:26:22.701463 algoliasearch-4.0.0b8/algoliasearch/search/models/search_params_object.py
--rw-r--r--   0        0        0     1806 2024-02-29 16:26:22.701463 algoliasearch-4.0.0b8/algoliasearch/search/models/search_params_query.py
--rw-r--r--   0        0        0     1830 2024-02-29 16:26:22.701463 algoliasearch-4.0.0b8/algoliasearch/search/models/search_params_string.py
--rw-r--r--   0        0        0     3225 2024-02-29 16:26:22.701463 algoliasearch-4.0.0b8/algoliasearch/search/models/search_query.py
--rw-r--r--   0        0        0    12084 2024-02-29 16:26:22.701463 algoliasearch-4.0.0b8/algoliasearch/search/models/search_response.py
--rw-r--r--   0        0        0     2178 2024-02-29 16:26:22.701463 algoliasearch-4.0.0b8/algoliasearch/search/models/search_responses.py
--rw-r--r--   0        0        0     3365 2024-02-29 16:26:22.701463 algoliasearch-4.0.0b8/algoliasearch/search/models/search_result.py
--rw-r--r--   0        0        0     3491 2024-02-29 16:26:22.701463 algoliasearch-4.0.0b8/algoliasearch/search/models/search_rules_params.py
--rw-r--r--   0        0        0     2517 2024-02-29 16:26:22.701463 algoliasearch-4.0.0b8/algoliasearch/search/models/search_rules_response.py
--rw-r--r--   0        0        0      832 2024-02-29 16:26:22.701463 algoliasearch-4.0.0b8/algoliasearch/search/models/search_strategy.py
--rw-r--r--   0        0        0     2438 2024-02-29 16:26:22.701463 algoliasearch-4.0.0b8/algoliasearch/search/models/search_synonyms_params.py
--rw-r--r--   0        0        0     3041 2024-02-29 16:26:22.701463 algoliasearch-4.0.0b8/algoliasearch/search/models/search_synonyms_response.py
--rw-r--r--   0        0        0      781 2024-02-29 16:26:22.701463 algoliasearch-4.0.0b8/algoliasearch/search/models/search_type_default.py
--rw-r--r--   0        0        0      773 2024-02-29 16:26:22.701463 algoliasearch-4.0.0b8/algoliasearch/search/models/search_type_facet.py
--rw-r--r--   0        0        0     2607 2024-02-29 16:26:22.701463 algoliasearch-4.0.0b8/algoliasearch/search/models/search_user_ids_params.py
--rw-r--r--   0        0        0     2970 2024-02-29 16:26:22.701463 algoliasearch-4.0.0b8/algoliasearch/search/models/search_user_ids_response.py
--rw-r--r--   0        0        0     4582 2024-02-29 16:26:22.701463 algoliasearch-4.0.0b8/algoliasearch/search/models/secured_api_key_restrictions.py
--rw-r--r--   0        0        0     2290 2024-02-29 16:26:22.701463 algoliasearch-4.0.0b8/algoliasearch/search/models/semantic_search.py
--rw-r--r--   0        0        0     4234 2024-02-29 16:26:22.701463 algoliasearch-4.0.0b8/algoliasearch/search/models/snippet_result.py
--rw-r--r--   0        0        0     2072 2024-02-29 16:26:22.701463 algoliasearch-4.0.0b8/algoliasearch/search/models/snippet_result_option.py
--rw-r--r--   0        0        0      792 2024-02-29 16:26:22.701463 algoliasearch-4.0.0b8/algoliasearch/search/models/sort_remaining_by.py
--rw-r--r--   0        0        0     1899 2024-02-29 16:26:22.701463 algoliasearch-4.0.0b8/algoliasearch/search/models/source.py
--rw-r--r--   0        0        0     3183 2024-02-29 16:26:22.701463 algoliasearch-4.0.0b8/algoliasearch/search/models/standard_entries.py
--rw-r--r--   0        0        0     3686 2024-02-29 16:26:22.701463 algoliasearch-4.0.0b8/algoliasearch/search/models/synonym_hit.py
--rw-r--r--   0        0        0      750 2024-02-29 16:26:22.701463 algoliasearch-4.0.0b8/algoliasearch/search/models/synonym_type.py
--rw-r--r--   0        0        0     3392 2024-02-29 16:26:22.701463 algoliasearch-4.0.0b8/algoliasearch/search/models/tag_filters.py
--rw-r--r--   0        0        0      698 2024-02-29 16:26:22.701463 algoliasearch-4.0.0b8/algoliasearch/search/models/task_status.py
--rw-r--r--   0        0        0     1906 2024-02-29 16:26:22.701463 algoliasearch-4.0.0b8/algoliasearch/search/models/time_range.py
--rw-r--r--   0        0        0     3375 2024-02-29 16:26:22.701463 algoliasearch-4.0.0b8/algoliasearch/search/models/typo_tolerance.py
--rw-r--r--   0        0        0      636 2024-02-29 16:26:22.701463 algoliasearch-4.0.0b8/algoliasearch/search/models/typo_tolerance_enum.py
--rw-r--r--   0        0        0     1979 2024-02-29 16:26:22.701463 algoliasearch-4.0.0b8/algoliasearch/search/models/update_api_key_response.py
--rw-r--r--   0        0        0     2245 2024-02-29 16:26:22.701463 algoliasearch-4.0.0b8/algoliasearch/search/models/updated_at_response.py
--rw-r--r--   0        0        0     2610 2024-02-29 16:26:22.701463 algoliasearch-4.0.0b8/algoliasearch/search/models/updated_at_with_object_id_response.py
--rw-r--r--   0        0        0     2433 2024-02-29 16:26:22.701463 algoliasearch-4.0.0b8/algoliasearch/search/models/updated_rule_response.py
--rw-r--r--   0        0        0     2361 2024-02-29 16:26:22.701463 algoliasearch-4.0.0b8/algoliasearch/search/models/user_highlight_result.py
--rw-r--r--   0        0        0     3376 2024-02-29 16:26:22.701463 algoliasearch-4.0.0b8/algoliasearch/search/models/user_hit.py
--rw-r--r--   0        0        0     2729 2024-02-29 16:26:22.701463 algoliasearch-4.0.0b8/algoliasearch/search/models/user_id.py
--rw-r--r--   0        0        0     2023 2024-02-29 16:26:22.701463 algoliasearch-4.0.0b8/algoliasearch/search/models/value.py
--rw-r--r--   0        0        0     1075 2024-02-29 16:26:22.701463 algoliasearch-4.0.0b8/pyproject.toml
--rw-r--r--   0        0        0     4761 1970-01-01 00:00:00.000000 algoliasearch-4.0.0b8/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-03-05 09:23:25.753859 algoliasearch-4.0.0b9/LICENSE
+-rw-r--r--   0        0        0     3718 2024-03-05 09:23:25.753859 algoliasearch-4.0.0b9/README.md
+-rw-r--r--   0        0        0     5988 2024-03-05 09:23:25.753859 algoliasearch-4.0.0b9/algoliasearch/.openapi-generator/FILES
+-rw-r--r--   0        0        0        5 2024-03-05 09:23:25.753859 algoliasearch-4.0.0b9/algoliasearch/.openapi-generator/VERSION
+-rw-r--r--   0        0        0     1040 2024-03-05 09:23:25.753859 algoliasearch-4.0.0b9/algoliasearch/.openapi-generator-ignore
+-rw-r--r--   0        0        0      270 2024-03-05 09:23:25.753859 algoliasearch-4.0.0b9/algoliasearch/__init__.py
+-rw-r--r--   0        0        0      270 2024-03-05 09:23:25.753859 algoliasearch-4.0.0b9/algoliasearch/abtesting/__init__.py
+-rw-r--r--   0        0        0    30767 2024-03-05 09:23:25.753859 algoliasearch-4.0.0b9/algoliasearch/abtesting/client.py
+-rw-r--r--   0        0        0     1547 2024-03-05 09:23:25.753859 algoliasearch-4.0.0b9/algoliasearch/abtesting/config.py
+-rw-r--r--   0        0        0      270 2024-03-05 09:23:25.753859 algoliasearch-4.0.0b9/algoliasearch/abtesting/models/__init__.py
+-rw-r--r--   0        0        0     7051 2024-03-05 09:23:25.753859 algoliasearch-4.0.0b9/algoliasearch/abtesting/models/ab_test.py
+-rw-r--r--   0        0        0     2267 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/abtesting/models/ab_test_response.py
+-rw-r--r--   0        0        0     2165 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/abtesting/models/ab_tests_variant.py
+-rw-r--r--   0        0        0     2375 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/abtesting/models/ab_tests_variant_search_params.py
+-rw-r--r--   0        0        0     2653 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/abtesting/models/add_ab_tests_request.py
+-rw-r--r--   0        0        0     3359 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/abtesting/models/add_ab_tests_variant.py
+-rw-r--r--   0        0        0     2470 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/abtesting/models/currencies_value.py
+-rw-r--r--   0        0        0     2029 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/abtesting/models/custom_search_params.py
+-rw-r--r--   0        0        0     2376 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/abtesting/models/error_base.py
+-rw-r--r--   0        0        0     2627 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/abtesting/models/filter_effects.py
+-rw-r--r--   0        0        0     2281 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/abtesting/models/filter_effects_empty_search.py
+-rw-r--r--   0        0        0     2266 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/abtesting/models/filter_effects_outliers.py
+-rw-r--r--   0        0        0     2659 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/abtesting/models/list_ab_tests_response.py
+-rw-r--r--   0        0        0     9910 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/abtesting/models/variant.py
+-rw-r--r--   0        0        0      270 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/analytics/__init__.py
+-rw-r--r--   0        0        0   129977 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/analytics/client.py
+-rw-r--r--   0        0        0     1547 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/analytics/config.py
+-rw-r--r--   0        0        0      270 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/analytics/models/__init__.py
+-rw-r--r--   0        0        0     2208 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/analytics/models/average_click_event.py
+-rw-r--r--   0        0        0     2154 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/analytics/models/click_position.py
+-rw-r--r--   0        0        0     3004 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/analytics/models/click_through_rate_event.py
+-rw-r--r--   0        0        0     3020 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/analytics/models/conversion_rate_event.py
+-rw-r--r--   0        0        0      608 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/analytics/models/direction.py
+-rw-r--r--   0        0        0     2376 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/analytics/models/error_base.py
+-rw-r--r--   0        0        0     2662 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/analytics/models/get_average_click_position_response.py
+-rw-r--r--   0        0        0     2357 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/analytics/models/get_click_positions_response.py
+-rw-r--r--   0        0        0     3454 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/analytics/models/get_click_through_rate_response.py
+-rw-r--r--   0        0        0     3452 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/analytics/models/get_conversation_rate_response.py
+-rw-r--r--   0        0        0     2967 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/analytics/models/get_no_click_rate_response.py
+-rw-r--r--   0        0        0     2986 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/analytics/models/get_no_results_rate_response.py
+-rw-r--r--   0        0        0     2385 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/analytics/models/get_searches_count_response.py
+-rw-r--r--   0        0        0     2317 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/analytics/models/get_searches_no_clicks_response.py
+-rw-r--r--   0        0        0     2346 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/analytics/models/get_searches_no_results_response.py
+-rw-r--r--   0        0        0     1871 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/analytics/models/get_status_response.py
+-rw-r--r--   0        0        0     2259 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/analytics/models/get_top_countries_response.py
+-rw-r--r--   0        0        0     1899 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/analytics/models/get_top_filter_attribute.py
+-rw-r--r--   0        0        0     2396 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/analytics/models/get_top_filter_attributes_response.py
+-rw-r--r--   0        0        0     2168 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/analytics/models/get_top_filter_for_attribute.py
+-rw-r--r--   0        0        0     2398 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/analytics/models/get_top_filter_for_attribute_response.py
+-rw-r--r--   0        0        0     2400 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/analytics/models/get_top_filters_no_results_response.py
+-rw-r--r--   0        0        0     2059 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/analytics/models/get_top_filters_no_results_value.py
+-rw-r--r--   0        0        0     2510 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/analytics/models/get_top_filters_no_results_values.py
+-rw-r--r--   0        0        0     3397 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/analytics/models/get_top_hits_response.py
+-rw-r--r--   0        0        0     3495 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/analytics/models/get_top_searches_response.py
+-rw-r--r--   0        0        0     2318 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/analytics/models/get_users_count_response.py
+-rw-r--r--   0        0        0     2580 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/analytics/models/no_click_rate_event.py
+-rw-r--r--   0        0        0     2590 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/analytics/models/no_results_rate_event.py
+-rw-r--r--   0        0        0      879 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/analytics/models/order_by.py
+-rw-r--r--   0        0        0     1882 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/analytics/models/search_event.py
+-rw-r--r--   0        0        0     2102 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/analytics/models/search_no_click_event.py
+-rw-r--r--   0        0        0     2087 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/analytics/models/search_no_result_event.py
+-rw-r--r--   0        0        0     1842 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/analytics/models/top_country.py
+-rw-r--r--   0        0        0     1788 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/analytics/models/top_hit.py
+-rw-r--r--   0        0        0     3597 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/analytics/models/top_hit_with_analytics.py
+-rw-r--r--   0        0        0     2138 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/analytics/models/top_hits_response.py
+-rw-r--r--   0        0        0     2282 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/analytics/models/top_hits_response_with_analytics.py
+-rw-r--r--   0        0        0     2134 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/analytics/models/top_search.py
+-rw-r--r--   0        0        0     4192 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/analytics/models/top_search_with_analytics.py
+-rw-r--r--   0        0        0     2258 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/analytics/models/top_searches_response.py
+-rw-r--r--   0        0        0     2421 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/analytics/models/top_searches_response_with_analytics.py
+-rw-r--r--   0        0        0     1886 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/analytics/models/user_with_date.py
+-rw-r--r--   0        0        0      270 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/http/__init__.py
+-rw-r--r--   0        0        0     2770 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/http/api_response.py
+-rw-r--r--   0        0        0     1062 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/http/base_config.py
+-rw-r--r--   0        0        0     4756 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/http/exceptions.py
+-rw-r--r--   0        0        0     1228 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/http/helpers.py
+-rw-r--r--   0        0        0     1244 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/http/hosts.py
+-rw-r--r--   0        0        0     2945 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/http/request_options.py
+-rw-r--r--   0        0        0     1461 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/http/retry.py
+-rw-r--r--   0        0        0     1811 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/http/serializer.py
+-rw-r--r--   0        0        0     5911 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/http/transporter.py
+-rw-r--r--   0        0        0      497 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/http/user_agent.py
+-rw-r--r--   0        0        0      104 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/http/verb.py
+-rw-r--r--   0        0        0      270 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/ingestion/__init__.py
+-rw-r--r--   0        0        0   124701 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/ingestion/client.py
+-rw-r--r--   0        0        0     1409 2024-03-05 09:23:25.757859 algoliasearch-4.0.0b9/algoliasearch/ingestion/config.py
+-rw-r--r--   0        0        0      270 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/__init__.py
+-rw-r--r--   0        0        0      676 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/action_type.py
+-rw-r--r--   0        0        0     1962 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/auth_algolia.py
+-rw-r--r--   0        0        0     2070 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/auth_algolia_partial.py
+-rw-r--r--   0        0        0     1702 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/auth_api_key.py
+-rw-r--r--   0        0        0     1750 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/auth_api_key_partial.py
+-rw-r--r--   0        0        0     1809 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/auth_basic.py
+-rw-r--r--   0        0        0     1874 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/auth_basic_partial.py
+-rw-r--r--   0        0        0     2071 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/auth_google_service_account.py
+-rw-r--r--   0        0        0     2184 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/auth_google_service_account_partial.py
+-rw-r--r--   0        0        0     4409 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/auth_input.py
+-rw-r--r--   0        0        0     4852 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/auth_input_partial.py
+-rw-r--r--   0        0        0     2031 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/auth_o_auth.py
+-rw-r--r--   0        0        0     2148 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/auth_o_auth_partial.py
+-rw-r--r--   0        0        0     3306 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/authentication.py
+-rw-r--r--   0        0        0     2684 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/authentication_create.py
+-rw-r--r--   0        0        0     2264 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/authentication_create_response.py
+-rw-r--r--   0        0        0     1868 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/authentication_search.py
+-rw-r--r--   0        0        0      765 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/authentication_sort_keys.py
+-rw-r--r--   0        0        0      798 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/authentication_type.py
+-rw-r--r--   0        0        0     2787 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/authentication_update.py
+-rw-r--r--   0        0        0     2267 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/authentication_update_response.py
+-rw-r--r--   0        0        0     2063 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/big_commerce_channel.py
+-rw-r--r--   0        0        0     1908 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/big_commerce_metafield.py
+-rw-r--r--   0        0        0      631 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/big_query_data_type.py
+-rw-r--r--   0        0        0     2955 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/commercetools_custom_fields.py
+-rw-r--r--   0        0        0     1797 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/delete_response.py
+-rw-r--r--   0        0        0     3095 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/destination.py
+-rw-r--r--   0        0        0     2535 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/destination_create.py
+-rw-r--r--   0        0        0     2237 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/destination_create_response.py
+-rw-r--r--   0        0        0     2703 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/destination_index_name.py
+-rw-r--r--   0        0        0     1838 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/destination_index_prefix.py
+-rw-r--r--   0        0        0     3382 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/destination_input.py
+-rw-r--r--   0        0        0     1841 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/destination_search.py
+-rw-r--r--   0        0        0      720 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/destination_sort_keys.py
+-rw-r--r--   0        0        0      725 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/destination_type.py
+-rw-r--r--   0        0        0     2609 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/destination_update.py
+-rw-r--r--   0        0        0     2240 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/destination_update_response.py
+-rw-r--r--   0        0        0      667 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/docker_image_type.py
+-rw-r--r--   0        0        0      660 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/docker_registry.py
+-rw-r--r--   0        0        0     1944 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/docker_source_discover.py
+-rw-r--r--   0        0        0     1718 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/docker_source_streams.py
+-rw-r--r--   0        0        0     2376 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/error_base.py
+-rw-r--r--   0        0        0     2905 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/event.py
+-rw-r--r--   0        0        0      682 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/event_sort_keys.py
+-rw-r--r--   0        0        0      728 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/event_status.py
+-rw-r--r--   0        0        0      660 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/event_type.py
+-rw-r--r--   0        0        0     2647 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/list_authentications_response.py
+-rw-r--r--   0        0        0     2582 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/list_destinations_response.py
+-rw-r--r--   0        0        0     2744 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/list_events_response.py
+-rw-r--r--   0        0        0     2469 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/list_sources_response.py
+-rw-r--r--   0        0        0     2462 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/list_tasks_response.py
+-rw-r--r--   0        0        0     2021 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/mapping_field_directive.py
+-rw-r--r--   0        0        0     2452 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/mapping_input.py
+-rw-r--r--   0        0        0     3013 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/mapping_kit_action.py
+-rw-r--r--   0        0        0      697 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/mapping_type_csv.py
+-rw-r--r--   0        0        0      611 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/method_type.py
+-rw-r--r--   0        0        0     2531 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/on_demand_date_utils_input.py
+-rw-r--r--   0        0        0     2066 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/on_demand_trigger.py
+-rw-r--r--   0        0        0     1826 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/on_demand_trigger_input.py
+-rw-r--r--   0        0        0      671 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/on_demand_trigger_type.py
+-rw-r--r--   0        0        0      630 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/order_keys.py
+-rw-r--r--   0        0        0     2036 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/pagination.py
+-rw-r--r--   0        0        0      686 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/platform.py
+-rw-r--r--   0        0        0      645 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/platform_none.py
+-rw-r--r--   0        0        0     3187 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/platform_with_none.py
+-rw-r--r--   0        0        0      685 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/record_type.py
+-rw-r--r--   0        0        0     4007 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/run.py
+-rw-r--r--   0        0        0     2710 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/run_list_response.py
+-rw-r--r--   0        0        0      655 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/run_outcome.py
+-rw-r--r--   0        0        0     2040 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/run_progress.py
+-rw-r--r--   0        0        0      810 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/run_reason_code.py
+-rw-r--r--   0        0        0     1999 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/run_response.py
+-rw-r--r--   0        0        0      682 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/run_sort_keys.py
+-rw-r--r--   0        0        0      692 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/run_status.py
+-rw-r--r--   0        0        0      640 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/run_type.py
+-rw-r--r--   0        0        0     2381 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/schedule_date_utils_input.py
+-rw-r--r--   0        0        0     2472 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/schedule_trigger.py
+-rw-r--r--   0        0        0     1994 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/schedule_trigger_input.py
+-rw-r--r--   0        0        0      669 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/schedule_trigger_type.py
+-rw-r--r--   0        0        0     2876 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/source.py
+-rw-r--r--   0        0        0     3755 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/source_big_commerce.py
+-rw-r--r--   0        0        0     3154 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/source_big_query.py
+-rw-r--r--   0        0        0     3161 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/source_commercetools.py
+-rw-r--r--   0        0        0     2388 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/source_create.py
+-rw-r--r--   0        0        0     2067 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/source_create_response.py
+-rw-r--r--   0        0        0     2908 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/source_csv.py
+-rw-r--r--   0        0        0     2468 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/source_docker.py
+-rw-r--r--   0        0        0     4991 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/source_input.py
+-rw-r--r--   0        0        0     2208 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/source_json.py
+-rw-r--r--   0        0        0     1737 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/source_search.py
+-rw-r--r--   0        0        0      705 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/source_sort_keys.py
+-rw-r--r--   0        0        0      727 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/source_type.py
+-rw-r--r--   0        0        0     2319 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/source_update.py
+-rw-r--r--   0        0        0     3190 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/source_update_commercetools.py
+-rw-r--r--   0        0        0     2360 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/source_update_docker.py
+-rw-r--r--   0        0        0     4665 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/source_update_input.py
+-rw-r--r--   0        0        0     2070 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/source_update_response.py
+-rw-r--r--   0        0        0     1842 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/subscription_trigger.py
+-rw-r--r--   0        0        0      696 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/subscription_trigger_type.py
+-rw-r--r--   0        0        0     3713 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/task.py
+-rw-r--r--   0        0        0     3337 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/task_create.py
+-rw-r--r--   0        0        0     1971 2024-03-05 09:23:25.761859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/task_create_response.py
+-rw-r--r--   0        0        0     3805 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/task_create_trigger.py
+-rw-r--r--   0        0        0     3387 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/task_input.py
+-rw-r--r--   0        0        0     1721 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/task_search.py
+-rw-r--r--   0        0        0      741 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/task_sort_keys.py
+-rw-r--r--   0        0        0     3114 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/task_update.py
+-rw-r--r--   0        0        0     1972 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/task_update_response.py
+-rw-r--r--   0        0        0     3689 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/trigger.py
+-rw-r--r--   0        0        0      929 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/trigger_type.py
+-rw-r--r--   0        0        0     1835 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/trigger_update_input.py
+-rw-r--r--   0        0        0     2158 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/ingestion/models/window.py
+-rw-r--r--   0        0        0      270 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/insights/__init__.py
+-rw-r--r--   0        0        0    22116 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/insights/client.py
+-rw-r--r--   0        0        0     1541 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/insights/config.py
+-rw-r--r--   0        0        0      270 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/insights/models/__init__.py
+-rw-r--r--   0        0        0      617 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/insights/models/add_to_cart_event.py
+-rw-r--r--   0        0        0     6815 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/insights/models/added_to_cart_object_ids.py
+-rw-r--r--   0        0        0     7492 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/insights/models/added_to_cart_object_ids_after_search.py
+-rw-r--r--   0        0        0      597 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/insights/models/click_event.py
+-rw-r--r--   0        0        0     5013 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/insights/models/clicked_filters.py
+-rw-r--r--   0        0        0     5218 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/insights/models/clicked_object_ids.py
+-rw-r--r--   0        0        0     6196 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/insights/models/clicked_object_ids_after_search.py
+-rw-r--r--   0        0        0      622 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/insights/models/conversion_event.py
+-rw-r--r--   0        0        0     4972 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/insights/models/converted_filters.py
+-rw-r--r--   0        0        0     5251 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/insights/models/converted_object_ids.py
+-rw-r--r--   0        0        0     6007 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/insights/models/converted_object_ids_after_search.py
+-rw-r--r--   0        0        0     3286 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/insights/models/discount.py
+-rw-r--r--   0        0        0     2376 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/insights/models/error_base.py
+-rw-r--r--   0        0        0     8136 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/insights/models/events_items.py
+-rw-r--r--   0        0        0     2024 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/insights/models/events_response.py
+-rw-r--r--   0        0        0     2494 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/insights/models/insights_events.py
+-rw-r--r--   0        0        0     2624 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/insights/models/object_data.py
+-rw-r--r--   0        0        0     3425 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/insights/models/object_data_after_search.py
+-rw-r--r--   0        0        0     3282 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/insights/models/price.py
+-rw-r--r--   0        0        0      612 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/insights/models/purchase_event.py
+-rw-r--r--   0        0        0     6780 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/insights/models/purchased_object_ids.py
+-rw-r--r--   0        0        0     6759 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/insights/models/purchased_object_ids_after_search.py
+-rw-r--r--   0        0        0     3262 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/insights/models/value.py
+-rw-r--r--   0        0        0      592 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/insights/models/view_event.py
+-rw-r--r--   0        0        0     5069 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/insights/models/viewed_filters.py
+-rw-r--r--   0        0        0     5008 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/insights/models/viewed_object_ids.py
+-rw-r--r--   0        0        0      270 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/monitoring/__init__.py
+-rw-r--r--   0        0        0    38131 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/monitoring/client.py
+-rw-r--r--   0        0        0     1085 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/monitoring/config.py
+-rw-r--r--   0        0        0      270 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/monitoring/models/__init__.py
+-rw-r--r--   0        0        0     2376 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/monitoring/models/error_base.py
+-rw-r--r--   0        0        0     1752 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/monitoring/models/get_inventory403_response.py
+-rw-r--r--   0        0        0     1924 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/monitoring/models/incident.py
+-rw-r--r--   0        0        0     2182 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/monitoring/models/incidents_inner.py
+-rw-r--r--   0        0        0     2526 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/monitoring/models/incidents_response.py
+-rw-r--r--   0        0        0     2109 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/monitoring/models/indexing_time_response.py
+-rw-r--r--   0        0        0     2538 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/monitoring/models/indexing_time_response_metrics.py
+-rw-r--r--   0        0        0     2124 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/monitoring/models/infrastructure_response.py
+-rw-r--r--   0        0        0     6267 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/monitoring/models/infrastructure_response_metrics.py
+-rw-r--r--   0        0        0     2168 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/monitoring/models/inventory_response.py
+-rw-r--r--   0        0        0     2068 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/monitoring/models/latency_response.py
+-rw-r--r--   0        0        0     2510 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/monitoring/models/latency_response_metrics.py
+-rw-r--r--   0        0        0      762 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/monitoring/models/metric.py
+-rw-r--r--   0        0        0      659 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/monitoring/models/period.py
+-rw-r--r--   0        0        0     1943 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/monitoring/models/probes_metric.py
+-rw-r--r--   0        0        0      817 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/monitoring/models/region.py
+-rw-r--r--   0        0        0     2886 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/monitoring/models/server.py
+-rw-r--r--   0        0        0      613 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/monitoring/models/server_status.py
+-rw-r--r--   0        0        0      735 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/monitoring/models/status.py
+-rw-r--r--   0        0        0     1831 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/monitoring/models/status_response.py
+-rw-r--r--   0        0        0     1922 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/monitoring/models/time_inner.py
+-rw-r--r--   0        0        0      583 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/monitoring/models/type.py
+-rw-r--r--   0        0        0      270 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/personalization/__init__.py
+-rw-r--r--   0        0        0    28661 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/personalization/client.py
+-rw-r--r--   0        0        0     1432 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/personalization/config.py
+-rw-r--r--   0        0        0      270 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/personalization/models/__init__.py
+-rw-r--r--   0        0        0     2227 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/personalization/models/delete_user_profile_response.py
+-rw-r--r--   0        0        0     2376 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/personalization/models/error_base.py
+-rw-r--r--   0        0        0     2109 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/personalization/models/event_scoring.py
+-rw-r--r--   0        0        0     1906 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/personalization/models/facet_scoring.py
+-rw-r--r--   0        0        0     2233 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/personalization/models/get_user_token_response.py
+-rw-r--r--   0        0        0     3371 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/personalization/models/personalization_strategy_params.py
+-rw-r--r--   0        0        0     1844 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/personalization/models/set_personalization_strategy_response.py
+-rw-r--r--   0        0        0        0 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/py.typed
+-rw-r--r--   0        0        0      270 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/query_suggestions/__init__.py
+-rw-r--r--   0        0        0    34436 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/query_suggestions/client.py
+-rw-r--r--   0        0        0     1436 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/query_suggestions/config.py
+-rw-r--r--   0        0        0      270 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/query_suggestions/models/__init__.py
+-rw-r--r--   0        0        0     2637 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/query_suggestions/models/base_query_suggestions_configuration_response.py
+-rw-r--r--   0        0        0     1904 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/query_suggestions/models/base_query_suggestions_configuration_with_index.py
+-rw-r--r--   0        0        0     1963 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/query_suggestions/models/base_response.py
+-rw-r--r--   0        0        0     2376 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/query_suggestions/models/error_base.py
+-rw-r--r--   0        0        0     1926 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/query_suggestions/models/facet.py
+-rw-r--r--   0        0        0     3150 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/query_suggestions/models/get_config_status200_response.py
+-rw-r--r--   0        0        0     2642 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/query_suggestions/models/get_log_file200_response.py
+-rw-r--r--   0        0        0     3301 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/query_suggestions/models/languages.py
+-rw-r--r--   0        0        0      903 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/query_suggestions/models/log_level.py
+-rw-r--r--   0        0        0     3796 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/query_suggestions/models/query_suggestions_configuration.py
+-rw-r--r--   0        0        0     4825 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/query_suggestions/models/query_suggestions_configuration_response.py
+-rw-r--r--   0        0        0     3986 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/query_suggestions/models/query_suggestions_configuration_with_index.py
+-rw-r--r--   0        0        0     5389 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/query_suggestions/models/source_index.py
+-rw-r--r--   0        0        0      270 2024-03-05 09:23:25.765859 algoliasearch-4.0.0b9/algoliasearch/recommend/__init__.py
+-rw-r--r--   0        0        0    37789 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/client.py
+-rw-r--r--   0        0        0     1638 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/config.py
+-rw-r--r--   0        0        0      270 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/__init__.py
+-rw-r--r--   0        0        0      679 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/advanced_syntax_features.py
+-rw-r--r--   0        0        0      728 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/alternatives_as_exact.py
+-rw-r--r--   0        0        0      827 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/anchoring.py
+-rw-r--r--   0        0        0     3944 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/around_precision.py
+-rw-r--r--   0        0        0     1875 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/around_precision_from_value_inner.py
+-rw-r--r--   0        0        0     3398 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/around_radius.py
+-rw-r--r--   0        0        0      608 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/around_radius_all.py
+-rw-r--r--   0        0        0     2350 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/automatic_facet_filter.py
+-rw-r--r--   0        0        0     3519 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/automatic_facet_filters.py
+-rw-r--r--   0        0        0     2592 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/base_recommend_request.py
+-rw-r--r--   0        0        0     3020 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/base_recommendations_query.py
+-rw-r--r--   0        0        0     2974 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/base_recommended_for_you_query.py
+-rw-r--r--   0        0        0     1981 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/base_recommended_for_you_query_parameters.py
+-rw-r--r--   0        0        0    14304 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/base_search_params.py
+-rw-r--r--   0        0        0    14197 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/base_search_params_without_query.py
+-rw-r--r--   0        0        0    11592 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/base_search_response.py
+-rw-r--r--   0        0        0     2023 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/base_trending_facets_query.py
+-rw-r--r--   0        0        0     3252 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/base_trending_items_query.py
+-rw-r--r--   0        0        0     2381 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/condition.py
+-rw-r--r--   0        0        0     4232 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/consequence.py
+-rw-r--r--   0        0        0     1813 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/consequence_hide.py
+-rw-r--r--   0        0        0    33338 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/consequence_params.py
+-rw-r--r--   0        0        0     3437 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/consequence_query.py
+-rw-r--r--   0        0        0     2367 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/consequence_query_object.py
+-rw-r--r--   0        0        0     2240 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/deleted_at_response.py
+-rw-r--r--   0        0        0     3396 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/distinct.py
+-rw-r--r--   0        0        0     2190 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/edit.py
+-rw-r--r--   0        0        0      622 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/edit_type.py
+-rw-r--r--   0        0        0     2376 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/error_base.py
+-rw-r--r--   0        0        0      926 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/exact_on_single_word_query.py
+-rw-r--r--   0        0        0     3981 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/exhaustive.py
+-rw-r--r--   0        0        0     3408 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/facet_filters.py
+-rw-r--r--   0        0        0     2657 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/facet_ordering.py
+-rw-r--r--   0        0        0     1796 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/facets.py
+-rw-r--r--   0        0        0     2386 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/facets_stats.py
+-rw-r--r--   0        0        0     1786 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/get_recommend_task_response.py
+-rw-r--r--   0        0        0     2404 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/get_recommendations_params.py
+-rw-r--r--   0        0        0     2321 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/get_recommendations_response.py
+-rw-r--r--   0        0        0     4159 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/highlight_result.py
+-rw-r--r--   0        0        0     2567 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/highlight_result_option.py
+-rw-r--r--   0        0        0     4005 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/ignore_plurals.py
+-rw-r--r--   0        0        0    19465 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/index_settings_as_search_params.py
+-rw-r--r--   0        0        0      685 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/match_level.py
+-rw-r--r--   0        0        0     2293 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/matched_geo_location.py
+-rw-r--r--   0        0        0     3199 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/mixed_search_filters.py
+-rw-r--r--   0        0        0      677 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/mode.py
+-rw-r--r--   0        0        0     3416 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/numeric_filters.py
+-rw-r--r--   0        0        0     3603 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/optional_filters.py
+-rw-r--r--   0        0        0     3692 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/params.py
+-rw-r--r--   0        0        0     2235 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/personalization.py
+-rw-r--r--   0        0        0     3255 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/promote.py
+-rw-r--r--   0        0        0     2153 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/promote_object_id.py
+-rw-r--r--   0        0        0     2175 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/promote_object_ids.py
+-rw-r--r--   0        0        0      846 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/query_type.py
+-rw-r--r--   0        0        0     5053 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/ranking_info.py
+-rw-r--r--   0        0        0     3555 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/re_ranking_apply_filter.py
+-rw-r--r--   0        0        0     5201 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/recommend_hit.py
+-rw-r--r--   0        0        0      776 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/recommend_models.py
+-rw-r--r--   0        0        0      702 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/recommendation_models.py
+-rw-r--r--   0        0        0     3251 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/recommendations_hit.py
+-rw-r--r--   0        0        0     2557 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/recommendations_hits.py
+-rw-r--r--   0        0        0     3880 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/recommendations_query.py
+-rw-r--r--   0        0        0     4383 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/recommendations_request.py
+-rw-r--r--   0        0        0    10919 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/recommendations_results.py
+-rw-r--r--   0        0        0      677 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/recommended_for_you_model.py
+-rw-r--r--   0        0        0     3845 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/recommended_for_you_query.py
+-rw-r--r--   0        0        0    32016 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/recommended_for_you_query_parameters.py
+-rw-r--r--   0        0        0     2374 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/redirect.py
+-rw-r--r--   0        0        0     2607 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/redirect_rule_index_metadata.py
+-rw-r--r--   0        0        0     1796 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/redirect_rule_index_metadata_data.py
+-rw-r--r--   0        0        0     3937 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/remove_stop_words.py
+-rw-r--r--   0        0        0      924 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/remove_words_if_no_results.py
+-rw-r--r--   0        0        0     2511 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/rendering_content.py
+-rw-r--r--   0        0        0     3881 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/rule_response.py
+-rw-r--r--   0        0        0     1929 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/rule_response_metadata.py
+-rw-r--r--   0        0        0    31992 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/search_params_object.py
+-rw-r--r--   0        0        0     1806 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/search_params_query.py
+-rw-r--r--   0        0        0     3111 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/search_recommend_rules_params.py
+-rw-r--r--   0        0        0     2717 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/search_recommend_rules_response.py
+-rw-r--r--   0        0        0     2290 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/semantic_search.py
+-rw-r--r--   0        0        0     4237 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/snippet_result.py
+-rw-r--r--   0        0        0     2075 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/snippet_result_option.py
+-rw-r--r--   0        0        0      792 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/sort_remaining_by.py
+-rw-r--r--   0        0        0     3395 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/tag_filters.py
+-rw-r--r--   0        0        0      698 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/task_status.py
+-rw-r--r--   0        0        0     2294 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/trending_facet_hit.py
+-rw-r--r--   0        0        0      653 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/trending_facets_model.py
+-rw-r--r--   0        0        0     2930 2024-03-05 09:23:25.769859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/trending_facets_query.py
+-rw-r--r--   0        0        0      648 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/trending_items_model.py
+-rw-r--r--   0        0        0     4112 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/trending_items_query.py
+-rw-r--r--   0        0        0     3378 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/typo_tolerance.py
+-rw-r--r--   0        0        0      636 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/typo_tolerance_enum.py
+-rw-r--r--   0        0        0     2026 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/recommend/models/value.py
+-rw-r--r--   0        0        0      270 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/__init__.py
+-rw-r--r--   0        0        0   214867 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/client.py
+-rw-r--r--   0        0        0     1632 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/config.py
+-rw-r--r--   0        0        0      270 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/__init__.py
+-rw-r--r--   0        0        0     1856 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/acl.py
+-rw-r--r--   0        0        0      833 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/action.py
+-rw-r--r--   0        0        0     1960 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/add_api_key_response.py
+-rw-r--r--   0        0        0      679 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/advanced_syntax_features.py
+-rw-r--r--   0        0        0      728 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/alternatives_as_exact.py
+-rw-r--r--   0        0        0      827 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/anchoring.py
+-rw-r--r--   0        0        0     5481 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/api_key.py
+-rw-r--r--   0        0        0      652 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/api_key_operation.py
+-rw-r--r--   0        0        0     3941 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/around_precision.py
+-rw-r--r--   0        0        0     1875 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/around_precision_from_value_inner.py
+-rw-r--r--   0        0        0     3395 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/around_radius.py
+-rw-r--r--   0        0        0      608 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/around_radius_all.py
+-rw-r--r--   0        0        0     1759 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/assign_user_id_params.py
+-rw-r--r--   0        0        0     3317 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/attribute_to_update.py
+-rw-r--r--   0        0        0     2350 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/automatic_facet_filter.py
+-rw-r--r--   0        0        0     3516 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/automatic_facet_filters.py
+-rw-r--r--   0        0        0     2044 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/base_get_api_key_response.py
+-rw-r--r--   0        0        0     8818 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/base_index_settings.py
+-rw-r--r--   0        0        0    14286 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/base_search_params.py
+-rw-r--r--   0        0        0    14179 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/base_search_params_without_query.py
+-rw-r--r--   0        0        0    11580 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/base_search_response.py
+-rw-r--r--   0        0        0     1902 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/batch_assign_user_ids_params.py
+-rw-r--r--   0        0        0     2836 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/batch_dictionary_entries_params.py
+-rw-r--r--   0        0        0     2184 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/batch_dictionary_entries_request.py
+-rw-r--r--   0        0        0     2228 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/batch_params.py
+-rw-r--r--   0        0        0     1892 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/batch_request.py
+-rw-r--r--   0        0        0     2158 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/batch_response.py
+-rw-r--r--   0        0        0     2190 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/batch_write_params.py
+-rw-r--r--   0        0        0     3299 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/browse_params.py
+-rw-r--r--   0        0        0    32333 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/browse_params_object.py
+-rw-r--r--   0        0        0    11120 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/browse_response.py
+-rw-r--r--   0        0        0     2141 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/built_in_operation.py
+-rw-r--r--   0        0        0      815 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/built_in_operation_type.py
+-rw-r--r--   0        0        0     2378 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/condition.py
+-rw-r--r--   0        0        0     4223 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/consequence.py
+-rw-r--r--   0        0        0     1813 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/consequence_hide.py
+-rw-r--r--   0        0        0    33266 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/consequence_params.py
+-rw-r--r--   0        0        0     3425 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/consequence_query.py
+-rw-r--r--   0        0        0     2364 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/consequence_query_object.py
+-rw-r--r--   0        0        0     1879 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/created_at_response.py
+-rw-r--r--   0        0        0     2014 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/cursor.py
+-rw-r--r--   0        0        0     1876 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/delete_api_key_response.py
+-rw-r--r--   0        0        0     4903 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/delete_by_params.py
+-rw-r--r--   0        0        0     1876 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/delete_source_response.py
+-rw-r--r--   0        0        0     2240 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/deleted_at_response.py
+-rw-r--r--   0        0        0      656 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/dictionary_action.py
+-rw-r--r--   0        0        0     4691 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/dictionary_entry.py
+-rw-r--r--   0        0        0      721 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/dictionary_entry_state.py
+-rw-r--r--   0        0        0     2049 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/dictionary_language.py
+-rw-r--r--   0        0        0     2282 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/dictionary_settings_params.py
+-rw-r--r--   0        0        0      669 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/dictionary_type.py
+-rw-r--r--   0        0        0     3396 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/distinct.py
+-rw-r--r--   0        0        0     2187 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/edit.py
+-rw-r--r--   0        0        0      622 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/edit_type.py
+-rw-r--r--   0        0        0     2376 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/error_base.py
+-rw-r--r--   0        0        0      926 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/exact_on_single_word_query.py
+-rw-r--r--   0        0        0     3981 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/exhaustive.py
+-rw-r--r--   0        0        0     3405 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/facet_filters.py
+-rw-r--r--   0        0        0     2343 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/facet_hits.py
+-rw-r--r--   0        0        0     2651 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/facet_ordering.py
+-rw-r--r--   0        0        0     1796 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/facets.py
+-rw-r--r--   0        0        0     2386 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/facets_stats.py
+-rw-r--r--   0        0        0     3925 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/fetched_index.py
+-rw-r--r--   0        0        0     5876 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/get_api_key_response.py
+-rw-r--r--   0        0        0     2251 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/get_dictionary_settings_response.py
+-rw-r--r--   0        0        0     2082 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/get_logs_response.py
+-rw-r--r--   0        0        0     2213 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/get_objects_params.py
+-rw-r--r--   0        0        0     2355 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/get_objects_request.py
+-rw-r--r--   0        0        0     1763 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/get_objects_response.py
+-rw-r--r--   0        0        0     1747 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/get_task_response.py
+-rw-r--r--   0        0        0     1987 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/get_top_user_ids_response.py
+-rw-r--r--   0        0        0     2124 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/has_pending_mappings_response.py
+-rw-r--r--   0        0        0     4156 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/highlight_result.py
+-rw-r--r--   0        0        0     2564 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/highlight_result_option.py
+-rw-r--r--   0        0        0     4880 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/hit.py
+-rw-r--r--   0        0        0     4005 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/ignore_plurals.py
+-rw-r--r--   0        0        0    26249 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/index_settings.py
+-rw-r--r--   0        0        0    19417 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/index_settings_as_search_params.py
+-rw-r--r--   0        0        0     3244 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/languages.py
+-rw-r--r--   0        0        0     2235 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/list_api_keys_response.py
+-rw-r--r--   0        0        0     1912 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/list_clusters_response.py
+-rw-r--r--   0        0        0     2415 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/list_indices_response.py
+-rw-r--r--   0        0        0     2186 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/list_user_ids_response.py
+-rw-r--r--   0        0        0     4460 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/log.py
+-rw-r--r--   0        0        0     2153 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/log_query.py
+-rw-r--r--   0        0        0      644 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/log_type.py
+-rw-r--r--   0        0        0      685 2024-03-05 09:23:25.773859 algoliasearch-4.0.0b9/algoliasearch/search/models/match_level.py
+-rw-r--r--   0        0        0     2293 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/matched_geo_location.py
+-rw-r--r--   0        0        0     3199 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/mixed_search_filters.py
+-rw-r--r--   0        0        0      677 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/mode.py
+-rw-r--r--   0        0        0     2151 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/multiple_batch_request.py
+-rw-r--r--   0        0        0     2006 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/multiple_batch_response.py
+-rw-r--r--   0        0        0     3413 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/numeric_filters.py
+-rw-r--r--   0        0        0     2398 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/operation_index_params.py
+-rw-r--r--   0        0        0      649 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/operation_type.py
+-rw-r--r--   0        0        0     3600 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/optional_filters.py
+-rw-r--r--   0        0        0     3683 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/params.py
+-rw-r--r--   0        0        0     2235 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/personalization.py
+-rw-r--r--   0        0        0     3249 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/promote.py
+-rw-r--r--   0        0        0     2153 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/promote_object_id.py
+-rw-r--r--   0        0        0     2175 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/promote_object_ids.py
+-rw-r--r--   0        0        0      846 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/query_type.py
+-rw-r--r--   0        0        0     5047 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/ranking_info.py
+-rw-r--r--   0        0        0     3552 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/re_ranking_apply_filter.py
+-rw-r--r--   0        0        0     2371 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/redirect.py
+-rw-r--r--   0        0        0     2604 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/redirect_rule_index_metadata.py
+-rw-r--r--   0        0        0     1796 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/redirect_rule_index_metadata_data.py
+-rw-r--r--   0        0        0     3937 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/remove_stop_words.py
+-rw-r--r--   0        0        0     1876 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/remove_user_id_response.py
+-rw-r--r--   0        0        0      924 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/remove_words_if_no_results.py
+-rw-r--r--   0        0        0     2508 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/rendering_content.py
+-rw-r--r--   0        0        0     1887 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/replace_source_response.py
+-rw-r--r--   0        0        0     4129 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/rule.py
+-rw-r--r--   0        0        0     2402 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/save_object_response.py
+-rw-r--r--   0        0        0     2395 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/save_synonym_response.py
+-rw-r--r--   0        0        0      646 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/scope_type.py
+-rw-r--r--   0        0        0     2613 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/search_dictionary_entries_params.py
+-rw-r--r--   0        0        0     2542 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/search_for_facet_values_request.py
+-rw-r--r--   0        0        0     2832 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/search_for_facet_values_response.py
+-rw-r--r--   0        0        0    32686 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/search_for_facets.py
+-rw-r--r--   0        0        0     2727 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/search_for_facets_options.py
+-rw-r--r--   0        0        0    32384 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/search_for_hits.py
+-rw-r--r--   0        0        0     1973 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/search_for_hits_options.py
+-rw-r--r--   0        0        0     3039 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/search_hits.py
+-rw-r--r--   0        0        0     2370 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/search_method_params.py
+-rw-r--r--   0        0        0     3299 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/search_params.py
+-rw-r--r--   0        0        0    31926 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/search_params_object.py
+-rw-r--r--   0        0        0     1806 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/search_params_query.py
+-rw-r--r--   0        0        0     1830 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/search_params_string.py
+-rw-r--r--   0        0        0     3225 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/search_query.py
+-rw-r--r--   0        0        0    12084 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/search_response.py
+-rw-r--r--   0        0        0     2178 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/search_responses.py
+-rw-r--r--   0        0        0     3365 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/search_result.py
+-rw-r--r--   0        0        0     3491 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/search_rules_params.py
+-rw-r--r--   0        0        0     2517 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/search_rules_response.py
+-rw-r--r--   0        0        0      832 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/search_strategy.py
+-rw-r--r--   0        0        0     2438 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/search_synonyms_params.py
+-rw-r--r--   0        0        0     3041 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/search_synonyms_response.py
+-rw-r--r--   0        0        0      781 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/search_type_default.py
+-rw-r--r--   0        0        0      773 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/search_type_facet.py
+-rw-r--r--   0        0        0     2607 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/search_user_ids_params.py
+-rw-r--r--   0        0        0     2970 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/search_user_ids_response.py
+-rw-r--r--   0        0        0     4582 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/secured_api_key_restrictions.py
+-rw-r--r--   0        0        0     2290 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/semantic_search.py
+-rw-r--r--   0        0        0     4234 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/snippet_result.py
+-rw-r--r--   0        0        0     2072 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/snippet_result_option.py
+-rw-r--r--   0        0        0      792 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/sort_remaining_by.py
+-rw-r--r--   0        0        0     1899 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/source.py
+-rw-r--r--   0        0        0     3183 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/standard_entries.py
+-rw-r--r--   0        0        0     3686 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/synonym_hit.py
+-rw-r--r--   0        0        0      750 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/synonym_type.py
+-rw-r--r--   0        0        0     3392 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/tag_filters.py
+-rw-r--r--   0        0        0      698 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/task_status.py
+-rw-r--r--   0        0        0     1906 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/time_range.py
+-rw-r--r--   0        0        0     3375 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/typo_tolerance.py
+-rw-r--r--   0        0        0      636 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/typo_tolerance_enum.py
+-rw-r--r--   0        0        0     1979 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/update_api_key_response.py
+-rw-r--r--   0        0        0     2245 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/updated_at_response.py
+-rw-r--r--   0        0        0     2610 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/updated_at_with_object_id_response.py
+-rw-r--r--   0        0        0     2433 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/updated_rule_response.py
+-rw-r--r--   0        0        0     2361 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/user_highlight_result.py
+-rw-r--r--   0        0        0     3376 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/user_hit.py
+-rw-r--r--   0        0        0     2729 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/user_id.py
+-rw-r--r--   0        0        0     2023 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/algoliasearch/search/models/value.py
+-rw-r--r--   0        0        0     1075 2024-03-05 09:23:25.777859 algoliasearch-4.0.0b9/pyproject.toml
+-rw-r--r--   0        0        0     4761 1970-01-01 00:00:00.000000 algoliasearch-4.0.0b9/PKG-INFO
```

### Comparing `algoliasearch-4.0.0b8/LICENSE` & `algoliasearch-4.0.0b9/LICENSE`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/README.md` & `algoliasearch-4.0.0b9/README.md`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/.openapi-generator/FILES` & `algoliasearch-4.0.0b9/algoliasearch/.openapi-generator/FILES`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/.openapi-generator-ignore` & `algoliasearch-4.0.0b9/algoliasearch/.openapi-generator-ignore`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/abtesting/client.py` & `algoliasearch-4.0.0b9/algoliasearch/abtesting/client.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/abtesting/config.py` & `algoliasearch-4.0.0b9/algoliasearch/abtesting/config.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/abtesting/models/ab_test.py` & `algoliasearch-4.0.0b9/algoliasearch/abtesting/models/ab_test.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/abtesting/models/ab_test_response.py` & `algoliasearch-4.0.0b9/algoliasearch/abtesting/models/ab_test_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/abtesting/models/ab_tests_variant.py` & `algoliasearch-4.0.0b9/algoliasearch/abtesting/models/ab_tests_variant.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/abtesting/models/ab_tests_variant_search_params.py` & `algoliasearch-4.0.0b9/algoliasearch/abtesting/models/ab_tests_variant_search_params.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/abtesting/models/add_ab_tests_request.py` & `algoliasearch-4.0.0b9/algoliasearch/abtesting/models/add_ab_tests_request.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/abtesting/models/add_ab_tests_variant.py` & `algoliasearch-4.0.0b9/algoliasearch/abtesting/models/add_ab_tests_variant.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/abtesting/models/currencies_value.py` & `algoliasearch-4.0.0b9/algoliasearch/abtesting/models/currencies_value.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/abtesting/models/custom_search_params.py` & `algoliasearch-4.0.0b9/algoliasearch/abtesting/models/custom_search_params.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/abtesting/models/error_base.py` & `algoliasearch-4.0.0b9/algoliasearch/abtesting/models/error_base.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/abtesting/models/filter_effects.py` & `algoliasearch-4.0.0b9/algoliasearch/abtesting/models/filter_effects.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/abtesting/models/filter_effects_empty_search.py` & `algoliasearch-4.0.0b9/algoliasearch/abtesting/models/filter_effects_empty_search.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/abtesting/models/filter_effects_outliers.py` & `algoliasearch-4.0.0b9/algoliasearch/abtesting/models/filter_effects_outliers.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/abtesting/models/list_ab_tests_response.py` & `algoliasearch-4.0.0b9/algoliasearch/abtesting/models/list_ab_tests_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/abtesting/models/variant.py` & `algoliasearch-4.0.0b9/algoliasearch/abtesting/models/variant.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/analytics/client.py` & `algoliasearch-4.0.0b9/algoliasearch/analytics/client.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/analytics/config.py` & `algoliasearch-4.0.0b9/algoliasearch/analytics/config.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/analytics/models/average_click_event.py` & `algoliasearch-4.0.0b9/algoliasearch/analytics/models/average_click_event.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/analytics/models/click_position.py` & `algoliasearch-4.0.0b9/algoliasearch/analytics/models/click_position.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/analytics/models/click_through_rate_event.py` & `algoliasearch-4.0.0b9/algoliasearch/analytics/models/click_through_rate_event.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/analytics/models/conversion_rate_event.py` & `algoliasearch-4.0.0b9/algoliasearch/analytics/models/conversion_rate_event.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/analytics/models/direction.py` & `algoliasearch-4.0.0b9/algoliasearch/analytics/models/direction.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/analytics/models/error_base.py` & `algoliasearch-4.0.0b9/algoliasearch/analytics/models/error_base.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/analytics/models/get_average_click_position_response.py` & `algoliasearch-4.0.0b9/algoliasearch/analytics/models/get_average_click_position_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/analytics/models/get_click_positions_response.py` & `algoliasearch-4.0.0b9/algoliasearch/analytics/models/get_click_positions_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/analytics/models/get_click_through_rate_response.py` & `algoliasearch-4.0.0b9/algoliasearch/analytics/models/get_click_through_rate_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/analytics/models/get_conversation_rate_response.py` & `algoliasearch-4.0.0b9/algoliasearch/analytics/models/get_conversation_rate_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/analytics/models/get_no_click_rate_response.py` & `algoliasearch-4.0.0b9/algoliasearch/analytics/models/get_no_click_rate_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/analytics/models/get_no_results_rate_response.py` & `algoliasearch-4.0.0b9/algoliasearch/analytics/models/get_no_results_rate_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/analytics/models/get_searches_count_response.py` & `algoliasearch-4.0.0b9/algoliasearch/analytics/models/get_searches_count_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/analytics/models/get_searches_no_clicks_response.py` & `algoliasearch-4.0.0b9/algoliasearch/analytics/models/get_searches_no_clicks_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/analytics/models/get_searches_no_results_response.py` & `algoliasearch-4.0.0b9/algoliasearch/analytics/models/get_searches_no_results_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/analytics/models/get_status_response.py` & `algoliasearch-4.0.0b9/algoliasearch/analytics/models/get_status_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/analytics/models/get_top_countries_response.py` & `algoliasearch-4.0.0b9/algoliasearch/analytics/models/get_top_countries_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/analytics/models/get_top_filter_attribute.py` & `algoliasearch-4.0.0b9/algoliasearch/analytics/models/get_top_filter_attribute.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/analytics/models/get_top_filter_attributes_response.py` & `algoliasearch-4.0.0b9/algoliasearch/analytics/models/get_top_filter_attributes_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/analytics/models/get_top_filter_for_attribute.py` & `algoliasearch-4.0.0b9/algoliasearch/analytics/models/get_top_filter_for_attribute.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/analytics/models/get_top_filter_for_attribute_response.py` & `algoliasearch-4.0.0b9/algoliasearch/analytics/models/get_top_filter_for_attribute_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/analytics/models/get_top_filters_no_results_response.py` & `algoliasearch-4.0.0b9/algoliasearch/analytics/models/get_top_filters_no_results_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/analytics/models/get_top_filters_no_results_value.py` & `algoliasearch-4.0.0b9/algoliasearch/analytics/models/get_top_filters_no_results_value.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/analytics/models/get_top_filters_no_results_values.py` & `algoliasearch-4.0.0b9/algoliasearch/analytics/models/get_top_filters_no_results_values.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/analytics/models/get_top_hits_response.py` & `algoliasearch-4.0.0b9/algoliasearch/analytics/models/get_top_hits_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/analytics/models/get_top_searches_response.py` & `algoliasearch-4.0.0b9/algoliasearch/analytics/models/get_top_searches_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/analytics/models/get_users_count_response.py` & `algoliasearch-4.0.0b9/algoliasearch/analytics/models/get_users_count_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/analytics/models/no_click_rate_event.py` & `algoliasearch-4.0.0b9/algoliasearch/analytics/models/no_click_rate_event.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/analytics/models/no_results_rate_event.py` & `algoliasearch-4.0.0b9/algoliasearch/analytics/models/no_results_rate_event.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/analytics/models/order_by.py` & `algoliasearch-4.0.0b9/algoliasearch/analytics/models/order_by.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/analytics/models/search_event.py` & `algoliasearch-4.0.0b9/algoliasearch/analytics/models/search_event.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/analytics/models/search_no_click_event.py` & `algoliasearch-4.0.0b9/algoliasearch/analytics/models/search_no_click_event.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/analytics/models/search_no_result_event.py` & `algoliasearch-4.0.0b9/algoliasearch/analytics/models/search_no_result_event.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/analytics/models/top_country.py` & `algoliasearch-4.0.0b9/algoliasearch/analytics/models/top_country.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/analytics/models/top_hit.py` & `algoliasearch-4.0.0b9/algoliasearch/analytics/models/top_hit.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/analytics/models/top_hit_with_analytics.py` & `algoliasearch-4.0.0b9/algoliasearch/analytics/models/top_hit_with_analytics.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/analytics/models/top_hits_response.py` & `algoliasearch-4.0.0b9/algoliasearch/analytics/models/top_hits_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/analytics/models/top_hits_response_with_analytics.py` & `algoliasearch-4.0.0b9/algoliasearch/analytics/models/top_hits_response_with_analytics.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/analytics/models/top_search.py` & `algoliasearch-4.0.0b9/algoliasearch/analytics/models/top_search.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/analytics/models/top_search_with_analytics.py` & `algoliasearch-4.0.0b9/algoliasearch/analytics/models/top_search_with_analytics.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/analytics/models/top_searches_response.py` & `algoliasearch-4.0.0b9/algoliasearch/analytics/models/top_searches_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/analytics/models/top_searches_response_with_analytics.py` & `algoliasearch-4.0.0b9/algoliasearch/analytics/models/top_searches_response_with_analytics.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/analytics/models/user_with_date.py` & `algoliasearch-4.0.0b9/algoliasearch/analytics/models/user_with_date.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/http/api_response.py` & `algoliasearch-4.0.0b9/algoliasearch/http/api_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/http/base_config.py` & `algoliasearch-4.0.0b9/algoliasearch/http/base_config.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/http/exceptions.py` & `algoliasearch-4.0.0b9/algoliasearch/http/exceptions.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/http/helpers.py` & `algoliasearch-4.0.0b9/algoliasearch/http/helpers.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/http/hosts.py` & `algoliasearch-4.0.0b9/algoliasearch/http/hosts.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/http/request_options.py` & `algoliasearch-4.0.0b9/algoliasearch/http/request_options.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/http/retry.py` & `algoliasearch-4.0.0b9/algoliasearch/http/retry.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/http/serializer.py` & `algoliasearch-4.0.0b9/algoliasearch/http/serializer.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/http/transporter.py` & `algoliasearch-4.0.0b9/algoliasearch/http/transporter.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/client.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/client.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/config.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/config.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/action_type.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/action_type.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/auth_algolia.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/auth_algolia.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/auth_algolia_partial.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/auth_algolia_partial.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/auth_api_key.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/auth_api_key.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/auth_api_key_partial.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/auth_api_key_partial.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/auth_basic.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/auth_basic.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/auth_basic_partial.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/auth_basic_partial.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/auth_google_service_account.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/auth_google_service_account.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/auth_google_service_account_partial.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/auth_google_service_account_partial.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/auth_input.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/auth_input.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/auth_input_partial.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/auth_input_partial.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/auth_o_auth.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/auth_o_auth.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/auth_o_auth_partial.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/auth_o_auth_partial.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/authentication.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/authentication.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/authentication_create.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/authentication_create.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/authentication_create_response.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/authentication_create_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/authentication_search.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/authentication_search.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/authentication_sort_keys.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/authentication_sort_keys.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/authentication_type.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/authentication_type.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/authentication_update.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/authentication_update.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/authentication_update_response.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/authentication_update_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/big_commerce_channel.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/big_commerce_channel.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/big_commerce_metafield.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/big_commerce_metafield.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/big_query_data_type.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/big_query_data_type.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/commercetools_custom_fields.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/commercetools_custom_fields.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/delete_response.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/delete_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/destination.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/destination.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/destination_create.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/destination_create.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/destination_create_response.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/destination_create_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/destination_index_name.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/destination_index_name.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/destination_index_prefix.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/destination_index_prefix.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/destination_input.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/destination_input.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/destination_search.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/destination_search.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/destination_sort_keys.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/destination_sort_keys.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/destination_type.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/destination_type.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/destination_update.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/destination_update.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/destination_update_response.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/destination_update_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/docker_image_type.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/docker_image_type.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/docker_registry.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/docker_registry.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/docker_source_discover.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/docker_source_discover.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/docker_source_streams.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/docker_source_streams.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/error_base.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/error_base.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/event.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/event.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/event_sort_keys.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/event_sort_keys.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/event_status.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/event_status.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/event_type.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/event_type.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/list_authentications_response.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/list_authentications_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/list_destinations_response.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/list_destinations_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/list_events_response.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/list_events_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/list_sources_response.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/list_sources_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/list_tasks_response.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/list_tasks_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/mapping_type_csv.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/mapping_type_csv.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/method_type.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/method_type.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/on_demand_date_utils_input.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/on_demand_date_utils_input.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,31 +2,34 @@
 
 """
 Code generated by OpenAPI Generator (https://openapi-generator.tech), manual changes will be lost - read more on https://github.com/algolia/api-clients-automation. DO NOT EDIT.
 """
 from __future__ import annotations
 
 from json import loads
-from typing import Any, Dict, Self
+from typing import Any, Dict, Optional, Self
 
 from pydantic import BaseModel, Field, StrictStr
 
+from algoliasearch.ingestion.models.mapping_input import MappingInput
+
 
 class OnDemandDateUtilsInput(BaseModel):
     """
     The input for an `onDemand` task whose source is of type `bigquery` and for which extracted data spans a given time range.
     """
 
     start_date: StrictStr = Field(
         description="The start date of the extraction (RFC3339 format).",
         alias="startDate",
     )
     end_date: StrictStr = Field(
         description="The end date of the extraction (RFC3339 format).", alias="endDate"
     )
+    mapping: Optional[MappingInput] = None
 
     model_config = {"populate_by_name": True, "validate_assignment": True}
 
     def to_json(self) -> str:
         return self.model_dump_json(by_alias=True, exclude_unset=True)
 
     @classmethod
@@ -45,22 +48,30 @@
           are ignored.
         """
         _dict = self.model_dump(
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
+        if self.mapping:
+            _dict["mapping"] = self.mapping.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of OnDemandDateUtilsInput from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate(
-            {"startDate": obj.get("startDate"), "endDate": obj.get("endDate")}
+            {
+                "startDate": obj.get("startDate"),
+                "endDate": obj.get("endDate"),
+                "mapping": MappingInput.from_dict(obj.get("mapping"))
+                if obj.get("mapping") is not None
+                else None,
+            }
         )
         return _obj
```

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/on_demand_trigger.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/on_demand_trigger.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/on_demand_trigger_input.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/on_demand_trigger_input.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/on_demand_trigger_type.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/on_demand_trigger_type.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/order_keys.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/order_keys.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/pagination.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/pagination.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/platform.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/platform.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/platform_none.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/platform_none.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/platform_with_none.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/platform_with_none.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/record_type.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/record_type.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/run.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/run.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/run_list_response.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/run_list_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/run_outcome.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/run_outcome.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/run_progress.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/run_progress.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/run_reason_code.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/run_reason_code.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/run_response.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/run_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/run_sort_keys.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/run_sort_keys.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/run_status.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/run_status.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/run_type.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/run_type.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/schedule_date_utils_input.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/schedule_date_utils_input.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,27 +2,30 @@
 
 """
 Code generated by OpenAPI Generator (https://openapi-generator.tech), manual changes will be lost - read more on https://github.com/algolia/api-clients-automation. DO NOT EDIT.
 """
 from __future__ import annotations
 
 from json import loads
-from typing import Annotated, Any, Dict, Self
+from typing import Annotated, Any, Dict, Optional, Self
 
 from pydantic import BaseModel, Field
 
+from algoliasearch.ingestion.models.mapping_input import MappingInput
+
 
 class ScheduleDateUtilsInput(BaseModel):
     """
     The input for a `schedule` task whose source is of type `bigquery` and for which extracted data spans a fixed number of days.
     """
 
     timeframe: Annotated[int, Field(le=30, strict=True, ge=1)] = Field(
         description="The timeframe of the extraction, in number of days from today."
     )
+    mapping: Optional[MappingInput] = None
 
     model_config = {"populate_by_name": True, "validate_assignment": True}
 
     def to_json(self) -> str:
         return self.model_dump_json(by_alias=True, exclude_unset=True)
 
     @classmethod
@@ -41,20 +44,29 @@
           are ignored.
         """
         _dict = self.model_dump(
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
+        if self.mapping:
+            _dict["mapping"] = self.mapping.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of ScheduleDateUtilsInput from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
-        _obj = cls.model_validate({"timeframe": obj.get("timeframe")})
+        _obj = cls.model_validate(
+            {
+                "timeframe": obj.get("timeframe"),
+                "mapping": MappingInput.from_dict(obj.get("mapping"))
+                if obj.get("mapping") is not None
+                else None,
+            }
+        )
         return _obj
```

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/schedule_trigger.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/schedule_trigger.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/schedule_trigger_input.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/schedule_trigger_input.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/schedule_trigger_type.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/schedule_trigger_type.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/source.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/source.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/source_big_commerce.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/source_big_commerce.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/source_big_query.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/source_big_query.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/source_commercetools.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/source_commercetools.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/source_create.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/source_create.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/source_create_response.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/source_create_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/source_csv.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/source_csv.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/source_docker.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/source_docker.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/source_input.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/source_input.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/source_json.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/source_json.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/source_search.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/source_search.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/source_sort_keys.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/source_sort_keys.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/source_type.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/source_type.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/source_update.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/source_update.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/source_update_commercetools.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/source_update_commercetools.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/source_update_docker.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/source_update_docker.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/source_update_input.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/source_update_input.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/source_update_response.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/source_update_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/subscription_trigger.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/subscription_trigger.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/subscription_trigger_type.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/subscription_trigger_type.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/task.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/task.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/task_create.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/task_create.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/task_create_response.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/task_create_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/task_create_trigger.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/task_create_trigger.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/task_input.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/task_input.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/task_search.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/task_search.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/task_sort_keys.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/task_sort_keys.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/task_update.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/task_update.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/task_update_response.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/task_update_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/trigger.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/trigger.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/trigger_type.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/trigger_type.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/trigger_update_input.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/trigger_update_input.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/ingestion/models/window.py` & `algoliasearch-4.0.0b9/algoliasearch/ingestion/models/window.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/insights/client.py` & `algoliasearch-4.0.0b9/algoliasearch/insights/client.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/insights/config.py` & `algoliasearch-4.0.0b9/algoliasearch/insights/config.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/insights/models/add_to_cart_event.py` & `algoliasearch-4.0.0b9/algoliasearch/insights/models/add_to_cart_event.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/insights/models/added_to_cart_object_ids.py` & `algoliasearch-4.0.0b9/algoliasearch/insights/models/added_to_cart_object_ids.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/insights/models/added_to_cart_object_ids_after_search.py` & `algoliasearch-4.0.0b9/algoliasearch/insights/models/added_to_cart_object_ids_after_search.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/insights/models/click_event.py` & `algoliasearch-4.0.0b9/algoliasearch/insights/models/click_event.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/insights/models/clicked_filters.py` & `algoliasearch-4.0.0b9/algoliasearch/insights/models/clicked_filters.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/insights/models/clicked_object_ids.py` & `algoliasearch-4.0.0b9/algoliasearch/insights/models/clicked_object_ids.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/insights/models/clicked_object_ids_after_search.py` & `algoliasearch-4.0.0b9/algoliasearch/insights/models/clicked_object_ids_after_search.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/insights/models/conversion_event.py` & `algoliasearch-4.0.0b9/algoliasearch/insights/models/conversion_event.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/insights/models/converted_filters.py` & `algoliasearch-4.0.0b9/algoliasearch/insights/models/converted_filters.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/insights/models/converted_object_ids.py` & `algoliasearch-4.0.0b9/algoliasearch/insights/models/converted_object_ids.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/insights/models/converted_object_ids_after_search.py` & `algoliasearch-4.0.0b9/algoliasearch/insights/models/converted_object_ids_after_search.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/insights/models/discount.py` & `algoliasearch-4.0.0b9/algoliasearch/insights/models/discount.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/insights/models/error_base.py` & `algoliasearch-4.0.0b9/algoliasearch/insights/models/error_base.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/insights/models/events_items.py` & `algoliasearch-4.0.0b9/algoliasearch/insights/models/events_items.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/insights/models/events_response.py` & `algoliasearch-4.0.0b9/algoliasearch/insights/models/events_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/insights/models/insights_events.py` & `algoliasearch-4.0.0b9/algoliasearch/insights/models/insights_events.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/insights/models/object_data.py` & `algoliasearch-4.0.0b9/algoliasearch/insights/models/object_data.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/insights/models/object_data_after_search.py` & `algoliasearch-4.0.0b9/algoliasearch/insights/models/object_data_after_search.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/insights/models/price.py` & `algoliasearch-4.0.0b9/algoliasearch/insights/models/price.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/insights/models/purchase_event.py` & `algoliasearch-4.0.0b9/algoliasearch/insights/models/purchase_event.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/insights/models/purchased_object_ids.py` & `algoliasearch-4.0.0b9/algoliasearch/insights/models/purchased_object_ids.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/insights/models/purchased_object_ids_after_search.py` & `algoliasearch-4.0.0b9/algoliasearch/insights/models/purchased_object_ids_after_search.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/insights/models/value.py` & `algoliasearch-4.0.0b9/algoliasearch/insights/models/value.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/insights/models/view_event.py` & `algoliasearch-4.0.0b9/algoliasearch/insights/models/view_event.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/insights/models/viewed_filters.py` & `algoliasearch-4.0.0b9/algoliasearch/insights/models/viewed_filters.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/insights/models/viewed_object_ids.py` & `algoliasearch-4.0.0b9/algoliasearch/insights/models/viewed_object_ids.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/monitoring/client.py` & `algoliasearch-4.0.0b9/algoliasearch/monitoring/client.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/monitoring/config.py` & `algoliasearch-4.0.0b9/algoliasearch/monitoring/config.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/monitoring/models/error_base.py` & `algoliasearch-4.0.0b9/algoliasearch/monitoring/models/error_base.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/monitoring/models/get_inventory403_response.py` & `algoliasearch-4.0.0b9/algoliasearch/monitoring/models/get_inventory403_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/monitoring/models/incident.py` & `algoliasearch-4.0.0b9/algoliasearch/monitoring/models/incident.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/monitoring/models/incidents_inner.py` & `algoliasearch-4.0.0b9/algoliasearch/monitoring/models/incidents_inner.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/monitoring/models/incidents_response.py` & `algoliasearch-4.0.0b9/algoliasearch/monitoring/models/incidents_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/monitoring/models/indexing_time_response.py` & `algoliasearch-4.0.0b9/algoliasearch/monitoring/models/indexing_time_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/monitoring/models/indexing_time_response_metrics.py` & `algoliasearch-4.0.0b9/algoliasearch/monitoring/models/indexing_time_response_metrics.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/monitoring/models/infrastructure_response.py` & `algoliasearch-4.0.0b9/algoliasearch/monitoring/models/infrastructure_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/monitoring/models/infrastructure_response_metrics.py` & `algoliasearch-4.0.0b9/algoliasearch/monitoring/models/infrastructure_response_metrics.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/monitoring/models/inventory_response.py` & `algoliasearch-4.0.0b9/algoliasearch/monitoring/models/inventory_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/monitoring/models/latency_response.py` & `algoliasearch-4.0.0b9/algoliasearch/monitoring/models/latency_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/monitoring/models/latency_response_metrics.py` & `algoliasearch-4.0.0b9/algoliasearch/monitoring/models/latency_response_metrics.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/monitoring/models/metric.py` & `algoliasearch-4.0.0b9/algoliasearch/monitoring/models/metric.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/monitoring/models/period.py` & `algoliasearch-4.0.0b9/algoliasearch/monitoring/models/period.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/monitoring/models/probes_metric.py` & `algoliasearch-4.0.0b9/algoliasearch/monitoring/models/probes_metric.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/monitoring/models/region.py` & `algoliasearch-4.0.0b9/algoliasearch/monitoring/models/region.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/monitoring/models/server.py` & `algoliasearch-4.0.0b9/algoliasearch/monitoring/models/server.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/monitoring/models/server_status.py` & `algoliasearch-4.0.0b9/algoliasearch/monitoring/models/server_status.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/monitoring/models/status.py` & `algoliasearch-4.0.0b9/algoliasearch/monitoring/models/status.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/monitoring/models/status_response.py` & `algoliasearch-4.0.0b9/algoliasearch/monitoring/models/status_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/monitoring/models/time_inner.py` & `algoliasearch-4.0.0b9/algoliasearch/monitoring/models/time_inner.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/monitoring/models/type.py` & `algoliasearch-4.0.0b9/algoliasearch/monitoring/models/type.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/personalization/client.py` & `algoliasearch-4.0.0b9/algoliasearch/personalization/client.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/personalization/config.py` & `algoliasearch-4.0.0b9/algoliasearch/personalization/config.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/personalization/models/delete_user_profile_response.py` & `algoliasearch-4.0.0b9/algoliasearch/personalization/models/delete_user_profile_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/personalization/models/error_base.py` & `algoliasearch-4.0.0b9/algoliasearch/personalization/models/error_base.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/personalization/models/event_scoring.py` & `algoliasearch-4.0.0b9/algoliasearch/personalization/models/event_scoring.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/personalization/models/facet_scoring.py` & `algoliasearch-4.0.0b9/algoliasearch/personalization/models/facet_scoring.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/personalization/models/get_user_token_response.py` & `algoliasearch-4.0.0b9/algoliasearch/personalization/models/get_user_token_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/personalization/models/personalization_strategy_params.py` & `algoliasearch-4.0.0b9/algoliasearch/personalization/models/personalization_strategy_params.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/personalization/models/set_personalization_strategy_response.py` & `algoliasearch-4.0.0b9/algoliasearch/personalization/models/set_personalization_strategy_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/query_suggestions/client.py` & `algoliasearch-4.0.0b9/algoliasearch/query_suggestions/client.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/query_suggestions/config.py` & `algoliasearch-4.0.0b9/algoliasearch/query_suggestions/config.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/query_suggestions/models/base_query_suggestions_configuration_response.py` & `algoliasearch-4.0.0b9/algoliasearch/query_suggestions/models/base_query_suggestions_configuration_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/query_suggestions/models/base_query_suggestions_configuration_with_index.py` & `algoliasearch-4.0.0b9/algoliasearch/query_suggestions/models/base_query_suggestions_configuration_with_index.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/query_suggestions/models/base_response.py` & `algoliasearch-4.0.0b9/algoliasearch/query_suggestions/models/base_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/query_suggestions/models/error_base.py` & `algoliasearch-4.0.0b9/algoliasearch/query_suggestions/models/error_base.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/query_suggestions/models/facet.py` & `algoliasearch-4.0.0b9/algoliasearch/query_suggestions/models/facet.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/query_suggestions/models/get_config_status200_response.py` & `algoliasearch-4.0.0b9/algoliasearch/query_suggestions/models/get_config_status200_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/query_suggestions/models/get_log_file200_response.py` & `algoliasearch-4.0.0b9/algoliasearch/query_suggestions/models/get_log_file200_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/query_suggestions/models/languages.py` & `algoliasearch-4.0.0b9/algoliasearch/query_suggestions/models/languages.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/query_suggestions/models/log_level.py` & `algoliasearch-4.0.0b9/algoliasearch/query_suggestions/models/log_level.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/query_suggestions/models/query_suggestions_configuration.py` & `algoliasearch-4.0.0b9/algoliasearch/query_suggestions/models/query_suggestions_configuration.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/query_suggestions/models/query_suggestions_configuration_response.py` & `algoliasearch-4.0.0b9/algoliasearch/query_suggestions/models/query_suggestions_configuration_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/query_suggestions/models/query_suggestions_configuration_with_index.py` & `algoliasearch-4.0.0b9/algoliasearch/query_suggestions/models/query_suggestions_configuration_with_index.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/query_suggestions/models/source_index.py` & `algoliasearch-4.0.0b9/algoliasearch/query_suggestions/models/source_index.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/client.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/client.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/config.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/config.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/advanced_syntax_features.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/advanced_syntax_features.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/alternatives_as_exact.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/alternatives_as_exact.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/anchoring.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/anchoring.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/around_precision.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/around_precision.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/around_precision_from_value_inner.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/around_precision_from_value_inner.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/around_radius.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/around_radius.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/around_radius_all.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/around_radius_all.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/automatic_facet_filter.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/automatic_facet_filter.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/automatic_facet_filters.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/automatic_facet_filters.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/base_recommend_request.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/base_recommend_request.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/base_recommendations_query.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/base_recommendations_query.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/base_recommended_for_you_query.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/base_recommended_for_you_query.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/base_recommended_for_you_query_parameters.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/base_recommended_for_you_query_parameters.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/base_search_params.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/base_search_params.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/base_search_params_without_query.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/base_search_params_without_query.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/base_search_response.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/base_search_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/base_trending_facets_query.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/base_trending_facets_query.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/base_trending_items_query.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/base_trending_items_query.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/condition.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/condition.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/consequence.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/consequence.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/consequence_hide.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/consequence_hide.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/consequence_params.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/consequence_params.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/consequence_query.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/consequence_query.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/consequence_query_object.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/consequence_query_object.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/deleted_at_response.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/deleted_at_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/distinct.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/distinct.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/edit.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/edit.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/edit_type.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/edit_type.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/error_base.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/error_base.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/exact_on_single_word_query.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/exact_on_single_word_query.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/exhaustive.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/exhaustive.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/facet_filters.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/facet_filters.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/facet_ordering.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/facet_ordering.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/facets.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/facets.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/facets_stats.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/facets_stats.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/get_recommend_task_response.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/get_recommend_task_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/get_recommendations_params.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/get_recommendations_params.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/get_recommendations_response.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/get_recommendations_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/highlight_result.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/highlight_result.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/highlight_result_option.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/highlight_result_option.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/ignore_plurals.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/ignore_plurals.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/index_settings_as_search_params.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/index_settings_as_search_params.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/match_level.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/match_level.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/matched_geo_location.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/matched_geo_location.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/mixed_search_filters.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/mixed_search_filters.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/mode.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/mode.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/numeric_filters.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/numeric_filters.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/optional_filters.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/optional_filters.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/params.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/params.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/personalization.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/personalization.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/promote.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/promote.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/promote_object_id.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/promote_object_id.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/promote_object_ids.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/promote_object_ids.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/query_type.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/query_type.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/ranking_info.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/ranking_info.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/re_ranking_apply_filter.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/re_ranking_apply_filter.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/recommend_hit.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/recommend_hit.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/recommend_models.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/recommend_models.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/recommendation_models.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/recommendation_models.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/recommendations_hit.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/recommendations_hit.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/recommendations_hits.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/recommendations_hits.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/recommendations_query.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/recommendations_query.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/recommendations_request.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/recommendations_request.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/recommendations_results.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/recommendations_results.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/recommended_for_you_model.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/recommended_for_you_model.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/recommended_for_you_query.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/recommended_for_you_query.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/recommended_for_you_query_parameters.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/recommended_for_you_query_parameters.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/redirect.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/redirect.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/redirect_rule_index_metadata.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/redirect_rule_index_metadata.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/redirect_rule_index_metadata_data.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/redirect_rule_index_metadata_data.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/remove_stop_words.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/remove_stop_words.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/remove_words_if_no_results.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/remove_words_if_no_results.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/rendering_content.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/rendering_content.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/rule_response.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/rule_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/rule_response_metadata.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/rule_response_metadata.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/search_params_object.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/search_params_object.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/search_params_query.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/search_params_query.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/search_recommend_rules_params.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/search_recommend_rules_params.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/search_recommend_rules_response.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/search_recommend_rules_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/semantic_search.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/semantic_search.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/snippet_result.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/snippet_result.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/snippet_result_option.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/snippet_result_option.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/sort_remaining_by.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/sort_remaining_by.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/tag_filters.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/tag_filters.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/task_status.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/task_status.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/trending_facet_hit.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/trending_facet_hit.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/trending_facets_model.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/trending_facets_model.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/trending_facets_query.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/trending_facets_query.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/trending_items_model.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/trending_items_model.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/trending_items_query.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/trending_items_query.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/typo_tolerance.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/typo_tolerance.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/typo_tolerance_enum.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/typo_tolerance_enum.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/recommend/models/value.py` & `algoliasearch-4.0.0b9/algoliasearch/recommend/models/value.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/client.py` & `algoliasearch-4.0.0b9/algoliasearch/search/client.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/config.py` & `algoliasearch-4.0.0b9/algoliasearch/search/config.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/acl.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/acl.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/action.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/action.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/add_api_key_response.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/add_api_key_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/advanced_syntax_features.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/advanced_syntax_features.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/alternatives_as_exact.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/alternatives_as_exact.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/anchoring.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/anchoring.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/api_key.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/api_key.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/api_key_operation.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/api_key_operation.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/around_precision.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/around_precision.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/around_precision_from_value_inner.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/around_precision_from_value_inner.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/around_radius.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/around_radius.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/around_radius_all.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/around_radius_all.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/assign_user_id_params.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/assign_user_id_params.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/attribute_to_update.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/attribute_to_update.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/automatic_facet_filter.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/automatic_facet_filter.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/automatic_facet_filters.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/automatic_facet_filters.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/base_get_api_key_response.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/base_get_api_key_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/base_index_settings.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/base_index_settings.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/base_search_params.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/base_search_params.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/base_search_params_without_query.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/base_search_params_without_query.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/base_search_response.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/base_search_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/batch_assign_user_ids_params.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/batch_assign_user_ids_params.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/batch_dictionary_entries_params.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/batch_dictionary_entries_params.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/batch_dictionary_entries_request.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/batch_dictionary_entries_request.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/batch_params.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/batch_params.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/batch_request.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/batch_request.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/batch_response.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/batch_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/batch_write_params.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/batch_write_params.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/browse_params.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/browse_params.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/browse_params_object.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/browse_params_object.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/browse_response.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/browse_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/built_in_operation.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/built_in_operation.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/built_in_operation_type.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/built_in_operation_type.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/condition.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/condition.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/consequence.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/consequence.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/consequence_hide.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/consequence_hide.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/consequence_params.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/consequence_params.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/consequence_query.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/consequence_query.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/consequence_query_object.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/consequence_query_object.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/created_at_response.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/created_at_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/cursor.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/cursor.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/delete_api_key_response.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/delete_api_key_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/delete_by_params.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/delete_by_params.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/delete_source_response.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/delete_source_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/deleted_at_response.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/deleted_at_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/dictionary_action.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/dictionary_action.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/dictionary_entry.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/dictionary_entry.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/dictionary_entry_state.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/dictionary_entry_state.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/dictionary_language.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/dictionary_language.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/dictionary_settings_params.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/dictionary_settings_params.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/dictionary_type.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/dictionary_type.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/distinct.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/distinct.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/edit.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/edit.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/edit_type.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/edit_type.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/error_base.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/error_base.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/exact_on_single_word_query.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/exact_on_single_word_query.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/exhaustive.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/exhaustive.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/facet_filters.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/facet_filters.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/facet_hits.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/facet_hits.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/facet_ordering.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/facet_ordering.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/facets.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/facets.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/facets_stats.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/facets_stats.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/fetched_index.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/fetched_index.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/get_api_key_response.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/get_api_key_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/get_dictionary_settings_response.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/get_dictionary_settings_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/get_logs_response.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/get_logs_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/get_objects_params.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/get_objects_params.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/get_objects_request.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/get_objects_request.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/get_objects_response.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/get_objects_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/get_task_response.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/get_task_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/get_top_user_ids_response.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/get_top_user_ids_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/has_pending_mappings_response.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/has_pending_mappings_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/highlight_result.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/highlight_result.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/highlight_result_option.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/highlight_result_option.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/hit.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/hit.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/ignore_plurals.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/ignore_plurals.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/index_settings.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/index_settings.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/index_settings_as_search_params.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/index_settings_as_search_params.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/languages.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/languages.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/list_api_keys_response.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/list_api_keys_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/list_clusters_response.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/list_clusters_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/list_indices_response.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/list_indices_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/list_user_ids_response.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/list_user_ids_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/log.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/log.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/log_query.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/log_query.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/log_type.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/log_type.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/match_level.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/match_level.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/matched_geo_location.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/matched_geo_location.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/mixed_search_filters.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/mixed_search_filters.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/mode.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/mode.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/multiple_batch_request.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/multiple_batch_request.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/multiple_batch_response.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/multiple_batch_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/numeric_filters.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/numeric_filters.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/operation_index_params.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/operation_index_params.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/operation_type.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/operation_type.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/optional_filters.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/optional_filters.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/params.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/params.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/personalization.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/personalization.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/promote.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/promote.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/promote_object_id.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/promote_object_id.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/promote_object_ids.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/promote_object_ids.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/query_type.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/query_type.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/ranking_info.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/ranking_info.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/re_ranking_apply_filter.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/re_ranking_apply_filter.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/redirect.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/redirect.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/redirect_rule_index_metadata.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/redirect_rule_index_metadata.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/redirect_rule_index_metadata_data.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/redirect_rule_index_metadata_data.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/remove_stop_words.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/remove_stop_words.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/remove_user_id_response.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/remove_user_id_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/remove_words_if_no_results.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/remove_words_if_no_results.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/rendering_content.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/rendering_content.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/replace_source_response.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/replace_source_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/rule.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/rule.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/save_object_response.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/save_object_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/save_synonym_response.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/save_synonym_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/scope_type.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/scope_type.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/search_dictionary_entries_params.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/search_dictionary_entries_params.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/search_for_facet_values_request.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/search_for_facet_values_request.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/search_for_facet_values_response.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/search_for_facet_values_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/search_for_facets.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/search_for_facets.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/search_for_facets_options.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/search_for_facets_options.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/search_for_hits.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/search_for_hits.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/search_for_hits_options.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/search_for_hits_options.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/search_hits.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/search_hits.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/search_method_params.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/search_method_params.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/search_params.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/search_params.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/search_params_object.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/search_params_object.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/search_params_query.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/search_params_query.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/search_params_string.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/search_params_string.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/search_query.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/search_query.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/search_response.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/search_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/search_responses.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/search_responses.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/search_result.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/search_result.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/search_rules_params.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/search_rules_params.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/search_rules_response.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/search_rules_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/search_strategy.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/search_strategy.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/search_synonyms_params.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/search_synonyms_params.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/search_synonyms_response.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/search_synonyms_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/search_type_default.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/search_type_default.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/search_type_facet.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/search_type_facet.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/search_user_ids_params.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/search_user_ids_params.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/search_user_ids_response.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/search_user_ids_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/secured_api_key_restrictions.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/secured_api_key_restrictions.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/semantic_search.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/semantic_search.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/snippet_result.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/snippet_result.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/snippet_result_option.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/snippet_result_option.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/sort_remaining_by.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/sort_remaining_by.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/source.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/source.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/standard_entries.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/standard_entries.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/synonym_hit.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/synonym_hit.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/synonym_type.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/synonym_type.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/tag_filters.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/tag_filters.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/task_status.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/task_status.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/time_range.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/time_range.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/typo_tolerance.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/typo_tolerance.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/typo_tolerance_enum.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/typo_tolerance_enum.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/update_api_key_response.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/update_api_key_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/updated_at_response.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/updated_at_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/updated_at_with_object_id_response.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/updated_at_with_object_id_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/updated_rule_response.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/updated_rule_response.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/user_highlight_result.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/user_highlight_result.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/user_hit.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/user_hit.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/user_id.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/user_id.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/algoliasearch/search/models/value.py` & `algoliasearch-4.0.0b9/algoliasearch/search/models/value.py`

 * *Files identical despite different names*

### Comparing `algoliasearch-4.0.0b8/pyproject.toml` & `algoliasearch-4.0.0b9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "algoliasearch"
-version = "4.0.0b8"
+version = "4.0.0b9"
 description = "A fully-featured and blazing-fast Python API client to interact with Algolia."
 authors = ["Algolia Team <support@algolia.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://www.algolia.com"
 repository = "https://github.com/algolia/algoliasearch-client-python"
 keywords = ["algolia", "search", "full-text-search", "neural-search"]
```

### Comparing `algoliasearch-4.0.0b8/PKG-INFO` & `algoliasearch-4.0.0b9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algoliasearch
-Version: 4.0.0b8
+Version: 4.0.0b9
 Summary: A fully-featured and blazing-fast Python API client to interact with Algolia.
 Home-page: https://www.algolia.com
 License: MIT
 Keywords: algolia,search,full-text-search,neural-search
 Author: Algolia Team
 Author-email: support@algolia.com
 Requires-Python: >=3.8.1,<4.0.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: algoliasearch Version: 4.0.0b8 Summary: A fully-
+Metadata-Version: 2.1 Name: algoliasearch Version: 4.0.0b9 Summary: A fully-
 featured and blazing-fast Python API client to interact with Algolia. Home-
 page: https://www.algolia.com License: MIT Keywords: algolia,search,full-text-
 search,neural-search Author: Algolia Team Author-email: support@algolia.com
 Requires-Python: >=3.8.1,<4.0.0 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
```

