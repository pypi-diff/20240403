# Comparing `tmp/s4_platform_api-1.2.0.tar.gz` & `tmp/s4_platform_api-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s4_platform_api-1.2.0.tar", max compression
+gzip compressed data, was "s4_platform_api-1.3.0.tar", max compression
```

## Comparing `s4_platform_api-1.2.0.tar` & `s4_platform_api-1.3.0.tar`

### file list

```diff
@@ -1,70 +1,71 @@
--rw-r--r--   0        0        0     1076 2023-12-18 23:30:30.806683 s4_platform_api-1.2.0/LICENSE
--rw-r--r--   0        0        0     2733 2023-12-18 23:30:30.806683 s4_platform_api-1.2.0/README.md
--rw-r--r--   0        0        0      707 2023-12-18 23:30:46.634908 s4_platform_api-1.2.0/pyproject.toml
--rw-r--r--   0        0        0       20 2023-12-18 23:30:30.810683 s4_platform_api-1.2.0/s4/platform/.env
--rw-r--r--   0        0        0        0 2023-12-18 23:30:30.810683 s4_platform_api-1.2.0/s4/platform/__init__.py
--rw-r--r--   0        0        0    14537 2023-12-18 23:30:30.810683 s4_platform_api-1.2.0/s4/platform/api.py
--rw-r--r--   0        0        0     1530 2023-12-18 23:30:30.810683 s4_platform_api-1.2.0/s4/platform/authentication_utils.py
--rw-r--r--   0        0        0     3688 2023-12-18 23:30:30.810683 s4_platform_api-1.2.0/s4/platform/changeset/changeset.py
--rw-r--r--   0        0        0     1437 2023-12-18 23:30:30.810683 s4_platform_api-1.2.0/s4/platform/changeset/changeset_config.py
--rw-r--r--   0        0        0     1019 2023-12-18 23:30:30.810683 s4_platform_api-1.2.0/s4/platform/changeset/deploy_changeset.py
--rw-r--r--   0        0        0     2256 2023-12-18 23:30:30.810683 s4_platform_api-1.2.0/s4/platform/claim/claim.py
--rw-r--r--   0        0        0     6752 2023-12-18 23:30:30.810683 s4_platform_api-1.2.0/s4/platform/connection.py
--rw-r--r--   0        0        0     1444 2023-12-18 23:30:30.810683 s4_platform_api-1.2.0/s4/platform/constants.py
--rw-r--r--   0        0        0     2233 2023-12-18 23:30:30.810683 s4_platform_api-1.2.0/s4/platform/deployment/deployment.py
--rw-r--r--   0        0        0     2174 2023-12-18 23:30:30.810683 s4_platform_api-1.2.0/s4/platform/entity/ad_hoc_entity.py
--rw-r--r--   0        0        0     8138 2023-12-18 23:30:30.810683 s4_platform_api-1.2.0/s4/platform/entity/entity.py
--rw-r--r--   0        0        0      872 2023-12-18 23:30:30.810683 s4_platform_api-1.2.0/s4/platform/entity/field_value.py
--rw-r--r--   0        0        0     1196 2023-12-18 23:30:30.810683 s4_platform_api-1.2.0/s4/platform/entity_location/entity_location.py
--rw-r--r--   0        0        0     6827 2023-12-18 23:30:30.810683 s4_platform_api-1.2.0/s4/platform/entity_type/entity_type.py
--rw-r--r--   0        0        0     2233 2023-12-18 23:30:30.810683 s4_platform_api-1.2.0/s4/platform/environment/environment.py
--rw-r--r--   0        0        0      584 2023-12-18 23:30:30.810683 s4_platform_api-1.2.0/s4/platform/environment/environment_configuration.py
--rw-r--r--   0        0        0     2171 2023-12-18 23:30:30.810683 s4_platform_api-1.2.0/s4/platform/environment/migration_plan.py
--rw-r--r--   0        0        0      246 2023-12-18 23:30:30.810683 s4_platform_api-1.2.0/s4/platform/faas/custom_errors.py
--rw-r--r--   0        0        0     2749 2023-12-18 23:30:30.810683 s4_platform_api-1.2.0/s4/platform/faas/faas_function.py
--rw-r--r--   0        0        0     5635 2023-12-18 23:30:30.810683 s4_platform_api-1.2.0/s4/platform/faas/faas_utils.py
--rw-r--r--   0        0        0     4437 2023-12-18 23:30:30.810683 s4_platform_api-1.2.0/s4/platform/file/file_reference.py
--rw-r--r--   0        0        0     1184 2023-12-18 23:30:30.810683 s4_platform_api-1.2.0/s4/platform/function/function.py
--rw-r--r--   0        0        0      248 2023-12-18 23:30:30.810683 s4_platform_api-1.2.0/s4/platform/internal/base_model.py
--rw-r--r--   0        0        0     1221 2023-12-18 23:30:30.810683 s4_platform_api-1.2.0/s4/platform/internal/base_schema.py
--rw-r--r--   0        0        0      637 2023-12-18 23:30:30.810683 s4_platform_api-1.2.0/s4/platform/internal/camel_case_schema.py
--rw-r--r--   0        0        0     2717 2023-12-18 23:30:30.810683 s4_platform_api-1.2.0/s4/platform/internal/fields_mixin.py
--rw-r--r--   0        0        0     2153 2023-12-18 23:30:30.810683 s4_platform_api-1.2.0/s4/platform/internal/lazy_property.py
--rw-r--r--   0        0        0     2030 2023-12-18 23:30:30.810683 s4_platform_api-1.2.0/s4/platform/internal/lazy_property_list.py
--rw-r--r--   0        0        0       80 2023-12-18 23:30:30.810683 s4_platform_api-1.2.0/s4/platform/internal/sort_direction.py
--rw-r--r--   0        0        0        0 2023-12-18 23:30:30.810683 s4_platform_api-1.2.0/s4/platform/link_config/__init__.py
--rw-r--r--   0        0        0      791 2023-12-18 23:30:30.810683 s4_platform_api-1.2.0/s4/platform/link_config/link_config.py
--rw-r--r--   0        0        0      564 2023-12-18 23:30:30.810683 s4_platform_api-1.2.0/s4/platform/link_config/new_workbook_link.py
--rw-r--r--   0        0        0      674 2023-12-18 23:30:30.810683 s4_platform_api-1.2.0/s4/platform/page_config/page_config.py
--rw-r--r--   0        0        0      801 2023-12-18 23:30:30.810683 s4_platform_api-1.2.0/s4/platform/page_config/page_container.py
--rw-r--r--   0        0        0      618 2023-12-18 23:30:30.810683 s4_platform_api-1.2.0/s4/platform/page_config/page_container_page_config.py
--rw-r--r--   0        0        0     2783 2023-12-18 23:30:30.810683 s4_platform_api-1.2.0/s4/platform/prospective_task/ProspectiveTaskSummary.py
--rw-r--r--   0        0        0      728 2023-12-18 23:30:30.810683 s4_platform_api-1.2.0/s4/platform/prospective_task/function_list.py
--rw-r--r--   0        0        0      910 2023-12-18 23:30:30.810683 s4_platform_api-1.2.0/s4/platform/prospective_task/function_status.py
--rw-r--r--   0        0        0     1287 2023-12-18 23:30:30.810683 s4_platform_api-1.2.0/s4/platform/prospective_task/io_group.py
--rw-r--r--   0        0        0     2162 2023-12-18 23:30:30.810683 s4_platform_api-1.2.0/s4/platform/prospective_task/prospective_entity.py
--rw-r--r--   0        0        0     1024 2023-12-18 23:30:30.810683 s4_platform_api-1.2.0/s4/platform/prospective_task/prospective_field_value.py
--rw-r--r--   0        0        0    14083 2023-12-18 23:30:30.810683 s4_platform_api-1.2.0/s4/platform/prospective_task/prospective_task.py
--rw-r--r--   0        0        0     2386 2023-12-18 23:30:30.810683 s4_platform_api-1.2.0/s4/platform/prospective_task/search.py
--rw-r--r--   0        0        0     2471 2023-12-18 23:30:30.810683 s4_platform_api-1.2.0/s4/platform/prospective_task_config/field_config.py
--rw-r--r--   0        0        0     1582 2023-12-18 23:30:30.810683 s4_platform_api-1.2.0/s4/platform/prospective_task_config/field_type.py
--rw-r--r--   0        0        0      749 2023-12-18 23:30:30.810683 s4_platform_api-1.2.0/s4/platform/prospective_task_config/field_validation.py
--rw-r--r--   0        0        0      639 2023-12-18 23:30:30.810683 s4_platform_api-1.2.0/s4/platform/prospective_task_config/from_pool_config.py
--rw-r--r--   0        0        0     1726 2023-12-18 23:30:30.810683 s4_platform_api-1.2.0/s4/platform/prospective_task_config/group_config.py
--rw-r--r--   0        0        0     1161 2023-12-18 23:30:30.810683 s4_platform_api-1.2.0/s4/platform/prospective_task_config/io_group_config.py
--rw-r--r--   0        0        0     1137 2023-12-18 23:30:30.810683 s4_platform_api-1.2.0/s4/platform/prospective_task_config/pattern.py
--rw-r--r--   0        0        0     4627 2023-12-18 23:30:30.810683 s4_platform_api-1.2.0/s4/platform/prospective_task_config/prospective_task_config.py
--rw-r--r--   0        0        0     2404 2023-12-18 23:30:30.814683 s4_platform_api-1.2.0/s4/platform/queue/entity.py
--rw-r--r--   0        0        0      540 2023-12-18 23:30:30.814683 s4_platform_api-1.2.0/s4/platform/queue/field_value.py
--rw-r--r--   0        0        0      824 2023-12-18 23:30:30.814683 s4_platform_api-1.2.0/s4/platform/queue/queue.py
--rw-r--r--   0        0        0      416 2023-12-18 23:30:30.814683 s4_platform_api-1.2.0/s4/platform/shared_schemas/field_restriction.py
--rw-r--r--   0        0        0      549 2023-12-18 23:30:30.814683 s4_platform_api-1.2.0/s4/platform/shared_schemas/field_search_request.py
--rw-r--r--   0        0        0      534 2023-12-18 23:30:30.814683 s4_platform_api-1.2.0/s4/platform/shared_schemas/iri_list_schema.py
--rw-r--r--   0        0        0      648 2023-12-18 23:30:30.814683 s4_platform_api-1.2.0/s4/platform/shared_schemas/sort_order.py
--rw-r--r--   0        0        0     1359 2023-12-18 23:30:30.814683 s4_platform_api-1.2.0/s4/platform/task/ad_hoc_task.py
--rw-r--r--   0        0        0     3262 2023-12-18 23:30:30.814683 s4_platform_api-1.2.0/s4/platform/task/task.py
--rw-r--r--   0        0        0      834 2023-12-18 23:30:30.814683 s4_platform_api-1.2.0/s4/platform/tenant_config/tenant_config.py
--rw-r--r--   0        0        0      562 2023-12-18 23:30:30.814683 s4_platform_api-1.2.0/s4/platform/workflow/config_mapping.py
--rw-r--r--   0        0        0     1833 2023-12-18 23:30:30.814683 s4_platform_api-1.2.0/s4/platform/workflow/workflow.py
--rw-r--r--   0        0        0        0 2023-12-18 23:30:30.814683 s4_platform_api-1.2.0/s4/py.typed
--rw-r--r--   0        0        0     3577 1970-01-01 00:00:00.000000 s4_platform_api-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-04-02 22:19:02.696388 s4_platform_api-1.3.0/LICENSE
+-rw-r--r--   0        0        0       76 2024-04-02 22:19:02.696388 s4_platform_api-1.3.0/README.md
+-rw-r--r--   0        0        0      760 2024-04-02 22:19:15.080399 s4_platform_api-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0       20 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/.env
+-rw-r--r--   0        0        0        0 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/__init__.py
+-rw-r--r--   0        0        0    14537 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/api.py
+-rw-r--r--   0        0        0     1530 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/authentication_utils.py
+-rw-r--r--   0        0        0     3829 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/changeset/changeset.py
+-rw-r--r--   0        0        0     1437 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/changeset/changeset_config.py
+-rw-r--r--   0        0        0     1019 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/changeset/deploy_changeset.py
+-rw-r--r--   0        0        0     2256 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/claim/claim.py
+-rw-r--r--   0        0        0     6752 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/connection.py
+-rw-r--r--   0        0        0     1444 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/constants.py
+-rw-r--r--   0        0        0     2233 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/deployment/deployment.py
+-rw-r--r--   0        0        0     2174 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/entity/ad_hoc_entity.py
+-rw-r--r--   0        0        0     8301 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/entity/entity.py
+-rw-r--r--   0        0        0     1015 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/entity/field_value.py
+-rw-r--r--   0        0        0     1196 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/entity_location/entity_location.py
+-rw-r--r--   0        0        0     7065 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/entity_type/entity_type.py
+-rw-r--r--   0        0        0     2424 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/environment/environment.py
+-rw-r--r--   0        0        0      584 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/environment/environment_configuration.py
+-rw-r--r--   0        0        0     2193 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/environment/migration_plan.py
+-rw-r--r--   0        0        0      246 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/faas/custom_errors.py
+-rw-r--r--   0        0        0     2749 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/faas/faas_function.py
+-rw-r--r--   0        0        0     5635 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/faas/faas_utils.py
+-rw-r--r--   0        0        0     4437 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/file/file_reference.py
+-rw-r--r--   0        0        0     1184 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/function/function.py
+-rw-r--r--   0        0        0      248 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/internal/base_model.py
+-rw-r--r--   0        0        0     1221 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/internal/base_schema.py
+-rw-r--r--   0        0        0      637 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/internal/camel_case_schema.py
+-rw-r--r--   0        0        0     2717 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/internal/fields_mixin.py
+-rw-r--r--   0        0        0     2153 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/internal/lazy_property.py
+-rw-r--r--   0        0        0     2030 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/internal/lazy_property_list.py
+-rw-r--r--   0        0        0       80 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/internal/sort_direction.py
+-rw-r--r--   0        0        0        0 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/link_config/__init__.py
+-rw-r--r--   0        0        0      791 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/link_config/link_config.py
+-rw-r--r--   0        0        0      564 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/link_config/new_workbook_link.py
+-rw-r--r--   0        0        0      674 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/page_config/page_config.py
+-rw-r--r--   0        0        0      801 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/page_config/page_container.py
+-rw-r--r--   0        0        0      618 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/page_config/page_container_page_config.py
+-rw-r--r--   0        0        0     3229 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/prospective_task/ProspectiveTaskSummary.py
+-rw-r--r--   0        0        0      728 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/prospective_task/function_list.py
+-rw-r--r--   0        0        0      910 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/prospective_task/function_status.py
+-rw-r--r--   0        0        0     1287 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/prospective_task/io_group.py
+-rw-r--r--   0        0        0     2162 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/prospective_task/prospective_entity.py
+-rw-r--r--   0        0        0     1024 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/prospective_task/prospective_field_value.py
+-rw-r--r--   0        0        0    14272 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/prospective_task/prospective_task.py
+-rw-r--r--   0        0        0     3260 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/prospective_task/search.py
+-rw-r--r--   0        0        0      370 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/prospective_task_config/copy_forward_config.py
+-rw-r--r--   0        0        0     2471 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/prospective_task_config/field_config.py
+-rw-r--r--   0        0        0     1886 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/prospective_task_config/field_type.py
+-rw-r--r--   0        0        0      749 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/prospective_task_config/field_validation.py
+-rw-r--r--   0        0        0      639 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/prospective_task_config/from_pool_config.py
+-rw-r--r--   0        0        0     1914 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/prospective_task_config/group_config.py
+-rw-r--r--   0        0        0     1343 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/prospective_task_config/io_group_config.py
+-rw-r--r--   0        0        0     1561 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/prospective_task_config/pattern.py
+-rw-r--r--   0        0        0     4627 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/prospective_task_config/prospective_task_config.py
+-rw-r--r--   0        0        0     2568 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/queue/entity.py
+-rw-r--r--   0        0        0      874 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/queue/field_value.py
+-rw-r--r--   0        0        0     1023 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/queue/queue.py
+-rw-r--r--   0        0        0      416 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/shared_schemas/field_restriction.py
+-rw-r--r--   0        0        0      549 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/shared_schemas/field_search_request.py
+-rw-r--r--   0        0        0      534 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/shared_schemas/iri_list_schema.py
+-rw-r--r--   0        0        0      648 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/shared_schemas/sort_order.py
+-rw-r--r--   0        0        0     1585 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/task/ad_hoc_task.py
+-rw-r--r--   0        0        0     6115 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/task/task.py
+-rw-r--r--   0        0        0      834 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/tenant_config/tenant_config.py
+-rw-r--r--   0        0        0      562 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/workflow/config_mapping.py
+-rw-r--r--   0        0        0     1948 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/platform/workflow/workflow.py
+-rw-r--r--   0        0        0        0 2024-04-02 22:19:02.700388 s4_platform_api-1.3.0/s4/py.typed
+-rw-r--r--   0        0        0      920 1970-01-01 00:00:00.000000 s4_platform_api-1.3.0/PKG-INFO
```

### Comparing `s4_platform_api-1.2.0/LICENSE` & `s4_platform_api-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.2.0/pyproject.toml` & `s4_platform_api-1.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [tool.poetry]
 name = "s4-platform-api"
 # version dynamically populated by CI for releases
