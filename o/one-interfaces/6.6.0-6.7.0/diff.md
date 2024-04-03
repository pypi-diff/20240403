# Comparing `tmp/one_interfaces-6.6.0.tar.gz` & `tmp/one_interfaces-6.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\one_interfaces-6.6.0.tar", last modified: Fri Mar 29 15:40:42 2024, max compression
+gzip compressed data, was "dist\one_interfaces-6.7.0.tar", last modified: Wed Apr  3 13:42:35 2024, max compression
```

## Comparing `one_interfaces-6.6.0.tar` & `one_interfaces-6.7.0.tar`

### file list

```diff
@@ -1,192 +1,194 @@
-drwxrwxrwx   0        0        0        0 2024-03-29 15:40:42.437103 one_interfaces-6.6.0/
--rw-rw-rw-   0        0        0      580 2022-07-05 14:29:22.000000 one_interfaces-6.6.0/LICENSE.txt
--rw-rw-rw-   0        0        0       62 2022-07-05 14:29:22.000000 one_interfaces-6.6.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1217 2024-03-29 15:40:42.438109 one_interfaces-6.6.0/PKG-INFO
--rw-rw-rw-   0        0        0      394 2022-11-11 17:33:49.000000 one_interfaces-6.6.0/README.md
-drwxrwxrwx   0        0        0        0 2024-03-29 15:40:42.422100 one_interfaces-6.6.0/one_interfaces/
--rw-rw-rw-   0        0        0       23 2024-03-29 15:17:04.000000 one_interfaces-6.6.0/one_interfaces/__init__.py
--rw-rw-rw-   0        0        0     1670 2024-03-29 15:29:26.000000 one_interfaces-6.6.0/one_interfaces/account_status_pb2.py
--rw-rw-rw-   0        0        0     2440 2024-03-29 15:29:26.000000 one_interfaces-6.6.0/one_interfaces/activity_pb2.py
--rw-rw-rw-   0        0        0     1899 2024-03-29 15:29:26.000000 one_interfaces-6.6.0/one_interfaces/activity_type_pb2.py
--rw-rw-rw-   0        0        0     2231 2024-03-29 15:29:27.000000 one_interfaces-6.6.0/one_interfaces/address_pb2.py
--rw-rw-rw-   0        0        0     1681 2024-03-29 15:29:27.000000 one_interfaces-6.6.0/one_interfaces/agency_pb2.py
--rw-rw-rw-   0        0        0     1874 2024-03-29 15:29:27.000000 one_interfaces-6.6.0/one_interfaces/analyte_pb2.py
--rw-rw-rw-   0        0        0     2811 2024-03-29 15:29:27.000000 one_interfaces-6.6.0/one_interfaces/analyte_result_pb2.py
--rw-rw-rw-   0        0        0     1769 2024-03-29 15:29:27.000000 one_interfaces-6.6.0/one_interfaces/analyte_results_import_profile_pb2.py
--rw-rw-rw-   0        0        0     1758 2024-03-29 15:29:27.000000 one_interfaces-6.6.0/one_interfaces/analyte_results_import_telemetry_pb2.py
--rw-rw-rw-   0        0        0     1223 2024-03-29 15:29:27.000000 one_interfaces-6.6.0/one_interfaces/apierror_pb2.py
--rw-rw-rw-   0        0        0     1393 2024-03-29 15:29:27.000000 one_interfaces-6.6.0/one_interfaces/apiresponse_pb2.py
--rw-rw-rw-   0        0        0     1941 2024-03-29 15:29:27.000000 one_interfaces-6.6.0/one_interfaces/auditevent_pb2.py
--rw-rw-rw-   0        0        0     1474 2024-03-29 15:29:27.000000 one_interfaces-6.6.0/one_interfaces/cell_monitor_backup_pb2.py
--rw-rw-rw-   0        0        0     1519 2024-03-29 15:29:27.000000 one_interfaces-6.6.0/one_interfaces/cell_pb2.py
--rw-rw-rw-   0        0        0     1541 2024-03-29 15:29:27.000000 one_interfaces-6.6.0/one_interfaces/celldata_binding_pb2.py
--rw-rw-rw-   0        0        0     1988 2024-03-29 15:29:27.000000 one_interfaces-6.6.0/one_interfaces/celldata_pb2.py
--rw-rw-rw-   0        0        0     1534 2024-03-29 15:29:27.000000 one_interfaces-6.6.0/one_interfaces/cells_pb2.py
--rw-rw-rw-   0        0        0     1871 2024-03-29 15:29:27.000000 one_interfaces-6.6.0/one_interfaces/cellvalue_backup_pb2.py
--rw-rw-rw-   0        0        0     4778 2024-03-29 15:29:27.000000 one_interfaces-6.6.0/one_interfaces/client_pb2.py
--rw-rw-rw-   0        0        0     2054 2024-03-29 15:29:27.000000 one_interfaces-6.6.0/one_interfaces/coagmeasurement_pb2.py
--rw-rw-rw-   0        0        0     2429 2024-03-29 15:29:27.000000 one_interfaces-6.6.0/one_interfaces/column_pb2.py
--rw-rw-rw-   0        0        0     2097 2024-03-29 15:29:27.000000 one_interfaces-6.6.0/one_interfaces/computation_binding_pb2.py
--rw-rw-rw-   0        0        0     2564 2024-03-29 15:29:27.000000 one_interfaces-6.6.0/one_interfaces/computation_pb2.py
--rw-rw-rw-   0        0        0     1893 2024-03-29 15:29:27.000000 one_interfaces-6.6.0/one_interfaces/computation_variable_binding_pb2.py
--rw-rw-rw-   0        0        0     2027 2024-03-29 15:29:28.000000 one_interfaces-6.6.0/one_interfaces/configuration_note_pb2.py
--rw-rw-rw-   0        0        0     2970 2024-03-29 15:29:27.000000 one_interfaces-6.6.0/one_interfaces/configuration_pb2.py
--rw-rw-rw-   0        0        0     1499 2024-03-29 15:29:28.000000 one_interfaces-6.6.0/one_interfaces/configuration_tag_pb2.py
--rw-rw-rw-   0        0        0    13264 2024-03-29 15:29:28.000000 one_interfaces-6.6.0/one_interfaces/content_pb2.py
--rw-rw-rw-   0        0        0     1951 2024-03-29 15:29:28.000000 one_interfaces-6.6.0/one_interfaces/csv_configuration_file_pb2.py
--rw-rw-rw-   0        0        0     1743 2024-03-29 15:29:28.000000 one_interfaces-6.6.0/one_interfaces/data_source_binding_pb2.py
--rw-rw-rw-   0        0        0     2052 2024-03-29 15:29:28.000000 one_interfaces-6.6.0/one_interfaces/data_source_configuration_pb2.py
--rw-rw-rw-   0        0        0     1536 2024-03-29 15:29:28.000000 one_interfaces-6.6.0/one_interfaces/digital_twin_column_telemetry_propertybag_pb2.py
--rw-rw-rw-   0        0        0     2041 2024-03-29 15:29:28.000000 one_interfaces-6.6.0/one_interfaces/digital_twin_enterprise_data_telemetry_pb2.py
--rw-rw-rw-   0        0        0     1523 2024-03-29 15:29:28.000000 one_interfaces-6.6.0/one_interfaces/digital_twin_instrument_telemetry_propertybag_pb2.py
--rw-rw-rw-   0        0        0     3269 2024-03-29 15:29:28.000000 one_interfaces-6.6.0/one_interfaces/digital_twin_pb2.py
--rw-rw-rw-   0        0        0     2247 2024-03-29 15:29:28.000000 one_interfaces-6.6.0/one_interfaces/digital_twin_subtype_pb2.py
--rw-rw-rw-   0        0        0     3800 2024-03-29 15:29:28.000000 one_interfaces-6.6.0/one_interfaces/digital_twin_subtype_propertybag_pb2.py
--rw-rw-rw-   0        0        0     2063 2024-03-29 15:29:28.000000 one_interfaces-6.6.0/one_interfaces/digital_twin_type_pb2.py
--rw-rw-rw-   0        0        0     2020 2024-03-29 15:29:28.000000 one_interfaces-6.6.0/one_interfaces/digital_twin_user_right_pb2.py
--rw-rw-rw-   0        0        0     1342 2024-03-29 15:29:28.000000 one_interfaces-6.6.0/one_interfaces/display_options_pb2.py
--rw-rw-rw-   0        0        0     1820 2024-03-29 15:29:28.000000 one_interfaces-6.6.0/one_interfaces/enterprise_data_source_definition_pb2.py
--rw-rw-rw-   0        0        0     1669 2024-03-29 15:29:28.000000 one_interfaces-6.6.0/one_interfaces/enterprise_data_table_definition_pb2.py
--rw-rw-rw-   0        0        0     1376 2024-03-29 15:29:28.000000 one_interfaces-6.6.0/one_interfaces/enterprise_data_table_field_pb2.py
--rw-rw-rw-   0        0        0     1605 2024-03-29 15:29:28.000000 one_interfaces-6.6.0/one_interfaces/enterprise_data_table_query_parameter_pb2.py
--rw-rw-rw-   0        0        0     1508 2024-03-29 15:29:28.000000 one_interfaces-6.6.0/one_interfaces/enterprise_data_table_query_pb2.py
--rw-rw-rw-   0        0        0     2309 2024-03-29 15:29:28.000000 one_interfaces-6.6.0/one_interfaces/enterprise_dataset_definition_pb2.py
--rw-rw-rw-   0        0        0     1303 2024-03-29 15:29:28.000000 one_interfaces-6.6.0/one_interfaces/enum_aggregate_pb2.py
--rw-rw-rw-   0        0        0     1408 2024-03-29 15:29:29.000000 one_interfaces-6.6.0/one_interfaces/enum_auditevent_pb2.py
--rw-rw-rw-   0        0        0     1385 2024-03-29 15:29:29.000000 one_interfaces-6.6.0/one_interfaces/enum_azure_notification_hubtype_pb2.py
--rw-rw-rw-   0        0        0     1642 2024-03-29 15:29:29.000000 one_interfaces-6.6.0/one_interfaces/enum_cell_range_action_pb2.py
--rw-rw-rw-   0        0        0     1730 2024-03-29 15:29:29.000000 one_interfaces-6.6.0/one_interfaces/enum_datasource_pb2.py
--rw-rw-rw-   0        0        0     1392 2024-03-29 15:29:29.000000 one_interfaces-6.6.0/one_interfaces/enum_day_pb2.py
--rw-rw-rw-   0        0        0     1515 2024-03-29 15:29:29.000000 one_interfaces-6.6.0/one_interfaces/enum_digital_twin_dataset_output_format_pb2.py
--rw-rw-rw-   0        0        0     1381 2024-03-29 15:29:29.000000 one_interfaces-6.6.0/one_interfaces/enum_digital_twin_restriction_pb2.py
--rw-rw-rw-   0        0        0     1422 2024-03-29 15:29:29.000000 one_interfaces-6.6.0/one_interfaces/enum_digital_twin_user_right_pb2.py
--rw-rw-rw-   0        0        0     1339 2024-03-29 15:29:29.000000 one_interfaces-6.6.0/one_interfaces/enum_domain_source_pb2.py
--rw-rw-rw-   0        0        0     1373 2024-03-29 15:29:29.000000 one_interfaces-6.6.0/one_interfaces/enum_entity_pb2.py
--rw-rw-rw-   0        0        0     1433 2024-03-29 15:29:29.000000 one_interfaces-6.6.0/one_interfaces/enum_identity_provider_pb2.py
--rw-rw-rw-   0        0        0     1552 2024-03-29 15:29:29.000000 one_interfaces-6.6.0/one_interfaces/enum_import_status_pb2.py
--rw-rw-rw-   0        0        0     1416 2024-03-29 15:29:29.000000 one_interfaces-6.6.0/one_interfaces/enum_limit_operation_pb2.py
--rw-rw-rw-   0        0        0     1394 2024-03-29 15:29:29.000000 one_interfaces-6.6.0/one_interfaces/enum_limit_pb2.py
--rw-rw-rw-   0        0        0     1545 2024-03-29 15:29:29.000000 one_interfaces-6.6.0/one_interfaces/enum_month_pb2.py
--rw-rw-rw-   0        0        0     1606 2024-03-29 15:29:29.000000 one_interfaces-6.6.0/one_interfaces/enum_notification_category_pb2.py
--rw-rw-rw-   0        0        0     1557 2024-03-29 15:29:29.000000 one_interfaces-6.6.0/one_interfaces/enum_notification_delivery_method_pb2.py
--rw-rw-rw-   0        0        0     1427 2024-03-29 15:29:29.000000 one_interfaces-6.6.0/one_interfaces/enum_notification_message_type_pb2.py
--rw-rw-rw-   0        0        0     1346 2024-03-29 15:29:29.000000 one_interfaces-6.6.0/one_interfaces/enum_notification_platform_pb2.py
--rw-rw-rw-   0        0        0     1452 2024-03-29 15:29:29.000000 one_interfaces-6.6.0/one_interfaces/enum_one_log_level_pb2.py
--rw-rw-rw-   0        0        0     1374 2024-03-29 15:29:29.000000 one_interfaces-6.6.0/one_interfaces/enum_output_placement_pb2.py
--rw-rw-rw-   0        0        0     1269 2024-03-29 15:29:29.000000 one_interfaces-6.6.0/one_interfaces/enum_rendering_engine_pb2.py
--rw-rw-rw-   0        0        0     1681 2024-03-29 15:29:29.000000 one_interfaces-6.6.0/one_interfaces/enum_reportable_qualifier_definition_pb2.py
--rw-rw-rw-   0        0        0     1663 2024-03-29 15:29:29.000000 one_interfaces-6.6.0/one_interfaces/enum_reportable_qualifier_pb2.py
--rw-rw-rw-   0        0        0     3080 2024-03-29 15:29:29.000000 one_interfaces-6.6.0/one_interfaces/enum_sampling_statistic_pb2.py
--rw-rw-rw-   0        0        0     1483 2024-03-29 15:29:29.000000 one_interfaces-6.6.0/one_interfaces/enum_time_context_pb2.py
--rw-rw-rw-   0        0        0     1388 2024-03-29 15:29:29.000000 one_interfaces-6.6.0/one_interfaces/enum_time_unit_pb2.py
--rw-rw-rw-   0        0        0    27482 2024-03-29 15:29:29.000000 one_interfaces-6.6.0/one_interfaces/enum_timezone_pb2.py
--rw-rw-rw-   0        0        0     1415 2024-03-29 15:29:29.000000 one_interfaces-6.6.0/one_interfaces/enum_valid_value_restriction_pb2.py
--rw-rw-rw-   0        0        0     1376 2024-03-29 15:29:30.000000 one_interfaces-6.6.0/one_interfaces/enum_variable_type_pb2.py
--rw-rw-rw-   0        0        0     2357 2024-03-29 15:29:30.000000 one_interfaces-6.6.0/one_interfaces/enum_wims_week_definition_pb2.py
--rw-rw-rw-   0        0        0     1341 2024-03-29 15:29:30.000000 one_interfaces-6.6.0/one_interfaces/enum_worksheet_pb2.py
--rw-rw-rw-   0        0        0     1768 2024-03-29 15:29:30.000000 one_interfaces-6.6.0/one_interfaces/execution_details_pb2.py
--rw-rw-rw-   0        0        0     1211 2024-03-29 15:29:30.000000 one_interfaces-6.6.0/one_interfaces/expression_line_pb2.py
--rw-rw-rw-   0        0        0     2205 2024-03-29 15:29:30.000000 one_interfaces-6.6.0/one_interfaces/feature_pb2.py
--rw-rw-rw-   0        0        0     1589 2024-03-29 15:29:30.000000 one_interfaces-6.6.0/one_interfaces/feature_state_type_pb2.py
--rw-rw-rw-   0        0        0     1793 2024-03-29 15:29:30.000000 one_interfaces-6.6.0/one_interfaces/file_configuration_pb2.py
--rw-rw-rw-   0        0        0     1563 2024-03-29 15:29:30.000000 one_interfaces-6.6.0/one_interfaces/gauge_data_point_pb2.py
--rw-rw-rw-   0        0        0     1560 2024-03-29 15:29:30.000000 one_interfaces-6.6.0/one_interfaces/gis_pb2.py
--rw-rw-rw-   0        0        0     1231 2024-03-29 15:29:30.000000 one_interfaces-6.6.0/one_interfaces/historian_binding_pb2.py
--rw-rw-rw-   0        0        0     1981 2024-03-29 15:29:30.000000 one_interfaces-6.6.0/one_interfaces/historian_data_pb2.py
--rw-rw-rw-   0        0        0     1536 2024-03-29 15:29:30.000000 one_interfaces-6.6.0/one_interfaces/i18nkey_text_reference_pb2.py
--rw-rw-rw-   0        0        0     1855 2024-03-29 15:29:30.000000 one_interfaces-6.6.0/one_interfaces/ingest_client_pb2.py
--rw-rw-rw-   0        0        0     1698 2024-03-29 15:29:30.000000 one_interfaces-6.6.0/one_interfaces/jsonTicksDateTime_pb2.py
--rw-rw-rw-   0        0        0     1325 2024-03-29 15:29:30.000000 one_interfaces-6.6.0/one_interfaces/key_value_pb2.py
--rw-rw-rw-   0        0        0     1668 2024-03-29 15:29:30.000000 one_interfaces-6.6.0/one_interfaces/limit_configuration_pb2.py
--rw-rw-rw-   0        0        0     2385 2024-03-29 15:29:30.000000 one_interfaces-6.6.0/one_interfaces/limit_pb2.py
--rw-rw-rw-   0        0        0     1948 2024-03-29 15:29:30.000000 one_interfaces-6.6.0/one_interfaces/measurement_pb2.py
--rw-rw-rw-   0        0        0     2412 2024-03-29 15:29:30.000000 one_interfaces-6.6.0/one_interfaces/model_execution_pb2.py
--rw-rw-rw-   0        0        0     1424 2024-03-29 15:29:30.000000 one_interfaces-6.6.0/one_interfaces/model_location_pb2.py
--rw-rw-rw-   0        0        0     2487 2024-03-29 15:29:30.000000 one_interfaces-6.6.0/one_interfaces/model_parameter_pb2.py
--rw-rw-rw-   0        0        0     1233 2024-03-29 15:29:30.000000 one_interfaces-6.6.0/one_interfaces/multi_point2d_pb2.py
--rw-rw-rw-   0        0        0     1233 2024-03-29 15:29:30.000000 one_interfaces-6.6.0/one_interfaces/multi_point3d_pb2.py
--rw-rw-rw-   0        0        0     1472 2024-03-29 15:29:30.000000 one_interfaces-6.6.0/one_interfaces/note_pb2.py
--rw-rw-rw-   0        0        0     1695 2024-03-29 15:29:31.000000 one_interfaces-6.6.0/one_interfaces/notification_broadcast_pb2.py
--rw-rw-rw-   0        0        0     1448 2024-03-29 15:29:31.000000 one_interfaces-6.6.0/one_interfaces/notification_contact_pb2.py
--rw-rw-rw-   0        0        0     1859 2024-03-29 15:29:31.000000 one_interfaces-6.6.0/one_interfaces/notification_device_pb2.py
--rw-rw-rw-   0        0        0     2430 2024-03-29 15:29:31.000000 one_interfaces-6.6.0/one_interfaces/notification_direct_preference_pb2.py
--rw-rw-rw-   0        0        0     2254 2024-03-29 15:29:31.000000 one_interfaces-6.6.0/one_interfaces/notification_event_pb2.py
--rw-rw-rw-   0        0        0     2267 2024-03-29 15:29:31.000000 one_interfaces-6.6.0/one_interfaces/notification_in_app_notification_message_pb2.py
--rw-rw-rw-   0        0        0     1743 2024-03-29 15:29:31.000000 one_interfaces-6.6.0/one_interfaces/notification_preference_pb2.py
--rw-rw-rw-   0        0        0     2174 2024-03-29 15:29:31.000000 one_interfaces-6.6.0/one_interfaces/notification_template_pb2.py
--rw-rw-rw-   0        0        0     2201 2024-03-29 15:29:31.000000 one_interfaces-6.6.0/one_interfaces/notification_topic_pb2.py
--rw-rw-rw-   0        0        0     1828 2024-03-29 15:29:31.000000 one_interfaces-6.6.0/one_interfaces/notification_topic_variable_pb2.py
--rw-rw-rw-   0        0        0     2450 2024-03-29 15:29:31.000000 one_interfaces-6.6.0/one_interfaces/notification_user_preference_pb2.py
--rw-rw-rw-   0        0        0     2455 2024-03-29 15:29:31.000000 one_interfaces-6.6.0/one_interfaces/operation_export_pb2.py
--rw-rw-rw-   0        0        0     2111 2024-03-29 15:29:31.000000 one_interfaces-6.6.0/one_interfaces/outputcell_backup_pb2.py
--rw-rw-rw-   0        0        0     1552 2024-03-29 15:29:31.000000 one_interfaces-6.6.0/one_interfaces/pagination_pb2.py
--rw-rw-rw-   0        0        0     2177 2024-03-29 15:29:31.000000 one_interfaces-6.6.0/one_interfaces/parameter_agency_code_pb2.py
--rw-rw-rw-   0        0        0     1674 2024-03-29 15:29:31.000000 one_interfaces-6.6.0/one_interfaces/parameter_agency_code_type_pb2.py
--rw-rw-rw-   0        0        0     1819 2024-03-29 15:29:31.000000 one_interfaces-6.6.0/one_interfaces/parameter_definition_pb2.py
--rw-rw-rw-   0        0        0     2356 2024-03-29 15:29:31.000000 one_interfaces-6.6.0/one_interfaces/parameter_pb2.py
--rw-rw-rw-   0        0        0     2569 2024-03-29 15:29:31.000000 one_interfaces-6.6.0/one_interfaces/plant_status_pb2.py
--rw-rw-rw-   0        0        0     1158 2024-03-29 15:29:31.000000 one_interfaces-6.6.0/one_interfaces/point2d_pb2.py
--rw-rw-rw-   0        0        0     1186 2024-03-29 15:29:31.000000 one_interfaces-6.6.0/one_interfaces/point3d_pb2.py
--rw-rw-rw-   0        0        0     1637 2024-03-29 15:29:31.000000 one_interfaces-6.6.0/one_interfaces/post_filtering_column_definition_pb2.py
--rw-rw-rw-   0        0        0     1878 2024-03-29 15:29:31.000000 one_interfaces-6.6.0/one_interfaces/post_filtering_pb2.py
--rw-rw-rw-   0        0        0     1585 2024-03-29 15:29:32.000000 one_interfaces-6.6.0/one_interfaces/privileges_pb2.py
--rw-rw-rw-   0        0        0     2503 2024-03-29 15:29:32.000000 one_interfaces-6.6.0/one_interfaces/product_offering_pb2.py
--rw-rw-rw-   0        0        0     2064 2024-03-29 15:29:32.000000 one_interfaces-6.6.0/one_interfaces/quantity_type_pb2.py
--rw-rw-rw-   0        0        0     1448 2024-03-29 15:29:32.000000 one_interfaces-6.6.0/one_interfaces/record_auditinfo_pb2.py
--rw-rw-rw-   0        0        0     2076 2024-03-29 15:29:32.000000 one_interfaces-6.6.0/one_interfaces/report_definition_json_v2_pb2.py
--rw-rw-rw-   0        0        0     2780 2024-03-29 15:29:32.000000 one_interfaces-6.6.0/one_interfaces/report_definition_pb2.py
--rw-rw-rw-   0        0        0     2178 2024-03-29 15:29:32.000000 one_interfaces-6.6.0/one_interfaces/report_definition_runs_pb2.py
--rw-rw-rw-   0        0        0     1842 2024-03-29 15:29:32.000000 one_interfaces-6.6.0/one_interfaces/report_definition_tags_pb2.py
--rw-rw-rw-   0        0        0     1677 2024-03-29 15:29:32.000000 one_interfaces-6.6.0/one_interfaces/report_parameter_pb2.py
--rw-rw-rw-   0        0        0     2382 2024-03-29 15:29:32.000000 one_interfaces-6.6.0/one_interfaces/report_run_pb2.py
--rw-rw-rw-   0        0        0     1971 2024-03-29 15:29:32.000000 one_interfaces-6.6.0/one_interfaces/reportable_qualifier_definition_pb2.py
--rw-rw-rw-   0        0        0     1417 2024-03-29 15:29:32.000000 one_interfaces-6.6.0/one_interfaces/reportable_qualifier_pb2.py
--rw-rw-rw-   0        0        0     1252 2024-03-29 15:29:32.000000 one_interfaces-6.6.0/one_interfaces/rights_pb2.py
--rw-rw-rw-   0        0        0     2008 2024-03-29 15:29:32.000000 one_interfaces-6.6.0/one_interfaces/role_pb2.py
--rw-rw-rw-   0        0        0     1972 2024-03-29 15:29:32.000000 one_interfaces-6.6.0/one_interfaces/row_index_pb2.py
--rw-rw-rw-   0        0        0     1346 2024-03-29 15:29:32.000000 one_interfaces-6.6.0/one_interfaces/row_merge_result_pb2.py
--rw-rw-rw-   0        0        0     1692 2024-03-29 15:29:32.000000 one_interfaces-6.6.0/one_interfaces/row_pb2.py
--rw-rw-rw-   0        0        0     1403 2024-03-29 15:29:32.000000 one_interfaces-6.6.0/one_interfaces/schedule_occurrence_pb2.py
--rw-rw-rw-   0        0        0     2186 2024-03-29 15:29:32.000000 one_interfaces-6.6.0/one_interfaces/schedule_pb2.py
--rw-rw-rw-   0        0        0     1472 2024-03-29 15:29:32.000000 one_interfaces-6.6.0/one_interfaces/schedule_recurrence_pattern_pb2.py
--rw-rw-rw-   0        0        0     1887 2024-03-29 15:29:32.000000 one_interfaces-6.6.0/one_interfaces/schedule_type_pb2.py
--rw-rw-rw-   0        0        0     2533 2024-03-29 15:29:32.000000 one_interfaces-6.6.0/one_interfaces/scope_pb2.py
--rw-rw-rw-   0        0        0     1931 2024-03-29 15:29:32.000000 one_interfaces-6.6.0/one_interfaces/search_option_pb2.py
--rw-rw-rw-   0        0        0     2186 2024-03-29 15:29:32.000000 one_interfaces-6.6.0/one_interfaces/series_pb2.py
--rw-rw-rw-   0        0        0     2279 2024-03-29 15:29:33.000000 one_interfaces-6.6.0/one_interfaces/service_tech_tenant_request_pb2.py
--rw-rw-rw-   0        0        0     1649 2024-03-29 15:29:33.000000 one_interfaces-6.6.0/one_interfaces/signalr_one_hub_connection_info_pb2.py
--rw-rw-rw-   0        0        0     1261 2024-03-29 15:29:33.000000 one_interfaces-6.6.0/one_interfaces/signalr_one_hub_dataset_event_pb2.py
--rw-rw-rw-   0        0        0     1567 2024-03-29 15:29:33.000000 one_interfaces-6.6.0/one_interfaces/signalr_one_hub_event_payload_pb2.py
--rw-rw-rw-   0        0        0     1598 2024-03-29 15:29:33.000000 one_interfaces-6.6.0/one_interfaces/signalr_one_hub_event_pb2.py
--rw-rw-rw-   0        0        0     1624 2024-03-29 15:29:33.000000 one_interfaces-6.6.0/one_interfaces/signalr_one_hub_message_pb2.py
--rw-rw-rw-   0        0        0     1197 2024-03-29 15:29:33.000000 one_interfaces-6.6.0/one_interfaces/spreadsheet_binding_pb2.py
--rw-rw-rw-   0        0        0     1699 2024-03-29 15:29:33.000000 one_interfaces-6.6.0/one_interfaces/spreadsheet_computation_pb2.py
--rw-rw-rw-   0        0        0     1753 2024-03-29 15:29:33.000000 one_interfaces-6.6.0/one_interfaces/spreadsheet_definition_pb2.py
--rw-rw-rw-   0        0        0     1500 2024-03-29 15:29:33.000000 one_interfaces-6.6.0/one_interfaces/spreadsheet_pb2.py
--rw-rw-rw-   0        0        0     2465 2024-03-29 15:29:33.000000 one_interfaces-6.6.0/one_interfaces/tenant_pb2.py
--rw-rw-rw-   0        0        0     1680 2024-03-29 15:29:33.000000 one_interfaces-6.6.0/one_interfaces/tenant_product_offering_pb2.py
--rw-rw-rw-   0        0        0     2113 2024-03-29 15:29:33.000000 one_interfaces-6.6.0/one_interfaces/test_analyte_group_pb2.py
--rw-rw-rw-   0        0        0     1415 2024-03-29 15:29:33.000000 one_interfaces-6.6.0/one_interfaces/time_context_pb2.py
--rw-rw-rw-   0        0        0     2106 2024-03-29 15:29:33.000000 one_interfaces-6.6.0/one_interfaces/timeseriesdata_pb2.py
--rw-rw-rw-   0        0        0     1372 2024-03-29 15:29:33.000000 one_interfaces-6.6.0/one_interfaces/timewindow_pb2.py
--rw-rw-rw-   0        0        0     1499 2024-03-29 15:29:33.000000 one_interfaces-6.6.0/one_interfaces/timezones_pb2.py
--rw-rw-rw-   0        0        0     1835 2024-03-29 15:29:33.000000 one_interfaces-6.6.0/one_interfaces/unit_agency_code_pb2.py
--rw-rw-rw-   0        0        0     1627 2024-03-29 15:29:33.000000 one_interfaces-6.6.0/one_interfaces/unit_agency_code_type_pb2.py
--rw-rw-rw-   0        0        0     1701 2024-03-29 15:29:33.000000 one_interfaces-6.6.0/one_interfaces/unit_pb2.py
--rw-rw-rw-   0        0        0     1308 2024-03-29 15:29:33.000000 one_interfaces-6.6.0/one_interfaces/user_password_management_pb2.py
--rw-rw-rw-   0        0        0     4289 2024-03-29 15:29:33.000000 one_interfaces-6.6.0/one_interfaces/user_pb2.py
--rw-rw-rw-   0        0        0     1812 2024-03-29 15:29:33.000000 one_interfaces-6.6.0/one_interfaces/user_preference_pb2.py
--rw-rw-rw-   0        0        0     1969 2024-03-29 15:29:33.000000 one_interfaces-6.6.0/one_interfaces/user_profile_pb2.py
--rw-rw-rw-   0        0        0     1784 2024-03-29 15:29:34.000000 one_interfaces-6.6.0/one_interfaces/valid_value_pb2.py
--rw-rw-rw-   0        0        0     1966 2024-03-29 15:29:34.000000 one_interfaces-6.6.0/one_interfaces/variable_pb2.py
--rw-rw-rw-   0        0        0     1799 2024-03-29 15:29:34.000000 one_interfaces-6.6.0/one_interfaces/worksheet_definition_pb2.py
--rw-rw-rw-   0        0        0     1511 2024-03-29 15:29:34.000000 one_interfaces-6.6.0/one_interfaces/worksheet_pb2.py
--rw-rw-rw-   0        0        0     1789 2024-03-29 15:29:34.000000 one_interfaces-6.6.0/one_interfaces/worksheet_view_pb2.py
-drwxrwxrwx   0        0        0        0 2024-03-29 15:40:42.435099 one_interfaces-6.6.0/one_interfaces.egg-info/
--rw-rw-rw-   0        0        0     1217 2024-03-29 15:40:41.000000 one_interfaces-6.6.0/one_interfaces.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7463 2024-03-29 15:40:41.000000 one_interfaces-6.6.0/one_interfaces.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-29 15:40:41.000000 one_interfaces-6.6.0/one_interfaces.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-03-29 15:40:41.000000 one_interfaces-6.6.0/one_interfaces.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        4 2022-07-05 14:29:22.000000 one_interfaces-6.6.0/requirements.txt
--rw-rw-rw-   0        0        0      159 2024-03-29 15:40:42.439102 one_interfaces-6.6.0/setup.cfg
--rw-rw-rw-   0        0        0     1714 2022-11-11 17:30:03.000000 one_interfaces-6.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 13:42:35.730317 one_interfaces-6.7.0/
+-rw-rw-rw-   0        0        0      580 2022-07-05 14:29:22.000000 one_interfaces-6.7.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       62 2022-07-05 14:29:22.000000 one_interfaces-6.7.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1217 2024-04-03 13:42:35.730317 one_interfaces-6.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0      394 2022-11-11 17:33:49.000000 one_interfaces-6.7.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-03 13:42:35.716018 one_interfaces-6.7.0/one_interfaces/
+-rw-rw-rw-   0        0        0       23 2024-04-02 22:03:12.000000 one_interfaces-6.7.0/one_interfaces/__init__.py
+-rw-rw-rw-   0        0        0     1670 2024-04-03 13:42:08.000000 one_interfaces-6.7.0/one_interfaces/account_status_pb2.py
+-rw-rw-rw-   0        0        0     2440 2024-04-03 13:42:08.000000 one_interfaces-6.7.0/one_interfaces/activity_pb2.py
+-rw-rw-rw-   0        0        0     1899 2024-04-03 13:42:08.000000 one_interfaces-6.7.0/one_interfaces/activity_type_pb2.py
+-rw-rw-rw-   0        0        0     2231 2024-04-03 13:42:08.000000 one_interfaces-6.7.0/one_interfaces/address_pb2.py
+-rw-rw-rw-   0        0        0     1681 2024-04-03 13:42:08.000000 one_interfaces-6.7.0/one_interfaces/agency_pb2.py
+-rw-rw-rw-   0        0        0     1874 2024-04-03 13:42:08.000000 one_interfaces-6.7.0/one_interfaces/analyte_pb2.py
+-rw-rw-rw-   0        0        0     2811 2024-04-03 13:42:08.000000 one_interfaces-6.7.0/one_interfaces/analyte_result_pb2.py
+-rw-rw-rw-   0        0        0     1769 2024-04-03 13:42:08.000000 one_interfaces-6.7.0/one_interfaces/analyte_results_import_profile_pb2.py
+-rw-rw-rw-   0        0        0     1758 2024-04-03 13:42:08.000000 one_interfaces-6.7.0/one_interfaces/analyte_results_import_telemetry_pb2.py
+-rw-rw-rw-   0        0        0     1223 2024-04-03 13:42:08.000000 one_interfaces-6.7.0/one_interfaces/apierror_pb2.py
+-rw-rw-rw-   0        0        0     1393 2024-04-03 13:42:08.000000 one_interfaces-6.7.0/one_interfaces/apiresponse_pb2.py
+-rw-rw-rw-   0        0        0     1941 2024-04-03 13:42:08.000000 one_interfaces-6.7.0/one_interfaces/auditevent_pb2.py
+-rw-rw-rw-   0        0        0     1474 2024-04-03 13:42:08.000000 one_interfaces-6.7.0/one_interfaces/cell_monitor_backup_pb2.py
+-rw-rw-rw-   0        0        0     1519 2024-04-03 13:42:08.000000 one_interfaces-6.7.0/one_interfaces/cell_pb2.py
+-rw-rw-rw-   0        0        0     1541 2024-04-03 13:42:08.000000 one_interfaces-6.7.0/one_interfaces/celldata_binding_pb2.py
+-rw-rw-rw-   0        0        0     1988 2024-04-03 13:42:08.000000 one_interfaces-6.7.0/one_interfaces/celldata_pb2.py
+-rw-rw-rw-   0        0        0     1534 2024-04-03 13:42:08.000000 one_interfaces-6.7.0/one_interfaces/cells_pb2.py
+-rw-rw-rw-   0        0        0     1871 2024-04-03 13:42:08.000000 one_interfaces-6.7.0/one_interfaces/cellvalue_backup_pb2.py
+-rw-rw-rw-   0        0        0     4778 2024-04-03 13:42:08.000000 one_interfaces-6.7.0/one_interfaces/client_pb2.py
+-rw-rw-rw-   0        0        0     2054 2024-04-03 13:42:09.000000 one_interfaces-6.7.0/one_interfaces/coagmeasurement_pb2.py
+-rw-rw-rw-   0        0        0     2429 2024-04-03 13:42:09.000000 one_interfaces-6.7.0/one_interfaces/column_pb2.py
+-rw-rw-rw-   0        0        0     2097 2024-04-03 13:42:09.000000 one_interfaces-6.7.0/one_interfaces/computation_binding_pb2.py
+-rw-rw-rw-   0        0        0     2564 2024-04-03 13:42:09.000000 one_interfaces-6.7.0/one_interfaces/computation_pb2.py
+-rw-rw-rw-   0        0        0     1893 2024-04-03 13:42:09.000000 one_interfaces-6.7.0/one_interfaces/computation_variable_binding_pb2.py
+-rw-rw-rw-   0        0        0     2027 2024-04-03 13:42:09.000000 one_interfaces-6.7.0/one_interfaces/configuration_note_pb2.py
+-rw-rw-rw-   0        0        0     2970 2024-04-03 13:42:09.000000 one_interfaces-6.7.0/one_interfaces/configuration_pb2.py
+-rw-rw-rw-   0        0        0     1499 2024-04-03 13:42:09.000000 one_interfaces-6.7.0/one_interfaces/configuration_tag_pb2.py
+-rw-rw-rw-   0        0        0    13410 2024-04-03 13:42:09.000000 one_interfaces-6.7.0/one_interfaces/content_pb2.py
+-rw-rw-rw-   0        0        0     1951 2024-04-03 13:42:09.000000 one_interfaces-6.7.0/one_interfaces/csv_configuration_file_pb2.py
+-rw-rw-rw-   0        0        0     1743 2024-04-03 13:42:09.000000 one_interfaces-6.7.0/one_interfaces/data_source_binding_pb2.py
+-rw-rw-rw-   0        0        0     2052 2024-04-03 13:42:09.000000 one_interfaces-6.7.0/one_interfaces/data_source_configuration_pb2.py
+-rw-rw-rw-   0        0        0     1536 2024-04-03 13:42:09.000000 one_interfaces-6.7.0/one_interfaces/digital_twin_column_telemetry_propertybag_pb2.py
+-rw-rw-rw-   0        0        0     2041 2024-04-03 13:42:09.000000 one_interfaces-6.7.0/one_interfaces/digital_twin_enterprise_data_telemetry_pb2.py
+-rw-rw-rw-   0        0        0     1523 2024-04-03 13:42:09.000000 one_interfaces-6.7.0/one_interfaces/digital_twin_instrument_telemetry_propertybag_pb2.py
+-rw-rw-rw-   0        0        0     3269 2024-04-03 13:42:09.000000 one_interfaces-6.7.0/one_interfaces/digital_twin_pb2.py
+-rw-rw-rw-   0        0        0     2247 2024-04-03 13:42:09.000000 one_interfaces-6.7.0/one_interfaces/digital_twin_subtype_pb2.py
+-rw-rw-rw-   0        0        0     3800 2024-04-03 13:42:09.000000 one_interfaces-6.7.0/one_interfaces/digital_twin_subtype_propertybag_pb2.py
+-rw-rw-rw-   0        0        0     2063 2024-04-03 13:42:09.000000 one_interfaces-6.7.0/one_interfaces/digital_twin_type_pb2.py
+-rw-rw-rw-   0        0        0     2020 2024-04-03 13:42:10.000000 one_interfaces-6.7.0/one_interfaces/digital_twin_user_right_pb2.py
+-rw-rw-rw-   0        0        0     1342 2024-04-03 13:42:10.000000 one_interfaces-6.7.0/one_interfaces/display_options_pb2.py
+-rw-rw-rw-   0        0        0     1820 2024-04-03 13:42:10.000000 one_interfaces-6.7.0/one_interfaces/enterprise_data_source_definition_pb2.py
+-rw-rw-rw-   0        0        0     1669 2024-04-03 13:42:10.000000 one_interfaces-6.7.0/one_interfaces/enterprise_data_table_definition_pb2.py
+-rw-rw-rw-   0        0        0     1376 2024-04-03 13:42:10.000000 one_interfaces-6.7.0/one_interfaces/enterprise_data_table_field_pb2.py
+-rw-rw-rw-   0        0        0     1605 2024-04-03 13:42:10.000000 one_interfaces-6.7.0/one_interfaces/enterprise_data_table_query_parameter_pb2.py
+-rw-rw-rw-   0        0        0     1508 2024-04-03 13:42:10.000000 one_interfaces-6.7.0/one_interfaces/enterprise_data_table_query_pb2.py
+-rw-rw-rw-   0        0        0     2309 2024-04-03 13:42:10.000000 one_interfaces-6.7.0/one_interfaces/enterprise_dataset_definition_pb2.py
+-rw-rw-rw-   0        0        0     1303 2024-04-03 13:42:10.000000 one_interfaces-6.7.0/one_interfaces/enum_aggregate_pb2.py
+-rw-rw-rw-   0        0        0     1408 2024-04-03 13:42:10.000000 one_interfaces-6.7.0/one_interfaces/enum_auditevent_pb2.py
+-rw-rw-rw-   0        0        0     1385 2024-04-03 13:42:10.000000 one_interfaces-6.7.0/one_interfaces/enum_azure_notification_hubtype_pb2.py
+-rw-rw-rw-   0        0        0     1642 2024-04-03 13:42:10.000000 one_interfaces-6.7.0/one_interfaces/enum_cell_range_action_pb2.py
+-rw-rw-rw-   0        0        0     1730 2024-04-03 13:42:10.000000 one_interfaces-6.7.0/one_interfaces/enum_datasource_pb2.py
+-rw-rw-rw-   0        0        0     1392 2024-04-03 13:42:10.000000 one_interfaces-6.7.0/one_interfaces/enum_day_pb2.py
+-rw-rw-rw-   0        0        0     1515 2024-04-03 13:42:10.000000 one_interfaces-6.7.0/one_interfaces/enum_digital_twin_dataset_output_format_pb2.py
+-rw-rw-rw-   0        0        0     1381 2024-04-03 13:42:10.000000 one_interfaces-6.7.0/one_interfaces/enum_digital_twin_restriction_pb2.py
+-rw-rw-rw-   0        0        0     1422 2024-04-03 13:42:10.000000 one_interfaces-6.7.0/one_interfaces/enum_digital_twin_user_right_pb2.py
+-rw-rw-rw-   0        0        0     1339 2024-04-03 13:42:10.000000 one_interfaces-6.7.0/one_interfaces/enum_domain_source_pb2.py
+-rw-rw-rw-   0        0        0     1373 2024-04-03 13:42:10.000000 one_interfaces-6.7.0/one_interfaces/enum_entity_pb2.py
+-rw-rw-rw-   0        0        0     1433 2024-04-03 13:42:10.000000 one_interfaces-6.7.0/one_interfaces/enum_identity_provider_pb2.py
+-rw-rw-rw-   0        0        0     1552 2024-04-03 13:42:10.000000 one_interfaces-6.7.0/one_interfaces/enum_import_status_pb2.py
+-rw-rw-rw-   0        0        0     1416 2024-04-03 13:42:10.000000 one_interfaces-6.7.0/one_interfaces/enum_limit_operation_pb2.py
+-rw-rw-rw-   0        0        0     1394 2024-04-03 13:42:10.000000 one_interfaces-6.7.0/one_interfaces/enum_limit_pb2.py
+-rw-rw-rw-   0        0        0     1545 2024-04-03 13:42:10.000000 one_interfaces-6.7.0/one_interfaces/enum_month_pb2.py
+-rw-rw-rw-   0        0        0     1606 2024-04-03 13:42:10.000000 one_interfaces-6.7.0/one_interfaces/enum_notification_category_pb2.py
+-rw-rw-rw-   0        0        0     1557 2024-04-03 13:42:10.000000 one_interfaces-6.7.0/one_interfaces/enum_notification_delivery_method_pb2.py
+-rw-rw-rw-   0        0        0     1427 2024-04-03 13:42:11.000000 one_interfaces-6.7.0/one_interfaces/enum_notification_message_type_pb2.py
+-rw-rw-rw-   0        0        0     1346 2024-04-03 13:42:11.000000 one_interfaces-6.7.0/one_interfaces/enum_notification_platform_pb2.py
+-rw-rw-rw-   0        0        0     1452 2024-04-03 13:42:11.000000 one_interfaces-6.7.0/one_interfaces/enum_one_log_level_pb2.py
+-rw-rw-rw-   0        0        0     1374 2024-04-03 13:42:11.000000 one_interfaces-6.7.0/one_interfaces/enum_output_placement_pb2.py
+-rw-rw-rw-   0        0        0     1269 2024-04-03 13:42:11.000000 one_interfaces-6.7.0/one_interfaces/enum_rendering_engine_pb2.py
+-rw-rw-rw-   0        0        0     1681 2024-04-03 13:42:11.000000 one_interfaces-6.7.0/one_interfaces/enum_reportable_qualifier_definition_pb2.py
+-rw-rw-rw-   0        0        0     1663 2024-04-03 13:42:11.000000 one_interfaces-6.7.0/one_interfaces/enum_reportable_qualifier_pb2.py
+-rw-rw-rw-   0        0        0     3080 2024-04-03 13:42:11.000000 one_interfaces-6.7.0/one_interfaces/enum_sampling_statistic_pb2.py
+-rw-rw-rw-   0        0        0     1483 2024-04-03 13:42:11.000000 one_interfaces-6.7.0/one_interfaces/enum_time_context_pb2.py
+-rw-rw-rw-   0        0        0     1388 2024-04-03 13:42:11.000000 one_interfaces-6.7.0/one_interfaces/enum_time_unit_pb2.py
+-rw-rw-rw-   0        0        0    27482 2024-04-03 13:42:11.000000 one_interfaces-6.7.0/one_interfaces/enum_timezone_pb2.py
+-rw-rw-rw-   0        0        0     1415 2024-04-03 13:42:11.000000 one_interfaces-6.7.0/one_interfaces/enum_valid_value_restriction_pb2.py
+-rw-rw-rw-   0        0        0     1376 2024-04-03 13:42:11.000000 one_interfaces-6.7.0/one_interfaces/enum_variable_type_pb2.py
+-rw-rw-rw-   0        0        0     2357 2024-04-03 13:42:11.000000 one_interfaces-6.7.0/one_interfaces/enum_wims_week_definition_pb2.py
+-rw-rw-rw-   0        0        0     1341 2024-04-03 13:42:11.000000 one_interfaces-6.7.0/one_interfaces/enum_worksheet_pb2.py
+-rw-rw-rw-   0        0        0     1768 2024-04-03 13:42:11.000000 one_interfaces-6.7.0/one_interfaces/execution_details_pb2.py
+-rw-rw-rw-   0        0        0     2010 2024-04-03 13:42:11.000000 one_interfaces-6.7.0/one_interfaces/execution_parameter_pb2.py
+-rw-rw-rw-   0        0        0     1211 2024-04-03 13:42:11.000000 one_interfaces-6.7.0/one_interfaces/expression_line_pb2.py
+-rw-rw-rw-   0        0        0     2205 2024-04-03 13:42:11.000000 one_interfaces-6.7.0/one_interfaces/feature_pb2.py
+-rw-rw-rw-   0        0        0     1589 2024-04-03 13:42:11.000000 one_interfaces-6.7.0/one_interfaces/feature_state_type_pb2.py
+-rw-rw-rw-   0        0        0     1793 2024-04-03 13:42:11.000000 one_interfaces-6.7.0/one_interfaces/file_configuration_pb2.py
+-rw-rw-rw-   0        0        0     1563 2024-04-03 13:42:11.000000 one_interfaces-6.7.0/one_interfaces/gauge_data_point_pb2.py
+-rw-rw-rw-   0        0        0     1560 2024-04-03 13:42:11.000000 one_interfaces-6.7.0/one_interfaces/gis_pb2.py
+-rw-rw-rw-   0        0        0     1231 2024-04-03 13:42:11.000000 one_interfaces-6.7.0/one_interfaces/historian_binding_pb2.py
+-rw-rw-rw-   0        0        0     1981 2024-04-03 13:42:11.000000 one_interfaces-6.7.0/one_interfaces/historian_data_pb2.py
+-rw-rw-rw-   0        0        0     1536 2024-04-03 13:42:12.000000 one_interfaces-6.7.0/one_interfaces/i18nkey_text_reference_pb2.py
+-rw-rw-rw-   0        0        0     1855 2024-04-03 13:42:12.000000 one_interfaces-6.7.0/one_interfaces/ingest_client_pb2.py
+-rw-rw-rw-   0        0        0     1698 2024-04-03 13:42:12.000000 one_interfaces-6.7.0/one_interfaces/jsonTicksDateTime_pb2.py
+-rw-rw-rw-   0        0        0     1325 2024-04-03 13:42:12.000000 one_interfaces-6.7.0/one_interfaces/key_value_pb2.py
+-rw-rw-rw-   0        0        0     1668 2024-04-03 13:42:12.000000 one_interfaces-6.7.0/one_interfaces/limit_configuration_pb2.py
+-rw-rw-rw-   0        0        0     2385 2024-04-03 13:42:12.000000 one_interfaces-6.7.0/one_interfaces/limit_pb2.py
+-rw-rw-rw-   0        0        0     1948 2024-04-03 13:42:12.000000 one_interfaces-6.7.0/one_interfaces/measurement_pb2.py
+-rw-rw-rw-   0        0        0     1768 2024-04-03 13:42:12.000000 one_interfaces-6.7.0/one_interfaces/model_execution_pb2.py
+-rw-rw-rw-   0        0        0     1424 2024-04-03 13:42:12.000000 one_interfaces-6.7.0/one_interfaces/model_location_pb2.py
+-rw-rw-rw-   0        0        0     2391 2024-04-03 13:42:12.000000 one_interfaces-6.7.0/one_interfaces/model_template_pb2.py
+-rw-rw-rw-   0        0        0     1233 2024-04-03 13:42:12.000000 one_interfaces-6.7.0/one_interfaces/multi_point2d_pb2.py
+-rw-rw-rw-   0        0        0     1233 2024-04-03 13:42:12.000000 one_interfaces-6.7.0/one_interfaces/multi_point3d_pb2.py
+-rw-rw-rw-   0        0        0     1472 2024-04-03 13:42:12.000000 one_interfaces-6.7.0/one_interfaces/note_pb2.py
+-rw-rw-rw-   0        0        0     1695 2024-04-03 13:42:12.000000 one_interfaces-6.7.0/one_interfaces/notification_broadcast_pb2.py
+-rw-rw-rw-   0        0        0     1448 2024-04-03 13:42:12.000000 one_interfaces-6.7.0/one_interfaces/notification_contact_pb2.py
+-rw-rw-rw-   0        0        0     1859 2024-04-03 13:42:12.000000 one_interfaces-6.7.0/one_interfaces/notification_device_pb2.py
+-rw-rw-rw-   0        0        0     2430 2024-04-03 13:42:12.000000 one_interfaces-6.7.0/one_interfaces/notification_direct_preference_pb2.py
+-rw-rw-rw-   0        0        0     2254 2024-04-03 13:42:12.000000 one_interfaces-6.7.0/one_interfaces/notification_event_pb2.py
+-rw-rw-rw-   0        0        0     2267 2024-04-03 13:42:12.000000 one_interfaces-6.7.0/one_interfaces/notification_in_app_notification_message_pb2.py
+-rw-rw-rw-   0        0        0     1743 2024-04-03 13:42:12.000000 one_interfaces-6.7.0/one_interfaces/notification_preference_pb2.py
+-rw-rw-rw-   0        0        0     2174 2024-04-03 13:42:12.000000 one_interfaces-6.7.0/one_interfaces/notification_template_pb2.py
+-rw-rw-rw-   0        0        0     2201 2024-04-03 13:42:12.000000 one_interfaces-6.7.0/one_interfaces/notification_topic_pb2.py
+-rw-rw-rw-   0        0        0     1828 2024-04-03 13:42:13.000000 one_interfaces-6.7.0/one_interfaces/notification_topic_variable_pb2.py
+-rw-rw-rw-   0        0        0     2450 2024-04-03 13:42:13.000000 one_interfaces-6.7.0/one_interfaces/notification_user_preference_pb2.py
+-rw-rw-rw-   0        0        0     2455 2024-04-03 13:42:13.000000 one_interfaces-6.7.0/one_interfaces/operation_export_pb2.py
+-rw-rw-rw-   0        0        0     2111 2024-04-03 13:42:13.000000 one_interfaces-6.7.0/one_interfaces/outputcell_backup_pb2.py
+-rw-rw-rw-   0        0        0     1552 2024-04-03 13:42:13.000000 one_interfaces-6.7.0/one_interfaces/pagination_pb2.py
+-rw-rw-rw-   0        0        0     2177 2024-04-03 13:42:13.000000 one_interfaces-6.7.0/one_interfaces/parameter_agency_code_pb2.py
+-rw-rw-rw-   0        0        0     1674 2024-04-03 13:42:13.000000 one_interfaces-6.7.0/one_interfaces/parameter_agency_code_type_pb2.py
+-rw-rw-rw-   0        0        0     1819 2024-04-03 13:42:13.000000 one_interfaces-6.7.0/one_interfaces/parameter_definition_pb2.py
+-rw-rw-rw-   0        0        0     2356 2024-04-03 13:42:13.000000 one_interfaces-6.7.0/one_interfaces/parameter_pb2.py
+-rw-rw-rw-   0        0        0     2569 2024-04-03 13:42:13.000000 one_interfaces-6.7.0/one_interfaces/plant_status_pb2.py
+-rw-rw-rw-   0        0        0     1158 2024-04-03 13:42:13.000000 one_interfaces-6.7.0/one_interfaces/point2d_pb2.py
+-rw-rw-rw-   0        0        0     1186 2024-04-03 13:42:13.000000 one_interfaces-6.7.0/one_interfaces/point3d_pb2.py
+-rw-rw-rw-   0        0        0     1637 2024-04-03 13:42:13.000000 one_interfaces-6.7.0/one_interfaces/post_filtering_column_definition_pb2.py
+-rw-rw-rw-   0        0        0     1878 2024-04-03 13:42:13.000000 one_interfaces-6.7.0/one_interfaces/post_filtering_pb2.py
+-rw-rw-rw-   0        0        0     1585 2024-04-03 13:42:13.000000 one_interfaces-6.7.0/one_interfaces/privileges_pb2.py
+-rw-rw-rw-   0        0        0     2503 2024-04-03 13:42:13.000000 one_interfaces-6.7.0/one_interfaces/product_offering_pb2.py
+-rw-rw-rw-   0        0        0     2064 2024-04-03 13:42:13.000000 one_interfaces-6.7.0/one_interfaces/quantity_type_pb2.py
+-rw-rw-rw-   0        0        0     1448 2024-04-03 13:42:13.000000 one_interfaces-6.7.0/one_interfaces/record_auditinfo_pb2.py
+-rw-rw-rw-   0        0        0     2076 2024-04-03 13:42:14.000000 one_interfaces-6.7.0/one_interfaces/report_definition_json_v2_pb2.py
+-rw-rw-rw-   0        0        0     2780 2024-04-03 13:42:13.000000 one_interfaces-6.7.0/one_interfaces/report_definition_pb2.py
+-rw-rw-rw-   0        0        0     2178 2024-04-03 13:42:14.000000 one_interfaces-6.7.0/one_interfaces/report_definition_runs_pb2.py
+-rw-rw-rw-   0        0        0     1842 2024-04-03 13:42:14.000000 one_interfaces-6.7.0/one_interfaces/report_definition_tags_pb2.py
+-rw-rw-rw-   0        0        0     1677 2024-04-03 13:42:14.000000 one_interfaces-6.7.0/one_interfaces/report_parameter_pb2.py
+-rw-rw-rw-   0        0        0     2382 2024-04-03 13:42:14.000000 one_interfaces-6.7.0/one_interfaces/report_run_pb2.py
+-rw-rw-rw-   0        0        0     1971 2024-04-03 13:42:13.000000 one_interfaces-6.7.0/one_interfaces/reportable_qualifier_definition_pb2.py
+-rw-rw-rw-   0        0        0     1417 2024-04-03 13:42:13.000000 one_interfaces-6.7.0/one_interfaces/reportable_qualifier_pb2.py
+-rw-rw-rw-   0        0        0     1252 2024-04-03 13:42:14.000000 one_interfaces-6.7.0/one_interfaces/rights_pb2.py
+-rw-rw-rw-   0        0        0     2008 2024-04-03 13:42:14.000000 one_interfaces-6.7.0/one_interfaces/role_pb2.py
+-rw-rw-rw-   0        0        0     1972 2024-04-03 13:42:14.000000 one_interfaces-6.7.0/one_interfaces/row_index_pb2.py
+-rw-rw-rw-   0        0        0     1346 2024-04-03 13:42:14.000000 one_interfaces-6.7.0/one_interfaces/row_merge_result_pb2.py
+-rw-rw-rw-   0        0        0     1692 2024-04-03 13:42:14.000000 one_interfaces-6.7.0/one_interfaces/row_pb2.py
+-rw-rw-rw-   0        0        0     1403 2024-04-03 13:42:14.000000 one_interfaces-6.7.0/one_interfaces/schedule_occurrence_pb2.py
+-rw-rw-rw-   0        0        0     2186 2024-04-03 13:42:14.000000 one_interfaces-6.7.0/one_interfaces/schedule_pb2.py
+-rw-rw-rw-   0        0        0     1472 2024-04-03 13:42:14.000000 one_interfaces-6.7.0/one_interfaces/schedule_recurrence_pattern_pb2.py
+-rw-rw-rw-   0        0        0     1887 2024-04-03 13:42:14.000000 one_interfaces-6.7.0/one_interfaces/schedule_type_pb2.py
+-rw-rw-rw-   0        0        0     2533 2024-04-03 13:42:14.000000 one_interfaces-6.7.0/one_interfaces/scope_pb2.py
+-rw-rw-rw-   0        0        0     1931 2024-04-03 13:42:14.000000 one_interfaces-6.7.0/one_interfaces/search_option_pb2.py
+-rw-rw-rw-   0        0        0     2186 2024-04-03 13:42:14.000000 one_interfaces-6.7.0/one_interfaces/series_pb2.py
+-rw-rw-rw-   0        0        0     2279 2024-04-03 13:42:14.000000 one_interfaces-6.7.0/one_interfaces/service_tech_tenant_request_pb2.py
+-rw-rw-rw-   0        0        0     1649 2024-04-03 13:42:14.000000 one_interfaces-6.7.0/one_interfaces/signalr_one_hub_connection_info_pb2.py
+-rw-rw-rw-   0        0        0     1261 2024-04-03 13:42:14.000000 one_interfaces-6.7.0/one_interfaces/signalr_one_hub_dataset_event_pb2.py
+-rw-rw-rw-   0        0        0     1567 2024-04-03 13:42:14.000000 one_interfaces-6.7.0/one_interfaces/signalr_one_hub_event_payload_pb2.py
+-rw-rw-rw-   0        0        0     1598 2024-04-03 13:42:14.000000 one_interfaces-6.7.0/one_interfaces/signalr_one_hub_event_pb2.py
+-rw-rw-rw-   0        0        0     1624 2024-04-03 13:42:15.000000 one_interfaces-6.7.0/one_interfaces/signalr_one_hub_message_pb2.py
+-rw-rw-rw-   0        0        0     1197 2024-04-03 13:42:15.000000 one_interfaces-6.7.0/one_interfaces/spreadsheet_binding_pb2.py
+-rw-rw-rw-   0        0        0     1699 2024-04-03 13:42:15.000000 one_interfaces-6.7.0/one_interfaces/spreadsheet_computation_pb2.py
+-rw-rw-rw-   0        0        0     1753 2024-04-03 13:42:15.000000 one_interfaces-6.7.0/one_interfaces/spreadsheet_definition_pb2.py
+-rw-rw-rw-   0        0        0     1500 2024-04-03 13:42:15.000000 one_interfaces-6.7.0/one_interfaces/spreadsheet_pb2.py
+-rw-rw-rw-   0        0        0     1820 2024-04-03 13:42:15.000000 one_interfaces-6.7.0/one_interfaces/template_parameter_pb2.py
+-rw-rw-rw-   0        0        0     2465 2024-04-03 13:42:15.000000 one_interfaces-6.7.0/one_interfaces/tenant_pb2.py
+-rw-rw-rw-   0        0        0     1680 2024-04-03 13:42:15.000000 one_interfaces-6.7.0/one_interfaces/tenant_product_offering_pb2.py
+-rw-rw-rw-   0        0        0     2113 2024-04-03 13:42:15.000000 one_interfaces-6.7.0/one_interfaces/test_analyte_group_pb2.py
+-rw-rw-rw-   0        0        0     1415 2024-04-03 13:42:15.000000 one_interfaces-6.7.0/one_interfaces/time_context_pb2.py
+-rw-rw-rw-   0        0        0     2106 2024-04-03 13:42:15.000000 one_interfaces-6.7.0/one_interfaces/timeseriesdata_pb2.py
+-rw-rw-rw-   0        0        0     1372 2024-04-03 13:42:15.000000 one_interfaces-6.7.0/one_interfaces/timewindow_pb2.py
+-rw-rw-rw-   0        0        0     1499 2024-04-03 13:42:15.000000 one_interfaces-6.7.0/one_interfaces/timezones_pb2.py
+-rw-rw-rw-   0        0        0     1835 2024-04-03 13:42:15.000000 one_interfaces-6.7.0/one_interfaces/unit_agency_code_pb2.py
+-rw-rw-rw-   0        0        0     1627 2024-04-03 13:42:15.000000 one_interfaces-6.7.0/one_interfaces/unit_agency_code_type_pb2.py
+-rw-rw-rw-   0        0        0     1701 2024-04-03 13:42:15.000000 one_interfaces-6.7.0/one_interfaces/unit_pb2.py
+-rw-rw-rw-   0        0        0     1308 2024-04-03 13:42:15.000000 one_interfaces-6.7.0/one_interfaces/user_password_management_pb2.py
+-rw-rw-rw-   0        0        0     4289 2024-04-03 13:42:15.000000 one_interfaces-6.7.0/one_interfaces/user_pb2.py
+-rw-rw-rw-   0        0        0     1812 2024-04-03 13:42:15.000000 one_interfaces-6.7.0/one_interfaces/user_preference_pb2.py
+-rw-rw-rw-   0        0        0     1969 2024-04-03 13:42:15.000000 one_interfaces-6.7.0/one_interfaces/user_profile_pb2.py
+-rw-rw-rw-   0        0        0     1784 2024-04-03 13:42:15.000000 one_interfaces-6.7.0/one_interfaces/valid_value_pb2.py
+-rw-rw-rw-   0        0        0     1966 2024-04-03 13:42:16.000000 one_interfaces-6.7.0/one_interfaces/variable_pb2.py
+-rw-rw-rw-   0        0        0     1799 2024-04-03 13:42:16.000000 one_interfaces-6.7.0/one_interfaces/worksheet_definition_pb2.py
+-rw-rw-rw-   0        0        0     1511 2024-04-03 13:42:16.000000 one_interfaces-6.7.0/one_interfaces/worksheet_pb2.py
+-rw-rw-rw-   0        0        0     1789 2024-04-03 13:42:16.000000 one_interfaces-6.7.0/one_interfaces/worksheet_view_pb2.py
+drwxrwxrwx   0        0        0        0 2024-04-03 13:42:35.728315 one_interfaces-6.7.0/one_interfaces.egg-info/
+-rw-rw-rw-   0        0        0     1217 2024-04-03 13:42:34.000000 one_interfaces-6.7.0/one_interfaces.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7545 2024-04-03 13:42:34.000000 one_interfaces-6.7.0/one_interfaces.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 13:42:34.000000 one_interfaces-6.7.0/one_interfaces.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-03 13:42:34.000000 one_interfaces-6.7.0/one_interfaces.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        4 2022-07-05 14:29:22.000000 one_interfaces-6.7.0/requirements.txt
+-rw-rw-rw-   0        0        0      159 2024-04-03 13:42:35.732314 one_interfaces-6.7.0/setup.cfg
+-rw-rw-rw-   0        0        0     1714 2022-11-11 17:30:03.000000 one_interfaces-6.7.0/setup.py
```

### Comparing `one_interfaces-6.6.0/LICENSE.txt` & `one_interfaces-6.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/PKG-INFO` & `one_interfaces-6.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: one_interfaces
-Version: 6.6.0
+Version: 6.7.0
 Summary: Python bindings for ONE.
 Home-page: https://github.com/aquaticinformatics/one_interfaces
 Author: Aquatic Informatics
 Author-email: info@aquaticinformatics.com
 Maintainer: Aquatic Informatics
 License: BSD
 Description: One_Interfaces
