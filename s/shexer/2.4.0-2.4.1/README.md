# Comparing `tmp/shexer-2.4.0.tar.gz` & `tmp/shexer-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shexer-2.4.0.tar", last modified: Fri Apr  5 16:49:50 2024, max compression
+gzip compressed data, was "shexer-2.4.1.tar", last modified: Thu May  2 11:36:41 2024, max compression
```

## Comparing `shexer-2.4.0.tar` & `shexer-2.4.1.tar`

### file list

```diff
@@ -1,256 +1,253 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 16:49:50.232527 shexer-2.4.0/
--rw-rw-rw-   0        0        0    11558 2023-06-27 16:13:11.000000 shexer-2.4.0/LICENSE
--rw-rw-rw-   0        0        0    27740 2024-04-05 16:49:50.233523 shexer-2.4.0/PKG-INFO
--rw-rw-rw-   0        0        0    26865 2024-04-05 16:49:28.000000 shexer-2.4.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-05 16:49:48.504761 shexer-2.4.0/local_code/
--rw-rw-rw-   0        0        0        0 2023-07-20 16:50:30.000000 shexer-2.4.0/local_code/__init__.py
--rw-rw-rw-   0        0        0     1278 2023-11-10 20:18:22.000000 shexer-2.4.0/local_code/beyza_test.py
--rw-rw-rw-   0        0        0     1411 2023-11-30 17:16:03.000000 shexer-2.4.0/local_code/img_example.py
--rw-rw-rw-   0        0        0     2756 2023-09-04 15:19:36.000000 shexer-2.4.0/local_code/split_non_split_thats_the_question.py
--rw-rw-rw-   0        0        0     9733 2023-11-08 19:45:06.000000 shexer-2.4.0/local_code/tictactoe.py
--rw-rw-rw-   0        0        0       88 2023-11-13 10:50:47.000000 shexer-2.4.0/local_code/whatever.py
--rw-rw-rw-   0        0        0     1428 2023-10-02 17:19:16.000000 shexer-2.4.0/local_code/yasunori_Test.py
--rw-rw-rw-   0        0        0       86 2024-04-05 16:49:50.236516 shexer-2.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1370 2024-04-05 16:49:28.000000 shexer-2.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-05 16:49:48.511716 shexer-2.4.0/shexer/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/__init__.py
--rw-rw-rw-   0        0        0      713 2024-04-05 16:49:28.000000 shexer-2.4.0/shexer/consts.py
-drwxrwxrwx   0        0        0        0 2024-04-05 16:49:48.554611 shexer-2.4.0/shexer/core/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 16:49:48.577540 shexer-2.4.0/shexer/core/instances/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/instances/__init__.py
--rw-rw-rw-   0        0        0      713 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/instances/abstract_instance_tracker.py
-drwxrwxrwx   0        0        0        0 2024-04-05 16:49:48.610452 shexer-2.4.0/shexer/core/instances/annotators/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/instances/annotators/__init__.py
--rw-rw-rw-   0        0        0      383 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/instances/annotators/annotator_func.py
--rw-rw-rw-   0        0        0     1817 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/instances/annotators/annotator_tracking_instances.py
--rw-rw-rw-   0        0        0     3895 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/instances/annotators/base_annotator.py
-drwxrwxrwx   0        0        0        0 2024-04-05 16:49:48.689272 shexer-2.4.0/shexer/core/instances/annotators/strategy_mode/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/instances/annotators/strategy_mode/__init__.py
--rw-rw-rw-   0        0        0      665 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/instances/annotators/strategy_mode/all_classes_mode.py
--rw-rw-rw-   0        0        0      760 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/instances/annotators/strategy_mode/base_strategy_mode.py
--rw-rw-rw-   0        0        0      807 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/instances/annotators/strategy_mode/compound_strategy_mode.py
--rw-rw-rw-   0        0        0     2675 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/instances/annotators/strategy_mode/instance_cap_mode.py
--rw-rw-rw-   0        0        0       86 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/instances/annotators/strategy_mode/instances_cap_exception.py
--rw-rw-rw-   0        0        0     1793 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/instances/annotators/strategy_mode/shape_qualifiers_mode.py
--rw-rw-rw-   0        0        0      815 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/instances/annotators/strategy_mode/target_classes_mode.py
--rw-rw-rw-   0        0        0     4553 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/instances/instance_tracker.py
-drwxrwxrwx   0        0        0        0 2024-04-05 16:49:48.700220 shexer-2.4.0/shexer/core/instances/mappings/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/instances/mappings/__init__.py
--rw-rw-rw-   0        0        0     1081 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/instances/mappings/shape_map_instance_tracker.py
-drwxrwxrwx   0        0        0        0 2024-04-05 16:49:48.712226 shexer-2.4.0/shexer/core/instances/mix/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/instances/mix/__init__.py
--rw-rw-rw-   0        0        0     2652 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/instances/mix/mixed_instance_tracker.py
--rw-rw-rw-   0        0        0       22 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/instances/pconsts.py
-drwxrwxrwx   0        0        0        0 2024-04-05 16:49:48.737144 shexer-2.4.0/shexer/core/profiling/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/profiling/__init__.py
--rw-rw-rw-   0        0        0     8613 2023-10-20 16:00:26.000000 shexer-2.4.0/shexer/core/profiling/class_profiler.py
--rw-rw-rw-   0        0        0      182 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/profiling/consts.py
-drwxrwxrwx   0        0        0        0 2024-04-05 16:49:48.774024 shexer-2.4.0/shexer/core/profiling/strategy/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/profiling/strategy/__init__.py
--rw-rw-rw-   0        0        0     6976 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/profiling/strategy/abstract_feature_direction_strategy.py
--rw-rw-rw-   0        0        0     1349 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/profiling/strategy/direct_features_strategy.py
--rw-rw-rw-   0        0        0     7395 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/profiling/strategy/include_reverse_features_strategy.py
-drwxrwxrwx   0        0        0        0 2024-04-05 16:49:48.786988 shexer-2.4.0/shexer/core/shexing/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/shexing/__init__.py
--rw-rw-rw-   0        0        0     6186 2023-10-20 16:00:26.000000 shexer-2.4.0/shexer/core/shexing/class_shexer.py
-drwxrwxrwx   0        0        0        0 2024-04-05 16:49:48.822929 shexer-2.4.0/shexer/core/shexing/strategy/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/shexing/strategy/__init__.py
--rw-rw-rw-   0        0        0    17141 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/shexing/strategy/abstract_shexing_strategy.py
--rw-rw-rw-   0        0        0     5685 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/shexing/strategy/direct_and_inverse_shexing_strategy.py
--rw-rw-rw-   0        0        0     2804 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/shexing/strategy/direct_shexing_strategy.py
-drwxrwxrwx   0        0        0        0 2024-04-05 16:49:48.855806 shexer-2.4.0/shexer/core/shexing/strategy/minimal_iri_strategy/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/shexing/strategy/minimal_iri_strategy/__init__.py
--rw-rw-rw-   0        0        0      118 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/shexing/strategy/minimal_iri_strategy/abstract_min_iri_strategy.py
--rw-rw-rw-   0        0        0     1088 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/shexing/strategy/minimal_iri_strategy/annotate_min_iri_strategy.py
--rw-rw-rw-   0        0        0      412 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/core/shexing/strategy/minimal_iri_strategy/ignore_min_iri_strategy.py
-drwxrwxrwx   0        0        0        0 2024-04-05 16:49:48.875752 shexer-2.4.0/shexer/io/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/__init__.py
--rw-rw-rw-   0        0        0      103 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/file.py
-drwxrwxrwx   0        0        0        0 2024-04-05 16:49:48.877745 shexer-2.4.0/shexer/io/graph/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/graph/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 16:49:48.996509 shexer-2.4.0/shexer/io/graph/yielder/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/graph/yielder/__init__.py
--rw-rw-rw-   0        0        0     1431 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/graph/yielder/base_triples_yielder.py
--rw-rw-rw-   0        0        0    16304 2023-10-20 16:00:26.000000 shexer-2.4.0/shexer/io/graph/yielder/big_ttl_triples_yielder.py
-drwxrwxrwx   0        0        0        0 2024-04-05 16:49:49.008477 shexer-2.4.0/shexer/io/graph/yielder/filter/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/graph/yielder/filter/__init__.py
--rw-rw-rw-   0        0        0      862 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/graph/yielder/filter/filter_namespaces_triple_yielder.py
--rw-rw-rw-   0        0        0     1131 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/graph/yielder/multi_big_ttl_files_triple_yielder.py
--rw-rw-rw-   0        0        0     1132 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/graph/yielder/multi_nt_triples_yielder.py
--rw-rw-rw-   0        0        0     1757 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/graph/yielder/multi_rdflib_triple_yielder.py
--rw-rw-rw-   0        0        0     1166 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/graph/yielder/multi_tsv_nt_triples_yielder.py
--rw-rw-rw-   0        0        0     1483 2024-04-03 12:10:04.000000 shexer-2.4.0/shexer/io/graph/yielder/multi_zip_triples_yielder.py
--rw-rw-rw-   0        0        0     2670 2024-04-03 12:10:04.000000 shexer-2.4.0/shexer/io/graph/yielder/multifile_base_triples_yielder.py
--rw-rw-rw-   0        0        0     5686 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/graph/yielder/nt_triples_yielder.py
--rw-rw-rw-   0        0        0     6817 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/graph/yielder/rdflib_triple_yielder.py
-drwxrwxrwx   0        0        0        0 2024-04-05 16:49:49.023474 shexer-2.4.0/shexer/io/graph/yielder/remote/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/graph/yielder/remote/__init__.py
--rw-rw-rw-   0        0        0     3826 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/graph/yielder/remote/sgraph_from_selectors_triple_yielder.py
--rw-rw-rw-   0        0        0     4724 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/graph/yielder/tsv_nt_triples_yielder.py
-drwxrwxrwx   0        0        0        0 2024-04-05 16:49:49.034444 shexer-2.4.0/shexer/io/json/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/json/__init__.py
--rw-rw-rw-   0        0        0      207 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/json/json_loader.py
-drwxrwxrwx   0        0        0        0 2024-04-05 16:49:49.070349 shexer-2.4.0/shexer/io/line_reader/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/line_reader/__init__.py
--rw-rw-rw-   0        0        0      285 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/line_reader/file_line_reader.py
--rw-rw-rw-   0        0        0      332 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/line_reader/gz_line_reader.py
--rw-rw-rw-   0        0        0      260 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/line_reader/raw_string_line_reader.py
--rw-rw-rw-   0        0        0      353 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/line_reader/zip_file_line_reader.py
-drwxrwxrwx   0        0        0        0 2024-04-05 16:49:49.072322 shexer-2.4.0/shexer/io/profile/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/profile/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 16:49:49.077299 shexer-2.4.0/shexer/io/profile/formater/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/profile/formater/__init__.py
--rw-rw-rw-   0        0        0      409 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/profile/formater/abstract_profile_serializer.py
-drwxrwxrwx   0        0        0        0 2024-04-05 16:49:49.079288 shexer-2.4.0/shexer/io/shacl/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/shacl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 16:49:49.091256 shexer-2.4.0/shexer/io/shacl/formater/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/shacl/formater/__init__.py
--rw-rw-rw-   0        0        0    16449 2023-11-10 20:24:47.000000 shexer-2.4.0/shexer/io/shacl/formater/shacl_serializer.py
-drwxrwxrwx   0        0        0        0 2024-04-05 16:49:49.105256 shexer-2.4.0/shexer/io/shape_map/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/shape_map/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 16:49:49.117186 shexer-2.4.0/shexer/io/shape_map/label/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/shape_map/label/__init__.py
--rw-rw-rw-   0        0        0     1410 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/shape_map/label/shape_map_label_parser.py
-drwxrwxrwx   0        0        0        0 2024-04-05 16:49:49.135177 shexer-2.4.0/shexer/io/shape_map/node_selector/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/shape_map/node_selector/__init__.py
--rw-rw-rw-   0        0        0     6755 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/shape_map/node_selector/node_selector_parser.py
--rw-rw-rw-   0        0        0     4966 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/shape_map/shape_map_parser.py
-drwxrwxrwx   0        0        0        0 2024-04-05 16:49:49.139156 shexer-2.4.0/shexer/io/shex/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/shex/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 16:49:49.160118 shexer-2.4.0/shexer/io/shex/formater/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/shex/formater/__init__.py
--rw-rw-rw-   0        0        0      244 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/shex/formater/consts.py
--rw-rw-rw-   0        0        0     7006 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/shex/formater/shex_serializer.py
-drwxrwxrwx   0        0        0        0 2024-04-05 16:49:49.211973 shexer-2.4.0/shexer/io/shex/formater/statement_serializers/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/shex/formater/statement_serializers/__init__.py
--rw-rw-rw-   0        0        0     6083 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/shex/formater/statement_serializers/base_statement_serializer.py
--rw-rw-rw-   0        0        0     2287 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/shex/formater/statement_serializers/fixed_prop_choice_statement_serializer.py
-drwxrwxrwx   0        0        0        0 2024-04-05 16:49:49.262874 shexer-2.4.0/shexer/io/shex/formater/statement_serializers/frequency_strategy/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/shex/formater/statement_serializers/frequency_strategy/__init__.py
--rw-rw-rw-   0        0        0      383 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/shex/formater/statement_serializers/frequency_strategy/abs_freq_serializer.py
--rw-rw-rw-   0        0        0      171 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/shex/formater/statement_serializers/frequency_strategy/base_frequency_strategy.py
--rw-rw-rw-   0        0        0      887 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/shex/formater/statement_serializers/frequency_strategy/mixed_frequency_strategy.py
--rw-rw-rw-   0        0        0     1278 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/shex/formater/statement_serializers/frequency_strategy/ratio_freq_serializer.py
--rw-rw-rw-   0        0        0     1500 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/shex/formater/statement_serializers/inverse_statement_serializer.py
--rw-rw-rw-   0        0        0     3211 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/shex/formater/statement_serializers/st_serializers_factory.py
-drwxrwxrwx   0        0        0        0 2024-04-05 16:49:49.268820 shexer-2.4.0/shexer/io/sparql/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/sparql/__init__.py
--rw-rw-rw-   0        0        0     4538 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/sparql/query.py
-drwxrwxrwx   0        0        0        0 2024-04-05 16:49:49.273807 shexer-2.4.0/shexer/io/uml/
--rw-rw-rw-   0        0        0        0 2024-04-05 16:49:28.000000 shexer-2.4.0/shexer/io/uml/__init__.py
--rw-rw-rw-   0        0        0     6256 2024-04-05 16:49:28.000000 shexer-2.4.0/shexer/io/uml/uml_serializer.py
--rw-rw-rw-   0        0        0      469 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/io/wikidata.py
-drwxrwxrwx   0        0        0        0 2024-04-05 16:49:49.383542 shexer-2.4.0/shexer/model/
--rw-rw-rw-   0        0        0      552 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/model/IRI.py
--rw-rw-rw-   0        0        0      280 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/model/Literal.py
--rw-rw-rw-   0        0        0      810 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/model/Macro.py
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/model/__init__.py
--rw-rw-rw-   0        0        0      502 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/model/bnode.py
--rw-rw-rw-   0        0        0      100 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/model/const_elem_types.py
--rw-rw-rw-   0        0        0     1119 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/model/fixed_prop_choice_statement.py
-drwxrwxrwx   0        0        0        0 2024-04-05 16:49:49.403500 shexer-2.4.0/shexer/model/graph/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/model/graph/__init__.py
--rw-rw-rw-   0        0        0     6186 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/model/graph/abstract_sgraph.py
--rw-rw-rw-   0        0        0     7633 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/model/graph/endpoint_sgraph.py
--rw-rw-rw-   0        0        0     6201 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/model/graph/rdflib_sgraph.py
--rw-rw-rw-   0        0        0     4173 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/model/hierarchy_tree.py
--rw-rw-rw-   0        0        0     2527 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/model/node_selector.py
--rw-rw-rw-   0        0        0      427 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/model/property.py
--rw-rw-rw-   0        0        0     3361 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/model/shape.py
--rw-rw-rw-   0        0        0      858 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/model/shape_map.py
--rw-rw-rw-   0        0        0     2716 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/model/statement.py
--rw-rw-rw-   0        0        0    25844 2024-04-05 16:49:28.000000 shexer-2.4.0/shexer/shaper.py
-drwxrwxrwx   0        0        0        0 2024-04-05 16:49:49.486249 shexer-2.4.0/shexer/utils/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/utils/__init__.py
--rw-rw-rw-   0        0        0      621 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/utils/compression.py
--rw-rw-rw-   0        0        0       94 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/utils/dict.py
-drwxrwxrwx   0        0        0        0 2024-04-05 16:49:49.588078 shexer-2.4.0/shexer/utils/factories/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/utils/factories/__init__.py
--rw-rw-rw-   0        0        0     4300 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/utils/factories/class_profiler_factory.py
--rw-rw-rw-   0        0        0     2322 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/utils/factories/class_shexer_factory.py
--rw-rw-rw-   0        0        0      728 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/utils/factories/h_tree.py
--rw-rw-rw-   0        0        0    12338 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/utils/factories/instance_tracker_factory.py
--rw-rw-rw-   0        0        0      437 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/utils/factories/iri_factory.py
--rw-rw-rw-   0        0        0      286 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/utils/factories/remote_graph_factory.py
--rw-rw-rw-   0        0        0     1985 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/utils/factories/shape_map_factory.py
--rw-rw-rw-   0        0        0      616 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/utils/factories/shape_map_parser_factory.py
--rw-rw-rw-   0        0        0     2109 2024-04-05 16:49:28.000000 shexer-2.4.0/shexer/utils/factories/shape_serializer_factory.py
--rw-rw-rw-   0        0        0    21108 2024-04-03 12:10:04.000000 shexer-2.4.0/shexer/utils/factories/triple_yielders_factory.py
--rw-rw-rw-   0        0        0      123 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/utils/file.py
--rw-rw-rw-   0        0        0      397 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/utils/log.py
--rw-rw-rw-   0        0        0      761 2024-04-05 16:49:28.000000 shexer-2.4.0/shexer/utils/namespaces.py
--rw-rw-rw-   0        0        0      967 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/utils/obj_references.py
--rw-rw-rw-   0        0        0     2008 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/utils/shapes.py
--rw-rw-rw-   0        0        0     1397 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/utils/target_elements.py
-drwxrwxrwx   0        0        0        0 2024-04-05 16:49:49.601024 shexer-2.4.0/shexer/utils/translators/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/utils/translators/__init__.py
--rw-rw-rw-   0        0        0     2881 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/utils/translators/list_of_classes_to_shape_map.py
--rw-rw-rw-   0        0        0     3026 2023-06-27 16:13:11.000000 shexer-2.4.0/shexer/utils/triple_yielders.py
--rw-rw-rw-   0        0        0     5749 2024-04-05 16:49:28.000000 shexer-2.4.0/shexer/utils/uri.py
-drwxrwxrwx   0        0        0        0 2024-04-05 16:49:48.551609 shexer-2.4.0/shexer.egg-info/
--rw-rw-rw-   0        0        0    27740 2024-04-05 16:49:48.000000 shexer-2.4.0/shexer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     8346 2024-04-05 16:49:48.000000 shexer-2.4.0/shexer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 16:49:48.000000 shexer-2.4.0/shexer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2024-04-05 16:49:48.000000 shexer-2.4.0/shexer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-04-05 16:49:48.000000 shexer-2.4.0/shexer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-05 16:49:50.130805 shexer-2.4.0/test/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/test/__init__.py
--rw-rw-rw-   0        0        0     1903 2023-06-27 16:13:11.000000 shexer-2.4.0/test/const.py
--rw-rw-rw-   0        0        0     9389 2024-04-05 16:49:28.000000 shexer-2.4.0/test/t_utils.py
--rw-rw-rw-   0        0        0     1488 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_all_classes_mode.py
--rw-rw-rw-   0        0        0     1525 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_allow_opt_cardinality.py
--rw-rw-rw-   0        0        0     3541 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_allow_redundant_or.py
-drwxrwxrwx   0        0        0        0 2024-04-05 16:49:50.158753 shexer-2.4.0/test/test_bugs/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_bugs/__init__.py
--rw-rw-rw-   0        0        0      796 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_bugs/test_no_sharp_in_auto_shape_names.py
--rw-rw-rw-   0        0        0     1192 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_bugs/test_no_sharp_nor_slash_due_to_prefixing.py
--rw-rw-rw-   0        0        0    11274 2024-04-03 12:10:04.000000 shexer-2.4.0/test/test_compression_mode.py
--rw-rw-rw-   0        0        0     2171 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_decimals.py
--rw-rw-rw-   0        0        0     5564 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_depth_for_building_subgraph.py
--rw-rw-rw-   0        0        0     3526 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_detect_minimal_iri.py
--rw-rw-rw-   0        0        0     1388 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_disable_comments.py
--rw-rw-rw-   0        0        0     2922 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_disable_endpoint_cache.py
--rw-rw-rw-   0        0        0     1491 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_disable_exact_cardinality.py
--rw-rw-rw-   0        0        0     2557 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_disable_or_statements.py
--rw-rw-rw-   0        0        0     3786 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_discard_and_compliant.py
--rw-rw-rw-   0        0        0     2090 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_file_target_classes.py
--rw-rw-rw-   0        0        0     1677 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_graph_file_input.py
--rw-rw-rw-   0        0        0     3456 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_graph_list_of_file_inputs.py
--rw-rw-rw-   0        0        0     1951 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_infer_numeric_types_for_untyped_literals.py
--rw-rw-rw-   0        0        0     7818 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_input_format.py
--rw-rw-rw-   0        0        0     4648 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_instances_cap.py
--rw-rw-rw-   0        0        0     3367 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_instances_file_input.py
--rw-rw-rw-   0        0        0     3852 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_instances_report.py
--rw-rw-rw-   0        0        0     3548 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_instantiation_property.py
--rw-rw-rw-   0        0        0     1964 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_inverse_paths.py
--rw-rw-rw-   0        0        0     3594 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_keep_less_specific.py
--rw-rw-rw-   0        0        0     4051 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_list_of_url_input.py
--rw-rw-rw-   0        0        0     4106 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_namespaces_dict.py
--rw-rw-rw-   0        0        0     2082 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_namespaces_to_ignore.py
--rw-rw-rw-   0        0        0     5000 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_raw_graph.py
--rw-rw-rw-   0        0        0     4300 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_raw_shape_map.py
--rw-rw-rw-   0        0        0     1711 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_rdflib_graph.py
--rw-rw-rw-   0        0        0     2932 2023-10-20 16:00:26.000000 shexer-2.4.0/test/test_remove_empty_sahpes.py
-drwxrwxrwx   0        0        0        0 2024-04-05 16:49:50.209586 shexer-2.4.0/test/test_shacl/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_shacl/__init__.py
--rw-rw-rw-   0        0        0     2225 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_shacl/test_annotation.py
--rw-rw-rw-   0        0        0     2242 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_shacl/test_class_selection.py
--rw-rw-rw-   0        0        0     3291 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_shacl/test_detect_minimal_iri.py
--rw-rw-rw-   0        0        0      875 2023-11-10 20:24:47.000000 shexer-2.4.0/test/test_shacl/test_https.py
--rw-rw-rw-   0        0        0     1534 2023-11-10 20:24:47.000000 shexer-2.4.0/test/test_shacl/test_literal_types.py
--rw-rw-rw-   0        0        0     4313 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_shape_map_file.py
--rw-rw-rw-   0        0        0     6086 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_shape_map_format.py
--rw-rw-rw-   0        0        0     2307 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_shape_qualifiers_mode.py
--rw-rw-rw-   0        0        0     2889 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_shapes_namespaces.py
--rw-rw-rw-   0        0        0     2452 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_sort.py
--rw-rw-rw-   0        0        0     2058 2023-10-20 15:05:20.000000 shexer-2.4.0/test/test_target_classes.py
--rw-rw-rw-   0        0        0     3120 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_threshold.py
--rw-rw-rw-   0        0        0     2729 2024-04-05 16:49:28.000000 shexer-2.4.0/test/test_uml_gen.py
--rw-rw-rw-   0        0        0     2578 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_url_endpoint.py
--rw-rw-rw-   0        0        0     1867 2023-06-27 16:13:11.000000 shexer-2.4.0/test/test_url_graph.py
--rw-rw-rw-   0        0        0     1931 2024-04-05 16:49:28.000000 shexer-2.4.0/test/test_wikidata_annotation.py
-drwxrwxrwx   0        0        0        0 2024-04-05 16:49:50.230531 shexer-2.4.0/ws/
--rw-rw-rw-   0        0        0        0 2023-06-27 16:13:11.000000 shexer-2.4.0/ws/__init__.py
--rw-rw-rw-   0        0        0    19884 2023-06-27 16:13:11.000000 shexer-2.4.0/ws/shexer_rest.py
--rw-rw-rw-   0        0        0       28 2023-06-27 16:13:11.000000 shexer-2.4.0/ws/wsgi.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:36:41.509736 shexer-2.4.1/
+-rw-rw-rw-   0        0        0    11558 2023-01-30 11:26:57.000000 shexer-2.4.1/LICENSE
+-rw-rw-rw-   0        0        0    27781 2024-05-02 11:36:41.509736 shexer-2.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0    26865 2024-05-02 10:31:57.000000 shexer-2.4.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-02 11:36:40.569297 shexer-2.4.1/local_code/
+-rw-rw-rw-   0        0        0        0 2023-06-13 16:22:19.000000 shexer-2.4.1/local_code/__init__.py
+-rw-rw-rw-   0        0        0     2925 2023-10-20 11:37:58.000000 shexer-2.4.1/local_code/anything_shex_allclasses.py
+-rw-rw-rw-   0        0        0     4424 2023-11-14 11:54:22.000000 shexer-2.4.1/local_code/aventura_ruben.py
+-rw-rw-rw-   0        0        0     3252 2023-06-13 16:23:19.000000 shexer-2.4.1/local_code/yy_test.py
+-rw-rw-rw-   0        0        0       86 2024-05-02 11:36:41.514270 shexer-2.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     1393 2024-05-02 11:22:19.000000 shexer-2.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:36:40.571737 shexer-2.4.1/shexer/
+-rw-rw-rw-   0        0        0        0 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/__init__.py
+-rw-rw-rw-   0        0        0      713 2024-05-02 10:31:57.000000 shexer-2.4.1/shexer/consts.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:36:40.594146 shexer-2.4.1/shexer/core/
+-rw-rw-rw-   0        0        0        0 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/core/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:36:40.606215 shexer-2.4.1/shexer/core/instances/
+-rw-rw-rw-   0        0        0        0 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/core/instances/__init__.py
+-rw-rw-rw-   0        0        0      713 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/core/instances/abstract_instance_tracker.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:36:40.626037 shexer-2.4.1/shexer/core/instances/annotators/
+-rw-rw-rw-   0        0        0        0 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/core/instances/annotators/__init__.py
+-rw-rw-rw-   0        0        0      383 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/core/instances/annotators/annotator_func.py
+-rw-rw-rw-   0        0        0     1817 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/core/instances/annotators/annotator_tracking_instances.py
+-rw-rw-rw-   0        0        0     3895 2023-06-13 16:20:36.000000 shexer-2.4.1/shexer/core/instances/annotators/base_annotator.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:36:40.669546 shexer-2.4.1/shexer/core/instances/annotators/strategy_mode/
+-rw-rw-rw-   0        0        0        0 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/core/instances/annotators/strategy_mode/__init__.py
+-rw-rw-rw-   0        0        0      665 2023-06-13 16:20:36.000000 shexer-2.4.1/shexer/core/instances/annotators/strategy_mode/all_classes_mode.py
+-rw-rw-rw-   0        0        0      760 2023-06-13 16:20:36.000000 shexer-2.4.1/shexer/core/instances/annotators/strategy_mode/base_strategy_mode.py
+-rw-rw-rw-   0        0        0      807 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/core/instances/annotators/strategy_mode/compound_strategy_mode.py
+-rw-rw-rw-   0        0        0     2675 2023-06-13 16:20:36.000000 shexer-2.4.1/shexer/core/instances/annotators/strategy_mode/instance_cap_mode.py
+-rw-rw-rw-   0        0        0       86 2023-06-13 16:20:36.000000 shexer-2.4.1/shexer/core/instances/annotators/strategy_mode/instances_cap_exception.py
+-rw-rw-rw-   0        0        0     1793 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/core/instances/annotators/strategy_mode/shape_qualifiers_mode.py
+-rw-rw-rw-   0        0        0      815 2023-06-13 16:20:36.000000 shexer-2.4.1/shexer/core/instances/annotators/strategy_mode/target_classes_mode.py
+-rw-rw-rw-   0        0        0     4553 2023-06-13 16:20:36.000000 shexer-2.4.1/shexer/core/instances/instance_tracker.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:36:40.676623 shexer-2.4.1/shexer/core/instances/mappings/
+-rw-rw-rw-   0        0        0        0 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/core/instances/mappings/__init__.py
+-rw-rw-rw-   0        0        0     1081 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/core/instances/mappings/shape_map_instance_tracker.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:36:40.683168 shexer-2.4.1/shexer/core/instances/mix/
+-rw-rw-rw-   0        0        0        0 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/core/instances/mix/__init__.py
+-rw-rw-rw-   0        0        0     2652 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/core/instances/mix/mixed_instance_tracker.py
+-rw-rw-rw-   0        0        0       22 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/core/instances/pconsts.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:36:40.694991 shexer-2.4.1/shexer/core/profiling/
+-rw-rw-rw-   0        0        0        0 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/core/profiling/__init__.py
+-rw-rw-rw-   0        0        0     8613 2023-10-20 11:58:54.000000 shexer-2.4.1/shexer/core/profiling/class_profiler.py
+-rw-rw-rw-   0        0        0      182 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/core/profiling/consts.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:36:40.724771 shexer-2.4.1/shexer/core/profiling/strategy/
+-rw-rw-rw-   0        0        0        0 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/core/profiling/strategy/__init__.py
+-rw-rw-rw-   0        0        0     6976 2023-05-03 10:30:03.000000 shexer-2.4.1/shexer/core/profiling/strategy/abstract_feature_direction_strategy.py
+-rw-rw-rw-   0        0        0     1349 2023-05-03 10:30:03.000000 shexer-2.4.1/shexer/core/profiling/strategy/direct_features_strategy.py
+-rw-rw-rw-   0        0        0     7395 2023-05-03 10:30:03.000000 shexer-2.4.1/shexer/core/profiling/strategy/include_reverse_features_strategy.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:36:40.733051 shexer-2.4.1/shexer/core/shexing/
+-rw-rw-rw-   0        0        0        0 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/core/shexing/__init__.py
+-rw-rw-rw-   0        0        0     6186 2023-10-20 11:58:54.000000 shexer-2.4.1/shexer/core/shexing/class_shexer.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:36:40.753289 shexer-2.4.1/shexer/core/shexing/strategy/
+-rw-rw-rw-   0        0        0        0 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/core/shexing/strategy/__init__.py
+-rw-rw-rw-   0        0        0    17141 2023-05-08 09:57:05.000000 shexer-2.4.1/shexer/core/shexing/strategy/abstract_shexing_strategy.py
+-rw-rw-rw-   0        0        0     5685 2023-05-03 10:30:03.000000 shexer-2.4.1/shexer/core/shexing/strategy/direct_and_inverse_shexing_strategy.py
+-rw-rw-rw-   0        0        0     2804 2023-05-03 10:30:03.000000 shexer-2.4.1/shexer/core/shexing/strategy/direct_shexing_strategy.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:36:40.771739 shexer-2.4.1/shexer/core/shexing/strategy/minimal_iri_strategy/
+-rw-rw-rw-   0        0        0        0 2023-05-03 10:30:03.000000 shexer-2.4.1/shexer/core/shexing/strategy/minimal_iri_strategy/__init__.py
+-rw-rw-rw-   0        0        0      118 2023-05-03 10:30:03.000000 shexer-2.4.1/shexer/core/shexing/strategy/minimal_iri_strategy/abstract_min_iri_strategy.py
+-rw-rw-rw-   0        0        0     1088 2023-05-03 10:30:03.000000 shexer-2.4.1/shexer/core/shexing/strategy/minimal_iri_strategy/annotate_min_iri_strategy.py
+-rw-rw-rw-   0        0        0      412 2023-05-03 10:30:03.000000 shexer-2.4.1/shexer/core/shexing/strategy/minimal_iri_strategy/ignore_min_iri_strategy.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:36:40.783707 shexer-2.4.1/shexer/io/
+-rw-rw-rw-   0        0        0        0 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/io/__init__.py
+-rw-rw-rw-   0        0        0      103 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/io/file.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:36:40.783707 shexer-2.4.1/shexer/io/graph/
+-rw-rw-rw-   0        0        0        0 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/io/graph/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:36:40.836166 shexer-2.4.1/shexer/io/graph/yielder/
+-rw-rw-rw-   0        0        0        0 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/io/graph/yielder/__init__.py
+-rw-rw-rw-   0        0        0     1431 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/io/graph/yielder/base_triples_yielder.py
+-rw-rw-rw-   0        0        0    17014 2024-05-02 11:22:19.000000 shexer-2.4.1/shexer/io/graph/yielder/big_ttl_triples_yielder.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:36:40.842940 shexer-2.4.1/shexer/io/graph/yielder/filter/
+-rw-rw-rw-   0        0        0        0 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/io/graph/yielder/filter/__init__.py
+-rw-rw-rw-   0        0        0      862 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/io/graph/yielder/filter/filter_namespaces_triple_yielder.py
+-rw-rw-rw-   0        0        0     1131 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/io/graph/yielder/multi_big_ttl_files_triple_yielder.py
+-rw-rw-rw-   0        0        0     1132 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/io/graph/yielder/multi_nt_triples_yielder.py
+-rw-rw-rw-   0        0        0     1757 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/io/graph/yielder/multi_rdflib_triple_yielder.py
+-rw-rw-rw-   0        0        0     1166 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/io/graph/yielder/multi_tsv_nt_triples_yielder.py
+-rw-rw-rw-   0        0        0     1483 2024-05-02 10:31:57.000000 shexer-2.4.1/shexer/io/graph/yielder/multi_zip_triples_yielder.py
+-rw-rw-rw-   0        0        0     2670 2024-05-02 10:31:57.000000 shexer-2.4.1/shexer/io/graph/yielder/multifile_base_triples_yielder.py
+-rw-rw-rw-   0        0        0     5686 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/io/graph/yielder/nt_triples_yielder.py
+-rw-rw-rw-   0        0        0     6817 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/io/graph/yielder/rdflib_triple_yielder.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:36:40.849614 shexer-2.4.1/shexer/io/graph/yielder/remote/
+-rw-rw-rw-   0        0        0        0 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/io/graph/yielder/remote/__init__.py
+-rw-rw-rw-   0        0        0     3826 2023-05-03 10:30:03.000000 shexer-2.4.1/shexer/io/graph/yielder/remote/sgraph_from_selectors_triple_yielder.py
+-rw-rw-rw-   0        0        0     4724 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/io/graph/yielder/tsv_nt_triples_yielder.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:36:40.855600 shexer-2.4.1/shexer/io/json/
+-rw-rw-rw-   0        0        0        0 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/io/json/__init__.py
+-rw-rw-rw-   0        0        0      207 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/io/json/json_loader.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:36:40.875537 shexer-2.4.1/shexer/io/line_reader/
+-rw-rw-rw-   0        0        0        0 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/io/line_reader/__init__.py
+-rw-rw-rw-   0        0        0      285 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/io/line_reader/file_line_reader.py
+-rw-rw-rw-   0        0        0      332 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/io/line_reader/gz_line_reader.py
+-rw-rw-rw-   0        0        0      260 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/io/line_reader/raw_string_line_reader.py
+-rw-rw-rw-   0        0        0      353 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/io/line_reader/zip_file_line_reader.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:36:40.877149 shexer-2.4.1/shexer/io/profile/
+-rw-rw-rw-   0        0        0        0 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/io/profile/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:36:40.882142 shexer-2.4.1/shexer/io/profile/formater/
+-rw-rw-rw-   0        0        0        0 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/io/profile/formater/__init__.py
+-rw-rw-rw-   0        0        0      409 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/io/profile/formater/abstract_profile_serializer.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:36:40.883135 shexer-2.4.1/shexer/io/shacl/
+-rw-rw-rw-   0        0        0        0 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/io/shacl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:36:40.890119 shexer-2.4.1/shexer/io/shacl/formater/
+-rw-rw-rw-   0        0        0        0 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/io/shacl/formater/__init__.py
+-rw-rw-rw-   0        0        0    16449 2024-04-01 11:02:47.000000 shexer-2.4.1/shexer/io/shacl/formater/shacl_serializer.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:36:40.898310 shexer-2.4.1/shexer/io/shape_map/
+-rw-rw-rw-   0        0        0        0 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/io/shape_map/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:36:40.904300 shexer-2.4.1/shexer/io/shape_map/label/
+-rw-rw-rw-   0        0        0        0 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/io/shape_map/label/__init__.py
+-rw-rw-rw-   0        0        0     1410 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/io/shape_map/label/shape_map_label_parser.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:36:40.910605 shexer-2.4.1/shexer/io/shape_map/node_selector/
+-rw-rw-rw-   0        0        0        0 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/io/shape_map/node_selector/__init__.py
+-rw-rw-rw-   0        0        0     6755 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/io/shape_map/node_selector/node_selector_parser.py
+-rw-rw-rw-   0        0        0     4966 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/io/shape_map/shape_map_parser.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:36:40.911599 shexer-2.4.1/shexer/io/shex/
+-rw-rw-rw-   0        0        0        0 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/io/shex/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:36:40.923088 shexer-2.4.1/shexer/io/shex/formater/
+-rw-rw-rw-   0        0        0        0 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/io/shex/formater/__init__.py
+-rw-rw-rw-   0        0        0      244 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/io/shex/formater/consts.py
+-rw-rw-rw-   0        0        0     7006 2023-05-03 10:30:03.000000 shexer-2.4.1/shexer/io/shex/formater/shex_serializer.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:36:40.949319 shexer-2.4.1/shexer/io/shex/formater/statement_serializers/
+-rw-rw-rw-   0        0        0        0 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/io/shex/formater/statement_serializers/__init__.py
+-rw-rw-rw-   0        0        0     6083 2023-05-08 09:57:05.000000 shexer-2.4.1/shexer/io/shex/formater/statement_serializers/base_statement_serializer.py
+-rw-rw-rw-   0        0        0     2287 2023-05-03 10:30:03.000000 shexer-2.4.1/shexer/io/shex/formater/statement_serializers/fixed_prop_choice_statement_serializer.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:36:40.971584 shexer-2.4.1/shexer/io/shex/formater/statement_serializers/frequency_strategy/
+-rw-rw-rw-   0        0        0        0 2023-05-03 10:30:03.000000 shexer-2.4.1/shexer/io/shex/formater/statement_serializers/frequency_strategy/__init__.py
+-rw-rw-rw-   0        0        0      383 2023-05-03 10:30:03.000000 shexer-2.4.1/shexer/io/shex/formater/statement_serializers/frequency_strategy/abs_freq_serializer.py
+-rw-rw-rw-   0        0        0      171 2023-05-03 10:30:03.000000 shexer-2.4.1/shexer/io/shex/formater/statement_serializers/frequency_strategy/base_frequency_strategy.py
+-rw-rw-rw-   0        0        0      887 2023-05-03 10:30:03.000000 shexer-2.4.1/shexer/io/shex/formater/statement_serializers/frequency_strategy/mixed_frequency_strategy.py
+-rw-rw-rw-   0        0        0     1278 2023-05-03 10:30:03.000000 shexer-2.4.1/shexer/io/shex/formater/statement_serializers/frequency_strategy/ratio_freq_serializer.py
+-rw-rw-rw-   0        0        0     1500 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/io/shex/formater/statement_serializers/inverse_statement_serializer.py
+-rw-rw-rw-   0        0        0     3211 2023-05-03 10:30:03.000000 shexer-2.4.1/shexer/io/shex/formater/statement_serializers/st_serializers_factory.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:36:40.978177 shexer-2.4.1/shexer/io/sparql/
+-rw-rw-rw-   0        0        0        0 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/io/sparql/__init__.py
+-rw-rw-rw-   0        0        0     4538 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/io/sparql/query.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:36:40.981172 shexer-2.4.1/shexer/io/uml/
+-rw-rw-rw-   0        0        0        0 2024-05-02 10:31:57.000000 shexer-2.4.1/shexer/io/uml/__init__.py
+-rw-rw-rw-   0        0        0     6256 2024-05-02 10:31:57.000000 shexer-2.4.1/shexer/io/uml/uml_serializer.py
+-rw-rw-rw-   0        0        0      469 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/io/wikidata.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:36:41.047668 shexer-2.4.1/shexer/model/
+-rw-rw-rw-   0        0        0      552 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/model/IRI.py
+-rw-rw-rw-   0        0        0      280 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/model/Literal.py
+-rw-rw-rw-   0        0        0      810 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/model/Macro.py
+-rw-rw-rw-   0        0        0        0 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/model/__init__.py
+-rw-rw-rw-   0        0        0      502 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/model/bnode.py
+-rw-rw-rw-   0        0        0      100 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/model/const_elem_types.py
+-rw-rw-rw-   0        0        0     1119 2023-05-03 10:30:03.000000 shexer-2.4.1/shexer/model/fixed_prop_choice_statement.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:36:41.068150 shexer-2.4.1/shexer/model/graph/
+-rw-rw-rw-   0        0        0        0 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/model/graph/__init__.py
+-rw-rw-rw-   0        0        0     6186 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/model/graph/abstract_sgraph.py
+-rw-rw-rw-   0        0        0     7633 2023-05-03 10:30:03.000000 shexer-2.4.1/shexer/model/graph/endpoint_sgraph.py
+-rw-rw-rw-   0        0        0     6201 2023-05-03 10:30:03.000000 shexer-2.4.1/shexer/model/graph/rdflib_sgraph.py
+-rw-rw-rw-   0        0        0     4173 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/model/hierarchy_tree.py
+-rw-rw-rw-   0        0        0     2527 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/model/node_selector.py
+-rw-rw-rw-   0        0        0      427 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/model/property.py
+-rw-rw-rw-   0        0        0     3361 2023-05-03 10:30:03.000000 shexer-2.4.1/shexer/model/shape.py
+-rw-rw-rw-   0        0        0      858 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/model/shape_map.py
+-rw-rw-rw-   0        0        0     2716 2023-05-03 10:30:03.000000 shexer-2.4.1/shexer/model/statement.py
+-rw-rw-rw-   0        0        0    25844 2024-05-02 10:31:57.000000 shexer-2.4.1/shexer/shaper.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:36:41.112908 shexer-2.4.1/shexer/utils/
+-rw-rw-rw-   0        0        0        0 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/utils/__init__.py
+-rw-rw-rw-   0        0        0      621 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/utils/compression.py
+-rw-rw-rw-   0        0        0       94 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/utils/dict.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:36:41.160504 shexer-2.4.1/shexer/utils/factories/
+-rw-rw-rw-   0        0        0        0 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/utils/factories/__init__.py
+-rw-rw-rw-   0        0        0     4300 2023-05-03 10:30:03.000000 shexer-2.4.1/shexer/utils/factories/class_profiler_factory.py
+-rw-rw-rw-   0        0        0     2322 2023-05-08 09:57:05.000000 shexer-2.4.1/shexer/utils/factories/class_shexer_factory.py
+-rw-rw-rw-   0        0        0      728 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/utils/factories/h_tree.py
+-rw-rw-rw-   0        0        0    12338 2023-06-13 16:20:36.000000 shexer-2.4.1/shexer/utils/factories/instance_tracker_factory.py
+-rw-rw-rw-   0        0        0      437 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/utils/factories/iri_factory.py
+-rw-rw-rw-   0        0        0      286 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/utils/factories/remote_graph_factory.py
+-rw-rw-rw-   0        0        0     1985 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/utils/factories/shape_map_factory.py
+-rw-rw-rw-   0        0        0      616 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/utils/factories/shape_map_parser_factory.py
+-rw-rw-rw-   0        0        0     2109 2024-05-02 10:31:57.000000 shexer-2.4.1/shexer/utils/factories/shape_serializer_factory.py
+-rw-rw-rw-   0        0        0    21108 2024-05-02 10:31:57.000000 shexer-2.4.1/shexer/utils/factories/triple_yielders_factory.py
+-rw-rw-rw-   0        0        0      123 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/utils/file.py
+-rw-rw-rw-   0        0        0      397 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/utils/log.py
+-rw-rw-rw-   0        0        0      761 2024-05-02 10:31:57.000000 shexer-2.4.1/shexer/utils/namespaces.py
+-rw-rw-rw-   0        0        0      967 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/utils/obj_references.py
+-rw-rw-rw-   0        0        0     2008 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/utils/shapes.py
+-rw-rw-rw-   0        0        0     1397 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/utils/target_elements.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:36:41.167484 shexer-2.4.1/shexer/utils/translators/
+-rw-rw-rw-   0        0        0        0 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/utils/translators/__init__.py
+-rw-rw-rw-   0        0        0     2881 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/utils/translators/list_of_classes_to_shape_map.py
+-rw-rw-rw-   0        0        0     3026 2023-01-30 11:26:57.000000 shexer-2.4.1/shexer/utils/triple_yielders.py
+-rw-rw-rw-   0        0        0     5749 2024-05-02 10:31:57.000000 shexer-2.4.1/shexer/utils/uri.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:36:40.592901 shexer-2.4.1/shexer.egg-info/
+-rw-rw-rw-   0        0        0    27781 2024-05-02 11:36:40.000000 shexer-2.4.1/shexer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8261 2024-05-02 11:36:40.000000 shexer-2.4.1/shexer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 11:36:40.000000 shexer-2.4.1/shexer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2024-05-02 11:36:40.000000 shexer-2.4.1/shexer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-05-02 11:36:40.000000 shexer-2.4.1/shexer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-02 11:36:41.445436 shexer-2.4.1/test/
+-rw-rw-rw-   0        0        0        0 2023-01-30 11:26:57.000000 shexer-2.4.1/test/__init__.py
+-rw-rw-rw-   0        0        0     1975 2024-05-02 11:22:19.000000 shexer-2.4.1/test/const.py
+-rw-rw-rw-   0        0        0     9389 2024-05-02 10:31:57.000000 shexer-2.4.1/test/t_utils.py
+-rw-rw-rw-   0        0        0     1488 2023-01-30 11:26:57.000000 shexer-2.4.1/test/test_all_classes_mode.py
+-rw-rw-rw-   0        0        0     1525 2023-01-30 11:26:57.000000 shexer-2.4.1/test/test_allow_opt_cardinality.py
+-rw-rw-rw-   0        0        0     3541 2023-05-08 09:57:05.000000 shexer-2.4.1/test/test_allow_redundant_or.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:36:41.459401 shexer-2.4.1/test/test_bugs/
+-rw-rw-rw-   0        0        0        0 2023-01-30 11:26:57.000000 shexer-2.4.1/test/test_bugs/__init__.py
+-rw-rw-rw-   0        0        0      796 2023-01-30 11:26:57.000000 shexer-2.4.1/test/test_bugs/test_no_sharp_in_auto_shape_names.py
+-rw-rw-rw-   0        0        0     1192 2023-05-08 09:57:05.000000 shexer-2.4.1/test/test_bugs/test_no_sharp_nor_slash_due_to_prefixing.py
+-rw-rw-rw-   0        0        0    11274 2024-05-02 10:31:57.000000 shexer-2.4.1/test/test_compression_mode.py
+-rw-rw-rw-   0        0        0     2171 2023-05-03 10:30:03.000000 shexer-2.4.1/test/test_decimals.py
+-rw-rw-rw-   0        0        0     5564 2023-01-30 11:26:57.000000 shexer-2.4.1/test/test_depth_for_building_subgraph.py
+-rw-rw-rw-   0        0        0     3526 2023-05-04 09:27:52.000000 shexer-2.4.1/test/test_detect_minimal_iri.py
+-rw-rw-rw-   0        0        0     1388 2023-05-03 10:30:03.000000 shexer-2.4.1/test/test_disable_comments.py
+-rw-rw-rw-   0        0        0     2922 2023-05-03 10:30:03.000000 shexer-2.4.1/test/test_disable_endpoint_cache.py
+-rw-rw-rw-   0        0        0     1491 2023-01-30 11:26:57.000000 shexer-2.4.1/test/test_disable_exact_cardinality.py
+-rw-rw-rw-   0        0        0     2557 2023-05-08 09:57:05.000000 shexer-2.4.1/test/test_disable_or_statements.py
+-rw-rw-rw-   0        0        0     3786 2023-01-30 11:26:57.000000 shexer-2.4.1/test/test_discard_and_compliant.py
+-rw-rw-rw-   0        0        0     2090 2023-01-30 11:26:57.000000 shexer-2.4.1/test/test_file_target_classes.py
+-rw-rw-rw-   0        0        0     1677 2023-01-30 11:26:57.000000 shexer-2.4.1/test/test_graph_file_input.py
+-rw-rw-rw-   0        0        0     3456 2023-01-30 11:26:57.000000 shexer-2.4.1/test/test_graph_list_of_file_inputs.py
+-rw-rw-rw-   0        0        0     1951 2023-01-30 11:26:57.000000 shexer-2.4.1/test/test_infer_numeric_types_for_untyped_literals.py
+-rw-rw-rw-   0        0        0     8663 2024-05-02 11:22:19.000000 shexer-2.4.1/test/test_input_format.py
+-rw-rw-rw-   0        0        0     4648 2023-06-13 16:20:36.000000 shexer-2.4.1/test/test_instances_cap.py
+-rw-rw-rw-   0        0        0     3367 2023-01-30 11:26:57.000000 shexer-2.4.1/test/test_instances_file_input.py
+-rw-rw-rw-   0        0        0     3852 2023-05-03 10:30:03.000000 shexer-2.4.1/test/test_instances_report.py
+-rw-rw-rw-   0        0        0     3548 2023-01-30 11:26:57.000000 shexer-2.4.1/test/test_instantiation_property.py
+-rw-rw-rw-   0        0        0     1964 2023-01-30 11:26:57.000000 shexer-2.4.1/test/test_inverse_paths.py
+-rw-rw-rw-   0        0        0     3594 2023-01-30 11:26:57.000000 shexer-2.4.1/test/test_keep_less_specific.py
+-rw-rw-rw-   0        0        0     4051 2023-01-30 11:26:57.000000 shexer-2.4.1/test/test_list_of_url_input.py
+-rw-rw-rw-   0        0        0     4106 2023-01-30 11:26:57.000000 shexer-2.4.1/test/test_namespaces_dict.py
+-rw-rw-rw-   0        0        0     2082 2023-01-30 11:26:57.000000 shexer-2.4.1/test/test_namespaces_to_ignore.py
+-rw-rw-rw-   0        0        0     5000 2023-01-30 11:26:57.000000 shexer-2.4.1/test/test_raw_graph.py
+-rw-rw-rw-   0        0        0     4300 2023-01-30 11:26:57.000000 shexer-2.4.1/test/test_raw_shape_map.py
+-rw-rw-rw-   0        0        0     1711 2023-01-30 11:26:57.000000 shexer-2.4.1/test/test_rdflib_graph.py
+-rw-rw-rw-   0        0        0     2932 2023-10-20 11:58:54.000000 shexer-2.4.1/test/test_remove_empty_sahpes.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:36:41.496613 shexer-2.4.1/test/test_shacl/
+-rw-rw-rw-   0        0        0        0 2023-01-30 11:26:57.000000 shexer-2.4.1/test/test_shacl/__init__.py
+-rw-rw-rw-   0        0        0     2225 2023-01-30 11:26:57.000000 shexer-2.4.1/test/test_shacl/test_annotation.py
+-rw-rw-rw-   0        0        0     2242 2023-01-30 11:26:57.000000 shexer-2.4.1/test/test_shacl/test_class_selection.py
+-rw-rw-rw-   0        0        0     3291 2023-05-03 10:30:03.000000 shexer-2.4.1/test/test_shacl/test_detect_minimal_iri.py
+-rw-rw-rw-   0        0        0      875 2024-04-01 11:02:47.000000 shexer-2.4.1/test/test_shacl/test_https.py
+-rw-rw-rw-   0        0        0     1534 2024-04-01 11:02:47.000000 shexer-2.4.1/test/test_shacl/test_literal_types.py
+-rw-rw-rw-   0        0        0     4313 2023-01-30 11:26:57.000000 shexer-2.4.1/test/test_shape_map_file.py
+-rw-rw-rw-   0        0        0     6086 2023-01-30 11:26:57.000000 shexer-2.4.1/test/test_shape_map_format.py
+-rw-rw-rw-   0        0        0     2307 2023-01-30 11:26:57.000000 shexer-2.4.1/test/test_shape_qualifiers_mode.py
+-rw-rw-rw-   0        0        0     2889 2023-01-30 11:26:57.000000 shexer-2.4.1/test/test_shapes_namespaces.py
+-rw-rw-rw-   0        0        0     2452 2023-01-30 11:26:57.000000 shexer-2.4.1/test/test_sort.py
+-rw-rw-rw-   0        0        0     2058 2023-01-30 11:26:57.000000 shexer-2.4.1/test/test_target_classes.py
+-rw-rw-rw-   0        0        0     3120 2023-01-30 11:26:57.000000 shexer-2.4.1/test/test_threshold.py
+-rw-rw-rw-   0        0        0     2729 2024-05-02 10:31:57.000000 shexer-2.4.1/test/test_uml_gen.py
+-rw-rw-rw-   0        0        0     2578 2023-01-30 11:26:57.000000 shexer-2.4.1/test/test_url_endpoint.py
+-rw-rw-rw-   0        0        0     1867 2023-01-30 11:26:57.000000 shexer-2.4.1/test/test_url_graph.py
+-rw-rw-rw-   0        0        0     1931 2024-05-02 10:31:57.000000 shexer-2.4.1/test/test_wikidata_annotation.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:36:41.508772 shexer-2.4.1/ws/
+-rw-rw-rw-   0        0        0        0 2023-01-30 11:26:57.000000 shexer-2.4.1/ws/__init__.py
+-rw-rw-rw-   0        0        0    19884 2023-01-30 11:26:57.000000 shexer-2.4.1/ws/shexer_rest.py
+-rw-rw-rw-   0        0        0       28 2023-01-30 11:26:57.000000 shexer-2.4.1/ws/wsgi.py
```

### Comparing `shexer-2.4.0/LICENSE` & `shexer-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/PKG-INFO` & `shexer-2.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: shexer
-Version: 2.4.0
+Version: 2.4.1
 Summary: Automatic schema extraction for RDF graphs
 Home-page: https://github.com/DaniFdezAlvarez/shexer
