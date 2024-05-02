# Comparing `tmp/nucliadb_node_binding-3.0.3.post1233.tar.gz` & `tmp/nucliadb_node_binding-3.0.3.post1240.tar.gz`

## Comparing `nucliadb_node_binding-3.0.3.post1233.tar` & `nucliadb_node_binding-3.0.3.post1240.tar`

### file list

```diff
@@ -1,283 +1,284 @@
--rw-r--r--   0        0        0      708 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_relations2/Cargo.toml
--rw-r--r--   0     1001      127     3593 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_relations2/src/io_maps.rs
--rw-r--r--   0     1001      127      916 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_relations2/src/lib.rs
--rw-r--r--   0     1001      127    17039 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_relations2/src/reader.rs
--rw-r--r--   0     1001      127     7123 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_relations2/src/schema.rs
--rw-r--r--   0     1001      127     8007 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_relations2/src/writer.rs
--rw-r--r--   0     1001      127     1802 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_relations2/tests/common/mod.rs
--rw-r--r--   0     1001      127     9445 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_relations2/tests/test_reader.rs
--rw-r--r--   0     1001      127     3297 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_relations2/tests/test_writer.rs
--rw-r--r--   0        0        0      399 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_texts2/Cargo.toml
--rw-r--r--   0     1001      127      931 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_texts2/src/lib.rs
--rw-r--r--   0     1001      127     2755 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_texts2/src/query_io.rs
--rw-r--r--   0     1001      127    22721 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_texts2/src/reader.rs
--rw-r--r--   0     1001      127     3105 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_texts2/src/schema.rs
--rw-r--r--   0     1001      127     8682 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_texts2/src/search_query.rs
--rw-r--r--   0     1001      127    10109 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_texts2/src/writer.rs
--rw-r--r--   0     1001      127     3396 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_texts2/tests/common/mod.rs
--rw-r--r--   0     1001      127     2068 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_texts2/tests/test_reader.rs
--rw-r--r--   0     1001      127     9567 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_texts2/tests/test_search.rs
--rw-r--r--   0     1001      127     1249 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_texts2/tests/test_streaming.rs
--rw-r--r--   0     1001      127     3469 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_texts2/tests/test_writer.rs
--rw-r--r--   0        0        0      931 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_core/Cargo.toml
--rw-r--r--   0     1001      127     5872 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_core/src/fs_state.rs
--rw-r--r--   0     1001      127     2969 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_core/src/lib.rs
--rw-r--r--   0     1001      127     2295 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_core/src/merge.rs
--rw-r--r--   0     1001      127      906 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_core/src/metrics/meters/mod.rs
--rw-r--r--   0     1001      127     4869 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_core/src/metrics/meters/prometheus.rs
--rw-r--r--   0     1001      127     1702 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_core/src/metrics/metric/grpc_ops.rs
--rw-r--r--   0     1001      127     1442 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_core/src/metrics/metric/mod.rs
--rw-r--r--   0     1001      127     1950 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_core/src/metrics/metric/replication.rs
--rw-r--r--   0     1001      127     2626 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_core/src/metrics/metric/request_time.rs
--rw-r--r--   0     1001      127     1644 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_core/src/metrics/metric/shard_cache.rs
--rw-r--r--   0     1001      127    21641 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_core/src/metrics/metric/tokio_runtime.rs
--rw-r--r--   0     1001      127    16736 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_core/src/metrics/metric/tokio_tasks.rs
--rw-r--r--   0     1001      127     3415 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_core/src/metrics/metric/vectors.rs
--rw-r--r--   0     1001      127     1324 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_core/src/metrics/mod.rs
--rw-r--r--   0     1001      127     3074 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_core/src/metrics/task_monitor.rs
--rw-r--r--   0     1001      127     3920 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_core/src/metrics/tests.rs
--rw-r--r--   0     1001      127     2990 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_core/src/paragraphs.rs
--rw-r--r--   0     1001      127    17305 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_core/src/query_language/mod.rs
--rw-r--r--   0     1001      127    15367 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_core/src/query_planner.rs
--rw-r--r--   0     1001      127     2069 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_core/src/relations.rs
--rw-r--r--   0     1001      127     8250 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_core/src/tantivy_replica.rs
--rw-r--r--   0     1001      127     2603 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_core/src/texts.rs
--rw-r--r--   0     1001      127     3559 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_core/src/vectors.rs
--rw-r--r--   0        0        0      629 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/Cargo.toml
--rw-r--r--   0     1001      127     7796 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/src/fuzzy_query.rs
--rw-r--r--   0     1001      127     1024 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/src/lib.rs
--rw-r--r--   0     1001      127     2780 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/src/query_io.rs
--rw-r--r--   0     1001      127    42885 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/src/reader.rs
--rw-r--r--   0     1001      127     4407 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/src/schema.rs
--rw-r--r--   0     1001      127    21349 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/src/search_query.rs
--rw-r--r--   0     1001      127    11723 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/src/search_response.rs
--rw-r--r--   0     1001      127     2846 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/src/set_query.rs
--rw-r--r--   0     1001      127     4090 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/src/stop_words.rs
--rw-r--r--   0     1001      127    17057 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/src/writer.rs
--rw-r--r--   0     1001      127       88 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/stop_words/README.md
--rw-r--r--   0     1001      127    19791 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/stop_words/ar.json
--rw-r--r--   0     1001      127     1923 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/stop_words/az.json
--rw-r--r--   0     1001      127    11684 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/stop_words/bn.json
--rw-r--r--   0     1001      127     2513 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/stop_words/ca.json
--rw-r--r--   0     1001      127    12802 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/stop_words/ch.json
--rw-r--r--   0     1001      127      730 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/stop_words/da.json
--rw-r--r--   0     1001      127     2090 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/stop_words/de.json
--rw-r--r--   0     1001      127     6284 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/stop_words/el.json
--rw-r--r--   0     1001      127     1473 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/stop_words/en.json
--rw-r--r--   0     1001      127     3451 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/stop_words/es.json
--rw-r--r--   0     1001      127     3182 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/stop_words/eu.json
--rw-r--r--   0     1001      127     2126 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/stop_words/extract.py
--rw-r--r--   0     1001      127     2748 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/stop_words/fi.json
--rw-r--r--   0     1001      127     1388 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/stop_words/fr.json
--rw-r--r--   0     1001      127     5716 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/stop_words/he.json
--rw-r--r--   0     1001      127     2108 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/stop_words/hu.json
--rw-r--r--   0     1001      127     8721 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/stop_words/id.json
--rw-r--r--   0     1001      127     2535 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/stop_words/it.json
--rw-r--r--   0     1001      127    11737 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/stop_words/kk.json
--rw-r--r--   0     1001      127     7730 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/stop_words/ne.json
--rw-r--r--   0     1001      127      756 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/stop_words/nl.json
--rw-r--r--   0     1001      127     1447 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/stop_words/no.json
--rw-r--r--   0     1001      127     2055 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/stop_words/pt.json
--rw-r--r--   0     1001      127     3327 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/stop_words/ro.json
--rw-r--r--   0     1001      127     3856 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/stop_words/ru.json
--rw-r--r--   0     1001      127    23032 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/stop_words/sl.json
--rw-r--r--   0     1001      127      993 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/stop_words/sv.json
--rw-r--r--   0     1001      127     5424 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/stop_words/tg.json
--rw-r--r--   0     1001      127      491 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/stop_words/tr.json
--rw-r--r--   0        0        0      742 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_vectors/Cargo.toml
--rw-r--r--   0     1001      127       69 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_vectors/README.md
--rw-r--r--   0     1001      127       43 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_vectors/docs/README.md
--rw-r--r--   0     1001      127    25718 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_vectors/docs/labels.drawio.svg
--rw-r--r--   0     1001      127    12340 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_vectors/src/data_point/disk_hnsw.rs
--rw-r--r--   0     1001      127    24470 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_vectors/src/data_point/mod.rs
--rw-r--r--   0     1001      127    11214 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_vectors/src/data_point/node.rs
--rw-r--r--   0     1001      127    14638 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_vectors/src/data_point/ops_hnsw.rs
--rw-r--r--   0     1001      127     1642 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_vectors/src/data_point/params.rs
--rw-r--r--   0     1001      127     3952 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_vectors/src/data_point/ram_hnsw.rs
--rw-r--r--   0     1001      127    14175 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_vectors/src/data_point/tests.rs
--rw-r--r--   0     1001      127     5798 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_vectors/src/data_point_provider/garbage_collector.rs
--rw-r--r--   0     1001      127     2777 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_vectors/src/data_point_provider/mod.rs
--rw-r--r--   0     1001      127    10613 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_vectors/src/data_point_provider/reader.rs
--rw-r--r--   0     1001      127     2304 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_vectors/src/data_point_provider/replication.rs
--rw-r--r--   0     1001      127     5288 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_vectors/src/data_point_provider/state.rs
--rw-r--r--   0     1001      127    20587 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_vectors/src/data_point_provider/writer.rs
--rw-r--r--   0     1001      127    23710 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_vectors/src/data_types/data_store.rs
--rw-r--r--   0     1001      127     6916 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_vectors/src/data_types/dtrie_ram.rs
--rw-r--r--   0     1001      127     1959 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_vectors/src/data_types/mod.rs
--rw-r--r--   0     1001      127     6143 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_vectors/src/data_types/trie.rs
--rw-r--r--   0     1001      127     2904 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_vectors/src/data_types/trie_ram.rs
--rw-r--r--   0     1001      127     4433 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_vectors/src/data_types/vector.rs
--rw-r--r--   0     1001      127    10472 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_vectors/src/formula/mod.rs
--rw-r--r--   0     1001      127     2165 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_vectors/src/lib.rs
--rw-r--r--   0     1001      127     1278 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_vectors/src/service/mod.rs
--rw-r--r--   0     1001      127     1897 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_vectors/src/service/query_io.rs
--rw-r--r--   0     1001      127    17192 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_vectors/src/service/reader.rs
--rw-r--r--   0     1001      127    15294 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_vectors/src/service/writer.rs
--rw-r--r--   0     1001      127     1668 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_vectors/src/utils.rs
--rw-r--r--   0     1001      127     2884 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_vectors/tests/test_merge.rs
--rw-r--r--   0        0        0     3212 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/Cargo.toml
--rw-r--r--   0     1001      127     1045 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/.rustc_info.json
--rw-r--r--   0     1001      127      877 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/Makefile
--rw-r--r--   0     1001      127     1500 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/README.md
--rw-r--r--   0     1001      127     1757 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/nucliadb_node/__init__.py
--rw-r--r--   0     1001      127     3957 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/nucliadb_node/app.py
--rw-r--r--   0     1001      127    17752 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/nucliadb_node/indexer.py
--rw-r--r--   0     1001      127      890 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/nucliadb_node/listeners/__init__.py
--rw-r--r--   0     1001      127     2424 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/nucliadb_node/listeners/indexed_publisher.py
--rw-r--r--   0     1001      127     4015 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/nucliadb_node/pull.py
--rw-r--r--   0     1001      127     1535 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/nucliadb_node/service.py
--rw-r--r--   0     1001      127     1487 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/nucliadb_node/settings.py
--rw-r--r--   0     1001      127     1133 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/nucliadb_node/signals.py
--rw-r--r--   0     1001      127      835 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/nucliadb_node/tests/__init__.py
--rw-r--r--   0     1001      127     1092 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/nucliadb_node/tests/conftest.py
--rw-r--r--   0     1001      127    10810 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/nucliadb_node/tests/fixtures.py
--rw-r--r--   0     1001      127    13788 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/nucliadb_node/tests/integration/test_indexing.py
--rw-r--r--   0     1001      127     2289 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_app.py
--rw-r--r--   0     1001      127     2361 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexed_publisher.py
--rw-r--r--   0     1001      127    12553 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexer.py
--rw-r--r--   0     1001      127     3379 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_pull.py
--rw-r--r--   0     1001      127     2323 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/nucliadb_node/writer.py
--rw-r--r--   0     1001      127      101 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/requirements-sources.txt
--rw-r--r--   0     1001      127      276 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/requirements.txt
--rw-r--r--   0     1001      127      249 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/setup.cfg
--rw-r--r--   0     1001      127     1405 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/setup.py
--rw-r--r--   0     1001      127     2518 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/analytics/blocking.rs
--rw-r--r--   0     1001      127     1219 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/analytics/mod.rs
--rw-r--r--   0     1001      127     4931 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/analytics/payload.rs
--rw-r--r--   0     1001      127    12828 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/analytics/sender.rs
--rw-r--r--   0     1001      127     3085 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/analytics/sink.rs
--rw-r--r--   0     1001      127     1900 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/analytics/sync.rs
--rw-r--r--   0     1001      127     5045 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/bin/reader.rs
--rw-r--r--   0     1001      127     8050 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/bin/writer.rs
--rw-r--r--   0     1001      127     1345 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/cache/mod.rs
--rw-r--r--   0     1001      127     3035 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/cache/reader_cache.rs
--rw-r--r--   0     1001      127    14199 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/cache/resource_cache.rs
--rw-r--r--   0     1001      127    11265 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/cache/writer_cache.rs
--rw-r--r--   0     1001      127     1771 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/disk_structure.rs
--rw-r--r--   0     1001      127     1111 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/errors.rs
--rw-r--r--   0     1001      127     2656 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/grpc/collect_garbage.rs
--rw-r--r--   0     1001      127    18813 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/grpc/grpc_reader.rs
--rw-r--r--   0     1001      127    13710 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/grpc/grpc_writer.rs
--rw-r--r--   0     1001      127     3186 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/grpc/middleware/debug.rs
--rw-r--r--   0     1001      127     3440 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/grpc/middleware/metrics.rs
--rw-r--r--   0     1001      127     1009 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/grpc/middleware/mod.rs
--rw-r--r--   0     1001      127     4158 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/grpc/middleware/telemetry.rs
--rw-r--r--   0     1001      127     1283 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/grpc/mod.rs
--rw-r--r--   0     1001      127     2581 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/grpc/update.rs
--rw-r--r--   0     1001      127     1173 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/http_server/metrics_service.rs
--rw-r--r--   0     1001      127     1465 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/http_server/mod.rs
--rw-r--r--   0     1001      127     1943 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/http_server/traces_service.rs
--rw-r--r--   0     1001      127     1504 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/lib.rs
--rw-r--r--   0     1001      127     2757 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/lifecycle.rs
--rw-r--r--   0     1001      127     1778 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/merge/global.rs
--rw-r--r--   0     1001      127     1089 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/merge/mod.rs
--rw-r--r--   0     1001      127    13672 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/merge/scheduler.rs
--rw-r--r--   0     1001      127     3677 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/merge/work.rs
--rw-r--r--   0     1001      127     1935 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/node_metadata.rs
--rw-r--r--   0     1001      127     2417 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/replication/health.rs
--rw-r--r--   0     1001      127     1070 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/replication/mod.rs
--rw-r--r--   0     1001      127    14144 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/replication/replicator.rs
--rw-r--r--   0     1001      127    11803 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/replication/service.rs
--rw-r--r--   0     1001      127    11615 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/settings.rs
--rw-r--r--   0     1001      127     1111 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/shards/errors.rs
--rw-r--r--   0     1001      127    11052 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/shards/metadata.rs
--rw-r--r--   0     1001      127     1127 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/shards/mod.rs
--rw-r--r--   0     1001      127    27129 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/shards/shard_reader.rs
--rw-r--r--   0     1001      127    23537 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/shards/shard_writer.rs
--rw-r--r--   0     1001      127     1887 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/shards/versioning.rs
--rw-r--r--   0     1001      127    10170 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/telemetry.rs
--rw-r--r--   0     1001      127     6396 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/utils.rs
--rw-r--r--   0     1001      127       42 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/test.sh
--rw-r--r--   0     1001      127     1115 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/tests/common/mod.rs
--rw-r--r--   0     1001      127    12731 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/tests/common/node_services.rs
--rw-r--r--   0     1001      127     7823 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/tests/common/resources.rs
--rw-r--r--   0     1001      127     8173 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/tests/test_date_range_search.rs
--rw-r--r--   0     1001      127     4089 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/tests/test_download.rs
--rw-r--r--   0     1001      127     1684 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/tests/test_merge.rs
--rw-r--r--   0     1001      127     6003 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/tests/test_replication.rs
--rw-r--r--   0     1001      127    22494 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/tests/test_search_relations.rs
--rw-r--r--   0     1001      127     6958 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/tests/test_search_sorting.rs
--rw-r--r--   0     1001      127     7044 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/tests/test_security_search.rs
--rw-r--r--   0     1001      127     6862 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/tests/test_shards.rs
--rw-r--r--   0     1001      127    10698 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/tests/test_suggest.rs
--rw-r--r--   0     1001      127     5438 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/tests/test_vector_normalization.rs
--rw-r--r--   0        0        0      629 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/Cargo.toml
--rw-r--r--   0     1001      127     7796 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/src/fuzzy_query.rs
--rw-r--r--   0     1001      127     1009 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/src/lib.rs
--rw-r--r--   0     1001      127     2780 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/src/query_io.rs
--rw-r--r--   0     1001      127    42940 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/src/reader.rs
--rw-r--r--   0     1001      127     4808 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/src/schema.rs
--rw-r--r--   0     1001      127    22494 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/src/search_query.rs
--rw-r--r--   0     1001      127    11391 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/src/search_response.rs
--rw-r--r--   0     1001      127     4090 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/src/stop_words.rs
--rw-r--r--   0     1001      127    17965 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/src/writer.rs
--rw-r--r--   0     1001      127       88 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/stop_words/README.md
--rw-r--r--   0     1001      127    19791 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/stop_words/ar.json
--rw-r--r--   0     1001      127     1923 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/stop_words/az.json
--rw-r--r--   0     1001      127    11684 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/stop_words/bn.json
--rw-r--r--   0     1001      127     2513 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/stop_words/ca.json
--rw-r--r--   0     1001      127    12802 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/stop_words/ch.json
--rw-r--r--   0     1001      127      730 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/stop_words/da.json
--rw-r--r--   0     1001      127     2090 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/stop_words/de.json
--rw-r--r--   0     1001      127     6284 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/stop_words/el.json
--rw-r--r--   0     1001      127     1473 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/stop_words/en.json
--rw-r--r--   0     1001      127     3451 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/stop_words/es.json
--rw-r--r--   0     1001      127     3182 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/stop_words/eu.json
--rw-r--r--   0     1001      127     2126 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/stop_words/extract.py
--rw-r--r--   0     1001      127     2748 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/stop_words/fi.json
--rw-r--r--   0     1001      127     1388 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/stop_words/fr.json
--rw-r--r--   0     1001      127     5716 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/stop_words/he.json
--rw-r--r--   0     1001      127     2108 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/stop_words/hu.json
--rw-r--r--   0     1001      127     8721 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/stop_words/id.json
--rw-r--r--   0     1001      127     2535 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/stop_words/it.json
--rw-r--r--   0     1001      127    11737 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/stop_words/kk.json
--rw-r--r--   0     1001      127     7730 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/stop_words/ne.json
--rw-r--r--   0     1001      127      756 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/stop_words/nl.json
--rw-r--r--   0     1001      127     1447 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/stop_words/no.json
--rw-r--r--   0     1001      127     2055 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/stop_words/pt.json
--rw-r--r--   0     1001      127     3327 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/stop_words/ro.json
--rw-r--r--   0     1001      127     3856 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/stop_words/ru.json
--rw-r--r--   0     1001      127    23032 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/stop_words/sl.json
--rw-r--r--   0     1001      127      993 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/stop_words/sv.json
--rw-r--r--   0     1001      127     5424 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/stop_words/tg.json
--rw-r--r--   0     1001      127      491 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/stop_words/tr.json
--rw-r--r--   0        0        0      361 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_procs/Cargo.toml
--rw-r--r--   0     1001      127     3409 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_procs/src/lib.rs
--rw-r--r--   0     1001      127     2885 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_procs/src/measure.rs
--rw-r--r--   0     1001      127     1081 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.rs
--rw-r--r--   0     1001      127      222 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.stderr
--rw-r--r--   0     1001      127     1038 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.rs
--rw-r--r--   0     1001      127      327 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.stderr
--rw-r--r--   0     1001      127     1086 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.rs
--rw-r--r--   0     1001      127      249 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.stderr
--rw-r--r--   0     1001      127     1046 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.rs
--rw-r--r--   0     1001      127     1303 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.stderr
--rw-r--r--   0     1001      127     1408 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_procs/tests/test_measure.rs
--rw-r--r--   0        0        0      501 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_protos/Cargo.toml
--rw-r--r--   0     1001      127     2155 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_protos/build.rs
--rw-r--r--   0     1001      127    26110 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_protos/src/fdbwriter.rs
--rw-r--r--   0     1001      127        0 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_protos/src/google.protobuf.rs
--rw-r--r--   0     1001      127     9795 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_protos/src/knowledgebox.rs
--rw-r--r--   0     1001      127     1256 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_protos/src/lib.rs
--rw-r--r--   0     1001      127    77311 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_protos/src/nodereader.rs
--rw-r--r--   0     1001      127    10240 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_protos/src/noderesources.rs
--rw-r--r--   0     1001      127    43352 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_protos/src/nodewriter.rs
--rw-r--r--   0     1001      127    19106 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_protos/src/replication.rs
--rw-r--r--   0     1001      127    33352 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_protos/src/resources.rs
--rw-r--r--   0     1001      127     5528 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_protos/src/utils.rs
--rw-r--r--   0        0        0      943 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1233/Cargo.toml
--rw-r--r--   0     1001      127     1553 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/CHANGELOG.md
--rw-r--r--   0     1001      127      895 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/Makefile
--rw-r--r--   0     1001      127       52 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/README.md
--rwxr-xr-x   0     1001      127      978 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/cov.sh
--rw-r--r--   0     1001      127     1309 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/pyproject.toml
--rw-r--r--   0     1001      127     2195 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/src/collect_garbage.rs
--rw-r--r--   0     1001      127     1212 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/src/errors.rs
--rw-r--r--   0     1001      127     2337 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/src/lib.rs
--rw-r--r--   0     1001      127     9405 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/src/reader.rs
--rw-r--r--   0     1001      127     2154 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/src/update.rs
--rw-r--r--   0     1001      127     9150 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/src/writer.rs
--rw-r--r--   0     1001      127      835 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/tests/__init__.py
--rw-r--r--   0     1001      127      892 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/tests/conftest.py
--rw-r--r--   0     1001      127     3903 2024-04-30 12:16:54.000000 nucliadb_node_binding-3.0.3.post1233/tests/integration/test_indexing.py
--rw-r--r--   0        0        0      401 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1233/PKG-INFO
+-rw-r--r--   0        0        0      742 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_vectors/Cargo.toml
+-rw-r--r--   0     1001      127       69 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_vectors/README.md
+-rw-r--r--   0     1001      127       43 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_vectors/docs/README.md
+-rw-r--r--   0     1001      127    25718 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_vectors/docs/labels.drawio.svg
+-rw-r--r--   0     1001      127    12340 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_vectors/src/data_point/disk_hnsw.rs
+-rw-r--r--   0     1001      127    24470 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_vectors/src/data_point/mod.rs
+-rw-r--r--   0     1001      127    11214 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_vectors/src/data_point/node.rs
+-rw-r--r--   0     1001      127    14638 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_vectors/src/data_point/ops_hnsw.rs
+-rw-r--r--   0     1001      127     1642 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_vectors/src/data_point/params.rs
+-rw-r--r--   0     1001      127     3952 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_vectors/src/data_point/ram_hnsw.rs
+-rw-r--r--   0     1001      127    14175 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_vectors/src/data_point/tests.rs
+-rw-r--r--   0     1001      127     5798 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_vectors/src/data_point_provider/garbage_collector.rs
+-rw-r--r--   0     1001      127     2777 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_vectors/src/data_point_provider/mod.rs
+-rw-r--r--   0     1001      127    10613 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_vectors/src/data_point_provider/reader.rs
+-rw-r--r--   0     1001      127     2304 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_vectors/src/data_point_provider/replication.rs
+-rw-r--r--   0     1001      127     5288 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_vectors/src/data_point_provider/state.rs
+-rw-r--r--   0     1001      127    20587 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_vectors/src/data_point_provider/writer.rs
+-rw-r--r--   0     1001      127    23710 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_vectors/src/data_types/data_store.rs
+-rw-r--r--   0     1001      127     6916 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_vectors/src/data_types/dtrie_ram.rs
+-rw-r--r--   0     1001      127     1959 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_vectors/src/data_types/mod.rs
+-rw-r--r--   0     1001      127     6143 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_vectors/src/data_types/trie.rs
+-rw-r--r--   0     1001      127     2904 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_vectors/src/data_types/trie_ram.rs
+-rw-r--r--   0     1001      127     4433 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_vectors/src/data_types/vector.rs
+-rw-r--r--   0     1001      127    10472 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_vectors/src/formula/mod.rs
+-rw-r--r--   0     1001      127     2165 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_vectors/src/lib.rs
+-rw-r--r--   0     1001      127     1278 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_vectors/src/service/mod.rs
+-rw-r--r--   0     1001      127     1897 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_vectors/src/service/query_io.rs
+-rw-r--r--   0     1001      127    17192 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_vectors/src/service/reader.rs
+-rw-r--r--   0     1001      127    15294 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_vectors/src/service/writer.rs
+-rw-r--r--   0     1001      127     1668 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_vectors/src/utils.rs
+-rw-r--r--   0     1001      127     2884 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_vectors/tests/test_merge.rs
+-rw-r--r--   0        0        0     3294 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/Cargo.toml
+-rw-r--r--   0     1001      127     1045 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/.rustc_info.json
+-rw-r--r--   0     1001      127      877 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/Makefile
+-rw-r--r--   0     1001      127     1500 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/README.md
+-rw-r--r--   0     1001      127     1757 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/nucliadb_node/__init__.py
+-rw-r--r--   0     1001      127     3957 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/nucliadb_node/app.py
+-rw-r--r--   0     1001      127    19056 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/nucliadb_node/indexer.py
+-rw-r--r--   0     1001      127      890 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/nucliadb_node/listeners/__init__.py
+-rw-r--r--   0     1001      127     2424 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/nucliadb_node/listeners/indexed_publisher.py
+-rw-r--r--   0     1001      127     4015 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/nucliadb_node/pull.py
+-rw-r--r--   0     1001      127     1535 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/nucliadb_node/service.py
+-rw-r--r--   0     1001      127     1487 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/nucliadb_node/settings.py
+-rw-r--r--   0     1001      127     1133 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/nucliadb_node/signals.py
+-rw-r--r--   0     1001      127      835 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/nucliadb_node/tests/__init__.py
+-rw-r--r--   0     1001      127     1092 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/nucliadb_node/tests/conftest.py
+-rw-r--r--   0     1001      127    11293 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/nucliadb_node/tests/fixtures.py
+-rw-r--r--   0     1001      127    13795 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/nucliadb_node/tests/integration/test_indexing.py
+-rw-r--r--   0     1001      127     2289 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_app.py
+-rw-r--r--   0     1001      127     2361 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexed_publisher.py
+-rw-r--r--   0     1001      127    12984 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexer.py
+-rw-r--r--   0     1001      127     3379 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_pull.py
+-rw-r--r--   0     1001      127     2489 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/nucliadb_node/writer.py
+-rw-r--r--   0     1001      127      101 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/requirements-sources.txt
+-rw-r--r--   0     1001      127      276 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/requirements.txt
+-rw-r--r--   0     1001      127      249 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/setup.cfg
+-rw-r--r--   0     1001      127     1405 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/setup.py
+-rw-r--r--   0     1001      127     2518 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/analytics/blocking.rs
+-rw-r--r--   0     1001      127     1219 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/analytics/mod.rs
+-rw-r--r--   0     1001      127     4931 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/analytics/payload.rs
+-rw-r--r--   0     1001      127    12828 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/analytics/sender.rs
+-rw-r--r--   0     1001      127     3085 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/analytics/sink.rs
+-rw-r--r--   0     1001      127     1900 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/analytics/sync.rs
+-rw-r--r--   0     1001      127     5045 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/bin/reader.rs
+-rw-r--r--   0     1001      127     8050 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/bin/writer.rs
+-rw-r--r--   0     1001      127     1345 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/cache/mod.rs
+-rw-r--r--   0     1001      127     3035 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/cache/reader_cache.rs
+-rw-r--r--   0     1001      127    14199 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/cache/resource_cache.rs
+-rw-r--r--   0     1001      127    11265 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/cache/writer_cache.rs
+-rw-r--r--   0     1001      127     1771 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/disk_structure.rs
+-rw-r--r--   0     1001      127     1111 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/errors.rs
+-rw-r--r--   0     1001      127     2656 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/grpc/collect_garbage.rs
+-rw-r--r--   0     1001      127    18813 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/grpc/grpc_reader.rs
+-rw-r--r--   0     1001      127    15105 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/grpc/grpc_writer.rs
+-rw-r--r--   0     1001      127     3186 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/grpc/middleware/debug.rs
+-rw-r--r--   0     1001      127     3440 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/grpc/middleware/metrics.rs
+-rw-r--r--   0     1001      127     1009 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/grpc/middleware/mod.rs
+-rw-r--r--   0     1001      127     4158 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/grpc/middleware/telemetry.rs
+-rw-r--r--   0     1001      127     1283 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/grpc/mod.rs
+-rw-r--r--   0     1001      127     2581 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/grpc/update.rs
+-rw-r--r--   0     1001      127     1173 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/http_server/metrics_service.rs
+-rw-r--r--   0     1001      127     1465 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/http_server/mod.rs
+-rw-r--r--   0     1001      127     1943 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/http_server/traces_service.rs
+-rw-r--r--   0     1001      127     1504 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/lib.rs
+-rw-r--r--   0     1001      127     2757 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/lifecycle.rs
+-rw-r--r--   0     1001      127     1778 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/merge/global.rs
+-rw-r--r--   0     1001      127     1089 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/merge/mod.rs
+-rw-r--r--   0     1001      127    13672 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/merge/scheduler.rs
+-rw-r--r--   0     1001      127     3677 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/merge/work.rs
+-rw-r--r--   0     1001      127     1935 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/node_metadata.rs
+-rw-r--r--   0     1001      127     2417 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/replication/health.rs
+-rw-r--r--   0     1001      127     1070 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/replication/mod.rs
+-rw-r--r--   0     1001      127    14144 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/replication/replicator.rs
+-rw-r--r--   0     1001      127    11803 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/replication/service.rs
+-rw-r--r--   0     1001      127    14210 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/settings.rs
+-rw-r--r--   0     1001      127     1111 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/shards/errors.rs
+-rw-r--r--   0     1001      127    11052 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/shards/metadata.rs
+-rw-r--r--   0     1001      127     1127 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/shards/mod.rs
+-rw-r--r--   0     1001      127    27129 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/shards/shard_reader.rs
+-rw-r--r--   0     1001      127    23537 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/shards/shard_writer.rs
+-rw-r--r--   0     1001      127     1887 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/shards/versioning.rs
+-rw-r--r--   0     1001      127    10170 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/telemetry.rs
+-rw-r--r--   0     1001      127     6396 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/utils.rs
+-rw-r--r--   0     1001      127       42 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/test.sh
+-rw-r--r--   0     1001      127     1115 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/tests/common/mod.rs
+-rw-r--r--   0     1001      127    12731 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/tests/common/node_services.rs
+-rw-r--r--   0     1001      127     7823 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/tests/common/resources.rs
+-rw-r--r--   0     1001      127     8173 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/tests/test_date_range_search.rs
+-rw-r--r--   0     1001      127     4089 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/tests/test_download.rs
+-rw-r--r--   0     1001      127     1684 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/tests/test_merge.rs
+-rw-r--r--   0     1001      127     6003 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/tests/test_replication.rs
+-rw-r--r--   0     1001      127    22494 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/tests/test_search_relations.rs
+-rw-r--r--   0     1001      127     6958 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/tests/test_search_sorting.rs
+-rw-r--r--   0     1001      127     7044 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/tests/test_security_search.rs
+-rw-r--r--   0     1001      127     2402 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/tests/test_set_resource_from_storage.rs
+-rw-r--r--   0     1001      127     6862 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/tests/test_shards.rs
+-rw-r--r--   0     1001      127    10698 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/tests/test_suggest.rs
+-rw-r--r--   0     1001      127     5438 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/tests/test_vector_normalization.rs
+-rw-r--r--   0        0        0      399 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_texts2/Cargo.toml
+-rw-r--r--   0     1001      127      931 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_texts2/src/lib.rs
+-rw-r--r--   0     1001      127     2755 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_texts2/src/query_io.rs
+-rw-r--r--   0     1001      127    22721 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_texts2/src/reader.rs
+-rw-r--r--   0     1001      127     3105 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_texts2/src/schema.rs
+-rw-r--r--   0     1001      127     8682 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_texts2/src/search_query.rs
+-rw-r--r--   0     1001      127    10109 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_texts2/src/writer.rs
+-rw-r--r--   0     1001      127     3396 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_texts2/tests/common/mod.rs
+-rw-r--r--   0     1001      127     2068 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_texts2/tests/test_reader.rs
+-rw-r--r--   0     1001      127     9567 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_texts2/tests/test_search.rs
+-rw-r--r--   0     1001      127     1249 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_texts2/tests/test_streaming.rs
+-rw-r--r--   0     1001      127     3469 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_texts2/tests/test_writer.rs
+-rw-r--r--   0        0        0      361 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_procs/Cargo.toml
+-rw-r--r--   0     1001      127     3409 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_procs/src/lib.rs
+-rw-r--r--   0     1001      127     2885 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_procs/src/measure.rs
+-rw-r--r--   0     1001      127     1081 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.rs
+-rw-r--r--   0     1001      127      222 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.stderr
+-rw-r--r--   0     1001      127     1038 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.rs
+-rw-r--r--   0     1001      127      327 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.stderr
+-rw-r--r--   0     1001      127     1086 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.rs
+-rw-r--r--   0     1001      127      249 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.stderr
+-rw-r--r--   0     1001      127     1046 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.rs
+-rw-r--r--   0     1001      127     1303 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.stderr
+-rw-r--r--   0     1001      127     1408 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_procs/tests/test_measure.rs
+-rw-r--r--   0        0        0      931 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_core/Cargo.toml
+-rw-r--r--   0     1001      127     5872 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_core/src/fs_state.rs
+-rw-r--r--   0     1001      127     2969 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_core/src/lib.rs
+-rw-r--r--   0     1001      127     2295 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_core/src/merge.rs
+-rw-r--r--   0     1001      127      906 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_core/src/metrics/meters/mod.rs
+-rw-r--r--   0     1001      127     5462 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_core/src/metrics/meters/prometheus.rs
+-rw-r--r--   0     1001      127     1702 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_core/src/metrics/metric/grpc_ops.rs
+-rw-r--r--   0     1001      127     1442 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_core/src/metrics/metric/mod.rs
+-rw-r--r--   0     1001      127     1950 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_core/src/metrics/metric/replication.rs
+-rw-r--r--   0     1001      127     2626 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_core/src/metrics/metric/request_time.rs
+-rw-r--r--   0     1001      127     1644 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_core/src/metrics/metric/shard_cache.rs
+-rw-r--r--   0     1001      127    21641 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_core/src/metrics/metric/tokio_runtime.rs
+-rw-r--r--   0     1001      127    16736 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_core/src/metrics/metric/tokio_tasks.rs
+-rw-r--r--   0     1001      127     3415 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_core/src/metrics/metric/vectors.rs
+-rw-r--r--   0     1001      127     1324 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_core/src/metrics/mod.rs
+-rw-r--r--   0     1001      127     3074 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_core/src/metrics/task_monitor.rs
+-rw-r--r--   0     1001      127     3920 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_core/src/metrics/tests.rs
+-rw-r--r--   0     1001      127     2990 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_core/src/paragraphs.rs
+-rw-r--r--   0     1001      127    17305 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_core/src/query_language/mod.rs
+-rw-r--r--   0     1001      127    15367 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_core/src/query_planner.rs
+-rw-r--r--   0     1001      127     2069 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_core/src/relations.rs
+-rw-r--r--   0     1001      127     8250 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_core/src/tantivy_replica.rs
+-rw-r--r--   0     1001      127     2603 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_core/src/texts.rs
+-rw-r--r--   0     1001      127     3559 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_core/src/vectors.rs
+-rw-r--r--   0        0        0      708 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_relations2/Cargo.toml
+-rw-r--r--   0     1001      127     3593 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_relations2/src/io_maps.rs
+-rw-r--r--   0     1001      127      916 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_relations2/src/lib.rs
+-rw-r--r--   0     1001      127    17039 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_relations2/src/reader.rs
+-rw-r--r--   0     1001      127     7123 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_relations2/src/schema.rs
+-rw-r--r--   0     1001      127     8007 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_relations2/src/writer.rs
+-rw-r--r--   0     1001      127     1802 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_relations2/tests/common/mod.rs
+-rw-r--r--   0     1001      127     9445 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_relations2/tests/test_reader.rs
+-rw-r--r--   0     1001      127     3297 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_relations2/tests/test_writer.rs
+-rw-r--r--   0        0        0      629 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/Cargo.toml
+-rw-r--r--   0     1001      127     7796 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/src/fuzzy_query.rs
+-rw-r--r--   0     1001      127     1009 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/src/lib.rs
+-rw-r--r--   0     1001      127     2780 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/src/query_io.rs
+-rw-r--r--   0     1001      127    42940 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/src/reader.rs
+-rw-r--r--   0     1001      127     4808 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/src/schema.rs
+-rw-r--r--   0     1001      127    22494 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/src/search_query.rs
+-rw-r--r--   0     1001      127    11391 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/src/search_response.rs
+-rw-r--r--   0     1001      127     4090 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/src/stop_words.rs
+-rw-r--r--   0     1001      127    17965 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/src/writer.rs
+-rw-r--r--   0     1001      127       88 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/stop_words/README.md
+-rw-r--r--   0     1001      127    19791 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/stop_words/ar.json
+-rw-r--r--   0     1001      127     1923 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/stop_words/az.json
+-rw-r--r--   0     1001      127    11684 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/stop_words/bn.json
+-rw-r--r--   0     1001      127     2513 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/stop_words/ca.json
+-rw-r--r--   0     1001      127    12802 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/stop_words/ch.json
+-rw-r--r--   0     1001      127      730 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/stop_words/da.json
+-rw-r--r--   0     1001      127     2090 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/stop_words/de.json
+-rw-r--r--   0     1001      127     6284 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/stop_words/el.json
+-rw-r--r--   0     1001      127     1473 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/stop_words/en.json
+-rw-r--r--   0     1001      127     3451 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/stop_words/es.json
+-rw-r--r--   0     1001      127     3182 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/stop_words/eu.json
+-rw-r--r--   0     1001      127     2126 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/stop_words/extract.py
+-rw-r--r--   0     1001      127     2748 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/stop_words/fi.json
+-rw-r--r--   0     1001      127     1388 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/stop_words/fr.json
+-rw-r--r--   0     1001      127     5716 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/stop_words/he.json
+-rw-r--r--   0     1001      127     2108 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/stop_words/hu.json
+-rw-r--r--   0     1001      127     8721 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/stop_words/id.json
+-rw-r--r--   0     1001      127     2535 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/stop_words/it.json
+-rw-r--r--   0     1001      127    11737 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/stop_words/kk.json
+-rw-r--r--   0     1001      127     7730 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/stop_words/ne.json
+-rw-r--r--   0     1001      127      756 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/stop_words/nl.json
+-rw-r--r--   0     1001      127     1447 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/stop_words/no.json
+-rw-r--r--   0     1001      127     2055 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/stop_words/pt.json
+-rw-r--r--   0     1001      127     3327 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/stop_words/ro.json
+-rw-r--r--   0     1001      127     3856 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/stop_words/ru.json
+-rw-r--r--   0     1001      127    23032 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/stop_words/sl.json
+-rw-r--r--   0     1001      127      993 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/stop_words/sv.json
+-rw-r--r--   0     1001      127     5424 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/stop_words/tg.json
+-rw-r--r--   0     1001      127      491 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/stop_words/tr.json
+-rw-r--r--   0        0        0      629 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/Cargo.toml
+-rw-r--r--   0     1001      127     7796 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/src/fuzzy_query.rs
+-rw-r--r--   0     1001      127     1024 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/src/lib.rs
+-rw-r--r--   0     1001      127     2780 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/src/query_io.rs
+-rw-r--r--   0     1001      127    42885 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/src/reader.rs
+-rw-r--r--   0     1001      127     4407 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/src/schema.rs
+-rw-r--r--   0     1001      127    21349 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/src/search_query.rs
+-rw-r--r--   0     1001      127    11723 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/src/search_response.rs
+-rw-r--r--   0     1001      127     2846 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/src/set_query.rs
+-rw-r--r--   0     1001      127     4090 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/src/stop_words.rs
+-rw-r--r--   0     1001      127    17057 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/src/writer.rs
+-rw-r--r--   0     1001      127       88 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/stop_words/README.md
+-rw-r--r--   0     1001      127    19791 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/stop_words/ar.json
+-rw-r--r--   0     1001      127     1923 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/stop_words/az.json
+-rw-r--r--   0     1001      127    11684 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/stop_words/bn.json
+-rw-r--r--   0     1001      127     2513 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/stop_words/ca.json
+-rw-r--r--   0     1001      127    12802 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/stop_words/ch.json
+-rw-r--r--   0     1001      127      730 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/stop_words/da.json
+-rw-r--r--   0     1001      127     2090 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/stop_words/de.json
+-rw-r--r--   0     1001      127     6284 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/stop_words/el.json
+-rw-r--r--   0     1001      127     1473 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/stop_words/en.json
+-rw-r--r--   0     1001      127     3451 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/stop_words/es.json
+-rw-r--r--   0     1001      127     3182 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/stop_words/eu.json
+-rw-r--r--   0     1001      127     2126 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/stop_words/extract.py
+-rw-r--r--   0     1001      127     2748 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/stop_words/fi.json
+-rw-r--r--   0     1001      127     1388 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/stop_words/fr.json
+-rw-r--r--   0     1001      127     5716 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/stop_words/he.json
+-rw-r--r--   0     1001      127     2108 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/stop_words/hu.json
+-rw-r--r--   0     1001      127     8721 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/stop_words/id.json
+-rw-r--r--   0     1001      127     2535 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/stop_words/it.json
+-rw-r--r--   0     1001      127    11737 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/stop_words/kk.json
+-rw-r--r--   0     1001      127     7730 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/stop_words/ne.json
+-rw-r--r--   0     1001      127      756 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/stop_words/nl.json
+-rw-r--r--   0     1001      127     1447 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/stop_words/no.json
+-rw-r--r--   0     1001      127     2055 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/stop_words/pt.json
+-rw-r--r--   0     1001      127     3327 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/stop_words/ro.json
+-rw-r--r--   0     1001      127     3856 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/stop_words/ru.json
+-rw-r--r--   0     1001      127    23032 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/stop_words/sl.json
+-rw-r--r--   0     1001      127      993 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/stop_words/sv.json
+-rw-r--r--   0     1001      127     5424 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/stop_words/tg.json
+-rw-r--r--   0     1001      127      491 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/stop_words/tr.json
+-rw-r--r--   0        0        0      501 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_protos/Cargo.toml
+-rw-r--r--   0     1001      127     2155 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_protos/build.rs
+-rw-r--r--   0     1001      127    26110 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_protos/src/fdbwriter.rs
+-rw-r--r--   0     1001      127        0 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_protos/src/google.protobuf.rs
+-rw-r--r--   0     1001      127     9795 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_protos/src/knowledgebox.rs
+-rw-r--r--   0     1001      127     1256 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_protos/src/lib.rs
+-rw-r--r--   0     1001      127    77311 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_protos/src/nodereader.rs
+-rw-r--r--   0     1001      127    10240 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_protos/src/noderesources.rs
+-rw-r--r--   0     1001      127    46332 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_protos/src/nodewriter.rs
+-rw-r--r--   0     1001      127    19106 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_protos/src/replication.rs
+-rw-r--r--   0     1001      127    33352 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_protos/src/resources.rs
+-rw-r--r--   0     1001      127     5528 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_protos/src/utils.rs
+-rw-r--r--   0        0        0      943 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1240/Cargo.toml
+-rw-r--r--   0     1001      127     1553 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/CHANGELOG.md
+-rw-r--r--   0     1001      127      895 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/Makefile
+-rw-r--r--   0     1001      127       52 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/README.md
+-rwxr-xr-x   0     1001      127      978 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/cov.sh
+-rw-r--r--   0     1001      127     1309 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/pyproject.toml
+-rw-r--r--   0     1001      127     2195 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/src/collect_garbage.rs
+-rw-r--r--   0     1001      127     1212 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/src/errors.rs
+-rw-r--r--   0     1001      127     2337 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/src/lib.rs
+-rw-r--r--   0     1001      127     9405 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/src/reader.rs
+-rw-r--r--   0     1001      127     2154 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/src/update.rs
+-rw-r--r--   0     1001      127     9338 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/src/writer.rs
+-rw-r--r--   0     1001      127      835 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/tests/__init__.py
+-rw-r--r--   0     1001      127      892 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/tests/conftest.py
+-rw-r--r--   0     1001      127     3903 2024-05-02 14:00:46.000000 nucliadb_node_binding-3.0.3.post1240/tests/integration/test_indexing.py
+-rw-r--r--   0        0        0      401 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.0.3.post1240/PKG-INFO
```

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_relations2/Cargo.toml` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_relations2/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_relations2/src/io_maps.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_relations2/src/io_maps.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_relations2/src/lib.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_relations2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_relations2/src/reader.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_relations2/src/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_relations2/src/schema.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_relations2/src/schema.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_relations2/src/writer.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_relations2/src/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_relations2/tests/common/mod.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_relations2/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_relations2/tests/test_reader.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_relations2/tests/test_reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_relations2/tests/test_writer.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_relations2/tests/test_writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_texts2/src/lib.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_texts2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_texts2/src/query_io.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_texts2/src/query_io.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_texts2/src/reader.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_texts2/src/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_texts2/src/schema.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_texts2/src/schema.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_texts2/src/search_query.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_texts2/src/search_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_texts2/src/writer.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_texts2/src/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_texts2/tests/common/mod.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_texts2/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_texts2/tests/test_reader.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_texts2/tests/test_reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_texts2/tests/test_search.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_texts2/tests/test_search.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_texts2/tests/test_streaming.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_texts2/tests/test_streaming.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_texts2/tests/test_writer.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_texts2/tests/test_writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_core/Cargo.toml` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_core/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_core/src/fs_state.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_core/src/fs_state.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_core/src/lib.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_core/src/merge.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_core/src/merge.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_core/src/metrics/meters/mod.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_core/src/metrics/meters/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_core/src/metrics/meters/prometheus.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_core/src/metrics/meters/prometheus.rs`

 * *Files 6% similar despite different names*

```diff
@@ -14,36 +14,40 @@
 // MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 // GNU Affero General Public License for more details.
 //
 // You should have received a copy of the GNU Affero General Public License
 // along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 use prometheus_client::encoding;
