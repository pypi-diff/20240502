# Comparing `tmp/vdf_io-0.1.85.tar.gz` & `tmp/vdf_io-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vdf_io-0.1.85.tar", last modified: Tue Feb 20 13:45:50 2024, max compression
+gzip compressed data, was "vdf_io-0.1.9.tar", last modified: Mon Feb 12 11:58:40 2024, max compression
```

## Comparing `vdf_io-0.1.85.tar` & `vdf_io-0.1.9.tar`

### file list

```diff
@@ -1,49 +1,47 @@
-drwxr-xr-x   0 dhruvanand   (501) staff       (20)        0 2024-02-20 13:45:50.563191 vdf_io-0.1.85/
--rw-r--r--   0 dhruvanand   (501) staff       (20)    11357 2024-01-15 10:34:58.000000 vdf_io-0.1.85/LICENSE
--rw-r--r--   0 dhruvanand   (501) staff       (20)      969 2024-02-20 13:45:50.562963 vdf_io-0.1.85/PKG-INFO
--rw-r--r--   0 dhruvanand   (501) staff       (20)    10474 2024-02-16 08:01:05.000000 vdf_io-0.1.85/README.md
--rw-r--r--   0 dhruvanand   (501) staff       (20)       38 2024-02-20 13:45:50.563233 vdf_io-0.1.85/setup.cfg
--rw-r--r--   0 dhruvanand   (501) staff       (20)     1182 2024-02-20 13:45:50.000000 vdf_io-0.1.85/setup.py
-drwxr-xr-x   0 dhruvanand   (501) staff       (20)        0 2024-02-20 13:45:50.551279 vdf_io-0.1.85/src/
-drwxr-xr-x   0 dhruvanand   (501) staff       (20)        0 2024-02-20 13:45:50.554841 vdf_io-0.1.85/src/vdf_io/
--rw-r--r--   0 dhruvanand   (501) staff       (20)       22 2024-02-20 13:45:50.000000 vdf_io-0.1.85/src/vdf_io/__init__.py
--rw-r--r--   0 dhruvanand   (501) staff       (20)       37 2024-02-16 10:46:03.000000 vdf_io-0.1.85/src/vdf_io/constants.py
-drwxr-xr-x   0 dhruvanand   (501) staff       (20)        0 2024-02-20 13:45:50.558076 vdf_io-0.1.85/src/vdf_io/export_vdf/
--rw-r--r--   0 dhruvanand   (501) staff       (20)        0 2024-02-06 19:27:30.000000 vdf_io-0.1.85/src/vdf_io/export_vdf/__init__.py
--rw-r--r--   0 dhruvanand   (501) staff       (20)     4495 2024-02-12 09:27:52.000000 vdf_io-0.1.85/src/vdf_io/export_vdf/kdbai_export.py
--rw-r--r--   0 dhruvanand   (501) staff       (20)     5839 2024-02-12 09:27:52.000000 vdf_io-0.1.85/src/vdf_io/export_vdf/milvus_export.py
--rw-r--r--   0 dhruvanand   (501) staff       (20)    23395 2024-02-16 08:01:05.000000 vdf_io-0.1.85/src/vdf_io/export_vdf/pinecone_export.py
--rw-r--r--   0 dhruvanand   (501) staff       (20)     7003 2024-02-12 09:27:52.000000 vdf_io-0.1.85/src/vdf_io/export_vdf/qdrant_export.py
--rw-r--r--   0 dhruvanand   (501) staff       (20)     2228 2024-02-13 04:59:21.000000 vdf_io-0.1.85/src/vdf_io/export_vdf/vdb_export_cls.py
--rw-r--r--   0 dhruvanand   (501) staff       (20)    11239 2024-02-12 09:27:52.000000 vdf_io-0.1.85/src/vdf_io/export_vdf/vertexai_vector_search_export.py
--rwxr-xr-x   0 dhruvanand   (501) staff       (20)     5157 2024-02-13 07:29:38.000000 vdf_io-0.1.85/src/vdf_io/export_vdf_cli.py
-drwxr-xr-x   0 dhruvanand   (501) staff       (20)        0 2024-02-20 13:45:50.560088 vdf_io-0.1.85/src/vdf_io/import_vdf/
--rw-r--r--   0 dhruvanand   (501) staff       (20)        0 2024-02-06 19:27:30.000000 vdf_io-0.1.85/src/vdf_io/import_vdf/__init__.py
--rw-r--r--   0 dhruvanand   (501) staff       (20)     8661 2024-02-13 04:59:21.000000 vdf_io-0.1.85/src/vdf_io/import_vdf/kdbai_import.py
--rw-r--r--   0 dhruvanand   (501) staff       (20)     8025 2024-02-13 07:16:57.000000 vdf_io-0.1.85/src/vdf_io/import_vdf/milvus_import.py
--rw-r--r--   0 dhruvanand   (501) staff       (20)    11890 2024-02-19 10:46:30.000000 vdf_io-0.1.85/src/vdf_io/import_vdf/pinecone_import.py
--rw-r--r--   0 dhruvanand   (501) staff       (20)    12114 2024-02-20 11:42:37.000000 vdf_io-0.1.85/src/vdf_io/import_vdf/qdrant_import.py
--rw-r--r--   0 dhruvanand   (501) staff       (20)     6997 2024-02-20 12:15:07.000000 vdf_io-0.1.85/src/vdf_io/import_vdf/vdf_import_cls.py
--rw-r--r--   0 dhruvanand   (501) staff       (20)    43207 2024-02-13 07:16:57.000000 vdf_io-0.1.85/src/vdf_io/import_vdf/vertexai_vector_search_import.py
--rwxr-xr-x   0 dhruvanand   (501) staff       (20)     5875 2024-02-20 12:13:35.000000 vdf_io-0.1.85/src/vdf_io/import_vdf_cli.py
--rw-r--r--   0 dhruvanand   (501) staff       (20)      603 2024-02-16 11:29:25.000000 vdf_io-0.1.85/src/vdf_io/meta_types.py
--rw-r--r--   0 dhruvanand   (501) staff       (20)      144 2024-02-06 19:27:30.000000 vdf_io-0.1.85/src/vdf_io/names.py
--rw-r--r--   0 dhruvanand   (501) staff       (20)        0 2024-02-06 19:27:30.000000 vdf_io-0.1.85/src/vdf_io/print_help_rec.py
-drwxr-xr-x   0 dhruvanand   (501) staff       (20)        0 2024-02-20 13:45:50.562298 vdf_io-0.1.85/src/vdf_io/scripts/
--rw-r--r--   0 dhruvanand   (501) staff       (20)        0 2024-02-06 19:27:30.000000 vdf_io-0.1.85/src/vdf_io/scripts/__init__.py
--rwxr-xr-x   0 dhruvanand   (501) staff       (20)     2477 2024-02-12 09:27:52.000000 vdf_io-0.1.85/src/vdf_io/scripts/bump_version.py
--rw-r--r--   0 dhruvanand   (501) staff       (20)      735 2024-02-13 04:59:21.000000 vdf_io-0.1.85/src/vdf_io/scripts/check_for_updates.py
--rwxr-xr-x   0 dhruvanand   (501) staff       (20)     3396 2024-02-07 06:01:34.000000 vdf_io-0.1.85/src/vdf_io/scripts/consolidate_parquet.py
--rwxr-xr-x   0 dhruvanand   (501) staff       (20)     1207 2024-02-07 06:01:34.000000 vdf_io-0.1.85/src/vdf_io/scripts/count_rows.py
--rw-r--r--   0 dhruvanand   (501) staff       (20)      363 2024-02-20 11:49:24.000000 vdf_io-0.1.85/src/vdf_io/scripts/count_rows_hf.py
--rwxr-xr-x   0 dhruvanand   (501) staff       (20)     1654 2024-02-13 07:16:57.000000 vdf_io-0.1.85/src/vdf_io/scripts/get_id_list.py
--rwxr-xr-x   0 dhruvanand   (501) staff       (20)     3193 2024-02-07 06:01:34.000000 vdf_io-0.1.85/src/vdf_io/scripts/push_to_hub_vdf.py
--rwxr-xr-x   0 dhruvanand   (501) staff       (20)     7722 2024-02-13 07:16:57.000000 vdf_io-0.1.85/src/vdf_io/scripts/reembed.py
--rw-r--r--   0 dhruvanand   (501) staff       (20)     8874 2024-02-20 12:04:18.000000 vdf_io-0.1.85/src/vdf_io/util.py
-drwxr-xr-x   0 dhruvanand   (501) staff       (20)        0 2024-02-20 13:45:50.562631 vdf_io-0.1.85/src/vdf_io.egg-info/
--rw-r--r--   0 dhruvanand   (501) staff       (20)      969 2024-02-20 13:45:50.000000 vdf_io-0.1.85/src/vdf_io.egg-info/PKG-INFO
--rw-r--r--   0 dhruvanand   (501) staff       (20)     1321 2024-02-20 13:45:50.000000 vdf_io-0.1.85/src/vdf_io.egg-info/SOURCES.txt
--rw-r--r--   0 dhruvanand   (501) staff       (20)        1 2024-02-20 13:45:50.000000 vdf_io-0.1.85/src/vdf_io.egg-info/dependency_links.txt
--rw-r--r--   0 dhruvanand   (501) staff       (20)      424 2024-02-20 13:45:50.000000 vdf_io-0.1.85/src/vdf_io.egg-info/entry_points.txt
--rw-r--r--   0 dhruvanand   (501) staff       (20)      288 2024-02-20 13:45:50.000000 vdf_io-0.1.85/src/vdf_io.egg-info/requires.txt
--rw-r--r--   0 dhruvanand   (501) staff       (20)        7 2024-02-20 13:45:50.000000 vdf_io-0.1.85/src/vdf_io.egg-info/top_level.txt
+drwxr-xr-x   0 dhruvanand   (501) staff       (20)        0 2024-02-12 11:58:40.543367 vdf_io-0.1.9/
+-rw-r--r--   0 dhruvanand   (501) staff       (20)    11357 2024-01-15 10:34:58.000000 vdf_io-0.1.9/LICENSE
+-rw-r--r--   0 dhruvanand   (501) staff       (20)      395 2024-02-12 11:58:40.543146 vdf_io-0.1.9/PKG-INFO
+-rw-r--r--   0 dhruvanand   (501) staff       (20)    10477 2024-02-12 09:27:52.000000 vdf_io-0.1.9/README.md
+-rw-r--r--   0 dhruvanand   (501) staff       (20)       38 2024-02-12 11:58:40.543477 vdf_io-0.1.9/setup.cfg
+-rw-r--r--   0 dhruvanand   (501) staff       (20)     1180 2024-02-12 11:58:40.000000 vdf_io-0.1.9/setup.py
+drwxr-xr-x   0 dhruvanand   (501) staff       (20)        0 2024-02-12 11:58:40.529003 vdf_io-0.1.9/src/
+drwxr-xr-x   0 dhruvanand   (501) staff       (20)        0 2024-02-12 11:58:40.531458 vdf_io-0.1.9/src/vdf_io/
+-rw-r--r--   0 dhruvanand   (501) staff       (20)       21 2024-02-12 11:58:40.000000 vdf_io-0.1.9/src/vdf_io/__init__.py
+drwxr-xr-x   0 dhruvanand   (501) staff       (20)        0 2024-02-12 11:58:40.534254 vdf_io-0.1.9/src/vdf_io/export_vdf/
+-rw-r--r--   0 dhruvanand   (501) staff       (20)        0 2024-02-06 19:27:30.000000 vdf_io-0.1.9/src/vdf_io/export_vdf/__init__.py
+-rw-r--r--   0 dhruvanand   (501) staff       (20)     4495 2024-02-12 09:27:52.000000 vdf_io-0.1.9/src/vdf_io/export_vdf/kdbai_export.py
+-rw-r--r--   0 dhruvanand   (501) staff       (20)     5839 2024-02-12 09:27:52.000000 vdf_io-0.1.9/src/vdf_io/export_vdf/milvus_export.py
+-rw-r--r--   0 dhruvanand   (501) staff       (20)    23423 2024-02-12 09:27:52.000000 vdf_io-0.1.9/src/vdf_io/export_vdf/pinecone_export.py
+-rw-r--r--   0 dhruvanand   (501) staff       (20)     7003 2024-02-12 09:27:52.000000 vdf_io-0.1.9/src/vdf_io/export_vdf/qdrant_export.py
+-rw-r--r--   0 dhruvanand   (501) staff       (20)     2174 2024-02-12 09:27:52.000000 vdf_io-0.1.9/src/vdf_io/export_vdf/vdb_export_cls.py
+-rw-r--r--   0 dhruvanand   (501) staff       (20)    11239 2024-02-12 09:27:52.000000 vdf_io-0.1.9/src/vdf_io/export_vdf/vertexai_vector_search_export.py
+-rwxr-xr-x   0 dhruvanand   (501) staff       (20)     5018 2024-02-12 09:27:52.000000 vdf_io-0.1.9/src/vdf_io/export_vdf_cli.py
+drwxr-xr-x   0 dhruvanand   (501) staff       (20)        0 2024-02-12 11:58:40.537584 vdf_io-0.1.9/src/vdf_io/import_vdf/
+-rw-r--r--   0 dhruvanand   (501) staff       (20)        0 2024-02-06 19:27:30.000000 vdf_io-0.1.9/src/vdf_io/import_vdf/__init__.py
+-rw-r--r--   0 dhruvanand   (501) staff       (20)     8856 2024-02-12 11:41:14.000000 vdf_io-0.1.9/src/vdf_io/import_vdf/kdbai_import.py
+-rw-r--r--   0 dhruvanand   (501) staff       (20)     7957 2024-02-12 11:49:35.000000 vdf_io-0.1.9/src/vdf_io/import_vdf/milvus_import.py
+-rw-r--r--   0 dhruvanand   (501) staff       (20)    11037 2024-02-12 09:27:52.000000 vdf_io-0.1.9/src/vdf_io/import_vdf/pinecone_import.py
+-rw-r--r--   0 dhruvanand   (501) staff       (20)     9116 2024-02-12 11:42:38.000000 vdf_io-0.1.9/src/vdf_io/import_vdf/qdrant_import.py
+-rw-r--r--   0 dhruvanand   (501) staff       (20)     3176 2024-02-12 11:28:36.000000 vdf_io-0.1.9/src/vdf_io/import_vdf/vdf_import_cls.py
+-rw-r--r--   0 dhruvanand   (501) staff       (20)    43134 2024-02-12 11:46:45.000000 vdf_io-0.1.9/src/vdf_io/import_vdf/vertexai_vector_search_import.py
+-rwxr-xr-x   0 dhruvanand   (501) staff       (20)     5134 2024-02-12 11:03:31.000000 vdf_io-0.1.9/src/vdf_io/import_vdf_cli.py
+-rw-r--r--   0 dhruvanand   (501) staff       (20)      557 2024-02-06 19:27:30.000000 vdf_io-0.1.9/src/vdf_io/meta_types.py
+-rw-r--r--   0 dhruvanand   (501) staff       (20)      144 2024-02-06 19:27:30.000000 vdf_io-0.1.9/src/vdf_io/names.py
+-rw-r--r--   0 dhruvanand   (501) staff       (20)        0 2024-02-06 19:27:30.000000 vdf_io-0.1.9/src/vdf_io/print_help_rec.py
+drwxr-xr-x   0 dhruvanand   (501) staff       (20)        0 2024-02-12 11:58:40.542632 vdf_io-0.1.9/src/vdf_io/scripts/
+-rw-r--r--   0 dhruvanand   (501) staff       (20)        0 2024-02-06 19:27:30.000000 vdf_io-0.1.9/src/vdf_io/scripts/__init__.py
+-rwxr-xr-x   0 dhruvanand   (501) staff       (20)     2477 2024-02-12 09:27:52.000000 vdf_io-0.1.9/src/vdf_io/scripts/bump_version.py
+-rw-r--r--   0 dhruvanand   (501) staff       (20)      735 2024-02-12 11:58:35.000000 vdf_io-0.1.9/src/vdf_io/scripts/check_for_updates.py
+-rwxr-xr-x   0 dhruvanand   (501) staff       (20)     3396 2024-02-07 06:01:34.000000 vdf_io-0.1.9/src/vdf_io/scripts/consolidate_parquet.py
+-rwxr-xr-x   0 dhruvanand   (501) staff       (20)     1207 2024-02-07 06:01:34.000000 vdf_io-0.1.9/src/vdf_io/scripts/count_rows.py
+-rwxr-xr-x   0 dhruvanand   (501) staff       (20)     1576 2024-02-07 06:01:34.000000 vdf_io-0.1.9/src/vdf_io/scripts/get_id_list.py
+-rwxr-xr-x   0 dhruvanand   (501) staff       (20)     3193 2024-02-07 06:01:34.000000 vdf_io-0.1.9/src/vdf_io/scripts/push_to_hub_vdf.py
+-rwxr-xr-x   0 dhruvanand   (501) staff       (20)     7709 2024-02-07 06:01:34.000000 vdf_io-0.1.9/src/vdf_io/scripts/reembed.py
+-rw-r--r--   0 dhruvanand   (501) staff       (20)     7588 2024-02-12 11:32:07.000000 vdf_io-0.1.9/src/vdf_io/util.py
+drwxr-xr-x   0 dhruvanand   (501) staff       (20)        0 2024-02-12 11:58:40.532589 vdf_io-0.1.9/src/vdf_io.egg-info/
+-rw-r--r--   0 dhruvanand   (501) staff       (20)      395 2024-02-12 11:58:40.000000 vdf_io-0.1.9/src/vdf_io.egg-info/PKG-INFO
+-rw-r--r--   0 dhruvanand   (501) staff       (20)     1261 2024-02-12 11:58:40.000000 vdf_io-0.1.9/src/vdf_io.egg-info/SOURCES.txt
+-rw-r--r--   0 dhruvanand   (501) staff       (20)        1 2024-02-12 11:58:40.000000 vdf_io-0.1.9/src/vdf_io.egg-info/dependency_links.txt
+-rw-r--r--   0 dhruvanand   (501) staff       (20)      424 2024-02-12 11:58:40.000000 vdf_io-0.1.9/src/vdf_io.egg-info/entry_points.txt
+-rw-r--r--   0 dhruvanand   (501) staff       (20)      288 2024-02-12 11:58:40.000000 vdf_io-0.1.9/src/vdf_io.egg-info/requires.txt
+-rw-r--r--   0 dhruvanand   (501) staff       (20)        7 2024-02-12 11:58:40.000000 vdf_io-0.1.9/src/vdf_io.egg-info/top_level.txt
```

### Comparing `vdf_io-0.1.85/LICENSE` & `vdf_io-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `vdf_io-0.1.85/README.md` & `vdf_io-0.1.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -30,63 +30,62 @@
 
 <details open>
 
   <summary>Coming Soon</summary>
   
 | Vector Database                | Import | Export |
 |--------------------------------|--------|--------|
-| MongoDB Atlas                  | 🔜     | 🔜     |
-
+| Azure AI Search                | 🔜     | 🔜     |
+| Rockset                        | 🔜     | 🔜     |
+| Vespa                          | 🔜     | 🔜     |
 </details>
 <!-- line break -->
 
 -----
 
 <details>
   <summary>In Progress</summary>
 
 | Vector Database                | Import | Export |
 |--------------------------------|--------|--------|
-| Azure AI Search                | ⏳     | ⏳     |
-| Rockset                        | ⏳     | ⏳     |
-| Vespa                          | ⏳     | ⏳     |
 | Weaviate                       | ⏳     | ⏳     |
+| MongoDB Atlas                  | ⏳     | ⏳     |
 | Epsilla                        | ⏳     | ⏳     |
 | txtai                          | ⏳     | ⏳     |
 | Redis Search                   | ⏳     | ⏳     |
 | OpenSearch                     | ⏳     | ⏳     |
 </details>
 
 -----
 
 <details>
   <summary>Not Supported</summary>
 
 | Vector Database                | Import | Export |
 |--------------------------------|--------|--------|
-| DataStax Astra DB              | ❌     | ❌     |
-| Marqo                          | ❌     | ❌     |
 | Activeloop Deep Lake           | ❌     | ❌     |
+| Anari AI                       | ❌     | ❌     |
 | Apache Cassandra               | ❌     | ❌     |
 | ApertureDB                     | ❌     | ❌     |
 | Chroma                         | ❌     | ❌     |
 | ClickHouse                     | ❌     | ❌     |
 | CrateDB                        | ❌     | ❌     |
+| DataStax Astra DB              | ❌     | ❌     |
 | Elasticsearch                  | ❌     | ❌     |
 | LanceDB                        | ❌     | ❌     |
+| Marqo                          | ❌     | ❌     |
 | Meilisearch                    | ❌     | ❌     |
 | MyScale                        | ❌     | ❌     |
 | Neo4j                          | ❌     | ❌     |
 | Nuclia DB                      | ❌     | ❌     |
 | OramaSearch                    | ❌     | ❌     |
 | pgvector                       | ❌     | ❌     |
 | Turbopuffer                    | ❌     | ❌     |
 | Typesense                      | ❌     | ❌     |
 | USearch                        | ❌     | ❌     |
-| Anari AI                       | ❌     | ❌     |
 | Vald                           | ❌     | ❌     |
 | Apache Solr                    | ❌     | ❌     |
 </details>
 
 ## Installation
 
 ### Using pip
```

