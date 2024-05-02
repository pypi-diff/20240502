# Comparing `tmp/bioomics-0.2.6.tar.gz` & `tmp/bioomics-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioomics-0.2.6.tar", last modified: Tue Apr 30 12:21:58 2024, max compression
+gzip compressed data, was "bioomics-0.2.8.tar", last modified: Thu May  2 20:09:47 2024, max compression
```

## Comparing `bioomics-0.2.6.tar` & `bioomics-0.2.8.tar`

### file list

```diff
@@ -1,64 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:21:58.724175 bioomics-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-30 12:21:49.000000 bioomics-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-04-30 12:21:58.724175 bioomics-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-30 12:21:49.000000 bioomics-0.2.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 12:21:58.724175 bioomics-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-30 12:21:49.000000 bioomics-0.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:21:58.716174 bioomics-0.2.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:21:58.716174 bioomics-0.2.6/src/bioomics/
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-30 12:21:49.000000 bioomics-0.2.6/src/bioomics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-04-30 12:21:49.000000 bioomics-0.2.6/src/bioomics/bio_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-30 12:21:49.000000 bioomics-0.2.6/src/bioomics/bio_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:21:58.720174 bioomics-0.2.6/src/bioomics/connector/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:21:49.000000 bioomics-0.2.6/src/bioomics/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-04-30 12:21:49.000000 bioomics-0.2.6/src/bioomics/connector/conn_ftp.py
--rw-r--r--   0 runner    (1001) docker     (127)     6451 2024-04-30 12:21:49.000000 bioomics-0.2.6/src/bioomics/connector/conn_ftplib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-30 12:21:49.000000 bioomics-0.2.6/src/bioomics/connector/conn_http.py
--rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-04-30 12:21:49.000000 bioomics-0.2.6/src/bioomics/connector/conn_redis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:21:58.720174 bioomics-0.2.6/src/bioomics/constants/
--rw-r--r--   0 runner    (1001) docker     (127)    26628 2024-04-30 12:21:49.000000 bioomics-0.2.6/src/bioomics/constants/IEDB.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:21:58.720174 bioomics-0.2.6/src/bioomics/immune/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:21:49.000000 bioomics-0.2.6/src/bioomics/immune/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15672 2024-04-30 12:21:49.000000 bioomics-0.2.6/src/bioomics/immune/iedb.py
--rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-04-30 12:21:49.000000 bioomics-0.2.6/src/bioomics/immune/iedb_antigen.py
--rw-r--r--   0 runner    (1001) docker     (127)     5110 2024-04-30 12:21:49.000000 bioomics-0.2.6/src/bioomics/immune/iedb_epitope.py
--rw-r--r--   0 runner    (1001) docker     (127)     4731 2024-04-30 12:21:49.000000 bioomics-0.2.6/src/bioomics/integrate_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-30 12:21:49.000000 bioomics-0.2.6/src/bioomics/mirbase.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:21:58.720174 bioomics-0.2.6/src/bioomics/ncbi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:21:49.000000 bioomics-0.2.6/src/bioomics/ncbi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-04-30 12:21:49.000000 bioomics-0.2.6/src/bioomics/ncbi/ncbi.py
--rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-04-30 12:21:49.000000 bioomics-0.2.6/src/bioomics/ncbi/refseq.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-30 12:21:49.000000 bioomics-0.2.6/src/bioomics/ncbi/retrieve_ncbi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:21:58.720174 bioomics-0.2.6/src/bioomics/protein/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:21:49.000000 bioomics-0.2.6/src/bioomics/protein/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-30 12:21:49.000000 bioomics-0.2.6/src/bioomics/protein/expasy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4023 2024-04-30 12:21:49.000000 bioomics-0.2.6/src/bioomics/protein/uniprot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-30 12:21:49.000000 bioomics-0.2.6/src/bioomics/protein/uniprot_sprot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-30 12:21:49.000000 bioomics-0.2.6/src/bioomics/protein/uniprot_trembl.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-30 12:21:49.000000 bioomics-0.2.6/src/bioomics/rnacentral.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:21:58.724175 bioomics-0.2.6/src/bioomics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-04-30 12:21:58.000000 bioomics-0.2.6/src/bioomics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-30 12:21:58.000000 bioomics-0.2.6/src/bioomics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 12:21:58.000000 bioomics-0.2.6/src/bioomics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-30 12:21:58.000000 bioomics-0.2.6/src/bioomics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-30 12:21:58.000000 bioomics-0.2.6/src/bioomics.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:21:58.720174 bioomics-0.2.6/src/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:21:49.000000 bioomics-0.2.6/src/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:21:49.000000 bioomics-0.2.6/src/pipelines/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-30 12:21:49.000000 bioomics-0.2.6/src/pipelines/retrieve_epitopes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:21:58.724175 bioomics-0.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-30 12:21:49.000000 bioomics-0.2.6/tests/test_conn_ftp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-04-30 12:21:49.000000 bioomics-0.2.6/tests/test_conn_ftplib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-30 12:21:49.000000 bioomics-0.2.6/tests/test_conn_http.py
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-30 12:21:49.000000 bioomics-0.2.6/tests/test_conn_redis.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-30 12:21:49.000000 bioomics-0.2.6/tests/test_expasy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-04-30 12:21:49.000000 bioomics-0.2.6/tests/test_iedb.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-30 12:21:49.000000 bioomics-0.2.6/tests/test_iedb_antigen.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-30 12:21:49.000000 bioomics-0.2.6/tests/test_iedb_epitope.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-30 12:21:49.000000 bioomics-0.2.6/tests/test_mirbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-04-30 12:21:49.000000 bioomics-0.2.6/tests/test_ncbi.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-30 12:21:49.000000 bioomics-0.2.6/tests/test_refseq.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-30 12:21:49.000000 bioomics-0.2.6/tests/test_rnacentral.py
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-30 12:21:49.000000 bioomics-0.2.6/tests/test_uniprot.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-30 12:21:49.000000 bioomics-0.2.6/tests/test_uniprot_sprot.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-30 12:21:49.000000 bioomics-0.2.6/tests/test_uniprot_trembl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:09:47.741722 bioomics-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-02 20:09:42.000000 bioomics-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-05-02 20:09:47.741722 bioomics-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-02 20:09:42.000000 bioomics-0.2.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 20:09:47.741722 bioomics-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-02 20:09:42.000000 bioomics-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:09:47.729722 bioomics-0.2.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:09:47.733722 bioomics-0.2.8/src/bioomics/
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-02 20:09:42.000000 bioomics-0.2.8/src/bioomics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-05-02 20:09:42.000000 bioomics-0.2.8/src/bioomics/bio_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-02 20:09:42.000000 bioomics-0.2.8/src/bioomics/bio_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:09:47.733722 bioomics-0.2.8/src/bioomics/connector/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 20:09:42.000000 bioomics-0.2.8/src/bioomics/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-05-02 20:09:42.000000 bioomics-0.2.8/src/bioomics/connector/conn_ftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6451 2024-05-02 20:09:42.000000 bioomics-0.2.8/src/bioomics/connector/conn_ftplib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-02 20:09:42.000000 bioomics-0.2.8/src/bioomics/connector/conn_http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-05-02 20:09:42.000000 bioomics-0.2.8/src/bioomics/connector/conn_redis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:09:47.733722 bioomics-0.2.8/src/bioomics/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)    26628 2024-05-02 20:09:42.000000 bioomics-0.2.8/src/bioomics/constants/IEDB.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:09:47.737722 bioomics-0.2.8/src/bioomics/immune/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 20:09:42.000000 bioomics-0.2.8/src/bioomics/immune/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15672 2024-05-02 20:09:42.000000 bioomics-0.2.8/src/bioomics/immune/iedb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-05-02 20:09:42.000000 bioomics-0.2.8/src/bioomics/immune/iedb_antigen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5110 2024-05-02 20:09:42.000000 bioomics-0.2.8/src/bioomics/immune/iedb_epitope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5516 2024-05-02 20:09:42.000000 bioomics-0.2.8/src/bioomics/integrate_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-02 20:09:42.000000 bioomics-0.2.8/src/bioomics/mirbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-02 20:09:42.000000 bioomics-0.2.8/src/bioomics/multi_threads.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:09:47.737722 bioomics-0.2.8/src/bioomics/ncbi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 20:09:42.000000 bioomics-0.2.8/src/bioomics/ncbi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-05-02 20:09:42.000000 bioomics-0.2.8/src/bioomics/ncbi/genBank.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5519 2024-05-02 20:09:42.000000 bioomics-0.2.8/src/bioomics/ncbi/integrate_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-05-02 20:09:42.000000 bioomics-0.2.8/src/bioomics/ncbi/ncbi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-02 20:09:42.000000 bioomics-0.2.8/src/bioomics/ncbi/parse_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-05-02 20:09:42.000000 bioomics-0.2.8/src/bioomics/ncbi/refseq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:09:47.737722 bioomics-0.2.8/src/bioomics/protein/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 20:09:42.000000 bioomics-0.2.8/src/bioomics/protein/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-02 20:09:42.000000 bioomics-0.2.8/src/bioomics/protein/expasy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4023 2024-05-02 20:09:42.000000 bioomics-0.2.8/src/bioomics/protein/uniprot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-02 20:09:42.000000 bioomics-0.2.8/src/bioomics/protein/uniprot_sprot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-02 20:09:42.000000 bioomics-0.2.8/src/bioomics/protein/uniprot_trembl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-02 20:09:42.000000 bioomics-0.2.8/src/bioomics/rnacentral.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:09:47.741722 bioomics-0.2.8/src/bioomics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-05-02 20:09:47.000000 bioomics-0.2.8/src/bioomics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-05-02 20:09:47.000000 bioomics-0.2.8/src/bioomics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 20:09:47.000000 bioomics-0.2.8/src/bioomics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-02 20:09:47.000000 bioomics-0.2.8/src/bioomics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-02 20:09:47.000000 bioomics-0.2.8/src/bioomics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:09:47.737722 bioomics-0.2.8/src/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 20:09:42.000000 bioomics-0.2.8/src/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 20:09:42.000000 bioomics-0.2.8/src/pipelines/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-02 20:09:42.000000 bioomics-0.2.8/src/pipelines/retrieve_epitopes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:09:47.741722 bioomics-0.2.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-02 20:09:42.000000 bioomics-0.2.8/tests/test_conn_ftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-02 20:09:42.000000 bioomics-0.2.8/tests/test_conn_ftplib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-02 20:09:42.000000 bioomics-0.2.8/tests/test_conn_http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-05-02 20:09:42.000000 bioomics-0.2.8/tests/test_conn_redis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-02 20:09:42.000000 bioomics-0.2.8/tests/test_expasy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-02 20:09:42.000000 bioomics-0.2.8/tests/test_genbank.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-02 20:09:42.000000 bioomics-0.2.8/tests/test_iedb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-02 20:09:42.000000 bioomics-0.2.8/tests/test_iedb_antigen.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-02 20:09:42.000000 bioomics-0.2.8/tests/test_iedb_epitope.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-02 20:09:42.000000 bioomics-0.2.8/tests/test_integrate_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-02 20:09:42.000000 bioomics-0.2.8/tests/test_mirbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-02 20:09:42.000000 bioomics-0.2.8/tests/test_ncbi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-02 20:09:42.000000 bioomics-0.2.8/tests/test_parse_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-02 20:09:42.000000 bioomics-0.2.8/tests/test_refseq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-02 20:09:42.000000 bioomics-0.2.8/tests/test_rnacentral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-02 20:09:42.000000 bioomics-0.2.8/tests/test_uniprot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-02 20:09:42.000000 bioomics-0.2.8/tests/test_uniprot_sprot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-02 20:09:42.000000 bioomics-0.2.8/tests/test_uniprot_trembl.py
```

### Comparing `bioomics-0.2.6/LICENSE` & `bioomics-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.6/PKG-INFO` & `bioomics-0.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioomics
-Version: 0.2.6
+Version: 0.2.8
 Summary: Download, retrieve and process omics data for further bioinformatics
 Home-page: https://github.com/Tiezhengyuan/bio_omics
 Author: Tiezheng Yuan
 Author-email: tiezhengyuan@hotmail.com
 Keywords: pypi,cicd,python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `bioomics-0.2.6/README.md` & `bioomics-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.6/setup.py` & `bioomics-0.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\\n" + fh.read()
 
 setup(
     name="bioomics",
-    version='0.2.6',
+    version='0.2.8',
     author="Tiezheng Yuan",
     author_email="tiezhengyuan@hotmail.com",
     description="Download, retrieve and process omics data for further bioinformatics",
     url = "https://github.com/Tiezhengyuan/bio_omics",
     long_description_content_type="text/markdown",
     long_description=long_description,
     package_dir={"": "src"},
```

