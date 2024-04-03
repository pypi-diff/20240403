# Comparing `tmp/shexer-2.2.2.tar.gz` & `tmp/shexer-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shexer-2.2.2.tar", last modified: Fri Nov 10 20:25:31 2023, max compression
+gzip compressed data, was "shexer-2.3.0.tar", last modified: Wed Apr  3 11:55:15 2024, max compression
```

## Comparing `shexer-2.2.2.tar` & `shexer-2.3.0.tar`

### file list

```diff
@@ -1,250 +1,252 @@
-drwxrwxrwx   0        0        0        0 2023-11-10 20:25:31.489400 shexer-2.2.2/
--rw-rw-rw-   0        0        0    11558 2023-06-27 16:13:11.000000 shexer-2.2.2/LICENSE
--rw-rw-rw-   0        0        0    27235 2023-11-10 20:25:31.489400 shexer-2.2.2/PKG-INFO
--rw-rw-rw-   0        0        0    26360 2023-06-27 16:13:11.000000 shexer-2.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-11-10 20:25:29.992838 shexer-2.2.2/local_code/
--rw-rw-rw-   0        0        0        0 2023-07-20 16:50:30.000000 shexer-2.2.2/local_code/__init__.py
--rw-rw-rw-   0        0        0     1278 2023-11-10 20:18:22.000000 shexer-2.2.2/local_code/beyza_test.py
--rw-rw-rw-   0        0        0     2756 2023-09-04 15:19:36.000000 shexer-2.2.2/local_code/split_non_split_thats_the_question.py
--rw-rw-rw-   0        0        0     9733 2023-11-08 19:45:06.000000 shexer-2.2.2/local_code/tictactoe.py
--rw-rw-rw-   0        0        0       25 2023-11-10 08:27:58.000000 shexer-2.2.2/local_code/whatever.py
--rw-rw-rw-   0        0        0     1428 2023-10-02 17:19:16.000000 shexer-2.2.2/local_code/yasunori_Test.py
--rw-rw-rw-   0        0        0       86 2023-11-10 20:25:31.495905 shexer-2.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1370 2023-11-10 20:24:47.000000 shexer-2.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-11-10 20:25:30.005098 shexer-2.2.2/shexer/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/__init__.py
--rw-rw-rw-   0        0        0      644 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/consts.py
-drwxrwxrwx   0        0        0        0 2023-11-10 20:25:30.047788 shexer-2.2.2/shexer/core/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-10 20:25:30.069202 shexer-2.2.2/shexer/core/instances/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/core/instances/__init__.py
--rw-rw-rw-   0        0        0      713 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/core/instances/abstract_instance_tracker.py
-drwxrwxrwx   0        0        0        0 2023-11-10 20:25:30.102936 shexer-2.2.2/shexer/core/instances/annotators/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/core/instances/annotators/__init__.py
--rw-rw-rw-   0        0        0      383 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/core/instances/annotators/annotator_func.py
--rw-rw-rw-   0        0        0     1817 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/core/instances/annotators/annotator_tracking_instances.py
--rw-rw-rw-   0        0        0     3895 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/core/instances/annotators/base_annotator.py
-drwxrwxrwx   0        0        0        0 2023-11-10 20:25:30.179588 shexer-2.2.2/shexer/core/instances/annotators/strategy_mode/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/core/instances/annotators/strategy_mode/__init__.py
--rw-rw-rw-   0        0        0      665 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/core/instances/annotators/strategy_mode/all_classes_mode.py
--rw-rw-rw-   0        0        0      760 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/core/instances/annotators/strategy_mode/base_strategy_mode.py
--rw-rw-rw-   0        0        0      807 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/core/instances/annotators/strategy_mode/compound_strategy_mode.py
--rw-rw-rw-   0        0        0     2675 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/core/instances/annotators/strategy_mode/instance_cap_mode.py
--rw-rw-rw-   0        0        0       86 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/core/instances/annotators/strategy_mode/instances_cap_exception.py
--rw-rw-rw-   0        0        0     1793 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/core/instances/annotators/strategy_mode/shape_qualifiers_mode.py
--rw-rw-rw-   0        0        0      815 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/core/instances/annotators/strategy_mode/target_classes_mode.py
--rw-rw-rw-   0        0        0     4553 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/core/instances/instance_tracker.py
-drwxrwxrwx   0        0        0        0 2023-11-10 20:25:30.190554 shexer-2.2.2/shexer/core/instances/mappings/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/core/instances/mappings/__init__.py
--rw-rw-rw-   0        0        0     1081 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/core/instances/mappings/shape_map_instance_tracker.py
-drwxrwxrwx   0        0        0        0 2023-11-10 20:25:30.194516 shexer-2.2.2/shexer/core/instances/mix/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/core/instances/mix/__init__.py
--rw-rw-rw-   0        0        0     2652 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/core/instances/mix/mixed_instance_tracker.py
--rw-rw-rw-   0        0        0       22 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/core/instances/pconsts.py
-drwxrwxrwx   0        0        0        0 2023-11-10 20:25:30.204519 shexer-2.2.2/shexer/core/profiling/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/core/profiling/__init__.py
--rw-rw-rw-   0        0        0     8613 2023-10-20 16:00:26.000000 shexer-2.2.2/shexer/core/profiling/class_profiler.py
--rw-rw-rw-   0        0        0      182 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/core/profiling/consts.py
-drwxrwxrwx   0        0        0        0 2023-11-10 20:25:30.228953 shexer-2.2.2/shexer/core/profiling/strategy/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/core/profiling/strategy/__init__.py
--rw-rw-rw-   0        0        0     6976 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/core/profiling/strategy/abstract_feature_direction_strategy.py
--rw-rw-rw-   0        0        0     1349 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/core/profiling/strategy/direct_features_strategy.py
--rw-rw-rw-   0        0        0     7395 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/core/profiling/strategy/include_reverse_features_strategy.py
-drwxrwxrwx   0        0        0        0 2023-11-10 20:25:30.232931 shexer-2.2.2/shexer/core/shexing/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/core/shexing/__init__.py
--rw-rw-rw-   0        0        0     6186 2023-10-20 16:00:26.000000 shexer-2.2.2/shexer/core/shexing/class_shexer.py
-drwxrwxrwx   0        0        0        0 2023-11-10 20:25:30.241085 shexer-2.2.2/shexer/core/shexing/strategy/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/core/shexing/strategy/__init__.py
--rw-rw-rw-   0        0        0    17141 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/core/shexing/strategy/abstract_shexing_strategy.py
--rw-rw-rw-   0        0        0     5685 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/core/shexing/strategy/direct_and_inverse_shexing_strategy.py
--rw-rw-rw-   0        0        0     2804 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/core/shexing/strategy/direct_shexing_strategy.py
-drwxrwxrwx   0        0        0        0 2023-11-10 20:25:30.257449 shexer-2.2.2/shexer/core/shexing/strategy/minimal_iri_strategy/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/core/shexing/strategy/minimal_iri_strategy/__init__.py
--rw-rw-rw-   0        0        0      118 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/core/shexing/strategy/minimal_iri_strategy/abstract_min_iri_strategy.py
--rw-rw-rw-   0        0        0     1088 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/core/shexing/strategy/minimal_iri_strategy/annotate_min_iri_strategy.py
--rw-rw-rw-   0        0        0      412 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/core/shexing/strategy/minimal_iri_strategy/ignore_min_iri_strategy.py
-drwxrwxrwx   0        0        0        0 2023-11-10 20:25:30.275574 shexer-2.2.2/shexer/io/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/io/__init__.py
--rw-rw-rw-   0        0        0      103 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/io/file.py
-drwxrwxrwx   0        0        0        0 2023-11-10 20:25:30.277806 shexer-2.2.2/shexer/io/graph/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/io/graph/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-10 20:25:30.371152 shexer-2.2.2/shexer/io/graph/yielder/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/io/graph/yielder/__init__.py
--rw-rw-rw-   0        0        0     1431 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/io/graph/yielder/base_triples_yielder.py
--rw-rw-rw-   0        0        0    16304 2023-10-20 16:00:26.000000 shexer-2.2.2/shexer/io/graph/yielder/big_ttl_triples_yielder.py
-drwxrwxrwx   0        0        0        0 2023-11-10 20:25:30.383839 shexer-2.2.2/shexer/io/graph/yielder/filter/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/io/graph/yielder/filter/__init__.py
--rw-rw-rw-   0        0        0      862 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/io/graph/yielder/filter/filter_namespaces_triple_yielder.py
--rw-rw-rw-   0        0        0     1131 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/io/graph/yielder/multi_big_ttl_files_triple_yielder.py
--rw-rw-rw-   0        0        0     1132 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/io/graph/yielder/multi_nt_triples_yielder.py
--rw-rw-rw-   0        0        0     1757 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/io/graph/yielder/multi_rdflib_triple_yielder.py
--rw-rw-rw-   0        0        0     1166 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/io/graph/yielder/multi_tsv_nt_triples_yielder.py
--rw-rw-rw-   0        0        0     2674 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/io/graph/yielder/multifile_base_triples_yielder.py
--rw-rw-rw-   0        0        0     5686 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/io/graph/yielder/nt_triples_yielder.py
--rw-rw-rw-   0        0        0     6817 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/io/graph/yielder/rdflib_triple_yielder.py
-drwxrwxrwx   0        0        0        0 2023-11-10 20:25:30.387922 shexer-2.2.2/shexer/io/graph/yielder/remote/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/io/graph/yielder/remote/__init__.py
--rw-rw-rw-   0        0        0     3826 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/io/graph/yielder/remote/sgraph_from_selectors_triple_yielder.py
--rw-rw-rw-   0        0        0     4724 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/io/graph/yielder/tsv_nt_triples_yielder.py
-drwxrwxrwx   0        0        0        0 2023-11-10 20:25:30.399892 shexer-2.2.2/shexer/io/json/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/io/json/__init__.py
--rw-rw-rw-   0        0        0      207 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/io/json/json_loader.py
-drwxrwxrwx   0        0        0        0 2023-11-10 20:25:30.435069 shexer-2.2.2/shexer/io/line_reader/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/io/line_reader/__init__.py
--rw-rw-rw-   0        0        0      285 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/io/line_reader/file_line_reader.py
--rw-rw-rw-   0        0        0      332 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/io/line_reader/gz_line_reader.py
--rw-rw-rw-   0        0        0      260 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/io/line_reader/raw_string_line_reader.py
--rw-rw-rw-   0        0        0      353 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/io/line_reader/zip_file_line_reader.py
-drwxrwxrwx   0        0        0        0 2023-11-10 20:25:30.436924 shexer-2.2.2/shexer/io/profile/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/io/profile/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-10 20:25:30.447915 shexer-2.2.2/shexer/io/profile/formater/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/io/profile/formater/__init__.py
--rw-rw-rw-   0        0        0      409 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/io/profile/formater/abstract_profile_serializer.py
-drwxrwxrwx   0        0        0        0 2023-11-10 20:25:30.448894 shexer-2.2.2/shexer/io/shacl/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/io/shacl/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-10 20:25:30.461569 shexer-2.2.2/shexer/io/shacl/formater/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/io/shacl/formater/__init__.py
--rw-rw-rw-   0        0        0    16449 2023-11-10 20:24:47.000000 shexer-2.2.2/shexer/io/shacl/formater/shacl_serializer.py
-drwxrwxrwx   0        0        0        0 2023-11-10 20:25:30.474753 shexer-2.2.2/shexer/io/shape_map/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/io/shape_map/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-10 20:25:30.485195 shexer-2.2.2/shexer/io/shape_map/label/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/io/shape_map/label/__init__.py
--rw-rw-rw-   0        0        0     1410 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/io/shape_map/label/shape_map_label_parser.py
-drwxrwxrwx   0        0        0        0 2023-11-10 20:25:30.497166 shexer-2.2.2/shexer/io/shape_map/node_selector/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/io/shape_map/node_selector/__init__.py
--rw-rw-rw-   0        0        0     6755 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/io/shape_map/node_selector/node_selector_parser.py
--rw-rw-rw-   0        0        0     4966 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/io/shape_map/shape_map_parser.py
-drwxrwxrwx   0        0        0        0 2023-11-10 20:25:30.500054 shexer-2.2.2/shexer/io/shex/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/io/shex/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-10 20:25:30.519869 shexer-2.2.2/shexer/io/shex/formater/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/io/shex/formater/__init__.py
--rw-rw-rw-   0        0        0      244 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/io/shex/formater/consts.py
--rw-rw-rw-   0        0        0     7006 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/io/shex/formater/shex_serializer.py
-drwxrwxrwx   0        0        0        0 2023-11-10 20:25:30.555111 shexer-2.2.2/shexer/io/shex/formater/statement_serializers/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/io/shex/formater/statement_serializers/__init__.py
--rw-rw-rw-   0        0        0     6083 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/io/shex/formater/statement_serializers/base_statement_serializer.py
--rw-rw-rw-   0        0        0     2287 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/io/shex/formater/statement_serializers/fixed_prop_choice_statement_serializer.py
-drwxrwxrwx   0        0        0        0 2023-11-10 20:25:30.594366 shexer-2.2.2/shexer/io/shex/formater/statement_serializers/frequency_strategy/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/io/shex/formater/statement_serializers/frequency_strategy/__init__.py
--rw-rw-rw-   0        0        0      383 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/io/shex/formater/statement_serializers/frequency_strategy/abs_freq_serializer.py
--rw-rw-rw-   0        0        0      171 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/io/shex/formater/statement_serializers/frequency_strategy/base_frequency_strategy.py
--rw-rw-rw-   0        0        0      887 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/io/shex/formater/statement_serializers/frequency_strategy/mixed_frequency_strategy.py
--rw-rw-rw-   0        0        0     1278 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/io/shex/formater/statement_serializers/frequency_strategy/ratio_freq_serializer.py
--rw-rw-rw-   0        0        0     1500 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/io/shex/formater/statement_serializers/inverse_statement_serializer.py
--rw-rw-rw-   0        0        0     3211 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/io/shex/formater/statement_serializers/st_serializers_factory.py
-drwxrwxrwx   0        0        0        0 2023-11-10 20:25:30.598371 shexer-2.2.2/shexer/io/sparql/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/io/sparql/__init__.py
--rw-rw-rw-   0        0        0     4538 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/io/sparql/query.py
--rw-rw-rw-   0        0        0      469 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/io/wikidata.py
-drwxrwxrwx   0        0        0        0 2023-11-10 20:25:30.711902 shexer-2.2.2/shexer/model/
--rw-rw-rw-   0        0        0      552 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/model/IRI.py
--rw-rw-rw-   0        0        0      280 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/model/Literal.py
--rw-rw-rw-   0        0        0      810 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/model/Macro.py
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/model/__init__.py
--rw-rw-rw-   0        0        0      502 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/model/bnode.py
--rw-rw-rw-   0        0        0      100 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/model/const_elem_types.py
--rw-rw-rw-   0        0        0     1119 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/model/fixed_prop_choice_statement.py
-drwxrwxrwx   0        0        0        0 2023-11-10 20:25:30.732903 shexer-2.2.2/shexer/model/graph/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/model/graph/__init__.py
--rw-rw-rw-   0        0        0     6186 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/model/graph/abstract_sgraph.py
--rw-rw-rw-   0        0        0     7633 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/model/graph/endpoint_sgraph.py
--rw-rw-rw-   0        0        0     6201 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/model/graph/rdflib_sgraph.py
--rw-rw-rw-   0        0        0     4173 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/model/hierarchy_tree.py
--rw-rw-rw-   0        0        0     2527 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/model/node_selector.py
--rw-rw-rw-   0        0        0      427 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/model/property.py
--rw-rw-rw-   0        0        0     3361 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/model/shape.py
--rw-rw-rw-   0        0        0      858 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/model/shape_map.py
--rw-rw-rw-   0        0        0     2716 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/model/statement.py
--rw-rw-rw-   0        0        0    24783 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/shaper.py
-drwxrwxrwx   0        0        0        0 2023-11-10 20:25:30.814652 shexer-2.2.2/shexer/utils/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/utils/__init__.py
--rw-rw-rw-   0        0        0      621 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/utils/compression.py
--rw-rw-rw-   0        0        0       94 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/utils/dict.py
-drwxrwxrwx   0        0        0        0 2023-11-10 20:25:30.909878 shexer-2.2.2/shexer/utils/factories/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/utils/factories/__init__.py
--rw-rw-rw-   0        0        0     4300 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/utils/factories/class_profiler_factory.py
--rw-rw-rw-   0        0        0     2322 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/utils/factories/class_shexer_factory.py
--rw-rw-rw-   0        0        0      728 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/utils/factories/h_tree.py
--rw-rw-rw-   0        0        0    12338 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/utils/factories/instance_tracker_factory.py
--rw-rw-rw-   0        0        0      437 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/utils/factories/iri_factory.py
--rw-rw-rw-   0        0        0      286 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/utils/factories/remote_graph_factory.py
--rw-rw-rw-   0        0        0     1985 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/utils/factories/shape_map_factory.py
--rw-rw-rw-   0        0        0      616 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/utils/factories/shape_map_parser_factory.py
--rw-rw-rw-   0        0        0     1723 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/utils/factories/shape_serializer_factory.py
--rw-rw-rw-   0        0        0    18627 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/utils/factories/triple_yielders_factory.py
--rw-rw-rw-   0        0        0      123 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/utils/file.py
--rw-rw-rw-   0        0        0      397 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/utils/log.py
--rw-rw-rw-   0        0        0      803 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/utils/namespaces.py
--rw-rw-rw-   0        0        0      967 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/utils/obj_references.py
--rw-rw-rw-   0        0        0     2008 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/utils/shapes.py
--rw-rw-rw-   0        0        0     1397 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/utils/target_elements.py
-drwxrwxrwx   0        0        0        0 2023-11-10 20:25:30.914903 shexer-2.2.2/shexer/utils/translators/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/utils/translators/__init__.py
--rw-rw-rw-   0        0        0     2881 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/utils/translators/list_of_classes_to_shape_map.py
--rw-rw-rw-   0        0        0     3026 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/utils/triple_yielders.py
--rw-rw-rw-   0        0        0     5708 2023-06-27 16:13:11.000000 shexer-2.2.2/shexer/utils/uri.py
-drwxrwxrwx   0        0        0        0 2023-11-10 20:25:30.044794 shexer-2.2.2/shexer.egg-info/
--rw-rw-rw-   0        0        0    27235 2023-11-10 20:25:29.000000 shexer-2.2.2/shexer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     8188 2023-11-10 20:25:29.000000 shexer-2.2.2/shexer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-10 20:25:29.000000 shexer-2.2.2/shexer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-11-10 20:25:29.000000 shexer-2.2.2/shexer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-11-10 20:25:29.000000 shexer-2.2.2/shexer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-11-10 20:25:31.388716 shexer-2.2.2/test/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.2.2/test/__init__.py
--rw-rw-rw-   0        0        0     1903 2023-06-27 16:13:11.000000 shexer-2.2.2/test/const.py
--rw-rw-rw-   0        0        0     8963 2023-06-27 16:13:11.000000 shexer-2.2.2/test/t_utils.py
--rw-rw-rw-   0        0        0     1488 2023-06-27 16:13:11.000000 shexer-2.2.2/test/test_all_classes_mode.py
--rw-rw-rw-   0        0        0     1525 2023-06-27 16:13:11.000000 shexer-2.2.2/test/test_allow_opt_cardinality.py
--rw-rw-rw-   0        0        0     3541 2023-06-27 16:13:11.000000 shexer-2.2.2/test/test_allow_redundant_or.py
-drwxrwxrwx   0        0        0        0 2023-11-10 20:25:31.413452 shexer-2.2.2/test/test_bugs/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.2.2/test/test_bugs/__init__.py
--rw-rw-rw-   0        0        0      796 2023-06-27 16:13:11.000000 shexer-2.2.2/test/test_bugs/test_no_sharp_in_auto_shape_names.py
--rw-rw-rw-   0        0        0     1192 2023-06-27 16:13:11.000000 shexer-2.2.2/test/test_bugs/test_no_sharp_nor_slash_due_to_prefixing.py
--rw-rw-rw-   0        0        0     9920 2023-06-27 16:13:11.000000 shexer-2.2.2/test/test_compression_mode.py
--rw-rw-rw-   0        0        0     2171 2023-06-27 16:13:11.000000 shexer-2.2.2/test/test_decimals.py
--rw-rw-rw-   0        0        0     5564 2023-06-27 16:13:11.000000 shexer-2.2.2/test/test_depth_for_building_subgraph.py
--rw-rw-rw-   0        0        0     3526 2023-06-27 16:13:11.000000 shexer-2.2.2/test/test_detect_minimal_iri.py
--rw-rw-rw-   0        0        0     1388 2023-06-27 16:13:11.000000 shexer-2.2.2/test/test_disable_comments.py
--rw-rw-rw-   0        0        0     2922 2023-06-27 16:13:11.000000 shexer-2.2.2/test/test_disable_endpoint_cache.py
--rw-rw-rw-   0        0        0     1491 2023-06-27 16:13:11.000000 shexer-2.2.2/test/test_disable_exact_cardinality.py
--rw-rw-rw-   0        0        0     2557 2023-06-27 16:13:11.000000 shexer-2.2.2/test/test_disable_or_statements.py
--rw-rw-rw-   0        0        0     3786 2023-06-27 16:13:11.000000 shexer-2.2.2/test/test_discard_and_compliant.py
--rw-rw-rw-   0        0        0     2090 2023-06-27 16:13:11.000000 shexer-2.2.2/test/test_file_target_classes.py
--rw-rw-rw-   0        0        0     1677 2023-06-27 16:13:11.000000 shexer-2.2.2/test/test_graph_file_input.py
--rw-rw-rw-   0        0        0     3456 2023-06-27 16:13:11.000000 shexer-2.2.2/test/test_graph_list_of_file_inputs.py
--rw-rw-rw-   0        0        0     1951 2023-06-27 16:13:11.000000 shexer-2.2.2/test/test_infer_numeric_types_for_untyped_literals.py
--rw-rw-rw-   0        0        0     7818 2023-06-27 16:13:11.000000 shexer-2.2.2/test/test_input_format.py
--rw-rw-rw-   0        0        0     4648 2023-06-27 16:13:11.000000 shexer-2.2.2/test/test_instances_cap.py
--rw-rw-rw-   0        0        0     3367 2023-06-27 16:13:11.000000 shexer-2.2.2/test/test_instances_file_input.py
--rw-rw-rw-   0        0        0     3852 2023-06-27 16:13:11.000000 shexer-2.2.2/test/test_instances_report.py
--rw-rw-rw-   0        0        0     3548 2023-06-27 16:13:11.000000 shexer-2.2.2/test/test_instantiation_property.py
--rw-rw-rw-   0        0        0     1964 2023-06-27 16:13:11.000000 shexer-2.2.2/test/test_inverse_paths.py
--rw-rw-rw-   0        0        0     3594 2023-06-27 16:13:11.000000 shexer-2.2.2/test/test_keep_less_specific.py
--rw-rw-rw-   0        0        0     4051 2023-06-27 16:13:11.000000 shexer-2.2.2/test/test_list_of_url_input.py
--rw-rw-rw-   0        0        0     4106 2023-06-27 16:13:11.000000 shexer-2.2.2/test/test_namespaces_dict.py
--rw-rw-rw-   0        0        0     2082 2023-06-27 16:13:11.000000 shexer-2.2.2/test/test_namespaces_to_ignore.py
--rw-rw-rw-   0        0        0     5000 2023-06-27 16:13:11.000000 shexer-2.2.2/test/test_raw_graph.py
--rw-rw-rw-   0        0        0     4300 2023-06-27 16:13:11.000000 shexer-2.2.2/test/test_raw_shape_map.py
--rw-rw-rw-   0        0        0     1711 2023-06-27 16:13:11.000000 shexer-2.2.2/test/test_rdflib_graph.py
--rw-rw-rw-   0        0        0     2932 2023-10-20 16:00:26.000000 shexer-2.2.2/test/test_remove_empty_sahpes.py
-drwxrwxrwx   0        0        0        0 2023-11-10 20:25:31.462779 shexer-2.2.2/test/test_shacl/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.2.2/test/test_shacl/__init__.py
--rw-rw-rw-   0        0        0     2225 2023-06-27 16:13:11.000000 shexer-2.2.2/test/test_shacl/test_annotation.py
--rw-rw-rw-   0        0        0     2242 2023-06-27 16:13:11.000000 shexer-2.2.2/test/test_shacl/test_class_selection.py
--rw-rw-rw-   0        0        0     3291 2023-06-27 16:13:11.000000 shexer-2.2.2/test/test_shacl/test_detect_minimal_iri.py
--rw-rw-rw-   0        0        0      875 2023-11-10 20:24:47.000000 shexer-2.2.2/test/test_shacl/test_https.py
--rw-rw-rw-   0        0        0     1534 2023-11-10 20:24:47.000000 shexer-2.2.2/test/test_shacl/test_literal_types.py
--rw-rw-rw-   0        0        0     4313 2023-06-27 16:13:11.000000 shexer-2.2.2/test/test_shape_map_file.py
--rw-rw-rw-   0        0        0     6086 2023-06-27 16:13:11.000000 shexer-2.2.2/test/test_shape_map_format.py
--rw-rw-rw-   0        0        0     2307 2023-06-27 16:13:11.000000 shexer-2.2.2/test/test_shape_qualifiers_mode.py
--rw-rw-rw-   0        0        0     2889 2023-06-27 16:13:11.000000 shexer-2.2.2/test/test_shapes_namespaces.py
--rw-rw-rw-   0        0        0     2452 2023-06-27 16:13:11.000000 shexer-2.2.2/test/test_sort.py
--rw-rw-rw-   0        0        0     2058 2023-10-20 15:05:20.000000 shexer-2.2.2/test/test_target_classes.py
--rw-rw-rw-   0        0        0     3120 2023-06-27 16:13:11.000000 shexer-2.2.2/test/test_threshold.py
--rw-rw-rw-   0        0        0     2578 2023-06-27 16:13:11.000000 shexer-2.2.2/test/test_url_endpoint.py
--rw-rw-rw-   0        0        0     1867 2023-06-27 16:13:11.000000 shexer-2.2.2/test/test_url_graph.py
--rw-rw-rw-   0        0        0     1900 2023-06-27 16:13:11.000000 shexer-2.2.2/test/test_wikidata_annotation.py
-drwxrwxrwx   0        0        0        0 2023-11-10 20:25:31.486715 shexer-2.2.2/ws/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.2.2/ws/__init__.py
--rw-rw-rw-   0        0        0    19884 2023-06-27 16:13:11.000000 shexer-2.2.2/ws/shexer_rest.py
--rw-rw-rw-   0        0        0       28 2023-06-27 16:13:11.000000 shexer-2.2.2/ws/wsgi.py
+drwxrwxrwx   0        0        0        0 2024-04-03 11:55:15.414820 shexer-2.3.0/
+-rw-rw-rw-   0        0        0    11558 2023-06-27 16:13:11.000000 shexer-2.3.0/LICENSE
+-rw-rw-rw-   0        0        0    27235 2024-04-03 11:55:15.415005 shexer-2.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0    26360 2023-06-27 16:13:11.000000 shexer-2.3.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-03 11:55:12.837550 shexer-2.3.0/local_code/
+-rw-rw-rw-   0        0        0        0 2023-07-20 16:50:30.000000 shexer-2.3.0/local_code/__init__.py
+-rw-rw-rw-   0        0        0     1278 2023-11-10 20:18:22.000000 shexer-2.3.0/local_code/beyza_test.py
+-rw-rw-rw-   0        0        0     1411 2023-11-30 17:16:03.000000 shexer-2.3.0/local_code/img_example.py
+-rw-rw-rw-   0        0        0     2756 2023-09-04 15:19:36.000000 shexer-2.3.0/local_code/split_non_split_thats_the_question.py
+-rw-rw-rw-   0        0        0     9733 2023-11-08 19:45:06.000000 shexer-2.3.0/local_code/tictactoe.py
+-rw-rw-rw-   0        0        0       88 2023-11-13 10:50:47.000000 shexer-2.3.0/local_code/whatever.py
+-rw-rw-rw-   0        0        0     1428 2023-10-02 17:19:16.000000 shexer-2.3.0/local_code/yasunori_Test.py
+-rw-rw-rw-   0        0        0       86 2024-04-03 11:55:15.419841 shexer-2.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1370 2024-04-03 11:54:32.000000 shexer-2.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 11:55:12.860170 shexer-2.3.0/shexer/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/__init__.py
+-rw-rw-rw-   0        0        0      644 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/consts.py
+drwxrwxrwx   0        0        0        0 2024-04-03 11:55:12.917785 shexer-2.3.0/shexer/core/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 11:55:12.965382 shexer-2.3.0/shexer/core/instances/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/instances/__init__.py
+-rw-rw-rw-   0        0        0      713 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/instances/abstract_instance_tracker.py
+drwxrwxrwx   0        0        0        0 2024-04-03 11:55:13.016640 shexer-2.3.0/shexer/core/instances/annotators/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/instances/annotators/__init__.py
+-rw-rw-rw-   0        0        0      383 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/instances/annotators/annotator_func.py
+-rw-rw-rw-   0        0        0     1817 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/instances/annotators/annotator_tracking_instances.py
+-rw-rw-rw-   0        0        0     3895 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/instances/annotators/base_annotator.py
+drwxrwxrwx   0        0        0        0 2024-04-03 11:55:13.100211 shexer-2.3.0/shexer/core/instances/annotators/strategy_mode/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/instances/annotators/strategy_mode/__init__.py
+-rw-rw-rw-   0        0        0      665 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/instances/annotators/strategy_mode/all_classes_mode.py
+-rw-rw-rw-   0        0        0      760 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/instances/annotators/strategy_mode/base_strategy_mode.py
+-rw-rw-rw-   0        0        0      807 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/instances/annotators/strategy_mode/compound_strategy_mode.py
+-rw-rw-rw-   0        0        0     2675 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/instances/annotators/strategy_mode/instance_cap_mode.py
+-rw-rw-rw-   0        0        0       86 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/instances/annotators/strategy_mode/instances_cap_exception.py
+-rw-rw-rw-   0        0        0     1793 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/instances/annotators/strategy_mode/shape_qualifiers_mode.py
+-rw-rw-rw-   0        0        0      815 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/instances/annotators/strategy_mode/target_classes_mode.py
+-rw-rw-rw-   0        0        0     4553 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/instances/instance_tracker.py
+drwxrwxrwx   0        0        0        0 2024-04-03 11:55:13.114576 shexer-2.3.0/shexer/core/instances/mappings/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/instances/mappings/__init__.py
+-rw-rw-rw-   0        0        0     1081 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/instances/mappings/shape_map_instance_tracker.py
+drwxrwxrwx   0        0        0        0 2024-04-03 11:55:13.135524 shexer-2.3.0/shexer/core/instances/mix/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/instances/mix/__init__.py
+-rw-rw-rw-   0        0        0     2652 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/instances/mix/mixed_instance_tracker.py
+-rw-rw-rw-   0        0        0       22 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/instances/pconsts.py
+drwxrwxrwx   0        0        0        0 2024-04-03 11:55:13.163451 shexer-2.3.0/shexer/core/profiling/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/profiling/__init__.py
+-rw-rw-rw-   0        0        0     8613 2023-10-20 16:00:26.000000 shexer-2.3.0/shexer/core/profiling/class_profiler.py
+-rw-rw-rw-   0        0        0      182 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/profiling/consts.py
+drwxrwxrwx   0        0        0        0 2024-04-03 11:55:13.217765 shexer-2.3.0/shexer/core/profiling/strategy/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/profiling/strategy/__init__.py
+-rw-rw-rw-   0        0        0     6976 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/profiling/strategy/abstract_feature_direction_strategy.py
+-rw-rw-rw-   0        0        0     1349 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/profiling/strategy/direct_features_strategy.py
+-rw-rw-rw-   0        0        0     7395 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/profiling/strategy/include_reverse_features_strategy.py
+drwxrwxrwx   0        0        0        0 2024-04-03 11:55:13.243220 shexer-2.3.0/shexer/core/shexing/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/shexing/__init__.py
+-rw-rw-rw-   0        0        0     6186 2023-10-20 16:00:26.000000 shexer-2.3.0/shexer/core/shexing/class_shexer.py
+drwxrwxrwx   0        0        0        0 2024-04-03 11:55:13.307048 shexer-2.3.0/shexer/core/shexing/strategy/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/shexing/strategy/__init__.py
+-rw-rw-rw-   0        0        0    17141 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/shexing/strategy/abstract_shexing_strategy.py
+-rw-rw-rw-   0        0        0     5685 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/shexing/strategy/direct_and_inverse_shexing_strategy.py
+-rw-rw-rw-   0        0        0     2804 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/shexing/strategy/direct_shexing_strategy.py
+drwxrwxrwx   0        0        0        0 2024-04-03 11:55:13.352536 shexer-2.3.0/shexer/core/shexing/strategy/minimal_iri_strategy/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/shexing/strategy/minimal_iri_strategy/__init__.py
+-rw-rw-rw-   0        0        0      118 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/shexing/strategy/minimal_iri_strategy/abstract_min_iri_strategy.py
+-rw-rw-rw-   0        0        0     1088 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/shexing/strategy/minimal_iri_strategy/annotate_min_iri_strategy.py
+-rw-rw-rw-   0        0        0      412 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/core/shexing/strategy/minimal_iri_strategy/ignore_min_iri_strategy.py
+drwxrwxrwx   0        0        0        0 2024-04-03 11:55:13.382225 shexer-2.3.0/shexer/io/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/__init__.py
+-rw-rw-rw-   0        0        0      103 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/file.py
+drwxrwxrwx   0        0        0        0 2024-04-03 11:55:13.383898 shexer-2.3.0/shexer/io/graph/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/graph/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 11:55:13.571397 shexer-2.3.0/shexer/io/graph/yielder/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/graph/yielder/__init__.py
+-rw-rw-rw-   0        0        0     1431 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/graph/yielder/base_triples_yielder.py
+-rw-rw-rw-   0        0        0    16304 2023-10-20 16:00:26.000000 shexer-2.3.0/shexer/io/graph/yielder/big_ttl_triples_yielder.py
+drwxrwxrwx   0        0        0        0 2024-04-03 11:55:13.583685 shexer-2.3.0/shexer/io/graph/yielder/filter/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/graph/yielder/filter/__init__.py
+-rw-rw-rw-   0        0        0      862 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/graph/yielder/filter/filter_namespaces_triple_yielder.py
+-rw-rw-rw-   0        0        0     1131 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/graph/yielder/multi_big_ttl_files_triple_yielder.py
+-rw-rw-rw-   0        0        0     1132 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/graph/yielder/multi_nt_triples_yielder.py
+-rw-rw-rw-   0        0        0     1757 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/graph/yielder/multi_rdflib_triple_yielder.py
+-rw-rw-rw-   0        0        0     1166 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/graph/yielder/multi_tsv_nt_triples_yielder.py
+-rw-rw-rw-   0        0        0     1483 2024-04-03 11:54:32.000000 shexer-2.3.0/shexer/io/graph/yielder/multi_zip_triples_yielder.py
+-rw-rw-rw-   0        0        0     2670 2024-04-03 11:54:32.000000 shexer-2.3.0/shexer/io/graph/yielder/multifile_base_triples_yielder.py
+-rw-rw-rw-   0        0        0     5686 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/graph/yielder/nt_triples_yielder.py
+-rw-rw-rw-   0        0        0     6817 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/graph/yielder/rdflib_triple_yielder.py
+drwxrwxrwx   0        0        0        0 2024-04-03 11:55:13.604438 shexer-2.3.0/shexer/io/graph/yielder/remote/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/graph/yielder/remote/__init__.py
+-rw-rw-rw-   0        0        0     3826 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/graph/yielder/remote/sgraph_from_selectors_triple_yielder.py
+-rw-rw-rw-   0        0        0     4724 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/graph/yielder/tsv_nt_triples_yielder.py
+drwxrwxrwx   0        0        0        0 2024-04-03 11:55:13.621320 shexer-2.3.0/shexer/io/json/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/json/__init__.py
+-rw-rw-rw-   0        0        0      207 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/json/json_loader.py
+drwxrwxrwx   0        0        0        0 2024-04-03 11:55:13.682312 shexer-2.3.0/shexer/io/line_reader/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/line_reader/__init__.py
+-rw-rw-rw-   0        0        0      285 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/line_reader/file_line_reader.py
+-rw-rw-rw-   0        0        0      332 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/line_reader/gz_line_reader.py
+-rw-rw-rw-   0        0        0      260 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/line_reader/raw_string_line_reader.py
+-rw-rw-rw-   0        0        0      353 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/line_reader/zip_file_line_reader.py
+drwxrwxrwx   0        0        0        0 2024-04-03 11:55:13.684308 shexer-2.3.0/shexer/io/profile/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/profile/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 11:55:13.701263 shexer-2.3.0/shexer/io/profile/formater/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/profile/formater/__init__.py
+-rw-rw-rw-   0        0        0      409 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/profile/formater/abstract_profile_serializer.py
+drwxrwxrwx   0        0        0        0 2024-04-03 11:55:13.704254 shexer-2.3.0/shexer/io/shacl/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/shacl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 11:55:13.722207 shexer-2.3.0/shexer/io/shacl/formater/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/shacl/formater/__init__.py
+-rw-rw-rw-   0        0        0    16449 2023-11-10 20:24:47.000000 shexer-2.3.0/shexer/io/shacl/formater/shacl_serializer.py
+drwxrwxrwx   0        0        0        0 2024-04-03 11:55:13.737436 shexer-2.3.0/shexer/io/shape_map/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/shape_map/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 11:55:13.755124 shexer-2.3.0/shexer/io/shape_map/label/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/shape_map/label/__init__.py
+-rw-rw-rw-   0        0        0     1410 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/shape_map/label/shape_map_label_parser.py
+drwxrwxrwx   0        0        0        0 2024-04-03 11:55:13.781071 shexer-2.3.0/shexer/io/shape_map/node_selector/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/shape_map/node_selector/__init__.py
+-rw-rw-rw-   0        0        0     6755 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/shape_map/node_selector/node_selector_parser.py
+-rw-rw-rw-   0        0        0     4966 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/shape_map/shape_map_parser.py
+drwxrwxrwx   0        0        0        0 2024-04-03 11:55:13.784119 shexer-2.3.0/shexer/io/shex/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/shex/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 11:55:13.818977 shexer-2.3.0/shexer/io/shex/formater/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/shex/formater/__init__.py
+-rw-rw-rw-   0        0        0      244 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/shex/formater/consts.py
+-rw-rw-rw-   0        0        0     7006 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/shex/formater/shex_serializer.py
+drwxrwxrwx   0        0        0        0 2024-04-03 11:55:13.879812 shexer-2.3.0/shexer/io/shex/formater/statement_serializers/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/shex/formater/statement_serializers/__init__.py
+-rw-rw-rw-   0        0        0     6083 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/shex/formater/statement_serializers/base_statement_serializer.py
+-rw-rw-rw-   0        0        0     2287 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/shex/formater/statement_serializers/fixed_prop_choice_statement_serializer.py
+drwxrwxrwx   0        0        0        0 2024-04-03 11:55:13.952657 shexer-2.3.0/shexer/io/shex/formater/statement_serializers/frequency_strategy/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/shex/formater/statement_serializers/frequency_strategy/__init__.py
+-rw-rw-rw-   0        0        0      383 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/shex/formater/statement_serializers/frequency_strategy/abs_freq_serializer.py
+-rw-rw-rw-   0        0        0      171 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/shex/formater/statement_serializers/frequency_strategy/base_frequency_strategy.py
+-rw-rw-rw-   0        0        0      887 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/shex/formater/statement_serializers/frequency_strategy/mixed_frequency_strategy.py
+-rw-rw-rw-   0        0        0     1278 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/shex/formater/statement_serializers/frequency_strategy/ratio_freq_serializer.py
+-rw-rw-rw-   0        0        0     1500 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/shex/formater/statement_serializers/inverse_statement_serializer.py
+-rw-rw-rw-   0        0        0     3211 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/shex/formater/statement_serializers/st_serializers_factory.py
+drwxrwxrwx   0        0        0        0 2024-04-03 11:55:13.969615 shexer-2.3.0/shexer/io/sparql/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/sparql/__init__.py
+-rw-rw-rw-   0        0        0     4538 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/sparql/query.py
+-rw-rw-rw-   0        0        0      469 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/io/wikidata.py
+drwxrwxrwx   0        0        0        0 2024-04-03 11:55:14.148009 shexer-2.3.0/shexer/model/
+-rw-rw-rw-   0        0        0      552 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/model/IRI.py
+-rw-rw-rw-   0        0        0      280 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/model/Literal.py
+-rw-rw-rw-   0        0        0      810 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/model/Macro.py
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/model/__init__.py
+-rw-rw-rw-   0        0        0      502 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/model/bnode.py
+-rw-rw-rw-   0        0        0      100 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/model/const_elem_types.py
+-rw-rw-rw-   0        0        0     1119 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/model/fixed_prop_choice_statement.py
+drwxrwxrwx   0        0        0        0 2024-04-03 11:55:14.185555 shexer-2.3.0/shexer/model/graph/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/model/graph/__init__.py
+-rw-rw-rw-   0        0        0     6186 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/model/graph/abstract_sgraph.py
+-rw-rw-rw-   0        0        0     7633 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/model/graph/endpoint_sgraph.py
+-rw-rw-rw-   0        0        0     6201 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/model/graph/rdflib_sgraph.py
+-rw-rw-rw-   0        0        0     4173 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/model/hierarchy_tree.py
+-rw-rw-rw-   0        0        0     2527 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/model/node_selector.py
+-rw-rw-rw-   0        0        0      427 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/model/property.py
+-rw-rw-rw-   0        0        0     3361 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/model/shape.py
+-rw-rw-rw-   0        0        0      858 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/model/shape_map.py
+-rw-rw-rw-   0        0        0     2716 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/model/statement.py
+-rw-rw-rw-   0        0        0    24783 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/shaper.py
+drwxrwxrwx   0        0        0        0 2024-04-03 11:55:14.299050 shexer-2.3.0/shexer/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/utils/__init__.py
+-rw-rw-rw-   0        0        0      621 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/utils/compression.py
+-rw-rw-rw-   0        0        0       94 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/utils/dict.py
+drwxrwxrwx   0        0        0        0 2024-04-03 11:55:14.457634 shexer-2.3.0/shexer/utils/factories/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/utils/factories/__init__.py
+-rw-rw-rw-   0        0        0     4300 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/utils/factories/class_profiler_factory.py
+-rw-rw-rw-   0        0        0     2322 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/utils/factories/class_shexer_factory.py
+-rw-rw-rw-   0        0        0      728 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/utils/factories/h_tree.py
+-rw-rw-rw-   0        0        0    12338 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/utils/factories/instance_tracker_factory.py
+-rw-rw-rw-   0        0        0      437 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/utils/factories/iri_factory.py
+-rw-rw-rw-   0        0        0      286 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/utils/factories/remote_graph_factory.py
+-rw-rw-rw-   0        0        0     1985 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/utils/factories/shape_map_factory.py
+-rw-rw-rw-   0        0        0      616 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/utils/factories/shape_map_parser_factory.py
+-rw-rw-rw-   0        0        0     1723 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/utils/factories/shape_serializer_factory.py
+-rw-rw-rw-   0        0        0    21108 2024-04-03 11:54:32.000000 shexer-2.3.0/shexer/utils/factories/triple_yielders_factory.py
+-rw-rw-rw-   0        0        0      123 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/utils/file.py
+-rw-rw-rw-   0        0        0      397 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/utils/log.py
+-rw-rw-rw-   0        0        0      761 2023-11-20 19:07:29.000000 shexer-2.3.0/shexer/utils/namespaces.py
+-rw-rw-rw-   0        0        0      967 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/utils/obj_references.py
+-rw-rw-rw-   0        0        0     2008 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/utils/shapes.py
+-rw-rw-rw-   0        0        0     1397 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/utils/target_elements.py
+drwxrwxrwx   0        0        0        0 2024-04-03 11:55:14.479570 shexer-2.3.0/shexer/utils/translators/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/utils/translators/__init__.py
+-rw-rw-rw-   0        0        0     2881 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/utils/translators/list_of_classes_to_shape_map.py
+-rw-rw-rw-   0        0        0     3026 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/utils/triple_yielders.py
+-rw-rw-rw-   0        0        0     5708 2023-06-27 16:13:11.000000 shexer-2.3.0/shexer/utils/uri.py
+drwxrwxrwx   0        0        0        0 2024-04-03 11:55:12.914793 shexer-2.3.0/shexer.egg-info/
+-rw-rw-rw-   0        0        0    27235 2024-04-03 11:55:12.000000 shexer-2.3.0/shexer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8267 2024-04-03 11:55:12.000000 shexer-2.3.0/shexer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 11:55:12.000000 shexer-2.3.0/shexer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2024-04-03 11:55:12.000000 shexer-2.3.0/shexer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-04-03 11:55:12.000000 shexer-2.3.0/shexer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-03 11:55:15.251578 shexer-2.3.0/test/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/test/__init__.py
+-rw-rw-rw-   0        0        0     1903 2023-06-27 16:13:11.000000 shexer-2.3.0/test/const.py
+-rw-rw-rw-   0        0        0     8963 2023-06-27 16:13:11.000000 shexer-2.3.0/test/t_utils.py
+-rw-rw-rw-   0        0        0     1488 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_all_classes_mode.py
+-rw-rw-rw-   0        0        0     1525 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_allow_opt_cardinality.py
+-rw-rw-rw-   0        0        0     3541 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_allow_redundant_or.py
+drwxrwxrwx   0        0        0        0 2024-04-03 11:55:15.282495 shexer-2.3.0/test/test_bugs/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_bugs/__init__.py
+-rw-rw-rw-   0        0        0      796 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_bugs/test_no_sharp_in_auto_shape_names.py
+-rw-rw-rw-   0        0        0     1192 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_bugs/test_no_sharp_nor_slash_due_to_prefixing.py
+-rw-rw-rw-   0        0        0    11274 2024-04-03 11:54:32.000000 shexer-2.3.0/test/test_compression_mode.py
+-rw-rw-rw-   0        0        0     2171 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_decimals.py
+-rw-rw-rw-   0        0        0     5564 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_depth_for_building_subgraph.py
+-rw-rw-rw-   0        0        0     3526 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_detect_minimal_iri.py
+-rw-rw-rw-   0        0        0     1388 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_disable_comments.py
+-rw-rw-rw-   0        0        0     2922 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_disable_endpoint_cache.py
+-rw-rw-rw-   0        0        0     1491 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_disable_exact_cardinality.py
+-rw-rw-rw-   0        0        0     2557 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_disable_or_statements.py
+-rw-rw-rw-   0        0        0     3786 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_discard_and_compliant.py
+-rw-rw-rw-   0        0        0     2090 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_file_target_classes.py
+-rw-rw-rw-   0        0        0     1677 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_graph_file_input.py
+-rw-rw-rw-   0        0        0     3456 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_graph_list_of_file_inputs.py
+-rw-rw-rw-   0        0        0     1951 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_infer_numeric_types_for_untyped_literals.py
+-rw-rw-rw-   0        0        0     7818 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_input_format.py
+-rw-rw-rw-   0        0        0     4648 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_instances_cap.py
+-rw-rw-rw-   0        0        0     3367 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_instances_file_input.py
+-rw-rw-rw-   0        0        0     3852 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_instances_report.py
+-rw-rw-rw-   0        0        0     3548 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_instantiation_property.py
+-rw-rw-rw-   0        0        0     1964 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_inverse_paths.py
+-rw-rw-rw-   0        0        0     3594 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_keep_less_specific.py
+-rw-rw-rw-   0        0        0     4051 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_list_of_url_input.py
+-rw-rw-rw-   0        0        0     4106 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_namespaces_dict.py
+-rw-rw-rw-   0        0        0     2082 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_namespaces_to_ignore.py
+-rw-rw-rw-   0        0        0     5000 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_raw_graph.py
+-rw-rw-rw-   0        0        0     4300 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_raw_shape_map.py
+-rw-rw-rw-   0        0        0     1711 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_rdflib_graph.py
+-rw-rw-rw-   0        0        0     2932 2023-10-20 16:00:26.000000 shexer-2.3.0/test/test_remove_empty_sahpes.py
+drwxrwxrwx   0        0        0        0 2024-04-03 11:55:15.368573 shexer-2.3.0/test/test_shacl/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_shacl/__init__.py
+-rw-rw-rw-   0        0        0     2225 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_shacl/test_annotation.py
+-rw-rw-rw-   0        0        0     2242 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_shacl/test_class_selection.py
+-rw-rw-rw-   0        0        0     3291 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_shacl/test_detect_minimal_iri.py
+-rw-rw-rw-   0        0        0      875 2023-11-10 20:24:47.000000 shexer-2.3.0/test/test_shacl/test_https.py
+-rw-rw-rw-   0        0        0     1534 2023-11-10 20:24:47.000000 shexer-2.3.0/test/test_shacl/test_literal_types.py
+-rw-rw-rw-   0        0        0     4313 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_shape_map_file.py
+-rw-rw-rw-   0        0        0     6086 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_shape_map_format.py
+-rw-rw-rw-   0        0        0     2307 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_shape_qualifiers_mode.py
+-rw-rw-rw-   0        0        0     2889 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_shapes_namespaces.py
+-rw-rw-rw-   0        0        0     2452 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_sort.py
+-rw-rw-rw-   0        0        0     2058 2023-10-20 15:05:20.000000 shexer-2.3.0/test/test_target_classes.py
+-rw-rw-rw-   0        0        0     3120 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_threshold.py
+-rw-rw-rw-   0        0        0     2578 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_url_endpoint.py
+-rw-rw-rw-   0        0        0     1867 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_url_graph.py
+-rw-rw-rw-   0        0        0     1900 2023-06-27 16:13:11.000000 shexer-2.3.0/test/test_wikidata_annotation.py
+drwxrwxrwx   0        0        0        0 2024-04-03 11:55:15.411863 shexer-2.3.0/ws/
+-rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.3.0/ws/__init__.py
+-rw-rw-rw-   0        0        0    19884 2023-06-27 16:13:11.000000 shexer-2.3.0/ws/shexer_rest.py
+-rw-rw-rw-   0        0        0       28 2023-06-27 16:13:11.000000 shexer-2.3.0/ws/wsgi.py
```

### Comparing `shexer-2.2.2/LICENSE` & `shexer-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/PKG-INFO` & `shexer-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: shexer
-Version: 2.2.2
+Version: 2.3.0
 Summary: Automatic schema extraction for RDF graphs
 Home-page: https://github.com/DaniFdezAlvarez/shexer