```

### Comparing `one_interfaces-6.6.0/one_interfaces/account_status_pb2.py` & `one_interfaces-6.7.0/one_interfaces/account_status_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/activity_pb2.py` & `one_interfaces-6.7.0/one_interfaces/activity_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/activity_type_pb2.py` & `one_interfaces-6.7.0/one_interfaces/activity_type_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/address_pb2.py` & `one_interfaces-6.7.0/one_interfaces/address_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/agency_pb2.py` & `one_interfaces-6.7.0/one_interfaces/agency_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/analyte_pb2.py` & `one_interfaces-6.7.0/one_interfaces/analyte_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/analyte_result_pb2.py` & `one_interfaces-6.7.0/one_interfaces/analyte_result_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/analyte_results_import_profile_pb2.py` & `one_interfaces-6.7.0/one_interfaces/analyte_results_import_profile_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/analyte_results_import_telemetry_pb2.py` & `one_interfaces-6.7.0/one_interfaces/analyte_results_import_telemetry_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/apierror_pb2.py` & `one_interfaces-6.7.0/one_interfaces/apierror_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/apiresponse_pb2.py` & `one_interfaces-6.7.0/one_interfaces/apiresponse_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/auditevent_pb2.py` & `one_interfaces-6.7.0/one_interfaces/auditevent_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/cell_monitor_backup_pb2.py` & `one_interfaces-6.7.0/one_interfaces/cell_monitor_backup_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/cell_pb2.py` & `one_interfaces-6.7.0/one_interfaces/cell_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/celldata_binding_pb2.py` & `one_interfaces-6.7.0/one_interfaces/celldata_binding_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/celldata_pb2.py` & `one_interfaces-6.7.0/one_interfaces/celldata_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/cells_pb2.py` & `one_interfaces-6.7.0/one_interfaces/cells_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/cellvalue_backup_pb2.py` & `one_interfaces-6.7.0/one_interfaces/cellvalue_backup_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/client_pb2.py` & `one_interfaces-6.7.0/one_interfaces/client_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/coagmeasurement_pb2.py` & `one_interfaces-6.7.0/one_interfaces/coagmeasurement_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/column_pb2.py` & `one_interfaces-6.7.0/one_interfaces/column_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/computation_binding_pb2.py` & `one_interfaces-6.7.0/one_interfaces/computation_binding_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/computation_pb2.py` & `one_interfaces-6.7.0/one_interfaces/computation_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/computation_variable_binding_pb2.py` & `one_interfaces-6.7.0/one_interfaces/computation_variable_binding_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/configuration_note_pb2.py` & `one_interfaces-6.7.0/one_interfaces/configuration_note_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/configuration_pb2.py` & `one_interfaces-6.7.0/one_interfaces/configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/configuration_tag_pb2.py` & `one_interfaces-6.7.0/one_interfaces/configuration_tag_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/content_pb2.py` & `one_interfaces-6.7.0/one_interfaces/content_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,20 +84,21 @@
 import report_run_pb2 as report__run__pb2
 import ingest_client_pb2 as ingest__client__pb2
 import cellvalue_backup_pb2 as cellvalue__backup__pb2
 import outputcell_backup_pb2 as outputcell__backup__pb2
 import operation_export_pb2 as operation__export__pb2
 import analyte_result_pb2 as analyte__result__pb2
 import model_execution_pb2 as model__execution__pb2