### Comparing `bioomics-0.2.6/src/bioomics/bio_dict.py` & `bioomics-0.2.8/src/bioomics/bio_dict.py`

 * *Files 9% similar despite different names*

```diff
@@ -78,8 +78,22 @@
         return {
             'feature_name': ft.key,
             'location': ft.location,
             'qualifiers': qualifiers,
             'seq_start': start,
             'seq_end': end,
             'seq': record.sequence[start-1:end],
-        }
+        }
+
+    @staticmethod
+    def fasta(record):
+        output =  {
+            'description': record.description,
+            'id': record.id,
+            'name': record.name,
+            'seq': str(record.seq),
+        }
+        for attr in ['annotations', 'features', 'dbxrefs']:
+            if hasattr(record, attr):
+                output[attr] = getattr(record, attr)
+        output['accession'] = record.id.split('.', 1)[0]
+        return output
```

### Comparing `bioomics-0.2.6/src/bioomics/connector/conn_ftp.py` & `bioomics-0.2.8/src/bioomics/connector/conn_ftp.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,23 +69,23 @@
         # doesn't download if file exists and overwrite is False
         if self.overwrite is False:
             if os.path.isfile(unzip_file):
                 return unzip_file
             elif os.path.isfile(local_file):
                 return local_file
         
-        # connect FTP
-        ftp = FTP(self.url)
-        ftp.login()
-        if endpoint:
-            ftp.cwd(endpoint)
-        ftp_file = f"{self.url}/{endpoint}/{file_name}"
-        
         # download
         try:
+            # connect FTP
+            ftp = FTP(self.url)
+            ftp.login()
+            if endpoint:
+                ftp.cwd(endpoint)
+            ftp_file = f"{self.url}/{endpoint}/{file_name}"
+            # donwload
             with open(local_file, 'wb') as f:
                 ftp.retrbinary(f"RETR {file_name}", f.write)
                 print(f"Download {ftp_file}")
         except Exception as e:
             print('Failure: download data from FTP, error=', e)
             os.remove(local_file)
             local_file = None
```

### Comparing `bioomics-0.2.6/src/bioomics/connector/conn_ftplib.py` & `bioomics-0.2.8/src/bioomics/connector/conn_ftplib.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.6/src/bioomics/connector/conn_http.py` & `bioomics-0.2.8/src/bioomics/connector/conn_http.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.6/src/bioomics/connector/conn_redis.py` & `bioomics-0.2.8/src/bioomics/connector/conn_redis.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.6/src/bioomics/constants/IEDB.py` & `bioomics-0.2.8/src/bioomics/constants/IEDB.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.6/src/bioomics/immune/iedb.py` & `bioomics-0.2.8/src/bioomics/immune/iedb.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.6/src/bioomics/immune/iedb_antigen.py` & `bioomics-0.2.8/src/bioomics/immune/iedb_antigen.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.6/src/bioomics/immune/iedb_epitope.py` & `bioomics-0.2.8/src/bioomics/immune/iedb_epitope.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.6/src/bioomics/integrate_data.py` & `bioomics-0.2.8/src/bioomics/integrate_data.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 '''
 '''
 from biosequtils import Dir
 import os
 import json
 import math
 from typing import Iterable