### Comparing `vdf_io-0.1.85/setup.py` & `vdf_io-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="vdf_io",
-    version="0.1.85",
+    version="0.1.9",
     description="This library uses a universal format for vector datasets to easily export and import data from all vector databases.",
     long_description="Check out the README for more information: https://github.com/AI-Northstar-Tech/vector-io/blob/main/README.md",
     license="Apache 2.0",
     author="Dhruv Anand",
     author_email="dhruv.anand@ainorthstartech.com",
     packages=find_packages(where="src"),
     package_dir={"": "src"},
@@ -15,12 +15,12 @@
             "export_vdf=vdf_io.export_vdf_cli:main",
             "import_vdf=vdf_io.import_vdf_cli:main",
             "reembed_vdf=vdf_io.scripts.reembed:main",
             "consolidate_parquet_vdf=vdf_io.scripts.consolidate_parquet:main",
             "get_id_list_vdf=vdf_io.scripts.get_id_list:main",
             "push_to_hub_vdf=vdf_io.scripts.push_to_hub_vdf:main",
             "bump_version_vdf=vdf_io.scripts.bump_version:main",
-            "check_for_updates_vdf=vdf_io.scripts.check_for_updates:main",
+            "check_for_updates_vdf=vdf_io.scripts.check_for_updates:main"
         ],
     },
     install_requires=open("requirements.txt").read().splitlines(),
 )