-Download-URL: https://github.com/DaniFdezAlvarez/shexer/archive/2.2.2.tar.gz
+Download-URL: https://github.com/DaniFdezAlvarez/shexer/archive/2.3.0.tar.gz
 Author: Daniel Fernandez-Alvarez
 Author-email: danifdezalvarez@gmail.com
 Keywords: testing,shexer,shexerp3,rdf,shex,shacl,schema
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `shexer-2.2.2/README.md` & `shexer-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/local_code/beyza_test.py` & `shexer-2.3.0/local_code/beyza_test.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/local_code/split_non_split_thats_the_question.py` & `shexer-2.3.0/local_code/split_non_split_thats_the_question.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/local_code/tictactoe.py` & `shexer-2.3.0/local_code/tictactoe.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/local_code/yasunori_Test.py` & `shexer-2.3.0/local_code/yasunori_Test.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/setup.py` & `shexer-2.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 def read(file_path):
 	with open(file_path, "r") as in_stream:
 		return in_stream.read()
 
 setup(
   name = 'shexer',
   packages = find_packages(exclude=["*.local_code.*"]), # this must be the same as the name above
-  version = '2.2.2',
+  version = '2.3.0',
   description = 'Automatic schema extraction for RDF graphs',
   author = 'Daniel Fernandez-Alvarez',
   author_email = 'danifdezalvarez@gmail.com',
   url = 'https://github.com/DaniFdezAlvarez/shexer',
-  download_url = 'https://github.com/DaniFdezAlvarez/shexer/archive/2.2.2.tar.gz',
+  download_url = 'https://github.com/DaniFdezAlvarez/shexer/archive/2.3.0.tar.gz',
   keywords = ['testing', 'shexer', 'shexerp3', "rdf", "shex", "shacl", "schema"],
   long_description = read('README.md'),
   long_description_content_type='text/markdown',
   classifiers=[
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
```