-version = "1.2.0"
+version = "1.3.0"
 description = "A general purpose library for interacting with the Semaphore Platform API"
 authors = ["Semaphore Solutions <info@semaphoresolutions.ca>"]
 readme = "README.md"
 packages = [{include = "s4"}]
 license = "MIT"
+exclude = ["README.internal.md"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 python-dotenv = "^0.19.2"
 requests = "^2.31.0"
 marshmallow = "^3.15.0"
 marshmallow-enum = "^1.5.1"
@@ -18,11 +19,12 @@
 ddtrace = "^1.17.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1.0"
 pytest-mock = "^3.7.0"
 mypy = "0.971"
 pip-licenses = "4.0.0"
+deepdiff = "^6.7.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `s4_platform_api-1.2.0/s4/platform/api.py` & `s4_platform_api-1.3.0/s4/platform/api.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.2.0/s4/platform/authentication_utils.py` & `s4_platform_api-1.3.0/s4/platform/authentication_utils.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.2.0/s4/platform/changeset/changeset.py` & `s4_platform_api-1.3.0/s4/platform/changeset/changeset.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,16 @@
         function_listener_iris: Optional[list[str]] = None,
         function_iris: Optional[list[str]] = None,
         configuration: Optional[ChangesetConfig] = None,
         attributed_to: Optional[str] = None,
         generated_at: Optional[datetime] = None,
         label: Optional[str] = None,
         links: Optional[list[str]] = None,
-        configs: Optional[list[str]] = None
+        configs: Optional[list[str]] = None,
+        sequences: Optional[list[str]] = None
 
     ):
         super().__init__(connection)
         self.iri = iri
         self.was_derived_from_iri = was_derived_from_iri
         self.type_iris = type_iris
         self.type_info_iris = type_info_iris
