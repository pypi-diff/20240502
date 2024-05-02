# Comparing `tmp/superlinked-3.9.0.tar.gz` & `tmp/superlinked-3.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superlinked-3.9.0.tar", max compression
+gzip compressed data, was "superlinked-3.9.1.tar", max compression
```

## Comparing `superlinked-3.9.0.tar` & `superlinked-3.9.1.tar`

### file list

```diff
@@ -1,171 +1,171 @@
--rw-r--r--   0        0        0    11354 2024-03-18 16:01:28.542189 superlinked-3.9.0/LICENSE
--rw-r--r--   0        0        0    28655 2024-03-18 16:01:28.546189 superlinked-3.9.0/NOTICE
--rw-r--r--   0        0        0     6382 2024-03-18 16:01:28.546189 superlinked-3.9.0/PYPI_README.md
--rw-r--r--   0        0        0     5371 2024-03-18 16:03:22.350188 superlinked-3.9.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-18 16:01:28.594189 superlinked-3.9.0/superlinked/__init__.py
--rw-r--r--   0        0        0     5228 2024-03-18 16:01:28.594189 superlinked-3.9.0/superlinked/evaluation/charts/recency_plotter.py
--rw-r--r--   0        0        0     5593 2024-03-18 16:01:28.594189 superlinked-3.9.0/superlinked/evaluation/vector_sampler.py
--rw-r--r--   0        0        0        0 2024-03-18 16:01:28.594189 superlinked-3.9.0/superlinked/framework/__init__.py
--rw-r--r--   0        0        0        0 2024-03-18 16:01:28.594189 superlinked-3.9.0/superlinked/framework/common/__init__.py
--rw-r--r--   0        0        0        0 2024-03-18 16:01:28.594189 superlinked-3.9.0/superlinked/framework/common/calculation/__init__.py
--rw-r--r--   0        0        0     1410 2024-03-18 16:01:28.594189 superlinked-3.9.0/superlinked/framework/common/calculation/vector_similarity.py
--rw-r--r--   0        0        0      682 2024-03-18 16:01:28.594189 superlinked-3.9.0/superlinked/framework/common/const.py
--rw-r--r--   0        0        0        0 2024-03-18 16:01:28.594189 superlinked-3.9.0/superlinked/framework/common/dag/__init__.py
--rw-r--r--   0        0        0     3270 2024-03-18 16:01:28.594189 superlinked-3.9.0/superlinked/framework/common/dag/aggregation_node.py
--rw-r--r--   0        0        0      940 2024-03-18 16:01:28.594189 superlinked-3.9.0/superlinked/framework/common/dag/chunking_node.py
--rw-r--r--   0        0        0     1857 2024-03-18 16:01:28.594189 superlinked-3.9.0/superlinked/framework/common/dag/comparison_filter_node.py
--rw-r--r--   0        0        0     2431 2024-03-18 16:01:28.594189 superlinked-3.9.0/superlinked/framework/common/dag/concatenation_node.py
--rw-r--r--   0        0        0      890 2024-03-18 16:01:28.594189 superlinked-3.9.0/superlinked/framework/common/dag/constant_node.py
--rw-r--r--   0        0        0     4571 2024-03-18 16:01:28.594189 superlinked-3.9.0/superlinked/framework/common/dag/context.py
--rw-r--r--   0        0        0     5016 2024-03-18 16:01:28.594189 superlinked-3.9.0/superlinked/framework/common/dag/dag.py
--rw-r--r--   0        0        0     1242 2024-03-18 16:01:28.594189 superlinked-3.9.0/superlinked/framework/common/dag/dag_effect.py
--rw-r--r--   0        0        0     3149 2024-03-18 16:01:28.594189 superlinked-3.9.0/superlinked/framework/common/dag/event_aggregation_node.py
--rw-r--r--   0        0        0      945 2024-03-18 16:01:28.594189 superlinked-3.9.0/superlinked/framework/common/dag/exception.py
--rw-r--r--   0        0        0     1795 2024-03-18 16:01:28.594189 superlinked-3.9.0/superlinked/framework/common/dag/index_node.py
--rw-r--r--   0        0        0     1119 2024-03-18 16:01:28.594189 superlinked-3.9.0/superlinked/framework/common/dag/named_function_node.py
--rw-r--r--   0        0        0     3263 2024-03-18 16:01:28.594189 superlinked-3.9.0/superlinked/framework/common/dag/node.py
--rw-r--r--   0        0        0     1313 2024-03-18 16:01:28.594189 superlinked-3.9.0/superlinked/framework/common/dag/number_embedding_node.py
--rw-r--r--   0        0        0     1331 2024-03-18 16:01:28.594189 superlinked-3.9.0/superlinked/framework/common/dag/number_similarity_node.py
--rw-r--r--   0        0        0     1818 2024-03-18 16:01:28.594189 superlinked-3.9.0/superlinked/framework/common/dag/period_time.py
--rw-r--r--   0        0        0      897 2024-03-18 16:01:28.594189 superlinked-3.9.0/superlinked/framework/common/dag/persistence_params.py
--rw-r--r--   0        0        0     1403 2024-03-18 16:01:28.594189 superlinked-3.9.0/superlinked/framework/common/dag/recency_node.py
--rw-r--r--   0        0        0     1015 2024-03-18 16:01:28.594189 superlinked-3.9.0/superlinked/framework/common/dag/resolved_schema_reference.py
--rw-r--r--   0        0        0     2019 2024-03-18 16:01:28.594189 superlinked-3.9.0/superlinked/framework/common/dag/schema_dag.py
--rw-r--r--   0        0        0     1111 2024-03-18 16:01:28.594189 superlinked-3.9.0/superlinked/framework/common/dag/schema_field_node.py
--rw-r--r--   0        0        0     1241 2024-03-18 16:01:28.594189 superlinked-3.9.0/superlinked/framework/common/dag/schema_object_reference.py
--rw-r--r--   0        0        0     1329 2024-03-18 16:01:28.594189 superlinked-3.9.0/superlinked/framework/common/dag/text_embedding_node.py
--rw-r--r--   0        0        0     4120 2024-03-18 16:01:28.594189 superlinked-3.9.0/superlinked/framework/common/data_types.py
--rw-r--r--   0        0        0        0 2024-03-18 16:01:28.594189 superlinked-3.9.0/superlinked/framework/common/embedding/__init__.py
--rw-r--r--   0        0        0     5317 2024-03-18 16:01:28.594189 superlinked-3.9.0/superlinked/framework/common/embedding/chunking_util.py
--rw-r--r--   0        0        0     1850 2024-03-18 16:01:28.594189 superlinked-3.9.0/superlinked/framework/common/embedding/number_embedding.py
--rw-r--r--   0        0        0     1848 2024-03-18 16:01:28.594189 superlinked-3.9.0/superlinked/framework/common/embedding/number_similarity_embedding.py
--rw-r--r--   0        0        0     4364 2024-03-18 16:01:28.594189 superlinked-3.9.0/superlinked/framework/common/embedding/recency_embedding.py
--rw-r--r--   0        0        0     1274 2024-03-18 16:01:28.594189 superlinked-3.9.0/superlinked/framework/common/embedding/sentence_transformer_embedding.py
--rw-r--r--   0        0        0     1143 2024-03-18 16:01:28.594189 superlinked-3.9.0/superlinked/framework/common/exception.py
--rw-r--r--   0        0        0        0 2024-03-18 16:01:28.594189 superlinked-3.9.0/superlinked/framework/common/interface/__init__.py
--rw-r--r--   0        0        0     5715 2024-03-18 16:01:28.594189 superlinked-3.9.0/superlinked/framework/common/interface/comparison_operand.py
--rw-r--r--   0        0        0      841 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/common/interface/comparison_operation_type.py
--rw-r--r--   0        0        0      718 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/common/interface/has_length.py
--rw-r--r--   0        0        0      836 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/common/interface/has_multiplier.py
--rw-r--r--   0        0        0      825 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/common/interface/weighted.py
--rw-r--r--   0        0        0     1307 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/common/observable.py
--rw-r--r--   0        0        0        0 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/common/parser/__init__.py
--rw-r--r--   0        0        0     5873 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/common/parser/data_parser.py
--rw-r--r--   0        0        0     4800 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/common/parser/dataframe_parser.py
--rw-r--r--   0        0        0      814 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/common/parser/exception.py
--rw-r--r--   0        0        0     4379 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/common/parser/json_parser.py
--rw-r--r--   0        0        0     1354 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/common/parser/parsed_schema.py
--rw-r--r--   0        0        0        0 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/common/schema/__init__.py
--rw-r--r--   0        0        0     1072 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/common/schema/event_schema.py
--rw-r--r--   0        0        0     1964 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/common/schema/event_schema_object.py
--rw-r--r--   0        0        0     1014 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/common/schema/exception.py
--rw-r--r--   0        0        0      627 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/common/schema/general_type.py
--rw-r--r--   0        0        0     1392 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/common/schema/id_schema_object.py
--rw-r--r--   0        0        0     1178 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/common/schema/schema.py
--rw-r--r--   0        0        0     3147 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/common/schema/schema_decorator.py
--rw-r--r--   0        0        0     3209 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/common/schema/schema_factory.py
--rw-r--r--   0        0        0     4804 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/common/schema/schema_object.py
--rw-r--r--   0        0        0     2962 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/common/schema/schema_reference.py
--rw-r--r--   0        0        0      686 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/common/schema/schema_type.py
--rw-r--r--   0        0        0     3201 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/common/schema/schema_validator.py
--rw-r--r--   0        0        0        0 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/common/source/__init__.py
--rw-r--r--   0        0        0      857 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/common/source/source.py
--rw-r--r--   0        0        0      647 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/common/source/types.py
--rw-r--r--   0        0        0        0 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/common/storage/__init__.py
--rw-r--r--   0        0        0      683 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/common/storage/persistence_type.py
--rw-r--r--   0        0        0        0 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/common/util/__init__.py
--rw-r--r--   0        0        0     2591 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/common/util/class_helper.py
--rw-r--r--   0        0        0     2074 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/common/util/dot_separated_path_util.py
--rw-r--r--   0        0        0      707 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/common/util/immutable_model.py
--rw-r--r--   0        0        0     1058 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/common/util/named_function_evaluator.py
--rw-r--r--   0        0        0      886 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/common/util/schema_util.py
--rw-r--r--   0        0        0      907 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/common/util/time_util.py
--rw-r--r--   0        0        0     4383 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/common/util/type_validator.py
--rw-r--r--   0        0        0        0 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/compiler/__init__.py
--rw-r--r--   0        0        0     3305 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/compiler/online_schema_dag_compiler.py
--rw-r--r--   0        0        0      108 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/dsl/__init__.py
--rw-r--r--   0        0        0      221 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/dsl/executor/__init__.py
--rw-r--r--   0        0        0      719 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/dsl/executor/exception.py
--rw-r--r--   0        0        0     4378 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/dsl/executor/executor.py
--rw-r--r--   0        0        0      124 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/dsl/executor/in_memory/__init__.py
--rw-r--r--   0        0        0     6524 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/dsl/executor/in_memory/in_memory_executor.py
--rw-r--r--   0        0        0      119 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/dsl/executor/query/__init__.py
--rw-r--r--   0        0        0     5732 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/dsl/executor/query/query_executor.py
--rw-r--r--   0        0        0        0 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/dsl/executor/rest/__init__.py
--rw-r--r--   0        0        0     1532 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/dsl/executor/rest/rest_configuration.py
--rw-r--r--   0        0        0      818 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/dsl/executor/rest/rest_descriptor.py
--rw-r--r--   0        0        0     4110 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/dsl/executor/rest/rest_executor.py
--rw-r--r--   0        0        0     3236 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/dsl/executor/rest/rest_handler.py
--rw-r--r--   0        0        0      176 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/dsl/index/__init__.py
--rw-r--r--   0        0        0     1776 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/dsl/index/effect.py
--rw-r--r--   0        0        0    10209 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/dsl/index/index.py
--rw-r--r--   0        0        0        0 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/dsl/index/util/__init__.py
--rw-r--r--   0        0        0     1516 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/dsl/index/util/aggregation_effect_group.py
--rw-r--r--   0        0        0     2448 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/dsl/index/util/aggregation_node_util.py
--rw-r--r--   0        0        0     6203 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/dsl/index/util/effect_with_referenced_schema_object.py
--rw-r--r--   0        0        0     2557 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/dsl/index/util/event_aggregation_effect_group.py
--rw-r--r--   0        0        0     3673 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/dsl/index/util/event_aggregation_node_util.py
--rw-r--r--   0        0        0      192 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/dsl/query/__init__.py
--rw-r--r--   0        0        0     1137 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/dsl/query/param.py
--rw-r--r--   0        0        0     2772 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/dsl/query/param_evaluator.py
--rw-r--r--   0        0        0        0 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/dsl/query/predicate/__init__.py
--rw-r--r--   0        0        0      756 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/dsl/query/predicate/binary_op.py
--rw-r--r--   0        0        0     1517 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/dsl/query/predicate/binary_predicate.py
--rw-r--r--   0        0        0      924 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/dsl/query/predicate/evaluated_binary_predicate.py
--rw-r--r--   0        0        0     1124 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/dsl/query/predicate/query_predicate.py
--rw-r--r--   0        0        0    11202 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/dsl/query/query.py
--rw-r--r--   0        0        0     6223 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/dsl/query/query_filters.py
--rw-r--r--   0        0        0     7954 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/dsl/query/query_vector_factory.py
--rw-r--r--   0        0        0     3329 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/dsl/query/query_weighting.py
--rw-r--r--   0        0        0     1890 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/dsl/query/result.py
--rw-r--r--   0        0        0      213 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/dsl/source/__init__.py
--rw-r--r--   0        0        0     2773 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/dsl/source/in_memory_source.py
--rw-r--r--   0        0        0     1987 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/dsl/source/rest_source.py
--rw-r--r--   0        0        0     1144 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/dsl/source/source.py
--rw-r--r--   0        0        0      183 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/dsl/space/__init__.py
--rw-r--r--   0        0        0      781 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/dsl/space/exception.py
--rw-r--r--   0        0        0     8004 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/dsl/space/number_space.py
--rw-r--r--   0        0        0     7301 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/dsl/space/recency_space.py
--rw-r--r--   0        0        0     2218 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/dsl/space/space.py
--rw-r--r--   0        0        0     1275 2024-03-18 16:01:28.598189 superlinked-3.9.0/superlinked/framework/dsl/space/space_field_set.py
--rw-r--r--   0        0        0     4414 2024-03-18 16:01:28.602189 superlinked-3.9.0/superlinked/framework/dsl/space/text_similarity_space.py
--rw-r--r--   0        0        0        0 2024-03-18 16:01:28.602189 superlinked-3.9.0/superlinked/framework/evaluator/__init__.py
--rw-r--r--   0        0        0     1016 2024-03-18 16:01:28.602189 superlinked-3.9.0/superlinked/framework/evaluator/dag_evaluator.py
--rw-r--r--   0        0        0     4650 2024-03-18 16:01:28.602189 superlinked-3.9.0/superlinked/framework/evaluator/online_dag_evaluator.py
--rw-r--r--   0        0        0     2278 2024-03-18 16:01:28.602189 superlinked-3.9.0/superlinked/framework/evaluator/query_dag_evaluator.py
--rw-r--r--   0        0        0        0 2024-03-18 16:01:28.602189 superlinked-3.9.0/superlinked/framework/online/__init__.py
--rw-r--r--   0        0        0        0 2024-03-18 16:01:28.602189 superlinked-3.9.0/superlinked/framework/online/dag/__init__.py
--rw-r--r--   0        0        0     4791 2024-03-18 16:01:28.602189 superlinked-3.9.0/superlinked/framework/online/dag/default_online_node.py
--rw-r--r--   0        0        0     1129 2024-03-18 16:01:28.602189 superlinked-3.9.0/superlinked/framework/online/dag/evaluation_result.py
--rw-r--r--   0        0        0      831 2024-03-18 16:01:28.602189 superlinked-3.9.0/superlinked/framework/online/dag/exception.py
--rw-r--r--   0        0        0     5312 2024-03-18 16:01:28.602189 superlinked-3.9.0/superlinked/framework/online/dag/online_aggregation_node.py
--rw-r--r--   0        0        0     3825 2024-03-18 16:01:28.602189 superlinked-3.9.0/superlinked/framework/online/dag/online_chunking_node.py
--rw-r--r--   0        0        0     2528 2024-03-18 16:01:28.602189 superlinked-3.9.0/superlinked/framework/online/dag/online_comparison_filter_node.py
--rw-r--r--   0        0        0     5093 2024-03-18 16:01:28.602189 superlinked-3.9.0/superlinked/framework/online/dag/online_concatenation_node.py
--rw-r--r--   0        0        0     2209 2024-03-18 16:01:28.602189 superlinked-3.9.0/superlinked/framework/online/dag/online_constant_node.py
--rw-r--r--   0        0        0     8871 2024-03-18 16:01:28.602189 superlinked-3.9.0/superlinked/framework/online/dag/online_event_aggregation_node.py
--rw-r--r--   0        0        0     3927 2024-03-18 16:01:28.602189 superlinked-3.9.0/superlinked/framework/online/dag/online_index_node.py
--rw-r--r--   0        0        0     2506 2024-03-18 16:01:28.602189 superlinked-3.9.0/superlinked/framework/online/dag/online_named_function_node.py
--rw-r--r--   0        0        0     3821 2024-03-18 16:01:28.602189 superlinked-3.9.0/superlinked/framework/online/dag/online_node.py
--rw-r--r--   0        0        0     3840 2024-03-18 16:01:28.602189 superlinked-3.9.0/superlinked/framework/online/dag/online_number_embedding_node.py
--rw-r--r--   0        0        0     3725 2024-03-18 16:01:28.602189 superlinked-3.9.0/superlinked/framework/online/dag/online_number_similarity_node.py
--rw-r--r--   0        0        0     2877 2024-03-18 16:01:28.602189 superlinked-3.9.0/superlinked/framework/online/dag/online_recency_node.py
--rw-r--r--   0        0        0     3718 2024-03-18 16:01:28.602189 superlinked-3.9.0/superlinked/framework/online/dag/online_schema_dag.py
--rw-r--r--   0        0        0     3609 2024-03-18 16:01:28.602189 superlinked-3.9.0/superlinked/framework/online/dag/online_schema_field_node.py
--rw-r--r--   0        0        0     2530 2024-03-18 16:01:28.602189 superlinked-3.9.0/superlinked/framework/online/dag/online_text_embedding_node.py
--rw-r--r--   0        0        0        0 2024-03-18 16:01:28.602189 superlinked-3.9.0/superlinked/framework/online/source/__init__.py
--rw-r--r--   0        0        0     3313 2024-03-18 16:01:28.602189 superlinked-3.9.0/superlinked/framework/online/source/in_memory_data_processor.py
--rw-r--r--   0        0        0     1479 2024-03-18 16:01:28.602189 superlinked-3.9.0/superlinked/framework/online/source/in_memory_object_writer.py
--rw-r--r--   0        0        0     1549 2024-03-18 16:01:28.602189 superlinked-3.9.0/superlinked/framework/online/source/in_memory_source.py
--rw-r--r--   0        0        0        0 2024-03-18 16:01:28.602189 superlinked-3.9.0/superlinked/framework/online/store_manager/__init__.py
--rw-r--r--   0        0        0     5813 2024-03-18 16:01:28.602189 superlinked-3.9.0/superlinked/framework/online/store_manager/evaluation_result_store_manager.py
--rw-r--r--   0        0        0        0 2024-03-18 16:01:28.602189 superlinked-3.9.0/superlinked/framework/storage/__init__.py
--rw-r--r--   0        0        0     2512 2024-03-18 16:01:28.602189 superlinked-3.9.0/superlinked/framework/storage/entity.py
--rw-r--r--   0        0        0     1936 2024-03-18 16:01:28.602189 superlinked-3.9.0/superlinked/framework/storage/entity_store.py
--rw-r--r--   0        0        0     4750 2024-03-18 16:01:28.602189 superlinked-3.9.0/superlinked/framework/storage/entity_store_manager.py
--rw-r--r--   0        0        0     1304 2024-03-18 16:01:28.602189 superlinked-3.9.0/superlinked/framework/storage/field.py
--rw-r--r--   0        0        0     7925 2024-03-18 16:01:28.602189 superlinked-3.9.0/superlinked/framework/storage/in_memory_entity_store.py
--rw-r--r--   0        0        0     1126 2024-03-18 16:01:28.602189 superlinked-3.9.0/superlinked/framework/storage/in_memory_object_store.py
--rw-r--r--   0        0        0     1125 2024-03-18 16:01:28.602189 superlinked-3.9.0/superlinked/framework/storage/object_store.py
--rw-r--r--   0        0        0     1570 2024-03-18 16:01:28.602189 superlinked-3.9.0/superlinked/framework/storage/object_store_manager.py
--rw-r--r--   0        0        0     9438 1970-01-01 00:00:00.000000 superlinked-3.9.0/PKG-INFO
+-rw-r--r--   0        0        0    11354 2024-03-20 12:30:06.973285 superlinked-3.9.1/LICENSE
+-rw-r--r--   0        0        0    28655 2024-03-20 12:30:06.973285 superlinked-3.9.1/NOTICE
+-rw-r--r--   0        0        0     6382 2024-03-20 12:30:06.973285 superlinked-3.9.1/PYPI_README.md
+-rw-r--r--   0        0        0     5333 2024-03-20 12:32:07.438558 superlinked-3.9.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/__init__.py
+-rw-r--r--   0        0        0     5228 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/evaluation/charts/recency_plotter.py
+-rw-r--r--   0        0        0     5593 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/evaluation/vector_sampler.py
+-rw-r--r--   0        0        0        0 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/calculation/__init__.py
+-rw-r--r--   0        0        0     1410 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/calculation/vector_similarity.py
+-rw-r--r--   0        0        0      682 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/const.py
+-rw-r--r--   0        0        0        0 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/dag/__init__.py
+-rw-r--r--   0        0        0     3270 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/dag/aggregation_node.py
+-rw-r--r--   0        0        0      940 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/dag/chunking_node.py
+-rw-r--r--   0        0        0     1857 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/dag/comparison_filter_node.py
+-rw-r--r--   0        0        0     2431 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/dag/concatenation_node.py
+-rw-r--r--   0        0        0      890 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/dag/constant_node.py
+-rw-r--r--   0        0        0     4571 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/dag/context.py
+-rw-r--r--   0        0        0     5016 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/dag/dag.py
+-rw-r--r--   0        0        0     1242 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/dag/dag_effect.py
+-rw-r--r--   0        0        0     3149 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/dag/event_aggregation_node.py
+-rw-r--r--   0        0        0      945 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/dag/exception.py
+-rw-r--r--   0        0        0     1795 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/dag/index_node.py
+-rw-r--r--   0        0        0     1119 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/dag/named_function_node.py
+-rw-r--r--   0        0        0     3263 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/dag/node.py
+-rw-r--r--   0        0        0     1313 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/dag/number_embedding_node.py
+-rw-r--r--   0        0        0     1331 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/dag/number_similarity_node.py
+-rw-r--r--   0        0        0     1818 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/dag/period_time.py
+-rw-r--r--   0        0        0      897 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/dag/persistence_params.py
+-rw-r--r--   0        0        0     1403 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/dag/recency_node.py
+-rw-r--r--   0        0        0     1015 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/dag/resolved_schema_reference.py
+-rw-r--r--   0        0        0     2019 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/dag/schema_dag.py
+-rw-r--r--   0        0        0     1111 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/dag/schema_field_node.py
+-rw-r--r--   0        0        0     1241 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/dag/schema_object_reference.py
+-rw-r--r--   0        0        0     1329 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/dag/text_embedding_node.py
+-rw-r--r--   0        0        0     4120 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/data_types.py
+-rw-r--r--   0        0        0        0 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/embedding/__init__.py
+-rw-r--r--   0        0        0     5317 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/embedding/chunking_util.py
+-rw-r--r--   0        0        0     1850 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/embedding/number_embedding.py
+-rw-r--r--   0        0        0     1848 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/embedding/number_similarity_embedding.py
+-rw-r--r--   0        0        0     4364 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/embedding/recency_embedding.py
+-rw-r--r--   0        0        0     1274 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/embedding/sentence_transformer_embedding.py
+-rw-r--r--   0        0        0     1143 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/exception.py
+-rw-r--r--   0        0        0        0 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/interface/__init__.py
+-rw-r--r--   0        0        0     5715 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/interface/comparison_operand.py
+-rw-r--r--   0        0        0      841 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/interface/comparison_operation_type.py
+-rw-r--r--   0        0        0      718 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/interface/has_length.py
+-rw-r--r--   0        0        0      836 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/interface/has_multiplier.py
+-rw-r--r--   0        0        0      825 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/interface/weighted.py
+-rw-r--r--   0        0        0     1307 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/observable.py
+-rw-r--r--   0        0        0        0 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/parser/__init__.py
+-rw-r--r--   0        0        0     5873 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/parser/data_parser.py
+-rw-r--r--   0        0        0     4800 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/parser/dataframe_parser.py
+-rw-r--r--   0        0        0      814 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/parser/exception.py
+-rw-r--r--   0        0        0     4379 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/parser/json_parser.py
+-rw-r--r--   0        0        0     1354 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/parser/parsed_schema.py
+-rw-r--r--   0        0        0        0 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/schema/__init__.py
+-rw-r--r--   0        0        0     1072 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/schema/event_schema.py
+-rw-r--r--   0        0        0     1964 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/schema/event_schema_object.py
+-rw-r--r--   0        0        0     1014 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/schema/exception.py
+-rw-r--r--   0        0        0      627 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/schema/general_type.py
+-rw-r--r--   0        0        0     1392 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/schema/id_schema_object.py
+-rw-r--r--   0        0        0     1178 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/schema/schema.py
+-rw-r--r--   0        0        0     3147 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/schema/schema_decorator.py
+-rw-r--r--   0        0        0     3209 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/schema/schema_factory.py
+-rw-r--r--   0        0        0     4804 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/schema/schema_object.py
+-rw-r--r--   0        0        0     2962 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/schema/schema_reference.py
+-rw-r--r--   0        0        0      686 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/schema/schema_type.py
+-rw-r--r--   0        0        0     3201 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/schema/schema_validator.py
+-rw-r--r--   0        0        0        0 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/source/__init__.py
+-rw-r--r--   0        0        0      857 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/source/source.py
+-rw-r--r--   0        0        0      647 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/source/types.py
+-rw-r--r--   0        0        0        0 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/storage/__init__.py
+-rw-r--r--   0        0        0      683 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/storage/persistence_type.py
+-rw-r--r--   0        0        0        0 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/util/__init__.py
+-rw-r--r--   0        0        0     2591 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/common/util/class_helper.py
+-rw-r--r--   0        0        0     2074 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/common/util/dot_separated_path_util.py
+-rw-r--r--   0        0        0      707 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/common/util/immutable_model.py
+-rw-r--r--   0        0        0     1058 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/common/util/named_function_evaluator.py
+-rw-r--r--   0        0        0      886 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/common/util/schema_util.py
+-rw-r--r--   0        0        0      907 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/common/util/time_util.py
+-rw-r--r--   0        0        0     4383 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/common/util/type_validator.py
+-rw-r--r--   0        0        0        0 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/compiler/__init__.py
+-rw-r--r--   0        0        0     3305 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/compiler/online_schema_dag_compiler.py
+-rw-r--r--   0        0        0      108 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/__init__.py
+-rw-r--r--   0        0        0      221 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/executor/__init__.py
+-rw-r--r--   0        0        0      719 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/executor/exception.py
+-rw-r--r--   0        0        0     4378 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/executor/executor.py
+-rw-r--r--   0        0        0      124 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/executor/in_memory/__init__.py
+-rw-r--r--   0        0        0     6524 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/executor/in_memory/in_memory_executor.py
+-rw-r--r--   0        0        0      119 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/executor/query/__init__.py
+-rw-r--r--   0        0        0     5732 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/executor/query/query_executor.py
+-rw-r--r--   0        0        0        0 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/executor/rest/__init__.py
+-rw-r--r--   0        0        0     1532 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/executor/rest/rest_configuration.py
+-rw-r--r--   0        0        0      818 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/executor/rest/rest_descriptor.py
+-rw-r--r--   0        0        0     4110 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/executor/rest/rest_executor.py
+-rw-r--r--   0        0        0     3236 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/executor/rest/rest_handler.py
+-rw-r--r--   0        0        0      176 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/index/__init__.py
+-rw-r--r--   0        0        0     1776 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/index/effect.py
+-rw-r--r--   0        0        0    10209 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/index/index.py
+-rw-r--r--   0        0        0        0 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/index/util/__init__.py
+-rw-r--r--   0        0        0     1516 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/index/util/aggregation_effect_group.py
+-rw-r--r--   0        0        0     2448 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/index/util/aggregation_node_util.py
+-rw-r--r--   0        0        0     6203 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/index/util/effect_with_referenced_schema_object.py
+-rw-r--r--   0        0        0     2557 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/index/util/event_aggregation_effect_group.py
+-rw-r--r--   0        0        0     3673 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/index/util/event_aggregation_node_util.py
+-rw-r--r--   0        0        0      192 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/query/__init__.py
+-rw-r--r--   0        0        0     1137 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/query/param.py
+-rw-r--r--   0        0        0     2772 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/query/param_evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/query/predicate/__init__.py
+-rw-r--r--   0        0        0      756 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/query/predicate/binary_op.py
+-rw-r--r--   0        0        0     1517 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/query/predicate/binary_predicate.py
+-rw-r--r--   0        0        0      924 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/query/predicate/evaluated_binary_predicate.py
+-rw-r--r--   0        0        0     1124 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/query/predicate/query_predicate.py
+-rw-r--r--   0        0        0    11202 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/query/query.py
+-rw-r--r--   0        0        0     6223 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/query/query_filters.py
+-rw-r--r--   0        0        0     7954 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/query/query_vector_factory.py
+-rw-r--r--   0        0        0     3329 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/query/query_weighting.py
+-rw-r--r--   0        0        0     1890 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/query/result.py
+-rw-r--r--   0        0        0      213 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/source/__init__.py
+-rw-r--r--   0        0        0     2773 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/source/in_memory_source.py
+-rw-r--r--   0        0        0     1987 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/source/rest_source.py
+-rw-r--r--   0        0        0     1144 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/source/source.py
+-rw-r--r--   0        0        0      183 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/space/__init__.py
+-rw-r--r--   0        0        0      781 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/space/exception.py
+-rw-r--r--   0        0        0     8004 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/space/number_space.py
+-rw-r--r--   0        0        0     7301 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/space/recency_space.py
+-rw-r--r--   0        0        0     2218 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/space/space.py
+-rw-r--r--   0        0        0     1275 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/space/space_field_set.py
+-rw-r--r--   0        0        0     4414 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/space/text_similarity_space.py
+-rw-r--r--   0        0        0        0 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/evaluator/__init__.py
+-rw-r--r--   0        0        0     1016 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/evaluator/dag_evaluator.py
+-rw-r--r--   0        0        0     4650 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/evaluator/online_dag_evaluator.py
+-rw-r--r--   0        0        0     2278 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/evaluator/query_dag_evaluator.py
+-rw-r--r--   0        0        0        0 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/online/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/online/dag/__init__.py
+-rw-r--r--   0        0        0     4791 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/online/dag/default_online_node.py
+-rw-r--r--   0        0        0     1129 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/online/dag/evaluation_result.py
+-rw-r--r--   0        0        0      831 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/online/dag/exception.py
+-rw-r--r--   0        0        0     5312 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/online/dag/online_aggregation_node.py
+-rw-r--r--   0        0        0     3825 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/online/dag/online_chunking_node.py
+-rw-r--r--   0        0        0     2528 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/online/dag/online_comparison_filter_node.py
+-rw-r--r--   0        0        0     5093 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/online/dag/online_concatenation_node.py
+-rw-r--r--   0        0        0     2209 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/online/dag/online_constant_node.py
+-rw-r--r--   0        0        0     8871 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/online/dag/online_event_aggregation_node.py
+-rw-r--r--   0        0        0     3927 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/online/dag/online_index_node.py
+-rw-r--r--   0        0        0     2506 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/online/dag/online_named_function_node.py
+-rw-r--r--   0        0        0     3821 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/online/dag/online_node.py
+-rw-r--r--   0        0        0     3840 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/online/dag/online_number_embedding_node.py
+-rw-r--r--   0        0        0     3725 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/online/dag/online_number_similarity_node.py
+-rw-r--r--   0        0        0     2877 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/online/dag/online_recency_node.py
+-rw-r--r--   0        0        0     3718 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/online/dag/online_schema_dag.py
+-rw-r--r--   0        0        0     3609 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/online/dag/online_schema_field_node.py
+-rw-r--r--   0        0        0     2530 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/online/dag/online_text_embedding_node.py
+-rw-r--r--   0        0        0        0 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/online/source/__init__.py
+-rw-r--r--   0        0        0     3313 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/online/source/in_memory_data_processor.py
+-rw-r--r--   0        0        0     1479 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/online/source/in_memory_object_writer.py
+-rw-r--r--   0        0        0     1549 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/online/source/in_memory_source.py
+-rw-r--r--   0        0        0        0 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/online/store_manager/__init__.py
+-rw-r--r--   0        0        0     5813 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/online/store_manager/evaluation_result_store_manager.py
+-rw-r--r--   0        0        0        0 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/storage/__init__.py
+-rw-r--r--   0        0        0     2512 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/storage/entity.py
+-rw-r--r--   0        0        0     1936 2024-03-20 12:30:07.033286 superlinked-3.9.1/superlinked/framework/storage/entity_store.py
+-rw-r--r--   0        0        0     4750 2024-03-20 12:30:07.033286 superlinked-3.9.1/superlinked/framework/storage/entity_store_manager.py
+-rw-r--r--   0        0        0     1304 2024-03-20 12:30:07.033286 superlinked-3.9.1/superlinked/framework/storage/field.py
+-rw-r--r--   0        0        0     7925 2024-03-20 12:30:07.033286 superlinked-3.9.1/superlinked/framework/storage/in_memory_entity_store.py
+-rw-r--r--   0        0        0     1126 2024-03-20 12:30:07.033286 superlinked-3.9.1/superlinked/framework/storage/in_memory_object_store.py
+-rw-r--r--   0        0        0     1125 2024-03-20 12:30:07.033286 superlinked-3.9.1/superlinked/framework/storage/object_store.py
+-rw-r--r--   0        0        0     1570 2024-03-20 12:30:07.033286 superlinked-3.9.1/superlinked/framework/storage/object_store_manager.py
+-rw-r--r--   0        0        0     9446 1970-01-01 00:00:00.000000 superlinked-3.9.1/PKG-INFO
```

### Comparing `superlinked-3.9.0/LICENSE` & `superlinked-3.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/NOTICE` & `superlinked-3.9.1/NOTICE`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/PYPI_README.md` & `superlinked-3.9.1/PYPI_README.md`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/pyproject.toml` & `superlinked-3.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 [tool.poetry]
 name = "superlinked"
