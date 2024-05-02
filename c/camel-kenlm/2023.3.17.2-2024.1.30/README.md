# Comparing `tmp/camel-kenlm-2023.3.17.2.tar.gz` & `tmp/camel-kenlm-2024.1.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "camel-kenlm-2023.3.17.2.tar", last modified: Fri Mar 17 11:38:54 2023, max compression
+gzip compressed data, was "camel-kenlm-2024.1.30.tar", last modified: Thu May  2 13:54:48 2024, max compression
```

## Comparing `camel-kenlm-2023.3.17.2.tar` & `camel-kenlm-2024.1.30.tar`

### file list

```diff
@@ -1,328 +1,328 @@
-drwxr-xr-x   0 oo11       (501) staff       (20)        0 2023-03-17 11:38:54.878406 camel-kenlm-2023.3.17.2/
-drwxr-xr-x   0 oo11       (501) staff       (20)        0 2023-03-17 11:38:53.823855 camel-kenlm-2023.3.17.2/.github/
-drwxr-xr-x   0 oo11       (501) staff       (20)        0 2023-03-17 11:38:53.929985 camel-kenlm-2023.3.17.2/.github/workflows/
--rw-r--r--   0 oo11       (501) staff       (20)      542 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/.github/workflows/mac.yml
--rw-r--r--   0 oo11       (501) staff       (20)      619 2023-03-04 11:18:36.000000 camel-kenlm-2023.3.17.2/.github/workflows/ubuntu.yml
--rw-r--r--   0 oo11       (501) staff       (20)      471 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/.github/workflows/windows.yml
--rw-r--r--   0 oo11       (501) staff       (20)      276 2023-03-17 09:29:18.000000 camel-kenlm-2023.3.17.2/.gitignore
--rw-r--r--   0 oo11       (501) staff       (20)      696 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/BUILDING
--rw-r--r--   0 oo11       (501) staff       (20)     4792 2023-03-04 11:18:36.000000 camel-kenlm-2023.3.17.2/CMakeLists.txt
--rw-r--r--   0 oo11       (501) staff       (20)    26530 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/COPYING
--rw-r--r--   0 oo11       (501) staff       (20)    35147 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/COPYING.3
--rw-r--r--   0 oo11       (501) staff       (20)     7637 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/COPYING.LESSER.3
--rw-r--r--   0 oo11       (501) staff       (20)    63537 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/Doxyfile
--rw-r--r--   0 oo11       (501) staff       (20)     1150 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/LICENSE
--rw-r--r--   0 oo11       (501) staff       (20)      220 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/MANIFEST.in
--rw-r--r--   0 oo11       (501) staff       (20)      212 2023-03-17 11:38:54.878026 camel-kenlm-2023.3.17.2/PKG-INFO
--rw-r--r--   0 oo11       (501) staff       (20)     6359 2023-03-17 09:22:54.000000 camel-kenlm-2023.3.17.2/README.md
-drwxr-xr-x   0 oo11       (501) staff       (20)        0 2023-03-17 11:38:53.937381 camel-kenlm-2023.3.17.2/camel_kenlm.egg-info/
--rw-r--r--   0 oo11       (501) staff       (20)      212 2023-03-17 11:38:53.000000 camel-kenlm-2023.3.17.2/camel_kenlm.egg-info/PKG-INFO
--rw-r--r--   0 oo11       (501) staff       (20)     7780 2023-03-17 11:38:53.000000 camel-kenlm-2023.3.17.2/camel_kenlm.egg-info/SOURCES.txt
--rw-r--r--   0 oo11       (501) staff       (20)        1 2023-03-17 11:38:53.000000 camel-kenlm-2023.3.17.2/camel_kenlm.egg-info/dependency_links.txt
--rw-r--r--   0 oo11       (501) staff       (20)        6 2023-03-17 11:38:53.000000 camel-kenlm-2023.3.17.2/camel_kenlm.egg-info/top_level.txt
--rwxr-xr-x   0 oo11       (501) staff       (20)       81 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/clean_query_only.sh
-drwxr-xr-x   0 oo11       (501) staff       (20)        0 2023-03-17 11:38:53.940353 camel-kenlm-2023.3.17.2/cmake/
--rw-r--r--   0 oo11       (501) staff       (20)     2821 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/cmake/KenLMFunctions.cmake
--rw-r--r--   0 oo11       (501) staff       (20)      334 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/cmake/kenlmConfig.cmake.in
-drwxr-xr-x   0 oo11       (501) staff       (20)        0 2023-03-17 11:38:53.942514 camel-kenlm-2023.3.17.2/cmake/modules/
--rw-r--r--   0 oo11       (501) staff       (20)     3185 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/cmake/modules/FindEigen3.cmake
--rwxr-xr-x   0 oo11       (501) staff       (20)     1154 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/compile_query_only.sh
-drwxr-xr-x   0 oo11       (501) staff       (20)        0 2023-03-17 11:38:54.099551 camel-kenlm-2023.3.17.2/lm/
--rw-r--r--   0 oo11       (501) staff       (20)     2097 2023-03-04 11:18:36.000000 camel-kenlm-2023.3.17.2/lm/CMakeLists.txt
--rw-r--r--   0 oo11       (501) staff       (20)     3710 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/bhiksha.cc
--rw-r--r--   0 oo11       (501) staff       (20)     4348 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/bhiksha.hh
--rw-r--r--   0 oo11       (501) staff       (20)    12931 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/binary_format.cc
--rw-r--r--   0 oo11       (501) staff       (20)     3498 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/binary_format.hh
--rw-r--r--   0 oo11       (501) staff       (20)     1379 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/blank.hh
--rw-r--r--   0 oo11       (501) staff       (20)     8154 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/build_binary_main.cc
-drwxr-xr-x   0 oo11       (501) staff       (20)        0 2023-03-17 11:38:54.225167 camel-kenlm-2023.3.17.2/lm/builder/
--rw-r--r--   0 oo11       (501) staff       (20)     1897 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/builder/CMakeLists.txt
--rw-r--r--   0 oo11       (501) staff       (20)      826 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/builder/README.md
--rw-r--r--   0 oo11       (501) staff       (20)      152 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/builder/TODO
--rw-r--r--   0 oo11       (501) staff       (20)    12607 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/builder/adjust_counts.cc
--rw-r--r--   0 oo11       (501) staff       (20)     2258 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/builder/adjust_counts.hh
--rw-r--r--   0 oo11       (501) staff       (20)     3509 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/builder/adjust_counts_test.cc
--rw-r--r--   0 oo11       (501) staff       (20)      899 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/builder/combine_counts.hh
--rw-r--r--   0 oo11       (501) staff       (20)     9550 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/builder/corpus_count.cc
--rw-r--r--   0 oo11       (501) staff       (20)     1701 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/builder/corpus_count.hh
--rw-r--r--   0 oo11       (501) staff       (20)     2820 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/builder/corpus_count_test.cc
--rw-r--r--   0 oo11       (501) staff       (20)     3992 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/builder/count_ngrams_main.cc
--rw-r--r--   0 oo11       (501) staff       (20)     2411 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/builder/debug_print.hh
--rw-r--r--   0 oo11       (501) staff       (20)      439 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/builder/discount.hh
--rw-r--r--   0 oo11       (501) staff       (20)     1869 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/builder/dump_counts_main.cc
--rw-r--r--   0 oo11       (501) staff       (20)      293 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/builder/hash_gamma.hh
--rw-r--r--   0 oo11       (501) staff       (20)      715 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/builder/header_info.hh
--rw-r--r--   0 oo11       (501) staff       (20)    10698 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/builder/initial_probabilities.cc
--rw-r--r--   0 oo11       (501) staff       (20)     1452 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/builder/initial_probabilities.hh
--rw-r--r--   0 oo11       (501) staff       (20)     6044 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/builder/interpolate.cc
--rw-r--r--   0 oo11       (501) staff       (20)     1136 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/builder/interpolate.hh
--rw-r--r--   0 oo11       (501) staff       (20)    11967 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/builder/lmplz_main.cc
--rw-r--r--   0 oo11       (501) staff       (20)     1625 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/builder/output.cc
--rw-r--r--   0 oo11       (501) staff       (20)     2529 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/builder/output.hh
--rw-r--r--   0 oo11       (501) staff       (20)     1051 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/builder/payload.hh
--rw-r--r--   0 oo11       (501) staff       (20)    17887 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/builder/pipeline.cc
--rw-r--r--   0 oo11       (501) staff       (20)     2572 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/builder/pipeline.hh
-drwxr-xr-x   0 oo11       (501) staff       (20)        0 2023-03-17 11:38:54.267702 camel-kenlm-2023.3.17.2/lm/common/
--rw-r--r--   0 oo11       (501) staff       (20)      889 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/common/CMakeLists.txt
--rw-r--r--   0 oo11       (501) staff       (20)     6078 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/common/compare.hh
--rw-r--r--   0 oo11       (501) staff       (20)     2366 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/common/joint_order.hh
--rw-r--r--   0 oo11       (501) staff       (20)     5186 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/common/model_buffer.cc
--rw-r--r--   0 oo11       (501) staff       (20)     2155 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/common/model_buffer.hh
--rw-r--r--   0 oo11       (501) staff       (20)     1713 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/common/model_buffer_test.cc
--rw-r--r--   0 oo11       (501) staff       (20)     2112 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/common/ngram.hh
--rw-r--r--   0 oo11       (501) staff       (20)     1872 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/common/ngram_stream.hh
--rw-r--r--   0 oo11       (501) staff       (20)     1890 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/common/print.cc
--rw-r--r--   0 oo11       (501) staff       (20)     1483 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/common/print.hh
--rw-r--r--   0 oo11       (501) staff       (20)      398 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/common/renumber.cc
--rw-r--r--   0 oo11       (501) staff       (20)      755 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/common/renumber.hh
--rw-r--r--   0 oo11       (501) staff       (20)      562 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/common/size_option.cc
--rw-r--r--   0 oo11       (501) staff       (20)      302 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/common/size_option.hh
--rw-r--r--   0 oo11       (501) staff       (20)      550 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/common/special.hh
-drwxr-xr-x   0 oo11       (501) staff       (20)        0 2023-03-17 11:38:54.278465 camel-kenlm-2023.3.17.2/lm/common/test_data/
-drwxr-xr-x   0 oo11       (501) staff       (20)        0 2023-03-17 11:38:54.303030 camel-kenlm-2023.3.17.2/lm/common/test_data/bigendian/
--rw-r--r--   0 oo11       (501) staff       (20)       60 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/common/test_data/bigendian/toy0.1
--rw-r--r--   0 oo11       (501) staff       (20)      112 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/common/test_data/bigendian/toy0.2
--rw-r--r--   0 oo11       (501) staff       (20)      140 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/common/test_data/bigendian/toy0.3
--rw-r--r--   0 oo11       (501) staff       (20)       55 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/common/test_data/bigendian/toy0.kenlm_intermediate
--rw-r--r--   0 oo11       (501) staff       (20)       19 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/common/test_data/bigendian/toy0.vocab
--rw-r--r--   0 oo11       (501) staff       (20)       72 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/common/test_data/bigendian/toy1.1
--rw-r--r--   0 oo11       (501) staff       (20)      112 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/common/test_data/bigendian/toy1.2
--rw-r--r--   0 oo11       (501) staff       (20)      120 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/common/test_data/bigendian/toy1.3
--rw-r--r--   0 oo11       (501) staff       (20)       55 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/common/test_data/bigendian/toy1.kenlm_intermediate
--rw-r--r--   0 oo11       (501) staff       (20)       21 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/common/test_data/bigendian/toy1.vocab
--rwxr-xr-x   0 oo11       (501) staff       (20)      270 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/common/test_data/generate.sh
-drwxr-xr-x   0 oo11       (501) staff       (20)        0 2023-03-17 11:38:54.317427 camel-kenlm-2023.3.17.2/lm/common/test_data/littleendian/
--rw-r--r--   0 oo11       (501) staff       (20)       60 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/common/test_data/littleendian/toy0.1
--rw-r--r--   0 oo11       (501) staff       (20)      112 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/common/test_data/littleendian/toy0.2
--rw-r--r--   0 oo11       (501) staff       (20)      140 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/common/test_data/littleendian/toy0.3
--rw-r--r--   0 oo11       (501) staff       (20)       55 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/common/test_data/littleendian/toy0.kenlm_intermediate
--rw-r--r--   0 oo11       (501) staff       (20)       19 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/common/test_data/littleendian/toy0.vocab
--rw-r--r--   0 oo11       (501) staff       (20)       72 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/common/test_data/littleendian/toy1.1
--rw-r--r--   0 oo11       (501) staff       (20)      112 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/common/test_data/littleendian/toy1.2
--rw-r--r--   0 oo11       (501) staff       (20)      120 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/common/test_data/littleendian/toy1.3
--rw-r--r--   0 oo11       (501) staff       (20)       55 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/common/test_data/littleendian/toy1.kenlm_intermediate
--rw-r--r--   0 oo11       (501) staff       (20)       21 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/common/test_data/littleendian/toy1.vocab
--rw-r--r--   0 oo11       (501) staff       (20)      475 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/common/test_data/toy0.arpa
--rw-r--r--   0 oo11       (501) staff       (20)      470 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/common/test_data/toy1.arpa
--rw-r--r--   0 oo11       (501) staff       (20)      675 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/config.cc
--rw-r--r--   0 oo11       (501) staff       (20)     3913 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/config.hh
--rw-r--r--   0 oo11       (501) staff       (20)      722 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/enumerate_vocab.hh
--rw-r--r--   0 oo11       (501) staff       (20)     2544 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/facade.hh
-drwxr-xr-x   0 oo11       (501) staff       (20)        0 2023-03-17 11:38:54.339543 camel-kenlm-2023.3.17.2/lm/filter/
--rw-r--r--   0 oo11       (501) staff       (20)     1327 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/filter/CMakeLists.txt
--rw-r--r--   0 oo11       (501) staff       (20)     1935 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/filter/arpa_io.cc
--rw-r--r--   0 oo11       (501) staff       (20)     2816 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/filter/arpa_io.hh
--rw-r--r--   0 oo11       (501) staff       (20)     2458 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/filter/count_io.hh
--rw-r--r--   0 oo11       (501) staff       (20)     9352 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/filter/filter_main.cc
--rw-r--r--   0 oo11       (501) staff       (20)     7379 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/filter/format.hh
--rw-r--r--   0 oo11       (501) staff       (20)     8212 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/filter/phrase.cc
--rw-r--r--   0 oo11       (501) staff       (20)     5778 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/filter/phrase.hh
--rw-r--r--   0 oo11       (501) staff       (20)     5027 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/filter/phrase_table_vocab_main.cc
--rw-r--r--   0 oo11       (501) staff       (20)     4205 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/filter/thread.hh
--rw-r--r--   0 oo11       (501) staff       (20)     1209 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/filter/vocab.cc
--rw-r--r--   0 oo11       (501) staff       (20)     4123 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/filter/vocab.hh
--rw-r--r--   0 oo11       (501) staff       (20)     1797 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/filter/wrapper.hh
--rw-r--r--   0 oo11       (501) staff       (20)     1068 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/fragment_main.cc
-drwxr-xr-x   0 oo11       (501) staff       (20)        0 2023-03-17 11:38:54.404091 camel-kenlm-2023.3.17.2/lm/interpolate/
--rw-r--r--   0 oo11       (501) staff       (20)     1774 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/interpolate/CMakeLists.txt
--rw-r--r--   0 oo11       (501) staff       (20)      737 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/interpolate/backoff_matrix.hh
--rw-r--r--   0 oo11       (501) staff       (20)     1952 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/interpolate/backoff_reunification.cc
--rw-r--r--   0 oo11       (501) staff       (20)      913 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/interpolate/backoff_reunification.hh
--rw-r--r--   0 oo11       (501) staff       (20)     4904 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/interpolate/backoff_reunification_test.cc
--rw-r--r--   0 oo11       (501) staff       (20)     1086 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/interpolate/bounded_sequence_encoding.cc
--rw-r--r--   0 oo11       (501) staff       (20)     2530 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/interpolate/bounded_sequence_encoding.hh
--rw-r--r--   0 oo11       (501) staff       (20)     3222 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/interpolate/bounded_sequence_encoding_test.cc
--rw-r--r--   0 oo11       (501) staff       (20)      693 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/interpolate/interpolate_info.hh
--rw-r--r--   0 oo11       (501) staff       (20)     5296 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/interpolate/interpolate_main.cc
--rw-r--r--   0 oo11       (501) staff       (20)    10010 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/interpolate/merge_probabilities.cc
--rw-r--r--   0 oo11       (501) staff       (20)     3385 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/interpolate/merge_probabilities.hh
--rw-r--r--   0 oo11       (501) staff       (20)     3586 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/interpolate/merge_vocab.cc
--rw-r--r--   0 oo11       (501) staff       (20)      572 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/interpolate/merge_vocab.hh
--rw-r--r--   0 oo11       (501) staff       (20)     5306 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/interpolate/merge_vocab_test.cc
--rw-r--r--   0 oo11       (501) staff       (20)    13813 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/interpolate/normalize.cc
--rw-r--r--   0 oo11       (501) staff       (20)     1101 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/interpolate/normalize.hh
--rw-r--r--   0 oo11       (501) staff       (20)     2758 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/interpolate/normalize_test.cc
--rw-r--r--   0 oo11       (501) staff       (20)     7645 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/interpolate/pipeline.cc
--rw-r--r--   0 oo11       (501) staff       (20)      552 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/interpolate/pipeline.hh
--rw-r--r--   0 oo11       (501) staff       (20)     1235 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/interpolate/split_worker.cc
--rw-r--r--   0 oo11       (501) staff       (20)     1100 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/interpolate/split_worker.hh
--rw-r--r--   0 oo11       (501) staff       (20)     7430 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/interpolate/streaming_example_main.cc
--rw-r--r--   0 oo11       (501) staff       (20)     5950 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/interpolate/tune_derivatives.cc
--rw-r--r--   0 oo11       (501) staff       (20)      590 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/interpolate/tune_derivatives.hh
--rw-r--r--   0 oo11       (501) staff       (20)     3969 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/interpolate/tune_derivatives_test.cc
--rw-r--r--   0 oo11       (501) staff       (20)    19605 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/interpolate/tune_instances.cc
--rw-r--r--   0 oo11       (501) staff       (20)     2956 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/interpolate/tune_instances.hh
--rw-r--r--   0 oo11       (501) staff       (20)     4571 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/interpolate/tune_instances_test.cc
--rw-r--r--   0 oo11       (501) staff       (20)      512 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/interpolate/tune_matrix.hh
--rw-r--r--   0 oo11       (501) staff       (20)     1366 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/interpolate/tune_weights.cc
--rw-r--r--   0 oo11       (501) staff       (20)      446 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/interpolate/tune_weights.hh
--rw-r--r--   0 oo11       (501) staff       (20)      342 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/interpolate/universal_vocab.cc
--rw-r--r--   0 oo11       (501) staff       (20)     1347 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/interpolate/universal_vocab.hh
--rw-r--r--   0 oo11       (501) staff       (20)     9039 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/kenlm_benchmark_main.cc
--rw-r--r--   0 oo11       (501) staff       (20)     7174 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/left.hh
--rw-r--r--   0 oo11       (501) staff       (20)    12402 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/left_test.cc
--rw-r--r--   0 oo11       (501) staff       (20)      637 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/lm_exception.cc
--rw-r--r--   0 oo11       (501) staff       (20)     1057 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/lm_exception.hh
--rw-r--r--   0 oo11       (501) staff       (20)      644 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/max_order.hh
--rw-r--r--   0 oo11       (501) staff       (20)    16256 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/model.cc
--rw-r--r--   0 oo11       (501) staff       (20)     7051 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/model.hh
--rw-r--r--   0 oo11       (501) staff       (20)    14544 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/model_test.cc
--rw-r--r--   0 oo11       (501) staff       (20)      798 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/model_type.hh
--rw-r--r--   0 oo11       (501) staff       (20)     3534 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/ngram_query.hh
--rw-r--r--   0 oo11       (501) staff       (20)     6003 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/partial.hh
--rw-r--r--   0 oo11       (501) staff       (20)     6672 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/partial_test.cc
--rw-r--r--   0 oo11       (501) staff       (20)     3743 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/quantize.cc
--rw-r--r--   0 oo11       (501) staff       (20)     7749 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/quantize.hh
--rw-r--r--   0 oo11       (501) staff       (20)     4675 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/query_main.cc
--rw-r--r--   0 oo11       (501) staff       (20)     7543 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/read_arpa.cc
--rw-r--r--   0 oo11       (501) staff       (20)     3016 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/read_arpa.hh
--rw-r--r--   0 oo11       (501) staff       (20)     1248 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/return.hh
--rw-r--r--   0 oo11       (501) staff       (20)    12060 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/search_hashed.cc
--rw-r--r--   0 oo11       (501) staff       (20)     5935 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/search_hashed.hh
--rw-r--r--   0 oo11       (501) staff       (20)    23394 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/search_trie.cc
--rw-r--r--   0 oo11       (501) staff       (20)     4906 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/search_trie.hh
--rw-r--r--   0 oo11       (501) staff       (20)     2594 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/sizes.cc
--rw-r--r--   0 oo11       (501) staff       (20)      374 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/sizes.hh
--rw-r--r--   0 oo11       (501) staff       (20)     3440 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/state.hh
--rw-r--r--   0 oo11       (501) staff       (20)     2780 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/test.arpa
--rw-r--r--   0 oo11       (501) staff       (20)     2694 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/test_nounk.arpa
--rw-r--r--   0 oo11       (501) staff       (20)     5639 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/trie.cc
--rw-r--r--   0 oo11       (501) staff       (20)     3563 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/trie.hh
--rw-r--r--   0 oo11       (501) staff       (20)    10982 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/trie_sort.cc
--rw-r--r--   0 oo11       (501) staff       (20)     2795 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/trie_sort.hh
--rw-r--r--   0 oo11       (501) staff       (20)     3935 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/value.hh
--rw-r--r--   0 oo11       (501) staff       (20)     2045 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/value_build.cc
--rw-r--r--   0 oo11       (501) staff       (20)     2568 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/value_build.hh
--rw-r--r--   0 oo11       (501) staff       (20)      380 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/virtual_interface.cc
--rw-r--r--   0 oo11       (501) staff       (20)     5668 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/virtual_interface.hh
--rw-r--r--   0 oo11       (501) staff       (20)    11083 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/vocab.cc
--rw-r--r--   0 oo11       (501) staff       (20)     8680 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/vocab.hh
--rw-r--r--   0 oo11       (501) staff       (20)      358 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/weights.hh
--rw-r--r--   0 oo11       (501) staff       (20)      293 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/word_index.hh
-drwxr-xr-x   0 oo11       (501) staff       (20)        0 2023-03-17 11:38:54.411416 camel-kenlm-2023.3.17.2/lm/wrappers/
--rw-r--r--   0 oo11       (501) staff       (20)      176 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/wrappers/README
--rw-r--r--   0 oo11       (501) staff       (20)     4261 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/wrappers/nplm.cc
--rw-r--r--   0 oo11       (501) staff       (20)     1975 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/lm/wrappers/nplm.hh
--rw-r--r--   0 oo11       (501) staff       (20)       59 2023-03-04 11:18:36.000000 camel-kenlm-2023.3.17.2/pyproject.toml
-drwxr-xr-x   0 oo11       (501) staff       (20)        0 2023-03-17 11:38:54.530851 camel-kenlm-2023.3.17.2/python/
--rw-r--r--   0 oo11       (501) staff       (20)      988 2023-03-04 11:18:36.000000 camel-kenlm-2023.3.17.2/python/CMakeLists.txt
--rw-r--r--   0 oo11       (501) staff       (20)     1957 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/python/_kenlm.pxd
--rwxr-xr-x   0 oo11       (501) staff       (20)     1427 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/python/example.py
--rw-r--r--   0 oo11       (501) staff       (20)   449861 2023-03-04 11:18:36.000000 camel-kenlm-2023.3.17.2/python/kenlm.cpp
--rw-r--r--   0 oo11       (501) staff       (20)     9323 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/python/kenlm.pyx
--rw-r--r--   0 oo11       (501) staff       (20)      906 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/python/score_sentence.cc
--rw-r--r--   0 oo11       (501) staff       (20)      325 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/python/score_sentence.hh
--rw-r--r--   0 oo11       (501) staff       (20)       38 2023-03-17 11:38:54.878636 camel-kenlm-2023.3.17.2/setup.cfg
--rw-r--r--   0 oo11       (501) staff       (20)     4420 2023-03-17 11:38:14.000000 camel-kenlm-2023.3.17.2/setup.py
-drwxr-xr-x   0 oo11       (501) staff       (20)        0 2023-03-17 11:38:54.666165 camel-kenlm-2023.3.17.2/util/
--rw-r--r--   0 oo11       (501) staff       (20)     3873 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/CMakeLists.txt
--rw-r--r--   0 oo11       (501) staff       (20)     1176 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/bit_packing.cc
--rw-r--r--   0 oo11       (501) staff       (20)     5967 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/bit_packing.hh
--rw-r--r--   0 oo11       (501) staff       (20)     1490 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/bit_packing_test.cc
--rw-r--r--   0 oo11       (501) staff       (20)     1227 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/cat_compressed_main.cc
-drwxr-xr-x   0 oo11       (501) staff       (20)        0 2023-03-17 11:38:54.829608 camel-kenlm-2023.3.17.2/util/double-conversion/
--rw-r--r--   0 oo11       (501) staff       (20)     1042 2023-03-04 11:18:36.000000 camel-kenlm-2023.3.17.2/util/double-conversion/CMakeLists.txt
--rw-r--r--   0 oo11       (501) staff       (20)     1527 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/double-conversion/LICENSE
--rw-r--r--   0 oo11       (501) staff       (20)    27617 2023-03-04 11:18:36.000000 camel-kenlm-2023.3.17.2/util/double-conversion/bignum-dtoa.cc
--rw-r--r--   0 oo11       (501) staff       (20)     4300 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/double-conversion/bignum-dtoa.h
--rw-r--r--   0 oo11       (501) staff       (20)    24726 2023-03-04 11:18:36.000000 camel-kenlm-2023.3.17.2/util/double-conversion/bignum.cc
--rw-r--r--   0 oo11       (501) staff       (20)     5891 2023-03-04 11:18:36.000000 camel-kenlm-2023.3.17.2/util/double-conversion/bignum.h
--rw-r--r--   0 oo11       (501) staff       (20)     9913 2023-03-04 11:18:36.000000 camel-kenlm-2023.3.17.2/util/double-conversion/cached-powers.cc
--rw-r--r--   0 oo11       (501) staff       (20)     3021 2023-03-04 11:18:36.000000 camel-kenlm-2023.3.17.2/util/double-conversion/cached-powers.h
--rw-r--r--   0 oo11       (501) staff       (20)     5030 2023-03-04 11:18:36.000000 camel-kenlm-2023.3.17.2/util/double-conversion/diy-fp.h
--rw-r--r--   0 oo11       (501) staff       (20)     1804 2023-03-04 11:18:36.000000 camel-kenlm-2023.3.17.2/util/double-conversion/double-conversion.h
--rw-r--r--   0 oo11       (501) staff       (20)    15851 2023-03-04 11:18:36.000000 camel-kenlm-2023.3.17.2/util/double-conversion/double-to-string.cc
--rw-r--r--   0 oo11       (501) staff       (20)    22349 2023-03-04 11:18:36.000000 camel-kenlm-2023.3.17.2/util/double-conversion/double-to-string.h
--rw-r--r--   0 oo11       (501) staff       (20)    31645 2023-03-04 11:18:36.000000 camel-kenlm-2023.3.17.2/util/double-conversion/fast-dtoa.cc
--rw-r--r--   0 oo11       (501) staff       (20)     4064 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/double-conversion/fast-dtoa.h
--rw-r--r--   0 oo11       (501) staff       (20)    15352 2023-03-04 11:18:36.000000 camel-kenlm-2023.3.17.2/util/double-conversion/fixed-dtoa.cc
--rw-r--r--   0 oo11       (501) staff       (20)     2770 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/double-conversion/fixed-dtoa.h
--rw-r--r--   0 oo11       (501) staff       (20)    15223 2023-03-04 11:18:36.000000 camel-kenlm-2023.3.17.2/util/double-conversion/ieee.h
--rw-r--r--   0 oo11       (501) staff       (20)    27857 2023-03-04 11:18:36.000000 camel-kenlm-2023.3.17.2/util/double-conversion/string-to-double.cc
--rw-r--r--   0 oo11       (501) staff       (20)    10848 2023-03-04 11:18:36.000000 camel-kenlm-2023.3.17.2/util/double-conversion/string-to-double.h
--rw-r--r--   0 oo11       (501) staff       (20)    23469 2023-03-04 11:18:36.000000 camel-kenlm-2023.3.17.2/util/double-conversion/strtod.cc
--rw-r--r--   0 oo11       (501) staff       (20)     3038 2023-03-04 11:18:36.000000 camel-kenlm-2023.3.17.2/util/double-conversion/strtod.h
--rw-r--r--   0 oo11       (501) staff       (20)    15340 2023-03-04 11:18:36.000000 camel-kenlm-2023.3.17.2/util/double-conversion/utils.h
--rw-r--r--   0 oo11       (501) staff       (20)     1367 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/ersatz_progress.cc
--rw-r--r--   0 oo11       (501) staff       (20)     1603 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/ersatz_progress.hh
--rw-r--r--   0 oo11       (501) staff       (20)     2765 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/exception.cc
--rw-r--r--   0 oo11       (501) staff       (20)     4392 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/exception.hh
--rw-r--r--   0 oo11       (501) staff       (20)     3994 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/fake_ostream.hh
--rw-r--r--   0 oo11       (501) staff       (20)    18350 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/file.cc
--rw-r--r--   0 oo11       (501) staff       (20)     4746 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/file.hh
--rw-r--r--   0 oo11       (501) staff       (20)    10877 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/file_piece.cc
--rw-r--r--   0 oo11       (501) staff       (20)     6515 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/file_piece.hh
--rw-r--r--   0 oo11       (501) staff       (20)     5364 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/file_piece_test.cc
--rw-r--r--   0 oo11       (501) staff       (20)     2424 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/file_stream.hh
--rw-r--r--   0 oo11       (501) staff       (20)     5545 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/fixed_array.hh
--rw-r--r--   0 oo11       (501) staff       (20)      729 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/float_to_string.cc
--rw-r--r--   0 oo11       (501) staff       (20)      609 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/float_to_string.hh
--rw-r--r--   0 oo11       (501) staff       (20)     1441 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/getopt.c
--rw-r--r--   0 oo11       (501) staff       (20)      472 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/getopt.hh
--rw-r--r--   0 oo11       (501) staff       (20)      270 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/have.hh
--rw-r--r--   0 oo11       (501) staff       (20)    22498 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/integer_to_string.cc
--rw-r--r--   0 oo11       (501) staff       (20)     1636 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/integer_to_string.hh
--rw-r--r--   0 oo11       (501) staff       (20)     1959 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/integer_to_string_test.cc
--rw-r--r--   0 oo11       (501) staff       (20)     4905 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/joint_sort.hh
--rw-r--r--   0 oo11       (501) staff       (20)     1738 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/joint_sort_test.cc
--rw-r--r--   0 oo11       (501) staff       (20)    13507 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/mmap.cc
--rw-r--r--   0 oo11       (501) staff       (20)     6780 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/mmap.hh
--rw-r--r--   0 oo11       (501) staff       (20)     3379 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/multi_intersection.hh
--rw-r--r--   0 oo11       (501) staff       (20)     1887 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/multi_intersection_test.cc
--rw-r--r--   0 oo11       (501) staff       (20)     4074 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/murmur_hash.cc
--rw-r--r--   0 oo11       (501) staff       (20)      616 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/murmur_hash.hh
--rw-r--r--   0 oo11       (501) staff       (20)     1546 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/parallel_read.cc
--rw-r--r--   0 oo11       (501) staff       (20)      461 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/parallel_read.hh
--rw-r--r--   0 oo11       (501) staff       (20)     3480 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/pcqueue.hh
--rw-r--r--   0 oo11       (501) staff       (20)      355 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/pcqueue_test.cc
--rw-r--r--   0 oo11       (501) staff       (20)      705 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/pool.cc
--rw-r--r--   0 oo11       (501) staff       (20)     2935 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/pool.hh
--rw-r--r--   0 oo11       (501) staff       (20)    13233 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/probing_hash_table.hh
--rw-r--r--   0 oo11       (501) staff       (20)    11788 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/probing_hash_table_benchmark_main.cc
--rw-r--r--   0 oo11       (501) staff       (20)     2269 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/probing_hash_table_test.cc
--rw-r--r--   0 oo11       (501) staff       (20)     3526 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/proxy_iterator.hh
--rw-r--r--   0 oo11       (501) staff       (20)    13086 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/read_compressed.cc
--rw-r--r--   0 oo11       (501) staff       (20)     2034 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/read_compressed.hh
--rw-r--r--   0 oo11       (501) staff       (20)     2669 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/read_compressed_test.cc
--rw-r--r--   0 oo11       (501) staff       (20)     1118 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/scoped.cc
--rw-r--r--   0 oo11       (501) staff       (20)     3660 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/scoped.hh
--rw-r--r--   0 oo11       (501) staff       (20)     6581 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/sized_iterator.hh
--rw-r--r--   0 oo11       (501) staff       (20)      559 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/sized_iterator_test.cc
--rw-r--r--   0 oo11       (501) staff       (20)     3257 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/sorted_uniform.hh
--rw-r--r--   0 oo11       (501) staff       (20)     3621 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/sorted_uniform_test.cc
--rw-r--r--   0 oo11       (501) staff       (20)      751 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/spaces.cc
--rw-r--r--   0 oo11       (501) staff       (20)      167 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/spaces.hh
-drwxr-xr-x   0 oo11       (501) staff       (20)        0 2023-03-17 11:38:54.876714 camel-kenlm-2023.3.17.2/util/stream/
--rw-r--r--   0 oo11       (501) staff       (20)     1237 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/stream/CMakeLists.txt
--rw-r--r--   0 oo11       (501) staff       (20)     2420 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/stream/block.hh
--rw-r--r--   0 oo11       (501) staff       (20)     4367 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/stream/chain.cc
--rw-r--r--   0 oo11       (501) staff       (20)     8996 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/stream/chain.hh
--rw-r--r--   0 oo11       (501) staff       (20)     1606 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/stream/config.hh
--rw-r--r--   0 oo11       (501) staff       (20)      278 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/stream/count_records.cc
--rw-r--r--   0 oo11       (501) staff       (20)      300 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/stream/count_records.hh
--rw-r--r--   0 oo11       (501) staff       (20)     2436 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/stream/io.cc
--rw-r--r--   0 oo11       (501) staff       (20)     1843 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/stream/io.hh
--rw-r--r--   0 oo11       (501) staff       (20)      823 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/stream/io_test.cc
--rw-r--r--   0 oo11       (501) staff       (20)     1418 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/stream/line_input.cc
--rw-r--r--   0 oo11       (501) staff       (20)      515 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/stream/line_input.hh
--rw-r--r--   0 oo11       (501) staff       (20)     2363 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/stream/multi_progress.cc
--rw-r--r--   0 oo11       (501) staff       (20)     1848 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/stream/multi_progress.hh
--rw-r--r--   0 oo11       (501) staff       (20)     3362 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/stream/multi_stream.hh
--rw-r--r--   0 oo11       (501) staff       (20)     3627 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/stream/rewindable_stream.cc
--rw-r--r--   0 oo11       (501) staff       (20)     3241 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/stream/rewindable_stream.hh
--rw-r--r--   0 oo11       (501) staff       (20)      899 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/stream/rewindable_stream_test.cc
--rw-r--r--   0 oo11       (501) staff       (20)    20450 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/stream/sort.hh
--rw-r--r--   0 oo11       (501) staff       (20)     1663 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/stream/sort_test.cc
--rw-r--r--   0 oo11       (501) staff       (20)     1821 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/stream/stream.hh
--rw-r--r--   0 oo11       (501) staff       (20)      759 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/stream/stream_test.cc
--rw-r--r--   0 oo11       (501) staff       (20)      732 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/stream/typed_stream.hh
--rw-r--r--   0 oo11       (501) staff       (20)     5480 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/string_piece.cc
--rw-r--r--   0 oo11       (501) staff       (20)     9185 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/string_piece.hh
--rw-r--r--   0 oo11       (501) staff       (20)     1478 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/string_piece_hash.hh
--rw-r--r--   0 oo11       (501) staff       (20)     1039 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/string_stream.hh
--rw-r--r--   0 oo11       (501) staff       (20)     1778 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/string_stream_test.cc
--rw-r--r--   0 oo11       (501) staff       (20)     3825 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/thread_pool.hh
--rw-r--r--   0 oo11       (501) staff       (20)     4890 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/tokenize_piece.hh
--rw-r--r--   0 oo11       (501) staff       (20)     1135 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/tokenize_piece_test.cc
--rw-r--r--   0 oo11       (501) staff       (20)    11091 2023-03-04 11:18:36.000000 camel-kenlm-2023.3.17.2/util/usage.cc
--rw-r--r--   0 oo11       (501) staff       (20)      702 2021-12-27 07:00:41.000000 camel-kenlm-2023.3.17.2/util/usage.hh
+drwxr-xr-x   0 oo11       (501) staff       (20)        0 2024-05-02 13:54:48.849623 camel-kenlm-2024.1.30/
+drwxr-xr-x   0 oo11       (501) staff       (20)        0 2024-05-02 13:54:48.704259 camel-kenlm-2024.1.30/.github/
+drwxr-xr-x   0 oo11       (501) staff       (20)        0 2024-05-02 13:54:48.714489 camel-kenlm-2024.1.30/.github/workflows/
+-rw-r--r--   0 oo11       (501) staff       (20)      542 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/.github/workflows/mac.yml
+-rw-r--r--   0 oo11       (501) staff       (20)      619 2023-03-04 11:18:36.000000 camel-kenlm-2024.1.30/.github/workflows/ubuntu.yml
+-rw-r--r--   0 oo11       (501) staff       (20)      471 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/.github/workflows/windows.yml
+-rw-r--r--   0 oo11       (501) staff       (20)      281 2024-01-30 16:41:55.000000 camel-kenlm-2024.1.30/.gitignore
+-rw-r--r--   0 oo11       (501) staff       (20)      696 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/BUILDING
+-rw-r--r--   0 oo11       (501) staff       (20)     4792 2023-04-05 15:17:16.000000 camel-kenlm-2024.1.30/CMakeLists.txt
+-rw-r--r--   0 oo11       (501) staff       (20)    26530 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/COPYING
+-rw-r--r--   0 oo11       (501) staff       (20)    35147 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/COPYING.3
+-rw-r--r--   0 oo11       (501) staff       (20)     7637 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/COPYING.LESSER.3
+-rw-r--r--   0 oo11       (501) staff       (20)    63537 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/Doxyfile
+-rw-r--r--   0 oo11       (501) staff       (20)     1150 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/LICENSE
+-rw-r--r--   0 oo11       (501) staff       (20)      220 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/MANIFEST.in
+-rw-r--r--   0 oo11       (501) staff       (20)      210 2024-05-02 13:54:48.849263 camel-kenlm-2024.1.30/PKG-INFO
+-rw-r--r--   0 oo11       (501) staff       (20)     6359 2023-03-17 09:22:54.000000 camel-kenlm-2024.1.30/README.md
+drwxr-xr-x   0 oo11       (501) staff       (20)        0 2024-05-02 13:54:48.716015 camel-kenlm-2024.1.30/camel_kenlm.egg-info/
+-rw-r--r--   0 oo11       (501) staff       (20)      210 2024-05-02 13:54:48.000000 camel-kenlm-2024.1.30/camel_kenlm.egg-info/PKG-INFO
+-rw-r--r--   0 oo11       (501) staff       (20)     7780 2024-05-02 13:54:48.000000 camel-kenlm-2024.1.30/camel_kenlm.egg-info/SOURCES.txt
+-rw-r--r--   0 oo11       (501) staff       (20)        1 2024-05-02 13:54:48.000000 camel-kenlm-2024.1.30/camel_kenlm.egg-info/dependency_links.txt
+-rw-r--r--   0 oo11       (501) staff       (20)        6 2024-05-02 13:54:48.000000 camel-kenlm-2024.1.30/camel_kenlm.egg-info/top_level.txt
+-rwxr-xr-x   0 oo11       (501) staff       (20)       81 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/clean_query_only.sh
+drwxr-xr-x   0 oo11       (501) staff       (20)        0 2024-05-02 13:54:48.716495 camel-kenlm-2024.1.30/cmake/
+-rw-r--r--   0 oo11       (501) staff       (20)     2821 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/cmake/KenLMFunctions.cmake
+-rw-r--r--   0 oo11       (501) staff       (20)      334 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/cmake/kenlmConfig.cmake.in
+drwxr-xr-x   0 oo11       (501) staff       (20)        0 2024-05-02 13:54:48.716732 camel-kenlm-2024.1.30/cmake/modules/
+-rw-r--r--   0 oo11       (501) staff       (20)     3185 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/cmake/modules/FindEigen3.cmake
+-rwxr-xr-x   0 oo11       (501) staff       (20)     1154 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/compile_query_only.sh
+drwxr-xr-x   0 oo11       (501) staff       (20)        0 2024-05-02 13:54:48.732235 camel-kenlm-2024.1.30/lm/
+-rw-r--r--   0 oo11       (501) staff       (20)     2097 2023-03-04 11:18:36.000000 camel-kenlm-2024.1.30/lm/CMakeLists.txt
+-rw-r--r--   0 oo11       (501) staff       (20)     3710 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/bhiksha.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     4348 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/bhiksha.hh
+-rw-r--r--   0 oo11       (501) staff       (20)    12931 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/binary_format.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     3498 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/binary_format.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     1379 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/blank.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     8154 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/build_binary_main.cc
+drwxr-xr-x   0 oo11       (501) staff       (20)        0 2024-05-02 13:54:48.739227 camel-kenlm-2024.1.30/lm/builder/
+-rw-r--r--   0 oo11       (501) staff       (20)     1897 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/builder/CMakeLists.txt
+-rw-r--r--   0 oo11       (501) staff       (20)      826 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/builder/README.md
+-rw-r--r--   0 oo11       (501) staff       (20)      152 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/builder/TODO
+-rw-r--r--   0 oo11       (501) staff       (20)    12607 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/builder/adjust_counts.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     2258 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/builder/adjust_counts.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     3509 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/builder/adjust_counts_test.cc
+-rw-r--r--   0 oo11       (501) staff       (20)      899 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/builder/combine_counts.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     9550 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/builder/corpus_count.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     1701 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/builder/corpus_count.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     2820 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/builder/corpus_count_test.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     3992 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/builder/count_ngrams_main.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     2411 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/builder/debug_print.hh
+-rw-r--r--   0 oo11       (501) staff       (20)      439 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/builder/discount.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     1869 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/builder/dump_counts_main.cc
+-rw-r--r--   0 oo11       (501) staff       (20)      293 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/builder/hash_gamma.hh
+-rw-r--r--   0 oo11       (501) staff       (20)      715 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/builder/header_info.hh
+-rw-r--r--   0 oo11       (501) staff       (20)    10698 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/builder/initial_probabilities.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     1452 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/builder/initial_probabilities.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     6044 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/builder/interpolate.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     1136 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/builder/interpolate.hh
+-rw-r--r--   0 oo11       (501) staff       (20)    11967 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/builder/lmplz_main.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     1625 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/builder/output.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     2529 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/builder/output.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     1051 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/builder/payload.hh
+-rw-r--r--   0 oo11       (501) staff       (20)    17887 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/builder/pipeline.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     2572 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/builder/pipeline.hh
+drwxr-xr-x   0 oo11       (501) staff       (20)        0 2024-05-02 13:54:48.743257 camel-kenlm-2024.1.30/lm/common/
+-rw-r--r--   0 oo11       (501) staff       (20)      889 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/common/CMakeLists.txt
+-rw-r--r--   0 oo11       (501) staff       (20)     6078 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/common/compare.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     2366 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/common/joint_order.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     5186 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/common/model_buffer.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     2155 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/common/model_buffer.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     1713 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/common/model_buffer_test.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     2112 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/common/ngram.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     1872 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/common/ngram_stream.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     1890 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/common/print.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     1483 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/common/print.hh
+-rw-r--r--   0 oo11       (501) staff       (20)      398 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/common/renumber.cc
+-rw-r--r--   0 oo11       (501) staff       (20)      755 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/common/renumber.hh
+-rw-r--r--   0 oo11       (501) staff       (20)      562 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/common/size_option.cc
+-rw-r--r--   0 oo11       (501) staff       (20)      302 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/common/size_option.hh
+-rw-r--r--   0 oo11       (501) staff       (20)      550 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/common/special.hh
+drwxr-xr-x   0 oo11       (501) staff       (20)        0 2024-05-02 13:54:48.744173 camel-kenlm-2024.1.30/lm/common/test_data/
+drwxr-xr-x   0 oo11       (501) staff       (20)        0 2024-05-02 13:54:48.746760 camel-kenlm-2024.1.30/lm/common/test_data/bigendian/
+-rw-r--r--   0 oo11       (501) staff       (20)       60 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/common/test_data/bigendian/toy0.1
+-rw-r--r--   0 oo11       (501) staff       (20)      112 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/common/test_data/bigendian/toy0.2
+-rw-r--r--   0 oo11       (501) staff       (20)      140 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/common/test_data/bigendian/toy0.3
+-rw-r--r--   0 oo11       (501) staff       (20)       55 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/common/test_data/bigendian/toy0.kenlm_intermediate
+-rw-r--r--   0 oo11       (501) staff       (20)       19 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/common/test_data/bigendian/toy0.vocab
+-rw-r--r--   0 oo11       (501) staff       (20)       72 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/common/test_data/bigendian/toy1.1
+-rw-r--r--   0 oo11       (501) staff       (20)      112 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/common/test_data/bigendian/toy1.2
+-rw-r--r--   0 oo11       (501) staff       (20)      120 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/common/test_data/bigendian/toy1.3
+-rw-r--r--   0 oo11       (501) staff       (20)       55 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/common/test_data/bigendian/toy1.kenlm_intermediate
+-rw-r--r--   0 oo11       (501) staff       (20)       21 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/common/test_data/bigendian/toy1.vocab
+-rwxr-xr-x   0 oo11       (501) staff       (20)      270 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/common/test_data/generate.sh
+drwxr-xr-x   0 oo11       (501) staff       (20)        0 2024-05-02 13:54:48.749536 camel-kenlm-2024.1.30/lm/common/test_data/littleendian/
+-rw-r--r--   0 oo11       (501) staff       (20)       60 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/common/test_data/littleendian/toy0.1
+-rw-r--r--   0 oo11       (501) staff       (20)      112 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/common/test_data/littleendian/toy0.2
+-rw-r--r--   0 oo11       (501) staff       (20)      140 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/common/test_data/littleendian/toy0.3
+-rw-r--r--   0 oo11       (501) staff       (20)       55 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/common/test_data/littleendian/toy0.kenlm_intermediate
+-rw-r--r--   0 oo11       (501) staff       (20)       19 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/common/test_data/littleendian/toy0.vocab
+-rw-r--r--   0 oo11       (501) staff       (20)       72 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/common/test_data/littleendian/toy1.1
+-rw-r--r--   0 oo11       (501) staff       (20)      112 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/common/test_data/littleendian/toy1.2
+-rw-r--r--   0 oo11       (501) staff       (20)      120 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/common/test_data/littleendian/toy1.3
+-rw-r--r--   0 oo11       (501) staff       (20)       55 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/common/test_data/littleendian/toy1.kenlm_intermediate
+-rw-r--r--   0 oo11       (501) staff       (20)       21 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/common/test_data/littleendian/toy1.vocab
+-rw-r--r--   0 oo11       (501) staff       (20)      475 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/common/test_data/toy0.arpa
+-rw-r--r--   0 oo11       (501) staff       (20)      470 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/common/test_data/toy1.arpa
+-rw-r--r--   0 oo11       (501) staff       (20)      675 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/config.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     3913 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/config.hh
+-rw-r--r--   0 oo11       (501) staff       (20)      722 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/enumerate_vocab.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     2544 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/facade.hh
+drwxr-xr-x   0 oo11       (501) staff       (20)        0 2024-05-02 13:54:48.752626 camel-kenlm-2024.1.30/lm/filter/
+-rw-r--r--   0 oo11       (501) staff       (20)     1327 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/filter/CMakeLists.txt
+-rw-r--r--   0 oo11       (501) staff       (20)     1935 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/filter/arpa_io.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     2816 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/filter/arpa_io.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     2458 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/filter/count_io.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     9352 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/filter/filter_main.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     7379 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/filter/format.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     8212 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/filter/phrase.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     5778 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/filter/phrase.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     5027 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/filter/phrase_table_vocab_main.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     4205 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/filter/thread.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     1209 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/filter/vocab.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     4123 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/filter/vocab.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     1797 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/filter/wrapper.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     1068 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/fragment_main.cc
+drwxr-xr-x   0 oo11       (501) staff       (20)        0 2024-05-02 13:54:48.763941 camel-kenlm-2024.1.30/lm/interpolate/
+-rw-r--r--   0 oo11       (501) staff       (20)     1774 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/interpolate/CMakeLists.txt
+-rw-r--r--   0 oo11       (501) staff       (20)      737 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/interpolate/backoff_matrix.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     1952 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/interpolate/backoff_reunification.cc
+-rw-r--r--   0 oo11       (501) staff       (20)      913 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/interpolate/backoff_reunification.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     4904 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/interpolate/backoff_reunification_test.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     1086 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/interpolate/bounded_sequence_encoding.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     2530 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/interpolate/bounded_sequence_encoding.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     3222 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/interpolate/bounded_sequence_encoding_test.cc
+-rw-r--r--   0 oo11       (501) staff       (20)      693 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/interpolate/interpolate_info.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     5296 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/interpolate/interpolate_main.cc
+-rw-r--r--   0 oo11       (501) staff       (20)    10010 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/interpolate/merge_probabilities.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     3385 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/interpolate/merge_probabilities.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     3586 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/interpolate/merge_vocab.cc
+-rw-r--r--   0 oo11       (501) staff       (20)      572 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/interpolate/merge_vocab.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     5306 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/interpolate/merge_vocab_test.cc
+-rw-r--r--   0 oo11       (501) staff       (20)    13813 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/interpolate/normalize.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     1101 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/interpolate/normalize.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     2758 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/interpolate/normalize_test.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     7645 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/interpolate/pipeline.cc
+-rw-r--r--   0 oo11       (501) staff       (20)      552 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/interpolate/pipeline.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     1235 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/interpolate/split_worker.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     1100 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/interpolate/split_worker.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     7430 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/interpolate/streaming_example_main.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     5950 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/interpolate/tune_derivatives.cc
+-rw-r--r--   0 oo11       (501) staff       (20)      590 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/interpolate/tune_derivatives.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     3969 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/interpolate/tune_derivatives_test.cc
+-rw-r--r--   0 oo11       (501) staff       (20)    19605 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/interpolate/tune_instances.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     2956 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/interpolate/tune_instances.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     4571 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/interpolate/tune_instances_test.cc
+-rw-r--r--   0 oo11       (501) staff       (20)      512 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/interpolate/tune_matrix.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     1366 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/interpolate/tune_weights.cc
+-rw-r--r--   0 oo11       (501) staff       (20)      446 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/interpolate/tune_weights.hh
+-rw-r--r--   0 oo11       (501) staff       (20)      342 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/interpolate/universal_vocab.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     1347 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/interpolate/universal_vocab.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     9039 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/kenlm_benchmark_main.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     7174 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/left.hh
+-rw-r--r--   0 oo11       (501) staff       (20)    12402 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/left_test.cc
+-rw-r--r--   0 oo11       (501) staff       (20)      637 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/lm_exception.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     1057 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/lm_exception.hh
+-rw-r--r--   0 oo11       (501) staff       (20)      644 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/max_order.hh
+-rw-r--r--   0 oo11       (501) staff       (20)    16256 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/model.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     7051 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/model.hh
+-rw-r--r--   0 oo11       (501) staff       (20)    14544 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/model_test.cc
+-rw-r--r--   0 oo11       (501) staff       (20)      798 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/model_type.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     3534 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/ngram_query.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     6003 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/partial.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     6672 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/partial_test.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     3743 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/quantize.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     7749 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/quantize.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     4675 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/query_main.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     7543 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/read_arpa.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     3016 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/read_arpa.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     1248 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/return.hh
+-rw-r--r--   0 oo11       (501) staff       (20)    12060 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/search_hashed.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     5935 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/search_hashed.hh
+-rw-r--r--   0 oo11       (501) staff       (20)    23394 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/search_trie.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     4906 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/search_trie.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     2594 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/sizes.cc
+-rw-r--r--   0 oo11       (501) staff       (20)      374 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/sizes.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     3440 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/state.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     2780 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/test.arpa
+-rw-r--r--   0 oo11       (501) staff       (20)     2694 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/test_nounk.arpa
+-rw-r--r--   0 oo11       (501) staff       (20)     5639 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/trie.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     3563 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/trie.hh
+-rw-r--r--   0 oo11       (501) staff       (20)    10982 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/trie_sort.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     2795 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/trie_sort.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     3935 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/value.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     2045 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/value_build.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     2568 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/value_build.hh
+-rw-r--r--   0 oo11       (501) staff       (20)      380 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/virtual_interface.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     5668 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/virtual_interface.hh
+-rw-r--r--   0 oo11       (501) staff       (20)    11083 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/vocab.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     8680 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/vocab.hh
+-rw-r--r--   0 oo11       (501) staff       (20)      358 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/weights.hh
+-rw-r--r--   0 oo11       (501) staff       (20)      293 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/word_index.hh
+drwxr-xr-x   0 oo11       (501) staff       (20)        0 2024-05-02 13:54:48.764760 camel-kenlm-2024.1.30/lm/wrappers/
+-rw-r--r--   0 oo11       (501) staff       (20)      176 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/wrappers/README
+-rw-r--r--   0 oo11       (501) staff       (20)     4261 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/wrappers/nplm.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     1975 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/lm/wrappers/nplm.hh
+-rw-r--r--   0 oo11       (501) staff       (20)       59 2023-03-04 11:18:36.000000 camel-kenlm-2024.1.30/pyproject.toml
+drwxr-xr-x   0 oo11       (501) staff       (20)        0 2024-05-02 13:54:48.766978 camel-kenlm-2024.1.30/python/
+-rw-r--r--   0 oo11       (501) staff       (20)      988 2023-03-04 11:18:36.000000 camel-kenlm-2024.1.30/python/CMakeLists.txt
+-rw-r--r--   0 oo11       (501) staff       (20)     1957 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/python/_kenlm.pxd
+-rwxr-xr-x   0 oo11       (501) staff       (20)     1427 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/python/example.py
+-rw-r--r--   0 oo11       (501) staff       (20)   450422 2024-01-30 16:43:40.000000 camel-kenlm-2024.1.30/python/kenlm.cpp
+-rw-r--r--   0 oo11       (501) staff       (20)     9323 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/python/kenlm.pyx
+-rw-r--r--   0 oo11       (501) staff       (20)      906 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/python/score_sentence.cc
+-rw-r--r--   0 oo11       (501) staff       (20)      325 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/python/score_sentence.hh
+-rw-r--r--   0 oo11       (501) staff       (20)       38 2024-05-02 13:54:48.849714 camel-kenlm-2024.1.30/setup.cfg
+-rw-r--r--   0 oo11       (501) staff       (20)     4534 2024-03-01 07:11:30.000000 camel-kenlm-2024.1.30/setup.py
+drwxr-xr-x   0 oo11       (501) staff       (20)        0 2024-05-02 13:54:48.822352 camel-kenlm-2024.1.30/util/
+-rw-r--r--   0 oo11       (501) staff       (20)     3873 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/CMakeLists.txt
+-rw-r--r--   0 oo11       (501) staff       (20)     1176 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/bit_packing.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     5967 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/bit_packing.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     1490 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/bit_packing_test.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     1227 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/cat_compressed_main.cc
+drwxr-xr-x   0 oo11       (501) staff       (20)        0 2024-05-02 13:54:48.840990 camel-kenlm-2024.1.30/util/double-conversion/
+-rw-r--r--   0 oo11       (501) staff       (20)     1042 2023-03-04 11:18:36.000000 camel-kenlm-2024.1.30/util/double-conversion/CMakeLists.txt
+-rw-r--r--   0 oo11       (501) staff       (20)     1527 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/double-conversion/LICENSE
+-rw-r--r--   0 oo11       (501) staff       (20)    27617 2023-03-04 11:18:36.000000 camel-kenlm-2024.1.30/util/double-conversion/bignum-dtoa.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     4300 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/double-conversion/bignum-dtoa.h
+-rw-r--r--   0 oo11       (501) staff       (20)    24726 2023-03-04 11:18:36.000000 camel-kenlm-2024.1.30/util/double-conversion/bignum.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     5891 2023-03-04 11:18:36.000000 camel-kenlm-2024.1.30/util/double-conversion/bignum.h
+-rw-r--r--   0 oo11       (501) staff       (20)     9913 2023-03-04 11:18:36.000000 camel-kenlm-2024.1.30/util/double-conversion/cached-powers.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     3021 2023-03-04 11:18:36.000000 camel-kenlm-2024.1.30/util/double-conversion/cached-powers.h
+-rw-r--r--   0 oo11       (501) staff       (20)     5030 2023-03-04 11:18:36.000000 camel-kenlm-2024.1.30/util/double-conversion/diy-fp.h
+-rw-r--r--   0 oo11       (501) staff       (20)     1804 2023-03-04 11:18:36.000000 camel-kenlm-2024.1.30/util/double-conversion/double-conversion.h
+-rw-r--r--   0 oo11       (501) staff       (20)    15851 2023-03-04 11:18:36.000000 camel-kenlm-2024.1.30/util/double-conversion/double-to-string.cc
+-rw-r--r--   0 oo11       (501) staff       (20)    22349 2023-03-04 11:18:36.000000 camel-kenlm-2024.1.30/util/double-conversion/double-to-string.h
+-rw-r--r--   0 oo11       (501) staff       (20)    31645 2023-03-04 11:18:36.000000 camel-kenlm-2024.1.30/util/double-conversion/fast-dtoa.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     4064 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/double-conversion/fast-dtoa.h
+-rw-r--r--   0 oo11       (501) staff       (20)    15352 2023-03-04 11:18:36.000000 camel-kenlm-2024.1.30/util/double-conversion/fixed-dtoa.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     2770 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/double-conversion/fixed-dtoa.h
+-rw-r--r--   0 oo11       (501) staff       (20)    15223 2023-03-04 11:18:36.000000 camel-kenlm-2024.1.30/util/double-conversion/ieee.h
+-rw-r--r--   0 oo11       (501) staff       (20)    27857 2023-03-04 11:18:36.000000 camel-kenlm-2024.1.30/util/double-conversion/string-to-double.cc
+-rw-r--r--   0 oo11       (501) staff       (20)    10848 2023-03-04 11:18:36.000000 camel-kenlm-2024.1.30/util/double-conversion/string-to-double.h
+-rw-r--r--   0 oo11       (501) staff       (20)    23469 2023-03-04 11:18:36.000000 camel-kenlm-2024.1.30/util/double-conversion/strtod.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     3038 2023-03-04 11:18:36.000000 camel-kenlm-2024.1.30/util/double-conversion/strtod.h
+-rw-r--r--   0 oo11       (501) staff       (20)    15340 2023-03-04 11:18:36.000000 camel-kenlm-2024.1.30/util/double-conversion/utils.h
+-rw-r--r--   0 oo11       (501) staff       (20)     1367 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/ersatz_progress.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     1603 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/ersatz_progress.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     2765 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/exception.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     4392 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/exception.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     3994 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/fake_ostream.hh
+-rw-r--r--   0 oo11       (501) staff       (20)    18350 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/file.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     4746 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/file.hh
+-rw-r--r--   0 oo11       (501) staff       (20)    10877 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/file_piece.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     6515 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/file_piece.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     5364 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/file_piece_test.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     2424 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/file_stream.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     5545 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/fixed_array.hh
+-rw-r--r--   0 oo11       (501) staff       (20)      729 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/float_to_string.cc
+-rw-r--r--   0 oo11       (501) staff       (20)      609 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/float_to_string.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     1441 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/getopt.c
+-rw-r--r--   0 oo11       (501) staff       (20)      472 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/getopt.hh
+-rw-r--r--   0 oo11       (501) staff       (20)      270 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/have.hh
+-rw-r--r--   0 oo11       (501) staff       (20)    22498 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/integer_to_string.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     1636 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/integer_to_string.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     1959 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/integer_to_string_test.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     4905 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/joint_sort.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     1738 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/joint_sort_test.cc
+-rw-r--r--   0 oo11       (501) staff       (20)    13507 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/mmap.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     6780 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/mmap.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     3379 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/multi_intersection.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     1887 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/multi_intersection_test.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     4074 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/murmur_hash.cc
+-rw-r--r--   0 oo11       (501) staff       (20)      616 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/murmur_hash.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     1546 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/parallel_read.cc
+-rw-r--r--   0 oo11       (501) staff       (20)      461 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/parallel_read.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     3480 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/pcqueue.hh
+-rw-r--r--   0 oo11       (501) staff       (20)      355 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/pcqueue_test.cc
+-rw-r--r--   0 oo11       (501) staff       (20)      705 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/pool.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     2956 2024-01-30 16:43:40.000000 camel-kenlm-2024.1.30/util/pool.hh
+-rw-r--r--   0 oo11       (501) staff       (20)    13233 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/probing_hash_table.hh
+-rw-r--r--   0 oo11       (501) staff       (20)    11788 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/probing_hash_table_benchmark_main.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     2269 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/probing_hash_table_test.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     3526 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/proxy_iterator.hh
+-rw-r--r--   0 oo11       (501) staff       (20)    13086 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/read_compressed.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     2034 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/read_compressed.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     2669 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/read_compressed_test.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     1118 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/scoped.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     3660 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/scoped.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     6581 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/sized_iterator.hh
+-rw-r--r--   0 oo11       (501) staff       (20)      559 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/sized_iterator_test.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     3257 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/sorted_uniform.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     3621 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/sorted_uniform_test.cc
+-rw-r--r--   0 oo11       (501) staff       (20)      751 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/spaces.cc
+-rw-r--r--   0 oo11       (501) staff       (20)      167 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/spaces.hh
+drwxr-xr-x   0 oo11       (501) staff       (20)        0 2024-05-02 13:54:48.848767 camel-kenlm-2024.1.30/util/stream/
+-rw-r--r--   0 oo11       (501) staff       (20)     1237 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/stream/CMakeLists.txt
+-rw-r--r--   0 oo11       (501) staff       (20)     2420 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/stream/block.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     4367 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/stream/chain.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     8996 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/stream/chain.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     1606 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/stream/config.hh
+-rw-r--r--   0 oo11       (501) staff       (20)      278 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/stream/count_records.cc
+-rw-r--r--   0 oo11       (501) staff       (20)      300 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/stream/count_records.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     2436 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/stream/io.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     1843 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/stream/io.hh
+-rw-r--r--   0 oo11       (501) staff       (20)      823 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/stream/io_test.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     1418 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/stream/line_input.cc
+-rw-r--r--   0 oo11       (501) staff       (20)      515 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/stream/line_input.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     2363 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/stream/multi_progress.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     1848 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/stream/multi_progress.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     3362 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/stream/multi_stream.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     3627 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/stream/rewindable_stream.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     3241 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/stream/rewindable_stream.hh
+-rw-r--r--   0 oo11       (501) staff       (20)      899 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/stream/rewindable_stream_test.cc
+-rw-r--r--   0 oo11       (501) staff       (20)    20450 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/stream/sort.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     1663 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/stream/sort_test.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     1821 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/stream/stream.hh
+-rw-r--r--   0 oo11       (501) staff       (20)      759 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/stream/stream_test.cc
+-rw-r--r--   0 oo11       (501) staff       (20)      732 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/stream/typed_stream.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     5480 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/string_piece.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     9185 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/string_piece.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     1500 2024-01-30 16:43:40.000000 camel-kenlm-2024.1.30/util/string_piece_hash.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     1039 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/string_stream.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     1778 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/string_stream_test.cc
+-rw-r--r--   0 oo11       (501) staff       (20)     3825 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/thread_pool.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     4890 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/tokenize_piece.hh
+-rw-r--r--   0 oo11       (501) staff       (20)     1135 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/tokenize_piece_test.cc
+-rw-r--r--   0 oo11       (501) staff       (20)    11091 2023-03-04 11:18:36.000000 camel-kenlm-2024.1.30/util/usage.cc
+-rw-r--r--   0 oo11       (501) staff       (20)      702 2021-12-27 07:00:41.000000 camel-kenlm-2024.1.30/util/usage.hh
```

### Comparing `camel-kenlm-2023.3.17.2/.github/workflows/mac.yml` & `camel-kenlm-2024.1.30/.github/workflows/mac.yml`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/.github/workflows/ubuntu.yml` & `camel-kenlm-2024.1.30/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/BUILDING` & `camel-kenlm-2024.1.30/BUILDING`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/CMakeLists.txt` & `camel-kenlm-2024.1.30/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/COPYING` & `camel-kenlm-2024.1.30/COPYING`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/COPYING.3` & `camel-kenlm-2024.1.30/COPYING.3`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/COPYING.LESSER.3` & `camel-kenlm-2024.1.30/COPYING.LESSER.3`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/Doxyfile` & `camel-kenlm-2024.1.30/Doxyfile`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/LICENSE` & `camel-kenlm-2024.1.30/LICENSE`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/README.md` & `camel-kenlm-2024.1.30/README.md`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/camel_kenlm.egg-info/SOURCES.txt` & `camel-kenlm-2024.1.30/camel_kenlm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/cmake/KenLMFunctions.cmake` & `camel-kenlm-2024.1.30/cmake/KenLMFunctions.cmake`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/cmake/modules/FindEigen3.cmake` & `camel-kenlm-2024.1.30/cmake/modules/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/compile_query_only.sh` & `camel-kenlm-2024.1.30/compile_query_only.sh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/CMakeLists.txt` & `camel-kenlm-2024.1.30/lm/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/bhiksha.cc` & `camel-kenlm-2024.1.30/lm/bhiksha.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/bhiksha.hh` & `camel-kenlm-2024.1.30/lm/bhiksha.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/binary_format.cc` & `camel-kenlm-2024.1.30/lm/binary_format.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/binary_format.hh` & `camel-kenlm-2024.1.30/lm/binary_format.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/blank.hh` & `camel-kenlm-2024.1.30/lm/blank.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/build_binary_main.cc` & `camel-kenlm-2024.1.30/lm/build_binary_main.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/builder/CMakeLists.txt` & `camel-kenlm-2024.1.30/lm/builder/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/builder/README.md` & `camel-kenlm-2024.1.30/lm/builder/README.md`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/builder/adjust_counts.cc` & `camel-kenlm-2024.1.30/lm/builder/adjust_counts.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/builder/adjust_counts.hh` & `camel-kenlm-2024.1.30/lm/builder/adjust_counts.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/builder/adjust_counts_test.cc` & `camel-kenlm-2024.1.30/lm/builder/adjust_counts_test.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/builder/combine_counts.hh` & `camel-kenlm-2024.1.30/lm/builder/combine_counts.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/builder/corpus_count.cc` & `camel-kenlm-2024.1.30/lm/builder/corpus_count.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/builder/corpus_count.hh` & `camel-kenlm-2024.1.30/lm/builder/corpus_count.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/builder/corpus_count_test.cc` & `camel-kenlm-2024.1.30/lm/builder/corpus_count_test.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/builder/count_ngrams_main.cc` & `camel-kenlm-2024.1.30/lm/builder/count_ngrams_main.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/builder/debug_print.hh` & `camel-kenlm-2024.1.30/lm/builder/debug_print.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/builder/dump_counts_main.cc` & `camel-kenlm-2024.1.30/lm/builder/dump_counts_main.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/builder/header_info.hh` & `camel-kenlm-2024.1.30/lm/builder/header_info.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/builder/initial_probabilities.cc` & `camel-kenlm-2024.1.30/lm/builder/initial_probabilities.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/builder/initial_probabilities.hh` & `camel-kenlm-2024.1.30/lm/builder/initial_probabilities.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/builder/interpolate.cc` & `camel-kenlm-2024.1.30/lm/builder/interpolate.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/builder/interpolate.hh` & `camel-kenlm-2024.1.30/lm/builder/interpolate.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/builder/lmplz_main.cc` & `camel-kenlm-2024.1.30/lm/builder/lmplz_main.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/builder/output.cc` & `camel-kenlm-2024.1.30/lm/builder/output.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/builder/output.hh` & `camel-kenlm-2024.1.30/lm/builder/output.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/builder/payload.hh` & `camel-kenlm-2024.1.30/lm/builder/payload.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/builder/pipeline.cc` & `camel-kenlm-2024.1.30/lm/builder/pipeline.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/builder/pipeline.hh` & `camel-kenlm-2024.1.30/lm/builder/pipeline.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/common/CMakeLists.txt` & `camel-kenlm-2024.1.30/lm/common/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/common/compare.hh` & `camel-kenlm-2024.1.30/lm/common/compare.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/common/joint_order.hh` & `camel-kenlm-2024.1.30/lm/common/joint_order.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/common/model_buffer.cc` & `camel-kenlm-2024.1.30/lm/common/model_buffer.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/common/model_buffer.hh` & `camel-kenlm-2024.1.30/lm/common/model_buffer.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/common/model_buffer_test.cc` & `camel-kenlm-2024.1.30/lm/common/model_buffer_test.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/common/ngram.hh` & `camel-kenlm-2024.1.30/lm/common/ngram.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/common/ngram_stream.hh` & `camel-kenlm-2024.1.30/lm/common/ngram_stream.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/common/print.cc` & `camel-kenlm-2024.1.30/lm/common/print.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/common/print.hh` & `camel-kenlm-2024.1.30/lm/common/print.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/common/renumber.hh` & `camel-kenlm-2024.1.30/lm/common/renumber.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/common/size_option.cc` & `camel-kenlm-2024.1.30/lm/common/size_option.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/common/special.hh` & `camel-kenlm-2024.1.30/lm/common/special.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/config.cc` & `camel-kenlm-2024.1.30/lm/config.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/config.hh` & `camel-kenlm-2024.1.30/lm/config.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/enumerate_vocab.hh` & `camel-kenlm-2024.1.30/lm/enumerate_vocab.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/facade.hh` & `camel-kenlm-2024.1.30/lm/facade.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/filter/CMakeLists.txt` & `camel-kenlm-2024.1.30/lm/filter/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/filter/arpa_io.cc` & `camel-kenlm-2024.1.30/lm/filter/arpa_io.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/filter/arpa_io.hh` & `camel-kenlm-2024.1.30/lm/filter/arpa_io.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/filter/count_io.hh` & `camel-kenlm-2024.1.30/lm/filter/count_io.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/filter/filter_main.cc` & `camel-kenlm-2024.1.30/lm/filter/filter_main.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/filter/format.hh` & `camel-kenlm-2024.1.30/lm/filter/format.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/filter/phrase.cc` & `camel-kenlm-2024.1.30/lm/filter/phrase.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/filter/phrase.hh` & `camel-kenlm-2024.1.30/lm/filter/phrase.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/filter/phrase_table_vocab_main.cc` & `camel-kenlm-2024.1.30/lm/filter/phrase_table_vocab_main.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/filter/thread.hh` & `camel-kenlm-2024.1.30/lm/filter/thread.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/filter/vocab.cc` & `camel-kenlm-2024.1.30/lm/filter/vocab.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/filter/vocab.hh` & `camel-kenlm-2024.1.30/lm/filter/vocab.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/filter/wrapper.hh` & `camel-kenlm-2024.1.30/lm/filter/wrapper.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/fragment_main.cc` & `camel-kenlm-2024.1.30/lm/fragment_main.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/interpolate/CMakeLists.txt` & `camel-kenlm-2024.1.30/lm/interpolate/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/interpolate/backoff_matrix.hh` & `camel-kenlm-2024.1.30/lm/interpolate/backoff_matrix.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/interpolate/backoff_reunification.cc` & `camel-kenlm-2024.1.30/lm/interpolate/backoff_reunification.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/interpolate/backoff_reunification.hh` & `camel-kenlm-2024.1.30/lm/interpolate/backoff_reunification.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/interpolate/backoff_reunification_test.cc` & `camel-kenlm-2024.1.30/lm/interpolate/backoff_reunification_test.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/interpolate/bounded_sequence_encoding.cc` & `camel-kenlm-2024.1.30/lm/interpolate/bounded_sequence_encoding.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/interpolate/bounded_sequence_encoding.hh` & `camel-kenlm-2024.1.30/lm/interpolate/bounded_sequence_encoding.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/interpolate/bounded_sequence_encoding_test.cc` & `camel-kenlm-2024.1.30/lm/interpolate/bounded_sequence_encoding_test.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/interpolate/interpolate_info.hh` & `camel-kenlm-2024.1.30/lm/interpolate/interpolate_info.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/interpolate/interpolate_main.cc` & `camel-kenlm-2024.1.30/lm/interpolate/interpolate_main.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/interpolate/merge_probabilities.cc` & `camel-kenlm-2024.1.30/lm/interpolate/merge_probabilities.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/interpolate/merge_probabilities.hh` & `camel-kenlm-2024.1.30/lm/interpolate/merge_probabilities.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/interpolate/merge_vocab.cc` & `camel-kenlm-2024.1.30/lm/interpolate/merge_vocab.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/interpolate/merge_vocab.hh` & `camel-kenlm-2024.1.30/lm/interpolate/merge_vocab.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/interpolate/merge_vocab_test.cc` & `camel-kenlm-2024.1.30/lm/interpolate/merge_vocab_test.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/interpolate/normalize.cc` & `camel-kenlm-2024.1.30/lm/interpolate/normalize.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/interpolate/normalize.hh` & `camel-kenlm-2024.1.30/lm/interpolate/normalize.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/interpolate/normalize_test.cc` & `camel-kenlm-2024.1.30/lm/interpolate/normalize_test.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/interpolate/pipeline.cc` & `camel-kenlm-2024.1.30/lm/interpolate/pipeline.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/interpolate/pipeline.hh` & `camel-kenlm-2024.1.30/lm/interpolate/pipeline.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/interpolate/split_worker.cc` & `camel-kenlm-2024.1.30/lm/interpolate/split_worker.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/interpolate/split_worker.hh` & `camel-kenlm-2024.1.30/lm/interpolate/split_worker.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/interpolate/streaming_example_main.cc` & `camel-kenlm-2024.1.30/lm/interpolate/streaming_example_main.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/interpolate/tune_derivatives.cc` & `camel-kenlm-2024.1.30/lm/interpolate/tune_derivatives.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/interpolate/tune_derivatives.hh` & `camel-kenlm-2024.1.30/lm/interpolate/tune_derivatives.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/interpolate/tune_derivatives_test.cc` & `camel-kenlm-2024.1.30/lm/interpolate/tune_derivatives_test.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/interpolate/tune_instances.cc` & `camel-kenlm-2024.1.30/lm/interpolate/tune_instances.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/interpolate/tune_instances.hh` & `camel-kenlm-2024.1.30/lm/interpolate/tune_instances.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/interpolate/tune_instances_test.cc` & `camel-kenlm-2024.1.30/lm/interpolate/tune_instances_test.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/interpolate/tune_matrix.hh` & `camel-kenlm-2024.1.30/lm/interpolate/tune_matrix.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/interpolate/tune_weights.cc` & `camel-kenlm-2024.1.30/lm/interpolate/tune_weights.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/interpolate/universal_vocab.hh` & `camel-kenlm-2024.1.30/lm/interpolate/universal_vocab.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/kenlm_benchmark_main.cc` & `camel-kenlm-2024.1.30/lm/kenlm_benchmark_main.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/left.hh` & `camel-kenlm-2024.1.30/lm/left.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/left_test.cc` & `camel-kenlm-2024.1.30/lm/left_test.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/lm_exception.cc` & `camel-kenlm-2024.1.30/lm/lm_exception.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/lm_exception.hh` & `camel-kenlm-2024.1.30/lm/lm_exception.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/max_order.hh` & `camel-kenlm-2024.1.30/lm/max_order.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/model.cc` & `camel-kenlm-2024.1.30/lm/model.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/model.hh` & `camel-kenlm-2024.1.30/lm/model.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/model_test.cc` & `camel-kenlm-2024.1.30/lm/model_test.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/model_type.hh` & `camel-kenlm-2024.1.30/lm/model_type.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/ngram_query.hh` & `camel-kenlm-2024.1.30/lm/ngram_query.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/partial.hh` & `camel-kenlm-2024.1.30/lm/partial.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/partial_test.cc` & `camel-kenlm-2024.1.30/lm/partial_test.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/quantize.cc` & `camel-kenlm-2024.1.30/lm/quantize.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/quantize.hh` & `camel-kenlm-2024.1.30/lm/quantize.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/query_main.cc` & `camel-kenlm-2024.1.30/lm/query_main.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/read_arpa.cc` & `camel-kenlm-2024.1.30/lm/read_arpa.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/read_arpa.hh` & `camel-kenlm-2024.1.30/lm/read_arpa.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/return.hh` & `camel-kenlm-2024.1.30/lm/return.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/search_hashed.cc` & `camel-kenlm-2024.1.30/lm/search_hashed.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/search_hashed.hh` & `camel-kenlm-2024.1.30/lm/search_hashed.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/search_trie.cc` & `camel-kenlm-2024.1.30/lm/search_trie.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/search_trie.hh` & `camel-kenlm-2024.1.30/lm/search_trie.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/sizes.cc` & `camel-kenlm-2024.1.30/lm/sizes.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/state.hh` & `camel-kenlm-2024.1.30/lm/state.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/test.arpa` & `camel-kenlm-2024.1.30/lm/test.arpa`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/test_nounk.arpa` & `camel-kenlm-2024.1.30/lm/test_nounk.arpa`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/trie.cc` & `camel-kenlm-2024.1.30/lm/trie.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/trie.hh` & `camel-kenlm-2024.1.30/lm/trie.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/trie_sort.cc` & `camel-kenlm-2024.1.30/lm/trie_sort.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/trie_sort.hh` & `camel-kenlm-2024.1.30/lm/trie_sort.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/value.hh` & `camel-kenlm-2024.1.30/lm/value.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/value_build.cc` & `camel-kenlm-2024.1.30/lm/value_build.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/value_build.hh` & `camel-kenlm-2024.1.30/lm/value_build.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/virtual_interface.hh` & `camel-kenlm-2024.1.30/lm/virtual_interface.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/vocab.cc` & `camel-kenlm-2024.1.30/lm/vocab.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/vocab.hh` & `camel-kenlm-2024.1.30/lm/vocab.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/wrappers/nplm.cc` & `camel-kenlm-2024.1.30/lm/wrappers/nplm.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/lm/wrappers/nplm.hh` & `camel-kenlm-2024.1.30/lm/wrappers/nplm.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/python/CMakeLists.txt` & `camel-kenlm-2024.1.30/python/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/python/_kenlm.pxd` & `camel-kenlm-2024.1.30/python/_kenlm.pxd`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/python/example.py` & `camel-kenlm-2024.1.30/python/example.py`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/python/kenlm.cpp` & `camel-kenlm-2024.1.30/python/kenlm.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.33 */
+/* Generated by Cython 0.29.35 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_33"
-#define CYTHON_HEX_VERSION 0x001D21F0
+#define CYTHON_ABI "0_29_35"
+#define CYTHON_HEX_VERSION 0x001D23F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -74,16 +74,20 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
@@ -199,15 +203,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -238,15 +242,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -6034,15 +6038,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyObject *__pyx_tp_new_5kenlm_State(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_5kenlm_State *p;
   PyObject *o;
@@ -6139,15 +6143,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyObject *__pyx_tp_new_5kenlm_Config(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_5kenlm_Config *p;
   PyObject *o;
@@ -6291,15 +6295,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyObject *__pyx_tp_new_5kenlm_Model(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_5kenlm_Model *p;
   PyObject *o;
@@ -6444,15 +6448,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_5kenlm___pyx_scope_struct__full_scores *__pyx_freelist_5kenlm___pyx_scope_struct__full_scores[8];
 static int __pyx_freecount_5kenlm___pyx_scope_struct__full_scores = 0;
 
@@ -6583,15 +6587,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
@@ -7805,28 +7809,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -8961,15 +8965,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -9271,15 +9275,15 @@
                         } else if (8 * sizeof(enum util::LoadMethod) >= 4 * PyLong_SHIFT) {
                             return (enum util::LoadMethod) (((((((((enum util::LoadMethod)digits[3]) << PyLong_SHIFT) | (enum util::LoadMethod)digits[2]) << PyLong_SHIFT) | (enum util::LoadMethod)digits[1]) << PyLong_SHIFT) | (enum util::LoadMethod)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -9467,15 +9471,15 @@
                         } else if (8 * sizeof(enum lm::ngram::Config::ARPALoadComplain) >= 4 * PyLong_SHIFT) {
                             return (enum lm::ngram::Config::ARPALoadComplain) (((((((((enum lm::ngram::Config::ARPALoadComplain)digits[3]) << PyLong_SHIFT) | (enum lm::ngram::Config::ARPALoadComplain)digits[2]) << PyLong_SHIFT) | (enum lm::ngram::Config::ARPALoadComplain)digits[1]) << PyLong_SHIFT) | (enum lm::ngram::Config::ARPALoadComplain)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -9777,15 +9781,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -11146,15 +11150,18 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
 static int __pyx_Generator_init(void) {
     __pyx_GeneratorType_type.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
     __pyx_GeneratorType_type.tp_iter = PyObject_SelfIter;
     __pyx_GeneratorType = __Pyx_FetchCommonType(&__pyx_GeneratorType_type);
```

### Comparing `camel-kenlm-2023.3.17.2/python/kenlm.pyx` & `camel-kenlm-2024.1.30/python/kenlm.pyx`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/python/score_sentence.cc` & `camel-kenlm-2024.1.30/python/score_sentence.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/setup.py` & `camel-kenlm-2024.1.30/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,15 +70,16 @@
 
         ext_dir = str(Path(self.get_ext_fullpath('libkenlm')).absolute().parent)
         source_dir = str(Path(__file__).absolute().parent)
 
         cmake_args = [
             "-DCMAKE_LIBRARY_OUTPUT_DIRECTORY=" + ext_dir,
             "-DBUILD_SHARED_LIBS=ON",
-            "-DBUILD_PYTHON_STANDALONE=OFF",
+            # Has to be off to compile bindings from pip package
+            "-DBUILD_PYTHON_STANDALONE=ON",
             f"-DKENLM_MAX_ORDER={max_order}",
         ]
         cfg = "Debug" if self.debug else "Release"
         build_args = ["--config", cfg]
 
         if platform.system() == "Windows":
             cmake_args += [
@@ -112,19 +113,20 @@
 
 
 ext_modules = [
     Extension(name='kenlm',
         sources=FILES + ['python/kenlm.cpp'],
         language='C++', 
         include_dirs=['.'] + INCLUDE_PATHS,
+        depends = ['python/BuildStandalone.cmake'],
         libraries=LIBS, 
         extra_compile_args=ARGS),
 ]
 
 setup(
     name='camel-kenlm',
-    version='2023.3.17.2',
+    version='2024.1.30',
     url='https://github.com/CAMeL-Lab/camel-kenlm',
     ext_modules=ext_modules,
     cmdclass={"build_ext": build_ext},
     include_package_data=True,
 )
```

### Comparing `camel-kenlm-2023.3.17.2/util/CMakeLists.txt` & `camel-kenlm-2024.1.30/util/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/bit_packing.cc` & `camel-kenlm-2024.1.30/util/bit_packing.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/bit_packing.hh` & `camel-kenlm-2024.1.30/util/bit_packing.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/bit_packing_test.cc` & `camel-kenlm-2024.1.30/util/bit_packing_test.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/cat_compressed_main.cc` & `camel-kenlm-2024.1.30/util/cat_compressed_main.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/double-conversion/CMakeLists.txt` & `camel-kenlm-2024.1.30/util/double-conversion/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/double-conversion/LICENSE` & `camel-kenlm-2024.1.30/util/double-conversion/LICENSE`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/double-conversion/bignum-dtoa.cc` & `camel-kenlm-2024.1.30/util/double-conversion/bignum-dtoa.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/double-conversion/bignum-dtoa.h` & `camel-kenlm-2024.1.30/util/double-conversion/bignum-dtoa.h`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/double-conversion/bignum.cc` & `camel-kenlm-2024.1.30/util/double-conversion/bignum.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/double-conversion/bignum.h` & `camel-kenlm-2024.1.30/util/double-conversion/bignum.h`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/double-conversion/cached-powers.cc` & `camel-kenlm-2024.1.30/util/double-conversion/cached-powers.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/double-conversion/cached-powers.h` & `camel-kenlm-2024.1.30/util/double-conversion/cached-powers.h`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/double-conversion/diy-fp.h` & `camel-kenlm-2024.1.30/util/double-conversion/diy-fp.h`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/double-conversion/double-conversion.h` & `camel-kenlm-2024.1.30/util/double-conversion/double-conversion.h`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/double-conversion/double-to-string.cc` & `camel-kenlm-2024.1.30/util/double-conversion/double-to-string.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/double-conversion/double-to-string.h` & `camel-kenlm-2024.1.30/util/double-conversion/double-to-string.h`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/double-conversion/fast-dtoa.cc` & `camel-kenlm-2024.1.30/util/double-conversion/fast-dtoa.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/double-conversion/fast-dtoa.h` & `camel-kenlm-2024.1.30/util/double-conversion/fast-dtoa.h`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/double-conversion/fixed-dtoa.cc` & `camel-kenlm-2024.1.30/util/double-conversion/fixed-dtoa.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/double-conversion/fixed-dtoa.h` & `camel-kenlm-2024.1.30/util/double-conversion/fixed-dtoa.h`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/double-conversion/ieee.h` & `camel-kenlm-2024.1.30/util/double-conversion/ieee.h`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/double-conversion/string-to-double.cc` & `camel-kenlm-2024.1.30/util/double-conversion/string-to-double.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/double-conversion/string-to-double.h` & `camel-kenlm-2024.1.30/util/double-conversion/string-to-double.h`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/double-conversion/strtod.cc` & `camel-kenlm-2024.1.30/util/double-conversion/strtod.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/double-conversion/strtod.h` & `camel-kenlm-2024.1.30/util/double-conversion/strtod.h`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/double-conversion/utils.h` & `camel-kenlm-2024.1.30/util/double-conversion/utils.h`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/ersatz_progress.cc` & `camel-kenlm-2024.1.30/util/ersatz_progress.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/ersatz_progress.hh` & `camel-kenlm-2024.1.30/util/ersatz_progress.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/exception.cc` & `camel-kenlm-2024.1.30/util/exception.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/exception.hh` & `camel-kenlm-2024.1.30/util/exception.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/fake_ostream.hh` & `camel-kenlm-2024.1.30/util/fake_ostream.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/file.cc` & `camel-kenlm-2024.1.30/util/file.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/file.hh` & `camel-kenlm-2024.1.30/util/file.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/file_piece.cc` & `camel-kenlm-2024.1.30/util/file_piece.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/file_piece.hh` & `camel-kenlm-2024.1.30/util/file_piece.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/file_piece_test.cc` & `camel-kenlm-2024.1.30/util/file_piece_test.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/file_stream.hh` & `camel-kenlm-2024.1.30/util/file_stream.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/fixed_array.hh` & `camel-kenlm-2024.1.30/util/fixed_array.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/float_to_string.cc` & `camel-kenlm-2024.1.30/util/float_to_string.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/float_to_string.hh` & `camel-kenlm-2024.1.30/util/float_to_string.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/getopt.c` & `camel-kenlm-2024.1.30/util/getopt.c`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/integer_to_string.cc` & `camel-kenlm-2024.1.30/util/integer_to_string.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/integer_to_string.hh` & `camel-kenlm-2024.1.30/util/integer_to_string.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/integer_to_string_test.cc` & `camel-kenlm-2024.1.30/util/integer_to_string_test.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/joint_sort.hh` & `camel-kenlm-2024.1.30/util/joint_sort.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/joint_sort_test.cc` & `camel-kenlm-2024.1.30/util/joint_sort_test.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/mmap.cc` & `camel-kenlm-2024.1.30/util/mmap.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/mmap.hh` & `camel-kenlm-2024.1.30/util/mmap.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/multi_intersection.hh` & `camel-kenlm-2024.1.30/util/multi_intersection.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/multi_intersection_test.cc` & `camel-kenlm-2024.1.30/util/multi_intersection_test.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/murmur_hash.cc` & `camel-kenlm-2024.1.30/util/murmur_hash.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/murmur_hash.hh` & `camel-kenlm-2024.1.30/util/murmur_hash.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/parallel_read.cc` & `camel-kenlm-2024.1.30/util/parallel_read.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/pcqueue.hh` & `camel-kenlm-2024.1.30/util/pcqueue.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/pool.cc` & `camel-kenlm-2024.1.30/util/pool.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/pool.hh` & `camel-kenlm-2024.1.30/util/pool.hh`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #ifndef UTIL_POOL_H
 #define UTIL_POOL_H
 
+#include <algorithm>
 #include <cassert>
 #include <cstring>
 #include <vector>
 
 #include <stdint.h>
 
 namespace util {
```

### Comparing `camel-kenlm-2023.3.17.2/util/probing_hash_table.hh` & `camel-kenlm-2024.1.30/util/probing_hash_table.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/probing_hash_table_benchmark_main.cc` & `camel-kenlm-2024.1.30/util/probing_hash_table_benchmark_main.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/probing_hash_table_test.cc` & `camel-kenlm-2024.1.30/util/probing_hash_table_test.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/proxy_iterator.hh` & `camel-kenlm-2024.1.30/util/proxy_iterator.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/read_compressed.cc` & `camel-kenlm-2024.1.30/util/read_compressed.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/read_compressed.hh` & `camel-kenlm-2024.1.30/util/read_compressed.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/read_compressed_test.cc` & `camel-kenlm-2024.1.30/util/read_compressed_test.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/scoped.cc` & `camel-kenlm-2024.1.30/util/scoped.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/scoped.hh` & `camel-kenlm-2024.1.30/util/scoped.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/sized_iterator.hh` & `camel-kenlm-2024.1.30/util/sized_iterator.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/sized_iterator_test.cc` & `camel-kenlm-2024.1.30/util/sized_iterator_test.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/sorted_uniform.hh` & `camel-kenlm-2024.1.30/util/sorted_uniform.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/sorted_uniform_test.cc` & `camel-kenlm-2024.1.30/util/sorted_uniform_test.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/spaces.cc` & `camel-kenlm-2024.1.30/util/spaces.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/stream/CMakeLists.txt` & `camel-kenlm-2024.1.30/util/stream/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/stream/block.hh` & `camel-kenlm-2024.1.30/util/stream/block.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/stream/chain.cc` & `camel-kenlm-2024.1.30/util/stream/chain.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/stream/chain.hh` & `camel-kenlm-2024.1.30/util/stream/chain.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/stream/config.hh` & `camel-kenlm-2024.1.30/util/stream/config.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/stream/io.cc` & `camel-kenlm-2024.1.30/util/stream/io.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/stream/io.hh` & `camel-kenlm-2024.1.30/util/stream/io.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/stream/io_test.cc` & `camel-kenlm-2024.1.30/util/stream/io_test.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/stream/line_input.cc` & `camel-kenlm-2024.1.30/util/stream/line_input.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/stream/line_input.hh` & `camel-kenlm-2024.1.30/util/stream/line_input.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/stream/multi_progress.cc` & `camel-kenlm-2024.1.30/util/stream/multi_progress.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/stream/multi_progress.hh` & `camel-kenlm-2024.1.30/util/stream/multi_progress.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/stream/multi_stream.hh` & `camel-kenlm-2024.1.30/util/stream/multi_stream.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/stream/rewindable_stream.cc` & `camel-kenlm-2024.1.30/util/stream/rewindable_stream.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/stream/rewindable_stream.hh` & `camel-kenlm-2024.1.30/util/stream/rewindable_stream.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/stream/rewindable_stream_test.cc` & `camel-kenlm-2024.1.30/util/stream/rewindable_stream_test.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/stream/sort.hh` & `camel-kenlm-2024.1.30/util/stream/sort.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/stream/sort_test.cc` & `camel-kenlm-2024.1.30/util/stream/sort_test.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/stream/stream.hh` & `camel-kenlm-2024.1.30/util/stream/stream.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/stream/stream_test.cc` & `camel-kenlm-2024.1.30/util/stream/stream_test.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/stream/typed_stream.hh` & `camel-kenlm-2024.1.30/util/stream/typed_stream.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/string_piece.cc` & `camel-kenlm-2024.1.30/util/string_piece.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/string_piece.hh` & `camel-kenlm-2024.1.30/util/string_piece.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/string_piece_hash.hh` & `camel-kenlm-2024.1.30/util/string_piece_hash.hh`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #ifndef UTIL_STRING_PIECE_HASH_H
 #define UTIL_STRING_PIECE_HASH_H
 
+#include <functional>
 #include "have.hh"
 #include "string_piece.hh"
 
 #include <boost/functional/hash.hpp>
 #include <boost/version.hpp>
 
 #ifdef HAVE_ICU
```

### Comparing `camel-kenlm-2023.3.17.2/util/string_stream.hh` & `camel-kenlm-2024.1.30/util/string_stream.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/string_stream_test.cc` & `camel-kenlm-2024.1.30/util/string_stream_test.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/thread_pool.hh` & `camel-kenlm-2024.1.30/util/thread_pool.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/tokenize_piece.hh` & `camel-kenlm-2024.1.30/util/tokenize_piece.hh`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/tokenize_piece_test.cc` & `camel-kenlm-2024.1.30/util/tokenize_piece_test.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/usage.cc` & `camel-kenlm-2024.1.30/util/usage.cc`

 * *Files identical despite different names*

### Comparing `camel-kenlm-2023.3.17.2/util/usage.hh` & `camel-kenlm-2024.1.30/util/usage.hh`

 * *Files identical despite different names*