+use prometheus_client::metrics::histogram::Histogram;
 use prometheus_client::registry::Registry;
 
 use crate::metrics::metric::grpc_ops::{GrpcOpKey, GrpcOpMetric, GrpcOpValue};
 use crate::metrics::metric::request_time::{RequestTimeKey, RequestTimeMetric, RequestTimeValue};
 use crate::metrics::metric::tokio_runtime::TokioRuntimeObserver;
 use crate::metrics::metric::tokio_tasks::TokioTasksObserver;
 use crate::metrics::metric::{grpc_ops, replication, request_time, shard_cache, vectors};
 use crate::metrics::task_monitor::{Monitor, TaskId};
 use crate::tracing::{debug, error};
 use crate::NodeResult;
 
+const TIME_BUCKETS: [f64; 12] = [0.005, 0.01, 0.025, 0.05, 0.1, 0.25, 0.5, 2.5, 5.0, 10.0, 30.0, 60.0];
+
 pub struct PrometheusMeter {
     registry: Registry,
     request_time_metric: RequestTimeMetric,
     grpc_op_metric: GrpcOpMetric,
     tokio_tasks_observer: TokioTasksObserver,
     tokio_runtime_observer: TokioRuntimeObserver,
     replicated_bytes_metric: replication::ReplicatedBytesMetric,
     replication_ops_metric: replication::ReplicationOpsMetric,
     open_shards_metric: shard_cache::OpenShardsMetric,
     evicted_shards_metric: shard_cache::EvictedShardsMetric,
 
+    pub indexing_resource_download_histogram: Histogram,
     pub vectors_metrics: vectors::VectorsMetrics,
 }
 
 impl Default for PrometheusMeter {
     fn default() -> Self {
         Self::new()
     }
@@ -104,21 +108,29 @@
 
         let vectors_metrics = vectors::VectorsMetrics::new(registry.sub_registry_with_prefix("nucliadb_vectors"));
 
         let prefixed_subregistry = registry.sub_registry_with_prefix("nucliadb_node");
         let tokio_tasks_observer = TokioTasksObserver::new(prefixed_subregistry);
         let tokio_runtime_observer = TokioRuntimeObserver::new(prefixed_subregistry);
 
+        let indexing_resource_download_histogram = Histogram::new(TIME_BUCKETS.iter().copied());
+        prefixed_subregistry.register(
+            "indexing_resource_download_seconds",
+            "Time to download indexing resources from object storage",
+            indexing_resource_download_histogram.clone(),
+        );
+
         Self {
             registry,
             request_time_metric,
             grpc_op_metric,
             tokio_tasks_observer,
             tokio_runtime_observer,
             replicated_bytes_metric,
             replication_ops_metric,
             open_shards_metric,
             evicted_shards_metric,
             vectors_metrics,
+            indexing_resource_download_histogram,
         }
     }
 }
