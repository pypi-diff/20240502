# Comparing `tmp/sosap-0.1.0.tar.gz` & `tmp/sosap-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sosap-0.1.0.tar", last modified: Thu May  2 02:23:20 2024, max compression
+gzip compressed data, was "sosap-0.1.1.tar", last modified: Thu May  2 02:40:44 2024, max compression
```

## Comparing `sosap-0.1.0.tar` & `sosap-0.1.1.tar`

### file list

```diff
@@ -1,31 +1,156 @@
-drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2024-05-02 02:23:20.312779 sosap-0.1.0/
--rw-r--r--   0 seanghay   (501) staff       (20)     1095 2024-05-02 02:14:09.000000 sosap-0.1.0/LICENSE
--rw-r--r--   0 seanghay   (501) staff       (20)     1058 2024-05-02 02:23:20.312576 sosap-0.1.0/PKG-INFO
--rw-r--r--   0 seanghay   (501) staff       (20)      453 2024-05-02 02:14:09.000000 sosap-0.1.0/README.md
--rw-r--r--   0 seanghay   (501) staff       (20)      771 2024-05-02 02:23:12.000000 sosap-0.1.0/pyproject.toml
--rw-r--r--   0 seanghay   (501) staff       (20)       38 2024-05-02 02:23:20.312819 sosap-0.1.0/setup.cfg
--rw-r--r--   0 seanghay   (501) staff       (20)     1005 2024-05-02 02:16:54.000000 sosap-0.1.0/setup.py
-drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2024-05-02 02:23:20.310332 sosap-0.1.0/src/
-drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2024-05-02 02:23:20.309538 sosap-0.1.0/src/Phonetisaurus/
-drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2024-05-02 02:23:20.310458 sosap-0.1.0/src/Phonetisaurus/lib/
--rw-r--r--   0 seanghay   (501) staff       (20)     8616 2024-05-02 02:14:09.000000 sosap-0.1.0/src/Phonetisaurus/lib/util.cc
--rw-r--r--   0 seanghay   (501) staff       (20)      599 2024-05-02 02:14:09.000000 sosap-0.1.0/src/core.pyx
-drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2024-05-02 02:23:20.309657 sosap-0.1.0/src/openfst/
-drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2024-05-02 02:23:20.311675 sosap-0.1.0/src/openfst/lib/
--rw-r--r--   0 seanghay   (501) staff       (20)      814 2024-05-02 02:14:09.000000 sosap-0.1.0/src/openfst/lib/compat.cc
--rw-r--r--   0 seanghay   (501) staff       (20)     4819 2024-05-02 02:14:09.000000 sosap-0.1.0/src/openfst/lib/flags.cc
--rw-r--r--   0 seanghay   (501) staff       (20)     1231 2024-05-02 02:14:09.000000 sosap-0.1.0/src/openfst/lib/fst-types.cc
--rw-r--r--   0 seanghay   (501) staff       (20)     4841 2024-05-02 02:14:09.000000 sosap-0.1.0/src/openfst/lib/fst.cc
--rw-r--r--   0 seanghay   (501) staff       (20)     4136 2024-05-02 02:14:09.000000 sosap-0.1.0/src/openfst/lib/mapped-file.cc
--rw-r--r--   0 seanghay   (501) staff       (20)    17562 2024-05-02 02:14:09.000000 sosap-0.1.0/src/openfst/lib/properties.cc
--rw-r--r--   0 seanghay   (501) staff       (20)     4193 2024-05-02 02:14:09.000000 sosap-0.1.0/src/openfst/lib/symbol-table-ops.cc
--rw-r--r--   0 seanghay   (501) staff       (20)    11312 2024-05-02 02:14:09.000000 sosap-0.1.0/src/openfst/lib/symbol-table.cc
--rw-r--r--   0 seanghay   (501) staff       (20)     2740 2024-05-02 02:14:09.000000 sosap-0.1.0/src/openfst/lib/util.cc
--rw-r--r--   0 seanghay   (501) staff       (20)     3929 2024-05-02 02:14:09.000000 sosap-0.1.0/src/openfst/lib/weight.cc
-drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2024-05-02 02:23:20.311786 sosap-0.1.0/src/sosap/
--rw-r--r--   0 seanghay   (501) staff       (20)       32 2024-05-02 02:14:09.000000 sosap-0.1.0/src/sosap/__init__.py
-drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2024-05-02 02:23:20.312375 sosap-0.1.0/src/sosap.egg-info/
--rw-r--r--   0 seanghay   (501) staff       (20)     1058 2024-05-02 02:23:20.000000 sosap-0.1.0/src/sosap.egg-info/PKG-INFO
--rw-r--r--   0 seanghay   (501) staff       (20)      520 2024-05-02 02:23:20.000000 sosap-0.1.0/src/sosap.egg-info/SOURCES.txt
--rw-r--r--   0 seanghay   (501) staff       (20)        1 2024-05-02 02:23:20.000000 sosap-0.1.0/src/sosap.egg-info/dependency_links.txt
--rw-r--r--   0 seanghay   (501) staff       (20)       43 2024-05-02 02:23:20.000000 sosap-0.1.0/src/sosap.egg-info/top_level.txt
+drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2024-05-02 02:40:44.235731 sosap-0.1.1/
+-rw-r--r--   0 seanghay   (501) staff       (20)     1095 2024-05-02 02:14:09.000000 sosap-0.1.1/LICENSE
+-rw-r--r--   0 seanghay   (501) staff       (20)     1058 2024-05-02 02:40:44.235504 sosap-0.1.1/PKG-INFO
+-rw-r--r--   0 seanghay   (501) staff       (20)      453 2024-05-02 02:14:09.000000 sosap-0.1.1/README.md
+-rw-r--r--   0 seanghay   (501) staff       (20)      770 2024-05-02 02:40:28.000000 sosap-0.1.1/pyproject.toml
+-rw-r--r--   0 seanghay   (501) staff       (20)       38 2024-05-02 02:40:44.235913 sosap-0.1.1/setup.cfg
+-rw-r--r--   0 seanghay   (501) staff       (20)     1077 2024-05-02 02:40:11.000000 sosap-0.1.1/setup.py
+drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2024-05-02 02:40:44.216828 sosap-0.1.1/src/
+drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2024-05-02 02:40:44.215798 sosap-0.1.1/src/Phonetisaurus/
+drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2024-05-02 02:40:44.215593 sosap-0.1.1/src/Phonetisaurus/3rdparty/
+drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2024-05-02 02:40:44.216939 sosap-0.1.1/src/Phonetisaurus/3rdparty/utfcpp/
+drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2024-05-02 02:40:44.217423 sosap-0.1.1/src/Phonetisaurus/3rdparty/utfcpp/utf8/
+-rw-r--r--   0 seanghay   (501) staff       (20)    11960 2024-05-02 02:14:09.000000 sosap-0.1.1/src/Phonetisaurus/3rdparty/utfcpp/utf8/checked.h
+-rwxr-xr-x   0 seanghay   (501) staff       (20)    11769 2024-05-02 02:14:09.000000 sosap-0.1.1/src/Phonetisaurus/3rdparty/utfcpp/utf8/core.h
+-rwxr-xr-x   0 seanghay   (501) staff       (20)     8640 2024-05-02 02:14:09.000000 sosap-0.1.1/src/Phonetisaurus/3rdparty/utfcpp/utf8/unchecked.h
+-rw-r--r--   0 seanghay   (501) staff       (20)     1521 2024-05-02 02:14:09.000000 sosap-0.1.1/src/Phonetisaurus/3rdparty/utfcpp/utf8.h
+drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2024-05-02 02:40:44.219030 sosap-0.1.1/src/Phonetisaurus/include/
+-rw-r--r--   0 seanghay   (501) staff       (20)    12608 2024-05-02 02:14:09.000000 sosap-0.1.1/src/Phonetisaurus/include/ARPA2WFST.h
+-rw-r--r--   0 seanghay   (501) staff       (20)     2752 2024-05-02 02:14:09.000000 sosap-0.1.1/src/Phonetisaurus/include/LatticePruner.h
+-rw-r--r--   0 seanghay   (501) staff       (20)     5322 2024-05-02 02:14:09.000000 sosap-0.1.1/src/Phonetisaurus/include/LegacyRnnLMDecodable.h
+-rw-r--r--   0 seanghay   (501) staff       (20)     5394 2024-05-02 02:14:09.000000 sosap-0.1.1/src/Phonetisaurus/include/LegacyRnnLMHash.h
+-rw-r--r--   0 seanghay   (501) staff       (20)     2257 2024-05-02 02:14:09.000000 sosap-0.1.1/src/Phonetisaurus/include/LegacyRnnLMReader.h
+-rw-r--r--   0 seanghay   (501) staff       (20)     5364 2024-05-02 02:14:09.000000 sosap-0.1.1/src/Phonetisaurus/include/M2MFstAligner.h
+-rw-r--r--   0 seanghay   (501) staff       (20)    14648 2024-05-02 02:14:09.000000 sosap-0.1.1/src/Phonetisaurus/include/PhonetisaurusRex.h
+-rw-r--r--   0 seanghay   (501) staff       (20)     7286 2024-05-02 02:14:09.000000 sosap-0.1.1/src/Phonetisaurus/include/PhonetisaurusScript.h
+-rw-r--r--   0 seanghay   (501) staff       (20)     9986 2024-05-02 02:14:09.000000 sosap-0.1.1/src/Phonetisaurus/include/RnnLMDecoder.h
+-rw-r--r--   0 seanghay   (501) staff       (20)     4859 2024-05-02 02:14:09.000000 sosap-0.1.1/src/Phonetisaurus/include/RnnLMPy.h
+-rw-r--r--   0 seanghay   (501) staff       (20)     2492 2024-05-02 02:14:09.000000 sosap-0.1.1/src/Phonetisaurus/include/util.h
+drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2024-05-02 02:40:44.219123 sosap-0.1.1/src/Phonetisaurus/lib/
+-rw-r--r--   0 seanghay   (501) staff       (20)     8616 2024-05-02 02:14:09.000000 sosap-0.1.1/src/Phonetisaurus/lib/util.cc
+-rw-r--r--   0 seanghay   (501) staff       (20)      599 2024-05-02 02:14:09.000000 sosap-0.1.1/src/core.pyx
+drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2024-05-02 02:40:44.216017 sosap-0.1.1/src/openfst/
+drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2024-05-02 02:40:44.215958 sosap-0.1.1/src/openfst/include/
+drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2024-05-02 02:40:44.232441 sosap-0.1.1/src/openfst/include/fst/
+-rw-r--r--   0 seanghay   (501) staff       (20)    29524 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/accumulator.h
+-rw-r--r--   0 seanghay   (501) staff       (20)     7442 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/add-on.h
+-rw-r--r--   0 seanghay   (501) staff       (20)     6405 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/arc-arena.h
+-rw-r--r--   0 seanghay   (501) staff       (20)    39401 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/arc-map.h
+-rw-r--r--   0 seanghay   (501) staff       (20)     8353 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/arc.h
+-rw-r--r--   0 seanghay   (501) staff       (20)     2314 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/arcfilter.h
+-rw-r--r--   0 seanghay   (501) staff       (20)     6587 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/arcsort.h
+-rw-r--r--   0 seanghay   (501) staff       (20)    15136 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/bi-table.h
+-rw-r--r--   0 seanghay   (501) staff       (20)    42957 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/cache.h
+-rw-r--r--   0 seanghay   (501) staff       (20)     4269 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/closure.h
+-rw-r--r--   0 seanghay   (501) staff       (20)    52849 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/compact-fst.h
+-rw-r--r--   0 seanghay   (501) staff       (20)     2749 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/compat.h
+-rw-r--r--   0 seanghay   (501) staff       (20)     7726 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/complement.h
+-rw-r--r--   0 seanghay   (501) staff       (20)    19892 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/compose-filter.h
+-rw-r--r--   0 seanghay   (501) staff       (20)    39087 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/compose.h
+-rw-r--r--   0 seanghay   (501) staff       (20)     7285 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/concat.h
+-rw-r--r--   0 seanghay   (501) staff       (20)      414 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/config.h
+-rw-r--r--   0 seanghay   (501) staff       (20)     9916 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/connect.h
+-rw-r--r--   0 seanghay   (501) staff       (20)    16266 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/const-fst.h
+-rw-r--r--   0 seanghay   (501) staff       (20)    40410 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/determinize.h
+-rw-r--r--   0 seanghay   (501) staff       (20)     6673 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/dfs-visit.h
+-rw-r--r--   0 seanghay   (501) staff       (20)     6964 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/difference.h
+-rw-r--r--   0 seanghay   (501) staff       (20)    20433 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/disambiguate.h
+-rw-r--r--   0 seanghay   (501) staff       (20)    27698 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/edit-fst.h
+-rw-r--r--   0 seanghay   (501) staff       (20)    17732 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/encode.h
+-rw-r--r--   0 seanghay   (501) staff       (20)     2111 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/epsnormalize.h
+-rw-r--r--   0 seanghay   (501) staff       (20)     6077 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/equal.h
+-rw-r--r--   0 seanghay   (501) staff       (20)     8823 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/equivalent.h
+-rw-r--r--   0 seanghay   (501) staff       (20)     5394 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/expanded-fst.h
+-rw-r--r--   0 seanghay   (501) staff       (20)     4511 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/expectation-weight.h
+-rw-r--r--   0 seanghay   (501) staff       (20)    16699 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/factor-weight.h
+-rw-r--r--   0 seanghay   (501) staff       (20)     4889 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/filter-state.h
+-rw-r--r--   0 seanghay   (501) staff       (20)     6664 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/flags.h
+-rw-r--r--   0 seanghay   (501) staff       (20)    28674 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/float-weight.h
+-rw-r--r--   0 seanghay   (501) staff       (20)     5232 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/fst-decl.h
+-rw-r--r--   0 seanghay   (501) staff       (20)    30981 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/fst.h
+-rw-r--r--   0 seanghay   (501) staff       (20)     3917 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/fstlib.h
+-rw-r--r--   0 seanghay   (501) staff       (20)     3709 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/generic-register.h
+-rw-r--r--   0 seanghay   (501) staff       (20)     4555 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/heap.h
+-rw-r--r--   0 seanghay   (501) staff       (20)     4574 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/icu.h
+-rw-r--r--   0 seanghay   (501) staff       (20)     5737 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/intersect.h
+-rw-r--r--   0 seanghay   (501) staff       (20)    12110 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/interval-set.h
+-rw-r--r--   0 seanghay   (501) staff       (20)     3893 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/invert.h
+-rw-r--r--   0 seanghay   (501) staff       (20)     5804 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/isomorphic.h
+-rw-r--r--   0 seanghay   (501) staff       (20)    18965 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/label-reachable.h
+-rw-r--r--   0 seanghay   (501) staff       (20)     5894 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/lexicographic-weight.h
+-rw-r--r--   0 seanghay   (501) staff       (20)     1540 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/lock.h
+-rw-r--r--   0 seanghay   (501) staff       (20)     2254 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/log.h
+-rw-r--r--   0 seanghay   (501) staff       (20)    23312 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/lookahead-filter.h
+-rw-r--r--   0 seanghay   (501) staff       (20)    28489 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/lookahead-matcher.h
+-rw-r--r--   0 seanghay   (501) staff       (20)     2895 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/map.h
+-rw-r--r--   0 seanghay   (501) staff       (20)     3037 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/mapped-file.h
+-rw-r--r--   0 seanghay   (501) staff       (20)    11433 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/matcher-fst.h
+-rw-r--r--   0 seanghay   (501) staff       (20)    51793 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/matcher.h
+-rw-r--r--   0 seanghay   (501) staff       (20)    12918 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/memory.h
+-rw-r--r--   0 seanghay   (501) staff       (20)    21100 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/minimize.h
+-rw-r--r--   0 seanghay   (501) staff       (20)    12012 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/mutable-fst.h
+-rw-r--r--   0 seanghay   (501) staff       (20)     4151 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/pair-weight.h
+-rw-r--r--   0 seanghay   (501) staff       (20)    12588 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/partition.h
+-rw-r--r--   0 seanghay   (501) staff       (20)     4740 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/power-weight.h
+-rw-r--r--   0 seanghay   (501) staff       (20)     3309 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/product-weight.h
+-rw-r--r--   0 seanghay   (501) staff       (20)     4563 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/project.h
+-rw-r--r--   0 seanghay   (501) staff       (20)    19044 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/properties.h
+-rw-r--r--   0 seanghay   (501) staff       (20)    13109 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/prune.h
+-rw-r--r--   0 seanghay   (501) staff       (20)     6039 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/push.h
+-rw-r--r--   0 seanghay   (501) staff       (20)    29804 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/queue.h
+-rw-r--r--   0 seanghay   (501) staff       (20)     4145 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/randequivalent.h
+-rw-r--r--   0 seanghay   (501) staff       (20)    25791 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/randgen.h
+-rw-r--r--   0 seanghay   (501) staff       (20)    10110 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/rational.h
+-rw-r--r--   0 seanghay   (501) staff       (20)     3298 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/register.h
+-rw-r--r--   0 seanghay   (501) staff       (20)    15947 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/relabel.h
+-rw-r--r--   0 seanghay   (501) staff       (20)    22753 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/replace-util.h
+-rw-r--r--   0 seanghay   (501) staff       (20)    56136 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/replace.h
+-rw-r--r--   0 seanghay   (501) staff       (20)     4243 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/reverse.h
+-rw-r--r--   0 seanghay   (501) staff       (20)     4877 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/reweight.h
+-rw-r--r--   0 seanghay   (501) staff       (20)    18370 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/rmepsilon.h
+-rw-r--r--   0 seanghay   (501) staff       (20)     2536 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/rmfinalepsilon.h
+-rw-r--r--   0 seanghay   (501) staff       (20)    18358 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/set-weight.h
+-rw-r--r--   0 seanghay   (501) staff       (20)    13204 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/shortest-distance.h
+-rw-r--r--   0 seanghay   (501) staff       (20)    23200 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/shortest-path.h
+-rw-r--r--   0 seanghay   (501) staff       (20)    13538 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/signed-log-weight.h
+-rw-r--r--   0 seanghay   (501) staff       (20)     6706 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/sparse-power-weight.h
+-rw-r--r--   0 seanghay   (501) staff       (20)    12794 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/sparse-tuple-weight.h
+-rw-r--r--   0 seanghay   (501) staff       (20)    18304 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/state-map.h
+-rw-r--r--   0 seanghay   (501) staff       (20)     7175 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/state-reachable.h
+-rw-r--r--   0 seanghay   (501) staff       (20)    16830 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/state-table.h
+-rw-r--r--   0 seanghay   (501) staff       (20)     2192 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/statesort.h
+-rw-r--r--   0 seanghay   (501) staff       (20)    25921 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/string-weight.h
+-rw-r--r--   0 seanghay   (501) staff       (20)     9416 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/string.h
+-rw-r--r--   0 seanghay   (501) staff       (20)     3040 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/symbol-table-ops.h
+-rw-r--r--   0 seanghay   (501) staff       (20)    14016 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/symbol-table.h
+-rw-r--r--   0 seanghay   (501) staff       (20)    13573 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/synchronize.h
+-rw-r--r--   0 seanghay   (501) staff       (20)     9443 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/test-properties.h
+-rw-r--r--   0 seanghay   (501) staff       (20)     2580 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/topsort.h
+-rw-r--r--   0 seanghay   (501) staff       (20)     4140 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/tuple-weight.h
+-rw-r--r--   0 seanghay   (501) staff       (20)     1082 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/types.h
+-rw-r--r--   0 seanghay   (501) staff       (20)     2621 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/union-find.h
+-rw-r--r--   0 seanghay   (501) staff       (20)    14641 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/union-weight.h
+-rw-r--r--   0 seanghay   (501) staff       (20)     5098 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/union.h
+-rw-r--r--   0 seanghay   (501) staff       (20)    12396 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/util.h
+-rw-r--r--   0 seanghay   (501) staff       (20)    24671 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/vector-fst.h
+-rw-r--r--   0 seanghay   (501) staff       (20)     3676 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/verify.h
+-rw-r--r--   0 seanghay   (501) staff       (20)     9330 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/visit.h
+-rw-r--r--   0 seanghay   (501) staff       (20)    12716 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/include/fst/weight.h
+drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2024-05-02 02:40:44.233528 sosap-0.1.1/src/openfst/lib/
+-rw-r--r--   0 seanghay   (501) staff       (20)      814 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/lib/compat.cc
+-rw-r--r--   0 seanghay   (501) staff       (20)     4819 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/lib/flags.cc
+-rw-r--r--   0 seanghay   (501) staff       (20)     1231 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/lib/fst-types.cc
+-rw-r--r--   0 seanghay   (501) staff       (20)     4841 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/lib/fst.cc
+-rw-r--r--   0 seanghay   (501) staff       (20)     4136 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/lib/mapped-file.cc
+-rw-r--r--   0 seanghay   (501) staff       (20)    17562 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/lib/properties.cc
+-rw-r--r--   0 seanghay   (501) staff       (20)     4193 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/lib/symbol-table-ops.cc
+-rw-r--r--   0 seanghay   (501) staff       (20)    11312 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/lib/symbol-table.cc
+-rw-r--r--   0 seanghay   (501) staff       (20)     2740 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/lib/util.cc
+-rw-r--r--   0 seanghay   (501) staff       (20)     3929 2024-05-02 02:14:09.000000 sosap-0.1.1/src/openfst/lib/weight.cc
+drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2024-05-02 02:40:44.233616 sosap-0.1.1/src/sosap/
+-rw-r--r--   0 seanghay   (501) staff       (20)       32 2024-05-02 02:14:09.000000 sosap-0.1.1/src/sosap/__init__.py
+drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2024-05-02 02:40:44.235196 sosap-0.1.1/src/sosap.egg-info/
+-rw-r--r--   0 seanghay   (501) staff       (20)     1058 2024-05-02 02:40:44.000000 sosap-0.1.1/src/sosap.egg-info/PKG-INFO
+-rw-r--r--   0 seanghay   (501) staff       (20)     4963 2024-05-02 02:40:44.000000 sosap-0.1.1/src/sosap.egg-info/SOURCES.txt
+-rw-r--r--   0 seanghay   (501) staff       (20)        1 2024-05-02 02:40:44.000000 sosap-0.1.1/src/sosap.egg-info/dependency_links.txt
+-rw-r--r--   0 seanghay   (501) staff       (20)       43 2024-05-02 02:40:44.000000 sosap-0.1.1/src/sosap.egg-info/top_level.txt
```

### Comparing `sosap-0.1.0/LICENSE` & `sosap-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sosap-0.1.0/PKG-INFO` & `sosap-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sosap
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python binding for Phonetisaurus
 Author-email: Seanghay Yath <seanghay.dev@gmail.com>
 Project-URL: repository, https://github.com/seanghay/sosap
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sosap-0.1.0/pyproject.toml` & `sosap-0.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "Cython"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sosap"
-version = "0.1.0"
+version = "0.1.1"
 authors = [{ name = "Seanghay Yath", email = "seanghay.dev@gmail.com" }]
 
 description = "Python binding for Phonetisaurus"
 readme = "README.md"
 requires-python = ">=3.7"
 
 classifiers = [
@@ -23,8 +23,8 @@
 [project.urls]
 repository = "https://github.com/seanghay/sosap"
 
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.packages.find]
-where = ["src"]
+where = ["src"]
```

### Comparing `sosap-0.1.0/setup.py` & `sosap-0.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 
 COMPILE_ARGS = ["-std=c++11", "-w"]
 
 if sys.platform.startswith("darwin"):
     COMPILE_ARGS.append("-stdlib=libc++")
     COMPILE_ARGS.append("-mmacosx-version-min=10.7")