@@ -54,14 +55,15 @@
         self.function_iris = function_iris
         self.configuration = configuration
         self.attributed_to = attributed_to
         self.generated_at = generated_at
         self.label = label
         self.links = links
         self.configs = configs
+        self.sequences = sequences
 
 
 class ChangesetSchema(ConnectedModelSchema):
     class Meta:
         unknown = EXCLUDE
 
     def __init__(self, **kwargs):
@@ -94,7 +96,8 @@
     )
     configuration_blob = fields.Str(dump_only=True, required=False)
     attributed_to = fields.Str(load_only=True)
     generated_at = fields.DateTime(load_only=True)
     label = fields.Str(allow_none=True)
     links = fields.List(fields.Str(), allow_none=True)
     configs = fields.List(fields.Str(), allow_none=True)
+    sequences = fields.List(fields.Str(), allow_none=True)
```

### Comparing `s4_platform_api-1.2.0/s4/platform/changeset/changeset_config.py` & `s4_platform_api-1.3.0/s4/platform/changeset/changeset_config.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.2.0/s4/platform/changeset/deploy_changeset.py` & `s4_platform_api-1.3.0/s4/platform/changeset/deploy_changeset.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.2.0/s4/platform/claim/claim.py` & `s4_platform_api-1.3.0/s4/platform/claim/claim.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.2.0/s4/platform/connection.py` & `s4_platform_api-1.3.0/s4/platform/connection.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.2.0/s4/platform/constants.py` & `s4_platform_api-1.3.0/s4/platform/constants.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.2.0/s4/platform/deployment/deployment.py` & `s4_platform_api-1.3.0/s4/platform/deployment/deployment.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.2.0/s4/platform/entity/ad_hoc_entity.py` & `s4_platform_api-1.3.0/s4/platform/entity/ad_hoc_entity.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.2.0/s4/platform/entity/entity.py` & `s4_platform_api-1.3.0/s4/platform/entity/entity.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,25 +28,27 @@
         derived_from_entity_iris: list[str],
         entity_derivations: dict[str, list[str]],
         type_: str,
         invalidated_by: str,
         created_at_time: datetime,
         generated_by_task_iri: str,
         label_field_name: str,