-Download-URL: https://github.com/DaniFdezAlvarez/shexer/archive/2.4.0.tar.gz
 Author: Daniel Fernandez-Alvarez
 Author-email: danifdezalvarez@gmail.com
+License: UNKNOWN
+Download-URL: https://github.com/DaniFdezAlvarez/shexer/archive/2.4.1.tar.gz
 Keywords: testing,shexer,shexerp3,rdf,shex,shacl,schema
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
@@ -248,7 +250,9 @@
 * output_file (default None): it specifies the path of the file in which the inferred shapes will be written. It must have a value different to None iff string_output is False.
 * output_format (default "ShExC"): format in which the inferred shapes will be serialized. The values currently supported are const.SHEXC and const.SHACLE_TURTLE.
 * aceptance_threshold (default 0): Given a certain inferred constraint __c__ for a shape __s__, the ammount of instances which conform to this constraint (ignoring constraints with '\*' cardinality) should be at least __aceptance\_threshold__. If this does not happen, then __c__ will not be included in __s__.
 * verbose (dafault False): when it is set to True, the extraction process will print log messages through the standard output.
 * to_uml_path (default None). This parameter expects to receive a disk path. If you provide a value here, sheXer will generate a UML diagram containing the extracted scheme and will save it in the path indicated as a PNG image. WARNING: you should be connected to Internet in  order to make this work.
 
 