```

### Comparing `vdf_io-0.1.85/src/vdf_io/export_vdf/kdbai_export.py` & `vdf_io-0.1.9/src/vdf_io/export_vdf/kdbai_export.py`

 * *Files identical despite different names*

### Comparing `vdf_io-0.1.85/src/vdf_io/export_vdf/milvus_export.py` & `vdf_io-0.1.9/src/vdf_io/export_vdf/milvus_export.py`

 * *Files identical despite different names*

### Comparing `vdf_io-0.1.85/src/vdf_io/export_vdf/pinecone_export.py` & `vdf_io-0.1.9/src/vdf_io/export_vdf/pinecone_export.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import datetime
 import os
 import json
 import numpy as np
 from tqdm import tqdm
 
 from pinecone import Pinecone, Vector
-from vdf_io.constants import ID_COLUMN
 
 from vdf_io.names import DBNames
 from vdf_io.meta_types import NamespaceMeta, VDFMeta
 from vdf_io.util import set_arg_from_input, set_arg_from_password, standardize_metric
 from vdf_io.export_vdf.vdb_export_cls import ExportVDB
 
 PINECONE_MAX_K = 10_000
@@ -139,15 +138,15 @@
                 top_k=PINECONE_MAX_K,
                 namespace=namespace,
             )
             if len(results["matches"]) == 0:
                 tqdm.write("No vectors found that have not been exported yet.")
                 return []
             # mark the vectors as exported
-            ids = [result[ID_COLUMN] for result in results["matches"]]
+            ids = [result["id"] for result in results["matches"]]
             ids_to_mark = list(set(ids) - all_ids)
             tqdm.write(
                 f"Found {len(ids_to_mark)} vectors that have not been exported yet."
             )
             # fetch the vectors and upsert them with the exported_vectorio flag with MAX_FETCH_SIZE at a time
             mark_pbar = tqdm(total=len(ids_to_mark), desc="Step 1/3: Marking vectors")
             mark_batch_size = MAX_FETCH_SIZE
@@ -200,15 +199,15 @@
         else:
             results = self.index.query(
                 vector=input_vector,
                 include_values=False,
                 top_k=PINECONE_MAX_K,
                 namespace=namespace,
             )
-        ids = set(result[ID_COLUMN] for result in results["matches"])
+        ids = set(result["id"] for result in results["matches"])
         return ids
 
     def get_all_ids_from_index(self, num_dimensions, namespace="", hash_value=""):
         if (
             self.args["id_range_start"] is not None
             and self.args["id_range_end"] is not None
         ):
@@ -233,15 +232,15 @@
         # do small random search and check if ids are int
         random_results = self.index.query(
             vector=np.random.rand(num_dimensions).tolist(),
             include_values=False,
             top_k=100,
             namespace=namespace,
         )
-        random_results_ids_strs = [x[ID_COLUMN] for x in random_results["matches"]]
+        random_results_ids_strs = [x["id"] for x in random_results["matches"]]
         all_ids = set()
         if not all(x.isdigit() for x in random_results_ids_strs):
             tqdm.write(
                 "The ids are not integers. Since a list of ids has not been provided"
                 " using --id_list_file, we will use random search to collect ids."
                 " This may take a while."
             )
@@ -437,14 +436,18 @@
             # check if index exists
             for index_name in index_names:
                 if index_name not in self.get_all_index_names():
                     tqdm.write(f"Index {index_name} does not exist, skipping...")
         index_metas = {}
         for index_name in tqdm(index_names, desc="Fetching indexes"):
             index_meta = self.get_data_for_index(index_name)
+            for index_meta_elem in index_meta:
+                index_meta_elem["metric"] = standardize_metric(
+                    self.pc.describe_index(index_name).metric, self.DB_NAME_SLUG
+                )
             index_metas[index_name] = index_meta
 
         # Create and save internal metadata JSON
         self.file_structure.append(os.path.join(self.vdf_directory, "VDF_META.json"))
         internal_metadata = VDFMeta(
             version=self.args.get("library_version"),
             file_structure=self.file_structure,
@@ -452,15 +455,15 @@
             exported_from=self.DB_NAME_SLUG,
             indexes=index_metas,
             exported_at=datetime.datetime.now().astimezone().isoformat(),
         )
         vdf_meta_text = json.dumps(internal_metadata.dict(), indent=4)
         tqdm.write(vdf_meta_text)
         with open(os.path.join(self.vdf_directory, "VDF_META.json"), "w") as json_file:
-            json_file.write(vdf_meta_text)
+            json.dump(vdf_meta_text, json_file, indent=4)
         return True
 
     def get_data_for_index(self, index_name):
         self.index = self.pc.Index(index_name)
         index_info = self.index.describe_index_stats()
         # Fetch the actual data from the Pinecone index
         index_meta = []
@@ -538,14 +541,11 @@
                 index_name=index_name,
                 total_vector_count=namespace_info["vector_count"],
                 exported_vector_count=total_size,
                 dimensions=index_info["dimension"],
                 model_name=self.args["model_name"],
                 vector_columns=["vector"],
                 data_path="/".join(vectors_directory.split("/")[1:]),
-                metric=standardize_metric(
-                    self.pc.describe_index(index_name).metric, self.DB_NAME_SLUG
-                ),
             )
             index_meta.append(namespace_meta)
             self.args["exported_count"] += total_size
         return index_meta
```

### Comparing `vdf_io-0.1.85/src/vdf_io/export_vdf/qdrant_export.py` & `vdf_io-0.1.9/src/vdf_io/export_vdf/qdrant_export.py`

 * *Files identical despite different names*

### Comparing `vdf_io-0.1.85/src/vdf_io/export_vdf/vdb_export_cls.py` & `vdf_io-0.1.9/src/vdf_io/export_vdf/vdb_export_cls.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations
 import datetime
 import pandas as pd
 import os
 import abc
 
 from vdf_io.util import extract_data_hash
-from vdf_io.constants import ID_COLUMN
 
 
 class ExportVDB(abc.ABC):
     def __init_subclass__(cls, **kwargs):
         super().__init_subclass__(**kwargs)
         if not hasattr(cls, "DB_NAME_SLUG"):
             raise TypeError(
@@ -41,21 +40,21 @@
 
     @classmethod
     @abc.abstractmethod
     def export_vdb(cls, args):
         raise NotImplementedError()
 
     def save_vectors_to_parquet(self, vectors, metadata, vectors_directory):
-        vectors_df = pd.DataFrame(list(vectors.items()), columns=[ID_COLUMN, "vector"])
+        vectors_df = pd.DataFrame(list(vectors.items()), columns=["id", "vector"])
         if metadata:
-            metadata_list = [{**{ID_COLUMN: k}, **v} for k, v in metadata.items()]
+            metadata_list = [{**{"id": k}, **v} for k, v in metadata.items()]
             # Convert the list to a DataFrame
             metadata_df = pd.DataFrame.from_records(metadata_list)
             # Now merge this metadata_df with your main DataFrame
-            df = vectors_df.merge(metadata_df, on=ID_COLUMN, how="left")
+            df = vectors_df.merge(metadata_df, on="id", how="left")
         else:
             df = vectors_df
 
         # Save the DataFrame to a parquet file
         parquet_file = os.path.join(vectors_directory, f"{self.file_ctr}.parquet")
         df.to_parquet(parquet_file)
         self.file_structure.append(parquet_file)
```

### Comparing `vdf_io-0.1.85/src/vdf_io/export_vdf/vertexai_vector_search_export.py` & `vdf_io-0.1.9/src/vdf_io/export_vdf/vertexai_vector_search_export.py`

 * *Files identical despite different names*

### Comparing `vdf_io-0.1.85/src/vdf_io/export_vdf_cli.py` & `vdf_io-0.1.9/src/vdf_io/export_vdf_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 #!/usr/bin/env python3
 
 import argparse
 import os
 import sys
 import time
-import traceback
 from dotenv import load_dotenv
 import warnings
 
 import sentry_sdk
 from opentelemetry import trace
 from opentelemetry.propagate import set_global_textmap
 from opentelemetry.sdk.trace import TracerProvider
@@ -17,15 +16,14 @@
 import vdf_io
 from vdf_io.export_vdf.milvus_export import ExportMilvus
 from vdf_io.export_vdf.pinecone_export import ExportPinecone
 from vdf_io.export_vdf.qdrant_export import ExportQdrant
 from vdf_io.export_vdf.kdbai_export import ExportKDBAI
 from vdf_io.export_vdf.vertexai_vector_search_export import ExportVertexAIVectorSearch
 from vdf_io.names import DBNames
-from vdf_io.scripts.check_for_updates import check_for_updates
 from vdf_io.scripts.push_to_hub_vdf import push_to_hub
 
 # Suppress specific warnings
 warnings.simplefilter("ignore", ResourceWarning)
 
 load_dotenv()
 
@@ -54,15 +52,14 @@
     with tracer.start_as_current_span("export_vdf_cli_main") as span:
         try:
             run_export(span)
             sentry_sdk.flush()
         except Exception as e:
             sentry_sdk.flush()
             print(f"Error: {e}")
-            traceback.print_exc()
             sys.exit(1)
         finally:
             sentry_sdk.flush()
     sentry_sdk.flush()
     return
 
 
@@ -138,16 +135,14 @@
         "Time taken to export data: ",
         time.strftime("%H:%M:%S", time.gmtime(t_end - t_start)),
     )
     span.set_attribute("export_time", t_end - t_start)
     if args["push_to_hub"]:
         push_to_hub(export_obj, args)
 