### Comparing `shexer-2.2.2/shexer/consts.py` & `shexer-2.3.0/shexer/consts.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/core/instances/abstract_instance_tracker.py` & `shexer-2.3.0/shexer/core/instances/abstract_instance_tracker.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/core/instances/annotators/annotator_tracking_instances.py` & `shexer-2.3.0/shexer/core/instances/annotators/annotator_tracking_instances.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/core/instances/annotators/base_annotator.py` & `shexer-2.3.0/shexer/core/instances/annotators/base_annotator.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/core/instances/annotators/strategy_mode/all_classes_mode.py` & `shexer-2.3.0/shexer/core/instances/annotators/strategy_mode/all_classes_mode.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/core/instances/annotators/strategy_mode/base_strategy_mode.py` & `shexer-2.3.0/shexer/core/instances/annotators/strategy_mode/base_strategy_mode.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/core/instances/annotators/strategy_mode/compound_strategy_mode.py` & `shexer-2.3.0/shexer/core/instances/annotators/strategy_mode/compound_strategy_mode.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/core/instances/annotators/strategy_mode/instance_cap_mode.py` & `shexer-2.3.0/shexer/core/instances/annotators/strategy_mode/instance_cap_mode.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/core/instances/annotators/strategy_mode/shape_qualifiers_mode.py` & `shexer-2.3.0/shexer/core/instances/annotators/strategy_mode/shape_qualifiers_mode.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/core/instances/annotators/strategy_mode/target_classes_mode.py` & `shexer-2.3.0/shexer/core/instances/annotators/strategy_mode/target_classes_mode.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/core/instances/instance_tracker.py` & `shexer-2.3.0/shexer/core/instances/instance_tracker.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/core/instances/mappings/shape_map_instance_tracker.py` & `shexer-2.3.0/shexer/core/instances/mappings/shape_map_instance_tracker.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/core/instances/mix/mixed_instance_tracker.py` & `shexer-2.3.0/shexer/core/instances/mix/mixed_instance_tracker.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/core/profiling/class_profiler.py` & `shexer-2.3.0/shexer/core/profiling/class_profiler.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/core/profiling/strategy/abstract_feature_direction_strategy.py` & `shexer-2.3.0/shexer/core/profiling/strategy/abstract_feature_direction_strategy.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/core/profiling/strategy/direct_features_strategy.py` & `shexer-2.3.0/shexer/core/profiling/strategy/direct_features_strategy.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/core/profiling/strategy/include_reverse_features_strategy.py` & `shexer-2.3.0/shexer/core/profiling/strategy/include_reverse_features_strategy.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/core/shexing/class_shexer.py` & `shexer-2.3.0/shexer/core/shexing/class_shexer.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/core/shexing/strategy/abstract_shexing_strategy.py` & `shexer-2.3.0/shexer/core/shexing/strategy/abstract_shexing_strategy.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/core/shexing/strategy/direct_and_inverse_shexing_strategy.py` & `shexer-2.3.0/shexer/core/shexing/strategy/direct_and_inverse_shexing_strategy.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/core/shexing/strategy/direct_shexing_strategy.py` & `shexer-2.3.0/shexer/core/shexing/strategy/direct_shexing_strategy.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/core/shexing/strategy/minimal_iri_strategy/annotate_min_iri_strategy.py` & `shexer-2.3.0/shexer/core/shexing/strategy/minimal_iri_strategy/annotate_min_iri_strategy.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/io/graph/yielder/base_triples_yielder.py` & `shexer-2.3.0/shexer/io/graph/yielder/base_triples_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/io/graph/yielder/big_ttl_triples_yielder.py` & `shexer-2.3.0/shexer/io/graph/yielder/big_ttl_triples_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/io/graph/yielder/filter/filter_namespaces_triple_yielder.py` & `shexer-2.3.0/shexer/io/graph/yielder/filter/filter_namespaces_triple_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/io/graph/yielder/multi_big_ttl_files_triple_yielder.py` & `shexer-2.3.0/shexer/io/graph/yielder/multi_big_ttl_files_triple_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/io/graph/yielder/multi_nt_triples_yielder.py` & `shexer-2.3.0/shexer/io/graph/yielder/multi_nt_triples_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/io/graph/yielder/multi_rdflib_triple_yielder.py` & `shexer-2.3.0/shexer/io/graph/yielder/multi_rdflib_triple_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/io/graph/yielder/multi_tsv_nt_triples_yielder.py` & `shexer-2.3.0/shexer/io/graph/yielder/multi_tsv_nt_triples_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/io/graph/yielder/multifile_base_triples_yielder.py` & `shexer-2.3.0/shexer/io/graph/yielder/multifile_base_triples_yielder.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,20 +32,20 @@
             self._error_triples_from_used_yielders += self._last_yielder.error_triples
         self._last_yielder = self._constructor_file_yielder(a_source_file=a_source_file)
         for a_triple in self._yield_triples_of_last_yielder(parse_namespaces):
             yield a_triple
 
     @property
     def yielded_triples(self):