+import model_template_pb2 as model__template__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\rcontent.proto\x1a\x0b\x63\x65lls.proto\x1a\x13\x63onfiguration.proto\x1a\x11\x63omputation.proto\x1a\x19limit_configuration.proto\x1a\x11measurement.proto\x1a\trow.proto\x1a\x0frow_index.proto\x1a\x1cspreadsheet_definition.proto\x1a\x1aworksheet_definition.proto\x1a\x1dspreadsheet_computation.proto\x1a\x1bnotification_template.proto\x1a\x1anotification_contact.proto\x1a\x19notification_device.proto\x1a\x1dnotification_preference.proto\x1a\"notification_user_preference.proto\x1a$notification_direct_preference.proto\x1a\x18notification_topic.proto\x1a\x0fparameter.proto\x1a\nunit.proto\x1a\x0ftimezones.proto\x1a\x0evariable.proto\x1a\raddress.proto\x1a\rfeature.proto\x1a\x16product_offering.proto\x1a\nrole.proto\x1a!service_tech_tenant_request.proto\x1a\x0ctenant.proto\x1a\x1dtenant_product_offering.proto\x1a\nuser.proto\x1a\x15user_preference.proto\x1a\x12user_profile.proto\x1a\x12\x64igital_twin.proto\x1a\x1d\x64igital_twin_user_right.proto\x1a\x14\x61\x63\x63ount_status.proto\x1a\x17\x64igital_twin_type.proto\x1a\x1a\x64igital_twin_subtype.proto\x1a\x12plant_status.proto\x1a.notification_in_app_notification_message.proto\x1a&digital_twin_subtype_propertybag.proto\x1a\x0c\x63lient.proto\x1a\x0bscope.proto\x1a\x16gauge_data_point.proto\x1a\x0cseries.proto\x1a/digital_twin_column_telemetry_propertybag.proto\x1a\x33\x64igital_twin_instrument_telemetry_propertybag.proto\x1a\x0e\x61\x63tivity.proto\x1a,digital_twin_enterprise_data_telemetry.proto\x1a\x16report_parameter.proto\x1a\x0c\x61gency.proto\x1a\x17report_definition.proto\x1a\x1bparameter_agency_code.proto\x1a parameter_agency_code_type.proto\x1a\x16unit_agency_code.proto\x1a\x1bunit_agency_code_type.proto\x1a\x1creport_definition_runs.proto\x1a\x1creport_definition_tags.proto\x1a\x0fkey_value.proto\x1a\x13quantity_type.proto\x1a\x15\x63oagmeasurement.proto\x1a\x14timeseriesdata.proto\x1a\x13schedule_type.proto\x1a\x0eschedule.proto\x1a\x14historian_data.proto\x1a\x19schedule_occurrence.proto\x1a\x18\x63onfiguration_note.proto\x1a\x17\x63onfiguration_tag.proto\x1a\ranalyte.proto\x1a\x18test_analyte_group.proto\x1a#enterprise_dataset_definition.proto\x1a\x10report_run.proto\x1a\x13ingest_client.proto\x1a\x16\x63\x65llvalue_backup.proto\x1a\x17outputcell_backup.proto\x1a\x16operation_export.proto\x1a\x14\x61nalyte_result.proto\x1a\x15model_execution.proto\"\xbb\x1b\n\x07\x43ontent\x12!\n\nactivities\x18@ \x01(\x0b\x32\x0b.ActivitiesH\x00\x12%\n\x0c\x63omputations\x18\x08 \x01(\x0b\x32\r.ComputationsH\x00\x12\x1f\n\tvariables\x18\t \x01(\x0b\x32\n.VariablesH\x00\x12)\n\x0e\x63onfigurations\x18\n \x01(\x0b\x32\x0f.ConfigurationsH\x00\x12\x31\n\x12\x63onfigurationNotes\x18\\ \x01(\x0b\x32\x13.ConfigurationNotesH\x00\x12/\n\x11\x63onfigurationTags\x18] \x01(\x0b\x32\x12.ConfigurationTagsH\x00\x12\x33\n\x13limitConfigurations\x18\x01 \x01(\x0b\x32\x14.LimitConfigurationsH\x00\x12%\n\x0cmeasurements\x18\x02 \x01(\x0b\x32\r.MeasurementsH\x00\x12\x1f\n\ttimezones\x18\x03 \x01(\x0b\x32\n.TimezonesH\x00\x12\x1f\n\taddresses\x18\x04 \x01(\x0b\x32\n.AddressesH\x00\x12)\n\x0egaugeDataPoint\x18; \x01(\x0b\x32\x0f.GaugeDataPointH\x00\x12\x19\n\x06series\x18< \x01(\x0b\x32\x07.SeriesH\x00\x12\x33\n\x13reportParameterSets\x18\x42 \x01(\x0b\x32\x14.ReportParameterSetsH\x00\x12\x1f\n\tKeyValues\x18P \x01(\x0b\x32\n.KeyValuesH\x00\x12!\n\nparameters\x18\x0c \x01(\x0b\x32\x0b.ParametersH\x00\x12\x17\n\x05units\x18\r \x01(\x0b\x32\x06.UnitsH\x00\x12\x1d\n\x08\x61gencies\x18G \x01(\x0b\x32\t.AgenciesH\x00\x12\x35\n\x14parameterAgencyCodes\x18J \x01(\x0b\x32\x15.ParameterAgencyCodesH\x00\x12=\n\x18parameterAgencyCodeTypes\x18K \x01(\x0b\x32\x19.ParameterAgencyCodeTypesH\x00\x12+\n\x0funitAgencyCodes\x18L \x01(\x0b\x32\x10.UnitAgencyCodesH\x00\x12\x33\n\x13unitAgencyCodeTypes\x18M \x01(\x0b\x32\x14.UnitAgencyCodeTypesH\x00\x12\'\n\rquantityTypes\x18Q \x01(\x0b\x32\x0e.QuantityTypesH\x00\x12+\n\x0fmodelExecutions\x18h \x01(\x0b\x32\x10.ModelExecutionsH\x00\x12\x37\n\x15notificationTemplates\x18\x19 \x01(\x0b\x32\x16.NotificationTemplatesH\x00\x12\x31\n\x12notificationTopics\x18\x1a \x01(\x0b\x32\x13.NotificationTopicsH\x00\x12\x35\n\x14notificationContacts\x18\x1b \x01(\x0b\x32\x15.NotificationContactsH\x00\x12\x33\n\x13notificationDevices\x18\x1c \x01(\x0b\x32\x14.NotificationDevicesH\x00\x12;\n\x17notificationPreferences\x18\x1d \x01(\x0b\x32\x18.NotificationPreferencesH\x00\x12\x43\n\x1buserNotificationPreferences\x18\x1e \x01(\x0b\x32\x1c.UserNotificationPreferencesH\x00\x12?\n\x19inAppNotificationMessages\x18\x32 \x01(\x0b\x32\x1a.InAppNotificationMessagesH\x00\x12G\n\x1dnotificationDirectPreferences\x18? \x01(\x0b\x32\x1e.NotificationDirectPreferencesH\x00\x12\'\n\rscheduleTypes\x18X \x01(\x0b\x32\x0e.ScheduleTypesH\x00\x12\x1f\n\tschedules\x18Y \x01(\x0b\x32\n.SchedulesH\x00\x12\x33\n\x13scheduleOccurrences\x18[ \x01(\x0b\x32\x14.ScheduleOccurrencesH\x00\x12\x1d\n\x08\x66\x65\x61tures\x18\x1f \x01(\x0b\x32\t.FeaturesH\x00\x12-\n\x10productOfferings\x18\" \x01(\x0b\x32\x11.ProductOfferingsH\x00\x12\x17\n\x05roles\x18# \x01(\x0b\x32\x06.RolesH\x00\x12?\n\x19serviceTechTenantRequests\x18$ \x01(\x0b\x32\x1a.ServiceTechTenantRequestsH\x00\x12\x1b\n\x07tenants\x18% \x01(\x0b\x32\x08.TenantsH\x00\x12\x39\n\x16tenantProductOfferings\x18W \x01(\x0b\x32\x17.TenantProductOfferingsH\x00\x12\x17\n\x05users\x18& \x01(\x0b\x32\x06.UsersH\x00\x12+\n\x0fuserPreferences\x18\' \x01(\x0b\x32\x10.UserPreferencesH\x00\x12%\n\x0cuserProfiles\x18( \x01(\x0b\x32\r.UserProfilesH\x00\x12\x1b\n\x07\x63lients\x18\x37 \x01(\x0b\x32\x08.ClientsH\x00\x12\x19\n\x06scopes\x18\x38 \x01(\x0b\x32\x07.ScopesH\x00\x12%\n\x0c\x44igitalTwins\x18) \x01(\x0b\x32\r.DigitalTwinsH\x00\x12\x37\n\x15\x44igitalTwinUserRights\x18* \x01(\x0b\x32\x16.DigitalTwinUserRightsH\x00\x12-\n\x10\x64igitalTwinTypes\x18- \x01(\x0b\x32\x11.DigitalTwinTypesH\x00\x12\x33\n\x13\x64igitalTwinSubtypes\x18. \x01(\x0b\x32\x14.DigitalTwinSubtypesH\x00\x12\x39\n\x16propertyBagCollections\x18\x34 \x01(\x0b\x32\x17.PropertyBagCollectionsH\x00\x12\x41\n\x1a\x63olumnTelemetryPropertyBag\x18= \x01(\x0b\x32\x1b.ColumnTelemetryPropertyBagH\x00\x12K\n\x1fmeasurementTelemetryPropertyBag\x18> \x01(\x0b\x32 .MeasurementTelemetryPropertyBagH\x00\x12;\n\x17\x65nterpriseDataTelemetry\x18\x43 \x01(\x0b\x32\x18.EnterpriseDataTelemetryH\x00\x12\'\n\rplantStatuses\x18\x31 \x01(\x0b\x32\x0e.PlantStatusesH\x00\x12+\n\x0f\x61\x63\x63ountStatuses\x18+ \x01(\x0b\x32\x10.AccountStatusesH\x00\x12\x45\n\x1c\x65nterpriseDatasetDefinitions\x18\x61 \x01(\x0b\x32\x1d.EnterpriseDatasetDefinitionsH\x00\x12/\n\x11ReportDefinitions\x18H \x01(\x0b\x32\x12.ReportDefinitionsH\x00\x12\x35\n\x14ReportDefinitionRuns\x18N \x01(\x0b\x32\x15.ReportDefinitionRunsH\x00\x12\x35\n\x14ReportDefinitionTags\x18O \x01(\x0b\x32\x15.ReportDefinitionTagsH\x00\x12!\n\nReportRuns\x18\x62 \x01(\x0b\x32\x0b.ReportRunsH\x00\x12-\n\x10operationExports\x18\x66 \x01(\x0b\x32\x11.OperationExportsH\x00\x12\x15\n\x04rows\x18\x0e \x01(\x0b\x32\x05.RowsH\x00\x12\x17\n\x05\x63\x65lls\x18\x0f \x01(\x0b\x32\x06.CellsH\x00\x12!\n\nrowIndices\x18\x10 \x01(\x0b\x32\x0b.RowIndicesH\x00\x12\x39\n\x16spreadsheetDefinitions\x18\x11 \x01(\x0b\x32\x17.SpreadsheetDefinitionsH\x00\x12\x35\n\x14worksheetDefinitions\x18\x12 \x01(\x0b\x32\x15.WorksheetDefinitionsH\x00\x12;\n\x17spreadsheetComputations\x18\x13 \x01(\x0b\x32\x18.SpreadsheetComputationsH\x00\x12\'\n\ncellValues\x18\x64 \x01(\x0b\x32\x11.CellValueBackupsH\x00\x12)\n\x0boutputCells\x18\x65 \x01(\x0b\x32\x12.OutputCellBackupsH\x00\x12\x34\n\x17\x63oagulationMeasurements\x18U \x01(\x0b\x32\x11.CoagMeasurementsH\x00\x12\x1d\n\x08\x41nalytes\x18^ \x01(\x0b\x32\t.AnalytesH\x00\x12/\n\x11TestAnalyteGroups\x18_ \x01(\x0b\x32\x12.TestAnalyteGroupsH\x00\x12)\n\x0e\x41nalyteResults\x18g \x01(\x0b\x32\x0f.AnalyteResultsH\x00\x12+\n\x0ftimeSeriesDatas\x18V \x01(\x0b\x32\x10.TimeSeriesDatasH\x00\x12)\n\x0ehistorianDatas\x18Z \x01(\x0b\x32\x0f.HistorianDatasH\x00\x12\'\n\ringestClients\x18\x63 \x01(\x0b\x32\x0e.IngestClientsH\x00\x42\t\n\x07\x63ontentB\x14\xaa\x02\x11ONE.Models.CSharpb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\rcontent.proto\x1a\x0b\x63\x65lls.proto\x1a\x13\x63onfiguration.proto\x1a\x11\x63omputation.proto\x1a\x19limit_configuration.proto\x1a\x11measurement.proto\x1a\trow.proto\x1a\x0frow_index.proto\x1a\x1cspreadsheet_definition.proto\x1a\x1aworksheet_definition.proto\x1a\x1dspreadsheet_computation.proto\x1a\x1bnotification_template.proto\x1a\x1anotification_contact.proto\x1a\x19notification_device.proto\x1a\x1dnotification_preference.proto\x1a\"notification_user_preference.proto\x1a$notification_direct_preference.proto\x1a\x18notification_topic.proto\x1a\x0fparameter.proto\x1a\nunit.proto\x1a\x0ftimezones.proto\x1a\x0evariable.proto\x1a\raddress.proto\x1a\rfeature.proto\x1a\x16product_offering.proto\x1a\nrole.proto\x1a!service_tech_tenant_request.proto\x1a\x0ctenant.proto\x1a\x1dtenant_product_offering.proto\x1a\nuser.proto\x1a\x15user_preference.proto\x1a\x12user_profile.proto\x1a\x12\x64igital_twin.proto\x1a\x1d\x64igital_twin_user_right.proto\x1a\x14\x61\x63\x63ount_status.proto\x1a\x17\x64igital_twin_type.proto\x1a\x1a\x64igital_twin_subtype.proto\x1a\x12plant_status.proto\x1a.notification_in_app_notification_message.proto\x1a&digital_twin_subtype_propertybag.proto\x1a\x0c\x63lient.proto\x1a\x0bscope.proto\x1a\x16gauge_data_point.proto\x1a\x0cseries.proto\x1a/digital_twin_column_telemetry_propertybag.proto\x1a\x33\x64igital_twin_instrument_telemetry_propertybag.proto\x1a\x0e\x61\x63tivity.proto\x1a,digital_twin_enterprise_data_telemetry.proto\x1a\x16report_parameter.proto\x1a\x0c\x61gency.proto\x1a\x17report_definition.proto\x1a\x1bparameter_agency_code.proto\x1a parameter_agency_code_type.proto\x1a\x16unit_agency_code.proto\x1a\x1bunit_agency_code_type.proto\x1a\x1creport_definition_runs.proto\x1a\x1creport_definition_tags.proto\x1a\x0fkey_value.proto\x1a\x13quantity_type.proto\x1a\x15\x63oagmeasurement.proto\x1a\x14timeseriesdata.proto\x1a\x13schedule_type.proto\x1a\x0eschedule.proto\x1a\x14historian_data.proto\x1a\x19schedule_occurrence.proto\x1a\x18\x63onfiguration_note.proto\x1a\x17\x63onfiguration_tag.proto\x1a\ranalyte.proto\x1a\x18test_analyte_group.proto\x1a#enterprise_dataset_definition.proto\x1a\x10report_run.proto\x1a\x13ingest_client.proto\x1a\x16\x63\x65llvalue_backup.proto\x1a\x17outputcell_backup.proto\x1a\x16operation_export.proto\x1a\x14\x61nalyte_result.proto\x1a\x15model_execution.proto\x1a\x14model_template.proto\"\xe6\x1b\n\x07\x43ontent\x12!\n\nactivities\x18@ \x01(\x0b\x32\x0b.ActivitiesH\x00\x12%\n\x0c\x63omputations\x18\x08 \x01(\x0b\x32\r.ComputationsH\x00\x12\x1f\n\tvariables\x18\t \x01(\x0b\x32\n.VariablesH\x00\x12)\n\x0e\x63onfigurations\x18\n \x01(\x0b\x32\x0f.ConfigurationsH\x00\x12\x31\n\x12\x63onfigurationNotes\x18\\ \x01(\x0b\x32\x13.ConfigurationNotesH\x00\x12/\n\x11\x63onfigurationTags\x18] \x01(\x0b\x32\x12.ConfigurationTagsH\x00\x12\x33\n\x13limitConfigurations\x18\x01 \x01(\x0b\x32\x14.LimitConfigurationsH\x00\x12%\n\x0cmeasurements\x18\x02 \x01(\x0b\x32\r.MeasurementsH\x00\x12\x1f\n\ttimezones\x18\x03 \x01(\x0b\x32\n.TimezonesH\x00\x12\x1f\n\taddresses\x18\x04 \x01(\x0b\x32\n.AddressesH\x00\x12)\n\x0egaugeDataPoint\x18; \x01(\x0b\x32\x0f.GaugeDataPointH\x00\x12\x19\n\x06series\x18< \x01(\x0b\x32\x07.SeriesH\x00\x12\x33\n\x13reportParameterSets\x18\x42 \x01(\x0b\x32\x14.ReportParameterSetsH\x00\x12\x1f\n\tKeyValues\x18P \x01(\x0b\x32\n.KeyValuesH\x00\x12!\n\nparameters\x18\x0c \x01(\x0b\x32\x0b.ParametersH\x00\x12\x17\n\x05units\x18\r \x01(\x0b\x32\x06.UnitsH\x00\x12\x1d\n\x08\x61gencies\x18G \x01(\x0b\x32\t.AgenciesH\x00\x12\x35\n\x14parameterAgencyCodes\x18J \x01(\x0b\x32\x15.ParameterAgencyCodesH\x00\x12=\n\x18parameterAgencyCodeTypes\x18K \x01(\x0b\x32\x19.ParameterAgencyCodeTypesH\x00\x12+\n\x0funitAgencyCodes\x18L \x01(\x0b\x32\x10.UnitAgencyCodesH\x00\x12\x33\n\x13unitAgencyCodeTypes\x18M \x01(\x0b\x32\x14.UnitAgencyCodeTypesH\x00\x12\'\n\rquantityTypes\x18Q \x01(\x0b\x32\x0e.QuantityTypesH\x00\x12+\n\x0fmodelExecutions\x18h \x01(\x0b\x32\x10.ModelExecutionsH\x00\x12)\n\x0emodelTemplates\x18i \x01(\x0b\x32\x0f.ModelTemplatesH\x00\x12\x37\n\x15notificationTemplates\x18\x19 \x01(\x0b\x32\x16.NotificationTemplatesH\x00\x12\x31\n\x12notificationTopics\x18\x1a \x01(\x0b\x32\x13.NotificationTopicsH\x00\x12\x35\n\x14notificationContacts\x18\x1b \x01(\x0b\x32\x15.NotificationContactsH\x00\x12\x33\n\x13notificationDevices\x18\x1c \x01(\x0b\x32\x14.NotificationDevicesH\x00\x12;\n\x17notificationPreferences\x18\x1d \x01(\x0b\x32\x18.NotificationPreferencesH\x00\x12\x43\n\x1buserNotificationPreferences\x18\x1e \x01(\x0b\x32\x1c.UserNotificationPreferencesH\x00\x12?\n\x19inAppNotificationMessages\x18\x32 \x01(\x0b\x32\x1a.InAppNotificationMessagesH\x00\x12G\n\x1dnotificationDirectPreferences\x18? \x01(\x0b\x32\x1e.NotificationDirectPreferencesH\x00\x12\'\n\rscheduleTypes\x18X \x01(\x0b\x32\x0e.ScheduleTypesH\x00\x12\x1f\n\tschedules\x18Y \x01(\x0b\x32\n.SchedulesH\x00\x12\x33\n\x13scheduleOccurrences\x18[ \x01(\x0b\x32\x14.ScheduleOccurrencesH\x00\x12\x1d\n\x08\x66\x65\x61tures\x18\x1f \x01(\x0b\x32\t.FeaturesH\x00\x12-\n\x10productOfferings\x18\" \x01(\x0b\x32\x11.ProductOfferingsH\x00\x12\x17\n\x05roles\x18# \x01(\x0b\x32\x06.RolesH\x00\x12?\n\x19serviceTechTenantRequests\x18$ \x01(\x0b\x32\x1a.ServiceTechTenantRequestsH\x00\x12\x1b\n\x07tenants\x18% \x01(\x0b\x32\x08.TenantsH\x00\x12\x39\n\x16tenantProductOfferings\x18W \x01(\x0b\x32\x17.TenantProductOfferingsH\x00\x12\x17\n\x05users\x18& \x01(\x0b\x32\x06.UsersH\x00\x12+\n\x0fuserPreferences\x18\' \x01(\x0b\x32\x10.UserPreferencesH\x00\x12%\n\x0cuserProfiles\x18( \x01(\x0b\x32\r.UserProfilesH\x00\x12\x1b\n\x07\x63lients\x18\x37 \x01(\x0b\x32\x08.ClientsH\x00\x12\x19\n\x06scopes\x18\x38 \x01(\x0b\x32\x07.ScopesH\x00\x12%\n\x0c\x44igitalTwins\x18) \x01(\x0b\x32\r.DigitalTwinsH\x00\x12\x37\n\x15\x44igitalTwinUserRights\x18* \x01(\x0b\x32\x16.DigitalTwinUserRightsH\x00\x12-\n\x10\x64igitalTwinTypes\x18- \x01(\x0b\x32\x11.DigitalTwinTypesH\x00\x12\x33\n\x13\x64igitalTwinSubtypes\x18. \x01(\x0b\x32\x14.DigitalTwinSubtypesH\x00\x12\x39\n\x16propertyBagCollections\x18\x34 \x01(\x0b\x32\x17.PropertyBagCollectionsH\x00\x12\x41\n\x1a\x63olumnTelemetryPropertyBag\x18= \x01(\x0b\x32\x1b.ColumnTelemetryPropertyBagH\x00\x12K\n\x1fmeasurementTelemetryPropertyBag\x18> \x01(\x0b\x32 .MeasurementTelemetryPropertyBagH\x00\x12;\n\x17\x65nterpriseDataTelemetry\x18\x43 \x01(\x0b\x32\x18.EnterpriseDataTelemetryH\x00\x12\'\n\rplantStatuses\x18\x31 \x01(\x0b\x32\x0e.PlantStatusesH\x00\x12+\n\x0f\x61\x63\x63ountStatuses\x18+ \x01(\x0b\x32\x10.AccountStatusesH\x00\x12\x45\n\x1c\x65nterpriseDatasetDefinitions\x18\x61 \x01(\x0b\x32\x1d.EnterpriseDatasetDefinitionsH\x00\x12/\n\x11ReportDefinitions\x18H \x01(\x0b\x32\x12.ReportDefinitionsH\x00\x12\x35\n\x14ReportDefinitionRuns\x18N \x01(\x0b\x32\x15.ReportDefinitionRunsH\x00\x12\x35\n\x14ReportDefinitionTags\x18O \x01(\x0b\x32\x15.ReportDefinitionTagsH\x00\x12!\n\nReportRuns\x18\x62 \x01(\x0b\x32\x0b.ReportRunsH\x00\x12-\n\x10operationExports\x18\x66 \x01(\x0b\x32\x11.OperationExportsH\x00\x12\x15\n\x04rows\x18\x0e \x01(\x0b\x32\x05.RowsH\x00\x12\x17\n\x05\x63\x65lls\x18\x0f \x01(\x0b\x32\x06.CellsH\x00\x12!\n\nrowIndices\x18\x10 \x01(\x0b\x32\x0b.RowIndicesH\x00\x12\x39\n\x16spreadsheetDefinitions\x18\x11 \x01(\x0b\x32\x17.SpreadsheetDefinitionsH\x00\x12\x35\n\x14worksheetDefinitions\x18\x12 \x01(\x0b\x32\x15.WorksheetDefinitionsH\x00\x12;\n\x17spreadsheetComputations\x18\x13 \x01(\x0b\x32\x18.SpreadsheetComputationsH\x00\x12\'\n\ncellValues\x18\x64 \x01(\x0b\x32\x11.CellValueBackupsH\x00\x12)\n\x0boutputCells\x18\x65 \x01(\x0b\x32\x12.OutputCellBackupsH\x00\x12\x34\n\x17\x63oagulationMeasurements\x18U \x01(\x0b\x32\x11.CoagMeasurementsH\x00\x12\x1d\n\x08\x41nalytes\x18^ \x01(\x0b\x32\t.AnalytesH\x00\x12/\n\x11TestAnalyteGroups\x18_ \x01(\x0b\x32\x12.TestAnalyteGroupsH\x00\x12)\n\x0e\x41nalyteResults\x18g \x01(\x0b\x32\x0f.AnalyteResultsH\x00\x12+\n\x0ftimeSeriesDatas\x18V \x01(\x0b\x32\x10.TimeSeriesDatasH\x00\x12)\n\x0ehistorianDatas\x18Z \x01(\x0b\x32\x0f.HistorianDatasH\x00\x12\'\n\ringestClients\x18\x63 \x01(\x0b\x32\x0e.IngestClientsH\x00\x42\t\n\x07\x63ontentB\x14\xaa\x02\x11ONE.Models.CSharpb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'content_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'\252\002\021ONE.Models.CSharp'
-  _globals['_CONTENT']._serialized_start=1869
-  _globals['_CONTENT']._serialized_end=5384
+  _globals['_CONTENT']._serialized_start=1891
+  _globals['_CONTENT']._serialized_end=5449
 # @@protoc_insertion_point(module_scope)