```

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_core/src/metrics/metric/grpc_ops.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_core/src/metrics/metric/grpc_ops.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_core/src/metrics/metric/mod.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_core/src/metrics/metric/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_core/src/metrics/metric/replication.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_core/src/metrics/metric/replication.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_core/src/metrics/metric/request_time.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_core/src/metrics/metric/request_time.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_core/src/metrics/metric/shard_cache.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_core/src/metrics/metric/shard_cache.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_core/src/metrics/metric/tokio_runtime.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_core/src/metrics/metric/tokio_runtime.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_core/src/metrics/metric/tokio_tasks.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_core/src/metrics/metric/tokio_tasks.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_core/src/metrics/metric/vectors.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_core/src/metrics/metric/vectors.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_core/src/metrics/mod.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_core/src/metrics/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_core/src/metrics/task_monitor.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_core/src/metrics/task_monitor.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_core/src/metrics/tests.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_core/src/metrics/tests.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_core/src/paragraphs.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_core/src/paragraphs.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_core/src/query_language/mod.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_core/src/query_language/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_core/src/query_planner.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_core/src/query_planner.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_core/src/relations.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_core/src/relations.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_core/src/tantivy_replica.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_core/src/tantivy_replica.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_core/src/texts.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_core/src/texts.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_core/src/vectors.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_core/src/vectors.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/Cargo.toml` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/src/fuzzy_query.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/src/fuzzy_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/src/lib.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/src/query_io.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/src/query_io.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/src/reader.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/src/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/src/schema.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/src/schema.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/src/search_query.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/src/search_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/src/search_response.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/src/search_response.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/src/set_query.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/src/set_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/src/stop_words.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/src/stop_words.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/src/writer.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/src/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/stop_words/ar.json` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/stop_words/ar.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/stop_words/az.json` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/stop_words/az.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/stop_words/bn.json` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/stop_words/bn.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/stop_words/ca.json` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/stop_words/ca.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/stop_words/ch.json` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/stop_words/ch.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/stop_words/da.json` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/stop_words/da.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/stop_words/de.json` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/stop_words/de.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/stop_words/el.json` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/stop_words/el.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/stop_words/en.json` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/stop_words/en.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/stop_words/es.json` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/stop_words/es.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/stop_words/eu.json` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/stop_words/eu.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/stop_words/extract.py` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/stop_words/extract.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/stop_words/fi.json` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/stop_words/fi.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/stop_words/fr.json` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/stop_words/fr.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/stop_words/he.json` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/stop_words/he.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/stop_words/hu.json` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/stop_words/hu.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/stop_words/id.json` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/stop_words/id.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/stop_words/it.json` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/stop_words/it.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/stop_words/kk.json` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/stop_words/kk.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/stop_words/ne.json` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/stop_words/ne.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/stop_words/nl.json` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/stop_words/nl.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/stop_words/no.json` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/stop_words/no.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/stop_words/pt.json` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/stop_words/pt.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/stop_words/ro.json` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/stop_words/ro.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/stop_words/ru.json` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/stop_words/ru.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/stop_words/sl.json` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/stop_words/sl.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/stop_words/sv.json` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/stop_words/sv.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs3/stop_words/tg.json` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/stop_words/tg.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_vectors/Cargo.toml` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_vectors/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_vectors/docs/labels.drawio.svg` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_vectors/docs/labels.drawio.svg`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_vectors/src/data_point/disk_hnsw.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_vectors/src/data_point/disk_hnsw.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_vectors/src/data_point/mod.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_vectors/src/data_point/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_vectors/src/data_point/node.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_vectors/src/data_point/node.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_vectors/src/data_point/ops_hnsw.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_vectors/src/data_point/ops_hnsw.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_vectors/src/data_point/params.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_vectors/src/data_point/params.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_vectors/src/data_point/ram_hnsw.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_vectors/src/data_point/ram_hnsw.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_vectors/src/data_point/tests.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_vectors/src/data_point/tests.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_vectors/src/data_point_provider/garbage_collector.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_vectors/src/data_point_provider/garbage_collector.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_vectors/src/data_point_provider/mod.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_vectors/src/data_point_provider/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_vectors/src/data_point_provider/reader.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_vectors/src/data_point_provider/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_vectors/src/data_point_provider/replication.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_vectors/src/data_point_provider/replication.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_vectors/src/data_point_provider/state.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_vectors/src/data_point_provider/state.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_vectors/src/data_point_provider/writer.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_vectors/src/data_point_provider/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_vectors/src/data_types/data_store.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_vectors/src/data_types/data_store.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_vectors/src/data_types/dtrie_ram.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_vectors/src/data_types/dtrie_ram.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_vectors/src/data_types/mod.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_vectors/src/data_types/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_vectors/src/data_types/trie.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_vectors/src/data_types/trie.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_vectors/src/data_types/trie_ram.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_vectors/src/data_types/trie_ram.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_vectors/src/data_types/vector.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_vectors/src/data_types/vector.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_vectors/src/formula/mod.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_vectors/src/formula/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_vectors/src/lib.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_vectors/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_vectors/src/service/mod.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_vectors/src/service/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_vectors/src/service/query_io.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_vectors/src/service/query_io.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_vectors/src/service/reader.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_vectors/src/service/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_vectors/src/service/writer.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_vectors/src/service/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_vectors/src/utils.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_vectors/src/utils.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_vectors/tests/test_merge.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_vectors/tests/test_merge.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/Cargo.toml` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/Cargo.toml`

 * *Files 3% similar despite different names*

```diff
@@ -51,14 +51,17 @@
 tower = "0.4.13"
 thiserror = "1"
 opentelemetry = { version = "0.17", features = ["rt-tokio", "trace"] }
 tracing-opentelemetry = "0.17.2"
 reqwest = { version = "0.11.16", features = ["json", "rustls-tls", "blocking"] }
 num_cpus = "1.16.0"
 crossbeam-utils = "0.8.16"