-    
+
 phonetisaurus_extension = Extension(
     name="_phonetisaurus",
     sources=[
         "src/openfst/lib/compat.cc",
         "src/openfst/lib/flags.cc",
         "src/openfst/lib/fst-types.cc",
         "src/openfst/lib/fst.cc",
@@ -28,8 +28,15 @@
         "src/openfst/include",
         "src/Phonetisaurus",
         "src/Phonetisaurus/3rdparty/utfcpp",
     ],
     extra_compile_args=COMPILE_ARGS,
 )
 
-setup(ext_modules=[phonetisaurus_extension])
+setup(
+    ext_modules=[phonetisaurus_extension],
+    package_data={
+        "": [
+            "*.h",
+        ]
+    },
+)
```

### Comparing `sosap-0.1.0/src/Phonetisaurus/lib/util.cc` & `sosap-0.1.1/src/Phonetisaurus/lib/util.cc`

 * *Files identical despite different names*

### Comparing `sosap-0.1.0/src/core.pyx` & `sosap-0.1.1/src/core.pyx`

 * *Files identical despite different names*

### Comparing `sosap-0.1.0/src/openfst/lib/compat.cc` & `sosap-0.1.1/src/openfst/lib/compat.cc`

 * *Files identical despite different names*

### Comparing `sosap-0.1.0/src/openfst/lib/flags.cc` & `sosap-0.1.1/src/openfst/lib/flags.cc`

 * *Files identical despite different names*

### Comparing `sosap-0.1.0/src/openfst/lib/fst-types.cc` & `sosap-0.1.1/src/openfst/lib/fst-types.cc`

 * *Files identical despite different names*

### Comparing `sosap-0.1.0/src/openfst/lib/fst.cc` & `sosap-0.1.1/src/openfst/lib/fst.cc`

 * *Files identical despite different names*

### Comparing `sosap-0.1.0/src/openfst/lib/mapped-file.cc` & `sosap-0.1.1/src/openfst/lib/mapped-file.cc`

 * *Files identical despite different names*

### Comparing `sosap-0.1.0/src/openfst/lib/properties.cc` & `sosap-0.1.1/src/openfst/lib/properties.cc`

 * *Files identical despite different names*

### Comparing `sosap-0.1.0/src/openfst/lib/symbol-table-ops.cc` & `sosap-0.1.1/src/openfst/lib/symbol-table-ops.cc`

 * *Files identical despite different names*

### Comparing `sosap-0.1.0/src/openfst/lib/symbol-table.cc` & `sosap-0.1.1/src/openfst/lib/symbol-table.cc`

 * *Files identical despite different names*

### Comparing `sosap-0.1.0/src/openfst/lib/util.cc` & `sosap-0.1.1/src/openfst/lib/util.cc`

 * *Files identical despite different names*

### Comparing `sosap-0.1.0/src/openfst/lib/weight.cc` & `sosap-0.1.1/src/openfst/lib/weight.cc`

 * *Files identical despite different names*

### Comparing `sosap-0.1.0/src/sosap.egg-info/PKG-INFO` & `sosap-0.1.1/src/sosap.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sosap
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python binding for Phonetisaurus
 Author-email: Seanghay Yath <seanghay.dev@gmail.com>
 Project-URL: repository, https://github.com/seanghay/sosap
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```