```

### Comparing `one_interfaces-6.6.0/one_interfaces/csv_configuration_file_pb2.py` & `one_interfaces-6.7.0/one_interfaces/csv_configuration_file_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/data_source_binding_pb2.py` & `one_interfaces-6.7.0/one_interfaces/data_source_binding_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/data_source_configuration_pb2.py` & `one_interfaces-6.7.0/one_interfaces/data_source_configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/digital_twin_column_telemetry_propertybag_pb2.py` & `one_interfaces-6.7.0/one_interfaces/digital_twin_column_telemetry_propertybag_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/digital_twin_enterprise_data_telemetry_pb2.py` & `one_interfaces-6.7.0/one_interfaces/digital_twin_enterprise_data_telemetry_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/digital_twin_instrument_telemetry_propertybag_pb2.py` & `one_interfaces-6.7.0/one_interfaces/digital_twin_instrument_telemetry_propertybag_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/digital_twin_pb2.py` & `one_interfaces-6.7.0/one_interfaces/digital_twin_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/digital_twin_subtype_pb2.py` & `one_interfaces-6.7.0/one_interfaces/digital_twin_subtype_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/digital_twin_subtype_propertybag_pb2.py` & `one_interfaces-6.7.0/one_interfaces/digital_twin_subtype_propertybag_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/digital_twin_type_pb2.py` & `one_interfaces-6.7.0/one_interfaces/digital_twin_type_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/digital_twin_user_right_pb2.py` & `one_interfaces-6.7.0/one_interfaces/digital_twin_user_right_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/display_options_pb2.py` & `one_interfaces-6.7.0/one_interfaces/display_options_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/enterprise_data_source_definition_pb2.py` & `one_interfaces-6.7.0/one_interfaces/enterprise_data_source_definition_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/enterprise_data_table_definition_pb2.py` & `one_interfaces-6.7.0/one_interfaces/enterprise_data_table_definition_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/enterprise_data_table_field_pb2.py` & `one_interfaces-6.7.0/one_interfaces/enterprise_data_table_field_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/enterprise_data_table_query_parameter_pb2.py` & `one_interfaces-6.7.0/one_interfaces/enterprise_data_table_query_parameter_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/enterprise_data_table_query_pb2.py` & `one_interfaces-6.7.0/one_interfaces/enterprise_data_table_query_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/enterprise_dataset_definition_pb2.py` & `one_interfaces-6.7.0/one_interfaces/enterprise_dataset_definition_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/enum_aggregate_pb2.py` & `one_interfaces-6.7.0/one_interfaces/enum_aggregate_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/enum_auditevent_pb2.py` & `one_interfaces-6.7.0/one_interfaces/enum_auditevent_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/enum_azure_notification_hubtype_pb2.py` & `one_interfaces-6.7.0/one_interfaces/enum_azure_notification_hubtype_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/enum_cell_range_action_pb2.py` & `one_interfaces-6.7.0/one_interfaces/enum_cell_range_action_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/enum_datasource_pb2.py` & `one_interfaces-6.7.0/one_interfaces/enum_datasource_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/enum_day_pb2.py` & `one_interfaces-6.7.0/one_interfaces/enum_day_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/enum_digital_twin_dataset_output_format_pb2.py` & `one_interfaces-6.7.0/one_interfaces/enum_digital_twin_dataset_output_format_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/enum_digital_twin_restriction_pb2.py` & `one_interfaces-6.7.0/one_interfaces/enum_digital_twin_restriction_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/enum_digital_twin_user_right_pb2.py` & `one_interfaces-6.7.0/one_interfaces/enum_digital_twin_user_right_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/enum_domain_source_pb2.py` & `one_interfaces-6.7.0/one_interfaces/enum_domain_source_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/enum_entity_pb2.py` & `one_interfaces-6.7.0/one_interfaces/enum_entity_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/enum_identity_provider_pb2.py` & `one_interfaces-6.7.0/one_interfaces/enum_identity_provider_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/enum_import_status_pb2.py` & `one_interfaces-6.7.0/one_interfaces/enum_import_status_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/enum_limit_operation_pb2.py` & `one_interfaces-6.7.0/one_interfaces/enum_limit_operation_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/enum_limit_pb2.py` & `one_interfaces-6.7.0/one_interfaces/enum_limit_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/enum_month_pb2.py` & `one_interfaces-6.7.0/one_interfaces/enum_month_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/enum_notification_category_pb2.py` & `one_interfaces-6.7.0/one_interfaces/enum_notification_category_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/enum_notification_delivery_method_pb2.py` & `one_interfaces-6.7.0/one_interfaces/enum_notification_delivery_method_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/enum_notification_message_type_pb2.py` & `one_interfaces-6.7.0/one_interfaces/enum_notification_message_type_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/enum_notification_platform_pb2.py` & `one_interfaces-6.7.0/one_interfaces/enum_notification_platform_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/enum_one_log_level_pb2.py` & `one_interfaces-6.7.0/one_interfaces/enum_one_log_level_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/enum_output_placement_pb2.py` & `one_interfaces-6.7.0/one_interfaces/enum_output_placement_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/enum_rendering_engine_pb2.py` & `one_interfaces-6.7.0/one_interfaces/enum_rendering_engine_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/enum_reportable_qualifier_definition_pb2.py` & `one_interfaces-6.7.0/one_interfaces/enum_reportable_qualifier_definition_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/enum_reportable_qualifier_pb2.py` & `one_interfaces-6.7.0/one_interfaces/enum_reportable_qualifier_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/enum_sampling_statistic_pb2.py` & `one_interfaces-6.7.0/one_interfaces/enum_sampling_statistic_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/enum_time_context_pb2.py` & `one_interfaces-6.7.0/one_interfaces/enum_time_context_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/enum_time_unit_pb2.py` & `one_interfaces-6.7.0/one_interfaces/enum_time_unit_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/enum_timezone_pb2.py` & `one_interfaces-6.7.0/one_interfaces/enum_timezone_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/enum_valid_value_restriction_pb2.py` & `one_interfaces-6.7.0/one_interfaces/enum_valid_value_restriction_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/enum_variable_type_pb2.py` & `one_interfaces-6.7.0/one_interfaces/enum_variable_type_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/enum_wims_week_definition_pb2.py` & `one_interfaces-6.7.0/one_interfaces/enum_wims_week_definition_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/enum_worksheet_pb2.py` & `one_interfaces-6.7.0/one_interfaces/enum_worksheet_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/execution_details_pb2.py` & `one_interfaces-6.7.0/one_interfaces/execution_details_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/expression_line_pb2.py` & `one_interfaces-6.7.0/one_interfaces/expression_line_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/feature_pb2.py` & `one_interfaces-6.7.0/one_interfaces/feature_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/feature_state_type_pb2.py` & `one_interfaces-6.7.0/one_interfaces/feature_state_type_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/file_configuration_pb2.py` & `one_interfaces-6.7.0/one_interfaces/file_configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/gauge_data_point_pb2.py` & `one_interfaces-6.7.0/one_interfaces/gauge_data_point_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/gis_pb2.py` & `one_interfaces-6.7.0/one_interfaces/gis_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/historian_binding_pb2.py` & `one_interfaces-6.7.0/one_interfaces/historian_binding_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/historian_data_pb2.py` & `one_interfaces-6.7.0/one_interfaces/historian_data_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/i18nkey_text_reference_pb2.py` & `one_interfaces-6.7.0/one_interfaces/i18nkey_text_reference_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/ingest_client_pb2.py` & `one_interfaces-6.7.0/one_interfaces/ingest_client_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/jsonTicksDateTime_pb2.py` & `one_interfaces-6.7.0/one_interfaces/jsonTicksDateTime_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/key_value_pb2.py` & `one_interfaces-6.7.0/one_interfaces/key_value_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/limit_configuration_pb2.py` & `one_interfaces-6.7.0/one_interfaces/limit_configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/limit_pb2.py` & `one_interfaces-6.7.0/one_interfaces/limit_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/measurement_pb2.py` & `one_interfaces-6.7.0/one_interfaces/measurement_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/model_execution_pb2.py` & `one_interfaces-6.7.0/one_interfaces/template_parameter_pb2.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,28 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: model_execution.proto
+# source: template_parameter.proto
 # Protobuf Python Version: 4.25.3
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
-import model_parameter_pb2 as model__parameter__pb2
-import model_location_pb2 as model__location__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15model_execution.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x15model_parameter.proto\x1a\x14model_location.proto\"\xf9\x03\n\x0eModelExecution\x12\x0e\n\x06schema\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x11\n\ttwinRefId\x18\x03 \x01(\t\x12\x17\n\x0f\x65xternalModelId\x18\x04 \x01(\t\x12\x1d\n\x15\x66orecastDurationHours\x18\x05 \x01(\x01\x12;\n\x15inputDataSourceDriver\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x34\n\x0einputDataSetId\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12<\n\x16outputDataSourceDriver\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x35\n\x0foutputDataSetId\x18\t \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12!\n\tlocations\x18\n \x03(\x0b\x32\x0e.ModelLocation\x12\x1f\n\x06inputs\x18\x0b \x03(\x0b\x32\x0f.ModelParameter\x12 \n\x07outputs\x18\x0c \x03(\x0b\x32\x0f.ModelParameter\x12-\n\x07\x63omment\x18\r \x01(\x0b\x32\x1c.google.protobuf.StringValue\"1\n\x0fModelExecutions\x12\x1e\n\x05items\x18\x01 \x03(\x0b\x32\x0f.ModelExecutionB\x14\xaa\x02\x11ONE.Models.CSharpb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18template_parameter.proto\x1a\x1egoogle/protobuf/wrappers.proto\"\xca\x02\n\x11TemplateParameter\x12\x13\n\x0bparameterId\x18\x01 \x01(\r\x12\x11\n\toneUnitId\x18\x02 \x01(\r\x12\x31\n\x0btelemetryId\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x10\n\x08location\x18\x04 \x01(\t\x12\x10\n\x08modelTag\x18\x05 \x01(\t\x12\x11\n\tmodelUnit\x18\x06 \x01(\t\x12\x0c\n\x04name\x18\x07 \x01(\t\x12\x31\n\x0b\x64\x65scription\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x30\n\nupperLimit\x18\t \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x30\n\nlowerLimit\x18\n \x01(\x0b\x32\x1c.google.protobuf.DoubleValueB\x14\xaa\x02\x11ONE.Models.CSharpb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'model_execution_pb2', _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'template_parameter_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'\252\002\021ONE.Models.CSharp'
-  _globals['_MODELEXECUTION']._serialized_start=103
-  _globals['_MODELEXECUTION']._serialized_end=608
-  _globals['_MODELEXECUTIONS']._serialized_start=610
-  _globals['_MODELEXECUTIONS']._serialized_end=659
+  _globals['_TEMPLATEPARAMETER']._serialized_start=61
+  _globals['_TEMPLATEPARAMETER']._serialized_end=391
 # @@protoc_insertion_point(module_scope)