+        changeset_iri: Optional[str] = None
     ):
         super().__init__(connection)
         self.iri = iri
         self.fields = fields
         self.derived_from_entity_iris = derived_from_entity_iris
         self.entity_derivations = entity_derivations
         self.type = type_
         self.invalidated_by = invalidated_by
         self.label_field_name = label_field_name
         self.created_at_time = created_at_time
         self.generated_by_task_iri = generated_by_task_iri
+        self.changeset_iri = changeset_iri
 
     @property
     def label(self) -> str:
         if self.label_field_name not in self.fields:
             raise RuntimeError(f"Entity has label_field_name {self.label_field_name} but that field is missing")
         return self.fields[self.label_field_name].value
 
@@ -201,14 +203,15 @@
         values=marshmallow_fields.List(marshmallow_fields.Str),
     )
     type = marshmallow_fields.Str(required=True)
     invalidated_by = marshmallow_fields.Str(allow_none=True)
     created_at_time = marshmallow_fields.DateTime()
     generated_by_task_iri = marshmallow_fields.Str(allow_none=True)
     label_field_name = marshmallow_fields.Str(required=True)
+    changeset_iri = marshmallow_fields.Str(allow_none=True, required=False)
 
 
 class EntityBatchSchema(ConnectedModelSchema):
     def __init__(self, **kwargs):
         super().__init__(list[Entity], **kwargs)
 
     entities = marshmallow_fields.List(marshmallow_fields.Nested(EntitySchema))
```

### Comparing `s4_platform_api-1.2.0/s4/platform/entity/field_value.py` & `s4_platform_api-1.3.0/s4/platform/entity/field_value.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,23 +7,26 @@
 
 class FieldValue(BaseFieldValue):
     def __init__(
         self,
         *,
         value: Optional[str],
         data_type: str,
-        validation_errors: Optional[list[str]] = None
+        validation_errors: Optional[list[str]] = None,
+        overridden: Optional[bool] = False
     ) -> None:
         self.value = value
         self.data_type = data_type
         # TODO: PF-1646
         #  There doesn't seem to be an obvious link for the validation_errors property
         self.validation_errors = validation_errors
+        self.overridden = overridden
 
 
 class FieldValueSchema(BaseSchema):
     def __init__(self, **kwargs):
         super().__init__(FieldValue, **kwargs)
 
     value = fields.Str(allow_none=True)
     data_type = fields.Str(required=True)
     validation_errors = fields.List(fields.Str(), allow_none=True)
+    overridden = fields.Bool(required=False, allow_none=True)
```

### Comparing `s4_platform_api-1.2.0/s4/platform/entity_location/entity_location.py` & `s4_platform_api-1.3.0/s4/platform/entity_location/entity_location.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.2.0/s4/platform/entity_type/entity_type.py` & `s4_platform_api-1.3.0/s4/platform/entity_type/entity_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,34 +114,37 @@
     def __init__(
         self,
         *,
         label: str,
         fields: dict[str, FieldValue],
         iri_local_name: Optional[str] = None,
         parent_type_iris: list[str] = [],
-        use_entity_type_infos: Optional[bool] = False
+        use_entity_type_infos: Optional[bool] = False,
+        direct_parent_type_iris: Optional[list[str]] = None,
     ):
         self.iri_local_name = iri_local_name
         self.label = label
         self.parent_type_iris = parent_type_iris
         self.fields = fields
-        self.use_entity_type_infos = use_entity_type_infos
+        self.use_entity_type_infos = use_entity_type_infos,
+        self.direct_parent_type_iris = direct_parent_type_iris
 
 
 class EntityTypeCreateRequestSchema(BaseSchema):
     def __init__(self, **kwargs):
         super().__init__(EntityTypeCreateRequest, **kwargs)
 
     iri_local_name = marshmallow_fields.Str()
     label = marshmallow_fields.Str()
     fields = marshmallow_fields.Dict(
         keys=marshmallow_fields.Str, values=marshmallow_fields.Nested(FieldValueSchema)
     )
     parent_type_iris = marshmallow_fields.List(marshmallow_fields.Str())
     use_entity_type_infos = marshmallow_fields.Bool()
+    direct_parent_type_iris= marshmallow_fields.List(marshmallow_fields.Str(), allow_none=True, required=False)
 
 
 class EntityTypeRequestSchema(BaseSchema):
     def __init__(self, **kwargs):
         super().__init__(EntityType, **kwargs)
 
     iri = marshmallow_fields.Str()
```

### Comparing `s4_platform_api-1.2.0/s4/platform/environment/environment.py` & `s4_platform_api-1.3.0/s4/platform/environment/environment.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,14 +22,16 @@
     def __init__(
         self,
         *,
         connection: Connection = None,
         iri: Optional[str],
         short_name: str,
         label: str,
+        # @deprecated. This parameter will always be None in objects returned from the Labbit backend and will
+        # be ignored by endpoints that expect objects of this type as a payload
         was_generated_by: Optional[str] = None,
         current_changeset_iri: Optional[str] = None,
         configuration: Optional[EnvironmentConfiguration] = None,
     ):
         super().__init__(connection)
         self.iri = iri
         self.short_name = short_name