-        triples_current_yielder = 0 if self._last_yielder is None else self._last_yielder.triples_yielded()
+        triples_current_yielder = 0 if self._last_yielder is None else self._last_yielder.yielded_triples
         return self._triples_yielded_from_used_yielders + triples_current_yielder
 
     @property
     def error_triples(self):
-        errors_current_yielder = 0 if self._last_yielder is None else self._last_yielder.error_triples()
+        errors_current_yielder = 0 if self._last_yielder is None else self._last_yielder.error_triples
         return self._error_triples_from_used_yielders  + errors_current_yielder
 
     def _reset_count(self):
         self._error_triples_from_used_yielders = 0
         self._triples_yielded_from_used_yielders = 0
 
     def _constructor_file_yielder(self, a_source_file):
```

### Comparing `shexer-2.2.2/shexer/io/graph/yielder/nt_triples_yielder.py` & `shexer-2.3.0/shexer/io/graph/yielder/nt_triples_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/io/graph/yielder/rdflib_triple_yielder.py` & `shexer-2.3.0/shexer/io/graph/yielder/rdflib_triple_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/io/graph/yielder/remote/sgraph_from_selectors_triple_yielder.py` & `shexer-2.3.0/shexer/io/graph/yielder/remote/sgraph_from_selectors_triple_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/io/graph/yielder/tsv_nt_triples_yielder.py` & `shexer-2.3.0/shexer/io/graph/yielder/tsv_nt_triples_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/io/shacl/formater/shacl_serializer.py` & `shexer-2.3.0/shexer/io/shacl/formater/shacl_serializer.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/io/shape_map/label/shape_map_label_parser.py` & `shexer-2.3.0/shexer/io/shape_map/label/shape_map_label_parser.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/io/shape_map/node_selector/node_selector_parser.py` & `shexer-2.3.0/shexer/io/shape_map/node_selector/node_selector_parser.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/io/shape_map/shape_map_parser.py` & `shexer-2.3.0/shexer/io/shape_map/shape_map_parser.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/io/shex/formater/shex_serializer.py` & `shexer-2.3.0/shexer/io/shex/formater/shex_serializer.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/io/shex/formater/statement_serializers/base_statement_serializer.py` & `shexer-2.3.0/shexer/io/shex/formater/statement_serializers/base_statement_serializer.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/io/shex/formater/statement_serializers/fixed_prop_choice_statement_serializer.py` & `shexer-2.3.0/shexer/io/shex/formater/statement_serializers/fixed_prop_choice_statement_serializer.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/io/shex/formater/statement_serializers/frequency_strategy/mixed_frequency_strategy.py` & `shexer-2.3.0/shexer/io/shex/formater/statement_serializers/frequency_strategy/mixed_frequency_strategy.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/io/shex/formater/statement_serializers/frequency_strategy/ratio_freq_serializer.py` & `shexer-2.3.0/shexer/io/shex/formater/statement_serializers/frequency_strategy/ratio_freq_serializer.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/io/shex/formater/statement_serializers/inverse_statement_serializer.py` & `shexer-2.3.0/shexer/io/shex/formater/statement_serializers/inverse_statement_serializer.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/io/shex/formater/statement_serializers/st_serializers_factory.py` & `shexer-2.3.0/shexer/io/shex/formater/statement_serializers/st_serializers_factory.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/io/sparql/query.py` & `shexer-2.3.0/shexer/io/sparql/query.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/model/IRI.py` & `shexer-2.3.0/shexer/model/IRI.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/model/Macro.py` & `shexer-2.3.0/shexer/model/Macro.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/model/fixed_prop_choice_statement.py` & `shexer-2.3.0/shexer/model/fixed_prop_choice_statement.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/model/graph/abstract_sgraph.py` & `shexer-2.3.0/shexer/model/graph/abstract_sgraph.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/model/graph/endpoint_sgraph.py` & `shexer-2.3.0/shexer/model/graph/endpoint_sgraph.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/model/graph/rdflib_sgraph.py` & `shexer-2.3.0/shexer/model/graph/rdflib_sgraph.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/model/hierarchy_tree.py` & `shexer-2.3.0/shexer/model/hierarchy_tree.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/model/node_selector.py` & `shexer-2.3.0/shexer/model/node_selector.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/model/shape.py` & `shexer-2.3.0/shexer/model/shape.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/model/shape_map.py` & `shexer-2.3.0/shexer/model/shape_map.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/model/statement.py` & `shexer-2.3.0/shexer/model/statement.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/shaper.py` & `shexer-2.3.0/shexer/shaper.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/utils/compression.py` & `shexer-2.3.0/shexer/utils/compression.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/utils/factories/class_profiler_factory.py` & `shexer-2.3.0/shexer/utils/factories/class_profiler_factory.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/utils/factories/class_shexer_factory.py` & `shexer-2.3.0/shexer/utils/factories/class_shexer_factory.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/utils/factories/h_tree.py` & `shexer-2.3.0/shexer/utils/factories/h_tree.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/utils/factories/instance_tracker_factory.py` & `shexer-2.3.0/shexer/utils/factories/instance_tracker_factory.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/utils/factories/shape_map_factory.py` & `shexer-2.3.0/shexer/utils/factories/shape_map_factory.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/utils/factories/shape_map_parser_factory.py` & `shexer-2.3.0/shexer/utils/factories/shape_map_parser_factory.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/utils/factories/shape_serializer_factory.py` & `shexer-2.3.0/shexer/utils/factories/shape_serializer_factory.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/utils/factories/triple_yielders_factory.py` & `shexer-2.3.0/shexer/utils/factories/triple_yielders_factory.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from shexer.io.graph.yielder.multi_tsv_nt_triples_yielder import MultiTsvNtTriplesYielder
 from shexer.io.graph.yielder.rdflib_triple_yielder import RdflibParserTripleYielder, RdflibTripleYielder
 from shexer.io.graph.yielder.multi_rdflib_triple_yielder import MultiRdfLibTripleYielder
 from shexer.io.graph.yielder.remote.sgraph_from_selectors_triple_yielder import SgraphFromSelectorsTripleYielder
 from shexer.io.graph.yielder.filter.filter_namespaces_triple_yielder import FilterNamespacesTriplesYielder
 from shexer.io.graph.yielder.big_ttl_triples_yielder import BigTtlTriplesYielder
 from shexer.io.graph.yielder.multi_big_ttl_files_triple_yielder import MultiBigTtlTriplesYielder