+object_store = { version = "0.10.0", features = ["gcp", "aws"]}
+base64 = "^0.21"
+
 
 # Text Service
 async-stream = "0.3.2"
 
 rand = "0.8.4"
 
 # nucliadb dependencies
```

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/.rustc_info.json` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/.rustc_info.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/Makefile` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/Makefile`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/README.md` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/README.md`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/nucliadb_node/__init__.py` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/nucliadb_node/__init__.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/nucliadb_node/app.py` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/nucliadb_node/app.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/nucliadb_node/indexer.py` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/nucliadb_node/indexer.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 import asyncio
+import contextlib
 import logging
 import time
 from functools import cached_property, partial, total_ordering
 from typing import Optional
 
 from grpc import StatusCode
 from grpc.aio import AioRpcError
@@ -34,20 +35,21 @@
     TypeMessage,
 )
 
 from nucliadb_node import SERVICE_NAME, logger, signals
 from nucliadb_node.settings import settings
 from nucliadb_node.signals import SuccessfulIndexingPayload
 from nucliadb_node.writer import Writer
-from nucliadb_telemetry import errors, metrics
+from nucliadb_telemetry import metrics
 from nucliadb_telemetry.errors import capture_exception
+from nucliadb_utils import const
 from nucliadb_utils.nats import MessageProgressUpdater
 from nucliadb_utils.settings import nats_consumer_settings
 from nucliadb_utils.storages.storage import Storage
-from nucliadb_utils.utilities import get_storage
+from nucliadb_utils.utilities import get_storage, has_feature
 
 CONCURRENT_INDEXERS_COUNT = metrics.Gauge(
     "nucliadb_concurrent_indexers_count", labels={"node": ""}
 )
 indexer_observer = metrics.Observer(
     "nucliadb_message_indexing",
     buckets=[
@@ -69,14 +71,22 @@
 )
 
 
 class IndexNodeError(Exception):
     pass
 
 
+class MetadataNotFoundError(IndexNodeError):
+    pass
+
+
+class ShardNotFound(IndexNodeError):
+    pass
+
+
 @total_ordering
 class WorkUnit:
     # Messages coming from processor take longer to index, so we want to
     # prioritize small messages coming from the writer (user
     # creations/updates/deletes).
     #
     # Priority order: lower values first
@@ -375,121 +385,158 @@
             extra={
                 **_extra,
                 "indexing_time": time.time() - start,
             },
         )
 
     async def _index_message(self, pb: IndexMessage):
-        status = None
         if pb.typemessage == TypeMessage.CREATION:
-            status = await self._set_resource(pb)
+            if has_feature(
+                const.Features.NODE_SET_RESOURCE_FROM_STORAGE, context={"kbid": pb.kbid}
+            ):
+                await self._set_resource_from_storage(pb)
+            else:
+                await self._set_resource(pb)
         elif pb.typemessage == TypeMessage.DELETION:
-            status = await self._delete_resource(pb)
-        if status is not None and status.status != OpStatus.Status.OK:
-            self._handle_index_message_error(pb, status)
+            await self._delete_resource(pb)
+        else:  # pragma: no cover
+            logger.error(
+                "Unknown message type",
+                extra={
+                    "storage_key": pb.storage_key,
+                    "type": str(pb.typemessage),
+                },
+            )
 
-    def _handle_index_message_error(self, pb: IndexMessage, status: OpStatus):
+    def _parse_op_status_errors(self, pb: IndexMessage, status: OpStatus):
+        if status.status == OpStatus.Status.OK:
+            return
         if (
             status.status == OpStatus.Status.ERROR
             and "Shard not found" in status.detail
         ):
             logger.warning(
                 f"Shard does not exist {pb.shard}. This message will be ignored",
                 extra={
                     "kbid": pb.kbid,
                     "shard": pb.shard,
                     "rid": pb.resource,
                     "storage_key": pb.storage_key,
                 },
             )
-            return
+            raise ShardNotFound()
         if (
             status.status == OpStatus.Status.ERROR
             and "Missing resource metadata" in status.detail
         ):
+            raise MetadataNotFoundError()
+        raise IndexNodeError(status.detail)
+
+    @contextlib.contextmanager
+    def _handled_grpc_errors(self):
+        try:
+            yield
+        except AioRpcError as grpc_error:
+            if grpc_error.code() == StatusCode.NOT_FOUND:
+                raise ShardNotFound()
+            else:
+                raise grpc_error
+
+    async def _set_resource(self, pb: IndexMessage) -> None:
+        brain = await self.storage.get_indexing(pb)
+        shard_id = pb.shard
+        rid = brain.resource.uuid
+        brain.shard_id = brain.resource.shard_id = shard_id
+        _extra = {
+            "kbid": pb.kbid,
+            "shard": pb.shard,
+            "rid": rid,
+            "storage_key": pb.storage_key,
+        }
+
+        logger.debug(f"Adding {rid} at {shard_id} otx:{pb.txid}", extra=_extra)
+        try:
+            with self._handled_grpc_errors():
+                status = await self.writer.set_resource(brain)
+                self._parse_op_status_errors(pb, status)
+                logger.debug(
+                    f"...done (Added {rid} at {shard_id} otx:{pb.txid})", extra=_extra
+                )
+                return
+        except ShardNotFound:
+            logger.error(
+                "Shard does not exist. This message will be ignored", extra=_extra
+            )
+            return
+        except MetadataNotFoundError:
             logger.error(
                 "Error on indexer worker trying to set a resource without metadata. "
                 "This message will be ignored",
                 extra={
                     "kbid": pb.kbid,
                     "shard": pb.shard,
                     "rid": pb.resource,
                     "storage_key": pb.storage_key,
                 },
             )
             return
-        raise IndexNodeError(status.detail)
 
-    async def _set_resource(self, pb: IndexMessage) -> Optional[OpStatus]:
-        brain = await self.storage.get_indexing(pb)
-        shard_id = pb.shard
-        rid = brain.resource.uuid
-        brain.shard_id = brain.resource.shard_id = shard_id
+    async def _set_resource_from_storage(self, pb: IndexMessage) -> None:
+        """
+        Set a resource using the new v2 method that doesn't
+        require the indexer to fetch the resource from storage.
+        """
         _extra = {
             "kbid": pb.kbid,
             "shard": pb.shard,
-            "rid": rid,
+            "otx": pb.txid,
             "storage_key": pb.storage_key,
         }
-
-        logger.debug(f"Adding {rid} at {shard_id} otx:{pb.txid}", extra=_extra)
         try:
-            status = await self.writer.set_resource(brain)
-
-        except AioRpcError as grpc_error:
-            if grpc_error.code() == StatusCode.NOT_FOUND:
-                logger.error(
-                    f"Shard does not exist {pb.shard}. This message will be ignored",
-                    extra=_extra,
-                )
-            else:
-                # REVIEW: we should always have metadata and the writer node
-                # should handle this in a better way than a panic
-                if brain.HasField("metadata"):
-                    # Hard fail if we have the correct data
-                    raise grpc_error
-                else:
-                    event_id = errors.capture_exception(grpc_error)
-                    logger.error(
-                        "Error on indexer worker trying to set a resource without metadata. "
-                        "This message won't be retried. Check sentry for more details. "
-                        f"Event id: {event_id}",
-                        extra=_extra,
-                    )
-            return None
-
-        else:
-            logger.debug(
-                f"...done (Added {rid} at {shard_id} otx:{pb.txid})", extra=_extra
+            with self._handled_grpc_errors():
+                status = await self.writer.set_resource_from_storage(pb)
+                self._parse_op_status_errors(pb, status)
+                return
+        except ShardNotFound:
+            logger.error(
+                "Shard does not exist. This message will be ignored", extra=_extra
+            )
+            return
+        except MetadataNotFoundError:
+            logger.error(
+                "Error on indexer worker trying to set a resource without metadata. "
+                "This message will be ignored",
+                extra={
+                    "kbid": pb.kbid,
+                    "shard": pb.shard,
+                    "rid": pb.resource,
+                    "storage_key": pb.storage_key,
+                },
             )
-            return status
+            return
 
-    async def _delete_resource(self, pb: IndexMessage) -> Optional[OpStatus]:
+    async def _delete_resource(self, pb: IndexMessage) -> None:
         shard_id = pb.shard
         rid = pb.resource
         resource = ResourceID(uuid=rid, shard_id=shard_id)
         _extra = {
             "kbid": pb.kbid,
             "shard": pb.shard,
             "rid": rid,
             "storage_key": pb.storage_key,
         }
 
         logger.debug(f"Deleting {rid} in {shard_id} otx:{pb.txid}", extra=_extra)
         try:
-            status = await self.writer.delete_resource(resource)
-
-        except AioRpcError as grpc_error:
-            if grpc_error.code() == StatusCode.NOT_FOUND:
-                logger.error(
-                    f"Shard does not exist {pb.shard}. This message will be ignored",
-                    extra=_extra,
+            with self._handled_grpc_errors():
+                status = await self.writer.delete_resource(resource)
+                self._parse_op_status_errors(pb, status)
+                logger.debug(
+                    f"...done (Deleted {rid} in {shard_id} otx:{pb.txid})", extra=_extra
                 )
-            else:
-                raise grpc_error
-            return None
-
-        else:
-            logger.debug(
-                f"...done (Deleted {rid} in {shard_id} otx:{pb.txid})", extra=_extra
+                return
+        except ShardNotFound:
+            logger.error(
+                f"Shard does not exist {pb.shard}. This message will be ignored",
+                extra=_extra,
             )
-            return status
+            return
```

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/nucliadb_node/listeners/__init__.py` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/nucliadb_node/listeners/__init__.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/nucliadb_node/listeners/indexed_publisher.py` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/nucliadb_node/listeners/indexed_publisher.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/nucliadb_node/pull.py` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/nucliadb_node/pull.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/nucliadb_node/service.py` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/nucliadb_node/service.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/nucliadb_node/settings.py` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/nucliadb_node/settings.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/nucliadb_node/signals.py` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/nucliadb_node/signals.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/nucliadb_node/tests/__init__.py` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/nucliadb_node/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/nucliadb_node/tests/conftest.py` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/nucliadb_node/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/nucliadb_node/tests/fixtures.py` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/nucliadb_node/tests/fixtures.py`

 * *Files 6% similar despite different names*

