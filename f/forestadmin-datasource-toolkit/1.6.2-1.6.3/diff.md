# Comparing `tmp/forestadmin_datasource_toolkit-1.6.2.tar.gz` & `tmp/forestadmin_datasource_toolkit-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forestadmin_datasource_toolkit-1.6.2.tar", max compression
+gzip compressed data, was "forestadmin_datasource_toolkit-1.6.3.tar", max compression
```

## Comparing `forestadmin_datasource_toolkit-1.6.2.tar` & `forestadmin_datasource_toolkit-1.6.3.tar`

### file list

```diff
@@ -1,147 +1,147 @@
--rw-r--r--   0        0        0        0 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/README.md
--rw-r--r--   0        0        0        0 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/__init__.py
--rw-r--r--   0        0        0     3538 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/collections.py
--rw-r--r--   0        0        0        0 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/context/__init__.py
--rw-r--r--   0        0        0      678 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/context/agent_context.py
--rw-r--r--   0        0        0      658 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/context/collection_context.py
--rw-r--r--   0        0        0        0 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/context/relaxed_wrappers/__init__.py
--rw-r--r--   0        0        0     7240 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/context/relaxed_wrappers/collection.py
--rw-r--r--   0        0        0    29444 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/datasource_customizer/collection_customizer.py
--rw-r--r--   0        0        0     5404 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/datasource_customizer/datasource_customizer.py
--rw-r--r--   0        0        0      279 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/datasource_customizer/types.py
--rw-r--r--   0        0        0     1658 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/datasources.py
--rw-r--r--   0        0        0        0 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/__init__.py
--rw-r--r--   0        0        0        0 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/action/__init__.py
--rw-r--r--   0        0        0     5983 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/action/collections.py
--rw-r--r--   0        0        0        0 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/action/context/__init__.py
--rw-r--r--   0        0        0     2276 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/action/context/base.py
--rw-r--r--   0        0        0      591 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/action/context/bulk.py
--rw-r--r--   0        0        0      974 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/action/context/single.py
--rw-r--r--   0        0        0     4677 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/action/result_builder.py
--rw-r--r--   0        0        0        0 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/action/types/__init__.py
--rw-r--r--   0        0        0     1360 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/action/types/actions.py
--rw-r--r--   0        0        0    22709 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/action/types/fields.py
--rw-r--r--   0        0        0     6215 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/action/types/widgets.py
--rw-r--r--   0        0        0        0 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/binary/__init__.py
--rw-r--r--   0        0        0     9653 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/binary/collection.py
--rw-r--r--   0        0        0      295 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/binary/utils.py
--rw-r--r--   0        0        0        0 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/chart/__init__.py
--rw-r--r--   0        0        0     2216 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/chart/chart_collection_decorator.py
--rw-r--r--   0        0        0     2362 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/chart/chart_datasource_decorator.py
--rw-r--r--   0        0        0     1567 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/chart/collection_chart_context.py
--rw-r--r--   0        0        0     7890 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/chart/result_builder.py
--rw-r--r--   0        0        0      728 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/chart/types.py
--rw-r--r--   0        0        0     5355 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/collection_decorator.py
--rw-r--r--   0        0        0        0 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/computed/__init__.py
--rw-r--r--   0        0        0     5310 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/computed/collections.py
--rw-r--r--   0        0        0      154 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/computed/exceptions.py
--rw-r--r--   0        0        0     3916 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/computed/helpers.py
--rw-r--r--   0        0        0      748 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/computed/types.py
--rw-r--r--   0        0        0     2812 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/computed/utils.py
--rw-r--r--   0        0        0     1666 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/datasource_decorator.py
--rw-r--r--   0        0        0     5079 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/decorator_stack.py
--rw-r--r--   0        0        0        0 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/empty/__init__.py
--rw-r--r--   0        0        0     4495 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/empty/collection.py
--rw-r--r--   0        0        0        0 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/hook/__init__.py
--rw-r--r--   0        0        0     4841 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/hook/collections.py
--rw-r--r--   0        0        0        0 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/hook/context/__init__.py
--rw-r--r--   0        0        0     1233 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/hook/context/aggregate.py
--rw-r--r--   0        0        0      870 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/hook/context/create.py
--rw-r--r--   0        0        0      599 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/hook/context/delete.py
--rw-r--r--   0        0        0      525 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/hook/context/hooks.py
--rw-r--r--   0        0        0     1153 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/hook/context/list.py
--rw-r--r--   0        0        0      777 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/hook/context/update.py
--rw-r--r--   0        0        0      852 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/hook/hooks.py
--rw-r--r--   0        0        0      392 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/hook/types.py
--rw-r--r--   0        0        0        0 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/operators_emulate/__init__.py
--rw-r--r--   0        0        0     6521 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/operators_emulate/collections.py
--rw-r--r--   0        0        0      371 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/operators_emulate/types.py
--rw-r--r--   0        0        0        0 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/operators_equivalence/__init__.py
--rw-r--r--   0        0        0     3855 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/operators_equivalence/collections.py
--rw-r--r--   0        0        0        0 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/publication/__init__.py
--rw-r--r--   0        0        0     3866 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/publication/collections.py
--rw-r--r--   0        0        0     2421 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/publication/datasource.py
--rw-r--r--   0        0        0        0 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/relation/__init__.py
--rw-r--r--   0        0        0    12558 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/relation/collections.py
--rw-r--r--   0        0        0     1125 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/relation/types.py
--rw-r--r--   0        0        0        0 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/rename_collection/__init__.py
--rw-r--r--   0        0        0     1041 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/rename_collection/collection.py
--rw-r--r--   0        0        0     2897 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/rename_collection/datasource.py
--rw-r--r--   0        0        0        0 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/rename_field/__init__.py
--rw-r--r--   0        0        0    10161 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/rename_field/collections.py
--rw-r--r--   0        0        0        0 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/schema/__init__.py
--rw-r--r--   0        0        0      671 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/schema/collection.py
--rw-r--r--   0        0        0        0 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/search/__init__.py
--rw-r--r--   0        0        0     6164 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/search/collections.py
--rw-r--r--   0        0        0        0 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/segments/__init__.py
--rw-r--r--   0        0        0     2627 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/segments/collections.py
--rw-r--r--   0        0        0        0 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/sort_emulate/__init__.py
--rw-r--r--   0        0        0     6009 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/sort_emulate/collections.py
--rw-r--r--   0        0        0        0 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/validation/__init__.py
--rw-r--r--   0        0        0     4019 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/validation/collection.py
--rw-r--r--   0        0        0        0 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/write/__init__.py
--rw-r--r--   0        0        0        0 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/write/create_relations/__init__.py
--rw-r--r--   0        0        0     4987 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/write/create_relations/create_relations_collection.py
--rw-r--r--   0        0        0        0 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/write/update_relations/__init__.py
--rw-r--r--   0        0        0     4845 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/write/update_relations/update_relations_collection.py
--rw-r--r--   0        0        0     1020 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/write/write_datasource_decorator.py
--rw-r--r--   0        0        0        0 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/write/write_replace/__init__.py
--rw-r--r--   0        0        0      420 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/write/write_replace/types.py
--rw-r--r--   0        0        0      932 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/write/write_replace/write_customization_context.py
--rw-r--r--   0        0        0     6436 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/write/write_replace/write_replace_collection.py
--rw-r--r--   0        0        0     2331 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/exceptions.py
--rw-r--r--   0        0        0     6148 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/.DS_Store
--rw-r--r--   0        0        0        0 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/__init__.py
--rw-r--r--   0        0        0     3551 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/actions.py
--rw-r--r--   0        0        0     1141 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/chart.py
--rw-r--r--   0        0        0     2463 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/collections.py
--rw-r--r--   0        0        0     5160 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/fields.py
--rw-r--r--   0        0        0        0 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/models/__init__.py
--rw-r--r--   0        0        0     1346 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/models/collections.py
--rw-r--r--   0        0        0     6148 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/.DS_Store
--rw-r--r--   0        0        0        0 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/__init__.py
--rw-r--r--   0        0        0     7998 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/aggregation.py
--rw-r--r--   0        0        0     6148 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/.DS_Store
--rw-r--r--   0        0        0        0 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/__init__.py
--rw-r--r--   0        0        0     4505 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/equivalence.py
--rw-r--r--   0        0        0     5340 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/factory.py
--rw-r--r--   0        0        0        0 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/__init__.py
--rw-r--r--   0        0        0     2696 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/base.py
--rw-r--r--   0        0        0     4844 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/branch.py
--rw-r--r--   0        0        0     9918 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/leaf.py
--rw-r--r--   0        0        0     1270 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/operators.py
--rw-r--r--   0        0        0        0 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/__init__.py
--rw-r--r--   0        0        0     3836 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/comparison.py
--rw-r--r--   0        0        0     1688 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/pattern.py
--rw-r--r--   0        0        0     7643 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/time.py
--rw-r--r--   0        0        0        0 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/filter/__init__.py
--rw-r--r--   0        0        0     8081 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/filter/factory.py
--rw-r--r--   0        0        0     2889 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/filter/paginated.py
--rw-r--r--   0        0        0     3110 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/filter/unpaginated.py
--rw-r--r--   0        0        0      759 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/page.py
--rw-r--r--   0        0        0     4442 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/projections/__init__.py
--rw-r--r--   0        0        0      902 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/projections/factory.py
--rw-r--r--   0        0        0     2455 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/sort/__init__.py
--rw-r--r--   0        0        0      595 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/sort/factory.py
--rw-r--r--   0        0        0      118 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/records.py
--rw-r--r--   0        0        0        0 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/plugins/__init__.py
--rw-r--r--   0        0        0     2514 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/plugins/add_external_relation.py
--rw-r--r--   0        0        0     4353 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/plugins/import_field.py
--rw-r--r--   0        0        0      395 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/plugins/plugin.py
--rw-r--r--   0        0        0       73 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/utils/__init__.py
--rw-r--r--   0        0        0     8601 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/utils/collections.py
--rw-r--r--   0        0        0     2559 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/utils/operators.py
--rw-r--r--   0        0        0     1169 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/utils/records.py
--rw-r--r--   0        0        0     1878 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/utils/schema.py
--rw-r--r--   0        0        0      449 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/utils/user_callable.py
--rw-r--r--   0        0        0        0 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/validations/__init__.py
--rw-r--r--   0        0        0     4790 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/validations/condition_tree.py
--rw-r--r--   0        0        0     4231 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/validations/field.py
--rw-r--r--   0        0        0      393 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/validations/projection.py
--rw-r--r--   0        0        0     1542 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/validations/records.py
--rw-r--r--   0        0        0     4573 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/validations/rules.py
--rw-r--r--   0        0        0      469 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/validations/sort.py
--rw-r--r--   0        0        0     4649 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/validations/type_getter.py
--rw-r--r--   0        0        0      372 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/validations/types.py
--rw-r--r--   0        0        0     1567 2024-04-02 07:31:36.310502 forestadmin_datasource_toolkit-1.6.2/pyproject.toml
--rw-r--r--   0        0        0      966 1970-01-01 00:00:00.000000 forestadmin_datasource_toolkit-1.6.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-03 08:04:21.672932 forestadmin_datasource_toolkit-1.6.3/README.md
+-rw-r--r--   0        0        0        0 2024-04-03 08:04:21.672932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/__init__.py
+-rw-r--r--   0        0        0     3538 2024-04-03 08:04:21.672932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/collections.py
+-rw-r--r--   0        0        0        0 2024-04-03 08:04:21.672932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/context/__init__.py
+-rw-r--r--   0        0        0      678 2024-04-03 08:04:21.672932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/context/agent_context.py
+-rw-r--r--   0        0        0      658 2024-04-03 08:04:21.672932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/context/collection_context.py
+-rw-r--r--   0        0        0        0 2024-04-03 08:04:21.672932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/context/relaxed_wrappers/__init__.py
+-rw-r--r--   0        0        0     7240 2024-04-03 08:04:21.672932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/context/relaxed_wrappers/collection.py
+-rw-r--r--   0        0        0    29444 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/datasource_customizer/collection_customizer.py
+-rw-r--r--   0        0        0     5404 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/datasource_customizer/datasource_customizer.py
+-rw-r--r--   0        0        0      279 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/datasource_customizer/types.py
+-rw-r--r--   0        0        0     1658 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/datasources.py
+-rw-r--r--   0        0        0        0 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/action/__init__.py
+-rw-r--r--   0        0        0     5983 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/action/collections.py
+-rw-r--r--   0        0        0        0 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/action/context/__init__.py
+-rw-r--r--   0        0        0     2276 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/action/context/base.py
+-rw-r--r--   0        0        0      591 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/action/context/bulk.py
+-rw-r--r--   0        0        0      974 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/action/context/single.py
+-rw-r--r--   0        0        0     4677 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/action/result_builder.py
+-rw-r--r--   0        0        0        0 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/action/types/__init__.py
+-rw-r--r--   0        0        0     1360 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/action/types/actions.py
+-rw-r--r--   0        0        0    22709 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/action/types/fields.py
+-rw-r--r--   0        0        0     6215 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/action/types/widgets.py
+-rw-r--r--   0        0        0        0 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/binary/__init__.py
+-rw-r--r--   0        0        0     9653 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/binary/collection.py
+-rw-r--r--   0        0        0      295 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/binary/utils.py
+-rw-r--r--   0        0        0        0 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/chart/__init__.py
+-rw-r--r--   0        0        0     2216 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/chart/chart_collection_decorator.py
+-rw-r--r--   0        0        0     2362 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/chart/chart_datasource_decorator.py
+-rw-r--r--   0        0        0     1567 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/chart/collection_chart_context.py
+-rw-r--r--   0        0        0     7890 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/chart/result_builder.py
+-rw-r--r--   0        0        0      728 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/chart/types.py
+-rw-r--r--   0        0        0     5355 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/collection_decorator.py
+-rw-r--r--   0        0        0        0 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/computed/__init__.py
+-rw-r--r--   0        0        0     5310 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/computed/collections.py
+-rw-r--r--   0        0        0      154 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/computed/exceptions.py
+-rw-r--r--   0        0        0     3890 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/computed/helpers.py
+-rw-r--r--   0        0        0      748 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/computed/types.py
+-rw-r--r--   0        0        0     2802 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/computed/utils.py
+-rw-r--r--   0        0        0     1666 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/datasource_decorator.py
+-rw-r--r--   0        0        0     5079 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/decorator_stack.py
+-rw-r--r--   0        0        0        0 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/empty/__init__.py
+-rw-r--r--   0        0        0     4495 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/empty/collection.py
+-rw-r--r--   0        0        0        0 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/hook/__init__.py
+-rw-r--r--   0        0        0     4841 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/hook/collections.py
+-rw-r--r--   0        0        0        0 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/hook/context/__init__.py
+-rw-r--r--   0        0        0     1233 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/hook/context/aggregate.py
+-rw-r--r--   0        0        0      870 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/hook/context/create.py
+-rw-r--r--   0        0        0      599 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/hook/context/delete.py
+-rw-r--r--   0        0        0      525 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/hook/context/hooks.py
+-rw-r--r--   0        0        0     1153 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/hook/context/list.py
+-rw-r--r--   0        0        0      777 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/hook/context/update.py
+-rw-r--r--   0        0        0      852 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/hook/hooks.py
+-rw-r--r--   0        0        0      392 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/hook/types.py
+-rw-r--r--   0        0        0        0 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/operators_emulate/__init__.py
+-rw-r--r--   0        0        0     6521 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/operators_emulate/collections.py
+-rw-r--r--   0        0        0      371 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/operators_emulate/types.py
+-rw-r--r--   0        0        0        0 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/operators_equivalence/__init__.py
+-rw-r--r--   0        0        0     3855 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/operators_equivalence/collections.py
+-rw-r--r--   0        0        0        0 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/publication/__init__.py
+-rw-r--r--   0        0        0     3866 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/publication/collections.py
+-rw-r--r--   0        0        0     2421 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/publication/datasource.py
+-rw-r--r--   0        0        0        0 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/relation/__init__.py
+-rw-r--r--   0        0        0    12558 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/relation/collections.py
+-rw-r--r--   0        0        0     1125 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/relation/types.py
+-rw-r--r--   0        0        0        0 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/rename_collection/__init__.py
+-rw-r--r--   0        0        0     1041 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/rename_collection/collection.py
+-rw-r--r--   0        0        0     2897 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/rename_collection/datasource.py
+-rw-r--r--   0        0        0        0 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/rename_field/__init__.py
+-rw-r--r--   0        0        0    10161 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/rename_field/collections.py
+-rw-r--r--   0        0        0        0 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/schema/__init__.py
+-rw-r--r--   0        0        0      671 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/schema/collection.py
+-rw-r--r--   0        0        0        0 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/search/__init__.py
+-rw-r--r--   0        0        0     6164 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/search/collections.py
+-rw-r--r--   0        0        0        0 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/segments/__init__.py
+-rw-r--r--   0        0        0     2627 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/segments/collections.py
+-rw-r--r--   0        0        0        0 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/sort_emulate/__init__.py
+-rw-r--r--   0        0        0     6009 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/sort_emulate/collections.py
+-rw-r--r--   0        0        0        0 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/validation/__init__.py
+-rw-r--r--   0        0        0     4019 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/validation/collection.py
+-rw-r--r--   0        0        0        0 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/write/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/write/create_relations/__init__.py
+-rw-r--r--   0        0        0     4987 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/write/create_relations/create_relations_collection.py
+-rw-r--r--   0        0        0        0 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/write/update_relations/__init__.py
+-rw-r--r--   0        0        0     4845 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/write/update_relations/update_relations_collection.py
+-rw-r--r--   0        0        0     1020 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/write/write_datasource_decorator.py
+-rw-r--r--   0        0        0        0 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/write/write_replace/__init__.py
+-rw-r--r--   0        0        0      420 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/write/write_replace/types.py
+-rw-r--r--   0        0        0      932 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/write/write_replace/write_customization_context.py
+-rw-r--r--   0        0        0     6436 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/write/write_replace/write_replace_collection.py
+-rw-r--r--   0        0        0     2331 2024-04-03 08:04:21.676932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/exceptions.py
+-rw-r--r--   0        0        0     6148 2024-04-03 08:04:21.680932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/interfaces/.DS_Store
+-rw-r--r--   0        0        0        0 2024-04-03 08:04:21.680932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/interfaces/__init__.py
+-rw-r--r--   0        0        0     3551 2024-04-03 08:04:21.680932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/interfaces/actions.py
+-rw-r--r--   0        0        0     1141 2024-04-03 08:04:21.680932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/interfaces/chart.py
+-rw-r--r--   0        0        0     2463 2024-04-03 08:04:21.680932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/interfaces/collections.py
+-rw-r--r--   0        0        0     5160 2024-04-03 08:04:21.680932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/interfaces/fields.py
+-rw-r--r--   0        0        0        0 2024-04-03 08:04:21.680932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/interfaces/models/__init__.py
+-rw-r--r--   0        0        0     1346 2024-04-03 08:04:21.680932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/interfaces/models/collections.py
+-rw-r--r--   0        0        0     6148 2024-04-03 08:04:21.680932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/interfaces/query/.DS_Store
+-rw-r--r--   0        0        0        0 2024-04-03 08:04:21.680932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/interfaces/query/__init__.py
+-rw-r--r--   0        0        0     7998 2024-04-03 08:04:21.680932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/interfaces/query/aggregation.py
+-rw-r--r--   0        0        0     6148 2024-04-03 08:04:21.680932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/interfaces/query/condition_tree/.DS_Store
+-rw-r--r--   0        0        0        0 2024-04-03 08:04:21.680932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/interfaces/query/condition_tree/__init__.py
+-rw-r--r--   0        0        0     4505 2024-04-03 08:04:21.680932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/interfaces/query/condition_tree/equivalence.py
+-rw-r--r--   0        0        0     5340 2024-04-03 08:04:21.680932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/interfaces/query/condition_tree/factory.py
+-rw-r--r--   0        0        0        0 2024-04-03 08:04:21.680932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/__init__.py
+-rw-r--r--   0        0        0     2696 2024-04-03 08:04:21.680932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/base.py
+-rw-r--r--   0        0        0     4844 2024-04-03 08:04:21.680932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/branch.py
+-rw-r--r--   0        0        0     9918 2024-04-03 08:04:21.680932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/leaf.py
+-rw-r--r--   0        0        0     1270 2024-04-03 08:04:21.680932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/operators.py
+-rw-r--r--   0        0        0        0 2024-04-03 08:04:21.680932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/__init__.py
+-rw-r--r--   0        0        0     3836 2024-04-03 08:04:21.680932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/comparison.py
+-rw-r--r--   0        0        0     1688 2024-04-03 08:04:21.680932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/pattern.py
+-rw-r--r--   0        0        0     7643 2024-04-03 08:04:21.680932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/time.py
+-rw-r--r--   0        0        0        0 2024-04-03 08:04:21.680932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/interfaces/query/filter/__init__.py
+-rw-r--r--   0        0        0     8081 2024-04-03 08:04:21.680932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/interfaces/query/filter/factory.py
+-rw-r--r--   0        0        0     2889 2024-04-03 08:04:21.680932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/interfaces/query/filter/paginated.py
+-rw-r--r--   0        0        0     3110 2024-04-03 08:04:21.680932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/interfaces/query/filter/unpaginated.py
+-rw-r--r--   0        0        0      759 2024-04-03 08:04:21.680932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/interfaces/query/page.py
+-rw-r--r--   0        0        0     4442 2024-04-03 08:04:21.680932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/interfaces/query/projections/__init__.py
+-rw-r--r--   0        0        0      902 2024-04-03 08:04:21.680932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/interfaces/query/projections/factory.py
+-rw-r--r--   0        0        0     2455 2024-04-03 08:04:21.680932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/interfaces/query/sort/__init__.py
+-rw-r--r--   0        0        0      595 2024-04-03 08:04:21.680932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/interfaces/query/sort/factory.py
+-rw-r--r--   0        0        0      118 2024-04-03 08:04:21.680932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/interfaces/records.py
+-rw-r--r--   0        0        0        0 2024-04-03 08:04:21.680932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/plugins/__init__.py
+-rw-r--r--   0        0        0     2514 2024-04-03 08:04:21.680932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/plugins/add_external_relation.py
+-rw-r--r--   0        0        0     4353 2024-04-03 08:04:21.680932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/plugins/import_field.py
+-rw-r--r--   0        0        0      395 2024-04-03 08:04:21.680932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/plugins/plugin.py
+-rw-r--r--   0        0        0       73 2024-04-03 08:04:21.680932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/utils/__init__.py
+-rw-r--r--   0        0        0     8601 2024-04-03 08:04:21.680932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/utils/collections.py
+-rw-r--r--   0        0        0     2559 2024-04-03 08:04:21.680932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/utils/operators.py
+-rw-r--r--   0        0        0     1169 2024-04-03 08:04:21.680932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/utils/records.py
+-rw-r--r--   0        0        0     1878 2024-04-03 08:04:21.680932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/utils/schema.py
+-rw-r--r--   0        0        0      449 2024-04-03 08:04:21.680932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/utils/user_callable.py
+-rw-r--r--   0        0        0        0 2024-04-03 08:04:21.680932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/validations/__init__.py
+-rw-r--r--   0        0        0     4790 2024-04-03 08:04:21.680932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/validations/condition_tree.py
+-rw-r--r--   0        0        0     4231 2024-04-03 08:04:21.680932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/validations/field.py
+-rw-r--r--   0        0        0      393 2024-04-03 08:04:21.680932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/validations/projection.py
+-rw-r--r--   0        0        0     1542 2024-04-03 08:04:21.680932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/validations/records.py
+-rw-r--r--   0        0        0     4573 2024-04-03 08:04:21.680932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/validations/rules.py
+-rw-r--r--   0        0        0      469 2024-04-03 08:04:21.680932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/validations/sort.py
+-rw-r--r--   0        0        0     4649 2024-04-03 08:04:21.680932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/validations/type_getter.py
+-rw-r--r--   0        0        0      372 2024-04-03 08:04:21.680932 forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/validations/types.py
+-rw-r--r--   0        0        0     1567 2024-04-03 08:04:35.208932 forestadmin_datasource_toolkit-1.6.3/pyproject.toml
+-rw-r--r--   0        0        0      966 1970-01-01 00:00:00.000000 forestadmin_datasource_toolkit-1.6.3/PKG-INFO
```

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/collections.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/context/agent_context.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/context/agent_context.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/context/collection_context.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/context/collection_context.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/context/relaxed_wrappers/collection.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/context/relaxed_wrappers/collection.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/datasource_customizer/collection_customizer.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/datasource_customizer/collection_customizer.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/datasource_customizer/datasource_customizer.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/datasource_customizer/datasource_customizer.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/datasources.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/datasources.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/action/collections.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/action/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/action/context/base.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/action/context/base.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/action/context/bulk.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/action/context/bulk.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/action/context/single.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/action/context/single.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/action/result_builder.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/action/result_builder.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/action/types/actions.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/action/types/actions.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/action/types/fields.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/action/types/fields.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/action/types/widgets.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/action/types/widgets.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/binary/collection.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/binary/collection.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/chart/chart_collection_decorator.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/chart/chart_collection_decorator.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/chart/chart_datasource_decorator.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/chart/chart_datasource_decorator.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/chart/collection_chart_context.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/chart/collection_chart_context.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/chart/result_builder.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/chart/result_builder.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/chart/types.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/chart/types.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/collection_decorator.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/collection_decorator.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/computed/collections.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/computed/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/computed/helpers.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/computed/helpers.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import copy
-from typing import Any, List, Optional, Tuple, cast
+from typing import Any, List, Tuple, cast
 
 from forestadmin.datasource_toolkit.context.collection_context import CollectionCustomizationContext
 from forestadmin.datasource_toolkit.decorators.computed.types import ComputedDefinition
 from forestadmin.datasource_toolkit.decorators.computed.utils import Output, flatten, transform_unique_values, unflatten
 from forestadmin.datasource_toolkit.interfaces.fields import RelationAlias
 from forestadmin.datasource_toolkit.interfaces.query.projections import Projection
 from forestadmin.datasource_toolkit.interfaces.records import RecordsDataAlias
@@ -40,48 +40,49 @@
 async def queue_field(
     ctx: CollectionCustomizationContext,
     collection: Any,
     new_path: str,
     paths: List[str],
     flatten_records: List[List[Any]],
 ):
+    # Skip double computations (we're not checking before adding to queue).
     if new_path not in paths:
         computed = collection.get_computed(new_path)
-        dependencies = Projection(*computed["dependencies"])
+        nested_dependencies = Projection(*computed["dependencies"])
         if ":" in new_path:
             nested_field = new_path.split(":")[0]
-            dependencies = cast(List[str], dependencies.nest(nested_field))
-            dependencies.sort()
-        for path in cast(List[str], dependencies):
+            nested_dependencies = nested_dependencies.nest(nested_field)
+        for path in nested_dependencies:
             await queue_field(ctx, collection, path, paths, flatten_records.copy())
-        dependency_values = [flatten_records[paths.index(path)] for path in cast(List[str], dependencies)]
+        dependency_values = [flatten_records[paths.index(path)] for path in nested_dependencies]
         paths.append(new_path)
 
         return await compute_field(ctx, computed, computed["dependencies"], copy.deepcopy(dependency_values)) or []
 
 
 async def compute_from_records(
     ctx: CollectionCustomizationContext,
     collection: Any,
     records_projection: Projection,
     desired_projections: Projection,
-    records: List[Optional[RecordsDataAlias]],
+    records: List[RecordsDataAlias],
 ) -> List[RecordsDataAlias]:
+    # As there is nothing to compute let's return
+    if len(records) == 0:
+        return []
+
     paths: List[str] = [*records_projection]
-    paths.sort()
-    cast(List[str], desired_projections).sort()
     flatten_records = flatten(records, paths)
     add_operations: List[Tuple[int, Any]] = []
     delete_operations: List[int] = []
 
-    for i, path in enumerate(cast(List[str], desired_projections)):
+    for i, path in enumerate(desired_projections):
         value = await queue_field(ctx, collection, path, paths, copy.deepcopy(flatten_records))
         if value is not None:
             add_operations.append((i, value))
-            # operations.append((i, value, 1))
 
     for path in paths:
         if path not in desired_projections:
             delete_operations.append(paths.index(path))
 
     delete_operations.sort(key=lambda o: o, reverse=True)
     add_operations.sort(key=lambda o: o[0])
```

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/computed/types.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/computed/types.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/computed/utils.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/computed/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         if any(record.values()):
             res.append(record)
         else:
             res.append(None)
     return res
 
 