-version = "3.9.0"  # The version will be dynamically updated
+version = "3.9.1"  # The version will be dynamically updated
 description = "The Superlinked vector computing library"
 authors = ["Superlinked Release <release@superlinked.com>"]
 readme = "PYPI_README.md"
 license = "Apache-2.0"
 include = ["NOTICE"]
 
 [tool.poetry.dependencies]
 python = "~3.10"
 numpy = "==1.22.4"
 pandas = "^2.2.1"
 sentence-transformers = "2.2.2"
 typing_extensions = ">=3.10.0.2"
 beartype = "^0.17.2"
+furl = "^2.1.3"
+pydantic = "^2.6.4"
 altair = { version = "5.2.0", optional = true }
 fastapi = { version = "0.109.0", optional = true }
 uvicorn = { version = "0.15.0", optional = true }
 supervisor = { version = "4.2.5", optional = true }
 deltalake = { version = "0.15.1", optional = true }
 dask = { version = "2024.1.0", extras = ["complete", "distributed"], optional = true }
 fsspec = { version = "2023.12.2", optional = true }
@@ -32,39 +34,37 @@
 pyyaml = { version = "6.0.1", optional = true }
 requests = { version = "2.27.1", optional = true }
 jupyter = { version = "^1.0.0", optional = true }
 yelp-gprof2dot = { version = "~1.2.0", optional = true }
 graphviz = { version = "~0.20.1", optional = true }
 snakeviz = { version = "~2.2.0", optional = true }
 pyspark = { version = "3.5.0", optional = true }