```diff
@@ -112,22 +112,35 @@
             return False
 
 
 class nucliadbNodeWriter(BaseImage):
     name = "nucliadb_node_writer"
     port = 4446
 
-    def run(self, volume):
+    def run(
+        self,
+        volume,
+        file_backend: str = "unset",
+        file_backend_config: Optional[dict[str, str]] = None,
+    ):
         self._volume = volume
         self._mount = "/data"
+        self._file_backend = file_backend
+        self._file_backend_config = file_backend_config or {}
         return super(nucliadbNodeWriter, self).run()
 
     def get_image_options(self):
         options = super(nucliadbNodeWriter, self).get_image_options()
         options["volumes"] = {self._volume.name: {"bind": "/data"}}
+
+        # Set the file backend and its configuration via environment variables
+        options["environment"]["FILE_BACKEND"] = self._file_backend
+        for key, value in self._file_backend_config.items():
+            options["environment"][key] = value
+
         return options
 
     def check(self):
         channel = insecure_channel(f"{self.host}:{self.get_port()}")
         stub = health_pb2_grpc.HealthStub(channel)
         pb = HealthCheckRequest(service="nodewriter.NodeWriter")
         try:
@@ -141,15 +154,14 @@
 nucliadb_node_writer = nucliadbNodeWriter()
 
 
 @pytest.fixture(scope="session")
 def node_single():
     docker_client = docker.from_env(version=BaseImage.docker_version)
     volume_node = docker_client.volumes.create(driver="local")
-
     writer1_host, writer1_port = nucliadb_node_writer.run(volume_node)
     reader1_host, reader1_port = nucliadb_node_reader.run(volume_node)
 
     settings.writer_listen_address = f"{writer1_host}:{writer1_port}"
     settings.reader_listen_address = f"{reader1_host}:{reader1_port}"
 
     yield
@@ -168,15 +180,15 @@
         nucliadb_node_writer.container_obj.id,
     ]
 
     nucliadb_node_reader.stop()
     nucliadb_node_writer.stop()
 
     for container_id in container_ids:
-        for i in range(5):
+        for _ in range(5):
             try:
                 docker_client.containers.get(container_id)
             except docker.errors.NotFound:
                 break
             time.sleep(2)  # pragma: no cover
 
     volume_node.remove()
```

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/nucliadb_node/tests/integration/test_indexing.py` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/nucliadb_node/tests/integration/test_indexing.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,15 +191,15 @@
 
         async def run_or_fail(func, fail_ratio: float, *args, **kwargs):
             nonlocal work_done_count
             work_done_count += 1
             if work_done_count % round(1 / fail_ratio) == 0:
                 raise Exception("Intended exception to test failure recovery")
             else:
-                await func(*args, **kwargs)
+                return await func(*args, **kwargs)
 
         original_set_resource = worker.writer.set_resource
         worker.writer.set_resource = partial(
             run_or_fail, original_set_resource, fail_ratio
         )
         original_delete_resource = worker.writer.delete_resource
         worker.writer.delete_resource = partial(
```

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_app.py` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_app.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexed_publisher.py` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexed_publisher.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexer.py` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexer.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,14 +100,19 @@
         assert (await queue.get()) == writer_work_unit_1
         assert (await queue.get()) == writer_work_unit_2
         assert (await queue.get()) == processor_work_unit
 
 
 class TestConcurrentShardIndexer:
     @pytest.fixture(autouse=True)
+    def from_storage_flag_enabled(self):
+        with patch("nucliadb_node.indexer.has_feature", return_value=True):
+            yield
+
+    @pytest.fixture(autouse=True)
     def storage(self):
         with patch("nucliadb_node.indexer.get_storage"):
             yield
 
     @pytest.fixture(autouse=True)
     def message_progress_updater(self):
         mpu = Mock(return_value=AsyncMock())
@@ -116,15 +121,15 @@
 
     @pytest.fixture
     def writer(self):
         writer = AsyncMock()
         status = OpStatus()
         status.status = OpStatus.Status.OK
         status.detail = "Successful"
-        writer.set_resource = AsyncMock(return_value=status)
+        writer.set_resource_from_storage = AsyncMock(return_value=status)
         writer.delete_resource = AsyncMock(return_value=status)
         yield writer
 
     @pytest.fixture
     @pytest.mark.asyncio
     async def csi(self, writer) -> AsyncIterator[ConcurrentShardIndexer]:
         csi = ConcurrentShardIndexer(writer=writer, node_id="node-id")
@@ -221,20 +226,25 @@
             yield mock
 
     @pytest.fixture(autouse=True)
     def storage(self):
         with patch("nucliadb_node.indexer.get_storage") as mock:
             yield mock
 
+    @pytest.fixture(autouse=True)
+    def from_storage_flag_enabled(self):
+        with patch("nucliadb_node.indexer.has_feature", return_value=True):
+            yield
+
     @pytest.fixture
     def writer(self):
         writer = Mock()
         status = OpStatus()
         status.status = OpStatus.Status.OK
-        writer.set_resource = AsyncMock(return_value=status)
+        writer.set_resource_from_storage = AsyncMock(return_value=status)
         writer.delete_resource = AsyncMock(return_value=status)
         yield writer
 
     @pytest.fixture
     @pytest.mark.asyncio
     async def indexer(self, writer: AsyncMock, storage):
         indexer = PriorityIndexer(writer=writer, storage=storage)
@@ -266,38 +276,38 @@
         for i in range(total):
             indexer.index_soon(self.work())
         assert indexer.work_queue.qsize() == total
 
         await indexer.work_until_finish()
 
         assert indexer.work_queue.qsize() == 0
-        assert writer.set_resource.await_count == total
+        assert writer.set_resource_from_storage.await_count == total
         assert successful_indexing.dispatch.await_count == total
 
     @pytest.mark.asyncio
     async def test_do_work_processes_a_work_unit(
         self, indexer: PriorityIndexer, writer: AsyncMock, successful_indexing
     ):
         work = self.work()
         work.seqid = 10
         await indexer._do_work(work)
 
-        assert writer.set_resource.await_count == 1  # type: ignore
+        assert writer.set_resource_from_storage.await_count == 1  # type: ignore
         assert successful_indexing.dispatch.await_count == 1
         assert successful_indexing.dispatch.await_args.args[0].seqid == 10
 
     @pytest.mark.asyncio
     async def test_node_writer_status_errors_are_handled(
         self, indexer: PriorityIndexer, writer: AsyncMock
     ):
         status = OpStatus()
         status.status = OpStatus.Status.ERROR
         status.detail = "node writer error"
 
-        writer.set_resource.return_value = status
+        writer.set_resource_from_storage.return_value = status
         with pytest.raises(IndexNodeError):
             pb = IndexMessage()
             pb.typemessage = TypeMessage.CREATION
             await indexer._index_message(pb)
 
         writer.delete_resource.return_value = status
         with pytest.raises(IndexNodeError):
@@ -309,24 +319,24 @@
     async def test_node_writer_status_shard_not_found_errors_are_handled(
         self, indexer: PriorityIndexer, writer: AsyncMock
     ):
         status = OpStatus()
         status.status = OpStatus.Status.ERROR
         status.detail = 'status: NotFound, message: "Shard not found: Shard'
 
-        writer.set_resource.return_value = status
+        writer.set_resource_from_storage.return_value = status
         pb = IndexMessage()
         pb.typemessage = TypeMessage.CREATION
         await indexer._index_message(pb)
 
     @pytest.mark.asyncio
     async def test_node_writer_aio_rpc_errors_are_handled(
         self, indexer: PriorityIndexer, writer: AsyncMock
     ):
-        writer.set_resource.side_effect = AioRpcError(
+        writer.set_resource_from_storage.side_effect = AioRpcError(
             code=StatusCode.UNKNOWN,
             initial_metadata=None,  # type: ignore
             trailing_metadata=None,  # type: ignore
             details="node writer error",
             debug_error_string="node writer error",
         )
         with pytest.raises(AioRpcError):
```

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_pull.py` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_pull.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/nucliadb_node/writer.py` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/nucliadb_node/writer.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from nucliadb_protos.noderesources_pb2 import (
     EmptyQuery,
     Resource,
     ResourceID,
     ShardId,
     ShardIds,
 )