+from shexer.io.graph.yielder.multi_zip_triples_yielder import MultiZipTriplesYielder
 from shexer.utils.factories.shape_map_parser_factory import get_shape_map_parser
 from shexer.model.graph.endpoint_sgraph import EndpointSGraph
 from shexer.utils.translators.list_of_classes_to_shape_map import ListOfClassesToShapeMap
 from shexer.utils.target_elements import tune_target_classes_if_needed
 from shexer.utils.dict import reverse_keys_and_values
 from shexer.utils.compression import list_of_zip_internal_files
 from zipfile import ZipFile
@@ -45,28 +46,29 @@
         else:
             target_classes = tune_target_classes_if_needed(list_target_classes=target_classes,
                                                            prefix_namespaces_dict=prefix_namespaces_dict) \
                 if target_classes is not None \
                 else read_target_classes_from_file(file_target_classes=file_target_classes,
                                                    prefix_namespaces_dict=prefix_namespaces_dict)
 
-
             return translator.str_class_list_to_shape_map_sparql_selectors(str_list=target_classes,
                                                                            instantiation_property=instantiation_property,
                                                                            limit_remote_instances=limit_remote_instances)
 
+
 def get_triple_yielder(source_file=None, list_of_source_files=None, input_format=NT, namespaces_to_ignore=None,
                        allow_untyped_numbers=False, raw_graph=None, namespaces_dict=None, url_input=None,
-                       list_of_url_input=None, rdflib_graph=None, shape_map_file=None, shape_map_raw=None, shape_map_format=FIXED_SHAPE_MAP,
+                       list_of_url_input=None, rdflib_graph=None, shape_map_file=None, shape_map_raw=None,
+                       shape_map_format=FIXED_SHAPE_MAP,
                        track_classes_for_entities_at_last_depth_level=True, depth_for_building_subgraph=1,
                        url_endpoint=None, instantiation_property=None, strict_syntax_with_corners=False,
                        target_classes=None, file_target_classes=None, built_remote_graph=None,
                        built_shape_map=None, limit_remote_instances=-1, inverse_paths=False, all_classes_mode=False,
                        compression_mode=None, disable_endpoint_cache=False):