-furl = { version = "^2.1.3", optional = true }
 cerberus = {version = "==1.3.5", optional = true}
 pydantic-settings = {version = "^2.2.1", optional = true}
 typing-inspect = {version = "^0.9.0", optional = true}
 umap-learn = {version = "==0.5.5", optional = true}
 transformers = {version = "==4.38.2", optional = true}
 accelerate = {version = "==0.27.2", optional = true}
 ipywidgets = {version = "==8.1.2", optional = true}
 inject = {version = "^5.2.0", optional = true}
 fastapi-restful = {version = "^0.5.0", optional = true}
 
 [tool.poetry.extras]
 interactive = ["altair", "jupyter", "umap-learn", "transformers", "accelerate", "ipywidgets"]
-deployment-executor = ["fastapi", "uvicorn", "supervisor", "deltalake", "dask", "typing-extensions", "fsspec", "gcsfs", "s3fs", "adlfs", "httpx", "furl", "cerberus", "pydantic-settings", "typing-inspect", "inject", "fastapi-restful"]
+deployment-executor = ["fastapi", "uvicorn", "supervisor", "deltalake", "dask", "typing-extensions", "fsspec", "gcsfs", "s3fs", "adlfs", "httpx", "cerberus", "pydantic-settings", "typing-inspect", "inject", "fastapi-restful"]
 deployment-poller = ["boto3", "boto3-stubs", "google-auth", "google-cloud-storage", "pyyaml", "requests", "cerberus"]
 profiler = ["jupyter", "yelp-gprof2dot", "graphviz", "snakeviz"]
 batch = ["pyspark"]
 
 [tool.poetry.group.dev.dependencies]
 types-google-cloud-ndb = "~2.2.0.20240205"
 types-jmespath = "~1.0.2.20240106"
 types-pyyaml = "~6.0.12.12"
 mypy-boto3 = "~1.34.41"
 types-requests = "<2.31.0.7"