```

### Comparing `s4_platform_api-1.2.0/s4/platform/environment/environment_configuration.py` & `s4_platform_api-1.3.0/s4/platform/environment/environment_configuration.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.2.0/s4/platform/environment/migration_plan.py` & `s4_platform_api-1.3.0/s4/platform/environment/migration_plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 class MigrationAction(Enum):
     DoNothing = "DoNothing"
     SwapChangeset = "SwapChangeset"
     Move = "Move"
     Upgrade = "Upgrade"
     Revise = "Revise"
+    Remove = "Remove"
 
 
 class ExecutionLocation(object):
     def __init__(
         self,
         activity_id: str,
         root_process_definition_key: str,
```

### Comparing `s4_platform_api-1.2.0/s4/platform/faas/faas_function.py` & `s4_platform_api-1.3.0/s4/platform/faas/faas_function.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.2.0/s4/platform/faas/faas_utils.py` & `s4_platform_api-1.3.0/s4/platform/faas/faas_utils.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.2.0/s4/platform/file/file_reference.py` & `s4_platform_api-1.3.0/s4/platform/file/file_reference.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.2.0/s4/platform/function/function.py` & `s4_platform_api-1.3.0/s4/platform/function/function.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.2.0/s4/platform/internal/base_schema.py` & `s4_platform_api-1.3.0/s4/platform/internal/base_schema.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.2.0/s4/platform/internal/camel_case_schema.py` & `s4_platform_api-1.3.0/s4/platform/internal/camel_case_schema.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.2.0/s4/platform/internal/fields_mixin.py` & `s4_platform_api-1.3.0/s4/platform/internal/fields_mixin.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.2.0/s4/platform/internal/lazy_property.py` & `s4_platform_api-1.3.0/s4/platform/internal/lazy_property.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.2.0/s4/platform/internal/lazy_property_list.py` & `s4_platform_api-1.3.0/s4/platform/internal/lazy_property_list.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.2.0/s4/platform/link_config/link_config.py` & `s4_platform_api-1.3.0/s4/platform/link_config/link_config.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.2.0/s4/platform/link_config/new_workbook_link.py` & `s4_platform_api-1.3.0/s4/platform/link_config/new_workbook_link.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.2.0/s4/platform/page_config/page_config.py` & `s4_platform_api-1.3.0/s4/platform/page_config/page_config.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.2.0/s4/platform/page_config/page_container.py` & `s4_platform_api-1.3.0/s4/platform/page_config/page_container.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.2.0/s4/platform/page_config/page_container_page_config.py` & `s4_platform_api-1.3.0/s4/platform/page_config/page_container_page_config.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.2.0/s4/platform/prospective_task/ProspectiveTaskSummary.py` & `s4_platform_api-1.3.0/s4/platform/prospective_task/ProspectiveTaskSummary.py`

 * *Files 15% similar despite different names*

```diff
@@ -23,15 +23,18 @@
         started_at_time: Optional[datetime] = None,
         fields: Optional[dict[str, ProspectiveFieldValue]] = None,
         last_changed_at_time: Optional[datetime] = None,
         was_committed_by: Optional[str] = None,
         was_last_changed_by: Optional[str] = None,
         review_requested: Optional[bool] = None,
         num_continuing_outputs: Optional[int] = None,
-        was_started_by: Optional[str] = None
+        was_started_by: Optional[str] = None,
+        workflow_iri: str,
+        workflow_name: Optional[str] = None,
+        environment: Optional[str] = None
     ):
         self.id_ = id_
         self.claim_iri = claim_iri
         self.activity_id = activity_id
         self.activity_name = activity_name
         self.created_at_time = created_at_time
         self.completed_at_time = completed_at_time
@@ -39,14 +42,17 @@
         self.fields = fields
         self.last_changed_at_time = last_changed_at_time
         self.was_committed_by = was_committed_by
         self.was_last_changed_by = was_last_changed_by
         self.review_requested = review_requested
         self.num_continuing_outputs = num_continuing_outputs
         self.was_started_by = was_started_by
+        self.workflow_iri = workflow_iri
+        self.workflow_name = workflow_name
+        self.environment = environment
 
 
 class ProspectiveTaskSummarySchema(BaseSchema):
     def __init__(self, **kwargs):
         super().__init__(ProspectiveTaskSummary, **kwargs)
 
     id_ = marshmallow_fields.Str(required=True, data_key="id")
@@ -62,7 +68,10 @@
     started_at_time = marshmallow_fields.DateTime()
     last_changed_at_time = marshmallow_fields.DateTime(allow_none=True)
     was_committed_by = marshmallow_fields.Str(allow_none=True)
     was_last_changed_by = marshmallow_fields.Str(allow_none=True, load_only=True)
     review_requested = marshmallow_fields.Bool(allow_none=True, load_only=True)
     num_continuing_outputs = marshmallow_fields.Int(allow_none=True, load_only=True)
     was_started_by = marshmallow_fields.Str(allow_none=True, load_only=True)
+    workflow_iri = marshmallow_fields.Str(load_only=True)
+    workflow_name = marshmallow_fields.Str(allow_none=True, load_only=True)
+    environment = marshmallow_fields.Str(allow_none=True, load_only=True)
```

### Comparing `s4_platform_api-1.2.0/s4/platform/prospective_task/function_list.py` & `s4_platform_api-1.3.0/s4/platform/prospective_task/function_list.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.2.0/s4/platform/prospective_task/function_status.py` & `s4_platform_api-1.3.0/s4/platform/prospective_task/function_status.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.2.0/s4/platform/prospective_task/io_group.py` & `s4_platform_api-1.3.0/s4/platform/prospective_task/io_group.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.2.0/s4/platform/prospective_task/prospective_entity.py` & `s4_platform_api-1.3.0/s4/platform/prospective_task/prospective_entity.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.2.0/s4/platform/prospective_task/prospective_field_value.py` & `s4_platform_api-1.3.0/s4/platform/prospective_task/prospective_field_value.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.2.0/s4/platform/prospective_task/prospective_task.py` & `s4_platform_api-1.3.0/s4/platform/prospective_task/prospective_task.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,16 @@
         was_last_changed_by: Optional[str] = None,
         review_state: ReviewState = ReviewState.NONE,
         running_function: Optional[FunctionStatus] = None,
         was_reverted_at_time: Optional[datetime] = None,
         was_reverted_by_user: Optional[str] = None,
         was_started_by: Optional[str] = None,
         workflow_name: Optional[str] = None,
-        ui_state: Optional[str] = None
+        ui_state: Optional[str] = None,
+        num_continuing_outputs: Optional[int] = None,
     ):
         super().__init__(connection)
 
         self.id_ = id_
         self.claim_iri = claim_iri
         self.task_iri = task_iri
         self.workflow_iri = workflow_iri