-    zip_base_archive = _get_base_zip_archive_if_needed(source_file, compression_mode)
+    zip_base_archives = _get_base_zip_archive_if_needed(source_file, list_of_source_files, compression_mode)
     result = None
     if url_endpoint is not None:
         result = _yielder_for_url_endpoint(built_remote_graph=built_remote_graph,
                                            url_endpoint=url_endpoint,
                                            built_shape_map=built_shape_map,
                                            shape_map_format=shape_map_format,
                                            namespaces_dict=namespaces_dict,
@@ -81,113 +83,140 @@
                                            track_classes_for_entities_at_last_depth_level=track_classes_for_entities_at_last_depth_level,
                                            strict_syntax_with_corners=strict_syntax_with_corners,
                                            allow_untyped_numbers=allow_untyped_numbers,
                                            inverse_paths=inverse_paths,
                                            disable_endpoint_cache=disable_endpoint_cache)
 
     elif url_input is not None or list_of_url_input is not None:  # Always use rdflib to parse remote graphs
-         result = _yielder_for_url_input(url_input=url_input,
+        result = _yielder_for_url_input(url_input=url_input,
                                         allow_untyped_numbers=allow_untyped_numbers,
                                         raw_graph=raw_graph,
                                         input_format=input_format,
                                         namespaces_dict=namespaces_dict,
                                         list_of_url_input=list_of_url_input)
     elif rdflib_graph is not None:
         result = RdflibTripleYielder(rdflib_graph=rdflib_graph,
                                      namespaces_dict=namespaces_dict)
     elif input_format == NT:
         result = _yielder_for_nt(source_file=source_file,
                                  raw_graph=raw_graph,
                                  allow_untyped_numbers=allow_untyped_numbers,
                                  list_of_source_files=list_of_source_files,
                                  compression_mode=compression_mode,
-                                 zip_base_archive=zip_base_archive)
+                                 zip_base_archives=zip_base_archives)
     elif input_format == TSV_SPO:
         result = _yielder_for_tsv_spo(source_file=source_file,
                                       allow_untyped_numbers=allow_untyped_numbers,
                                       raw_graph=raw_graph,
                                       list_of_files=list_of_source_files,
                                       compression_mode=compression_mode,
-                                      zip_base_archive=zip_base_archive)
+                                      zip_base_archives=zip_base_archives)
     elif input_format == TURTLE_ITER:
         result = _yielder_for_turtle_iter(source_file=source_file,
                                           allow_untyped_numbers=allow_untyped_numbers,
                                           raw_graph=raw_graph,
                                           list_of_files=list_of_source_files,
                                           compression_mode=compression_mode,
-                                          zip_base_archive=zip_base_archive)
+                                          zip_base_archives=zip_base_archives)
     elif input_format in [N3, RDF_XML, JSON_LD, TURTLE]:
         result = _yielder_for_rdflib_parser(source_file=source_file,
                                             allow_untyped_numbers=allow_untyped_numbers,
                                             raw_graph=raw_graph,
                                             input_format=input_format,
                                             namespaces_dict=namespaces_dict,
                                             list_of_source_files=list_of_source_files,
                                             compression_mode=compression_mode,
-                                            zip_base_archive=zip_base_archive)
+                                            zip_base_archives=zip_base_archives)
     else:
         raise ValueError("Not supported format: " + input_format)
 
     if namespaces_to_ignore is None:
         return result
     else:
         return FilterNamespacesTriplesYielder(actual_triple_yielder=result,
                                               namespaces_to_ignore=namespaces_to_ignore)
 
 