```

### Comparing `one_interfaces-6.6.0/one_interfaces/model_location_pb2.py` & `one_interfaces-6.7.0/one_interfaces/model_location_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/model_parameter_pb2.py` & `one_interfaces-6.7.0/one_interfaces/tenant_pb2.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: model_parameter.proto
+# source: tenant.proto
 # Protobuf Python Version: 4.25.3
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
+from google.protobuf import field_mask_pb2 as google_dot_protobuf_dot_field__mask__pb2
+import enum_timezone_pb2 as enum__timezone__pb2
+import record_auditinfo_pb2 as record__auditinfo__pb2
+import product_offering_pb2 as product__offering__pb2
+import service_tech_tenant_request_pb2 as service__tech__tenant__request__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15model_parameter.proto\x1a\x1egoogle/protobuf/wrappers.proto\"\xf1\x04\n\x0eModelParameter\x12,\n\x06\x61qiTag\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x61qiUnit\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x31\n\x0btelemetryId\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12.\n\x08location\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12.\n\x08modelTag\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tmodelUnit\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x31\n\x0b\x64\x65scription\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x30\n\nupperLimit\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x30\n\nlowerLimit\x18\t \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12-\n\x07\x63omment\x18\n \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x06values\x18\x0b \x03(\x0b\x32\x1b.ModelParameter.ValuesEntry\x1aK\n\x0bValuesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12+\n\x05value\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue:\x02\x38\x01\x42\x14\xaa\x02\x11ONE.Models.CSharpb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0ctenant.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a google/protobuf/field_mask.proto\x1a\x13\x65num_timezone.proto\x1a\x16record_auditinfo.proto\x1a\x16product_offering.proto\x1a!service_tech_tenant_request.proto\"\x8b\x03\n\x06Tenant\x12\n\n\x02id\x18\x01 \x01(\t\x12*\n\x04name\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63ulture\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12#\n\x0c\x65numTimeZone\x18\x04 \x01(\x0e\x32\r.EnumTimeZone\x12*\n\x10productOfferings\x18\x05 \x03(\x0b\x32\x10.ProductOffering\x12<\n\x19serviceTechTenantRequests\x18\x07 \x03(\x0b\x32\x19.ServiceTechTenantRequest\x12\x30\n\nchargifyId\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12.\n\nupdateMask\x18\x62 \x01(\x0b\x32\x1a.google.protobuf.FieldMask\x12)\n\x0frecordAuditInfo\x18\x63 \x01(\x0b\x32\x10.RecordAuditInfo\"!\n\x07Tenants\x12\x16\n\x05items\x18\x01 \x03(\x0b\x32\x07.TenantB\x14\xaa\x02\x11ONE.Models.CSharpb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'model_parameter_pb2', _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tenant_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'\252\002\021ONE.Models.CSharp'
-  _globals['_MODELPARAMETER_VALUESENTRY']._options = None
-  _globals['_MODELPARAMETER_VALUESENTRY']._serialized_options = b'8\001'
-  _globals['_MODELPARAMETER']._serialized_start=58
-  _globals['_MODELPARAMETER']._serialized_end=683
-  _globals['_MODELPARAMETER_VALUESENTRY']._serialized_start=608
-  _globals['_MODELPARAMETER_VALUESENTRY']._serialized_end=683
+  _globals['_TENANT']._serialized_start=187
+  _globals['_TENANT']._serialized_end=582
+  _globals['_TENANTS']._serialized_start=584
+  _globals['_TENANTS']._serialized_end=617
 # @@protoc_insertion_point(module_scope)