+
+
```

### Comparing `shexer-2.4.0/README.md` & `shexer-2.4.1/README.md`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/local_code/yasunori_Test.py` & `shexer-2.4.1/test/test_url_graph.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,37 @@
-from shexer.consts import TURTLE, MIXED_INSTANCES
+import unittest
 from shexer.shaper import Shaper
-import sys
-import argparse
+from test.const import BASE_FILES, default_namespaces, G1_ALL_CLASSES_NO_COMMENTS
+from test.t_utils import file_vs_str_tunned_comparison
+import os.path as pth
+from shexer.consts import NT, TURTLE
+
+_BASE_DIR = BASE_FILES + "general" + pth.sep
+
+class TestUrlGraphFormat(unittest.TestCase):
+
+    def test_ttl(self):
+        shaper = Shaper(target_classes=["http://xmlns.com/foaf/0.1/Person",
+                                        "http://xmlns.com/foaf/0.1/Document"],
+                        url_graph_input="https://raw.githubusercontent.com/DaniFdezAlvarez/shexerp3/develop/test/t_files/t_graph_1.ttl",
+                        namespaces_dict=default_namespaces(),
+                        all_classes_mode=False,
+                        input_format=TURTLE,
+                        disable_comments=True)
+        str_result = shaper.shex_graph(string_output=True)
+        self.assertTrue(file_vs_str_tunned_comparison(file_path=G1_ALL_CLASSES_NO_COMMENTS,
+                                                      str_target=str_result))
+
+
+    def test_nt(self):
+        shaper = Shaper(target_classes=["http://xmlns.com/foaf/0.1/Person",
+                                        "http://xmlns.com/foaf/0.1/Document"],
+                        url_graph_input="https://raw.githubusercontent.com/DaniFdezAlvarez/shexerp3/develop/test/t_files/t_graph_1.nt",
+                        namespaces_dict=default_namespaces(),
+                        all_classes_mode=False,
+                        input_format=NT,
+                        disable_comments=True)
+        str_result = shaper.shex_graph(string_output=True)
+        self.assertTrue(file_vs_str_tunned_comparison(file_path=G1_ALL_CLASSES_NO_COMMENTS,
+                                                      str_target=str_result))
 
-def run(namespaces):
 
-    #shaper = Shaper(graph_file_input='/proc/self/fd/0',
-    shaper = Shaper(graph_file_input="test.ttl",
-                    all_classes_mode=True,
-                    input_format=TURTLE,
-                    namespaces_dict=namespaces,
-                    disable_exact_cardinality=True,
-                    detect_minimal_iri=True,
-                    instances_report_mode=MIXED_INSTANCES)
-
-    print(shaper.shex_graph(string_output=True,
-                      verbose=True,
-                      acceptance_threshold=0.05))
-
-    print("Done!")
-
-if __name__ == "__main__":
-
-    parser = argparse.ArgumentParser()
-    # namespace-prefix pair to be used in the results
-    namespaces_dict = {"http://purl.org/dc/terms/": "dc",
-                       "http://rdfs.org/ns/void#": "void",
-                       "http://www.w3.org/2001/XMLSchema#": "xsd",
-                       "http://www.w3.org/1999/02/22-rdf-syntax-ns#": "rdf",
-                       "http://xmlns.com/foaf/0.1/": "foaf",
-                       "http://www.w3.org/2002/07/owl#": "owl",
-                       "http://www.w3.org/2000/01/rdf-schema#": "rdfs",
-                       "http://www.w3.org/2004/02/skos/core#": "skos",
-                       }
-    run(namespaces=namespaces_dict)
```