+from datetime import datetime
 
 class IntegrateData:
     def __init__(self, entity_path:str):
         '''
         args: entity_path: store integrated data.
+        args: key_index: use key as index or build new index if
         '''
         self.entity_path = entity_path
         Dir(self.entity_path).init_dir()
         self.index_meta = self.get_index_meta()
 
     def get_index_meta(self) -> dict:
         '''
@@ -51,17 +53,24 @@
             meta = {
                 'entity_path': self.entity_path,
                 'index_meta_file': self.index_meta_file,
                 'meta_file': meta_file,
             }
         # update meta
         meta.update(updated_meta)
+        meta['start_time'] = datetime.now()
         return meta
 
     def save_meta(self, meta:dict):
+        end_time = datetime.now()
+        delta = end_time - meta['start_time']
+        meta['duration'] = delta.seconds
+        meta['start_time'] = meta['start_time'].strftime("%m/%d/Y, %H:%M:%S")
+        meta['end_time'] = end_time.strftime("%m/%d/Y, %H:%M:%S")
+        # save
         with open(meta['meta_file'], 'w') as f:
             json.dump(meta, f, indent=4)
         return meta['meta_file']
         
     def scan(self) -> Iterable:
         '''
         Note: self.index_meta could be updated
@@ -72,48 +81,55 @@
             if os.path.isfile(file):
                 with open(file, 'r') as f:
                     data = json.load(f)
                     yield data
 
     def next_id(self) -> str:
         if self.index_meta:
-            ids = [int(i['ID']) for i in self.index_meta.values()]
+            ids = [int(i['key']) for i in self.index_meta.values()]
             return str(max(ids) + 1)
         return '1'
     
     def new_json_path(self, new_id:str) -> str:
         '''
         id = '1234'
         path: ./12/34/1234.json
         '''
         id_prefix = str(math.floor(int(new_id)/1000))
         sub_dirs = [id_prefix[i:i+2] for i in range(0, len(id_prefix), 2)]
-        path = os.path.join(self.entity_path, *sub_dirs)
+        path = os.path.join(self.entity_path, 'data', *sub_dirs)
         Dir(path).init_dir()
         json_file = os.path.join(path, f'{new_id}.json')
         return json_file