```

### Comparing `one_interfaces-6.6.0/one_interfaces/multi_point2d_pb2.py` & `one_interfaces-6.7.0/one_interfaces/multi_point2d_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/multi_point3d_pb2.py` & `one_interfaces-6.7.0/one_interfaces/multi_point3d_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/note_pb2.py` & `one_interfaces-6.7.0/one_interfaces/note_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/notification_broadcast_pb2.py` & `one_interfaces-6.7.0/one_interfaces/notification_broadcast_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/notification_contact_pb2.py` & `one_interfaces-6.7.0/one_interfaces/notification_contact_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/notification_device_pb2.py` & `one_interfaces-6.7.0/one_interfaces/notification_device_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/notification_direct_preference_pb2.py` & `one_interfaces-6.7.0/one_interfaces/notification_direct_preference_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/notification_event_pb2.py` & `one_interfaces-6.7.0/one_interfaces/notification_event_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/notification_in_app_notification_message_pb2.py` & `one_interfaces-6.7.0/one_interfaces/notification_in_app_notification_message_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/notification_preference_pb2.py` & `one_interfaces-6.7.0/one_interfaces/notification_preference_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/notification_template_pb2.py` & `one_interfaces-6.7.0/one_interfaces/notification_template_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/notification_topic_pb2.py` & `one_interfaces-6.7.0/one_interfaces/notification_topic_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/notification_topic_variable_pb2.py` & `one_interfaces-6.7.0/one_interfaces/notification_topic_variable_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/notification_user_preference_pb2.py` & `one_interfaces-6.7.0/one_interfaces/notification_user_preference_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/operation_export_pb2.py` & `one_interfaces-6.7.0/one_interfaces/operation_export_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/outputcell_backup_pb2.py` & `one_interfaces-6.7.0/one_interfaces/outputcell_backup_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/pagination_pb2.py` & `one_interfaces-6.7.0/one_interfaces/pagination_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/parameter_agency_code_pb2.py` & `one_interfaces-6.7.0/one_interfaces/parameter_agency_code_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/parameter_agency_code_type_pb2.py` & `one_interfaces-6.7.0/one_interfaces/parameter_agency_code_type_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/parameter_definition_pb2.py` & `one_interfaces-6.7.0/one_interfaces/parameter_definition_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/parameter_pb2.py` & `one_interfaces-6.7.0/one_interfaces/parameter_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/plant_status_pb2.py` & `one_interfaces-6.7.0/one_interfaces/plant_status_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/point2d_pb2.py` & `one_interfaces-6.7.0/one_interfaces/point2d_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/point3d_pb2.py` & `one_interfaces-6.7.0/one_interfaces/point3d_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/post_filtering_column_definition_pb2.py` & `one_interfaces-6.7.0/one_interfaces/post_filtering_column_definition_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/post_filtering_pb2.py` & `one_interfaces-6.7.0/one_interfaces/post_filtering_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/privileges_pb2.py` & `one_interfaces-6.7.0/one_interfaces/privileges_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/product_offering_pb2.py` & `one_interfaces-6.7.0/one_interfaces/product_offering_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/quantity_type_pb2.py` & `one_interfaces-6.7.0/one_interfaces/quantity_type_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/record_auditinfo_pb2.py` & `one_interfaces-6.7.0/one_interfaces/record_auditinfo_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/report_definition_json_v2_pb2.py` & `one_interfaces-6.7.0/one_interfaces/report_definition_json_v2_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/report_definition_pb2.py` & `one_interfaces-6.7.0/one_interfaces/report_definition_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/report_definition_runs_pb2.py` & `one_interfaces-6.7.0/one_interfaces/report_definition_runs_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/report_definition_tags_pb2.py` & `one_interfaces-6.7.0/one_interfaces/report_definition_tags_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/report_parameter_pb2.py` & `one_interfaces-6.7.0/one_interfaces/report_parameter_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/report_run_pb2.py` & `one_interfaces-6.7.0/one_interfaces/report_run_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/reportable_qualifier_definition_pb2.py` & `one_interfaces-6.7.0/one_interfaces/reportable_qualifier_definition_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/reportable_qualifier_pb2.py` & `one_interfaces-6.7.0/one_interfaces/reportable_qualifier_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/rights_pb2.py` & `one_interfaces-6.7.0/one_interfaces/rights_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/role_pb2.py` & `one_interfaces-6.7.0/one_interfaces/role_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/row_index_pb2.py` & `one_interfaces-6.7.0/one_interfaces/row_index_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/row_merge_result_pb2.py` & `one_interfaces-6.7.0/one_interfaces/row_merge_result_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/row_pb2.py` & `one_interfaces-6.7.0/one_interfaces/row_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/schedule_occurrence_pb2.py` & `one_interfaces-6.7.0/one_interfaces/schedule_occurrence_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/schedule_pb2.py` & `one_interfaces-6.7.0/one_interfaces/schedule_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/schedule_recurrence_pattern_pb2.py` & `one_interfaces-6.7.0/one_interfaces/schedule_recurrence_pattern_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/schedule_type_pb2.py` & `one_interfaces-6.7.0/one_interfaces/schedule_type_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/scope_pb2.py` & `one_interfaces-6.7.0/one_interfaces/scope_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/search_option_pb2.py` & `one_interfaces-6.7.0/one_interfaces/search_option_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/series_pb2.py` & `one_interfaces-6.7.0/one_interfaces/series_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/service_tech_tenant_request_pb2.py` & `one_interfaces-6.7.0/one_interfaces/service_tech_tenant_request_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/signalr_one_hub_connection_info_pb2.py` & `one_interfaces-6.7.0/one_interfaces/signalr_one_hub_connection_info_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/signalr_one_hub_dataset_event_pb2.py` & `one_interfaces-6.7.0/one_interfaces/signalr_one_hub_dataset_event_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/signalr_one_hub_event_payload_pb2.py` & `one_interfaces-6.7.0/one_interfaces/signalr_one_hub_event_payload_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/signalr_one_hub_event_pb2.py` & `one_interfaces-6.7.0/one_interfaces/signalr_one_hub_event_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/signalr_one_hub_message_pb2.py` & `one_interfaces-6.7.0/one_interfaces/signalr_one_hub_message_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/spreadsheet_binding_pb2.py` & `one_interfaces-6.7.0/one_interfaces/spreadsheet_binding_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/spreadsheet_computation_pb2.py` & `one_interfaces-6.7.0/one_interfaces/spreadsheet_computation_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/spreadsheet_definition_pb2.py` & `one_interfaces-6.7.0/one_interfaces/spreadsheet_definition_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/spreadsheet_pb2.py` & `one_interfaces-6.7.0/one_interfaces/spreadsheet_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/tenant_pb2.py` & `one_interfaces-6.7.0/one_interfaces/user_profile_pb2.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: tenant.proto
+# source: user_profile.proto
 # Protobuf Python Version: 4.25.3
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+import record_auditinfo_pb2 as record__auditinfo__pb2
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from google.protobuf import field_mask_pb2 as google_dot_protobuf_dot_field__mask__pb2
-import enum_timezone_pb2 as enum__timezone__pb2
-import record_auditinfo_pb2 as record__auditinfo__pb2
-import product_offering_pb2 as product__offering__pb2
-import service_tech_tenant_request_pb2 as service__tech__tenant__request__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0ctenant.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a google/protobuf/field_mask.proto\x1a\x13\x65num_timezone.proto\x1a\x16record_auditinfo.proto\x1a\x16product_offering.proto\x1a!service_tech_tenant_request.proto\"\x8b\x03\n\x06Tenant\x12\n\n\x02id\x18\x01 \x01(\t\x12*\n\x04name\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63ulture\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12#\n\x0c\x65numTimeZone\x18\x04 \x01(\x0e\x32\r.EnumTimeZone\x12*\n\x10productOfferings\x18\x05 \x03(\x0b\x32\x10.ProductOffering\x12<\n\x19serviceTechTenantRequests\x18\x07 \x03(\x0b\x32\x19.ServiceTechTenantRequest\x12\x30\n\nchargifyId\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12.\n\nupdateMask\x18\x62 \x01(\x0b\x32\x1a.google.protobuf.FieldMask\x12)\n\x0frecordAuditInfo\x18\x63 \x01(\x0b\x32\x10.RecordAuditInfo\"!\n\x07Tenants\x12\x16\n\x05items\x18\x01 \x03(\x0b\x32\x07.TenantB\x14\xaa\x02\x11ONE.Models.CSharpb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x12user_profile.proto\x1a\x16record_auditinfo.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a google/protobuf/field_mask.proto\"\xe1\x01\n\x0bUserProfile\x12\n\n\x02id\x18\x01 \x01(\t\x12\x32\n\x0clanguageCode\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x37\n\x11\x63urrentLocationId\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12.\n\nupdateMask\x18\x62 \x01(\x0b\x32\x1a.google.protobuf.FieldMask\x12)\n\x0frecordAuditInfo\x18\x63 \x01(\x0b\x32\x10.RecordAuditInfo\"+\n\x0cUserProfiles\x12\x1b\n\x05items\x18\x01 \x03(\x0b\x32\x0c.UserProfileB\x14\xaa\x02\x11ONE.Models.CSharpb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tenant_pb2', _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'user_profile_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'\252\002\021ONE.Models.CSharp'
-  _globals['_TENANT']._serialized_start=187
-  _globals['_TENANT']._serialized_end=582
-  _globals['_TENANTS']._serialized_start=584
-  _globals['_TENANTS']._serialized_end=617
+  _globals['_USERPROFILE']._serialized_start=113
+  _globals['_USERPROFILE']._serialized_end=338
+  _globals['_USERPROFILES']._serialized_start=340
+  _globals['_USERPROFILES']._serialized_end=383
 # @@protoc_insertion_point(module_scope)