### Comparing `shexer-2.4.0/setup.py` & `shexer-2.4.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 def read(file_path):
 	with open(file_path, "r") as in_stream:
 		return in_stream.read()
 
 setup(
   name = 'shexer',
   packages = find_packages(exclude=["*.local_code.*"]), # this must be the same as the name above
-  version = '2.4.0',
+  version = '2.4.1',
   description = 'Automatic schema extraction for RDF graphs',
   author = 'Daniel Fernandez-Alvarez',
   author_email = 'danifdezalvarez@gmail.com',
   url = 'https://github.com/DaniFdezAlvarez/shexer',
-  download_url = 'https://github.com/DaniFdezAlvarez/shexer/archive/2.4.0.tar.gz',
+  download_url = 'https://github.com/DaniFdezAlvarez/shexer/archive/2.4.1.tar.gz',
   keywords = ['testing', 'shexer', 'shexerp3', "rdf", "shex", "shacl", "schema"],
   long_description = read('README.md'),
   long_description_content_type='text/markdown',
   classifiers=[
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
@@ -28,10 +28,11 @@
         "Topic :: Software Development :: Libraries :: Python Modules"
     ],
   install_requires=[            
           'Flask',
           'Flask-Cors',
 		  'rdflib',
 		  'SPARQLWrapper',
-          'wlighter'
+          'wlighter',
+          'plantuml'
       ],
 )