-    check_for_updates()
-
 
 def make_common_options(parser):
     parser.add_argument(
         "-m",
         "--model_name",
         type=str,
         help="Name of model used",
```

### Comparing `vdf_io-0.1.85/src/vdf_io/import_vdf/kdbai_import.py` & `vdf_io-0.1.9/src/vdf_io/import_vdf/kdbai_import.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+import os
 from typing import Dict, List
 from dotenv import load_dotenv
 from tqdm import tqdm
+import json
 import pyarrow.parquet as pq
 
 import kdbai_client as kdbai
 
 from vdf_io.names import DBNames
 from vdf_io.import_vdf.vdf_import_cls import ImportVDB
 from vdf_io.meta_types import NamespaceMeta
@@ -91,27 +93,27 @@
                 index_name = index_name + (
                     f'_{namespace_meta["namespace"]}'
                     if namespace_meta["namespace"]
                     else ""
                 )
                 parquet_files = self.get_parquet_files(final_data_path)
                 for parquet_file in tqdm(parquet_files, desc="Importing parquet files"):
-                    parquet_file_path = self.get_file_path(
-                        final_data_path, parquet_file
-                    )
+                    parquet_file_path = self.new_method(final_data_path, parquet_file)
                     parquet_table = pq.read_table(parquet_file_path)
                     # rename columns by replacing "-" with "_"
                     parquet_table = parquet_table.rename_columns(
                         [col.replace("-", "_") for col in parquet_table.column_names]
                     )
                     parquet_schema = parquet_table.schema
+                    tqdm.write(str(parquet_schema))
                     parquet_columns = [
                         {"name": field.name, "type": str(field.type)}
                         for field in parquet_schema
                     ]
+                    tqdm.write(str(parquet_columns))
 
                     # Extract information from JSON
                     # namespace = indexes_content[index_names[0]][""][0]["namespace"]
                     (
                         vector_column_names,
                         vector_column_name,
                     ) = self.get_vector_column_name(index_name, namespace_meta)
@@ -202,7 +204,10 @@
                     f"Max rows to be imported {self.args['max_num_rows']} hit. Exiting"
                 )
                 break
 
         # table.insert(df)
         print("Data imported successfully")
         self.args["imported_count"] = total_imported_count
+
+    def new_method(self, final_data_path, parquet_file):
+        return os.path.join(final_data_path, parquet_file)
```

### Comparing `vdf_io-0.1.85/src/vdf_io/import_vdf/milvus_import.py` & `vdf_io-0.1.9/src/vdf_io/import_vdf/milvus_import.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
+import os
 from dotenv import load_dotenv
+import pandas as pd
 from tqdm import tqdm
 import json
 
 from pymilvus import (
     connections,
     utility,
     Collection,
     CollectionSchema,
     FieldSchema,
     DataType,
 )
 
 from vdf_io.names import DBNames
 from vdf_io.util import (
-    read_parquet_progress,
     set_arg_from_input,
     set_arg_from_password,
     standardize_metric_reverse,
 )
 from vdf_io.import_vdf.vdf_import_cls import ImportVDB
 
 
@@ -104,15 +105,15 @@
                             f_vector = f
                         if hasattr(f, "is_primary") and f.is_primary:
                             f_pk = f
                 else:
                     # create collection
                     try:
                         f_pk = FieldSchema(
-                            name=self.id_column,
+                            name="id",
                             dtype=DataType.VARCHAR,
                             max_length=65_535,
                             is_primary=True,
                             auto_id=False,
                         )
                         f_vector = FieldSchema(
                             name=vector_column_name,
@@ -156,35 +157,33 @@
 
                 # Load the data from the parquet files
                 final_data_path = self.get_final_data_path(data_path)
                 parquet_files = self.get_parquet_files(final_data_path)
 
                 num_inserted = 0
                 for file in tqdm(parquet_files, desc="Inserting data"):
-                    file_path = self.get_file_path(final_data_path, file)
-                    df = read_parquet_progress(file_path)
-                    df[self.id_column] = df[self.id_column].apply(lambda x: str(x))
+                    file_path = os.path.join(final_data_path, file)
+                    df = pd.read_parquet(file_path)
+                    df["id"] = df["id"].apply(lambda x: str(x))
                     data_rows = []
-
+                            
                     for _, row in df.iterrows():
                         row = json.loads(row.to_json())
                         # replace old_vector_column_name with vector_column_name
                         if old_vector_column_name != vector_column_name:
                             row[vector_column_name] = row[old_vector_column_name]
                             del row[old_vector_column_name]
                         assert isinstance(row[f_pk.name], str), row[f_pk.name]
                         assert isinstance(row[f_vector.name][0], float), type(
                             row[f_vector.name][0]
                         )
                         data_rows.append(row)
                     BATCH_SIZE = 100
                     if total_imported_count + BATCH_SIZE >= self.args["max_num_rows"]:
-                        data_rows = data_rows[
-                            : self.args["max_num_rows"] - total_imported_count
-                        ]
+                        data_rows = data_rows[:self.args["max_num_rows"]-total_imported_count]
                         max_hit = True
                     for i in tqdm(
                         range(0, len(data_rows), BATCH_SIZE),
                         desc="Upserting in Batches",
                     ):
                         mr = collection.insert(data_rows[i : i + BATCH_SIZE])
                         num_inserted += mr.succ_count
```

### Comparing `vdf_io-0.1.85/src/vdf_io/import_vdf/pinecone_import.py` & `vdf_io-0.1.9/src/vdf_io/import_vdf/pinecone_import.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import os
 from dotenv import load_dotenv
 
 from pinecone import Pinecone, ServerlessSpec, PodSpec, Vector
 
 from vdf_io.names import DBNames
 from vdf_io.util import (
-    read_parquet_progress,
     set_arg_from_input,
     set_arg_from_password,
     standardize_metric_reverse,
 )
 from vdf_io.import_vdf.vdf_import_cls import ImportVDB
 
 load_dotenv()
@@ -103,15 +102,14 @@
         )
 
     def __init__(self, args):
         super().__init__(args)
         self.pc = Pinecone(api_key=self.args["pinecone_api_key"])
 
     def upsert_data(self):
-        max_hit = False
         # Iterate over the indexes and import the data
         for index_name, index_meta in tqdm(
             self.vdf_meta["indexes"].items(), desc="Importing indexes"
         ):
             tqdm.write(f"Importing data for index '{index_name}'")
             # list indexes
             indexes = self.pc.list_indexes().names()
@@ -176,78 +174,63 @@
                 metadata = {}
                 vector_column_names, vector_column_name = self.get_vector_column_name(
                     index_name, namespace_meta
                 )
 
                 for file in tqdm(parquet_files, desc="Loading data from parquet files"):
                     file_path = os.path.join(final_data_path, file)
-                    df = read_parquet_progress(file_path)
+                    df = pd.read_parquet(file_path)
 
                     if self.args["subset"] is True:
                         if (
                             "id_list_file" in self.args
                             and self.args["id_list_file"] is not None
                         ):
                             id_list = pd.read_csv(
                                 self.args["id_list_file"], header=None
                             )[0].tolist()
-                            df = df[df[self.id_column].isin(id_list)]
+                            df = df[df["id"].isin(id_list)]
                         elif (
                             "id_range_start" in self.args
                             and self.args["id_range_start"] is not None
                             and "id_range_end" in self.args
                             and self.args["id_range_end"] is not None
                         ):
                             # convert id to int before comparison
                             df = df[
-                                (
-                                    df[self.id_column].astype(int)
-                                    >= self.args["id_range_start"]
-                                )
-                                & (
-                                    df[self.id_column].astype(int)
-                                    <= self.args["id_range_end"]
-                                )
+                                (df["id"].astype(int) >= self.args["id_range_start"])
+                                & (df["id"].astype(int) <= self.args["id_range_end"])
                             ]
                         else:
                             raise Exception(
                                 "Invalid arguments for subset export. "
                                 "Please provide either id_list_file or id_range_start and id_range_end"
                             )