```

### Comparing `one_interfaces-6.6.0/one_interfaces/tenant_product_offering_pb2.py` & `one_interfaces-6.7.0/one_interfaces/tenant_product_offering_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/test_analyte_group_pb2.py` & `one_interfaces-6.7.0/one_interfaces/test_analyte_group_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/time_context_pb2.py` & `one_interfaces-6.7.0/one_interfaces/time_context_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/timeseriesdata_pb2.py` & `one_interfaces-6.7.0/one_interfaces/timeseriesdata_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/timewindow_pb2.py` & `one_interfaces-6.7.0/one_interfaces/timewindow_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/timezones_pb2.py` & `one_interfaces-6.7.0/one_interfaces/timezones_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/unit_agency_code_pb2.py` & `one_interfaces-6.7.0/one_interfaces/unit_agency_code_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/unit_agency_code_type_pb2.py` & `one_interfaces-6.7.0/one_interfaces/unit_agency_code_type_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/unit_pb2.py` & `one_interfaces-6.7.0/one_interfaces/unit_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/user_password_management_pb2.py` & `one_interfaces-6.7.0/one_interfaces/user_password_management_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/user_pb2.py` & `one_interfaces-6.7.0/one_interfaces/user_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/user_preference_pb2.py` & `one_interfaces-6.7.0/one_interfaces/user_preference_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/user_profile_pb2.py` & `one_interfaces-6.7.0/one_interfaces/execution_parameter_pb2.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: user_profile.proto
+# source: execution_parameter.proto
 # Protobuf Python Version: 4.25.3
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-import record_auditinfo_pb2 as record__auditinfo__pb2
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
-from google.protobuf import field_mask_pb2 as google_dot_protobuf_dot_field__mask__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x12user_profile.proto\x1a\x16record_auditinfo.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a google/protobuf/field_mask.proto\"\xe1\x01\n\x0bUserProfile\x12\n\n\x02id\x18\x01 \x01(\t\x12\x32\n\x0clanguageCode\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x37\n\x11\x63urrentLocationId\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12.\n\nupdateMask\x18\x62 \x01(\x0b\x32\x1a.google.protobuf.FieldMask\x12)\n\x0frecordAuditInfo\x18\x63 \x01(\x0b\x32\x10.RecordAuditInfo\"+\n\x0cUserProfiles\x12\x1b\n\x05items\x18\x01 \x03(\x0b\x32\x0c.UserProfileB\x14\xaa\x02\x11ONE.Models.CSharpb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19\x65xecution_parameter.proto\x1a\x1egoogle/protobuf/wrappers.proto\"\x9b\x02\n\x12\x45xecutionParameter\x12\x10\n\x08modelTag\x18\x01 \x01(\t\x12\x11\n\tmodelUnit\x18\x02 \x01(\t\x12\x30\n\nupperLimit\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x30\n\nlowerLimit\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12/\n\x06values\x18\x05 \x03(\x0b\x32\x1f.ExecutionParameter.ValuesEntry\x1aK\n\x0bValuesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12+\n\x05value\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue:\x02\x38\x01\x42\x14\xaa\x02\x11ONE.Models.CSharpb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'user_profile_pb2', _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'execution_parameter_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'\252\002\021ONE.Models.CSharp'
-  _globals['_USERPROFILE']._serialized_start=113
-  _globals['_USERPROFILE']._serialized_end=338
-  _globals['_USERPROFILES']._serialized_start=340
-  _globals['_USERPROFILES']._serialized_end=383
+  _globals['_EXECUTIONPARAMETER_VALUESENTRY']._options = None
+  _globals['_EXECUTIONPARAMETER_VALUESENTRY']._serialized_options = b'8\001'
+  _globals['_EXECUTIONPARAMETER']._serialized_start=62
+  _globals['_EXECUTIONPARAMETER']._serialized_end=345
+  _globals['_EXECUTIONPARAMETER_VALUESENTRY']._serialized_start=270
+  _globals['_EXECUTIONPARAMETER_VALUESENTRY']._serialized_end=345
 # @@protoc_insertion_point(module_scope)