-from nucliadb_protos.nodewriter_pb2 import OpStatus
+from nucliadb_protos.nodewriter_pb2 import IndexMessage, OpStatus
 from nucliadb_protos.nodewriter_pb2_grpc import NodeWriterStub
 
 from nucliadb_node import SERVICE_NAME  # type: ignore
 from nucliadb_utils.grpc import get_traced_grpc_channel
 
 
 class Writer:
@@ -46,14 +46,17 @@
             grpc_writer_address, SERVICE_NAME, max_send_message=250
         )
         self.stub = NodeWriterStub(self.channel)  # type: ignore
 
     async def set_resource(self, pb: Resource) -> OpStatus:
         return await self.stub.SetResource(pb)  # type: ignore
 
+    async def set_resource_from_storage(self, pb: IndexMessage) -> OpStatus:
+        return await self.stub.SetResourceFromStorage(pb)  # type: ignore
+
     async def delete_resource(self, pb: ResourceID) -> OpStatus:
         return await self.stub.RemoveResource(pb)  # type: ignore
 
     async def garbage_collector(self, shard_id: str):
         return await self.stub.GC(ShardId(id=shard_id))  # type: ignore
 
     @backoff.on_exception(
```

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/setup.py` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/setup.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/analytics/blocking.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/analytics/blocking.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/analytics/mod.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/analytics/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/analytics/payload.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/analytics/payload.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/analytics/sender.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/analytics/sender.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/analytics/sink.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/analytics/sink.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/analytics/sync.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/analytics/sync.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/bin/reader.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/bin/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/bin/writer.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/bin/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/cache/mod.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/cache/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/cache/reader_cache.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/cache/reader_cache.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/cache/resource_cache.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/cache/resource_cache.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/cache/writer_cache.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/cache/writer_cache.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/disk_structure.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/disk_structure.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/errors.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/errors.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/grpc/collect_garbage.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/grpc/collect_garbage.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/grpc/grpc_reader.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/grpc/grpc_reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/grpc/grpc_writer.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/grpc/grpc_writer.rs`

 * *Files 5% similar despite different names*

```diff
@@ -25,22 +25,25 @@
 use crate::grpc::collect_garbage::{garbage_collection_loop, GCParameters};
 use crate::merge::{global_merger, MergePriority, MergeRequest, MergeWaiter};
 use crate::settings::Settings;
 use crate::shards::metadata::ShardMetadata;
 use crate::shards::writer::ShardWriter;
 use crate::telemetry::run_with_telemetry;
 use crate::utils::{get_primary_node_id, list_shards, read_host_key};
+use nucliadb_core::metrics::get_metrics;
 use nucliadb_core::protos::node_writer_server::NodeWriter;
+use nucliadb_core::protos::prost::Message;
 use nucliadb_core::protos::{
-    garbage_collector_response, merge_response, op_status, EmptyQuery, GarbageCollectorResponse, MergeResponse,
-    NewShardRequest, NewVectorSetRequest, NodeMetadata, OpStatus, Resource, ResourceId, ShardCreated, ShardId,
-    ShardIds, VectorSetId, VectorSetList,
+    garbage_collector_response, merge_response, op_status, EmptyQuery, GarbageCollectorResponse, IndexMessage,
+    MergeResponse, NewShardRequest, NewVectorSetRequest, NodeMetadata, OpStatus, Resource, ResourceId, ShardCreated,
+    ShardId, ShardIds, VectorSetId, VectorSetList,
 };
 use nucliadb_core::tracing::{self, Span, *};
 use nucliadb_core::Channel;
+use object_store::path::Path;
 use std::sync::Arc;
 use std::time::Duration;
 use tokio::sync::mpsc::UnboundedSender;
 use tokio::task::JoinHandle;
 use tonic::{Request, Response, Status};
 
 const GC_LOOP_INTERVAL: &str = "GC_INTERVAL_SECS";
@@ -180,15 +183,14 @@
             .collect();
 
         Ok(tonic::Response::new(ShardIds {
             ids: shard_ids,
         }))
     }
 