@@ -94,14 +95,15 @@
         self.review_state = review_state
         self.running_function = running_function
         self.was_reverted_at_time = was_reverted_at_time
         self.was_reverted_by_user = was_reverted_by_user
         self.was_started_by = was_started_by
         self.workflow_name = workflow_name
         self.ui_state = ui_state
+        self.num_continuing_outputs = num_continuing_outputs
 
     def claim(self) -> ProspectiveTask:
         json = self.connection.post_json(f"prospectiveTask/{self.id_}/claim", None)
         self._update_with_json(json)
         return self
 
     def commit(self) -> ProspectiveTask:
@@ -331,14 +333,15 @@
         FunctionStatusSchema, allow_none=True, load_only=True
     )
     was_reverted_at_time = marshmallow_fields.DateTime(allow_none=True, load_only=True)
     was_reverted_by_user = marshmallow_fields.Str(allow_none=True, load_only=True)
     was_started_by = marshmallow_fields.Str(allow_none=True)
     workflow_name = marshmallow_fields.Str(allow_none=True)
     ui_state = marshmallow_fields.Str(allow_none=True)
+    num_continuing_outputs = marshmallow_fields.Integer(allow_none=True)
 
 
 class CreateProspectiveTaskSchema(CamelCaseSchema):
     workflow_iri = marshmallow_fields.Str(dump_only=True)
     changeset_iri = marshmallow_fields.Str(dump_only=True)
     activity_id = marshmallow_fields.Str(dump_only=True)
     input_entities = marshmallow_fields.List(marshmallow_fields.Str(), dump_only=True)
```

### Comparing `s4_platform_api-1.2.0/s4/platform/prospective_task/search.py` & `s4_platform_api-1.3.0/s4/platform/prospective_task/search.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,28 +17,47 @@
 
 class SortDescriptor:
     def __init__(self, field: str, direction: SortDirection):
         self.field = field
         self.direction = direction
 
 
+class FilterDescriptor:
+    def __init__(self, users: Optional[list[str]] = None, activity_names: Optional[list[str]] = None,
+                 workflow_names: Optional[list[str]] = None):
+        self.users = users
+        self.activity_names = activity_names
+        self.workflow_names = workflow_names
+
+
+class FilterDescriptorSchema(BaseSchema):
+    def __init__(self, **kwargs):
+        super().__init__(FilterDescriptor, **kwargs)
+
+    users = fields.List(fields.Str(), dump_only=True, required=False)
+    activity_names = fields.List(fields.Str(), dump_only=True, required=False)
+    workflow_names = fields.List(fields.Str(), dump_only=True, required=False)
+
+
 class ProspectiveTaskSearchRequest:
     def __init__(
         self,
         search_term: str,
         offset: Optional[int],
         limit: Optional[int],
         sort_descriptors: Optional[list[SortDescriptor]],
         include_output_entities: Optional[bool],
+        filter_descriptor: Optional[FilterDescriptor] = None
     ):
         self.search_term = search_term
         self.offset = offset
         self.limit = limit
         self.sort_descriptors = sort_descriptors
         self.include_output_entities = include_output_entities