```

### Comparing `one_interfaces-6.6.0/one_interfaces/valid_value_pb2.py` & `one_interfaces-6.7.0/one_interfaces/valid_value_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/variable_pb2.py` & `one_interfaces-6.7.0/one_interfaces/variable_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/worksheet_definition_pb2.py` & `one_interfaces-6.7.0/one_interfaces/worksheet_definition_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/worksheet_pb2.py` & `one_interfaces-6.7.0/one_interfaces/worksheet_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces/worksheet_view_pb2.py` & `one_interfaces-6.7.0/one_interfaces/worksheet_view_pb2.py`

 * *Files identical despite different names*

### Comparing `one_interfaces-6.6.0/one_interfaces.egg-info/PKG-INFO` & `one_interfaces-6.7.0/one_interfaces.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: one-interfaces
-Version: 6.6.0
+Version: 6.7.0
 Summary: Python bindings for ONE.
 Home-page: https://github.com/aquaticinformatics/one_interfaces
 Author: Aquatic Informatics
 Author-email: info@aquaticinformatics.com
 Maintainer: Aquatic Informatics
 License: BSD
 Description: One_Interfaces
```

### Comparing `one_interfaces-6.6.0/one_interfaces.egg-info/SOURCES.txt` & `one_interfaces-6.7.0/one_interfaces.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -81,14 +81,15 @@
 one_interfaces/enum_time_unit_pb2.py
 one_interfaces/enum_timezone_pb2.py
 one_interfaces/enum_valid_value_restriction_pb2.py
 one_interfaces/enum_variable_type_pb2.py
 one_interfaces/enum_wims_week_definition_pb2.py
 one_interfaces/enum_worksheet_pb2.py
 one_interfaces/execution_details_pb2.py
+one_interfaces/execution_parameter_pb2.py
 one_interfaces/expression_line_pb2.py
 one_interfaces/feature_pb2.py
 one_interfaces/feature_state_type_pb2.py
 one_interfaces/file_configuration_pb2.py
 one_interfaces/gauge_data_point_pb2.py
 one_interfaces/gis_pb2.py
 one_interfaces/historian_binding_pb2.py
@@ -98,15 +99,15 @@
 one_interfaces/jsonTicksDateTime_pb2.py
 one_interfaces/key_value_pb2.py
 one_interfaces/limit_configuration_pb2.py
 one_interfaces/limit_pb2.py
 one_interfaces/measurement_pb2.py
 one_interfaces/model_execution_pb2.py
 one_interfaces/model_location_pb2.py
-one_interfaces/model_parameter_pb2.py
+one_interfaces/model_template_pb2.py
 one_interfaces/multi_point2d_pb2.py
 one_interfaces/multi_point3d_pb2.py
 one_interfaces/note_pb2.py
 one_interfaces/notification_broadcast_pb2.py
 one_interfaces/notification_contact_pb2.py
 one_interfaces/notification_device_pb2.py
 one_interfaces/notification_direct_preference_pb2.py
@@ -159,14 +160,15 @@
 one_interfaces/signalr_one_hub_event_payload_pb2.py
 one_interfaces/signalr_one_hub_event_pb2.py
 one_interfaces/signalr_one_hub_message_pb2.py
 one_interfaces/spreadsheet_binding_pb2.py
 one_interfaces/spreadsheet_computation_pb2.py
 one_interfaces/spreadsheet_definition_pb2.py
 one_interfaces/spreadsheet_pb2.py
+one_interfaces/template_parameter_pb2.py
 one_interfaces/tenant_pb2.py
 one_interfaces/tenant_product_offering_pb2.py
 one_interfaces/test_analyte_group_pb2.py
 one_interfaces/time_context_pb2.py
 one_interfaces/timeseriesdata_pb2.py
 one_interfaces/timewindow_pb2.py
 one_interfaces/timezones_pb2.py
```

### Comparing `one_interfaces-6.6.0/setup.py` & `one_interfaces-6.7.0/setup.py`

 * *Files identical despite different names*