+def _yielder_for_compressed_inputs(base_yielders):
+    if len(base_yielders) == 1:
+        result = base_yielders[0]
+        return base_yielders[0]
+    return MultiZipTriplesYielder(multiyielders=base_yielders)
+
+
 def _yielder_for_rdflib_parser(source_file, allow_untyped_numbers, raw_graph,
                                input_format, namespaces_dict, list_of_source_files,
-                               compression_mode, zip_base_archive):
-    if zip_base_archive is not None:
-        return MultiRdfLibTripleYielder(list_of_files=list_of_zip_internal_files(zip_base_archive),
-                                        allow_untyped_numbers=allow_untyped_numbers,
-                                        input_format=input_format,
-                                        namespaces_dict=namespaces_dict,
-                                        compression_mode=compression_mode,
-                                        zip_archive_file=zip_base_archive)
+                               compression_mode, zip_base_archives):
+    if zip_base_archives is not None:
+        # return MultiRdfLibTripleYielder(list_of_files=list_of_zip_internal_files(zip_base_archive),
+        #                                 allow_untyped_numbers=allow_untyped_numbers,
+        #                                 input_format=input_format,
+        #                                 namespaces_dict=namespaces_dict,
+        #                                 compression_mode=compression_mode,
+        #                                 zip_archive_file=zip_base_archives)
+        return _yielder_for_compressed_inputs(
+            base_yielders=[MultiRdfLibTripleYielder(list_of_files=list_of_zip_internal_files(a_zip_file),
+                                                    allow_untyped_numbers=allow_untyped_numbers,
+                                                    input_format=input_format,
+                                                    namespaces_dict=namespaces_dict,
+                                                    compression_mode=compression_mode,
+                                                    zip_archive_file=a_zip_file) for a_zip_file in
+                           zip_base_archives])
 
     elif source_file is not None or raw_graph is not None:
         return RdflibParserTripleYielder(source=source_file,
                                          allow_untyped_numbers=allow_untyped_numbers,
                                          raw_graph=raw_graph,
                                          input_format=input_format,
                                          namespaces_dict=namespaces_dict,
                                          compression_mode=compression_mode)
+
     else:
         return MultiRdfLibTripleYielder(list_of_files=list_of_source_files,
-                                          allow_untyped_numbers=allow_untyped_numbers,
-                                          input_format=input_format,
-                                          namespaces_dict=namespaces_dict,
+                                        allow_untyped_numbers=allow_untyped_numbers,
+                                        input_format=input_format,
+                                        namespaces_dict=namespaces_dict,
                                         compression_mode=compression_mode)
 
+
 def _yielder_for_turtle_iter(source_file, raw_graph, allow_untyped_numbers, list_of_files,
-                             compression_mode, zip_base_archive):
-    if zip_base_archive is not None:
-        return MultiBigTtlTriplesYielder(list_of_files=list_of_zip_internal_files(zip_base_archive),
-                                         compression_mode=compression_mode,
-                                         allow_untyped_numbers=allow_untyped_numbers,
-                                         zip_base_archive=zip_base_archive)
+                             compression_mode, zip_base_archives):
+    if zip_base_archives is not None:
+        # return MultiBigTtlTriplesYielder(list_of_files=list_of_zip_internal_files(zip_base_archive),
+        #                                  compression_mode=compression_mode,
+        #                                  allow_untyped_numbers=allow_untyped_numbers,
+        #                                  zip_base_archives=zip_base_archives)
+        return _yielder_for_compressed_inputs(
+            [MultiBigTtlTriplesYielder(list_of_files=list_of_zip_internal_files(a_zip_file),
+                                       compression_mode=compression_mode,
+                                       allow_untyped_numbers=allow_untyped_numbers,
+                                       zip_base_archive=a_zip_file) for a_zip_file in zip_base_archives])
     elif source_file is not None or raw_graph is not None:
         return BigTtlTriplesYielder(source_file=source_file,
                                     allow_untyped_numbers=allow_untyped_numbers,
                                     raw_graph=raw_graph,
                                     compression_mode=compression_mode)
     else:
         return MultiBigTtlTriplesYielder(list_of_files=list_of_files,
                                          allow_untyped_numbers=allow_untyped_numbers,
                                          compression_mode=compression_mode)
 
 
 def _yielder_for_tsv_spo(source_file, raw_graph, allow_untyped_numbers, list_of_files,
-                         compression_mode, zip_base_archive):
-    if zip_base_archive is not None:
-        return MultiTsvNtTriplesYielder(list_of_files=list_of_zip_internal_files(zip_base_archive),
-                                        compression_mode=compression_mode,
-                                        allow_untyped_numbers=allow_untyped_numbers,
-                                        zip_base_archive=zip_base_archive)
+                         compression_mode, zip_base_archives):
+    if zip_base_archives is not None:
+        # return MultiTsvNtTriplesYielder(list_of_files=list_of_zip_internal_files(zip_base_archive),
+        #                                 compression_mode=compression_mode,
+        #                                 allow_untyped_numbers=allow_untyped_numbers,
+        #                                 zip_base_archives=zip_base_archives)
+        return _yielder_for_compressed_inputs(
+            [MultiTsvNtTriplesYielder(list_of_files=list_of_zip_internal_files(a_zip_file),
+                                      compression_mode=compression_mode,
+                                      allow_untyped_numbers=allow_untyped_numbers,
+                                      zip_base_archive=a_zip_file) for a_zip_file in zip_base_archives])
     elif source_file is not None or raw_graph is not None:
         return TsvNtTriplesYielder(source_file=source_file,
                                    allow_untyped_numbers=allow_untyped_numbers,
                                    raw_graph=raw_graph,
                                    compression_mode=compression_mode)
     else:
         return MultiTsvNtTriplesYielder(list_of_files=list_of_files,
@@ -201,14 +230,15 @@
         for a_line in in_stream:
             candidate = a_line.strip()
             if candidate != "":
                 result.append(candidate)
     return tune_target_classes_if_needed(list_target_classes=result,
                                          prefix_namespaces_dict=prefix_namespaces_dict)
 
+
 def _yielder_for_url_endpoint(built_remote_graph, url_endpoint, built_shape_map, shape_map_format,
                               namespaces_dict, target_classes, file_target_classes, shape_map_file,
                               shape_map_raw, instantiation_property, limit_remote_instances, all_classes_mode,
                               depth_for_building_subgraph, track_classes_for_entities_at_last_depth_level,
                               strict_syntax_with_corners, allow_untyped_numbers, inverse_paths, disable_endpoint_cache):
     sgrpah = built_remote_graph if built_remote_graph is not None else EndpointSGraph(endpoint_url=url_endpoint,
                                                                                       store_locally=not disable_endpoint_cache)
@@ -229,44 +259,57 @@
                                             depth=depth_for_building_subgraph,
                                             classes_at_last_level=track_classes_for_entities_at_last_depth_level,
                                             instantiation_property=instantiation_property,
                                             strict_syntax_with_corners=strict_syntax_with_corners,
                                             allow_untyped_numbers=allow_untyped_numbers,
                                             inverse_paths=inverse_paths)
 
+
 def _yielder_for_url_input(url_input, allow_untyped_numbers, raw_graph,
-                          input_format, namespaces_dict, list_of_url_input):
+                           input_format, namespaces_dict, list_of_url_input):
     if url_input:
         return RdflibParserTripleYielder(source=url_input,
                                          allow_untyped_numbers=allow_untyped_numbers,
                                          raw_graph=raw_graph,
                                          input_format=input_format,
                                          namespaces_dict=namespaces_dict)
     else:  # elif list_of_url_input:
         return MultiRdfLibTripleYielder(list_of_files=list_of_url_input,
                                         allow_untyped_numbers=allow_untyped_numbers,
                                         input_format=input_format,
                                         namespaces_dict=namespaces_dict)
 
+
 def _yielder_for_nt(source_file, raw_graph, allow_untyped_numbers,
                     list_of_source_files, compression_mode,
-                    zip_base_archive):
-    if (source_file is not None or raw_graph is not None) and zip_base_archive is None:
+                    zip_base_archives):
+    if (source_file is not None or raw_graph is not None) and zip_base_archives is None:
         return NtTriplesYielder(source_file=source_file,
                                 allow_untyped_numbers=allow_untyped_numbers,
                                 raw_graph=raw_graph,
                                 compression_mode=compression_mode)
-    elif zip_base_archive is not None:
-        return MultiNtTriplesYielder(list_of_files=list_of_zip_internal_files(zip_base_archive),
-                                     allow_untyped_numbers=allow_untyped_numbers,
-                                     compression_mode=compression_mode,
-                                     zip_base_archive=zip_base_archive)
+    elif zip_base_archives is not None:
+        # return MultiNtTriplesYielder(list_of_files=list_of_zip_internal_files(zip_base_archive),
+        #                              allow_untyped_numbers=allow_untyped_numbers,
+        #                              compression_mode=compression_mode,
+        #                              zip_base_archives=zip_base_archives)
+        return _yielder_for_compressed_inputs(
+            [MultiNtTriplesYielder(list_of_files=list_of_zip_internal_files(a_zip_file),
+                                   allow_untyped_numbers=allow_untyped_numbers,
+                                   compression_mode=compression_mode,
+                                   zip_base_archive=a_zip_file) for a_zip_file in zip_base_archives])
 
     else:
         return MultiNtTriplesYielder(list_of_files=list_of_source_files,
                                      allow_untyped_numbers=allow_untyped_numbers,
                                      compression_mode=compression_mode)
 