-                    if len(vectors) > self.args["max_num_rows"]:
-                        max_hit = True
-                        break
-                    if len(vectors) + len(df) > self.args["max_num_rows"]:
-                        df = df.head(self.args["max_num_rows"] - len(vectors))
-                        max_hit = True
                     vectors.update(
                         {
-                            row[self.id_column]: row[vector_column_name].tolist()
+                            row["id"]: row[vector_column_name].tolist()
                             for _, row in df.iterrows()
                         }
                     )
                     metadata.update(
                         {
-                            row[self.id_column]: {
+                            row["id"]: {
                                 key: value
                                 for key, value in row.items()
-                                if key not in [self.id_column] + vector_column_names
+                                if key not in ["id"] + vector_column_names
                             }
                             for _, row in df.iterrows()
                         }
                     )
-                    if max_hit:
-                        break
                 tqdm.write(
                     f"Loaded {len(vectors)} vectors from {len(parquet_files)} parquet files"
                 )
                 # Upsert the vectors and metadata to the Pinecone index in batches
                 total_imported_count = 0
                 start_idx = 0
-                pbar = tqdm(total=len(vectors), desc="Upserting vectors")
                 while start_idx < len(vectors):
                     end_idx = min(start_idx + current_batch_size, len(vectors))
 
                     batch_vectors = [
                         (
                             Vector(
                                 id=str(id),
@@ -265,23 +248,22 @@
                             )
                         )
                         for id, vector in list(vectors.items())[start_idx:end_idx]
                     ]
                     try:
                         resp = index.upsert(vectors=batch_vectors, namespace=namespace)
                         total_imported_count += resp["upserted_count"]
-                        pbar.update(resp["upserted_count"])
                         start_idx += resp["upserted_count"]
                     except Exception as e:
                         tqdm.write(
-                            f"Error upserting vectors for index '{index_name}', {e}"
+                            f"Error upserting vectors for index '{index_name}'", e
                         )
                         if current_batch_size < BATCH_SIZE / 100:
                             tqdm.write("Batch size is not the issue. Aborting import")
                             raise e
-                        current_batch_size = int(2 * current_batch_size / 3)
+                        current_batch_size = int(9 * current_batch_size / 10)
                         tqdm.write(f"Reducing batch size to {current_batch_size}")
                         continue
         tqdm.write(
             f"Data import completed successfully. Imported {total_imported_count} vectors"
         )
         self.args["imported_count"] = total_imported_count
```

### Comparing `vdf_io-0.1.85/src/vdf_io/import_vdf/qdrant_import.py` & `vdf_io-0.1.9/src/vdf_io/import_vdf/qdrant_import.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,21 @@
+import os
 from dotenv import load_dotenv
-import numpy as np
+import pandas as pd
 from tqdm import tqdm
 from grpc import RpcError
 from typing import Any, Dict, List
 
 from qdrant_client import QdrantClient
 from qdrant_client.http.exceptions import UnexpectedResponse
 from qdrant_client.http.models import VectorParams, Distance, PointStruct
-from vdf_io.constants import ID_COLUMN
 
 from vdf_io.names import DBNames
 from vdf_io.util import (
-    expand_shorthand_path,
-    get_qdrant_id_from_id,
-    read_parquet_progress,
+    extract_numerical_hash,
     set_arg_from_input,
     set_arg_from_password,
 )
 from vdf_io.import_vdf.vdf_import_cls import ImportVDB
 from vdf_io.meta_types import NamespaceMeta
 
 load_dotenv()
@@ -43,21 +41,14 @@
             "prefer_grpc",
             "Whether to use GRPC. Recommended. (default: True): ",
             bool,
             True,
         )
         set_arg_from_input(
             args,
-            "qdrant_local_persist_path",
-            "Enter the path to the local persist directory (default: None): ",
-            str,
-            "DO_NOT_PROMPT",
-        )
-        set_arg_from_input(
-            args,
             "parallel",
             "Enter the batch size for upserts (default: 1): ",
             int,
             1,
         )
         set_arg_from_input(
             args,
@@ -81,44 +72,32 @@
         return qdrant_import
 
     @classmethod
     def make_parser(cls, subparsers):
         parser_qdrant = subparsers.add_parser(
             DBNames.QDRANT, help="Import data to Qdrant"
         )
-        parser_qdrant.add_argument(
-            "-u",
-            "--url",
-            type=str,
-            help="Qdrant instance url",
-            default="http://localhost:6334",
-        )
+        parser_qdrant.add_argument("-u", "--url", type=str, help="Qdrant url")
         parser_qdrant.add_argument(
             "--prefer_grpc",
             type=bool,
             help="Whether to use Qdrant's GRPC interface",
             default=True,
         )
         parser_qdrant.add_argument(
-            "--qdrant_local_persist_path",
-            type=str,
-            help="Path to the local persist directory (default: None)",
-            default=None,
-        )
-        parser_qdrant.add_argument(
             "--batch_size",
             type=int,
             help="Batch size for upserts (default: 64).",
             default=64,
         )
         parser_qdrant.add_argument(
             "--parallel",
             type=int,
-            help="Number of parallel processes of upload (default: 5).",
-            default=5,
+            help="Number of parallel processes of upload (default: 1).",
+            default=1,
         )
         parser_qdrant.add_argument(
             "--max_retries",
             type=int,
             help="Maximum number of retries in case of a failure (default: 3).",
             default=3,
         )
@@ -128,29 +107,18 @@
             help="Shard to be queried (default: None)",
             default=None,
         )
 
     def __init__(self, args):
         # call super class constructor
         super().__init__(args)
-        url, api_key, prefer_grpc, path = (
-            self.args.get("url", None),
-            self.args.get("qdrant_api_key", None),
-            self.args.get("prefer_grpc", True),
-            expand_shorthand_path(self.args.get("qdrant_local_persist_path", None)),
-        )
-        if path:
-            url = None
-        if url:
-            path = None
         self.client = QdrantClient(
-            url=url,
-            api_key=api_key,
-            prefer_grpc=prefer_grpc,
-            path=path,
+            url=self.args["url"],
+            api_key=self.args.get("qdrant_api_key", None),
+            prefer_grpc=self.args.get("prefer_grpc", True),
         )
 
     def upsert_data(self):
         max_hit = False
         total_imported_count = 0
         # we know that the self.vdf_meta["indexes"] is a list
         index_meta: Dict[str, List[NamespaceMeta]] = {}
@@ -170,44 +138,27 @@
                     f"_{namespace_meta['namespace']}"
                     if namespace_meta["namespace"]
                     else ""
                 )
                 if new_collection_name not in collections:
                     # create index
                     try:
-                        if namespace_meta["dimensions"] == -1:
-                            tqdm.write(
-                                f"Resolving dimensions for index '{new_collection_name}'"
-                            )
-                            dims = self.resolve_dims(
-                                namespace_meta, new_collection_name
-                            )
-                            if dims != -1:
-                                namespace_meta["dimensions"] = dims
-                                tqdm.write(f"Resolved dimensions: {dims}")
-                            else:
-                                tqdm.write(
-                                    f"Failed to resolve dimensions for index '{new_collection_name}'"
-                                )
-                                return
                         self.client.create_collection(
                             collection_name=new_collection_name,
                             vectors_config=VectorParams(
                                 size=namespace_meta["dimensions"],
                                 distance=(
                                     namespace_meta["metric"]
                                     if "metric" in namespace_meta
                                     else Distance.COSINE
                                 ),
                             ),
                         )
                     except Exception as e:
-                        tqdm.write(
-                            f"Failed to create index '{new_collection_name}' {e}"
-                        )
+                        tqdm.write(f"Failed to create index '{new_collection_name}'", e)
                         return
                 prev_vector_count = self.client.get_collection(
                     collection_name=new_collection_name
                 ).vectors_count
                 if prev_vector_count > 0:
                     tqdm.write(
                         f"Index '{new_collection_name}' has {prev_vector_count} vectors before import"
@@ -216,99 +167,75 @@
                 parquet_files = self.get_parquet_files(final_data_path)
 
                 vectors = {}
                 metadata = {}
                 vector_column_names, vector_column_name = self.get_vector_column_name(
                     new_collection_name, namespace_meta
                 )
-                for file in tqdm(parquet_files, desc="Iterating parquet files"):
-                    file_path = self.get_file_path(final_data_path, file)
-                    df = read_parquet_progress(file_path)
+                for file in parquet_files:
+                    file_path = os.path.join(final_data_path, file)
+                    df = pd.read_parquet(file_path)
                     vectors.update(
-                        {
-                            row[self.id_column]: row[vector_column_name]
-                            for _, row in df.iterrows()
-                        }
+                        {row["id"]: row[vector_column_name] for _, row in df.iterrows()}
                     )
                     metadata.update(
                         {
-                            row[self.id_column]: {
+                            row["id"]: {
                                 key: value
                                 for key, value in row.items()
-                                if key not in [ID_COLUMN] + vector_column_names
+                                if key not in ["id"] + vector_column_names
                             }
                             for _, row in df.iterrows()
                         }
                     )
-                    for k, v in vectors.items():
-                        vectors[k] = self.extract_vector(v)
-                    for k, v in metadata.items():
-                        for key, value in v.items():
-                            if isinstance(value, np.ndarray):
-                                metadata[k][key] = value.tolist()
-                    points = [
-                        PointStruct(
-                            id=get_qdrant_id_from_id(idx),
-                            vector=vectors[idx],
-                            payload=metadata.get(idx, {}),
-                        )
-                        for idx in vectors.keys()
-                    ]
+                vectors = {k: v.tolist() for k, v in vectors.items()}
+                points = [
+                    PointStruct(
+                        id=(
+                            int(idx)
+                            if (isinstance(idx, int) or idx.isdigit())
+                            else extract_numerical_hash(idx)
+                        ),
+                        vector=vectors[idx],
+                        payload=metadata.get(idx, {}),
+                    )
+                    for idx in vectors.keys()
+                ]
 
-                    if total_imported_count + len(points) >= self.args["max_num_rows"]:
-                        max_hit = True
-                        points = points[
-                            : self.args["max_num_rows"] - total_imported_count
-                        ]
-                        tqdm.write("Truncating data to limit to max rows")
-                    try:
-                        tqdm.write(f"Starting bulk upload for file '{file_path}'")
-                        self.client.upload_points(
-                            collection_name=new_collection_name,
-                            points=points,
-                            batch_size=self.args.get("batch_size", 64),
-                            parallel=self.args.get("parallel", 5),
-                            max_retries=self.args.get("max_retries", 3),
-                            shard_key_selector=self.args.get(
-                                "shard_key_selector", None
-                            ),
-                            wait=True,
-                        )
-                        tqdm.write(f"Completed bulk upload for file '{file_path}'")
-                        total_imported_count += len(points)
-                        if total_imported_count >= self.args["max_num_rows"]:
-                            max_hit = True
-                    except (UnexpectedResponse, RpcError, ValueError) as e:
-                        tqdm.write(
-                            f"Failed to upsert data for collection '{new_collection_name}', {e}"
-                        )
-                        continue
-                    vector_count = self.client.get_collection(
-                        collection_name=new_collection_name
-                    ).vectors_count
-                    if max_hit:
-                        break
-                    # END parquet file loop
+                if total_imported_count + len(points) >= self.args["max_num_rows"]:
+                    max_hit = True
+                    points = points[: self.args["max_num_rows"] - total_imported_count]
+
+                try:
+                    self.client.upload_points(
+                        collection_name=new_collection_name,
+                        points=points,
+                        batch_size=self.args.get("batch_size", 64),
+                        parallel=self.args.get("parallel", 1),
+                        max_retries=self.args.get("max_retries", 3),
+                        shard_key_selector=self.args.get("shard_key_selector", None),
+                        wait=True,
+                    )
+                except (UnexpectedResponse, RpcError, ValueError):
+                    tqdm.write(
+                        f"Failed to upsert data for collection '{new_collection_name}'"
+                    )
+                    continue
+                vector_count = self.client.get_collection(
+                    collection_name=new_collection_name
+                ).vectors_count
                 tqdm.write(
                     f"Index '{new_collection_name}' has {vector_count} vectors after import"
                 )
                 tqdm.write(f"{vector_count - prev_vector_count} vectors were imported")
+                total_imported_count += vector_count - prev_vector_count
+                if total_imported_count >= self.args["max_num_rows"]:
+                    max_hit = True
                 if max_hit:
                     break
-                # END namespace loop
             if max_hit:
                 tqdm.write(
                     f"Max rows to be imported {self.args['max_num_rows']} hit. Exiting"
                 )
                 break
-            # END index loop
         tqdm.write("Data import completed successfully.")
         self.args["imported_count"] = total_imported_count
-
-    def extract_vector(self, v):
-        if isinstance(v, list) and len(v) > 1:
-            return v
-        if isinstance(v, np.ndarray):
-            if v.shape[0] > 1:
-                return v.tolist()
-            if v.shape[0] == 1:
-                return v[0].tolist()
```

### Comparing `vdf_io-0.1.85/src/vdf_io/import_vdf/vdf_import_cls.py` & `vdf_io-0.1.9/src/vdf_io/scripts/reembed.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,164 +1,207 @@
-import datetime
-from functools import lru_cache
+#!/usr/bin/env python3
+
+import argparse
 import json
 import os
-import numpy as np
-from packaging.version import Version
-import abc
+import litellm
 from tqdm import tqdm
+import pandas as pd
+from dotenv import load_dotenv
+import sys
+from IPython.core import ultratb
+import warnings
 
-from qdrant_client.http.models import Distance
-
-import vdf_io
-from vdf_io.constants import ID_COLUMN
-from vdf_io.meta_types import NamespaceMeta, VDFMeta
 from vdf_io.util import (
-    expand_shorthand_path,
     get_final_data_path,
     get_parquet_files,
-    read_parquet_progress,
+    set_arg_from_input,
+    set_arg_from_password,
 )
 
 
-class ImportVDB(abc.ABC):
-    def __init_subclass__(cls, **kwargs):
-        super().__init_subclass__(**kwargs)
-        if not hasattr(cls, "DB_NAME_SLUG"):
-            raise TypeError(
-                f"Class {cls.__name__} lacks required class variable 'DB_NAME_SLUG'"
-            )
+warnings.filterwarnings("ignore", module="litellm")
+sys.excepthook = ultratb.FormattedTB(color_scheme="Linux", call_pdb=False)
 
-    def __init__(self, args):
-        self.args = args
-        self.temp_file_paths = []
-        if self.args.get("hf_dataset", None) is None:
-            self.args["dir"] = expand_shorthand_path(self.args["dir"])
-            if not os.path.isdir(self.args["dir"]):
-                raise Exception("Invalid dir path")
-            if not os.path.isfile(os.path.join(self.args["dir"], "VDF_META.json")):
-                raise Exception("Invalid dir path, VDF_META.json not found")
-            # Check if the VDF_META.json file exists
-            vdf_meta_path = os.path.join(self.args["dir"], "VDF_META.json")
-            if not os.path.isfile(vdf_meta_path):
-                raise Exception("VDF_META.json not found in the specified directory")
-            with open(vdf_meta_path) as f:
-                self.vdf_meta = json.load(f)
-        else:
-            hf_dataset = self.args.get("hf_dataset", None)
-            index_name = hf_dataset.split("/")[-1]
-            from huggingface_hub import HfFileSystem
-
-            fs = HfFileSystem()
-            hf_files = fs.ls(f"datasets/{hf_dataset}", detail=False)
-            if f"datasets/{hf_dataset}/VDF_META.json" in hf_files:
-                print(f"Found VDF_META.json in {hf_dataset} on HuggingFace Hub")
-                self.vdf_meta = json.loads(
-                    fs.read_text(f"datasets/{hf_dataset}/VDF_META.json")
-                )
-            else:
-                self.vdf_meta = VDFMeta(
-                    version=vdf_io.__version__,
-                    file_structure=[],
-                    author=hf_dataset.split("/")[0],
-                    exported_from="hf",
-                    indexes={
-                        index_name: [
-                            NamespaceMeta(
-                                namespace="",
-                                index_name=index_name,
-                                total_vector_count=self.args.get("max_num_rows"),
-                                exported_vector_count=self.args.get("max_num_rows"),
-                                dimensions=self.args.get("vector_dim", -1),
-                                model_name=self.args.get("model_name", ""),
-                                vector_columns=self.args.get(
-                                    "vector_columns", "vector"
-                                ).split(","),
-                                data_path=".",
-                                metric=self.args.get("metric", Distance.COSINE),
-                            )
-                        ]
-                    },
-                    exported_at=datetime.datetime.now().astimezone().isoformat(),
-                    id_column=self.args.get("id_column", ID_COLUMN),
-                ).dict()
-            print(json.dumps(self.vdf_meta, indent=4))
-        self.id_column = self.vdf_meta.get("id_column", ID_COLUMN)
-        if "indexes" not in self.vdf_meta:
-            raise Exception("Invalid VDF_META.json, 'indexes' key not found")
-        if "version" not in self.vdf_meta:
-            print("Warning: 'version' key not found in VDF_META.json")
-        elif "library_version" not in self.args:
-            print(
-                "Warning: 'library_version' not found in args. Skipping version check."
-            )
-        elif Version(self.vdf_meta["version"]) > Version(self.args["library_version"]):
-            print(
-                f"Warning: The version of vector-io library: ({self.args['library_version']}) is behind the version of the vdf directory: ({self.vdf_meta['version']})."
-            )
-            print(
-                "Please upgrade the vector-io library to the latest version to ensure compatibility."
-            )
+load_dotenv()
 
-    @abc.abstractmethod
-    def upsert_data():
-        """
-        Get data from vector database
-        """
-        raise NotImplementedError
-
-    def get_vector_column_name(self, index_name, namespace_meta):
-        if "vector_columns" not in namespace_meta:
-            print(
-                "vector_columns not found in namespace metadata. Using 'vector' as the vector column name."
-            )
-            vector_column_name = "vector"
-            vector_column_names = [vector_column_name]
-        else:
-            vector_column_names = namespace_meta["vector_columns"]
-            vector_column_name = vector_column_names[0]
-            if len(vector_column_names) > 1:
-                tqdm.write(
-                    f"Warning: More than one vector column found for index {index_name}."
-                    f" Only the first vector column {vector_column_name} will be imported."
-                )
-        return vector_column_names, vector_column_name
 
-    @lru_cache(maxsize=1)
-    def get_parquet_files(self, data_path):
-        return get_parquet_files(data_path, self.args, self.temp_file_paths)
-
-    def get_final_data_path(self, data_path):
-        return get_final_data_path(
-            self.args["cwd"], self.args["dir"], data_path, self.args
+def main():
+    parser = argparse.ArgumentParser(description="Reembed a vector dataset")
+
+    parser.add_argument(
+        "-d",
+        "--dir",
+        type=str,
+        help="Directory of vector dataset in the VDF format",
+        required=True,
+    )
+
+    parser.add_argument(
+        "-m",
+        "--new_model_name",
+        type=str,
+        help="Name of new model to be used",
+    )
+
+    parser.add_argument(
+        "-t",
+        "--text_column",
+        type=str,
+        help="Name of the column containing text to be embedded",
+        default="text",
+    )
+
+    parser.add_argument(
+        "--dimensions",
+        type=int,
+        help="Dimensions of the new model to be used",
+    )
+
+    args = parser.parse_args()
+    args = vars(args)
+
+    set_arg_from_input(
+        args,
+        "new_model_name",
+        "Enter the name of the new model to be used (default: 'text-embedding-3-small'): ",
+        str,
+        "text-embedding-3-small",
+    )
+
+    if args["new_model_name"].startswith("text-embedding-3"):
+        set_arg_from_input(
+            args,
+            "dimensions",
+            "Enter the dimensions of the new model to be used (default: 1536 for small, 3072 for large): ",
+            int,
         )
 
-    def get_file_path(self, final_data_path, parquet_file):
-        if self.args.get("hf_dataset", None):
-            return parquet_file
-        return os.path.join(final_data_path, parquet_file)
-
-    def resolve_dims(self, namespace_meta, new_collection_name):
-        final_data_path = self.get_final_data_path(namespace_meta["data_path"])
-        parquet_files = self.get_parquet_files(final_data_path)
-        _, vector_column_name = self.get_vector_column_name(
-            new_collection_name, namespace_meta
+    set_arg_from_password(
+        args,
+        "OPENAI_API_KEY",
+        "Enter the OpenAI API key (hit return to skip): ",
+        "OPENAI_API_KEY",
+    )
+
+    set_arg_from_input(
+        args,
+        "text_column",
+        "Enter the name of the column containing text to be embedded (default: 'text'): ",
+        str,
+        "text",
+    )
+
+    set_arg_from_input(
+        args,
+        "dir",
+        "Enter the directory of vector dataset in the VDF format: ",
+        str,
+    )
+
+    reembed_count = 0
+    # open VDF_META.json
+    with open(os.path.join(args["dir"], "VDF_META.json"), "r+") as f:
+        vdf_meta = json.load(f)
+        for _, index_meta in tqdm(
+            vdf_meta["indexes"].items(), desc="Iterating over indexes"
+        ):
+            new_vector_column = (
+                f"vec_{args['text_column']}_{args['new_model_name'].replace('/', '_')}"
+            )
+            overwrite_bool = False
+            for namespace_meta in tqdm(index_meta, desc="Iterating over namespaces"):
+                data_path = namespace_meta["data_path"]
+                final_data_path = get_final_data_path(
+                    os.getcwd(), args["dir"], data_path
+                )
+                parquet_files = get_parquet_files(final_data_path)
+                for file in tqdm(parquet_files, desc="Iterating over parquet files"):
+                    file_path = os.path.join(final_data_path, file)
+                    if (
+                        new_vector_column in namespace_meta["vector_columns"]
+                        and not overwrite_bool
+                    ):
+                        # ask user if they want to overwrite (y/n)
+                        overwrite = input(
+                            f"{new_vector_column} already exists in vector_columns. Overwrite? (y/n): "
+                        )
+                        overwrite_bool = overwrite.lower() == "y"
+                        if not overwrite_bool:
+                            tqdm.write(
+                                f"Skipping {file_path} because {new_vector_column} already exists in vector_columns.\n"
+                                "Aborting reembedding."
+                            )
+                            exit()
+                    if "dimensions" in args and args["dimensions"] is not None:
+                        new_vector_column += f"_{args['dimensions']}"
+                    tqdm.write(f"Reembedding {file_path}")
+                    # read parquet file
+                    df = pd.read_parquet(file_path)
+                    # get text column
+                    text_column = args["text_column"]
+                    if text_column not in df.columns:
+                        raise Exception(
+                            f"Text column {text_column} not found in {file_path}"
+                        )
+                    # get embeddings
+                    BATCH_SIZE = 100
+                    all_embeddings = []
+                    for i in tqdm(
+                        range(0, len(df), BATCH_SIZE), desc="Iterating over batches"
+                    ):
+                        batch_text = df[text_column][i : i + BATCH_SIZE].tolist()
+                        embeddings = litellm.embedding(
+                            model=args["new_model_name"],
+                            input=batch_text,
+                            dimensions=args.get("dimensions"),
+                        )
+                        # add embeddings to df
+                        # embeddings.data is a list of dicts. Each dict has keys "embedding" and "index"
+                        # first sort by "index" and then extract "embedding"
+                        vectors = [
+                            x["embedding"]
+                            for x in sorted(embeddings.data, key=lambda x: x["index"])
+                        ]
+                        dim = len(vectors[0])
+                        all_embeddings.extend(vectors)
+                    # add only the new_vector_column in parquet file
+                    df[new_vector_column] = all_embeddings
+                    df.to_parquet(file_path)
+                    tqdm.write(
+                        f"Computed {len(all_embeddings)} vectors for {len(df)} rows in column:{new_vector_column} of {file_path}"
+                    )
+                    reembed_count += len(all_embeddings)
+                # prepend new_vector_column to vector_columns in namespace_meta
+                if new_vector_column not in namespace_meta["vector_columns"]:
+                    namespace_meta["vector_columns"].insert(0, new_vector_column)
+                else:
+                    tqdm.write(
+                        f"Warning: {new_vector_column} already exists in vector_columns. Overwriting."
+                    )
+                if "model_map" not in namespace_meta:
+                    namespace_meta["model_map"] = {}
+                    for vector_column in namespace_meta["vector_columns"]:
+                        namespace_meta["model_map"][vector_column] = {
+                            "model_name": namespace_meta["model_name"],
+                            "text_column": args["text_column"],
+                            "dimensions": namespace_meta["dimensions"],
+                            "vector_column": vector_column,
+                        }
+                namespace_meta["model_map"][new_vector_column] = {
+                    "model_name": args["new_model_name"],
+                    "text_column": args["text_column"],
+                    "dimensions": dim,
+                    "vector_column": new_vector_column,
+                }
+                namespace_meta["model_name"] = args["new_model_name"]
+                namespace_meta["dimensions"] = dim
+        # write vdf_meta to VDF_META.json
+        f.seek(0)
+        json.dump(vdf_meta, f, indent=4)
+        tqdm.write(
+            f"Reembedding complete. Computed {reembed_count} vectors. Updated VDF_META.json"
         )
-        dims = -1
-        for file in tqdm(parquet_files, desc="Iterating parquet files"):
-            file_path = self.get_file_path(final_data_path, file)
-            df = read_parquet_progress(file_path)
-            first_el = df[vector_column_name].iloc[0]
-            if isinstance(first_el, list) and len(first_el) > 1:
-                return len(first_el)
-            if isinstance(first_el, np.ndarray):
-                if first_el.shape[0] > 1:
-                    return first_el.shape[0]
-                if first_el.shape[0] == 1:
-                    return first_el[0].shape[0]
-        return dims
-
-    # destructor
-    def cleanup(self):
-        for temp_file_path in self.temp_file_paths:
-            if os.path.isfile(temp_file_path):
-                os.remove(temp_file_path)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `vdf_io-0.1.85/src/vdf_io/import_vdf/vertexai_vector_search_import.py` & `vdf_io-0.1.9/src/vdf_io/import_vdf/vertexai_vector_search_import.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 """ 
 Import data to vertex ai vector search index
 """
 
 import argparse
 from typing import Dict, List
-import uuid
-import time
-import numpy as np
+
+from vdf_io.names import DBNames
+from vdf_io.import_vdf.vdf_import_cls import ImportVDB
+from vdf_io.util import set_arg_from_input
+
+# gcloud config set project $PROJECT_ID - users
+import os
 import json
 import itertools
+import pandas as pd
 from tqdm import tqdm
-from ratelimit import limits, sleep_and_retry
-from backoff import on_exception, expo
+from google.cloud import aiplatform as aip
+import google.cloud.aiplatform_v1 as aipv1
 
-# gcloud config set project $PROJECT_ID - users
 # SCOPES = ["https://www.googleapis.com/auth/cloud-platform"]
 
 # NEW
-from google.cloud import aiplatform as aip
-import google.cloud.aiplatform_v1 as aipv1
+import uuid
+import time
+import numpy as np
 from google.cloud import storage
 from google.protobuf import struct_pb2
 from google.cloud.aiplatform_v1.types.index import Index
 from google.cloud.aiplatform_v1.types.index_endpoint import IndexEndpoint
 from google.cloud.aiplatform_v1.types.index_endpoint import DeployedIndex
+from ratelimit import limits, sleep_and_retry
+from backoff import on_exception, expo
 import google.api_core.exceptions as google_exceptions
 
-from vdf_io.names import DBNames
-from vdf_io.import_vdf.vdf_import_cls import ImportVDB
-from vdf_io.util import read_parquet_progress, set_arg_from_input
-from vdf_io.constants import ID_COLUMN
-
 
 # exceptions
 class ResourceNotExistException(Exception):
     def __init__(self, resource: str, message="Resource Does Not Exist."):
         self.resource = resource
         self.message = message
         super().__init__(self.message)
@@ -359,15 +361,15 @@
                     self.local_file_name = "embeddings_0.json"
                     self.contents_delta_uri = (
                         f"gs://{self.gcs_bucket}/{self.gcs_folder}"
                     )
 
                     # dummy embedding - TODO: use input data from parquet(?)
                     init_embedding = {
-                        ID_COLUMN: str(unique_id),
+                        "id": str(unique_id),
                         "embedding": list(np.zeros(self.dimensions)),
                     }
 
                     # dump embedding to a local file
                     with open(self.local_file_name, "w") as f:
                         json.dump(init_embedding, f)
 
@@ -817,15 +819,15 @@
                         + f"already deployed {index.name} to endpoint {self.index_endpoint_name}"
                     )
                     return index_endpoint
 
             invoke_time = time.strftime("%Y%m%d_%H%M%S")
             deployed_index_id = f"{self.index_name.replace('-', '_')}_{invoke_time}"
             deploy_index_config = {
-                ID_COLUMN: deployed_index_id,
+                "id": deployed_index_id,
                 "display_name": deployed_index_id,
                 "index": index.name,
                 "dedicated_resources": {
                     "machine_spec": {
                         "machine_type": machine_type,
                     },
                     "min_replica_count": min_replicas,
@@ -909,26 +911,26 @@
                 print(f"vector_metadata_names : {vector_metadata_names}")
 
                 # Load the data from the parquet files
                 parquet_files = self.get_parquet_files(final_data_path)
 
                 total_ids = []
                 for file in tqdm(parquet_files, desc="Iterating over parquet files"):
-                    file_path = self.get_file_path(final_data_path, file)
-                    df = read_parquet_progress(file_path)
-                    df[ID_COLUMN] = df[ID_COLUMN].apply(lambda x: str(x))
+                    file_path = os.path.join(final_data_path, file)
+                    df = pd.read_parquet(file_path)
+                    df["id"] = df["id"].apply(lambda x: str(x))
 
                     insert_datapoints_payload = []
 
                     for idx, row in tqdm(
                         df.iterrows(), desc="Iterating over rows", total=len(df)
                     ):
                         row = json.loads(row.to_json())
 
-                        total_ids.append(row[ID_COLUMN])
+                        total_ids.append(row["id"])
                         row[vector_column_name] = [
                             float(emb) for emb in row[vector_column_name]
                         ]
                         numeric_restrict_entry_list = []
                         restrict_entry_list = []
                         allow_values = []
                         deny_values = []
@@ -989,15 +991,15 @@
                             # if idx == 10:
                             #     # sanity check
                             #     print(f"crowding_tag_col : {crowding_tag_col}")
                             #     print(f"crowding_tag_val : {crowding_tag_val}")
 
                         insert_datapoints_payload.append(
                             aipv1.IndexDatapoint(
-                                datapoint_id=row[ID_COLUMN],
+                                datapoint_id=row["id"],
                                 feature_vector=row[vector_column_name],
                                 restricts=restrict_entry_list,
                                 numeric_restricts=numeric_restrict_entry_list,
                                 crowding_tag=aipv1.IndexDatapoint.CrowdingTag(
                                     crowding_attribute=crowding_tag_val
                                 ),
                             )
```

### Comparing `vdf_io-0.1.85/src/vdf_io/import_vdf_cli.py` & `vdf_io-0.1.9/src/vdf_io/import_vdf_cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 #!/usr/bin/env python3
 
 import argparse
 import os
 import time
 from dotenv import load_dotenv
-import traceback
 
 import sentry_sdk
 from opentelemetry import trace
 from opentelemetry.propagate import set_global_textmap
 from opentelemetry.sdk.trace import TracerProvider
 from sentry_sdk.integrations.opentelemetry import SentrySpanProcessor, SentryPropagator
 
 import vdf_io
-from vdf_io.constants import ID_COLUMN, INT_MAX
 from vdf_io.names import DBNames
-from vdf_io.scripts.check_for_updates import check_for_updates
 from vdf_io.util import set_arg_from_input
 from vdf_io.import_vdf.pinecone_import import ImportPinecone
 from vdf_io.import_vdf.qdrant_import import ImportQdrant
 from vdf_io.import_vdf.kdbai_import import ImportKDBAI
 from vdf_io.import_vdf.milvus_import import ImportMilvus
 from vdf_io.import_vdf.vertexai_vector_search_import import ImportVertexAIVectorSearch
 from vdf_io.import_vdf.vdf_import_cls import ImportVDB
@@ -51,15 +48,14 @@
     with tracer.start_as_current_span("import_vdf_cli_main") as span:
         try:
             run_import(span)
             sentry_sdk.flush()
         except Exception as e:
             sentry_sdk.flush()
             print(f"Error: {e}")
-            traceback.print_exc()
             return
         finally:
             sentry_sdk.flush()
     sentry_sdk.flush()
     return
 
 
@@ -100,25 +96,24 @@
 
     make_common_options(parser)
     add_subparsers_for_dbs(subparsers, db_choices)
 
     args = parser.parse_args()
     args = vars(args)
     args["library_version"] = vdf_io.__version__
-    if args.get("hf_dataset") is None:
-        set_arg_from_input(
-            args, "dir", "Enter the directory of vector dataset to be imported: ", str
-        )
+    set_arg_from_input(
+        args, "dir", "Enter the directory of vector dataset to be imported: ", str
+    )
     if args["subset"]:
         set_arg_from_input(
             args,
             "max_num_rows",
             "Maximum number of vectors you'd like to load",
             int,
-            INT_MAX,
+            2**63-1,
         )
 
     args["cwd"] = os.getcwd()
 
     start_time = time.time()
 
     if (
@@ -140,16 +135,14 @@
 
     for key in list(import_obj.args.keys()):
         if key in ARGS_ALLOWLIST:
             span.set_attribute(key, import_obj.args[key])
 
     print(f"Time taken: {end_time - start_time:.2f} seconds")
     span.set_attribute("import_time", end_time - start_time)
-    import_obj.cleanup()
-    check_for_updates()
 
 
 def make_common_options(parser):
     parser.add_argument("-d", "--dir", type=str, help="Directory to import")
     parser.add_argument(
         "--hf_dataset",
         type=str,
@@ -163,38 +156,20 @@
         default=False,
         action=argparse.BooleanOptionalAction,
     )
     parser.add_argument(
         "--max_num_rows",
         type=int,
         help="Maximum number of rows you'd like to load",
-        default=INT_MAX,
+        default=2**63-1,
     )
     parser.add_argument(
         "--create_new",
         type=bool,
         help="Create a new index (default: False)",
         default=False,
         action=argparse.BooleanOptionalAction,
     )
-    parser.add_argument(
-        "--vector_columns",
-        type=str,
-        help="Vector column names (comma separated) eg: 'vector1,vector2'",
-        default="vector",
-    )
-    parser.add_argument(
-        "--metric",
-        type=str,
-        help="Distance metric to use (default: 'Cosine')",
-        default="Cosine",
-    )
-    parser.add_argument(
-        "--id_column",
-        type=str,
-        help="ID column name (default: 'id')",
-        default=ID_COLUMN,
-    )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `vdf_io-0.1.85/src/vdf_io/meta_types.py` & `vdf_io-0.1.9/src/vdf_io/meta_types.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pydantic import BaseModel, ConfigDict
-from typing import Dict, List, Optional
+from typing import Dict, List
 
 
 class NamespaceMeta(BaseModel):
     namespace: str
     index_name: str
     total_vector_count: int
     exported_vector_count: int
@@ -18,8 +18,7 @@
 class VDFMeta(BaseModel):
     version: str
     file_structure: List[str]
     author: str
     exported_from: str
     indexes: Dict[str, List[NamespaceMeta]]
     exported_at: str
-    id_column: Optional[str] = None
```

### Comparing `vdf_io-0.1.85/src/vdf_io/scripts/bump_version.py` & `vdf_io-0.1.9/src/vdf_io/scripts/bump_version.py`

 * *Files identical despite different names*

### Comparing `vdf_io-0.1.85/src/vdf_io/scripts/check_for_updates.py` & `vdf_io-0.1.9/src/vdf_io/scripts/check_for_updates.py`

 * *Files identical despite different names*

### Comparing `vdf_io-0.1.85/src/vdf_io/scripts/consolidate_parquet.py` & `vdf_io-0.1.9/src/vdf_io/scripts/consolidate_parquet.py`

 * *Files identical despite different names*

### Comparing `vdf_io-0.1.85/src/vdf_io/scripts/count_rows.py` & `vdf_io-0.1.9/src/vdf_io/scripts/count_rows.py`

 * *Files identical despite different names*

### Comparing `vdf_io-0.1.85/src/vdf_io/scripts/get_id_list.py` & `vdf_io-0.1.9/src/vdf_io/scripts/get_id_list.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 #!/usr/bin/env python3
 
 import os
 import pandas as pd
 
-from vdf_io.util import expand_shorthand_path, read_parquet_progress
-from vdf_io.constants import ID_COLUMN
+from vdf_io.util import expand_shorthand_path
 
 # script to get list of ids from directory of parquet files
 
 
 def get_ids_from_parquet(directory):
     # for os.walk
     ids = set()
@@ -19,16 +18,16 @@
             if file.endswith(".parquet"):
                 # get the path to the file
                 path = os.path.join(root, file)
                 # open the file
                 # read only the id column
                 try:
                     # Read only the 'id' column from the parquet file
-                    df = read_parquet_progress(path, columns=[ID_COLUMN])
-                    ids.update(df[ID_COLUMN].tolist())
+                    df = pd.read_parquet(path, columns=["id"])
+                    ids.update(df["id"].tolist())
                 except Exception as e:
                     print(f"Error reading {file}: {e}")
     return ids
 
 
 dir = input("Enter directory of parquet files: ")
 ids = get_ids_from_parquet(dir)
```

### Comparing `vdf_io-0.1.85/src/vdf_io/scripts/push_to_hub_vdf.py` & `vdf_io-0.1.9/src/vdf_io/scripts/push_to_hub_vdf.py`

 * *Files identical despite different names*

### Comparing `vdf_io-0.1.85/src/vdf_io/util.py` & `vdf_io-0.1.9/src/vdf_io/util.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 from pathlib import Path
 from collections import OrderedDict
 from getpass import getpass
 import hashlib
 import json
 import os
-from uuid import UUID
-import pandas as pd
+from qdrant_client.http.models import Distance
 from io import StringIO
 import sys
-from tqdm import tqdm
 
-from qdrant_client.http.models import Distance
 
 from vdf_io.names import DBNames
 
 
 def sort_recursive(d):
     """
     Recursively sort the nested dictionary by its keys.
@@ -74,17 +71,15 @@
     return int(hashlib.md5(string_value.encode("utf-8")).hexdigest(), 16)
 
 
 def set_arg_from_input(args, arg_name, prompt, type_name=str, default_value=None):
     """
     Set the value of an argument from user input if it is not already present
     """
-    if arg_name not in args or (
-        args[arg_name] is None and default_value != "DO_NOT_PROMPT"
-    ):
+    if arg_name not in args or args[arg_name] is None:
         inp = input(prompt)
         if inp == "":
             args[arg_name] = None if default_value is None else type_name(default_value)
         else:
             args[arg_name] = type_name(inp)
     return
 
@@ -103,16 +98,14 @@
 def expand_shorthand_path(shorthand_path):
     """
     Expand shorthand notations in a file path to a full path-like object.
 
     :param shorthand_path: A string representing the shorthand path.
     :return: A Path object representing the full path.
     """
-    if shorthand_path is None:
-        return None
     # Expand '~' to the user's home directory
     expanded_path = os.path.expanduser(shorthand_path)
 
     # Resolve '.' and '..' to get the absolute path
     full_path = Path(expanded_path).resolve()
 
     return str(full_path)
@@ -188,41 +181,20 @@
             f"Joined path: {final_data_path}\n"
             f"Current working directory: {cwd}\n"
             f"Command line arg (dir): {dir}"
         )
     return final_data_path
 
 
-def get_parquet_files(data_path, args, temp_file_paths=[]):
+def get_parquet_files(data_path, args):
     # Load the data from the parquet files
     if args.get("hf_dataset", None):
-        if args.get("max_num_rows", None):
-            from datasets import load_dataset
-
-            tqdm.write("Loading a subset of the dataset")
-            ds = load_dataset(args.get("hf_dataset"), split="train", streaming=True)
-            tqdm.write("Taking a subset of the dataset")
-            it_ds = ds.take(args.get("max_num_rows"))
-            tqdm.write("Converting to pandas dataframe")
-            df = pd.DataFrame(it_ds)
-            tqdm.write("Writing to parquet")
-            temp_file_path = f"{os.getcwd()}/temp.parquet"
-            df.to_parquet(temp_file_path)
-            temp_file_paths.append(temp_file_path)
-            tqdm.write("Writing complete")
-            return [temp_file_path]
         from huggingface_hub import HfFileSystem
-
-        fs = HfFileSystem()
-        return [
-            "hf://" + x
-            for x in fs.glob(
-                f"datasets/{args.get('hf_dataset')}/{data_path if data_path!='.' else ''}/**.parquet"
-            )
-        ]
+        fs = HfFileSystem(token=os.environ.get("HUGGING_FACE_TOKEN", ""))
+        return fs.glob(f"datasets/{args.get('hf_dataset')}/{data_path}/**.parquet")
     if not os.path.isdir(data_path):
         if data_path.endswith(".parquet"):
             return [data_path]
         else:
             raise Exception(f"Invalid data path '{data_path}'")
     else:
         parquet_files = sorted(
@@ -252,39 +224,24 @@
     # Check if the current parser has subparsers
     if hasattr(parser, "_subparsers"):
         for _, subparser in parser._subparsers._group_actions[0].choices.items():
             # Recursively print help for each subparser
             print_help_recursively(subparser, level + 1)
 
 
-def is_str_uuid(id_str):
-    try:
-        uuid_obj = UUID(id_str)
-        return str(uuid_obj)
-    except ValueError:
-        return False
-
+# Create the top-level parser
+# parser = argparse.ArgumentParser(description='Top-level parser')
+# parser.add_argument('--foo', help='foo help')
+
+# # Create a subparser
+# subparsers = parser.add_subparsers(help='sub-command help')
+
+# # Create the subparser for the "a" command
+# parser_a = subparsers.add_parser('a', help='a help')
+# parser_a.add_argument('--bar', type=int, help='bar help')
+
+# # Create another subparser for the "b" command
+# parser_b = subparsers.add_parser('b', help='b help')
+# parser_b.add_argument('--baz', choices='XYZ', help='baz help')
 
-def get_qdrant_id_from_id(idx):
-    if isinstance(idx, int) or idx.isdigit():
-        return int(idx)
-    elif not is_str_uuid(idx):
-        hex_string = hashlib.md5(idx.encode("UTF-8")).hexdigest()
-        return str(UUID(hex=hex_string))
-    else:
-        return str(UUID(idx))
-
-
-def read_parquet_progress(file_path):
-    if file_path.startswith("hf://"):
-        from huggingface_hub import HfFileSystem
-        from huggingface_hub import hf_hub_download
-
-        fs = HfFileSystem()
-        resolved_path = fs.resolve_path(file_path)
-        cache_path = hf_hub_download(
-            repo_id=resolved_path.repo_id,
-            filename=resolved_path.path_in_repo,
-            repo_type=resolved_path.repo_type,
-        )
-        return pd.read_parquet(cache_path)
-    return pd.read_parquet(file_path)
+# # Recursively print help messages
+# print_help_recursively(parser)
```

### Comparing `vdf_io-0.1.85/src/vdf_io.egg-info/SOURCES.txt` & `vdf_io-0.1.9/src/vdf_io.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 LICENSE
 README.md
 setup.py
 src/vdf_io/__init__.py
-src/vdf_io/constants.py
 src/vdf_io/export_vdf_cli.py
 src/vdf_io/import_vdf_cli.py
 src/vdf_io/meta_types.py
 src/vdf_io/names.py
 src/vdf_io/print_help_rec.py
 src/vdf_io/util.py
 src/vdf_io.egg-info/PKG-INFO
@@ -30,11 +29,10 @@
 src/vdf_io/import_vdf/vdf_import_cls.py
 src/vdf_io/import_vdf/vertexai_vector_search_import.py
 src/vdf_io/scripts/__init__.py
 src/vdf_io/scripts/bump_version.py
 src/vdf_io/scripts/check_for_updates.py
 src/vdf_io/scripts/consolidate_parquet.py
 src/vdf_io/scripts/count_rows.py
-src/vdf_io/scripts/count_rows_hf.py
 src/vdf_io/scripts/get_id_list.py
 src/vdf_io/scripts/push_to_hub_vdf.py
 src/vdf_io/scripts/reembed.py
```