-pydantic = "2.5.3"
 pytest = "7.4.3"
 pytest-mock = "3.12.0"
 pytest-emoji = "~0.2.0"
 pytest-md = "~0.2.0"
 autoflake = "~2.2.1"
 coverage = "~7.4.0"
 debugpy = "~1.8.0"
```

### Comparing `superlinked-3.9.0/superlinked/evaluation/charts/recency_plotter.py` & `superlinked-3.9.1/superlinked/evaluation/charts/recency_plotter.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/evaluation/vector_sampler.py` & `superlinked-3.9.1/superlinked/evaluation/vector_sampler.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/common/calculation/vector_similarity.py` & `superlinked-3.9.1/superlinked/framework/common/calculation/vector_similarity.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/common/const.py` & `superlinked-3.9.1/superlinked/framework/common/const.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/common/dag/aggregation_node.py` & `superlinked-3.9.1/superlinked/framework/common/dag/aggregation_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/common/dag/chunking_node.py` & `superlinked-3.9.1/superlinked/framework/common/dag/chunking_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/common/dag/comparison_filter_node.py` & `superlinked-3.9.1/superlinked/framework/common/dag/comparison_filter_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/common/dag/concatenation_node.py` & `superlinked-3.9.1/superlinked/framework/common/dag/concatenation_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/common/dag/constant_node.py` & `superlinked-3.9.1/superlinked/framework/common/dag/constant_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/common/dag/context.py` & `superlinked-3.9.1/superlinked/framework/common/dag/context.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/common/dag/dag.py` & `superlinked-3.9.1/superlinked/framework/common/dag/dag.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/common/dag/dag_effect.py` & `superlinked-3.9.1/superlinked/framework/common/dag/dag_effect.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/common/dag/event_aggregation_node.py` & `superlinked-3.9.1/superlinked/framework/common/dag/event_aggregation_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/common/dag/exception.py` & `superlinked-3.9.1/superlinked/framework/common/dag/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/common/dag/index_node.py` & `superlinked-3.9.1/superlinked/framework/common/dag/index_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/common/dag/named_function_node.py` & `superlinked-3.9.1/superlinked/framework/common/dag/named_function_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/common/dag/node.py` & `superlinked-3.9.1/superlinked/framework/common/dag/node.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/common/dag/number_embedding_node.py` & `superlinked-3.9.1/superlinked/framework/common/dag/number_embedding_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/common/dag/number_similarity_node.py` & `superlinked-3.9.1/superlinked/framework/common/dag/number_similarity_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/common/dag/period_time.py` & `superlinked-3.9.1/superlinked/framework/common/dag/period_time.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/common/dag/persistence_params.py` & `superlinked-3.9.1/superlinked/framework/common/dag/persistence_params.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/common/dag/recency_node.py` & `superlinked-3.9.1/superlinked/framework/common/dag/recency_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/common/dag/resolved_schema_reference.py` & `superlinked-3.9.1/superlinked/framework/common/dag/resolved_schema_reference.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/common/dag/schema_dag.py` & `superlinked-3.9.1/superlinked/framework/common/dag/schema_dag.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/common/dag/schema_field_node.py` & `superlinked-3.9.1/superlinked/framework/common/dag/schema_field_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/common/dag/schema_object_reference.py` & `superlinked-3.9.1/superlinked/framework/common/dag/schema_object_reference.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/common/dag/text_embedding_node.py` & `superlinked-3.9.1/superlinked/framework/common/dag/text_embedding_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/common/data_types.py` & `superlinked-3.9.1/superlinked/framework/common/data_types.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/common/embedding/chunking_util.py` & `superlinked-3.9.1/superlinked/framework/common/embedding/chunking_util.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/common/embedding/number_embedding.py` & `superlinked-3.9.1/superlinked/framework/common/embedding/number_embedding.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/common/embedding/number_similarity_embedding.py` & `superlinked-3.9.1/superlinked/framework/common/embedding/number_similarity_embedding.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/common/embedding/recency_embedding.py` & `superlinked-3.9.1/superlinked/framework/common/embedding/recency_embedding.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/common/embedding/sentence_transformer_embedding.py` & `superlinked-3.9.1/superlinked/framework/common/embedding/sentence_transformer_embedding.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/common/exception.py` & `superlinked-3.9.1/superlinked/framework/common/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/common/interface/comparison_operand.py` & `superlinked-3.9.1/superlinked/framework/common/interface/comparison_operand.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/common/interface/comparison_operation_type.py` & `superlinked-3.9.1/superlinked/framework/common/interface/comparison_operation_type.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/common/interface/has_length.py` & `superlinked-3.9.1/superlinked/framework/common/interface/has_length.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/common/interface/has_multiplier.py` & `superlinked-3.9.1/superlinked/framework/common/interface/has_multiplier.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/common/interface/weighted.py` & `superlinked-3.9.1/superlinked/framework/common/interface/weighted.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/common/observable.py` & `superlinked-3.9.1/superlinked/framework/common/observable.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/common/parser/data_parser.py` & `superlinked-3.9.1/superlinked/framework/common/parser/data_parser.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/common/parser/dataframe_parser.py` & `superlinked-3.9.1/superlinked/framework/common/parser/dataframe_parser.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/common/parser/exception.py` & `superlinked-3.9.1/superlinked/framework/common/parser/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/common/parser/json_parser.py` & `superlinked-3.9.1/superlinked/framework/common/parser/json_parser.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/common/parser/parsed_schema.py` & `superlinked-3.9.1/superlinked/framework/common/parser/parsed_schema.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/common/schema/event_schema.py` & `superlinked-3.9.1/superlinked/framework/common/schema/event_schema.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/common/schema/event_schema_object.py` & `superlinked-3.9.1/superlinked/framework/common/schema/event_schema_object.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/common/schema/exception.py` & `superlinked-3.9.1/superlinked/framework/common/schema/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/common/schema/general_type.py` & `superlinked-3.9.1/superlinked/framework/common/schema/general_type.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/common/schema/id_schema_object.py` & `superlinked-3.9.1/superlinked/framework/common/schema/id_schema_object.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/common/schema/schema.py` & `superlinked-3.9.1/superlinked/framework/common/schema/schema.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/common/schema/schema_decorator.py` & `superlinked-3.9.1/superlinked/framework/common/schema/schema_decorator.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/common/schema/schema_factory.py` & `superlinked-3.9.1/superlinked/framework/common/schema/schema_factory.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/common/schema/schema_object.py` & `superlinked-3.9.1/superlinked/framework/common/schema/schema_object.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/common/schema/schema_reference.py` & `superlinked-3.9.1/superlinked/framework/common/schema/schema_reference.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/common/schema/schema_type.py` & `superlinked-3.9.1/superlinked/framework/common/schema/schema_type.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/common/schema/schema_validator.py` & `superlinked-3.9.1/superlinked/framework/common/schema/schema_validator.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/common/source/source.py` & `superlinked-3.9.1/superlinked/framework/common/source/source.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/common/source/types.py` & `superlinked-3.9.1/superlinked/framework/common/source/types.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/common/storage/persistence_type.py` & `superlinked-3.9.1/superlinked/framework/common/storage/persistence_type.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/common/util/class_helper.py` & `superlinked-3.9.1/superlinked/framework/common/util/class_helper.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/common/util/dot_separated_path_util.py` & `superlinked-3.9.1/superlinked/framework/common/util/dot_separated_path_util.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/common/util/immutable_model.py` & `superlinked-3.9.1/superlinked/framework/common/util/immutable_model.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/common/util/named_function_evaluator.py` & `superlinked-3.9.1/superlinked/framework/common/util/named_function_evaluator.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/common/util/schema_util.py` & `superlinked-3.9.1/superlinked/framework/common/util/schema_util.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/common/util/time_util.py` & `superlinked-3.9.1/superlinked/framework/common/util/time_util.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/common/util/type_validator.py` & `superlinked-3.9.1/superlinked/framework/common/util/type_validator.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/compiler/online_schema_dag_compiler.py` & `superlinked-3.9.1/superlinked/framework/compiler/online_schema_dag_compiler.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/dsl/executor/exception.py` & `superlinked-3.9.1/superlinked/framework/dsl/executor/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/dsl/executor/executor.py` & `superlinked-3.9.1/superlinked/framework/dsl/executor/executor.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/dsl/executor/in_memory/in_memory_executor.py` & `superlinked-3.9.1/superlinked/framework/dsl/executor/in_memory/in_memory_executor.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/dsl/executor/query/query_executor.py` & `superlinked-3.9.1/superlinked/framework/dsl/executor/query/query_executor.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/dsl/executor/rest/rest_configuration.py` & `superlinked-3.9.1/superlinked/framework/dsl/executor/rest/rest_configuration.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/dsl/executor/rest/rest_descriptor.py` & `superlinked-3.9.1/superlinked/framework/dsl/executor/rest/rest_descriptor.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/dsl/executor/rest/rest_executor.py` & `superlinked-3.9.1/superlinked/framework/dsl/executor/rest/rest_executor.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/dsl/executor/rest/rest_handler.py` & `superlinked-3.9.1/superlinked/framework/dsl/executor/rest/rest_handler.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/dsl/index/effect.py` & `superlinked-3.9.1/superlinked/framework/dsl/index/effect.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/dsl/index/index.py` & `superlinked-3.9.1/superlinked/framework/dsl/index/index.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/dsl/index/util/aggregation_effect_group.py` & `superlinked-3.9.1/superlinked/framework/dsl/index/util/aggregation_effect_group.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/dsl/index/util/aggregation_node_util.py` & `superlinked-3.9.1/superlinked/framework/dsl/index/util/aggregation_node_util.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/dsl/index/util/effect_with_referenced_schema_object.py` & `superlinked-3.9.1/superlinked/framework/dsl/index/util/effect_with_referenced_schema_object.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/dsl/index/util/event_aggregation_effect_group.py` & `superlinked-3.9.1/superlinked/framework/dsl/index/util/event_aggregation_effect_group.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/dsl/index/util/event_aggregation_node_util.py` & `superlinked-3.9.1/superlinked/framework/dsl/index/util/event_aggregation_node_util.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/dsl/query/param.py` & `superlinked-3.9.1/superlinked/framework/dsl/query/param.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/dsl/query/param_evaluator.py` & `superlinked-3.9.1/superlinked/framework/dsl/query/param_evaluator.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/dsl/query/predicate/binary_op.py` & `superlinked-3.9.1/superlinked/framework/dsl/query/predicate/binary_op.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/dsl/query/predicate/binary_predicate.py` & `superlinked-3.9.1/superlinked/framework/dsl/query/predicate/binary_predicate.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/dsl/query/predicate/evaluated_binary_predicate.py` & `superlinked-3.9.1/superlinked/framework/dsl/query/predicate/evaluated_binary_predicate.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/dsl/query/predicate/query_predicate.py` & `superlinked-3.9.1/superlinked/framework/dsl/query/predicate/query_predicate.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/dsl/query/query.py` & `superlinked-3.9.1/superlinked/framework/dsl/query/query.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/dsl/query/query_filters.py` & `superlinked-3.9.1/superlinked/framework/dsl/query/query_filters.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/dsl/query/query_vector_factory.py` & `superlinked-3.9.1/superlinked/framework/dsl/query/query_vector_factory.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/dsl/query/query_weighting.py` & `superlinked-3.9.1/superlinked/framework/dsl/query/query_weighting.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/dsl/query/result.py` & `superlinked-3.9.1/superlinked/framework/dsl/query/result.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/dsl/source/in_memory_source.py` & `superlinked-3.9.1/superlinked/framework/dsl/source/in_memory_source.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/dsl/source/rest_source.py` & `superlinked-3.9.1/superlinked/framework/dsl/source/rest_source.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/dsl/source/source.py` & `superlinked-3.9.1/superlinked/framework/dsl/source/source.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/dsl/space/exception.py` & `superlinked-3.9.1/superlinked/framework/dsl/space/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/dsl/space/number_space.py` & `superlinked-3.9.1/superlinked/framework/dsl/space/number_space.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/dsl/space/recency_space.py` & `superlinked-3.9.1/superlinked/framework/dsl/space/recency_space.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/dsl/space/space.py` & `superlinked-3.9.1/superlinked/framework/dsl/space/space.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/dsl/space/space_field_set.py` & `superlinked-3.9.1/superlinked/framework/dsl/space/space_field_set.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/dsl/space/text_similarity_space.py` & `superlinked-3.9.1/superlinked/framework/dsl/space/text_similarity_space.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/evaluator/dag_evaluator.py` & `superlinked-3.9.1/superlinked/framework/evaluator/dag_evaluator.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/evaluator/online_dag_evaluator.py` & `superlinked-3.9.1/superlinked/framework/evaluator/online_dag_evaluator.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/evaluator/query_dag_evaluator.py` & `superlinked-3.9.1/superlinked/framework/evaluator/query_dag_evaluator.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/online/dag/default_online_node.py` & `superlinked-3.9.1/superlinked/framework/online/dag/default_online_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/online/dag/evaluation_result.py` & `superlinked-3.9.1/superlinked/framework/online/dag/evaluation_result.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/online/dag/exception.py` & `superlinked-3.9.1/superlinked/framework/online/dag/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/online/dag/online_aggregation_node.py` & `superlinked-3.9.1/superlinked/framework/online/dag/online_aggregation_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/online/dag/online_chunking_node.py` & `superlinked-3.9.1/superlinked/framework/online/dag/online_chunking_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/online/dag/online_comparison_filter_node.py` & `superlinked-3.9.1/superlinked/framework/online/dag/online_comparison_filter_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/online/dag/online_concatenation_node.py` & `superlinked-3.9.1/superlinked/framework/online/dag/online_concatenation_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/online/dag/online_constant_node.py` & `superlinked-3.9.1/superlinked/framework/online/dag/online_constant_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/online/dag/online_event_aggregation_node.py` & `superlinked-3.9.1/superlinked/framework/online/dag/online_event_aggregation_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/online/dag/online_index_node.py` & `superlinked-3.9.1/superlinked/framework/online/dag/online_index_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/online/dag/online_named_function_node.py` & `superlinked-3.9.1/superlinked/framework/online/dag/online_named_function_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/online/dag/online_node.py` & `superlinked-3.9.1/superlinked/framework/online/dag/online_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/online/dag/online_number_embedding_node.py` & `superlinked-3.9.1/superlinked/framework/online/dag/online_number_embedding_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/online/dag/online_number_similarity_node.py` & `superlinked-3.9.1/superlinked/framework/online/dag/online_number_similarity_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/online/dag/online_recency_node.py` & `superlinked-3.9.1/superlinked/framework/online/dag/online_recency_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/online/dag/online_schema_dag.py` & `superlinked-3.9.1/superlinked/framework/online/dag/online_schema_dag.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/online/dag/online_schema_field_node.py` & `superlinked-3.9.1/superlinked/framework/online/dag/online_schema_field_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/online/dag/online_text_embedding_node.py` & `superlinked-3.9.1/superlinked/framework/online/dag/online_text_embedding_node.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/online/source/in_memory_data_processor.py` & `superlinked-3.9.1/superlinked/framework/online/source/in_memory_data_processor.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/online/source/in_memory_object_writer.py` & `superlinked-3.9.1/superlinked/framework/online/source/in_memory_object_writer.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/online/source/in_memory_source.py` & `superlinked-3.9.1/superlinked/framework/online/source/in_memory_source.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/online/store_manager/evaluation_result_store_manager.py` & `superlinked-3.9.1/superlinked/framework/online/store_manager/evaluation_result_store_manager.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/storage/entity.py` & `superlinked-3.9.1/superlinked/framework/storage/entity.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/storage/entity_store.py` & `superlinked-3.9.1/superlinked/framework/storage/entity_store.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/storage/entity_store_manager.py` & `superlinked-3.9.1/superlinked/framework/storage/entity_store_manager.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/storage/field.py` & `superlinked-3.9.1/superlinked/framework/storage/field.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/storage/in_memory_entity_store.py` & `superlinked-3.9.1/superlinked/framework/storage/in_memory_entity_store.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/storage/in_memory_object_store.py` & `superlinked-3.9.1/superlinked/framework/storage/in_memory_object_store.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/storage/object_store.py` & `superlinked-3.9.1/superlinked/framework/storage/object_store.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/superlinked/framework/storage/object_store_manager.py` & `superlinked-3.9.1/superlinked/framework/storage/object_store_manager.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.0/PKG-INFO` & `superlinked-3.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superlinked
-Version: 3.9.0
+Version: 3.9.1
 Summary: The Superlinked vector computing library
 License: Apache-2.0
 Author: Superlinked Release
 Author-email: release@superlinked.com
 Requires-Python: >=3.10,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -22,25 +22,26 @@
 Requires-Dist: boto3-stubs[s3] (==1.34.13) ; extra == "deployment-poller"
 Requires-Dist: cerberus (==1.3.5) ; extra == "deployment-executor" or extra == "deployment-poller"
 Requires-Dist: dask[complete,distributed] (==2024.1.0) ; extra == "deployment-executor"
 Requires-Dist: deltalake (==0.15.1) ; extra == "deployment-executor"
 Requires-Dist: fastapi (==0.109.0) ; extra == "deployment-executor"
 Requires-Dist: fastapi-restful (>=0.5.0,<0.6.0) ; extra == "deployment-executor"
 Requires-Dist: fsspec (==2023.12.2) ; extra == "deployment-executor"