-def _get_base_zip_archive_if_needed(source_file, compression_mode):
+
+def _get_base_zip_archive_if_needed(source_file, list_of_source_files, compression_mode):
     if compression_mode != ZIP:
         return None
-    return ZipFile(source_file, 'r')
+    if source_file is not None:
+        return [ZipFile(source_file, 'r')]
+    result = []
+    for a_source_file in list_of_source_files:
+        result.append(ZipFile(a_source_file, 'r'))
+    return result
```

### Comparing `shexer-2.2.2/shexer/utils/namespaces.py` & `shexer-2.3.0/shexer/utils/namespaces.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,8 +13,8 @@
     candidate = get_random_string(3)
     while candidate in curr_prefixes:
         candidate = get_random_string(3)
     return candidate
 
 def get_random_string(length):
     result_str = ''.join(random.choice(string.ascii_lowercase) for i in range(length))
-    print("Random string of length", length, "is:", result_str)
+    return result_str
```

### Comparing `shexer-2.2.2/shexer/utils/obj_references.py` & `shexer-2.3.0/shexer/utils/obj_references.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/utils/shapes.py` & `shexer-2.3.0/shexer/utils/shapes.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/utils/target_elements.py` & `shexer-2.3.0/shexer/utils/target_elements.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/utils/translators/list_of_classes_to_shape_map.py` & `shexer-2.3.0/shexer/utils/translators/list_of_classes_to_shape_map.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/utils/triple_yielders.py` & `shexer-2.3.0/shexer/utils/triple_yielders.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer/utils/uri.py` & `shexer-2.3.0/shexer/utils/uri.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/shexer.egg-info/PKG-INFO` & `shexer-2.3.0/shexer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: shexer
-Version: 2.2.2
+Version: 2.3.0
 Summary: Automatic schema extraction for RDF graphs
 Home-page: https://github.com/DaniFdezAlvarez/shexer
-Download-URL: https://github.com/DaniFdezAlvarez/shexer/archive/2.2.2.tar.gz
+Download-URL: https://github.com/DaniFdezAlvarez/shexer/archive/2.3.0.tar.gz
 Author: Daniel Fernandez-Alvarez
 Author-email: danifdezalvarez@gmail.com
 Keywords: testing,shexer,shexerp3,rdf,shex,shacl,schema
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `shexer-2.2.2/shexer.egg-info/SOURCES.txt` & `shexer-2.3.0/shexer.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 local_code/__init__.py
 local_code/beyza_test.py
+local_code/img_example.py
 local_code/split_non_split_thats_the_question.py
 local_code/tictactoe.py
 local_code/whatever.py
 local_code/yasunori_Test.py
 shexer/__init__.py
 shexer/consts.py
 shexer/shaper.py
@@ -61,14 +62,15 @@
 shexer/io/graph/yielder/__init__.py
 shexer/io/graph/yielder/base_triples_yielder.py
 shexer/io/graph/yielder/big_ttl_triples_yielder.py
 shexer/io/graph/yielder/multi_big_ttl_files_triple_yielder.py
 shexer/io/graph/yielder/multi_nt_triples_yielder.py
 shexer/io/graph/yielder/multi_rdflib_triple_yielder.py
 shexer/io/graph/yielder/multi_tsv_nt_triples_yielder.py
+shexer/io/graph/yielder/multi_zip_triples_yielder.py
 shexer/io/graph/yielder/multifile_base_triples_yielder.py
 shexer/io/graph/yielder/nt_triples_yielder.py
 shexer/io/graph/yielder/rdflib_triple_yielder.py
 shexer/io/graph/yielder/tsv_nt_triples_yielder.py
 shexer/io/graph/yielder/filter/__init__.py
 shexer/io/graph/yielder/filter/filter_namespaces_triple_yielder.py
 shexer/io/graph/yielder/remote/__init__.py
```

### Comparing `shexer-2.2.2/test/const.py` & `shexer-2.3.0/test/const.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/test/t_utils.py` & `shexer-2.3.0/test/t_utils.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/test/test_all_classes_mode.py` & `shexer-2.3.0/test/test_all_classes_mode.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/test/test_allow_opt_cardinality.py` & `shexer-2.3.0/test/test_allow_opt_cardinality.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/test/test_allow_redundant_or.py` & `shexer-2.3.0/test/test_allow_redundant_or.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/test/test_bugs/test_no_sharp_in_auto_shape_names.py` & `shexer-2.3.0/test/test_bugs/test_no_sharp_in_auto_shape_names.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/test/test_bugs/test_no_sharp_nor_slash_due_to_prefixing.py` & `shexer-2.3.0/test/test_bugs/test_no_sharp_nor_slash_due_to_prefixing.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/test/test_compression_mode.py` & `shexer-2.3.0/test/test_compression_mode.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 
 
 _BASE_DIR = BASE_FILES + "compression" + pth.sep
 
 
 class TestCompressionMode(unittest.TestCase):
 
+    ######################### GZ
+
     def test_ttl_iter_gz(self):
         shaper = Shaper(
             graph_file_input=_BASE_DIR + "t_graph_1.ttl.gz",
             namespaces_dict=default_namespaces(),
             all_classes_mode=True,
             input_format=TURTLE_ITER,
             disable_comments=True,
@@ -230,7 +232,39 @@
                             all_classes_mode=False,
                             compression_mode=ZIP)
             self.fail("It should allow to use compression with a remote source")
         except ValueError:
             pass
         except:
             self.fail("The exception should be a ValueError")
+
+
+    ##################### SEVERAL FILES IN ZIP
+
+    def test_nt_zip(self):
+        shaper = Shaper(
+            graph_file_input=_BASE_DIR + "t1_graph_partials_1_2_3__3.nt.zip",
+            namespaces_dict=default_namespaces(),
+            all_classes_mode=True,
+            input_format=NT,
+            disable_comments=True,
+            compression_mode=ZIP
+        )
+        str_result = shaper.shex_graph(string_output=True)
+        self.assertTrue(file_vs_str_tunned_comparison(file_path=G1_ALL_CLASSES_NO_COMMENTS,
+                                                      str_target=str_result))
+
+    ##################### SEVERAL ZIPS
+
+    def test_nt_zip(self):
+        shaper = Shaper(
+            graph_list_of_files_input=[_BASE_DIR + "t1_graph_partials_1_2__3.nt.zip",
+                                       _BASE_DIR + "t1_graph_partials_3__3.nt.zip"],
+            namespaces_dict=default_namespaces(),
+            all_classes_mode=True,
+            input_format=NT,
+            disable_comments=True,
+            compression_mode=ZIP
+        )
+        str_result = shaper.shex_graph(string_output=True)
+        self.assertTrue(file_vs_str_tunned_comparison(file_path=G1_ALL_CLASSES_NO_COMMENTS,
+                                                      str_target=str_result))
```

### Comparing `shexer-2.2.2/test/test_decimals.py` & `shexer-2.3.0/test/test_decimals.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/test/test_depth_for_building_subgraph.py` & `shexer-2.3.0/test/test_depth_for_building_subgraph.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/test/test_detect_minimal_iri.py` & `shexer-2.3.0/test/test_detect_minimal_iri.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/test/test_disable_comments.py` & `shexer-2.3.0/test/test_disable_comments.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/test/test_disable_endpoint_cache.py` & `shexer-2.3.0/test/test_disable_endpoint_cache.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/test/test_disable_exact_cardinality.py` & `shexer-2.3.0/test/test_disable_exact_cardinality.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/test/test_disable_or_statements.py` & `shexer-2.3.0/test/test_disable_or_statements.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/test/test_discard_and_compliant.py` & `shexer-2.3.0/test/test_discard_and_compliant.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/test/test_file_target_classes.py` & `shexer-2.3.0/test/test_file_target_classes.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/test/test_graph_file_input.py` & `shexer-2.3.0/test/test_graph_file_input.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/test/test_graph_list_of_file_inputs.py` & `shexer-2.3.0/test/test_graph_list_of_file_inputs.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/test/test_infer_numeric_types_for_untyped_literals.py` & `shexer-2.3.0/test/test_infer_numeric_types_for_untyped_literals.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/test/test_input_format.py` & `shexer-2.3.0/test/test_input_format.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/test/test_instances_cap.py` & `shexer-2.3.0/test/test_instances_cap.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/test/test_instances_file_input.py` & `shexer-2.3.0/test/test_instances_file_input.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/test/test_instances_report.py` & `shexer-2.3.0/test/test_instances_report.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/test/test_instantiation_property.py` & `shexer-2.3.0/test/test_instantiation_property.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/test/test_inverse_paths.py` & `shexer-2.3.0/test/test_inverse_paths.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/test/test_keep_less_specific.py` & `shexer-2.3.0/test/test_keep_less_specific.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/test/test_list_of_url_input.py` & `shexer-2.3.0/test/test_list_of_url_input.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/test/test_namespaces_dict.py` & `shexer-2.3.0/test/test_namespaces_dict.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/test/test_namespaces_to_ignore.py` & `shexer-2.3.0/test/test_namespaces_to_ignore.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/test/test_raw_graph.py` & `shexer-2.3.0/test/test_raw_graph.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/test/test_raw_shape_map.py` & `shexer-2.3.0/test/test_raw_shape_map.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/test/test_rdflib_graph.py` & `shexer-2.3.0/test/test_rdflib_graph.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/test/test_remove_empty_sahpes.py` & `shexer-2.3.0/test/test_remove_empty_sahpes.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/test/test_shacl/test_annotation.py` & `shexer-2.3.0/test/test_shacl/test_annotation.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/test/test_shacl/test_class_selection.py` & `shexer-2.3.0/test/test_shacl/test_class_selection.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/test/test_shacl/test_detect_minimal_iri.py` & `shexer-2.3.0/test/test_shacl/test_detect_minimal_iri.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/test/test_shacl/test_https.py` & `shexer-2.3.0/test/test_shacl/test_https.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/test/test_shacl/test_literal_types.py` & `shexer-2.3.0/test/test_shacl/test_literal_types.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/test/test_shape_map_file.py` & `shexer-2.3.0/test/test_shape_map_file.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/test/test_shape_map_format.py` & `shexer-2.3.0/test/test_shape_map_format.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/test/test_shape_qualifiers_mode.py` & `shexer-2.3.0/test/test_shape_qualifiers_mode.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/test/test_shapes_namespaces.py` & `shexer-2.3.0/test/test_shapes_namespaces.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/test/test_sort.py` & `shexer-2.3.0/test/test_sort.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/test/test_target_classes.py` & `shexer-2.3.0/test/test_target_classes.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/test/test_threshold.py` & `shexer-2.3.0/test/test_threshold.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/test/test_url_endpoint.py` & `shexer-2.3.0/test/test_url_endpoint.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/test/test_url_graph.py` & `shexer-2.3.0/test/test_url_graph.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/test/test_wikidata_annotation.py` & `shexer-2.3.0/test/test_wikidata_annotation.py`

 * *Files identical despite different names*

### Comparing `shexer-2.2.2/ws/shexer_rest.py` & `shexer-2.3.0/ws/shexer_rest.py`

 * *Files identical despite different names*