-    // Incremental call that can be call multiple times for the same resource
     async fn set_resource(&self, request: Request<Resource>) -> Result<Response<OpStatus>, Status> {
         let span = Span::current();
         let resource = request.into_inner();
         let shard_id = resource.shard_id.clone();
         let shards = Arc::clone(&self.shards);
         let shard_id_clone = shard_id.clone();
         let info = info_span!(parent: &span, "set resource");
@@ -216,14 +218,41 @@
                     ..Default::default()
                 };
                 Ok(tonic::Response::new(status))
             }
         }
     }
 
+    async fn set_resource_from_storage(&self, request: Request<IndexMessage>) -> Result<Response<OpStatus>, Status> {
+        let download_start = std::time::Instant::now();
+
+        let storage_key = request.into_inner().storage_key;
+
+        let get_result = self.settings.object_store.get(&Path::from(storage_key)).await.map_err(|e| {
+            error!("Failed to get indexing resource from object store: {}", e);
+            tonic::Status::internal(format!("Failed to get indexing resource from object store: {}", e))
+        })?;
+
+        let bytes = get_result.bytes().await.map_err(|e| {
+            error!("Failed to download indexing resource from object store: {}", e);
+            tonic::Status::internal(format!("Failed to download indexing resource from object store: {}", e))
+        })?;
+
+        get_metrics().indexing_resource_download_histogram.observe(download_start.elapsed().as_secs_f64());
+
+        let handle = tokio::task::spawn_blocking(move || Resource::decode(bytes)).await.unwrap();
+        let resource = handle.map_err(|e| {
+            error!("Failed to decode indexing resource: {}", e);
+            tonic::Status::internal(format!("Failed to decode indexing resource: {}", e))
+        })?;
+
+        let set_resource_request = Request::new(resource);
+        self.set_resource(set_resource_request).await
+    }
+
     async fn remove_resource(&self, request: Request<ResourceId>) -> Result<Response<OpStatus>, Status> {
         let span = Span::current();
         let resource = request.into_inner();
         let shard_id = resource.shard_id.clone();
         let shards = Arc::clone(&self.shards);
         let shard_id_clone = shard_id.clone();
         let info = info_span!(parent: &span, "remove resource");
```

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/grpc/middleware/debug.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/grpc/middleware/debug.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/grpc/middleware/metrics.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/grpc/middleware/metrics.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/grpc/middleware/mod.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/grpc/middleware/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/grpc/middleware/telemetry.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/grpc/middleware/telemetry.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/grpc/mod.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/grpc/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/grpc/update.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/grpc/update.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/http_server/metrics_service.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/http_server/metrics_service.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/http_server/mod.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/http_server/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/http_server/traces_service.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/http_server/traces_service.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/lib.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/lifecycle.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/lifecycle.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/merge/global.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/merge/global.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/merge/mod.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/merge/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/merge/scheduler.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/merge/scheduler.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/merge/work.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/merge/work.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/node_metadata.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/node_metadata.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/replication/health.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/replication/health.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/replication/mod.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/replication/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/replication/replicator.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/replication/replicator.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/replication/service.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/replication/service.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/settings.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/settings.rs`

 * *Files 22% similar despite different names*

```diff
@@ -28,29 +28,34 @@
 //! variables.
 //!
 //! The trait `Provider` makes it easy to extend this module with more
 //! providers (to parse from CLI for example).
 
 use anyhow::anyhow;
 use nucliadb_core::tracing::Level;
+use object_store::ObjectStore;
 use serde::de::Unexpected;
 use std::net::SocketAddr;
 use std::num::NonZeroUsize;
 use std::ops::Deref;
 use std::path::PathBuf;
 use std::sync::Arc;
 use std::time::Duration;
 
-use nucliadb_core::NodeResult;
-use serde::{Deserialize, Deserializer};
-use tracing::error;
-
 use crate::disk_structure::{METADATA_FILE, SHARDS_DIR};
 use crate::replication::NodeRole;
 use crate::utils::{parse_log_levels, reliable_lookup_host};
+use base64::engine::general_purpose::STANDARD;
+use base64::Engine;
+use nucliadb_core::NodeResult;
+use object_store::aws::AmazonS3Builder;
+use object_store::gcp::GoogleCloudStorageBuilder;
+use object_store::memory::InMemory;
+use serde::{Deserialize, Deserializer};
+use tracing::error;
 
 fn parse_log_levels_serde<'de, D>(d: D) -> Result<Vec<(String, Level)>, D::Error>
 where
     D: Deserializer<'de>,
 {
     Ok(parse_log_levels(&String::deserialize(d)?))
 }
@@ -82,32 +87,73 @@
 // Allowed sentry environments
 const SENTRY_ENVS: [&str; 2] = ["stage", "prod"];
 const DEFAULT_ENV: &str = "stage";
 
 #[derive(Clone)]
 pub struct Settings {
     env: Arc<EnvSettings>,
+    pub object_store: Arc<dyn ObjectStore>,
 }
 
 impl From<EnvSettings> for Settings {
     fn from(value: EnvSettings) -> Self {
+        let object_store = build_object_store_driver(&value);
         Self {
             env: Arc::new(value),
+            object_store,
         }
     }
 }
 
+pub fn build_object_store_driver(settings: &EnvSettings) -> Arc<dyn ObjectStore> {
+    eprintln!("File backend: {:?}", settings.file_backend);
+    match settings.file_backend {
+        ObjectStoreType::GCS => {
+            let service_account_key = STANDARD.decode(&settings.gcs_base64_creds).unwrap();
+            Arc::new(
+                GoogleCloudStorageBuilder::new()
+                    .with_service_account_key(String::from_utf8(service_account_key).unwrap())
+                    .with_bucket_name(settings.gcs_indexing_bucket.clone())
+                    .build()
+                    .unwrap(),
+            )
+        }
+        ObjectStoreType::S3 => {
+            let mut builder = AmazonS3Builder::new()
+                .with_access_key_id(settings.s3_client_id.clone())
+                .with_secret_access_key(settings.s3_client_secret.clone())
+                .with_region(settings.s3_region_name.clone())
+                .with_bucket_name(settings.s3_indexing_bucket.clone());
+            if settings.s3_endpoint.is_some() {
+                // This is needed for minio compatibility
+                builder = builder.with_endpoint(settings.s3_endpoint.clone().unwrap()).with_allow_http(true);
+            }
+            Arc::new(builder.build().unwrap())
+        }
+        ObjectStoreType::UNSET => Arc::new(InMemory::new()),
+    }
+}
+
 impl Deref for Settings {
     type Target = EnvSettings;
 
     fn deref(&self) -> &Self::Target {
         &self.env
     }
 }
 
+#[derive(Deserialize, Default, Debug)]
+#[serde(rename_all = "lowercase")]
+pub enum ObjectStoreType {
+    #[default]
+    UNSET,
+    GCS,
+    S3,
+}
+
 #[derive(Deserialize)]
 #[serde(default)]
 pub struct EnvSettings {
     // Debug
     #[serde(deserialize_with = "parse_case_insensitive_bool")]
     pub debug: bool,
 
@@ -160,14 +206,25 @@
     // - segments_before_merge: minimum number of alive segments before considering a merge
     pub merge_scheduler_max_nodes_in_merge: usize,
     pub merge_scheduler_segments_before_merge: usize,
     pub merge_on_commit_max_nodes_in_merge: usize,
     pub merge_on_commit_segments_before_merge: usize,
 
     pub max_open_shards: Option<NonZeroUsize>,
+
+    // Object store settings coming from nucliadb_shared chart
+    #[serde(default)]
+    pub file_backend: ObjectStoreType,
+    pub gcs_indexing_bucket: String,
+    pub gcs_base64_creds: String,
+    pub s3_client_id: String,
+    pub s3_client_secret: String,
+    pub s3_region_name: String,
+    pub s3_indexing_bucket: String,
+    pub s3_endpoint: Option<String>,
 }
 
 impl EnvSettings {
     pub fn replication_delay(&self) -> Duration {
         Duration::from_secs(self.replication_delay_seconds)
     }
 
@@ -231,14 +288,22 @@
             num_global_rayon_threads: 10,
             merge_scheduler_free_time_work_scheduling_delay: Duration::from_secs(10),
             merge_scheduler_max_nodes_in_merge: 50_000,
             merge_scheduler_segments_before_merge: 2,
             merge_on_commit_max_nodes_in_merge: 10_000,
             merge_on_commit_segments_before_merge: 100,
             max_open_shards: None,
+            file_backend: ObjectStoreType::UNSET,
+            gcs_indexing_bucket: Default::default(),
+            gcs_base64_creds: Default::default(),
+            s3_client_id: Default::default(),
+            s3_client_secret: Default::default(),
+            s3_region_name: Default::default(),
+            s3_indexing_bucket: Default::default(),
+            s3_endpoint: None,
         }
     }
 }
 
 #[cfg(test)]
 mod tests {
     use std::{num::NonZeroUsize, path::PathBuf, time::Duration};
```

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/shards/errors.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/shards/errors.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/shards/metadata.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/shards/metadata.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/shards/mod.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/shards/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/shards/shard_reader.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/shards/shard_reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/shards/shard_writer.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/shards/shard_writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/shards/versioning.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/shards/versioning.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/telemetry.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/telemetry.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/src/utils.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/src/utils.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/tests/common/mod.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/tests/common/node_services.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/tests/common/node_services.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/tests/common/resources.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/tests/common/resources.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/tests/test_date_range_search.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/tests/test_date_range_search.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/tests/test_download.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/tests/test_download.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/tests/test_merge.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/tests/test_merge.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/tests/test_replication.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/tests/test_replication.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/tests/test_search_relations.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/tests/test_search_relations.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/tests/test_search_sorting.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/tests/test_search_sorting.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/tests/test_security_search.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/tests/test_security_search.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/tests/test_shards.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/tests/test_shards.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/tests/test_suggest.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/tests/test_suggest.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_node/tests/test_vector_normalization.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_node/tests/test_vector_normalization.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/Cargo.toml` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/src/fuzzy_query.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/src/fuzzy_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/src/lib.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/src/query_io.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/src/query_io.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/src/reader.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/src/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/src/schema.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/src/schema.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/src/search_query.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/src/search_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/src/search_response.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/src/search_response.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/src/stop_words.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/src/stop_words.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/src/writer.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs2/src/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/stop_words/ar.json` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/stop_words/ar.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/stop_words/az.json` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/stop_words/az.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/stop_words/bn.json` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/stop_words/bn.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/stop_words/ca.json` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/stop_words/ca.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/stop_words/ch.json` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/stop_words/ch.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/stop_words/da.json` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/stop_words/da.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/stop_words/de.json` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/stop_words/de.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/stop_words/el.json` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/stop_words/el.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/stop_words/en.json` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/stop_words/en.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/stop_words/es.json` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/stop_words/es.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/stop_words/eu.json` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/stop_words/eu.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/stop_words/extract.py` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/stop_words/extract.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/stop_words/fi.json` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/stop_words/fi.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/stop_words/fr.json` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/stop_words/fr.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/stop_words/he.json` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/stop_words/he.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/stop_words/hu.json` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/stop_words/hu.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/stop_words/id.json` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/stop_words/id.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/stop_words/it.json` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/stop_words/it.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/stop_words/kk.json` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/stop_words/kk.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/stop_words/ne.json` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/stop_words/ne.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/stop_words/nl.json` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/stop_words/nl.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/stop_words/no.json` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/stop_words/no.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/stop_words/pt.json` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/stop_words/pt.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/stop_words/ro.json` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/stop_words/ro.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/stop_words/ru.json` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/stop_words/ru.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/stop_words/sl.json` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/stop_words/sl.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/stop_words/sv.json` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/stop_words/sv.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_paragraphs2/stop_words/tg.json` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_paragraphs3/stop_words/tg.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_procs/src/lib.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_procs/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_procs/src/measure.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_procs/src/measure.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.stderr` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.stderr`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_procs/tests/test_measure.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_procs/tests/test_measure.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_protos/build.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_protos/build.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_protos/src/fdbwriter.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_protos/src/fdbwriter.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_protos/src/knowledgebox.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_protos/src/knowledgebox.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_protos/src/lib.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_protos/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_protos/src/nodereader.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_protos/src/nodereader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_protos/src/noderesources.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_protos/src/noderesources.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_protos/src/nodewriter.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_protos/src/nodewriter.rs`

 * *Files 2% similar despite different names*

```diff
@@ -292,14 +292,33 @@
                 })?;
             let codec = tonic::codec::ProstCodec::default();
             let path = http::uri::PathAndQuery::from_static(
                 "/nodewriter.NodeWriter/SetResource",
             );
             self.inner.unary(request.into_request(), path, codec).await
         }
+        pub async fn set_resource_from_storage(
+            &mut self,
+            request: impl tonic::IntoRequest<super::IndexMessage>,
+        ) -> Result<tonic::Response<super::OpStatus>, tonic::Status> {
+            self.inner
+                .ready()
+                .await
+                .map_err(|e| {
+                    tonic::Status::new(
+                        tonic::Code::Unknown,
+                        format!("Service was not ready: {}", e.into()),
+                    )
+                })?;
+            let codec = tonic::codec::ProstCodec::default();
+            let path = http::uri::PathAndQuery::from_static(
+                "/nodewriter.NodeWriter/SetResourceFromStorage",
+            );
+            self.inner.unary(request.into_request(), path, codec).await
+        }
         pub async fn remove_resource(
             &mut self,
             request: impl tonic::IntoRequest<super::super::noderesources::ResourceId>,
         ) -> Result<tonic::Response<super::OpStatus>, tonic::Status> {
             self.inner
                 .ready()
                 .await
@@ -435,14 +454,18 @@
             &self,
             request: tonic::Request<super::super::noderesources::ShardId>,
         ) -> Result<tonic::Response<super::MergeResponse>, tonic::Status>;
         async fn set_resource(
             &self,
             request: tonic::Request<super::super::noderesources::Resource>,
         ) -> Result<tonic::Response<super::OpStatus>, tonic::Status>;
+        async fn set_resource_from_storage(
+            &self,
+            request: tonic::Request<super::IndexMessage>,
+        ) -> Result<tonic::Response<super::OpStatus>, tonic::Status>;
         async fn remove_resource(
             &self,
             request: tonic::Request<super::super::noderesources::ResourceId>,
         ) -> Result<tonic::Response<super::OpStatus>, tonic::Status>;
         async fn add_vector_set(
             &self,
             request: tonic::Request<super::NewVectorSetRequest>,
@@ -742,14 +765,52 @@
                         let codec = tonic::codec::ProstCodec::default();
                         let mut grpc = tonic::server::Grpc::new(codec)
                             .apply_compression_config(
                                 accept_compression_encodings,
                                 send_compression_encodings,
                             );
                         let res = grpc.unary(method, req).await;
+                        Ok(res)
+                    };
+                    Box::pin(fut)
+                }
+                "/nodewriter.NodeWriter/SetResourceFromStorage" => {
+                    #[allow(non_camel_case_types)]
+                    struct SetResourceFromStorageSvc<T: NodeWriter>(pub Arc<T>);
+                    impl<T: NodeWriter> tonic::server::UnaryService<super::IndexMessage>
+                    for SetResourceFromStorageSvc<T> {
+                        type Response = super::OpStatus;
+                        type Future = BoxFuture<
+                            tonic::Response<Self::Response>,
+                            tonic::Status,
+                        >;
+                        fn call(
+                            &mut self,
+                            request: tonic::Request<super::IndexMessage>,
+                        ) -> Self::Future {
+                            let inner = self.0.clone();
+                            let fut = async move {
+                                (*inner).set_resource_from_storage(request).await
+                            };
+                            Box::pin(fut)
+                        }
+                    }
+                    let accept_compression_encodings = self.accept_compression_encodings;
+                    let send_compression_encodings = self.send_compression_encodings;
+                    let inner = self.inner.clone();
+                    let fut = async move {
+                        let inner = inner.0;
+                        let method = SetResourceFromStorageSvc(inner);
+                        let codec = tonic::codec::ProstCodec::default();
+                        let mut grpc = tonic::server::Grpc::new(codec)
+                            .apply_compression_config(
+                                accept_compression_encodings,
+                                send_compression_encodings,
+                            );
+                        let res = grpc.unary(method, req).await;
                         Ok(res)
                     };
                     Box::pin(fut)
                 }
                 "/nodewriter.NodeWriter/RemoveResource" => {
                     #[allow(non_camel_case_types)]
                     struct RemoveResourceSvc<T: NodeWriter>(pub Arc<T>);
```

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_protos/src/replication.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_protos/src/replication.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_protos/src/resources.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_protos/src/resources.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/local_dependencies/nucliadb_protos/src/utils.rs` & `nucliadb_node_binding-3.0.3.post1240/local_dependencies/nucliadb_protos/src/utils.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/Cargo.toml` & `nucliadb_node_binding-3.0.3.post1240/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "nucliadb_node_binding"
-version = "3.0.3-post1233"
+version = "3.0.3-post1240"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "nucliadb_node_binding"
 crate-type = ["cdylib"]
```

### Comparing `nucliadb_node_binding-3.0.3.post1233/CHANGELOG.md` & `nucliadb_node_binding-3.0.3.post1240/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/Makefile` & `nucliadb_node_binding-3.0.3.post1240/Makefile`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/cov.sh` & `nucliadb_node_binding-3.0.3.post1240/cov.sh`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/pyproject.toml` & `nucliadb_node_binding-3.0.3.post1240/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/src/collect_garbage.rs` & `nucliadb_node_binding-3.0.3.post1240/src/collect_garbage.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/src/errors.rs` & `nucliadb_node_binding-3.0.3.post1240/src/errors.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/src/lib.rs` & `nucliadb_node_binding-3.0.3.post1240/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/src/reader.rs` & `nucliadb_node_binding-3.0.3.post1240/src/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/src/update.rs` & `nucliadb_node_binding-3.0.3.post1240/src/update.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/src/writer.rs` & `nucliadb_node_binding-3.0.3.post1240/src/writer.rs`

 * *Files 2% similar despite different names*

```diff
@@ -174,14 +174,18 @@
                     ..Default::default()
                 };
                 Ok(PyList::new(py, status.encode_to_vec()))
             }
         }
     }
 
+    pub fn set_resource_from_storage<'p>(&mut self, _index_message: RawProtos, _py: Python<'p>) -> PyResult<&'p PyAny> {
+        Err(IndexNodeException::new_err("Not implemented"))
+    }
+
     pub fn remove_resource<'p>(&mut self, resource: RawProtos, py: Python<'p>) -> PyResult<&'p PyAny> {
         let resource = ResourceId::decode(&mut Cursor::new(resource)).expect("Error decoding arguments");
         let shard_id = resource.shard_id.clone();
         let shard = self.obtain_shard(shard_id.clone())?;
         let status = shard.remove_resource(&resource).and_then(|()| shard.get_opstatus());
         match status {
             Ok(mut status) => {
```

### Comparing `nucliadb_node_binding-3.0.3.post1233/tests/__init__.py` & `nucliadb_node_binding-3.0.3.post1240/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/tests/conftest.py` & `nucliadb_node_binding-3.0.3.post1240/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.0.3.post1233/tests/integration/test_indexing.py` & `nucliadb_node_binding-3.0.3.post1240/tests/integration/test_indexing.py`

 * *Files identical despite different names*