-def flatten(records: List[Optional[RecordsDataAlias]], projection: List[str]) -> FlatRecordList:
+def flatten(records: List[RecordsDataAlias], projection: List[str]) -> FlatRecordList:
     res: FlatRecordList = []
     for field_name in projection:
         values: List[Optional[str]] = []
         for record in records:
             if record:
                 values.append(RecordUtils.get_field_value(record, field_name))
             else:
```

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/datasource_decorator.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/datasource_decorator.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/decorator_stack.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/decorator_stack.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/empty/collection.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/empty/collection.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/hook/collections.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/hook/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/hook/context/aggregate.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/hook/context/aggregate.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/hook/context/create.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/hook/context/create.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/hook/context/delete.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/hook/context/delete.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/hook/context/hooks.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/hook/context/hooks.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/hook/context/list.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/hook/context/list.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/hook/context/update.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/hook/context/update.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/hook/hooks.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/hook/hooks.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/operators_emulate/collections.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/operators_emulate/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/operators_equivalence/collections.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/operators_equivalence/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/publication/collections.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/publication/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/publication/datasource.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/publication/datasource.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/relation/collections.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/relation/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/relation/types.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/relation/types.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/rename_collection/collection.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/rename_collection/collection.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/rename_collection/datasource.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/rename_collection/datasource.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/rename_field/collections.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/rename_field/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/schema/collection.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/schema/collection.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/search/collections.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/search/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/segments/collections.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/segments/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/sort_emulate/collections.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/sort_emulate/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/validation/collection.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/validation/collection.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/write/create_relations/create_relations_collection.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/write/create_relations/create_relations_collection.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/write/update_relations/update_relations_collection.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/write/update_relations/update_relations_collection.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/write/write_datasource_decorator.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/write/write_datasource_decorator.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/write/write_replace/write_customization_context.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/write/write_replace/write_customization_context.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/write/write_replace/write_replace_collection.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/decorators/write/write_replace/write_replace_collection.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/exceptions.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/exceptions.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/.DS_Store` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/interfaces/.DS_Store`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/actions.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/interfaces/actions.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/chart.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/interfaces/chart.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/collections.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/interfaces/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/fields.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/interfaces/fields.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/models/collections.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/interfaces/models/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/.DS_Store` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/interfaces/query/.DS_Store`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/aggregation.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/interfaces/query/aggregation.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/.DS_Store` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/interfaces/query/condition_tree/.DS_Store`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/equivalence.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/interfaces/query/condition_tree/equivalence.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/factory.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/interfaces/query/condition_tree/factory.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/base.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/base.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/branch.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/branch.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/leaf.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/leaf.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/operators.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/operators.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/comparison.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/comparison.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/pattern.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/pattern.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/time.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/time.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/filter/factory.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/interfaces/query/filter/factory.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/filter/paginated.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/interfaces/query/filter/paginated.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/filter/unpaginated.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/interfaces/query/filter/unpaginated.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/page.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/interfaces/query/page.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/projections/__init__.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/interfaces/query/projections/__init__.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/projections/factory.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/interfaces/query/projections/factory.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/sort/__init__.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/interfaces/query/sort/__init__.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/sort/factory.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/interfaces/query/sort/factory.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/plugins/add_external_relation.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/plugins/add_external_relation.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/plugins/import_field.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/plugins/import_field.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/utils/collections.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/utils/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/utils/operators.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/utils/operators.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/utils/records.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/utils/records.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/utils/schema.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/utils/schema.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/validations/condition_tree.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/validations/condition_tree.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/validations/field.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/validations/field.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/validations/records.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/validations/records.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/validations/rules.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/validations/rules.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/validations/type_getter.py` & `forestadmin_datasource_toolkit-1.6.3/forestadmin/datasource_toolkit/validations/type_getter.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.2/pyproject.toml` & `forestadmin_datasource_toolkit-1.6.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "forestadmin-datasource-toolkit"
 description = "datasource toolkit for forestadmin python agent"
-version = "1.6.2"
+version = "1.6.3"
 authors = [ "Valentin Monté <valentinm@forestadmin.com>", "Julien Barreau <julien.barreau@forestadmin.com>",]
 readme = "README.md"
 repository = "https://github.com/ForestAdmin/agent-python"
 documentation = "https://docs.forestadmin.com/developer-guide-agents-python/"
 homepage = "https://www.forestadmin.com"
 [[tool.poetry.packages]]
 include = "forestadmin"
```

### Comparing `forestadmin_datasource_toolkit-1.6.2/PKG-INFO` & `forestadmin_datasource_toolkit-1.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forestadmin-datasource-toolkit
-Version: 1.6.2
+Version: 1.6.3
 Summary: datasource toolkit for forestadmin python agent
 Home-page: https://www.forestadmin.com
 Author: Valentin Monté
 Author-email: valentinm@forestadmin.com
 Requires-Python: >=3.8,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