+
+    def key_json_path(self, key_value:str):
+        id_prefix = str(key_value)[:-2]
+        sub_dirs = [id_prefix[i:i+3] for i in range(0, len(id_prefix), 3)]
+        path = os.path.join(self.entity_path, 'data',  *sub_dirs)
+        Dir(path).init_dir()
+        json_file = os.path.join(path, f'{key_value}.json')
+        return json_file
     
     def add_data(self, data:dict, key_value:str=None, source:str=None):
         '''
-        'key' and 'ID' are added into new data
+        'key' is added into new data
         key is unique id for identification of data
         key could be new_id or accession
         '''
-        new_id = self.next_id()
-        json_file = self.new_json_path(new_id)
+        json_file = None
         if key_value is None:
-            key_value = new_id
-        new_data = {
-            'ID': new_id,
-            'key': key_value
-        }
+            key_value = self.next_id()
+            json_file = self.new_json_path(self.next_id())
+        else:
+            json_file = self.key_json_path(key_value)
+                    
+        new_data = {'key': key_value}
         new_data.update(data)
         # update index_meta
         self.index_meta[key_value] = {
-            'ID': new_id,
             'key': key_value,
             'json_file': json_file,
             'source': [source if source else "UNKNOWN",],
         }
         with open(json_file, 'w') as f:
             json.dump(new_data, f, indent=4)
             return json_file
```

### Comparing `bioomics-0.2.6/src/bioomics/mirbase.py` & `bioomics-0.2.8/src/bioomics/mirbase.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.6/src/bioomics/ncbi/ncbi.py` & `bioomics-0.2.8/src/bioomics/ncbi/ncbi.py`

 * *Files 15% similar despite different names*

```diff
@@ -49,14 +49,34 @@
         local_files = self.download_files(
             endpoint = ftp_path.replace('https://ftp.ncbi.nlm.nih.gov/', ''),
             match = '.gz',
             local_path = local_path,
         )
         return local_path, local_files
     