```

### Comparing `shexer-2.4.0/shexer/consts.py` & `shexer-2.4.1/shexer/consts.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/core/instances/abstract_instance_tracker.py` & `shexer-2.4.1/shexer/core/instances/abstract_instance_tracker.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/core/instances/annotators/annotator_tracking_instances.py` & `shexer-2.4.1/shexer/core/instances/annotators/annotator_tracking_instances.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/core/instances/annotators/base_annotator.py` & `shexer-2.4.1/shexer/core/instances/annotators/base_annotator.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/core/instances/annotators/strategy_mode/all_classes_mode.py` & `shexer-2.4.1/shexer/core/instances/annotators/strategy_mode/all_classes_mode.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/core/instances/annotators/strategy_mode/base_strategy_mode.py` & `shexer-2.4.1/shexer/core/instances/annotators/strategy_mode/base_strategy_mode.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/core/instances/annotators/strategy_mode/compound_strategy_mode.py` & `shexer-2.4.1/shexer/core/instances/annotators/strategy_mode/compound_strategy_mode.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/core/instances/annotators/strategy_mode/instance_cap_mode.py` & `shexer-2.4.1/shexer/core/instances/annotators/strategy_mode/instance_cap_mode.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/core/instances/annotators/strategy_mode/shape_qualifiers_mode.py` & `shexer-2.4.1/shexer/core/instances/annotators/strategy_mode/shape_qualifiers_mode.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/core/instances/annotators/strategy_mode/target_classes_mode.py` & `shexer-2.4.1/shexer/core/instances/annotators/strategy_mode/target_classes_mode.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/core/instances/instance_tracker.py` & `shexer-2.4.1/shexer/core/instances/instance_tracker.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/core/instances/mappings/shape_map_instance_tracker.py` & `shexer-2.4.1/shexer/core/instances/mappings/shape_map_instance_tracker.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/core/instances/mix/mixed_instance_tracker.py` & `shexer-2.4.1/shexer/core/instances/mix/mixed_instance_tracker.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/core/profiling/class_profiler.py` & `shexer-2.4.1/shexer/core/profiling/class_profiler.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/core/profiling/strategy/abstract_feature_direction_strategy.py` & `shexer-2.4.1/shexer/core/profiling/strategy/abstract_feature_direction_strategy.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/core/profiling/strategy/direct_features_strategy.py` & `shexer-2.4.1/shexer/core/profiling/strategy/direct_features_strategy.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/core/profiling/strategy/include_reverse_features_strategy.py` & `shexer-2.4.1/shexer/core/profiling/strategy/include_reverse_features_strategy.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/core/shexing/class_shexer.py` & `shexer-2.4.1/shexer/core/shexing/class_shexer.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/core/shexing/strategy/abstract_shexing_strategy.py` & `shexer-2.4.1/shexer/core/shexing/strategy/abstract_shexing_strategy.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/core/shexing/strategy/direct_and_inverse_shexing_strategy.py` & `shexer-2.4.1/shexer/core/shexing/strategy/direct_and_inverse_shexing_strategy.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/core/shexing/strategy/direct_shexing_strategy.py` & `shexer-2.4.1/shexer/core/shexing/strategy/direct_shexing_strategy.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/core/shexing/strategy/minimal_iri_strategy/annotate_min_iri_strategy.py` & `shexer-2.4.1/shexer/core/shexing/strategy/minimal_iri_strategy/annotate_min_iri_strategy.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/io/graph/yielder/base_triples_yielder.py` & `shexer-2.4.1/shexer/io/graph/yielder/base_triples_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/io/graph/yielder/big_ttl_triples_yielder.py` & `shexer-2.4.1/shexer/io/graph/yielder/big_ttl_triples_yielder.py`

 * *Files 8% similar despite different names*

```diff
@@ -192,19 +192,38 @@
 
 
     def _find_next_unescaped_quotes(self, target_str, start_index):
         pos = target_str.find('"', start_index)
         while pos != -1:
             if target_str[pos-1] != "\\":
                 return pos  # not escaped