+        self.filter_descriptor = filter_descriptor
 
 
 class ProspectiveTaskSummaryPage:
     def __init__(
         self,
         offset: int,
         total_count: int,
@@ -64,14 +83,15 @@
     search_term = fields.Str()
     offset = fields.Integer(dump_only=True, allow_none=True)
     limit = fields.Integer(dump_only=True, allow_none=True)
     sort_descriptors = fields.List(
         fields.Nested(SortDescriptorSchema), dump_only=True, allow_none=True
     )
     include_output_entities = fields.Bool(dump_only=True, allow_none=True)
+    filter_descriptor = fields.Nested(FilterDescriptorSchema, dump_only=True, allow_none=True)
 
 
 class ProspectiveTaskSummaryPageSchema(BaseSchema):
     def __init__(self, **kwargs):
         super().__init__(ProspectiveTaskSummaryPage, **kwargs)
 
     offset = fields.Integer(load_only=True)
```

### Comparing `s4_platform_api-1.2.0/s4/platform/prospective_task_config/field_config.py` & `s4_platform_api-1.3.0/s4/platform/prospective_task_config/field_config.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.2.0/s4/platform/prospective_task_config/field_type.py` & `s4_platform_api-1.3.0/s4/platform/prospective_task_config/field_type.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,14 +12,23 @@
     DATE = "http://www.w3.org/2001/XMLSchema#date"
     DATE_TIME = "http://www.w3.org/2001/XMLSchema#datetime"
     MARKDOWN = "http://www.semaphoresolutions.com/schema/2020/platform#text/markdown"
     FILE_REFERENCE = (
         "http://www.semaphoresolutions.com/schema/2020/platform#FileReference"
     )
     IRI = "http://www.w3.org/2001/XMLSchema#anyURI"
+    TYPE_REFERENCE = (
+        "http://www.semaphoresolutions.com/schema/2020/platform#TypeReference"
+    )
+    JSON = (
+        "http://www.semaphoresolutions.com/schema/2020/platform#text/json"
+    )
+    SEQUENCE_TYPE = (
+        "http://www.semaphoresolutions.com/schema/2020/platform#Sequence"
+    )
 
     @staticmethod
     def from_str(value: str) -> Optional["FieldType"]:
         for (name, member) in FieldType.__members__.items():
             if member.value == value:
                 return member
         return None
```

### Comparing `s4_platform_api-1.2.0/s4/platform/prospective_task_config/field_validation.py` & `s4_platform_api-1.3.0/s4/platform/prospective_task_config/field_validation.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.2.0/s4/platform/prospective_task_config/from_pool_config.py` & `s4_platform_api-1.3.0/s4/platform/prospective_task_config/from_pool_config.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.2.0/s4/platform/prospective_task_config/group_config.py` & `s4_platform_api-1.3.0/s4/platform/prospective_task_config/group_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List
+from typing import List, Optional
 
 from marshmallow import fields
 
 from s4.platform.internal.base_schema import BaseSchema
 from s4.platform.prospective_task_config.from_pool_config import (
     FromPoolConfig,
     FromPoolConfigSchema,
@@ -18,26 +18,28 @@
         entity_derivations: dict[str, List[str]] = None,
         count: int = None,
         min_count: int = None,
         max_count: int = None,
         invalidate: bool = None,
         from_reference: bool = False,
         for_each: List[str] = None,
-        from_pool: FromPoolConfig = None
+        from_pool: FromPoolConfig = None,
+        revise_stowaway_samples: Optional[bool] = None
     ):
         self.does_not_continue = does_not_continue
         self.derived_from = derived_from
         self.entity_derivations = entity_derivations
         self.count = count
         self.min_count = min_count
         self.max_count = max_count
         self.invalidate = invalidate
         self.from_reference = from_reference
         self.for_each = for_each
         self.from_pool = from_pool
+        self.revise_stowaway_samples = revise_stowaway_samples
 
 
 class GroupConfigSchema(BaseSchema):
     def __init__(self, **kwargs):
         super().__init__(GroupConfig, **kwargs)
 
     does_not_continue = fields.Bool()
@@ -46,7 +48,8 @@
     count = fields.Integer(allow_none=True)
     min_count = fields.Integer(allow_none=True)
     max_count = fields.Integer(allow_none=True)
     invalidate = fields.Bool(allow_none=True)
     from_reference = fields.Bool()
     for_each = fields.List(fields.Str, allow_none=True)
     from_pool = fields.Nested(FromPoolConfigSchema, allow_none=True)
+    revise_stowaway_samples = fields.Bool(allow_none=True)
```

### Comparing `s4_platform_api-1.2.0/s4/platform/prospective_task_config/io_group_config.py` & `s4_platform_api-1.3.0/s4/platform/prospective_task_config/io_group_config.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 from marshmallow import fields
 
-from typing import Dict, List
+from typing import Dict, List, Optional
 from s4.platform.internal.base_schema import BaseSchema
 from s4.platform.prospective_task_config.group_config import (
     GroupConfig,
     GroupConfigSchema,
 )
 
 
 class IoGroupConfig(object):
     def __init__(
-        self, *, inputs: Dict[str, GroupConfig], outputs: Dict[str, GroupConfig], manual: bool = False
+            self, *, inputs: Dict[str, GroupConfig], outputs: Dict[str, GroupConfig], manual: bool = False,
+            group_by: Optional[Dict[str, str]] = None
     ):
         self.inputs = inputs
         for key, inputConfig in self.inputs.items():
             if inputConfig.invalidate is None:
                 inputConfig.invalidate = True
         self.outputs = outputs
         for key, outputConfig in self.outputs.items():
             if outputConfig.invalidate is None:
                 outputConfig.invalidate = False
         self.manual = manual
+        self.group_by = group_by
 
 
 class IoGroupConfigSchema(BaseSchema):
     def __init__(self, **kwargs):
         super().__init__(IoGroupConfig, **kwargs)
 
     inputs = fields.Dict(
         keys=fields.Str, values=fields.Nested(GroupConfigSchema), required=True
     )
     outputs = fields.Dict(
         keys=fields.Str, values=fields.Nested(GroupConfigSchema), required=True
     )
     manual = fields.Bool(allow_none=True)
+    group_by = fields.Dict(keys=fields.Str, values=fields.Str, allow_none=True)
```

### Comparing `s4_platform_api-1.2.0/s4/platform/prospective_task_config/pattern.py` & `s4_platform_api-1.3.0/s4/platform/prospective_task_config/pattern.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 from marshmallow import fields as marshmallow_fields
 
-from typing import Dict
+from typing import Optional, Dict, List
 from s4.platform.internal.base_schema import BaseSchema
+from s4.platform.prospective_task_config.copy_forward_config import CopyForwardConfig, CopyForwardConfigSchema
 from s4.platform.prospective_task_config.field_config import (
     FieldConfig,
     FieldConfigSchema,
 )
 
 
 class Pattern(object):
     def __init__(
         self,
         *,
-        entity_type: str,
+        entity_type: Optional[str] = None,
         fields: Dict[str, FieldConfig],
-        label_field_name: str,
+        label_field_name: Optional[str] = None,
         is_outside_entity: bool = False,
-        can_be_subtype: bool = False
+        can_be_subtype: bool = False,
+        copy_fields_from: Optional[List[CopyForwardConfig]] = None
     ):
         self.entity_type = entity_type
         self.fields = fields
         self.is_outside_entity = is_outside_entity
         self.can_be_subtype = can_be_subtype
         self.label_field_name = label_field_name
+        self.copy_fields_from = copy_fields_from
 
 
 class PatternSchema(BaseSchema):
     def __init__(self, **kwargs):
         super().__init__(Pattern, **kwargs)
 
-    entity_type = marshmallow_fields.Str()
+    entity_type = marshmallow_fields.Str(allow_none=True)
     fields = marshmallow_fields.Dict(
         keys=marshmallow_fields.Str, values=marshmallow_fields.Nested(FieldConfigSchema)
     )
     is_outside_entity = marshmallow_fields.Bool()
     can_be_subtype = marshmallow_fields.Bool()
-    label_field_name = marshmallow_fields.Str()
+    label_field_name = marshmallow_fields.Str(allow_none=True)
+    copy_fields_from = marshmallow_fields.List(marshmallow_fields.Nested(CopyForwardConfigSchema), allow_none=True)
```

### Comparing `s4_platform_api-1.2.0/s4/platform/prospective_task_config/prospective_task_config.py` & `s4_platform_api-1.3.0/s4/platform/prospective_task_config/prospective_task_config.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.2.0/s4/platform/queue/entity.py` & `s4_platform_api-1.3.0/s4/platform/queue/entity.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,25 +17,27 @@
         fields: dict[str, FieldValue],
         derived_from_entity_iris: list[str],
         entity_derivations: dict[str, list[str]],
         type_: str,
         invalidated_by: str,
         created_at_time: datetime,
         label_field_name: str,
-        generated_by_task_iri: Optional[str] = None
+        generated_by_task_iri: Optional[str] = None,
+        changeset_iri: Optional[str] = None
     ):
         super().__init__(iri)
         self.fields = fields
         self.derived_from_entity_iris = derived_from_entity_iris
         self.entity_derivations = entity_derivations
         self.type_ = type_
         self.invalidated_by = invalidated_by
         self.created_at_time = created_at_time
         self.generated_by_task_iri = generated_by_task_iri
         self.label_field_name = label_field_name
+        self.changeset_iri = changeset_iri
 
 
 class QueuedEntity(object):
     def __init__(self, *, entity: Entity, queued_at_time: Optional[datetime]):
         self.entity = entity
         self.queued_at_time = queued_at_time
 
@@ -54,14 +56,15 @@
         values=marshmallow_fields.List(marshmallow_fields.Str),
     )
     type_ = marshmallow_fields.Str(data_key="type")
     invalidated_by = marshmallow_fields.Str(allow_none=True)
     created_at_time = marshmallow_fields.DateTime()
     generated_by_task_iri = marshmallow_fields.Str(allow_none=True, required=False)
     label_field_name = marshmallow_fields.Str()
+    changeset_iri = marshmallow_fields.Str(allow_none=True, required=False)
 
 
 class QueuedEntitySchema(BaseSchema):
     def __init__(self, **kwargs):
         super().__init__(QueuedEntity, **kwargs)
 
     entity = marshmallow_fields.Nested(EntitySchema)