+
+    def download_id_mapping(self):
+        '''
+        '''
+        local_files = []
+        file_names = ['gene2accession.gz', 'gene2ensembl.gz', 'gene2go.gz', \
+            'gene2pubmed.gz', 'gene2refseq.gz', 'gene_group.gz', 'gene_history.gz', \
+            'gene_info.gz', 'gene_neighbors.gz', 'gene_orthologs.gz', \
+            'gene_refseq_uniprotkb_collab.gz',]
+        for file_name in file_names:
+            local_file = self.download_file(
+                endpoint='gene/DATA',
+                file_name=file_name,
+                local_path=os.path.join(self.local_path, 'gene', 'DATA'),
+            )
+            if local_file:
+                local_files.append(local_file)
+        return local_files
+
+
     def download_refseq_uniprotkb(self):
         '''
         download gene_refseq_uniprotkb_collab.gz from 
         https://ftp.ncbi.nlm.nih.gov/refseq/uniprotkb/
         map refeseq ~ uniprotkb
         '''
         local_file = self.download_file(
@@ -85,14 +105,26 @@
             local_files += self.download_files(
             local_path = os.path.join(self.local_path, 'refseq', 'release', 'gpff'),
             endpoint = f'refseq/release/{sub}/',
             match = '.gpff.gz$'
         )
         return local_files
 
+    def download_protein_fasta(self):
+        local_files = []
+        for i in range(1, 260):
+            local_file = self.download_file(
+                endpoint='ncbi-asn1/protein_fasta/',
+                file_name=f"gbbct{i}.fsa_aa.gz",
+                local_path=os.path.join(self.local_path, 'protein_fasta'),
+            )
+            if local_file:
+                local_files.append(local_file)
+        return local_files
+
 
     def download_gene_data(self):
         '''
         download /gene/DATA including subdirectories and files
         '''
         local_files = self.download_tree(
             local_path = os.path.join(self.local_path, 'gene', 'DATA'),
```

### Comparing `bioomics-0.2.6/src/bioomics/ncbi/refseq.py` & `bioomics-0.2.8/src/bioomics/protein/uniprot.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,127 +1,109 @@
-
-import pandas as pd
+"""
+FTP of UniProtKB/Swiss-Prot
+"""
+from Bio import SeqIO
+from biosequtils import Dir
+import gzip
+import os
 import json
+from typing import Iterable
 
-
-from .ncbi import NCBI
-from ..bio_handler import BioHandler
+from ..connector.conn_ftp import ConnFTP
 from ..bio_dict import BioDict
 from ..integrate_data import IntegrateData
 
-class Refseq:
-    source = 'NCBI_refseq'
-    meta_file_name = 'ncbi_refseq_meta.json'
+class UniProt(ConnFTP):
+    url = "ftp.uniprot.org"
 
-    def __init__(self, local_path:str):
-        self.local_path = local_path
-
-    # NOTE: no epitopes detect in refseq
-    def process_epitope(self, entity_path):
-        entity_path = entity_path if entity_path \
-            else os.path.join(self.local_path, 'epitope')
+    def __init__(self, local_path:str, overwrite:bool=None):
+        super().__init__(url=self.url, overwrite=overwrite)
+        self.local_path = self.local_path = os.path.join(local_path, "UniProt")
+        Dir(self.local_path).init_dir()
         self.meta = {
-            'source': self.source,
-            'entity_path': entity_path,
+            'url': self.url,
+            'local_path': local_path,
         }
-        self.integrate = IntegrateData(entity_path)
-        self.meta = self.integrate.get_meta(self.meta)
-
-        # download
-        # NOTE: no epitopes detect in refseq
-        # local_files = NCBI(self.local_path).download_refseq_gpff()
-        local_files = NCBI(self.local_path).download_refseq_complete_gpff()
-
-        # detect epitope in feature.note
-        for gpff_gz in local_files:
-            if os.path.isfile(gpff_gz):
-                print(f"Try to detect epitopes in the file {gpff_gz}.")
-                entity_data = self.parse_epitope(gpff_gz)
-                count = self.integrate_epitope(entity_data)
-                print(count)
-                for k,v in count.items():
-                    if k not in self.meta:
-                        self.meta[k] = 0
-                    self.meta[k] += v
-
-        self.integrate.save_meta(self.meta)
-        self.integrate.save_index_meta()
-        return True
-    
-    def parse_epitope(self, local_gpff:str):
-        '''
-        detect proteins with epitopes defined
+  
+    def parse_dat(self, dat_file:str) -> Iterable:
         '''
-        data = {}
-        for record in BioHandler.parse_gbk(local_gpff):
+        attributes:
+            annotations is dict type
+            features: attributes are id, qualifiers, location  
+            dbxrefs is list type
+            id is str
+            seq is Sequence object
+            other attr: count, description, name, reverse_complement, translate
+        '''
+        if dat_file.endswith('gz'):
+            with gzip.open(dat_file, 'rt') as f:
+                for record in SeqIO.parse(f, 'swiss'):
+                    yield record
+        else:
+            with open(dat_file, 'r') as f:
+                for record in SeqIO.parse(f, 'swiss'):
+                    yield record
+
+    def parse_epitope(self, parser:Iterable):
+        '''
+        retrieve records according to keywords defined in features
+        args: parser is determined by self.parse_dat()
+        '''
+        print("Try to detect epitopes...")
+        data, m, n = {}, 0, 0
+        for record in parser:
             for ft in record.features:
-                if ft.key == 'Region':
-                    feature = BioDict.gbk_feature(record, ft)
-                    if 'epitope' in feature.get('qualifiers', {}).get('note', ''):
-                        acc = record.locus
-                        if acc not in data:
-                            data[acc] = {
-                                'source': BioDict.gbk_source(record),
-                                'epitopes': [],
-                            }
-                        data[acc]['epitopes'].append(feature)
-                        print(feature)
+                note = ft.qualifiers.get('note', '')
+                if 'epitope' in note:
+                    if record.id not in data:
+                        data[record.id] = {
+                            'accession': record.id,
+                            'source': BioDict.swiss_source(record),
+                            'epitopes': [],
+                        }
+                        m += 1
+                    n += 1
+                    # update epitope to data
+                    epitope = BioDict.swiss_feature(record, ft)
+                    data[record.id]['epitopes'].append(epitope)
+                    print(json.dumps(data[record.id], indent=4))
+        print(f"proteins={m},epitopes={n}")
         return data
 
-    def integrate_epitope(self, entity_data:dict):
+    def integrate_epitope(self, integrate_obj:IntegrateData, entity_data:dict):
         '''
-        integrate entity_data into json data in entity_path
+        integrate eiptope data into json data
         '''
         count = {
             'epitopes': 0,
             'epitope_proteins': len(entity_data),
             'updated_proteins': 0,
             'updated_epitopes': 0,
             'new_epitopes': 0,
             'new_proteins': 0,
         }
         # check if data exists in json
-        for json_data in self.integrate.scan():
+        for json_data in integrate_obj.scan():
             acc = json_data.get('key')
             if  acc in entity_data:
                 if 'epitopes' not in json_data:
                     json_data['epitopes'] = {}
                 json_data['epitopes'][self.source] = entity_data[acc]['epitopes']
                 json_data[self.source] = entity_data[acc]['source']
                 # print(json.dumps(json_data, indent=4))
-                self.integrate.save_data(json_data, (self.source, 'epitope'))
+                integrate_obj.save_data(json_data, (self.source, 'epitope'))
                 count['updated_epitopes'] += len(entity_data[acc]['epitopes'])
                 count['updated_proteins'] += 1
                 del entity_data[acc]
         # export new data
         for acc, data in entity_data.items():
             input = {
                 self.source: data['source'],
                 'epitopes': {
                     self.source: data['epitopes']
                 },
             }
-            self.integrate.add_data(input, acc, (self.source, 'epitope'))
+            integrate_obj.add_data(input, acc, (self.source, 'epitope'))
             count['new_epitopes'] += len(data['epitopes'])
             count['new_proteins'] += 1
         count['epitopes'] = count['updated_epitopes'] + count['new_epitopes']
-        return count
-
-    def parse_uniprotkb(self, by_uniprotkb:bool=None):
-        '''
-        gene_refseq_uniprotkb_collab.gz
-        index by refseq or unirpotkb accession
-        '''
-        by_uniprotkb = True if by_uniprotkb else False
-        gz_file = NCBI(self.local_path).download_refseq_uniprotkb()
-        df = pd.read_csv(gz_file, compression='gzip', sep='\t', header=0)
-
-        data = {}        
-        index_key = 'UniProtKB_protein_accession' if by_uniprotkb \
-            else '#NCBI_protein_accession'
-        groups = df.groupby(index_key)
-        for name, group in groups:
-            data[name] = group.to_dict(orient="records")
-            # if group.shape[0]>1:
-            #     print(name, json.dumps(data[name], indent=4))
-        return data
-
+        return count
```

### Comparing `bioomics-0.2.6/src/bioomics/protein/expasy.py` & `bioomics-0.2.8/src/bioomics/protein/expasy.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.6/src/bioomics/protein/uniprot_sprot.py` & `bioomics-0.2.8/src/bioomics/protein/uniprot_sprot.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.6/src/bioomics/protein/uniprot_trembl.py` & `bioomics-0.2.8/src/bioomics/protein/uniprot_trembl.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.6/src/bioomics/rnacentral.py` & `bioomics-0.2.8/src/bioomics/rnacentral.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.6/src/bioomics.egg-info/PKG-INFO` & `bioomics-0.2.8/src/bioomics.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioomics
-Version: 0.2.6
+Version: 0.2.8
 Summary: Download, retrieve and process omics data for further bioinformatics
 Home-page: https://github.com/Tiezhengyuan/bio_omics
 Author: Tiezheng Yuan
 Author-email: tiezhengyuan@hotmail.com
 Keywords: pypi,cicd,python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `bioomics-0.2.6/src/bioomics.egg-info/SOURCES.txt` & `bioomics-0.2.8/src/bioomics.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 README.md
 setup.py
 src/bioomics/__init__.py
 src/bioomics/bio_dict.py
 src/bioomics/bio_handler.py
 src/bioomics/integrate_data.py
 src/bioomics/mirbase.py
+src/bioomics/multi_threads.py
 src/bioomics/rnacentral.py
 src/bioomics.egg-info/PKG-INFO
 src/bioomics.egg-info/SOURCES.txt
 src/bioomics.egg-info/dependency_links.txt
 src/bioomics.egg-info/requires.txt
 src/bioomics.egg-info/top_level.txt
 src/bioomics/connector/__init__.py
@@ -19,33 +20,38 @@
 src/bioomics/connector/conn_redis.py
 src/bioomics/constants/IEDB.py
 src/bioomics/immune/__init__.py
 src/bioomics/immune/iedb.py
 src/bioomics/immune/iedb_antigen.py
 src/bioomics/immune/iedb_epitope.py
 src/bioomics/ncbi/__init__.py
+src/bioomics/ncbi/genBank.py
+src/bioomics/ncbi/integrate_id.py
 src/bioomics/ncbi/ncbi.py
+src/bioomics/ncbi/parse_id.py
 src/bioomics/ncbi/refseq.py
-src/bioomics/ncbi/retrieve_ncbi.py
 src/bioomics/protein/__init__.py
 src/bioomics/protein/expasy.py
 src/bioomics/protein/uniprot.py
 src/bioomics/protein/uniprot_sprot.py
 src/bioomics/protein/uniprot_trembl.py
 src/pipelines/__init__.py
 src/pipelines/app.py
 src/pipelines/retrieve_epitopes.py
 tests/test_conn_ftp.py
 tests/test_conn_ftplib.py
 tests/test_conn_http.py
 tests/test_conn_redis.py
 tests/test_expasy.py
+tests/test_genbank.py
 tests/test_iedb.py
 tests/test_iedb_antigen.py
 tests/test_iedb_epitope.py
+tests/test_integrate_id.py
 tests/test_mirbase.py
 tests/test_ncbi.py
+tests/test_parse_id.py
 tests/test_refseq.py
 tests/test_rnacentral.py
 tests/test_uniprot.py
 tests/test_uniprot_sprot.py
 tests/test_uniprot_trembl.py
```

### Comparing `bioomics-0.2.6/src/pipelines/retrieve_epitopes.py` & `bioomics-0.2.8/src/pipelines/retrieve_epitopes.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.6/tests/test_conn_ftp.py` & `bioomics-0.2.8/tests/test_conn_ftp.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.6/tests/test_conn_ftplib.py` & `bioomics-0.2.8/tests/test_conn_ftplib.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.6/tests/test_conn_http.py` & `bioomics-0.2.8/tests/test_conn_http.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.6/tests/test_conn_redis.py` & `bioomics-0.2.8/tests/test_conn_redis.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.6/tests/test_iedb.py` & `bioomics-0.2.8/tests/test_iedb.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.6/tests/test_mirbase.py` & `bioomics-0.2.8/tests/test_mirbase.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.6/tests/test_ncbi.py` & `bioomics-0.2.8/tests/test_ncbi.py`

 * *Files 13% similar despite different names*

```diff
@@ -34,18 +34,25 @@
         local_file = NCBI(DIR_DATA).download_refseq_uniprotkb()
         expect = os.path.join(DIR_DATA, 'NCBI', 'refseq', 'gene_refseq_uniprotkb_collab.gz')
         assert local_file == expect
 
     @skip
     def test_download_refseq_gpff(self):
         local_files = NCBI(DIR_DATA).download_refseq_gpff()
-        print(local_files)
 
+    @skip
     def test_download_refseq_complete_gpff(self):
         local_files = NCBI(DIR_DATA).download_refseq_complete_gpff()
+        
+    @skip
+    def test_download_protein_fasta(self):
+        local_files = NCBI(DIR_DATA).download_protein_fasta()
+
+    def test_download_id_mapping(self):
+        local_files = NCBI(DIR_DATA).download_id_mapping()
         print(local_files)
 
 
     @skip
     def test_download_gene_data(self):
         local_files = NCBI(DIR_DATA).download_gene_data()
         print(local_files)
```

### Comparing `bioomics-0.2.6/tests/test_refseq.py` & `bioomics-0.2.8/tests/test_uniprot_trembl.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 '''
-Test class ConnectNCBI
+Test class 
 '''
-from tests.helper import *
-from src.bioomics import Refseq
+from .helper import *
+from src.bioomics import UniProtTrembl
+
 
 @ddt
-class TestRefseq(TestCase):
+class TestUniProtTrembl(TestCase):
+
+    def setUp(self):
+        self.c = UniProtTrembl(DIR_DATA, False)
 
-    @skip
-    @data(
-        [False, "AP_000001.1"],
-        [True, "A0A0D3MVN2"],
-    )
-    @unpack
-    def test_parse_uniprotkb(self, by_uniprotkb, expect):
-        res = Refseq(DIR_DATA).parse_uniprotkb(by_uniprotkb)
-        assert expect in res
-    
     @skip
     def test_parse_epitope(self):
-        infile = '/home/yuan/bio/bio_omics/tests/data/NCBI/refseq/mRNA_Prot/human.10.protein.gpff.gz'
-        Refseq(DIR_DATA).parse_epitope(infile)
+        dat_gz = self.c.download_dat()
+        assert dat_gz == os.path.join(DIR_DATA, 'UniProt', 'uniprot_trembl.dat.gz')
 
+        parser = self.c.parse_dat(dat_gz)
+        assert parser
 
-    def test_process_epitope(self):
+        entity_data = self.c.parse_epitope(parser)
+        assert len(entity_data) > 0
+        
+    def test_process_epitopes(self):
         entity_path = os.path.join(DIR_DATA, 'epitope')
-        Refseq(DIR_DATA).process_epitope(entity_path)
+        self.c.process_epitopes(entity_path)
+
```

### Comparing `bioomics-0.2.6/tests/test_rnacentral.py` & `bioomics-0.2.8/tests/test_rnacentral.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.6/tests/test_uniprot.py` & `bioomics-0.2.8/tests/test_uniprot.py`

 * *Files identical despite different names*

### Comparing `bioomics-0.2.6/tests/test_uniprot_sprot.py` & `bioomics-0.2.8/tests/test_uniprot_sprot.py`

 * *Files identical despite different names*