-            if pos >= 2 and target_str[pos-2] == '\\':
-                return pos  # the scape is scaped, so not escaped
+            # if pos >= 2 and target_str[pos-2] == '\\':
+            #     return pos  # the scape is scaped, so not escaped
+            if self._count_prior_backslashes(an_str=target_str,
+                                             quote_pos=pos) % 2 == 0:
+                return pos # the scape is scaped, so not escaped
+            pos = target_str.find('"', pos+1)
         if pos == -1:
             raise ValueError("Is this line malformed? Can`t find quotes matching: " + target_str)
 
+    def _count_prior_backslashes(self, an_str, quote_pos):
+        """
+        We assume that there is at least a backslash at an_str[pos-1], so pos-1 is a non-negative index of an_str
+        """
+        counter = 1
+        quote_pos -= 2
+        while quote_pos >= 0:
+            if an_str[quote_pos] == "\\":
+                counter += 1
+            else:
+                return counter
+            quote_pos -= 1
+        return counter
+
+
     def _find_next_quoted_literal_ending(self, target_str, start_index):
         next_quotes = self._find_next_unescaped_quotes(target_str=target_str,
                                                        start_index=start_index+1)
         if next_quotes +1 > len(target_str) or target_str[next_quotes + 1] == " ":
             return next_quotes
         elif target_str[next_quotes + 1] == "^":
             return self._find_next_blank(target_str, next_quotes) - 1