```

### Comparing `s4_platform_api-1.2.0/s4/platform/queue/field_value.py` & `s4_platform_api-1.3.0/s4/platform/queue/field_value.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,18 +2,24 @@
 
 from marshmallow import fields
 from s4.platform.internal.base_schema import BaseSchema
 from s4.platform.internal.fields_mixin import BaseFieldValue
 
 
 class FieldValue(BaseFieldValue):
-    def __init__(self, *, value: Optional[str], data_type: str):
+    def __init__(self, *, value: Optional[str], data_type: str,
+                 validation_errors: Optional[list[str]] = None,
+                 overridden: Optional[bool] = False):
         self.value = value
         self.data_type = data_type
+        self.validation_errors = validation_errors
+        self.overridden = overridden
 
 
 class FieldValueSchema(BaseSchema):
     def __init__(self, **kwargs):
         super().__init__(FieldValue, **kwargs)
 
     value = fields.Str(required=True)
     data_type = fields.Str(required=True)
+    validation_errors = fields.List(fields.Str(), allow_none=True)
+    overridden = fields.Bool(required=False, allow_none=True)
```

### Comparing `s4_platform_api-1.2.0/s4/platform/queue/queue.py` & `s4_platform_api-1.3.0/s4/platform/queue/queue.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,10 +17,13 @@
         super().__init__(Queue, **kwargs)
 
     queued_entities = fields.List(fields.Nested(QueuedEntitySchema))
 
 
 class QueuedEntitiesRequestSchema(CamelCaseSchema):
     workflow_iri = fields.Str(dump_only=True)
+    # @deprecated Removed from the API endpoint 2022-04-26 in changeset 77090abd4b5f76553a6f98d068bf2b3a83c93f7f
+    # Values will be ignored by backend
     changeset_iri = fields.Str(dump_only=True)
     activity_id = fields.Str(dump_only=True)
     entity_iris = fields.List(fields.Str, dump_only=True)
+    workflow_id = fields.Str(allow_none=True)
```

### Comparing `s4_platform_api-1.2.0/s4/platform/shared_schemas/field_search_request.py` & `s4_platform_api-1.3.0/s4/platform/shared_schemas/field_search_request.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.2.0/s4/platform/shared_schemas/iri_list_schema.py` & `s4_platform_api-1.3.0/s4/platform/shared_schemas/iri_list_schema.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.2.0/s4/platform/shared_schemas/sort_order.py` & `s4_platform_api-1.3.0/s4/platform/shared_schemas/sort_order.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.2.0/s4/platform/task/ad_hoc_task.py` & `s4_platform_api-1.3.0/s4/platform/task/ad_hoc_task.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,26 +4,30 @@
 
 from s4.platform.entity.ad_hoc_entity import AdHocEntity, AdHocEntitySchema
 from s4.platform.entity.field_value import FieldValue, FieldValueSchema
 from s4.platform.internal.base_schema import BaseSchema
 
 
 class AdHocTask(object):
-    def __init__(self, *, fields: dict[str, FieldValue], used_entity_iris: list[str], invalidated_entity_iris: list[str],
-                 generated_entities: list[AdHocEntity], claim_iri: Optional[str] = None):
+    def __init__(self, *, fields: dict[str, FieldValue], used_entity_iris: list[str],
+                 invalidated_entity_iris: list[str],
+                 generated_entities: list[AdHocEntity], claim_iri: Optional[str] = None,
+                 execution_details_blob: Optional[str] = None):
         self.fields = fields
         self.used_entity_iris = used_entity_iris
         self.invalidated_entity_iris = invalidated_entity_iris
         self.generated_entities = generated_entities
         self.claim_iri = claim_iri
+        self.execution_details_blob = execution_details_blob
 
 
 class AdHocTaskSchema(BaseSchema):
     def __init__(self, **kwargs):
         super().__init__(AdHocTask, **kwargs)
 
     fields = marshmallow_fields.Dict(keys=marshmallow_fields.Str,
                                      values=marshmallow_fields.Nested(FieldValueSchema))
     used_entity_iris = marshmallow_fields.List(marshmallow_fields.Str, dump_only=True)
     invalidated_entity_iris = marshmallow_fields.List(marshmallow_fields.Str, dump_only=True)
     generated_entities = marshmallow_fields.List(marshmallow_fields.Nested(AdHocEntitySchema))
     claim_iri = marshmallow_fields.Str(dump_only=True)
+    execution_details_blob = marshmallow_fields.Str(allow_none=True, dump_only=True)
```

### Comparing `s4_platform_api-1.2.0/s4/platform/tenant_config/tenant_config.py` & `s4_platform_api-1.3.0/s4/platform/tenant_config/tenant_config.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.2.0/s4/platform/workflow/config_mapping.py` & `s4_platform_api-1.3.0/s4/platform/workflow/config_mapping.py`

 * *Files identical despite different names*

### Comparing `s4_platform_api-1.2.0/s4/platform/workflow/workflow.py` & `s4_platform_api-1.3.0/s4/platform/workflow/workflow.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,24 +15,26 @@
         config_mappings: list[ConfigMapping],
         workflow_execution_trigger_iris: Optional[list[str]],
         was_derived_from: Optional[str],
         can_start_without_inputs: Optional[bool],
         can_start_with_inputs: Optional[bool] = None,
         start_permission: Optional[str] = None,
         startable_by_public: Optional[bool] = False,
+        name: Optional[str] = None
     ):
         self.iri = iri
         self.process_definition_iri = process_definition_iri
         self.workflow_execution_trigger_iris = workflow_execution_trigger_iris
         self.was_derived_from = was_derived_from
         self.config_mappings = config_mappings
         self.can_start_without_inputs = can_start_without_inputs
         self.can_start_with_inputs = can_start_with_inputs
         self.start_permission = start_permission
         self.startable_by_public = startable_by_public
+        self.name = name
 
 
 class WorkflowSchema(BaseSchema):
     def __init__(self, **kwargs):
         super().__init__(Workflow, **kwargs)
 
     iri = fields.Str(allow_none=True, load_only=True)
@@ -40,7 +42,8 @@
     workflow_execution_trigger_iris = fields.List(fields.Str(), allow_none=True)
     was_derived_from = fields.Str(allow_none=True)
     can_start_without_inputs = fields.Boolean(allow_none=True)
     can_start_with_inputs = fields.Boolean(allow_none=True)
     config_mappings = fields.List(fields.Nested(ConfigMappingSchema))
     start_permission = fields.Str(allow_none=True, required=False)
     startable_by_public = fields.Bool(allow_none=True)
+    name = fields.Str(allow_none=True, required=False)
```