-Requires-Dist: furl (>=2.1.3,<3.0.0) ; extra == "deployment-executor"
+Requires-Dist: furl (>=2.1.3,<3.0.0)
 Requires-Dist: gcsfs (==2023.12.2.post1) ; extra == "deployment-executor"
 Requires-Dist: google-auth (==2.26.1) ; extra == "deployment-poller"
 Requires-Dist: google-cloud-storage (==2.14.0) ; extra == "deployment-poller"
 Requires-Dist: graphviz (>=0.20.1,<0.21.0) ; extra == "profiler"
 Requires-Dist: httpx (==0.26.0) ; extra == "deployment-executor"
 Requires-Dist: inject (>=5.2.0,<6.0.0) ; extra == "deployment-executor"
 Requires-Dist: ipywidgets (==8.1.2) ; extra == "interactive"
 Requires-Dist: jupyter (>=1.0.0,<2.0.0) ; extra == "interactive" or extra == "profiler"
 Requires-Dist: numpy (==1.22.4)
 Requires-Dist: pandas (>=2.2.1,<3.0.0)
+Requires-Dist: pydantic (>=2.6.4,<3.0.0)
 Requires-Dist: pydantic-settings (>=2.2.1,<3.0.0) ; extra == "deployment-executor"
 Requires-Dist: pyspark (==3.5.0) ; extra == "batch"
 Requires-Dist: pyyaml (==6.0.1) ; extra == "deployment-poller"
 Requires-Dist: requests (==2.27.1) ; extra == "deployment-poller"
 Requires-Dist: s3fs (==2023.12.2) ; extra == "deployment-executor"
 Requires-Dist: sentence-transformers (==2.2.2)
 Requires-Dist: snakeviz (>=2.2.0,<2.3.0) ; extra == "profiler"
```