```

### Comparing `shexer-2.4.0/shexer/io/graph/yielder/filter/filter_namespaces_triple_yielder.py` & `shexer-2.4.1/shexer/io/graph/yielder/filter/filter_namespaces_triple_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/io/graph/yielder/multi_big_ttl_files_triple_yielder.py` & `shexer-2.4.1/shexer/io/graph/yielder/multi_big_ttl_files_triple_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/io/graph/yielder/multi_nt_triples_yielder.py` & `shexer-2.4.1/shexer/io/graph/yielder/multi_nt_triples_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/io/graph/yielder/multi_rdflib_triple_yielder.py` & `shexer-2.4.1/shexer/io/graph/yielder/multi_rdflib_triple_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/io/graph/yielder/multi_tsv_nt_triples_yielder.py` & `shexer-2.4.1/shexer/io/graph/yielder/multi_tsv_nt_triples_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/io/graph/yielder/multi_zip_triples_yielder.py` & `shexer-2.4.1/shexer/io/graph/yielder/multi_zip_triples_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/io/graph/yielder/multifile_base_triples_yielder.py` & `shexer-2.4.1/shexer/io/graph/yielder/multifile_base_triples_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/io/graph/yielder/nt_triples_yielder.py` & `shexer-2.4.1/shexer/io/graph/yielder/nt_triples_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/io/graph/yielder/rdflib_triple_yielder.py` & `shexer-2.4.1/shexer/io/graph/yielder/rdflib_triple_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/io/graph/yielder/remote/sgraph_from_selectors_triple_yielder.py` & `shexer-2.4.1/shexer/io/graph/yielder/remote/sgraph_from_selectors_triple_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/io/graph/yielder/tsv_nt_triples_yielder.py` & `shexer-2.4.1/shexer/io/graph/yielder/tsv_nt_triples_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/io/shacl/formater/shacl_serializer.py` & `shexer-2.4.1/shexer/io/shacl/formater/shacl_serializer.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/io/shape_map/label/shape_map_label_parser.py` & `shexer-2.4.1/shexer/io/shape_map/label/shape_map_label_parser.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/io/shape_map/node_selector/node_selector_parser.py` & `shexer-2.4.1/shexer/io/shape_map/node_selector/node_selector_parser.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/io/shape_map/shape_map_parser.py` & `shexer-2.4.1/shexer/io/shape_map/shape_map_parser.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/io/shex/formater/shex_serializer.py` & `shexer-2.4.1/shexer/io/shex/formater/shex_serializer.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/io/shex/formater/statement_serializers/base_statement_serializer.py` & `shexer-2.4.1/shexer/io/shex/formater/statement_serializers/base_statement_serializer.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/io/shex/formater/statement_serializers/fixed_prop_choice_statement_serializer.py` & `shexer-2.4.1/shexer/io/shex/formater/statement_serializers/fixed_prop_choice_statement_serializer.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/io/shex/formater/statement_serializers/frequency_strategy/mixed_frequency_strategy.py` & `shexer-2.4.1/shexer/io/shex/formater/statement_serializers/frequency_strategy/mixed_frequency_strategy.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/io/shex/formater/statement_serializers/frequency_strategy/ratio_freq_serializer.py` & `shexer-2.4.1/shexer/io/shex/formater/statement_serializers/frequency_strategy/ratio_freq_serializer.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/io/shex/formater/statement_serializers/inverse_statement_serializer.py` & `shexer-2.4.1/shexer/io/shex/formater/statement_serializers/inverse_statement_serializer.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/io/shex/formater/statement_serializers/st_serializers_factory.py` & `shexer-2.4.1/shexer/io/shex/formater/statement_serializers/st_serializers_factory.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/io/sparql/query.py` & `shexer-2.4.1/shexer/io/sparql/query.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/io/uml/uml_serializer.py` & `shexer-2.4.1/shexer/io/uml/uml_serializer.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/model/IRI.py` & `shexer-2.4.1/shexer/model/IRI.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/model/Macro.py` & `shexer-2.4.1/shexer/model/Macro.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/model/fixed_prop_choice_statement.py` & `shexer-2.4.1/shexer/model/fixed_prop_choice_statement.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/model/graph/abstract_sgraph.py` & `shexer-2.4.1/shexer/model/graph/abstract_sgraph.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/model/graph/endpoint_sgraph.py` & `shexer-2.4.1/shexer/model/graph/endpoint_sgraph.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/model/graph/rdflib_sgraph.py` & `shexer-2.4.1/shexer/model/graph/rdflib_sgraph.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/model/hierarchy_tree.py` & `shexer-2.4.1/shexer/model/hierarchy_tree.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/model/node_selector.py` & `shexer-2.4.1/shexer/model/node_selector.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/model/shape.py` & `shexer-2.4.1/shexer/model/shape.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/model/shape_map.py` & `shexer-2.4.1/shexer/model/shape_map.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/model/statement.py` & `shexer-2.4.1/shexer/model/statement.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/shaper.py` & `shexer-2.4.1/shexer/shaper.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/utils/compression.py` & `shexer-2.4.1/shexer/utils/compression.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/utils/factories/class_profiler_factory.py` & `shexer-2.4.1/shexer/utils/factories/class_profiler_factory.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/utils/factories/class_shexer_factory.py` & `shexer-2.4.1/shexer/utils/factories/class_shexer_factory.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/utils/factories/h_tree.py` & `shexer-2.4.1/shexer/utils/factories/h_tree.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/utils/factories/instance_tracker_factory.py` & `shexer-2.4.1/shexer/utils/factories/instance_tracker_factory.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/utils/factories/shape_map_factory.py` & `shexer-2.4.1/shexer/utils/factories/shape_map_factory.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/utils/factories/shape_map_parser_factory.py` & `shexer-2.4.1/shexer/utils/factories/shape_map_parser_factory.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/utils/factories/shape_serializer_factory.py` & `shexer-2.4.1/shexer/utils/factories/shape_serializer_factory.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/utils/factories/triple_yielders_factory.py` & `shexer-2.4.1/shexer/utils/factories/triple_yielders_factory.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/utils/namespaces.py` & `shexer-2.4.1/shexer/utils/namespaces.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/utils/obj_references.py` & `shexer-2.4.1/shexer/utils/obj_references.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/utils/shapes.py` & `shexer-2.4.1/shexer/utils/shapes.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/utils/target_elements.py` & `shexer-2.4.1/shexer/utils/target_elements.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/utils/translators/list_of_classes_to_shape_map.py` & `shexer-2.4.1/shexer/utils/translators/list_of_classes_to_shape_map.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/utils/triple_yielders.py` & `shexer-2.4.1/shexer/utils/triple_yielders.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer/utils/uri.py` & `shexer-2.4.1/shexer/utils/uri.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/shexer.egg-info/PKG-INFO` & `shexer-2.4.1/shexer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: shexer
-Version: 2.4.0
+Version: 2.4.1
 Summary: Automatic schema extraction for RDF graphs
 Home-page: https://github.com/DaniFdezAlvarez/shexer
-Download-URL: https://github.com/DaniFdezAlvarez/shexer/archive/2.4.0.tar.gz
 Author: Daniel Fernandez-Alvarez
 Author-email: danifdezalvarez@gmail.com
+License: UNKNOWN
+Download-URL: https://github.com/DaniFdezAlvarez/shexer/archive/2.4.1.tar.gz
 Keywords: testing,shexer,shexerp3,rdf,shex,shacl,schema
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
@@ -248,7 +250,9 @@
 * output_file (default None): it specifies the path of the file in which the inferred shapes will be written. It must have a value different to None iff string_output is False.
 * output_format (default "ShExC"): format in which the inferred shapes will be serialized. The values currently supported are const.SHEXC and const.SHACLE_TURTLE.
 * aceptance_threshold (default 0): Given a certain inferred constraint __c__ for a shape __s__, the ammount of instances which conform to this constraint (ignoring constraints with '\*' cardinality) should be at least __aceptance\_threshold__. If this does not happen, then __c__ will not be included in __s__.
 * verbose (dafault False): when it is set to True, the extraction process will print log messages through the standard output.
 * to_uml_path (default None). This parameter expects to receive a disk path. If you provide a value here, sheXer will generate a UML diagram containing the extracted scheme and will save it in the path indicated as a PNG image. WARNING: you should be connected to Internet in  order to make this work.
 
 
+
+
```

### Comparing `shexer-2.4.0/shexer.egg-info/SOURCES.txt` & `shexer-2.4.1/shexer.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 local_code/__init__.py
-local_code/beyza_test.py
-local_code/img_example.py
-local_code/split_non_split_thats_the_question.py
-local_code/tictactoe.py
-local_code/whatever.py
-local_code/yasunori_Test.py
+local_code/anything_shex_allclasses.py
+local_code/aventura_ruben.py
+local_code/yy_test.py
 shexer/__init__.py
 shexer/consts.py
 shexer/shaper.py
 shexer.egg-info/PKG-INFO
 shexer.egg-info/SOURCES.txt
 shexer.egg-info/dependency_links.txt
 shexer.egg-info/requires.txt
```

### Comparing `shexer-2.4.0/test/const.py` & `shexer-2.4.1/test/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 G1_NT = BASE_FILES + "t_graph_1.nt"
 G1_TSVO_SPO = BASE_FILES + "t_graph_1.tsv"
 G1_JSON_LD = BASE_FILES + "t_graph_1.json"
 G1_XML = BASE_FILES + "t_graph_1.xml"
 G1_TTL_WITH_BASE = BASE_FILES + "t_graph_1_base.ttl"
 G1_TTL_WITH_ABSOLUTES = BASE_FILES + "t_graph_1_absolutes.ttl"
 G1_TTL_WITH_USELESS_BNODE = BASE_FILES + "t_graph_1_bnode.ttl"
+G1_TTL_WITH_SCAPED_QUOTES = BASE_FILES + "t_graph_1_scaped_quotes.ttl"
 
 G1_N3 = BASE_FILES + "t_graph_1.n3"
 
 G1_ALL_CLASSES_NO_COMMENTS = BASE_FILES_GENERAL + "g1_all_classes_no_comments.shex"
 
 
 # PREFIX xml: <http://www.w3.org/XML/1998/namespace/>
```

### Comparing `shexer-2.4.0/test/t_utils.py` & `shexer-2.4.1/test/t_utils.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/test/test_all_classes_mode.py` & `shexer-2.4.1/test/test_all_classes_mode.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/test/test_allow_opt_cardinality.py` & `shexer-2.4.1/test/test_allow_opt_cardinality.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/test/test_allow_redundant_or.py` & `shexer-2.4.1/test/test_allow_redundant_or.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/test/test_bugs/test_no_sharp_in_auto_shape_names.py` & `shexer-2.4.1/test/test_bugs/test_no_sharp_in_auto_shape_names.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/test/test_bugs/test_no_sharp_nor_slash_due_to_prefixing.py` & `shexer-2.4.1/test/test_bugs/test_no_sharp_nor_slash_due_to_prefixing.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/test/test_compression_mode.py` & `shexer-2.4.1/test/test_compression_mode.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/test/test_decimals.py` & `shexer-2.4.1/test/test_decimals.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/test/test_depth_for_building_subgraph.py` & `shexer-2.4.1/test/test_depth_for_building_subgraph.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/test/test_detect_minimal_iri.py` & `shexer-2.4.1/test/test_detect_minimal_iri.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/test/test_disable_comments.py` & `shexer-2.4.1/test/test_disable_comments.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/test/test_disable_endpoint_cache.py` & `shexer-2.4.1/test/test_disable_endpoint_cache.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/test/test_disable_exact_cardinality.py` & `shexer-2.4.1/test/test_disable_exact_cardinality.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/test/test_disable_or_statements.py` & `shexer-2.4.1/test/test_disable_or_statements.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/test/test_discard_and_compliant.py` & `shexer-2.4.1/test/test_discard_and_compliant.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/test/test_file_target_classes.py` & `shexer-2.4.1/test/test_file_target_classes.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/test/test_graph_file_input.py` & `shexer-2.4.1/test/test_graph_file_input.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/test/test_graph_list_of_file_inputs.py` & `shexer-2.4.1/test/test_graph_list_of_file_inputs.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/test/test_infer_numeric_types_for_untyped_literals.py` & `shexer-2.4.1/test/test_infer_numeric_types_for_untyped_literals.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/test/test_input_format.py` & `shexer-2.4.1/test/test_input_format.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import unittest
 from shexer.shaper import Shaper
 from test.const import G1, BASE_FILES, G1_JSON_LD, G1_NT, G1_TSVO_SPO, G1_XML, G1_N3, \
-    default_namespaces, G1_TTL_WITH_BASE, G1_TTL_WITH_USELESS_BNODE, G1_TTL_WITH_ABSOLUTES
+    default_namespaces, G1_TTL_WITH_BASE, G1_TTL_WITH_USELESS_BNODE, G1_TTL_WITH_ABSOLUTES, \
+    G1_TTL_WITH_SCAPED_QUOTES
 from test.t_utils import file_vs_str_tunned_comparison
 import os.path as pth
 from shexer.consts import NT, TSV_SPO, RDF_XML, JSON_LD, N3, TURTLE, TURTLE_ITER
 
 _BASE_DIR = BASE_FILES + "general" + pth.sep
 
 class TestInputFormat(unittest.TestCase):
@@ -132,9 +133,22 @@
                         namespaces_dict=default_namespaces(),
                         all_classes_mode=False,
                         input_format=TURTLE_ITER,
                         disable_comments=True,
                         infer_numeric_types_for_untyped_literals=True)
         str_result = shaper.shex_graph(string_output=True)
         self.assertTrue(file_vs_str_tunned_comparison(file_path=_BASE_DIR + "g1_all_classes_no_comments.shex",
+                                                      str_target=str_result))
+
+    def test_ttl_iter_with_scaped_quotes(self):
+        shaper = Shaper(target_classes=["http://xmlns.com/foaf/0.1/Person",
+                                        "http://xmlns.com/foaf/0.1/Document"],
+                        graph_file_input=G1_TTL_WITH_SCAPED_QUOTES,
+                        namespaces_dict=default_namespaces(),
+                        all_classes_mode=False,
+                        input_format=TURTLE_ITER,
+                        disable_comments=True,
+                        infer_numeric_types_for_untyped_literals=True)
+        str_result = shaper.shex_graph(string_output=True)
+        self.assertTrue(file_vs_str_tunned_comparison(file_path=_BASE_DIR + "g1_all_classes_no_comments.shex",
                                                       str_target=str_result))
```

### Comparing `shexer-2.4.0/test/test_instances_cap.py` & `shexer-2.4.1/test/test_instances_cap.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/test/test_instances_file_input.py` & `shexer-2.4.1/test/test_instances_file_input.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/test/test_instances_report.py` & `shexer-2.4.1/test/test_instances_report.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/test/test_instantiation_property.py` & `shexer-2.4.1/test/test_instantiation_property.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/test/test_inverse_paths.py` & `shexer-2.4.1/test/test_inverse_paths.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/test/test_keep_less_specific.py` & `shexer-2.4.1/test/test_keep_less_specific.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/test/test_list_of_url_input.py` & `shexer-2.4.1/test/test_list_of_url_input.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/test/test_namespaces_dict.py` & `shexer-2.4.1/test/test_namespaces_dict.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/test/test_namespaces_to_ignore.py` & `shexer-2.4.1/test/test_namespaces_to_ignore.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/test/test_raw_graph.py` & `shexer-2.4.1/test/test_raw_graph.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/test/test_raw_shape_map.py` & `shexer-2.4.1/test/test_raw_shape_map.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/test/test_rdflib_graph.py` & `shexer-2.4.1/test/test_rdflib_graph.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/test/test_remove_empty_sahpes.py` & `shexer-2.4.1/test/test_remove_empty_sahpes.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/test/test_shacl/test_annotation.py` & `shexer-2.4.1/test/test_shacl/test_annotation.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/test/test_shacl/test_class_selection.py` & `shexer-2.4.1/test/test_shacl/test_class_selection.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/test/test_shacl/test_detect_minimal_iri.py` & `shexer-2.4.1/test/test_shacl/test_detect_minimal_iri.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/test/test_shacl/test_https.py` & `shexer-2.4.1/test/test_shacl/test_https.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/test/test_shacl/test_literal_types.py` & `shexer-2.4.1/test/test_shacl/test_literal_types.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/test/test_shape_map_file.py` & `shexer-2.4.1/test/test_shape_map_file.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/test/test_shape_map_format.py` & `shexer-2.4.1/test/test_shape_map_format.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/test/test_shape_qualifiers_mode.py` & `shexer-2.4.1/test/test_shape_qualifiers_mode.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/test/test_shapes_namespaces.py` & `shexer-2.4.1/test/test_shapes_namespaces.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/test/test_sort.py` & `shexer-2.4.1/test/test_sort.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/test/test_target_classes.py` & `shexer-2.4.1/test/test_target_classes.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/test/test_threshold.py` & `shexer-2.4.1/test/test_threshold.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/test/test_uml_gen.py` & `shexer-2.4.1/test/test_uml_gen.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/test/test_url_endpoint.py` & `shexer-2.4.1/test/test_url_endpoint.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/test/test_wikidata_annotation.py` & `shexer-2.4.1/test/test_wikidata_annotation.py`

 * *Files identical despite different names*

### Comparing `shexer-2.4.0/ws/shexer_rest.py` & `shexer-2.4.1/ws/shexer_rest.py`

 * *Files identical despite different names*

