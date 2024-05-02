# Comparing `tmp/sosap-0.0.1.tar.gz` & `tmp/sosap-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/seanghay/phonetisaurus-js/build/dist/.tmp-k78j41kp/sosap-0.0.1.tar", last modified: Mon Dec 18 09:41:23 2023, max compression
+gzip compressed data, was "sosap-0.1.0.tar", last modified: Thu May  2 02:23:20 2024, max compression
```

## Comparing `sosap-0.0.1.tar` & `sosap-0.1.0.tar`

### file list

```diff
@@ -1,162 +1,31 @@
-drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2023-12-18 09:41:23.435777 sosap-0.0.1/
--rw-r--r--   0 seanghay   (501) staff       (20)     3498 2023-12-17 12:04:55.000000 sosap-0.0.1/.gitignore
--rw-r--r--   0 seanghay   (501) staff       (20)      897 2023-12-18 09:41:23.435278 sosap-0.0.1/PKG-INFO
--rw-r--r--   0 seanghay   (501) staff       (20)      314 2023-12-18 09:17:45.000000 sosap-0.0.1/README.md
--rw-r--r--   0 seanghay   (501) staff       (20)      842 2023-12-18 09:41:08.000000 sosap-0.0.1/pyproject.toml
--rw-r--r--   0 seanghay   (501) staff       (20)       38 2023-12-18 09:41:23.435935 sosap-0.0.1/setup.cfg
--rw-r--r--   0 seanghay   (501) staff       (20)     1005 2023-12-18 09:01:35.000000 sosap-0.0.1/setup.py
-drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2023-12-18 09:41:23.317893 sosap-0.0.1/src/
-drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2023-12-18 09:41:23.310823 sosap-0.0.1/src/Phonetisaurus/
-drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2023-12-18 09:41:23.310057 sosap-0.0.1/src/Phonetisaurus/3rdparty/
-drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2023-12-18 09:41:23.318601 sosap-0.0.1/src/Phonetisaurus/3rdparty/utfcpp/
-drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2023-12-18 09:41:23.321164 sosap-0.0.1/src/Phonetisaurus/3rdparty/utfcpp/utf8/
--rw-r--r--   0 seanghay   (501) staff       (20)    11960 2023-12-17 09:16:17.000000 sosap-0.0.1/src/Phonetisaurus/3rdparty/utfcpp/utf8/checked.h
--rwxr-xr-x   0 seanghay   (501) staff       (20)    11769 2023-12-17 09:16:17.000000 sosap-0.0.1/src/Phonetisaurus/3rdparty/utfcpp/utf8/core.h
--rwxr-xr-x   0 seanghay   (501) staff       (20)     8640 2023-12-17 09:16:17.000000 sosap-0.0.1/src/Phonetisaurus/3rdparty/utfcpp/utf8/unchecked.h
--rw-r--r--   0 seanghay   (501) staff       (20)     1521 2023-12-17 09:16:17.000000 sosap-0.0.1/src/Phonetisaurus/3rdparty/utfcpp/utf8.h
-drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2023-12-18 09:41:23.329352 sosap-0.0.1/src/Phonetisaurus/include/
--rw-r--r--   0 seanghay   (501) staff       (20)    12608 2023-12-17 09:16:17.000000 sosap-0.0.1/src/Phonetisaurus/include/ARPA2WFST.h
--rw-r--r--   0 seanghay   (501) staff       (20)     2752 2023-12-17 09:16:17.000000 sosap-0.0.1/src/Phonetisaurus/include/LatticePruner.h
--rw-r--r--   0 seanghay   (501) staff       (20)     5322 2023-12-17 09:16:17.000000 sosap-0.0.1/src/Phonetisaurus/include/LegacyRnnLMDecodable.h
--rw-r--r--   0 seanghay   (501) staff       (20)     5394 2023-12-17 09:16:17.000000 sosap-0.0.1/src/Phonetisaurus/include/LegacyRnnLMHash.h
--rw-r--r--   0 seanghay   (501) staff       (20)     2257 2023-12-17 09:16:17.000000 sosap-0.0.1/src/Phonetisaurus/include/LegacyRnnLMReader.h
--rw-r--r--   0 seanghay   (501) staff       (20)     5364 2023-12-17 09:16:17.000000 sosap-0.0.1/src/Phonetisaurus/include/M2MFstAligner.h
--rw-r--r--   0 seanghay   (501) staff       (20)    14648 2023-12-17 09:16:17.000000 sosap-0.0.1/src/Phonetisaurus/include/PhonetisaurusRex.h
--rw-r--r--   0 seanghay   (501) staff       (20)     7286 2023-12-17 09:16:17.000000 sosap-0.0.1/src/Phonetisaurus/include/PhonetisaurusScript.h
--rw-r--r--   0 seanghay   (501) staff       (20)     9986 2023-12-17 09:16:17.000000 sosap-0.0.1/src/Phonetisaurus/include/RnnLMDecoder.h
--rw-r--r--   0 seanghay   (501) staff       (20)     4859 2023-12-17 09:16:17.000000 sosap-0.0.1/src/Phonetisaurus/include/RnnLMPy.h
--rw-r--r--   0 seanghay   (501) staff       (20)     2492 2023-12-17 09:16:17.000000 sosap-0.0.1/src/Phonetisaurus/include/util.h
-drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2023-12-18 09:41:23.332575 sosap-0.0.1/src/Phonetisaurus/lib/
--rw-r--r--   0 seanghay   (501) staff       (20)     5283 2023-12-17 09:16:17.000000 sosap-0.0.1/src/Phonetisaurus/lib/LatticePruner.cc
--rw-r--r--   0 seanghay   (501) staff       (20)    21805 2023-12-17 09:16:17.000000 sosap-0.0.1/src/Phonetisaurus/lib/M2MFstAligner.cc
--rw-r--r--   0 seanghay   (501) staff       (20)     1850 2023-12-17 09:16:17.000000 sosap-0.0.1/src/Phonetisaurus/lib/feature-reader.cc
--rw-r--r--   0 seanghay   (501) staff       (20)     8616 2023-12-17 09:16:17.000000 sosap-0.0.1/src/Phonetisaurus/lib/util.cc
--rw-r--r--   0 seanghay   (501) staff       (20)   327291 2023-12-18 08:36:39.000000 sosap-0.0.1/src/core.cpp
--rw-r--r--   0 seanghay   (501) staff       (20)      599 2023-12-18 08:23:55.000000 sosap-0.0.1/src/core.pyx
-drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2023-12-18 09:41:23.311620 sosap-0.0.1/src/openfst/
-drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2023-12-18 09:41:23.311393 sosap-0.0.1/src/openfst/include/
-drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2023-12-18 09:41:23.425802 sosap-0.0.1/src/openfst/include/fst/
--rw-r--r--   0 seanghay   (501) staff       (20)    29524 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/accumulator.h
--rw-r--r--   0 seanghay   (501) staff       (20)     7442 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/add-on.h
--rw-r--r--   0 seanghay   (501) staff       (20)     6405 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/arc-arena.h
--rw-r--r--   0 seanghay   (501) staff       (20)    39401 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/arc-map.h
--rw-r--r--   0 seanghay   (501) staff       (20)     8353 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/arc.h
--rw-r--r--   0 seanghay   (501) staff       (20)     2314 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/arcfilter.h
--rw-r--r--   0 seanghay   (501) staff       (20)     6587 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/arcsort.h
--rw-r--r--   0 seanghay   (501) staff       (20)    15136 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/bi-table.h
--rw-r--r--   0 seanghay   (501) staff       (20)    42957 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/cache.h
--rw-r--r--   0 seanghay   (501) staff       (20)     4269 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/closure.h
--rw-r--r--   0 seanghay   (501) staff       (20)    52849 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/compact-fst.h
--rw-r--r--   0 seanghay   (501) staff       (20)     2749 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/compat.h
--rw-r--r--   0 seanghay   (501) staff       (20)     7726 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/complement.h
--rw-r--r--   0 seanghay   (501) staff       (20)    19892 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/compose-filter.h
--rw-r--r--   0 seanghay   (501) staff       (20)    39087 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/compose.h
--rw-r--r--   0 seanghay   (501) staff       (20)     7285 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/concat.h
--rw-r--r--   0 seanghay   (501) staff       (20)      414 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/config.h
--rw-r--r--   0 seanghay   (501) staff       (20)      333 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/config.h.in
--rw-r--r--   0 seanghay   (501) staff       (20)     9916 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/connect.h
--rw-r--r--   0 seanghay   (501) staff       (20)    16266 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/const-fst.h
--rw-r--r--   0 seanghay   (501) staff       (20)    40410 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/determinize.h
--rw-r--r--   0 seanghay   (501) staff       (20)     6673 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/dfs-visit.h
--rw-r--r--   0 seanghay   (501) staff       (20)     6964 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/difference.h
--rw-r--r--   0 seanghay   (501) staff       (20)    20433 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/disambiguate.h
--rw-r--r--   0 seanghay   (501) staff       (20)    27698 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/edit-fst.h
--rw-r--r--   0 seanghay   (501) staff       (20)    17732 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/encode.h
--rw-r--r--   0 seanghay   (501) staff       (20)     2111 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/epsnormalize.h
--rw-r--r--   0 seanghay   (501) staff       (20)     6077 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/equal.h
--rw-r--r--   0 seanghay   (501) staff       (20)     8823 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/equivalent.h
--rw-r--r--   0 seanghay   (501) staff       (20)     5394 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/expanded-fst.h
--rw-r--r--   0 seanghay   (501) staff       (20)     4511 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/expectation-weight.h
--rw-r--r--   0 seanghay   (501) staff       (20)    16699 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/factor-weight.h
--rw-r--r--   0 seanghay   (501) staff       (20)     4889 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/filter-state.h
--rw-r--r--   0 seanghay   (501) staff       (20)     6664 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/flags.h
--rw-r--r--   0 seanghay   (501) staff       (20)    28674 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/float-weight.h
--rw-r--r--   0 seanghay   (501) staff       (20)     5232 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/fst-decl.h
--rw-r--r--   0 seanghay   (501) staff       (20)    30981 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/fst.h
--rw-r--r--   0 seanghay   (501) staff       (20)     3917 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/fstlib.h
--rw-r--r--   0 seanghay   (501) staff       (20)     3709 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/generic-register.h
--rw-r--r--   0 seanghay   (501) staff       (20)     4555 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/heap.h
--rw-r--r--   0 seanghay   (501) staff       (20)     4574 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/icu.h
--rw-r--r--   0 seanghay   (501) staff       (20)     5737 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/intersect.h
--rw-r--r--   0 seanghay   (501) staff       (20)    12110 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/interval-set.h
--rw-r--r--   0 seanghay   (501) staff       (20)     3893 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/invert.h
--rw-r--r--   0 seanghay   (501) staff       (20)     5804 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/isomorphic.h
--rw-r--r--   0 seanghay   (501) staff       (20)    18965 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/label-reachable.h
--rw-r--r--   0 seanghay   (501) staff       (20)     5894 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/lexicographic-weight.h
--rw-r--r--   0 seanghay   (501) staff       (20)     1540 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/lock.h
--rw-r--r--   0 seanghay   (501) staff       (20)     2254 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/log.h
--rw-r--r--   0 seanghay   (501) staff       (20)    23312 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/lookahead-filter.h
--rw-r--r--   0 seanghay   (501) staff       (20)    28489 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/lookahead-matcher.h
--rw-r--r--   0 seanghay   (501) staff       (20)     2895 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/map.h
--rw-r--r--   0 seanghay   (501) staff       (20)     3037 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/mapped-file.h
--rw-r--r--   0 seanghay   (501) staff       (20)    11433 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/matcher-fst.h
--rw-r--r--   0 seanghay   (501) staff       (20)    51793 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/matcher.h
--rw-r--r--   0 seanghay   (501) staff       (20)    12918 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/memory.h
--rw-r--r--   0 seanghay   (501) staff       (20)    21100 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/minimize.h
--rw-r--r--   0 seanghay   (501) staff       (20)    12012 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/mutable-fst.h
--rw-r--r--   0 seanghay   (501) staff       (20)     4151 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/pair-weight.h
--rw-r--r--   0 seanghay   (501) staff       (20)    12588 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/partition.h
--rw-r--r--   0 seanghay   (501) staff       (20)     4740 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/power-weight.h
--rw-r--r--   0 seanghay   (501) staff       (20)     3309 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/product-weight.h
--rw-r--r--   0 seanghay   (501) staff       (20)     4563 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/project.h
--rw-r--r--   0 seanghay   (501) staff       (20)    19044 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/properties.h
--rw-r--r--   0 seanghay   (501) staff       (20)    13109 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/prune.h
--rw-r--r--   0 seanghay   (501) staff       (20)     6039 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/push.h
--rw-r--r--   0 seanghay   (501) staff       (20)    29804 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/queue.h
--rw-r--r--   0 seanghay   (501) staff       (20)     4145 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/randequivalent.h
--rw-r--r--   0 seanghay   (501) staff       (20)    25791 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/randgen.h
--rw-r--r--   0 seanghay   (501) staff       (20)    10110 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/rational.h
--rw-r--r--   0 seanghay   (501) staff       (20)     3298 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/register.h
--rw-r--r--   0 seanghay   (501) staff       (20)    15947 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/relabel.h
--rw-r--r--   0 seanghay   (501) staff       (20)    22753 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/replace-util.h
--rw-r--r--   0 seanghay   (501) staff       (20)    56136 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/replace.h
--rw-r--r--   0 seanghay   (501) staff       (20)     4243 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/reverse.h
--rw-r--r--   0 seanghay   (501) staff       (20)     4877 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/reweight.h
--rw-r--r--   0 seanghay   (501) staff       (20)    18370 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/rmepsilon.h
--rw-r--r--   0 seanghay   (501) staff       (20)     2536 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/rmfinalepsilon.h
--rw-r--r--   0 seanghay   (501) staff       (20)    18358 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/set-weight.h
--rw-r--r--   0 seanghay   (501) staff       (20)    13204 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/shortest-distance.h
--rw-r--r--   0 seanghay   (501) staff       (20)    23200 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/shortest-path.h
--rw-r--r--   0 seanghay   (501) staff       (20)    13538 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/signed-log-weight.h
--rw-r--r--   0 seanghay   (501) staff       (20)     6706 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/sparse-power-weight.h
--rw-r--r--   0 seanghay   (501) staff       (20)    12794 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/sparse-tuple-weight.h
--rw-r--r--   0 seanghay   (501) staff       (20)    18304 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/state-map.h
--rw-r--r--   0 seanghay   (501) staff       (20)     7175 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/state-reachable.h
--rw-r--r--   0 seanghay   (501) staff       (20)    16830 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/state-table.h
--rw-r--r--   0 seanghay   (501) staff       (20)     2192 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/statesort.h
--rw-r--r--   0 seanghay   (501) staff       (20)    25921 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/string-weight.h
--rw-r--r--   0 seanghay   (501) staff       (20)     9416 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/string.h
--rw-r--r--   0 seanghay   (501) staff       (20)     3040 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/symbol-table-ops.h
--rw-r--r--   0 seanghay   (501) staff       (20)    14016 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/symbol-table.h
--rw-r--r--   0 seanghay   (501) staff       (20)    13573 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/synchronize.h
--rw-r--r--   0 seanghay   (501) staff       (20)     9443 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/test-properties.h
--rw-r--r--   0 seanghay   (501) staff       (20)     2580 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/topsort.h
--rw-r--r--   0 seanghay   (501) staff       (20)     4140 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/tuple-weight.h
--rw-r--r--   0 seanghay   (501) staff       (20)     1082 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/types.h
--rw-r--r--   0 seanghay   (501) staff       (20)     2621 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/union-find.h
--rw-r--r--   0 seanghay   (501) staff       (20)    14641 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/union-weight.h
--rw-r--r--   0 seanghay   (501) staff       (20)     5098 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/union.h
--rw-r--r--   0 seanghay   (501) staff       (20)    12396 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/util.h
--rw-r--r--   0 seanghay   (501) staff       (20)    24671 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/vector-fst.h
--rw-r--r--   0 seanghay   (501) staff       (20)     3676 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/verify.h
--rw-r--r--   0 seanghay   (501) staff       (20)     9330 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/visit.h
--rw-r--r--   0 seanghay   (501) staff       (20)    12716 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/include/fst/weight.h
-drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2023-12-18 09:41:23.432380 sosap-0.0.1/src/openfst/lib/
--rw-r--r--   0 seanghay   (501) staff       (20)      814 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/lib/compat.cc
--rw-r--r--   0 seanghay   (501) staff       (20)     4819 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/lib/flags.cc
--rw-r--r--   0 seanghay   (501) staff       (20)     1231 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/lib/fst-types.cc
--rw-r--r--   0 seanghay   (501) staff       (20)     4841 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/lib/fst.cc
--rw-r--r--   0 seanghay   (501) staff       (20)     4136 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/lib/mapped-file.cc
--rw-r--r--   0 seanghay   (501) staff       (20)    17562 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/lib/properties.cc
--rw-r--r--   0 seanghay   (501) staff       (20)     4193 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/lib/symbol-table-ops.cc
--rw-r--r--   0 seanghay   (501) staff       (20)    11312 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/lib/symbol-table.cc
--rw-r--r--   0 seanghay   (501) staff       (20)     2740 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/lib/util.cc
--rw-r--r--   0 seanghay   (501) staff       (20)     3929 2023-12-17 09:16:17.000000 sosap-0.0.1/src/openfst/lib/weight.cc
--rw-r--r--   0 seanghay   (501) staff       (20)      604 2023-12-17 11:54:25.000000 sosap-0.0.1/src/phonemizer.cc
-drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2023-12-18 09:41:23.433026 sosap-0.0.1/src/sosap/
--rw-r--r--   0 seanghay   (501) staff       (20)       32 2023-12-18 09:01:51.000000 sosap-0.0.1/src/sosap/__init__.py
-drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2023-12-18 09:41:23.434650 sosap-0.0.1/src/sosap.egg-info/
--rw-r--r--   0 seanghay   (501) staff       (20)      897 2023-12-18 09:41:23.000000 sosap-0.0.1/src/sosap.egg-info/PKG-INFO
--rw-r--r--   0 seanghay   (501) staff       (20)     5151 2023-12-18 09:41:23.000000 sosap-0.0.1/src/sosap.egg-info/SOURCES.txt
--rw-r--r--   0 seanghay   (501) staff       (20)        1 2023-12-18 09:41:23.000000 sosap-0.0.1/src/sosap.egg-info/dependency_links.txt
--rw-r--r--   0 seanghay   (501) staff       (20)       43 2023-12-18 09:41:23.000000 sosap-0.0.1/src/sosap.egg-info/top_level.txt
+drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2024-05-02 02:23:20.312779 sosap-0.1.0/
+-rw-r--r--   0 seanghay   (501) staff       (20)     1095 2024-05-02 02:14:09.000000 sosap-0.1.0/LICENSE
+-rw-r--r--   0 seanghay   (501) staff       (20)     1058 2024-05-02 02:23:20.312576 sosap-0.1.0/PKG-INFO
+-rw-r--r--   0 seanghay   (501) staff       (20)      453 2024-05-02 02:14:09.000000 sosap-0.1.0/README.md
+-rw-r--r--   0 seanghay   (501) staff       (20)      771 2024-05-02 02:23:12.000000 sosap-0.1.0/pyproject.toml
+-rw-r--r--   0 seanghay   (501) staff       (20)       38 2024-05-02 02:23:20.312819 sosap-0.1.0/setup.cfg
+-rw-r--r--   0 seanghay   (501) staff       (20)     1005 2024-05-02 02:16:54.000000 sosap-0.1.0/setup.py
+drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2024-05-02 02:23:20.310332 sosap-0.1.0/src/
+drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2024-05-02 02:23:20.309538 sosap-0.1.0/src/Phonetisaurus/
+drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2024-05-02 02:23:20.310458 sosap-0.1.0/src/Phonetisaurus/lib/
+-rw-r--r--   0 seanghay   (501) staff       (20)     8616 2024-05-02 02:14:09.000000 sosap-0.1.0/src/Phonetisaurus/lib/util.cc
+-rw-r--r--   0 seanghay   (501) staff       (20)      599 2024-05-02 02:14:09.000000 sosap-0.1.0/src/core.pyx
+drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2024-05-02 02:23:20.309657 sosap-0.1.0/src/openfst/
+drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2024-05-02 02:23:20.311675 sosap-0.1.0/src/openfst/lib/
+-rw-r--r--   0 seanghay   (501) staff       (20)      814 2024-05-02 02:14:09.000000 sosap-0.1.0/src/openfst/lib/compat.cc
+-rw-r--r--   0 seanghay   (501) staff       (20)     4819 2024-05-02 02:14:09.000000 sosap-0.1.0/src/openfst/lib/flags.cc
+-rw-r--r--   0 seanghay   (501) staff       (20)     1231 2024-05-02 02:14:09.000000 sosap-0.1.0/src/openfst/lib/fst-types.cc
+-rw-r--r--   0 seanghay   (501) staff       (20)     4841 2024-05-02 02:14:09.000000 sosap-0.1.0/src/openfst/lib/fst.cc
+-rw-r--r--   0 seanghay   (501) staff       (20)     4136 2024-05-02 02:14:09.000000 sosap-0.1.0/src/openfst/lib/mapped-file.cc
+-rw-r--r--   0 seanghay   (501) staff       (20)    17562 2024-05-02 02:14:09.000000 sosap-0.1.0/src/openfst/lib/properties.cc
+-rw-r--r--   0 seanghay   (501) staff       (20)     4193 2024-05-02 02:14:09.000000 sosap-0.1.0/src/openfst/lib/symbol-table-ops.cc
+-rw-r--r--   0 seanghay   (501) staff       (20)    11312 2024-05-02 02:14:09.000000 sosap-0.1.0/src/openfst/lib/symbol-table.cc
+-rw-r--r--   0 seanghay   (501) staff       (20)     2740 2024-05-02 02:14:09.000000 sosap-0.1.0/src/openfst/lib/util.cc
+-rw-r--r--   0 seanghay   (501) staff       (20)     3929 2024-05-02 02:14:09.000000 sosap-0.1.0/src/openfst/lib/weight.cc
+drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2024-05-02 02:23:20.311786 sosap-0.1.0/src/sosap/
+-rw-r--r--   0 seanghay   (501) staff       (20)       32 2024-05-02 02:14:09.000000 sosap-0.1.0/src/sosap/__init__.py
+drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2024-05-02 02:23:20.312375 sosap-0.1.0/src/sosap.egg-info/
+-rw-r--r--   0 seanghay   (501) staff       (20)     1058 2024-05-02 02:23:20.000000 sosap-0.1.0/src/sosap.egg-info/PKG-INFO
+-rw-r--r--   0 seanghay   (501) staff       (20)      520 2024-05-02 02:23:20.000000 sosap-0.1.0/src/sosap.egg-info/SOURCES.txt
+-rw-r--r--   0 seanghay   (501) staff       (20)        1 2024-05-02 02:23:20.000000 sosap-0.1.0/src/sosap.egg-info/dependency_links.txt
+-rw-r--r--   0 seanghay   (501) staff       (20)       43 2024-05-02 02:23:20.000000 sosap-0.1.0/src/sosap.egg-info/top_level.txt
```

### Comparing `sosap-0.0.1/PKG-INFO` & `sosap-0.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: sosap
-Version: 0.0.1
+Version: 0.1.0
 Summary: Python binding for Phonetisaurus
 Author-email: Seanghay Yath <seanghay.dev@gmail.com>
 Project-URL: repository, https://github.com/seanghay/sosap
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Cython
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
-## 🗣️ sosap / សូរសព្ទ
+<img width=144 src="https://github.com/seanghay/sosap/assets/15277233/25c2ae30-4dd6-4350-a387-c30353cb2a98">
 
-Python binding for Phonetisaurus
+Python binding for [Phonetisaurus](https://github.com/AdolfVonKleist/Phonetisaurus) using Cython.
 
 ### Install
 
 ```shell
 # pypi
 pip install sosap
 
@@ -29,15 +30,16 @@
 
 ### Usage
 
 ```python
 from sosap import Model
 
 model = Model("g2p.fst")
-
 model.phoneticize("hello")
 ```
 
+---
 
 ### License
 
-MIT
+`MIT`
+
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `sosap-0.0.1/pyproject.toml` & `sosap-0.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["setuptools==67.4.0", "setuptools-scm[toml]==7.1.0", "Cython==0.29.33"]
+requires = ["setuptools", "Cython"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sosap"
-version = "0.0.1"
+version = "0.1.0"
 authors = [{ name = "Seanghay Yath", email = "seanghay.dev@gmail.com" }]
 
 description = "Python binding for Phonetisaurus"
 readme = "README.md"
 requires-python = ">=3.7"
 
 classifiers = [
@@ -22,11 +22,9 @@
 
 [project.urls]
 repository = "https://github.com/seanghay/sosap"
 
 [tool.setuptools]
 include-package-data = true
 
-[tool.setuptools_scm]
-
 [tool.setuptools.packages.find]
 where = ["src"]
```

### Comparing `sosap-0.0.1/setup.py` & `sosap-0.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `sosap-0.0.1/src/Phonetisaurus/lib/util.cc` & `sosap-0.1.0/src/Phonetisaurus/lib/util.cc`

 * *Files identical despite different names*

### Comparing `sosap-0.0.1/src/core.pyx` & `sosap-0.1.0/src/core.pyx`

 * *Files identical despite different names*

### Comparing `sosap-0.0.1/src/openfst/include/fst/properties.h` & `sosap-0.1.0/src/openfst/lib/properties.cc`

 * *Files 26% similar despite different names*

```diff
@@ -1,468 +1,421 @@
 // See www.openfst.org for extensive documentation on this weighted
 // finite-state transducer library.
 //
-// FST property bits.
+// Functions for updating property bits for various FST operations and
+// string names of the properties.
 
-#ifndef FST_PROPERTIES_H_
-#define FST_PROPERTIES_H_
+#include <fst/properties.h>
 
-#include <sys/types.h>
+#include <stddef.h>
 #include <vector>
 
-#include <fst/compat.h>
-
 namespace fst {
 
-// The property bits here assert facts about an FST. If individual bits are
-// added, then the composite properties below, the property functions and
-// property names in properties.cc, and TestProperties() in test-properties.h
-// should be updated.
-
-// BINARY PROPERTIES
-//
-// For each property below, there is a single bit. If it is set, the property is
-// true. If it is not set, the property is false.
-
-// The Fst is an ExpandedFst.
-constexpr uint64 kExpanded = 0x0000000000000001ULL;
-
-// The Fst is a MutableFst.
-constexpr uint64 kMutable = 0x0000000000000002ULL;
-
-// An error was detected while constructing/using the FST.
-constexpr uint64 kError = 0x0000000000000004ULL;
+// These functions determine the properties associated with the FST result of
+// various finite-state operations. The property arguments correspond to the
+// operation's FST arguments. The properties returned assume the operation
+// modifies its first argument. Bitwise-and this result with kCopyProperties for
+// the case when a new (possibly delayed) FST is instead constructed.
+
+// Properties for a concatenatively-closed FST.
+uint64 ClosureProperties(uint64 inprops, bool, bool delayed) {
+  auto outprops = (kError | kAcceptor | kUnweighted | kAccessible) & inprops;
+  if (inprops & kUnweighted) outprops |= kUnweightedCycles;
+  if (!delayed) {
+    outprops |=
+        (kExpanded | kMutable | kCoAccessible | kNotTopSorted | kNotString) &
+        inprops;
+  }
+  if (!delayed || inprops & kAccessible) {
+    outprops |= (kNotAcceptor | kNonIDeterministic | kNonODeterministic |
+                 kNotILabelSorted | kNotOLabelSorted | kWeighted |
+                 kWeightedCycles | kNotAccessible | kNotCoAccessible) & inprops;
+    if ((inprops & kWeighted) && (inprops & kAccessible) &&
+        (inprops & kCoAccessible)) {
+        outprops |= kWeightedCycles;
+    }
+  }
+  return outprops;
+}
 
-// TRINARY PROPERTIES
-//
-// For each of these properties below there is a pair of property bits, one
-// positive and one negative. If the positive bit is set, the property is true.
-// If the negative bit is set, the property is false. If neither is set, the
-// property has unknown value. Both should never be simultaneously set. The
-// individual positive and negative bit pairs should be adjacent with the
-// positive bit at an odd and lower position.
-
-// ilabel == olabel for each arc.
-constexpr uint64 kAcceptor = 0x0000000000010000ULL;
-// ilabel != olabel for some arc.
-constexpr uint64 kNotAcceptor = 0x0000000000020000ULL;
-
-// ilabels unique leaving each state.
-constexpr uint64 kIDeterministic = 0x0000000000040000ULL;
-// ilabels not unique leaving some state.
-constexpr uint64 kNonIDeterministic = 0x0000000000080000ULL;
-
-// olabels unique leaving each state.
-constexpr uint64 kODeterministic = 0x0000000000100000ULL;
-// olabels not unique leaving some state.
-constexpr uint64 kNonODeterministic = 0x0000000000200000ULL;
-
-// FST has input/output epsilons.
-constexpr uint64 kEpsilons = 0x0000000000400000ULL;
-// FST has no input/output epsilons.
-constexpr uint64 kNoEpsilons = 0x0000000000800000ULL;
-
-// FST has input epsilons.
-constexpr uint64 kIEpsilons = 0x0000000001000000ULL;
-// FST has no input epsilons.
-constexpr uint64 kNoIEpsilons = 0x0000000002000000ULL;
-
-// FST has output epsilons.
-constexpr uint64 kOEpsilons = 0x0000000004000000ULL;
-// FST has no output epsilons.
-constexpr uint64 kNoOEpsilons = 0x0000000008000000ULL;
-
-// ilabels sorted wrt < for each state.
-constexpr uint64 kILabelSorted = 0x0000000010000000ULL;
-// ilabels not sorted wrt < for some state.
-constexpr uint64 kNotILabelSorted = 0x0000000020000000ULL;
-
-// olabels sorted wrt < for each state.
-constexpr uint64 kOLabelSorted = 0x0000000040000000ULL;
-// olabels not sorted wrt < for some state.
-constexpr uint64 kNotOLabelSorted = 0x0000000080000000ULL;
-
-// Non-trivial arc or final weights.
-constexpr uint64 kWeighted = 0x0000000100000000ULL;
-// Only trivial arc and final weights.
-constexpr uint64 kUnweighted = 0x0000000200000000ULL;
-
-// FST has cycles.
-constexpr uint64 kCyclic = 0x0000000400000000ULL;
-// FST has no cycles.
-constexpr uint64 kAcyclic = 0x0000000800000000ULL;
-
-// FST has cycles containing the initial state.
-constexpr uint64 kInitialCyclic = 0x0000001000000000ULL;
-// FST has no cycles containing the initial state.
-constexpr uint64 kInitialAcyclic = 0x0000002000000000ULL;
-
-// FST is topologically sorted.
-constexpr uint64 kTopSorted = 0x0000004000000000ULL;
-// FST is not topologically sorted.
-constexpr uint64 kNotTopSorted = 0x0000008000000000ULL;
-
-// All states reachable from the initial state.
-constexpr uint64 kAccessible = 0x0000010000000000ULL;
-// Not all states reachable from the initial state.
-constexpr uint64 kNotAccessible = 0x0000020000000000ULL;
-
-// All states can reach a final state.
-constexpr uint64 kCoAccessible = 0x0000040000000000ULL;
-// Not all states can reach a final state.
-constexpr uint64 kNotCoAccessible = 0x0000080000000000ULL;
-
-// If NumStates() > 0, then state 0 is initial, state NumStates() - 1 is final,
-// there is a transition from each non-final state i to state i + 1, and there
-// are no other transitions.
-constexpr uint64 kString = 0x0000100000000000ULL;
-
-// Not a string FST.
-constexpr uint64 kNotString = 0x0000200000000000ULL;
-
-// FST has least one weighted cycle.
-constexpr uint64 kWeightedCycles = 0x0000400000000000ULL;
-
-// Only unweighted cycles.
-constexpr uint64 kUnweightedCycles = 0x0000800000000000ULL;
-
-// COMPOSITE PROPERTIES
-
-// Properties of an empty machine.
-constexpr uint64 kNullProperties =
-    kAcceptor | kIDeterministic | kODeterministic | kNoEpsilons | kNoIEpsilons |
-    kNoOEpsilons | kILabelSorted | kOLabelSorted | kUnweighted | kAcyclic |
-    kInitialAcyclic | kTopSorted | kAccessible | kCoAccessible | kString |
-    kUnweightedCycles;
-
-// Properties that are preserved when an FST is copied.
-constexpr uint64 kCopyProperties =
-    kError | kAcceptor | kNotAcceptor | kIDeterministic | kNonIDeterministic |
-    kODeterministic | kNonODeterministic | kEpsilons | kNoEpsilons |
-    kIEpsilons | kNoIEpsilons | kOEpsilons | kNoOEpsilons | kILabelSorted |
-    kNotILabelSorted | kOLabelSorted | kNotOLabelSorted | kWeighted |
-    kUnweighted | kCyclic | kAcyclic | kInitialCyclic | kInitialAcyclic |
-    kTopSorted | kNotTopSorted | kAccessible | kNotAccessible | kCoAccessible |
-    kNotCoAccessible | kString | kNotString | kWeightedCycles |
-    kUnweightedCycles;
-
-// Properties that are intrinsic to the FST.
-constexpr uint64 kIntrinsicProperties =
-    kExpanded | kMutable | kAcceptor | kNotAcceptor | kIDeterministic |
-    kNonIDeterministic | kODeterministic | kNonODeterministic | kEpsilons |
-    kNoEpsilons | kIEpsilons | kNoIEpsilons | kOEpsilons | kNoOEpsilons |
-    kILabelSorted | kNotILabelSorted | kOLabelSorted | kNotOLabelSorted |
-    kWeighted | kUnweighted | kCyclic | kAcyclic | kInitialCyclic |
-    kInitialAcyclic | kTopSorted | kNotTopSorted | kAccessible |
-    kNotAccessible | kCoAccessible | kNotCoAccessible | kString | kNotString |
-    kWeightedCycles | kUnweightedCycles;
-
-// Properties that are (potentially) extrinsic to the FST.
-constexpr uint64 kExtrinsicProperties = kError;
-
-// Properties that are preserved when an FST start state is set.
-constexpr uint64 kSetStartProperties =
-    kExpanded | kMutable | kError | kAcceptor | kNotAcceptor | kIDeterministic |
-    kNonIDeterministic | kODeterministic | kNonODeterministic | kEpsilons |
-    kNoEpsilons | kIEpsilons | kNoIEpsilons | kOEpsilons | kNoOEpsilons |
-    kILabelSorted | kNotILabelSorted | kOLabelSorted | kNotOLabelSorted |
-    kWeighted | kUnweighted | kCyclic | kAcyclic | kTopSorted | kNotTopSorted |
-    kCoAccessible | kNotCoAccessible | kWeightedCycles | kUnweightedCycles;
-
-// Properties that are preserved when an FST final weight is set.
-constexpr uint64 kSetFinalProperties =
-    kExpanded | kMutable | kError | kAcceptor | kNotAcceptor | kIDeterministic |
-    kNonIDeterministic | kODeterministic | kNonODeterministic | kEpsilons |
-    kNoEpsilons | kIEpsilons | kNoIEpsilons | kOEpsilons | kNoOEpsilons |
-    kILabelSorted | kNotILabelSorted | kOLabelSorted | kNotOLabelSorted |
-    kCyclic | kAcyclic | kInitialCyclic | kInitialAcyclic | kTopSorted |
-    kNotTopSorted | kAccessible | kNotAccessible | kWeightedCycles |
-    kUnweightedCycles;
-
-// Properties that are preserved when an FST state is added.
-constexpr uint64 kAddStateProperties =
-    kExpanded | kMutable | kError | kAcceptor | kNotAcceptor | kIDeterministic |
-    kNonIDeterministic | kODeterministic | kNonODeterministic | kEpsilons |
-    kNoEpsilons | kIEpsilons | kNoIEpsilons | kOEpsilons | kNoOEpsilons |
-    kILabelSorted | kNotILabelSorted | kOLabelSorted | kNotOLabelSorted |
-    kWeighted | kUnweighted | kCyclic | kAcyclic | kInitialCyclic |
-    kInitialAcyclic | kTopSorted | kNotTopSorted | kNotAccessible |
-    kNotCoAccessible | kNotString | kWeightedCycles | kUnweightedCycles;
-
-// Properties that are preserved when an FST arc is added.
-constexpr uint64 kAddArcProperties =
-    kExpanded | kMutable | kError | kNotAcceptor | kNonIDeterministic |
-    kNonODeterministic | kEpsilons | kIEpsilons | kOEpsilons |
-    kNotILabelSorted | kNotOLabelSorted | kWeighted | kCyclic | kInitialCyclic |
-    kNotTopSorted | kAccessible | kCoAccessible | kWeightedCycles;
-
-// Properties that are preserved when an FST arc is set.
-constexpr uint64 kSetArcProperties = kExpanded | kMutable | kError;
-
-// Properties that are preserved when FST states are deleted.
-constexpr uint64 kDeleteStatesProperties =
-    kExpanded | kMutable | kError | kAcceptor | kIDeterministic |
-    kODeterministic | kNoEpsilons | kNoIEpsilons | kNoOEpsilons |
-    kILabelSorted | kOLabelSorted | kUnweighted | kAcyclic | kInitialAcyclic |
-    kTopSorted | kUnweightedCycles;
-
-// Properties that are preserved when FST arcs are deleted.
-constexpr uint64 kDeleteArcsProperties =
-    kExpanded | kMutable | kError | kAcceptor | kIDeterministic |
-    kODeterministic | kNoEpsilons | kNoIEpsilons | kNoOEpsilons |
-    kILabelSorted | kOLabelSorted | kUnweighted | kAcyclic | kInitialAcyclic |
-    kTopSorted | kNotAccessible | kNotCoAccessible | kUnweightedCycles;
-
-// Properties that are preserved when an FST's states are reordered.
-constexpr uint64 kStateSortProperties =
-    kExpanded | kMutable | kError | kAcceptor | kNotAcceptor | kIDeterministic |
-    kNonIDeterministic | kODeterministic | kNonODeterministic | kEpsilons |
-    kNoEpsilons | kIEpsilons | kNoIEpsilons | kOEpsilons | kNoOEpsilons |
-    kILabelSorted | kNotILabelSorted | kOLabelSorted | kNotOLabelSorted |
-    kWeighted | kUnweighted | kCyclic | kAcyclic | kInitialCyclic |
-    kInitialAcyclic | kAccessible | kNotAccessible | kCoAccessible |
-    kNotCoAccessible | kWeightedCycles | kUnweightedCycles;
-
-// Properties that are preserved when an FST's arcs are reordered.
-constexpr uint64 kArcSortProperties =
-    kExpanded | kMutable | kError | kAcceptor | kNotAcceptor | kIDeterministic |
-    kNonIDeterministic | kODeterministic | kNonODeterministic | kEpsilons |
-    kNoEpsilons | kIEpsilons | kNoIEpsilons | kOEpsilons | kNoOEpsilons |
-    kWeighted | kUnweighted | kCyclic | kAcyclic | kInitialCyclic |
-    kInitialAcyclic | kTopSorted | kNotTopSorted | kAccessible |
-    kNotAccessible | kCoAccessible | kNotCoAccessible | kString | kNotString |
-    kWeightedCycles | kUnweightedCycles;
-
-// Properties that are preserved when an FST's input labels are changed.
-constexpr uint64 kILabelInvariantProperties =
-    kExpanded | kMutable | kError | kODeterministic | kNonODeterministic |
-    kOEpsilons | kNoOEpsilons | kOLabelSorted | kNotOLabelSorted | kWeighted |
-    kUnweighted | kCyclic | kAcyclic | kInitialCyclic | kInitialAcyclic |
-    kTopSorted | kNotTopSorted | kAccessible | kNotAccessible | kCoAccessible |
-    kNotCoAccessible | kString | kNotString | kWeightedCycles |
-    kUnweightedCycles;
-
-// Properties that are preserved when an FST's output labels are changed.
-constexpr uint64 kOLabelInvariantProperties =
-    kExpanded | kMutable | kError | kIDeterministic | kNonIDeterministic |
-    kIEpsilons | kNoIEpsilons | kILabelSorted | kNotILabelSorted | kWeighted |
-    kUnweighted | kCyclic | kAcyclic | kInitialCyclic | kInitialAcyclic |
-    kTopSorted | kNotTopSorted | kAccessible | kNotAccessible | kCoAccessible |
-    kNotCoAccessible | kString | kNotString | kWeightedCycles |
-    kUnweightedCycles;
-
-// Properties that are preserved when an FST's weights are changed. This
-// assumes that the set of states that are non-final is not changed.
-constexpr uint64 kWeightInvariantProperties =
-    kExpanded | kMutable | kError | kAcceptor | kNotAcceptor | kIDeterministic |
-    kNonIDeterministic | kODeterministic | kNonODeterministic | kEpsilons |
-    kNoEpsilons | kIEpsilons | kNoIEpsilons | kOEpsilons | kNoOEpsilons |
-    kILabelSorted | kNotILabelSorted | kOLabelSorted | kNotOLabelSorted |
-    kCyclic | kAcyclic | kInitialCyclic | kInitialAcyclic | kTopSorted |
-    kNotTopSorted | kAccessible | kNotAccessible | kCoAccessible |
-    kNotCoAccessible | kString | kNotString;
-
-// Properties that are preserved when a superfinal state is added and an FST's
-// final weights are directed to it via new transitions.
-constexpr uint64 kAddSuperFinalProperties =
-    kExpanded | kMutable | kError | kAcceptor | kNotAcceptor |
-    kNonIDeterministic | kNonODeterministic | kEpsilons | kIEpsilons |
-    kOEpsilons | kNotILabelSorted | kNotOLabelSorted | kWeighted | kUnweighted |
-    kCyclic | kAcyclic | kInitialCyclic | kInitialAcyclic | kNotTopSorted |
-    kNotAccessible | kCoAccessible | kNotCoAccessible | kNotString |
-    kWeightedCycles | kUnweightedCycles;
-
-// Properties that are preserved when a superfinal state is removed and the
-// epsilon transitions directed to it are made final weights.
-constexpr uint64 kRmSuperFinalProperties =
-    kExpanded | kMutable | kError | kAcceptor | kNotAcceptor | kIDeterministic |
-    kODeterministic | kNoEpsilons | kNoIEpsilons | kNoOEpsilons |
-    kILabelSorted | kOLabelSorted | kWeighted | kUnweighted | kCyclic |
-    kAcyclic | kInitialCyclic | kInitialAcyclic | kTopSorted | kAccessible |
-    kCoAccessible | kNotCoAccessible | kString | kWeightedCycles |
-    kUnweightedCycles;
-
-// All binary properties.
-constexpr uint64 kBinaryProperties = 0x0000000000000007ULL;
-
-// All trinary properties.
-constexpr uint64 kTrinaryProperties = 0x0000ffffffff0000ULL;
-
-// COMPUTED PROPERTIES
-
-// 1st bit of trinary properties.
-constexpr uint64 kPosTrinaryProperties = kTrinaryProperties &
-    0x5555555555555555ULL;
-
-// 2nd bit of trinary properties.
-constexpr uint64 kNegTrinaryProperties = kTrinaryProperties &
-    0xaaaaaaaaaaaaaaaaULL;
-
-// All properties.
-constexpr uint64 kFstProperties = kBinaryProperties | kTrinaryProperties;
-
-// PROPERTY FUNCTIONS and STRING NAMES (defined in properties.cc).
-
-// Below are functions for getting property bit vectors when executing
-// mutation operations.
-inline uint64 SetStartProperties(uint64 inprops);
-
-template <typename Weight>
-uint64 SetFinalProperties(uint64 inprops, const Weight &old_weight,
-                          const Weight &new_weight);
-
-inline uint64 AddStateProperties(uint64 inprops);
-
-template <typename A>
-uint64 AddArcProperties(uint64 inprops, typename A::StateId s, const A &arc,
-                        const A *prev_arc);
-
-inline uint64 DeleteStatesProperties(uint64 inprops);
-
-inline uint64 DeleteAllStatesProperties(uint64 inprops, uint64 staticProps);
-
-inline uint64 DeleteArcsProperties(uint64 inprops);
+// Properties for a complemented FST.
+uint64 ComplementProperties(uint64 inprops) {
+  auto outprops = kAcceptor | kUnweighted | kUnweightedCycles | kNoEpsilons |
+                  kNoIEpsilons | kNoOEpsilons | kIDeterministic |
+                  kODeterministic | kAccessible;
+  outprops |=
+      (kError | kILabelSorted | kOLabelSorted | kInitialCyclic) & inprops;
+  if (inprops & kAccessible) {
+    outprops |= kNotILabelSorted | kNotOLabelSorted | kCyclic;
+  }
+  return outprops;
+}
 
-uint64 ClosureProperties(uint64 inprops, bool star, bool delayed = false);
+// Properties for a composed FST.
+uint64 ComposeProperties(uint64 inprops1, uint64 inprops2) {
+  auto outprops = kError & (inprops1 | inprops2);
+  if (inprops1 & kAcceptor && inprops2 & kAcceptor) {
+    outprops |= kAcceptor | kAccessible;
+    outprops |= (kNoEpsilons | kNoIEpsilons | kNoOEpsilons | kAcyclic |
+                 kInitialAcyclic) &
+                inprops1 & inprops2;
+    if (kNoIEpsilons & inprops1 & inprops2) {
+      outprops |= (kIDeterministic | kODeterministic) & inprops1 & inprops2;
+    }
+  } else {
+    outprops |= kAccessible;
+    outprops |= (kAcceptor | kNoIEpsilons | kAcyclic | kInitialAcyclic) &
+                inprops1 & inprops2;
+    if (kNoIEpsilons & inprops1 & inprops2) {
+      outprops |= kIDeterministic & inprops1 & inprops2;
+    }
+  }
+  return outprops;
+}
 
-uint64 ComplementProperties(uint64 inprops);
+// Properties for a concatenated FST.
+uint64 ConcatProperties(uint64 inprops1, uint64 inprops2, bool delayed) {
+  auto outprops = (kAcceptor | kUnweighted | kUnweightedCycles | kAcyclic) &
+                  inprops1 & inprops2;
+  outprops |= kError & (inprops1 | inprops2);
+  const bool empty1 = delayed;  // Can the first FST be the empty machine?
+  const bool empty2 = delayed;  // Can the second FST be the empty machine?
+  if (!delayed) {
+    outprops |= (kExpanded | kMutable | kNotTopSorted | kNotString) & inprops1;
+    outprops |= (kNotTopSorted | kNotString) & inprops2;
+  }
+  if (!empty1) outprops |= (kInitialAcyclic | kInitialCyclic) & inprops1;
+  if (!delayed || inprops1 & kAccessible) {
+    outprops |= (kNotAcceptor | kNonIDeterministic | kNonODeterministic |
+                 kEpsilons | kIEpsilons | kOEpsilons | kNotILabelSorted |
+                 kNotOLabelSorted | kWeighted | kWeightedCycles | kCyclic |
+                 kNotAccessible | kNotCoAccessible) &
+                inprops1;
+  }
+  if ((inprops1 & (kAccessible | kCoAccessible)) ==
+          (kAccessible | kCoAccessible) &&
+      !empty1) {
+    outprops |= kAccessible & inprops2;
+    if (!empty2) outprops |= kCoAccessible & inprops2;
+    if (!delayed || inprops2 & kAccessible) {
+      outprops |= (kNotAcceptor | kNonIDeterministic | kNonODeterministic |
+                   kEpsilons | kIEpsilons | kOEpsilons | kNotILabelSorted |
+                   kNotOLabelSorted | kWeighted | kWeightedCycles | kCyclic |
+                   kNotAccessible | kNotCoAccessible) &
+                  inprops2;
+    }
+  }
+  return outprops;
+}
 
-uint64 ComposeProperties(uint64 inprops1, uint64 inprops2);
+// Properties for a determinized FST.
+uint64 DeterminizeProperties(uint64 inprops, bool has_subsequential_label,
+                             bool distinct_psubsequential_labels) {
+  auto outprops = kAccessible;
+  if ((kAcceptor & inprops) ||
+      ((kNoIEpsilons & inprops) && distinct_psubsequential_labels) ||
+      (has_subsequential_label && distinct_psubsequential_labels)) {
+    outprops |= kIDeterministic;
+  }
+  outprops |= (kError | kAcceptor | kAcyclic | kInitialAcyclic | kCoAccessible |
+               kString) &
+              inprops;
+  if ((inprops & kNoIEpsilons) && distinct_psubsequential_labels) {
+    outprops |= kNoEpsilons & inprops;
+  }
+  if (inprops & kAccessible) {
+    outprops |= (kIEpsilons | kOEpsilons | kCyclic) & inprops;
+  }
+  if (inprops & kAcceptor) outprops |= (kNoIEpsilons | kNoOEpsilons) & inprops;
+  if ((inprops & kNoIEpsilons) && has_subsequential_label) {
+    outprops |= kNoIEpsilons;
+  }
+  return outprops;
+}
 
-uint64 ConcatProperties(uint64 inprops1, uint64 inprops2, bool delayed = false);
+// Properties for factored weight FST.
+uint64 FactorWeightProperties(uint64 inprops) {
+  auto outprops = (kExpanded | kMutable | kError | kAcceptor | kAcyclic |
+                   kAccessible | kCoAccessible) &
+                  inprops;
+  if (inprops & kAccessible) {
+    outprops |= (kNotAcceptor | kNonIDeterministic | kNonODeterministic |
+                 kEpsilons | kIEpsilons | kOEpsilons | kCyclic |
+                 kNotILabelSorted | kNotOLabelSorted) &
+                inprops;
+  }
+  return outprops;
+}
 
-uint64 DeterminizeProperties(uint64 inprops, bool has_subsequential_label,
-                             bool distinct_psubsequential_labels);
+// Properties for an inverted FST.
+uint64 InvertProperties(uint64 inprops) {
+  auto outprops = (kExpanded | kMutable | kError | kAcceptor | kNotAcceptor |
+                   kEpsilons | kNoEpsilons | kWeighted | kUnweighted |
+                   kWeightedCycles | kUnweightedCycles | kCyclic | kAcyclic |
+                   kInitialCyclic | kInitialAcyclic | kTopSorted |
+                   kNotTopSorted | kAccessible | kNotAccessible |
+                   kCoAccessible | kNotCoAccessible | kString | kNotString) &
+                  inprops;
+  if (kIDeterministic & inprops) outprops |= kODeterministic;
+  if (kNonIDeterministic & inprops) outprops |= kNonODeterministic;
+  if (kODeterministic & inprops) outprops |= kIDeterministic;
+  if (kNonODeterministic & inprops) outprops |= kNonIDeterministic;
+
+  if (kIEpsilons & inprops) outprops |= kOEpsilons;
+  if (kNoIEpsilons & inprops) outprops |= kNoOEpsilons;
+  if (kOEpsilons & inprops) outprops |= kIEpsilons;
+  if (kNoOEpsilons & inprops) outprops |= kNoIEpsilons;
+
+  if (kILabelSorted & inprops) outprops |= kOLabelSorted;
+  if (kNotILabelSorted & inprops) outprops |= kNotOLabelSorted;
+  if (kOLabelSorted & inprops) outprops |= kILabelSorted;
+  if (kNotOLabelSorted & inprops) outprops |= kNotILabelSorted;
+  return outprops;
+}
 
-uint64 FactorWeightProperties(uint64 inprops);
+// Properties for a projected FST.
+uint64 ProjectProperties(uint64 inprops, bool project_input) {
+  auto outprops = kAcceptor;
+  outprops |= (kExpanded | kMutable | kError | kWeighted | kUnweighted |
+               kWeightedCycles | kUnweightedCycles |
+               kCyclic | kAcyclic | kInitialCyclic | kInitialAcyclic |
+               kTopSorted | kNotTopSorted | kAccessible | kNotAccessible |
+               kCoAccessible | kNotCoAccessible | kString | kNotString) &
+              inprops;
+  if (project_input) {
+    outprops |= (kIDeterministic | kNonIDeterministic | kIEpsilons |
+                 kNoIEpsilons | kILabelSorted | kNotILabelSorted) &
+                inprops;
+
+    if (kIDeterministic & inprops) outprops |= kODeterministic;
+    if (kNonIDeterministic & inprops) outprops |= kNonODeterministic;
+
+    if (kIEpsilons & inprops) outprops |= kOEpsilons | kEpsilons;
+    if (kNoIEpsilons & inprops) outprops |= kNoOEpsilons | kNoEpsilons;
+
+    if (kILabelSorted & inprops) outprops |= kOLabelSorted;
+    if (kNotILabelSorted & inprops) outprops |= kNotOLabelSorted;
+  } else {
+    outprops |= (kODeterministic | kNonODeterministic | kOEpsilons |
+                 kNoOEpsilons | kOLabelSorted | kNotOLabelSorted) &
+                inprops;
 
-uint64 InvertProperties(uint64 inprops);
+    if (kODeterministic & inprops) outprops |= kIDeterministic;
+    if (kNonODeterministic & inprops) outprops |= kNonIDeterministic;
 
-uint64 ProjectProperties(uint64 inprops, bool project_input);
+    if (kOEpsilons & inprops) outprops |= kIEpsilons | kEpsilons;
+    if (kNoOEpsilons & inprops) outprops |= kNoIEpsilons | kNoEpsilons;
 
-uint64 RandGenProperties(uint64 inprops, bool weighted);
+    if (kOLabelSorted & inprops) outprops |= kILabelSorted;
+    if (kNotOLabelSorted & inprops) outprops |= kNotILabelSorted;
+  }
+  return outprops;
+}
 
-uint64 RelabelProperties(uint64 inprops);
+// Properties for a randgen FST.
+uint64 RandGenProperties(uint64 inprops, bool weighted) {
+  auto outprops = kAcyclic | kInitialAcyclic | kAccessible | kUnweightedCycles;
+  outprops |= inprops & kError;
+  if (weighted) {
+    outprops |= kTopSorted;
+    outprops |=
+        (kAcceptor | kNoEpsilons | kNoIEpsilons | kNoOEpsilons |
+         kIDeterministic | kODeterministic | kILabelSorted | kOLabelSorted) &
+        inprops;
+  } else {
+    outprops |= kUnweighted;
+    outprops |= (kAcceptor | kILabelSorted | kOLabelSorted) & inprops;
+  }
+  return outprops;
+}
 
-uint64 ReplaceProperties(const std::vector<uint64> &inprops, size_t root,
+// Properties for a replace FST.
+uint64 ReplaceProperties(const std::vector<uint64>& inprops, size_t root,
                          bool epsilon_on_call, bool epsilon_on_return,
                          bool out_epsilon_on_call, bool out_epsilon_on_return,
-                         bool replace_transducer, bool no_empty_fst,
+                         bool replace_transducer, bool no_empty_fsts,
                          bool all_ilabel_sorted, bool all_olabel_sorted,
-                         bool all_negative_or_dense);
-
-uint64 ReverseProperties(uint64 inprops, bool has_superinitial);
-
-uint64 ReweightProperties(uint64 inprops);
-
-uint64 RmEpsilonProperties(uint64 inprops, bool delayed = false);
-
-uint64 ShortestPathProperties(uint64 props, bool tree = false);
-
-uint64 SynchronizeProperties(uint64 inprops);
-
-uint64 UnionProperties(uint64 inprops1, uint64 inprops2, bool delayed = false);
-
-// Definitions of inlined functions.
-
-uint64 SetStartProperties(uint64 inprops) {
-  auto outprops = inprops & kSetStartProperties;
-  if (inprops & kAcyclic) {
-    outprops |= kInitialAcyclic;
+                         bool all_negative_or_dense) {
+  if (inprops.empty()) return kNullProperties;
+  uint64 outprops = 0;
+  for (auto inprop : inprops) outprops |= kError & inprop;
+  uint64 access_props = no_empty_fsts ? kAccessible | kCoAccessible : 0;
+  for (auto inprop : inprops) {
+    access_props &= (inprop & (kAccessible | kCoAccessible));
+  }
+  if (access_props == (kAccessible | kCoAccessible)) {
+    outprops |= access_props;
+    if (inprops[root] & kInitialCyclic) outprops |= kInitialCyclic;
+    uint64 props = 0;
+    bool string = true;
+    for (auto inprop : inprops) {
+      if (replace_transducer) props |= kNotAcceptor & inprop;
+      props |= (kNonIDeterministic | kNonODeterministic | kEpsilons |
+                kIEpsilons | kOEpsilons | kWeighted | kWeightedCycles |
+                kCyclic | kNotTopSorted | kNotString) & inprop;
+      if (!(inprop & kString)) string = false;
+    }
+    outprops |= props;
+    if (string) outprops |= kString;
+  }
+  bool acceptor = !replace_transducer;
+  bool ideterministic = !epsilon_on_call && epsilon_on_return;
+  bool no_iepsilons = !epsilon_on_call && !epsilon_on_return;
+  bool acyclic = true;
+  bool unweighted = true;
+  for (size_t i = 0; i < inprops.size(); ++i) {
+    if (!(inprops[i] & kAcceptor)) acceptor = false;
+    if (!(inprops[i] & kIDeterministic)) ideterministic = false;
+    if (!(inprops[i] & kNoIEpsilons)) no_iepsilons = false;
+    if (!(inprops[i] & kAcyclic)) acyclic = false;
+    if (!(inprops[i] & kUnweighted)) unweighted = false;
+    if (i != root && !(inprops[i] & kNoIEpsilons)) ideterministic = false;
+  }
+  if (acceptor) outprops |= kAcceptor;
+  if (ideterministic) outprops |= kIDeterministic;
+  if (no_iepsilons) outprops |= kNoIEpsilons;
+  if (acyclic) outprops |= kAcyclic;
+  if (unweighted) outprops |= kUnweighted;
+  if (inprops[root] & kInitialAcyclic) outprops |= kInitialAcyclic;
+  // We assume that all terminals are positive. The resulting ReplaceFst is
+  // known to be kILabelSorted when: (1) all sub-FSTs are kILabelSorted, (2) the
+  // input label of the return arc is epsilon, and (3) one of the 3 following
+  // conditions is satisfied:
+  //
+  //  1. the input label of the call arc is not epsilon
+  //  2. all non-terminals are negative, or
+  //  3. all non-terninals are positive and form a dense range containing 1.
+  if (all_ilabel_sorted && epsilon_on_return &&
+      (!epsilon_on_call || all_negative_or_dense)) {
+    outprops |= kILabelSorted;
+  }
+  // Similarly, the resulting ReplaceFst is known to be kOLabelSorted when: (1)
+  // all sub-FSTs are kOLabelSorted, (2) the output label of the return arc is
+  // epsilon, and (3) one of the 3 following conditions is satisfied:
+  //
+  //  1. the output label of the call arc is not epsilon
+  //  2. all non-terminals are negative, or
+  //  3. all non-terninals are positive and form a dense range containing 1.
+  if (all_olabel_sorted && out_epsilon_on_return &&
+      (!out_epsilon_on_call || all_negative_or_dense)) {
+    outprops |= kOLabelSorted;
   }
   return outprops;
 }
 
-uint64 AddStateProperties(uint64 inprops) {
-  return inprops & kAddStateProperties;
+// Properties for a relabeled FST.
+uint64 RelabelProperties(uint64 inprops) {
+  static constexpr auto outprops =
+      kExpanded | kMutable | kError | kWeighted | kUnweighted |
+      kWeightedCycles | kUnweightedCycles | kCyclic | kAcyclic |
+      kInitialCyclic | kInitialAcyclic | kTopSorted | kNotTopSorted |
+      kAccessible | kNotAccessible | kCoAccessible | kNotCoAccessible |
+      kString | kNotString;
+  return outprops & inprops;
 }
 
-uint64 DeleteStatesProperties(uint64 inprops) {
-  return inprops & kDeleteStatesProperties;
+// Properties for a reversed FST (the superinitial state limits this set).
+uint64 ReverseProperties(uint64 inprops, bool has_superinitial) {
+  auto outprops = (kExpanded | kMutable | kError | kAcceptor | kNotAcceptor |
+                   kEpsilons | kIEpsilons | kOEpsilons | kUnweighted | kCyclic |
+                   kAcyclic | kWeightedCycles | kUnweightedCycles) &
+                  inprops;
+  if (has_superinitial) outprops |= kWeighted & inprops;
+  return outprops;
 }
 
-uint64 DeleteAllStatesProperties(uint64 inprops, uint64 staticprops) {
-  const auto outprops = inprops & kError;
-  return outprops | kNullProperties | staticprops;
+// Properties for re-weighted FST.
+uint64 ReweightProperties(uint64 inprops) {
+  auto outprops = inprops & kWeightInvariantProperties;
+  outprops = outprops & ~kCoAccessible;
+  return outprops;
 }
 
-uint64 DeleteArcsProperties(uint64 inprops) {
-  return inprops & kDeleteArcsProperties;
+// Properties for an epsilon-removed FST.
+uint64 RmEpsilonProperties(uint64 inprops, bool delayed) {
+  auto outprops = kNoEpsilons;
+  outprops |= (kError | kAcceptor | kAcyclic | kInitialAcyclic) & inprops;
+  if (inprops & kAcceptor) outprops |= kNoIEpsilons | kNoOEpsilons;
+  if (!delayed) {
+    outprops |= kExpanded | kMutable;
+    outprops |= kTopSorted & inprops;
+  }
+  if (!delayed || inprops & kAccessible) outprops |= kNotAcceptor & inprops;
+  return outprops;
 }
 
-// Definitions of template functions.
+// Properties for shortest path. This function computes how the properties of
+// the output of shortest path need to be updated, given that 'props' is already
+// known.
+uint64 ShortestPathProperties(uint64 props, bool tree) {
+  auto outprops =
+      props | kAcyclic | kInitialAcyclic | kAccessible | kUnweightedCycles;
+  if (!tree) outprops |= kCoAccessible;
+  return outprops;
+}
 
-template <typename Weight>
-uint64 SetFinalProperties(uint64 inprops, const Weight &old_weight,
-                          const Weight &new_weight) {
-  auto outprops = inprops;
-  if (old_weight != Weight::Zero() && old_weight != Weight::One()) {
-    outprops &= ~kWeighted;
-  }
-  if (new_weight != Weight::Zero() && new_weight != Weight::One()) {
-    outprops |= kWeighted;
-    outprops &= ~kUnweighted;
+// Properties for a synchronized FST.
+uint64 SynchronizeProperties(uint64 inprops) {
+  auto outprops = (kError | kAcceptor | kAcyclic | kAccessible | kCoAccessible |
+                   kUnweighted | kUnweightedCycles) &
+                  inprops;
+  if (inprops & kAccessible) {
+    outprops |= (kCyclic | kNotCoAccessible | kWeighted | kWeightedCycles) &
+        inprops;
   }
-  outprops &= kSetFinalProperties | kWeighted | kUnweighted;
   return outprops;
 }
 
-/// Gets the properties for the MutableFst::AddArc method.
-///
-/// \param inprops  the current properties of the FST
-/// \param s        the ID of the state to which an arc is being added.
-/// \param arc      the arc being added to the state with the specified ID
-/// \param prev_arc the previously-added (or "last") arc of state s, or nullptr
-//                  if s currently has no arcs.
-template <typename Arc>
-uint64 AddArcProperties(uint64 inprops, typename Arc::StateId s,
-                        const Arc &arc, const Arc *prev_arc) {
-  using Weight = typename Arc::Weight;
-  auto outprops = inprops;
-  if (arc.ilabel != arc.olabel) {
-    outprops |= kNotAcceptor;
-    outprops &= ~kAcceptor;
-  }
-  if (arc.ilabel == 0) {
-    outprops |= kIEpsilons;
-    outprops &= ~kNoIEpsilons;
-    if (arc.olabel == 0) {
-      outprops |= kEpsilons;
-      outprops &= ~kNoEpsilons;
-    }
+// Properties for a unioned FST.
+uint64 UnionProperties(uint64 inprops1, uint64 inprops2, bool delayed) {
+  auto outprops =
+      (kAcceptor | kUnweighted | kUnweightedCycles | kAcyclic | kAccessible) &
+      inprops1 & inprops2;
+  outprops |= kError & (inprops1 | inprops2);
+  outprops |= kInitialAcyclic;
+  bool empty1 = delayed;  // Can the first FST be the empty machine?
+  bool empty2 = delayed;  // Can the second FST be the empty machine?
+  if (!delayed) {
+    outprops |= (kExpanded | kMutable | kNotTopSorted) & inprops1;
+    outprops |= kNotTopSorted & inprops2;
   }
-  if (arc.olabel == 0) {
-    outprops |= kOEpsilons;
-    outprops &= ~kNoOEpsilons;
-  }
-  if (prev_arc) {
-    if (prev_arc->ilabel > arc.ilabel) {
-      outprops |= kNotILabelSorted;
-      outprops &= ~kILabelSorted;
-    }
-    if (prev_arc->olabel > arc.olabel) {
-      outprops |= kNotOLabelSorted;
-      outprops &= ~kOLabelSorted;
-    }
+  if (!empty1 && !empty2) {
+    outprops |= kEpsilons | kIEpsilons | kOEpsilons;
+    outprops |= kCoAccessible & inprops1 & inprops2;
   }
-  if (arc.weight != Weight::Zero() && arc.weight != Weight::One()) {
-    outprops |= kWeighted;
-    outprops &= ~kUnweighted;
+  // Note kNotCoAccessible does not hold because of kInitialAcyclic option.
+  if (!delayed || inprops1 & kAccessible) {
+    outprops |=
+        (kNotAcceptor | kNonIDeterministic | kNonODeterministic | kEpsilons |
+         kIEpsilons | kOEpsilons | kNotILabelSorted | kNotOLabelSorted |
+         kWeighted | kWeightedCycles | kCyclic | kNotAccessible) &
+        inprops1;
   }
-  if (arc.nextstate <= s) {
-    outprops |= kNotTopSorted;
-    outprops &= ~kTopSorted;
-  }
-  outprops &= kAddArcProperties | kAcceptor | kNoEpsilons | kNoIEpsilons |
-              kNoOEpsilons | kILabelSorted | kOLabelSorted | kUnweighted |
-              kTopSorted;
-  if (outprops & kTopSorted) {
-    outprops |= kAcyclic | kInitialAcyclic;
+  if (!delayed || inprops2 & kAccessible) {
+    outprops |= (kNotAcceptor | kNonIDeterministic | kNonODeterministic |
+                 kEpsilons | kIEpsilons | kOEpsilons | kNotILabelSorted |
+                 kNotOLabelSorted | kWeighted | kWeightedCycles | kCyclic |
+                 kNotAccessible | kNotCoAccessible) &
+                inprops2;
   }
   return outprops;
 }
 
-extern const char *PropertyNames[];
+// Property string names (indexed by bit position).
+const char* PropertyNames[] = {
+    // Binary.
+    "expanded", "mutable", "error", "", "", "", "", "", "", "", "", "", "", "",
+    "", "",
+    // Ternary.
+    "acceptor", "not acceptor", "input deterministic",
+    "non input deterministic", "output deterministic",
+    "non output deterministic", "input/output epsilons",
+    "no input/output epsilons", "input epsilons", "no input epsilons",
+    "output epsilons", "no output epsilons", "input label sorted",
+    "not input label sorted", "output label sorted", "not output label sorted",
+    "weighted", "unweighted", "cyclic", "acyclic", "cyclic at initial state",
+    "acyclic at initial state", "top sorted", "not top sorted", "accessible",
+    "not accessible", "coaccessible", "not coaccessible", "string",
+    "not string", "weighted cycles", "unweighted cycles"};
 
 }  // namespace fst
-
-#endif  // FST_PROPERTIES_H_
```

### Comparing `sosap-0.0.1/src/openfst/include/fst/symbol-table.h` & `sosap-0.1.0/src/openfst/lib/symbol-table.cc`

 * *Files 27% similar despite different names*

```diff
@@ -1,445 +1,337 @@
 // See www.openfst.org for extensive documentation on this weighted
 // finite-state transducer library.
 //
 // Classes to provide symbol-to-integer and integer-to-symbol mappings.
 
-#ifndef FST_SYMBOL_TABLE_H_
-#define FST_SYMBOL_TABLE_H_
+#include <fst/symbol-table.h>
 
-#include <functional>
-#include <ios>
-#include <iostream>
-#include <memory>
-#include <sstream>
-#include <string>
-#include <utility>
-#include <vector>
-
-#include <fst/compat.h>
 #include <fst/flags.h>
 #include <fst/log.h>
+
 #include <fstream>
-#include <map>
+#include <fst/util.h>
 
-DECLARE_bool(fst_compat_symbols);
+DEFINE_bool(fst_compat_symbols, true,
+            "Require symbol tables to match when appropriate");
+DEFINE_string(fst_field_separator, "\t ",
+              "Set of characters used as a separator between printed fields");
 
 namespace fst {
 
-constexpr int64 kNoSymbol = -1;
-
-// WARNING: Reading via symbol table read options should
-//          not be used. This is a temporary work around for
-//          reading symbol ranges of previously stored symbol sets.
-struct SymbolTableReadOptions {
-  SymbolTableReadOptions() {}
-
-  SymbolTableReadOptions(
-      std::vector<std::pair<int64, int64>> string_hash_ranges,
-      const string &source)
-      : string_hash_ranges(std::move(string_hash_ranges)), source(source) {}
-
-  std::vector<std::pair<int64, int64>> string_hash_ranges;
-  string source;
-};
-
-struct SymbolTableTextOptions {
-  explicit SymbolTableTextOptions(bool allow_negative_labels = false);
-
-  bool allow_negative_labels;
-  string fst_field_separator;
-};
+SymbolTableTextOptions::SymbolTableTextOptions(bool allow_negative_labels)
+    : allow_negative_labels(allow_negative_labels),
+      fst_field_separator(FLAGS_fst_field_separator) {}
 
 namespace internal {
 
-extern const int kLineLen;
-
-// List of symbols with a dense hash for looking up symbol index, rehashing at
-// 75% occupancy.
-class DenseSymbolMap {
- public:
-  DenseSymbolMap();
-
-  DenseSymbolMap(const DenseSymbolMap &x);
-
-  std::pair<int64, bool> InsertOrFind(const string &key);
-
-  int64 Find(const string &key) const;
-
-  size_t Size() const { return symbols_.size(); }
-
-  const string &GetSymbol(size_t idx) const { return symbols_[idx]; }
-
-  void RemoveSymbol(size_t idx);
-
- private:
-  // num_buckets must be power of 2.
-  void Rehash(size_t num_buckets);
-
-  int64 empty_;
-  std::vector<string> symbols_;
-  std::hash<string> str_hash_;
-  std::vector<int64> buckets_;
-  uint64 hash_mask_;
-};
-
-class SymbolTableImpl {
- public:
-  explicit SymbolTableImpl(const string &name)
-      : name_(name),
-        available_key_(0),
-        dense_key_limit_(0),
-        check_sum_finalized_(false) {}
-
-  SymbolTableImpl(const SymbolTableImpl &impl)
-      : name_(impl.name_),
-        available_key_(impl.available_key_),
-        dense_key_limit_(impl.dense_key_limit_),
-        symbols_(impl.symbols_),
-        idx_key_(impl.idx_key_),
-        key_map_(impl.key_map_),
-        check_sum_finalized_(false) {}
-
-  int64 AddSymbol(const string &symbol, int64 key);
-
-  int64 AddSymbol(const string &symbol) {
-    return AddSymbol(symbol, available_key_);
-  }
-
-  // Removes the symbol with the given key. The removal is costly
-  // (O(NumSymbols)) and may reduce the efficiency of Find() because of a
-  // potentially reduced size of the dense key interval.
-  void RemoveSymbol(int64 key);
-
-  static SymbolTableImpl *ReadText(
-      std::istream &strm, const string &name,
-      const SymbolTableTextOptions &opts = SymbolTableTextOptions());
-
-  static SymbolTableImpl* Read(std::istream &strm,
-                               const SymbolTableReadOptions &opts);
-
-  bool Write(std::ostream &strm) const;
-
-  // Return the string associated with the key. If the key is out of
-  // range (<0, >max), return an empty string.
-  string Find(int64 key) const {
-    int64 idx = key;
-    if (key < 0 || key >= dense_key_limit_) {
-      const auto it = key_map_.find(key);
-      if (it == key_map_.end()) return "";
-      idx = it->second;
-    }
-    if (idx < 0 || idx >= symbols_.Size()) return "";
-    return symbols_.GetSymbol(idx);
-  }
-
-  // Returns the key associated with the symbol; if the symbol
-  // does not exists, returns kNoSymbol.
-  int64 Find(const string &symbol) const {
-    int64 idx = symbols_.Find(symbol);
-    if (idx == kNoSymbol || idx < dense_key_limit_) return idx;
-    return idx_key_[idx - dense_key_limit_];
-  }
+// Maximum line length in textual symbols file.
+const int kLineLen = 8096;
 
-  bool Member(int64 key) const { return !Find(key).empty(); }
+// Identifies stream data as a symbol table (and its endianity).
+static constexpr int32 kSymbolTableMagicNumber = 2125658996;
 
-  bool Member(const string &symbol) const { return Find(symbol) != kNoSymbol; }
-
-  int64 GetNthKey(ssize_t pos) const {
-    if (pos < 0 || pos >= symbols_.Size()) return kNoSymbol;
-    if (pos < dense_key_limit_) return pos;
-    return Find(symbols_.GetSymbol(pos));
-  }
 
-  const string &Name() const { return name_; }
+DenseSymbolMap::DenseSymbolMap()
+    : empty_(-1), buckets_(1 << 4), hash_mask_(buckets_.size() - 1) {
+  std::uninitialized_fill(buckets_.begin(), buckets_.end(), empty_);
+}
 
-  void SetName(const string &new_name) { name_ = new_name; }
+DenseSymbolMap::DenseSymbolMap(const DenseSymbolMap &other)
+    : empty_(-1),
+      symbols_(other.symbols_),
+      buckets_(other.buckets_),
+      hash_mask_(other.hash_mask_) {}
+
+std::pair<int64, bool> DenseSymbolMap::InsertOrFind(const string &key) {
+  static constexpr float kMaxOccupancyRatio = 0.75;  // Grows when 75% full.
+  if (Size() >= kMaxOccupancyRatio * buckets_.size()) {
+    Rehash(buckets_.size() * 2);
+  }
+  size_t idx = str_hash_(key) & hash_mask_;
+  while (buckets_[idx] != empty_) {
+    const auto stored_value = buckets_[idx];
+    if (symbols_[stored_value] == key) return {stored_value, false};
+    idx = (idx + 1) & hash_mask_;
+  }
+  const auto next = Size();
+  buckets_[idx] = next;
+  symbols_.emplace_back(key);
+  return {next, true};
+}
 
-  const string &CheckSum() const {
-    MaybeRecomputeCheckSum();
-    return check_sum_string_;
+int64 DenseSymbolMap::Find(const string &key) const {
+  size_t idx = str_hash_(key) & hash_mask_;
+  while (buckets_[idx] != empty_) {
+    const auto stored_value = buckets_[idx];
+    if (symbols_[stored_value] == key) return stored_value;
+    idx = (idx + 1) & hash_mask_;
   }
+  return buckets_[idx];
+}
 
-  const string &LabeledCheckSum() const {
-    MaybeRecomputeCheckSum();
-    return labeled_check_sum_string_;
+void DenseSymbolMap::Rehash(size_t num_buckets) {
+  buckets_.resize(num_buckets);
+  hash_mask_ = buckets_.size() - 1;
+  std::uninitialized_fill(buckets_.begin(), buckets_.end(), empty_);
+  for (size_t i = 0; i < Size(); ++i) {
+    size_t idx = str_hash_(string(symbols_[i])) & hash_mask_;
+    while (buckets_[idx] != empty_) {
+      idx = (idx + 1) & hash_mask_;
+    }
+    buckets_[idx] = i;
   }
+}
 
-  int64 AvailableKey() const { return available_key_; }
-
-  size_t NumSymbols() const { return symbols_.Size(); }
-
- private:
-  // Recomputes the checksums (both of them) if we've had changes since the last
-  // computation (i.e., if check_sum_finalized_ is false).
-  // Takes ~2.5 microseconds (dbg) or ~230 nanoseconds (opt) on a 2.67GHz Xeon
-  // if the checksum is up-to-date (requiring no recomputation).
-  void MaybeRecomputeCheckSum() const;
-
-  string name_;
-  int64 available_key_;
-  int64 dense_key_limit_;
-
-  DenseSymbolMap symbols_;
-  // Maps index to key for index >= dense_key_limit:
-  //   key = idx_key_[index - dense_key_limit]
-  std::vector<int64> idx_key_;
-  // Maps key to index for key >= dense_key_limit_.
-  //  index = key_map_[key]
-  std::map<int64, int64> key_map_;
-
-  mutable bool check_sum_finalized_;
-  mutable string check_sum_string_;
-  mutable string labeled_check_sum_string_;
-  mutable Mutex check_sum_mutex_;
-};
-
-}  // namespace internal
+void DenseSymbolMap::RemoveSymbol(size_t idx) {
+  symbols_.erase(symbols_.begin() + idx);
+  Rehash(buckets_.size());
+}
 
-// Symbol (string) to integer (and reverse) mapping.
-//
-// The SymbolTable implements the mappings of labels to strings and reverse.
-// SymbolTables are used to describe the alphabet of the input and output
-// labels for arcs in a Finite State Transducer.
-//
-// SymbolTables are reference-counted and can therefore be shared across
-// multiple machines. For example a language model grammar G, with a
-// SymbolTable for the words in the language model can share this symbol
-// table with the lexical representation L o G.
-class SymbolTable {
- public:
-  // Constructs symbol table with an optional name.
-  explicit SymbolTable(const string &name = "<unspecified>")
-      : impl_(std::make_shared<internal::SymbolTableImpl>(name)) {}
-
-  virtual ~SymbolTable() {}
-
-  // Reads a text representation of the symbol table from an istream. Pass a
-  // name to give the resulting SymbolTable.
-  static SymbolTable *ReadText(
-      std::istream &strm, const string &name,
-      const SymbolTableTextOptions &opts = SymbolTableTextOptions()) {
-    auto *impl = internal::SymbolTableImpl::ReadText(strm, name, opts);
-    return impl ? new SymbolTable(impl) : nullptr;
-  }
-
-  // Reads a text representation of the symbol table.
-  static SymbolTable *ReadText(const string &filename,
-      const SymbolTableTextOptions &opts = SymbolTableTextOptions()) {
-    std::ifstream strm(filename, std::ios_base::in);
-    if (!strm.good()) {
-      LOG(ERROR) << "SymbolTable::ReadText: Can't open file " << filename;
+SymbolTableImpl *SymbolTableImpl::ReadText(std::istream &strm,
+                                           const string &filename,
+                                           const SymbolTableTextOptions &opts) {
+  std::unique_ptr<SymbolTableImpl> impl(new SymbolTableImpl(filename));
+  int64 nline = 0;
+  char line[kLineLen];
+  while (!strm.getline(line, kLineLen).fail()) {
+    ++nline;
+    std::vector<char *> col;
+    const auto separator = opts.fst_field_separator + "\n";
+    SplitString(line, separator.c_str(), &col, true);
+    if (col.empty()) continue;  // Empty line.
+    if (col.size() != 2) {
+      LOG(ERROR) << "SymbolTable::ReadText: Bad number of columns ("
+                 << col.size() << "), "
+                 << "file = " << filename << ", line = " << nline << ":<"
+                 << line << ">";
       return nullptr;
     }
-    return ReadText(strm, filename, opts);
-  }
-
-  // WARNING: Reading via symbol table read options should not be used. This is
-  // a temporary work-around.
-  static SymbolTable* Read(std::istream &strm,
-                           const SymbolTableReadOptions &opts) {
-    auto *impl = internal::SymbolTableImpl::Read(strm, opts);
-    return (impl) ? new SymbolTable(impl) : nullptr;
-  }
-
-  // Reads a binary dump of the symbol table from a stream.
-  static SymbolTable *Read(std::istream &strm,
-                           const string &source) {
-    SymbolTableReadOptions opts;
-    opts.source = source;
-    return Read(strm, opts);
-  }
-
-  // Reads a binary dump of the symbol table.
-  static SymbolTable *Read(const string& filename) {
-    std::ifstream strm(filename,
-                            std::ios_base::in | std::ios_base::binary);
-    if (!strm.good()) {
-      LOG(ERROR) << "SymbolTable::Read: Can't open file " << filename;
+    const char *symbol = col[0];
+    const char *value = col[1];
+    char *p;
+    const auto key = strtoll(value, &p, 10);
+    if (p < value + strlen(value) || (!opts.allow_negative_labels && key < 0) ||
+        key == kNoSymbol) {
+      LOG(ERROR) << "SymbolTable::ReadText: Bad non-negative integer \""
+                 << value << "\", "
+                 << "file = " << filename << ", line = " << nline;
       return nullptr;
     }
-    return Read(strm, filename);
-  }
-
-  // DERIVABLE INTERFACE
-
-  // Creates a reference counted copy.
-  virtual SymbolTable *Copy() const { return new SymbolTable(*this); }
-
-  // Adds a symbol with given key to table. A symbol table also keeps track of
-  // the last available key (highest key value in the symbol table).
-  virtual int64 AddSymbol(const string &symbol, int64 key) {
-    MutateCheck();
-    return impl_->AddSymbol(symbol, key);
-  }
-
-  // Adds a symbol to the table. The associated value key is automatically
-  // assigned by the symbol table.
-  virtual int64 AddSymbol(const string &symbol) {
-    MutateCheck();
-    return impl_->AddSymbol(symbol);
-  }
-
-  // Adds another symbol table to this table. All key values will be offset
-  // by the current available key (highest key value in the symbol table).
-  // Note string symbols with the same key value will still have the same
-  // key value after the symbol table has been merged, but a different
-  // value. Adding symbol tables do not result in changes in the base table.
-  virtual void AddTable(const SymbolTable &table);
-
-  // Returns the current available key (i.e., highest key + 1) in the symbol
-  // table.
-  virtual int64 AvailableKey() const { return impl_->AvailableKey(); }
-
-  // Return the label-agnostic MD5 check-sum for this table. All new symbols
-  // added to the table will result in an updated checksum. Deprecated.
-  virtual const string &CheckSum() const { return impl_->CheckSum(); }
-
-  virtual int64 GetNthKey(ssize_t pos) const { return impl_->GetNthKey(pos); }
-
-  // Returns the string associated with the key; if the key is out of
-  // range (<0, >max), returns an empty string.
-  virtual string Find(int64 key) const { return impl_->Find(key); }
-
-  // Returns the key associated with the symbol; if the symbol does not exist,
-  // kNoSymbol is returned.
-  virtual int64 Find(const string &symbol) const { return impl_->Find(symbol); }
-
-  // Same as CheckSum(), but returns an label-dependent version.
-  virtual const string &LabeledCheckSum() const {
-    return impl_->LabeledCheckSum();
-  }
-
-  virtual bool Member(int64 key) const { return impl_->Member(key); }
-
-  virtual bool Member(const string &symbol) const {
-    return impl_->Member(symbol);
-  }
-
-  // Returns the name of the symbol table.
-  virtual const string &Name() const { return impl_->Name(); }
-
-  // Returns the current number of symbols in table (not necessarily equal to
-  // AvailableKey()).
-  virtual size_t NumSymbols() const { return impl_->NumSymbols(); }
-
-  virtual void RemoveSymbol(int64 key) {
-    MutateCheck();
-    return impl_->RemoveSymbol(key);
+    impl->AddSymbol(symbol, key);
   }
+  return impl.release();
+}
 
-  // Sets the name of the symbol table.
-  virtual void SetName(const string &new_name) {
-    MutateCheck();
-    impl_->SetName(new_name);
+void SymbolTableImpl::MaybeRecomputeCheckSum() const {
+  {
+    ReaderMutexLock check_sum_lock(&check_sum_mutex_);
+    if (check_sum_finalized_) return;
+  }
+  // We'll acquire an exclusive lock to recompute the checksums.
+  MutexLock check_sum_lock(&check_sum_mutex_);
+  if (check_sum_finalized_) {  // Another thread (coming in around the same time
+    return;                    // might have done it already). So we recheck.
+  }
+  // Calculates the original label-agnostic checksum.
+  CheckSummer check_sum;
+  for (size_t i = 0; i < symbols_.Size(); ++i) {
+    const auto &symbol = symbols_.GetSymbol(i);
+    check_sum.Update(symbol.data(), symbol.size());
+    check_sum.Update("", 1);
+  }
+  check_sum_string_ = check_sum.Digest();
+  // Calculates the safer, label-dependent checksum.
+  CheckSummer labeled_check_sum;
+  for (int64 i = 0; i < dense_key_limit_; ++i) {
+    std::ostringstream line;
+    line << symbols_.GetSymbol(i) << '\t' << i;
+    labeled_check_sum.Update(line.str().data(), line.str().size());
+  }
+  using citer = std::map<int64, int64>::const_iterator;
+  for (citer it = key_map_.begin(); it != key_map_.end(); ++it) {
+    // TODO(tombagby, 2013-11-22) This line maintains a bug that ignores
+    // negative labels in the checksum that too many tests rely on.
+    if (it->first < dense_key_limit_) continue;
+    std::ostringstream line;
+    line << symbols_.GetSymbol(it->second) << '\t' << it->first;
+    labeled_check_sum.Update(line.str().data(), line.str().size());
   }
+  labeled_check_sum_string_ = labeled_check_sum.Digest();
+  check_sum_finalized_ = true;
+}
 
-  virtual bool Write(std::ostream &strm) const { return impl_->Write(strm); }
+int64 SymbolTableImpl::AddSymbol(const string &symbol, int64 key) {
+  if (key == kNoSymbol) return key;
+  const auto insert_key = symbols_.InsertOrFind(symbol);
+  if (!insert_key.second) {
+    const auto key_already = GetNthKey(insert_key.first);
+    if (key_already == key) return key;
+    VLOG(1) << "SymbolTable::AddSymbol: symbol = " << symbol
+            << " already in symbol_map_ with key = " << key_already
+            << " but supplied new key = " << key << " (ignoring new key)";
+    return key_already;
+  }
+  if (key + 1 == static_cast<int64>(symbols_.Size()) &&
+      key == dense_key_limit_) {
+    ++dense_key_limit_;
+  } else {
+    idx_key_.push_back(key);
+    key_map_[key] = symbols_.Size() - 1;
+  }
+  if (key >= available_key_) available_key_ = key + 1;
+  check_sum_finalized_ = false;
+  return key;
+}
 
-  virtual bool Write(const string &filename) const {
-    std::ofstream strm(filename,
-                             std::ios_base::out | std::ios_base::binary);
-    if (!strm.good()) {
-      LOG(ERROR) << "SymbolTable::Write: Can't open file " << filename;
-      return false;
+// TODO(rybach): Consider a more efficient implementation which re-uses holes in
+// the dense-key range or re-arranges the dense-key range from time to time.
+void SymbolTableImpl::RemoveSymbol(const int64 key) {
+  auto idx = key;
+  if (key < 0 || key >= dense_key_limit_) {
+    auto iter = key_map_.find(key);
+    if (iter == key_map_.end()) return;
+    idx = iter->second;
+    key_map_.erase(iter);
+  }
+  if (idx < 0 || idx >= static_cast<int64>(symbols_.Size())) return;
+  symbols_.RemoveSymbol(idx);
+  // Removed one symbol, all indexes > idx are shifted by -1.
+  for (auto &k : key_map_) {
+    if (k.second > idx) --k.second;
+  }
+  if (key >= 0 && key < dense_key_limit_) {
+    // Removal puts a hole in the dense key range. Adjusts range to [0, key).
+    const auto new_dense_key_limit = key;
+    for (int64 i = key + 1; i < dense_key_limit_; ++i) {
+      key_map_[i] = i - 1;
+    }
+    // Moves existing values in idx_key to new place.
+    idx_key_.resize(symbols_.Size() - new_dense_key_limit);
+    for (int64 i = symbols_.Size(); i >= dense_key_limit_; --i) {
+      idx_key_[i - new_dense_key_limit - 1] = idx_key_[i - dense_key_limit_];
+    }
+    // Adds indexes for previously dense keys.
+    for (int64 i = new_dense_key_limit; i < dense_key_limit_ - 1; ++i) {
+      idx_key_[i - new_dense_key_limit] = i + 1;
     }
-    return Write(strm);
+    dense_key_limit_ = new_dense_key_limit;
+  } else {
+    // Remove entry for removed index in idx_key.
+    for (size_t i = idx - dense_key_limit_; i + 1 < idx_key_.size(); ++i) {
+      idx_key_[i] = idx_key_[i + 1];
+    }
+    idx_key_.pop_back();
   }
+  if (key == available_key_ - 1) available_key_ = key;
+}
 
-  // Dump a text representation of the symbol table via a stream.
-  virtual bool WriteText(std::ostream &strm,
-      const SymbolTableTextOptions &opts = SymbolTableTextOptions()) const;
-
-  // Dump an text representation of the symbol table.
-  virtual bool WriteText(const string &filename) const {
-    std::ofstream strm(filename);
-    if (!strm.good()) {
-      LOG(ERROR) << "SymbolTable::WriteText: Can't open file " << filename;
-      return false;
+SymbolTableImpl *SymbolTableImpl::Read(
+    std::istream &strm, const SymbolTableReadOptions &) {
+  int32 magic_number = 0;
+  ReadType(strm, &magic_number);
+  if (strm.fail()) {
+    LOG(ERROR) << "SymbolTable::Read: Read failed";
+    return nullptr;
+  }
+  string name;
+  ReadType(strm, &name);
+  std::unique_ptr<SymbolTableImpl> impl(new SymbolTableImpl(name));
+  ReadType(strm, &impl->available_key_);
+  int64 size;
+  ReadType(strm, &size);
+  if (strm.fail()) {
+    LOG(ERROR) << "SymbolTable::Read: Read failed";
+    return nullptr;
+  }
+  string symbol;
+  int64 key;
+  impl->check_sum_finalized_ = false;
+  for (int64 i = 0; i < size; ++i) {
+    ReadType(strm, &symbol);
+    ReadType(strm, &key);
+    if (strm.fail()) {
+      LOG(ERROR) << "SymbolTable::Read: Read failed";
+      return nullptr;
     }
-    return WriteText(strm);
+    impl->AddSymbol(symbol, key);
   }
+  return impl.release();
+}
 
- private:
-  explicit SymbolTable(internal::SymbolTableImpl *impl) : impl_(impl) {}
-
-  void MutateCheck() {
-    if (!impl_.unique()) impl_.reset(new internal::SymbolTableImpl(*impl_));
+bool SymbolTableImpl::Write(std::ostream &strm) const {
+  WriteType(strm, kSymbolTableMagicNumber);
+  WriteType(strm, name_);
+  WriteType(strm, available_key_);
+  const int64 size = symbols_.Size();
+  WriteType(strm, size);
+  for (int64 i = 0; i < size; ++i) {
+    auto key = (i < dense_key_limit_) ? i : idx_key_[i - dense_key_limit_];
+    WriteType(strm, symbols_.GetSymbol(i));
+    WriteType(strm, key);
+  }
+  strm.flush();
+  if (strm.fail()) {
+    LOG(ERROR) << "SymbolTable::Write: Write failed";
+    return false;
   }
+  return true;
+}
 
-  const internal::SymbolTableImpl *Impl() const { return impl_.get(); }
-
- private:
-  std::shared_ptr<internal::SymbolTableImpl> impl_;
-};
-
-// Iterator class for symbols in a symbol table.
-class SymbolTableIterator {
- public:
-  explicit SymbolTableIterator(const SymbolTable &table)
-      : table_(table),
-        pos_(0),
-        nsymbols_(table.NumSymbols()),
-        key_(table.GetNthKey(0)) {}
-
-  ~SymbolTableIterator() {}
-
-  // Returns whether iterator is done.
-  bool Done() const { return (pos_ == nsymbols_); }
-
-  // Return the key of the current symbol.
-  int64 Value() const { return key_; }
-
-  // Return the string of the current symbol.
-  string Symbol() const { return table_.Find(key_); }
-
-  // Advances iterator.
-  void Next() {
-    ++pos_;
-    if (pos_ < nsymbols_) key_ = table_.GetNthKey(pos_);
-  }
+}  // namespace internal
 
-  // Resets iterator.
-  void Reset() {
-    pos_ = 0;
-    key_ = table_.GetNthKey(0);
+void SymbolTable::AddTable(const SymbolTable &table) {
+  MutateCheck();
+  for (SymbolTableIterator iter(table); !iter.Done(); iter.Next()) {
+    impl_->AddSymbol(iter.Symbol());
   }
+}
 
- private:
-  const SymbolTable &table_;
-  ssize_t pos_;
-  size_t nsymbols_;
-  int64 key_;
-};
-
-// Relabels a symbol table as specified by the input vector of pairs
-// (old label, new label). The new symbol table only retains symbols
-// for which a relabeling is explicitly specified.
-//
-// TODO(allauzen): consider adding options to allow for some form of implicit
-// identity relabeling.
-template <class Label>
-SymbolTable *RelabelSymbolTable(const SymbolTable *table,
-    const std::vector<std::pair<Label, Label>> &pairs) {
-  auto *new_table = new SymbolTable(
-      table->Name().empty() ? string()
-                            : (string("relabeled_") + table->Name()));
-  for (const auto &pair : pairs) {
-    new_table->AddSymbol(table->Find(pair.first), pair.second);
+bool SymbolTable::WriteText(std::ostream &strm,
+                            const SymbolTableTextOptions &opts) const {
+  if (opts.fst_field_separator.empty()) {
+    LOG(ERROR) << "Missing required field separator";
+    return false;
+  }
+  bool once_only = false;
+  for (SymbolTableIterator iter(*this); !iter.Done(); iter.Next()) {
+    std::ostringstream line;
+    if (iter.Value() < 0 && !opts.allow_negative_labels && !once_only) {
+      LOG(WARNING) << "Negative symbol table entry when not allowed";
+      once_only = true;
+    }
+    line << iter.Symbol() << opts.fst_field_separator[0] << iter.Value()
+         << '\n';
+    strm.write(line.str().data(), line.str().length());
   }
-  return new_table;
+  return true;
 }
 
-// Returns true if the two symbol tables have equal checksums. Passing in
-// nullptr for either table always returns true.
 bool CompatSymbols(const SymbolTable *syms1, const SymbolTable *syms2,
-                   bool warning = true);
-
-// Symbol Table serialization.
+                   bool warning) {
+  // Flag can explicitly override this check.
+  if (!FLAGS_fst_compat_symbols) return true;
+  if (syms1 && syms2 &&
+      (syms1->LabeledCheckSum() != syms2->LabeledCheckSum())) {
+    if (warning) {
+      LOG(WARNING) << "CompatSymbols: Symbol table checksums do not match. "
+                   << "Table sizes are " << syms1->NumSymbols() << " and "
+                   << syms2->NumSymbols();
+    }
+    return false;
+  } else {
+    return true;
+  }
+}
 
-void SymbolTableToString(const SymbolTable *table, string *result);
+void SymbolTableToString(const SymbolTable *table, string *result) {
+  std::ostringstream ostrm;
+  table->Write(ostrm);
+  *result = ostrm.str();
+}
 
-SymbolTable *StringToSymbolTable(const string &str);
+SymbolTable *StringToSymbolTable(const string &str) {
+  std::istringstream istrm(str);
+  return SymbolTable::Read(istrm, SymbolTableReadOptions());
+}
 
 }  // namespace fst
-
-#endif  // FST_SYMBOL_TABLE_H_
```

### Comparing `sosap-0.0.1/src/openfst/lib/compat.cc` & `sosap-0.1.0/src/openfst/lib/compat.cc`

 * *Files identical despite different names*

### Comparing `sosap-0.0.1/src/openfst/lib/flags.cc` & `sosap-0.1.0/src/openfst/lib/flags.cc`

 * *Files identical despite different names*

### Comparing `sosap-0.0.1/src/openfst/lib/fst-types.cc` & `sosap-0.1.0/src/openfst/lib/fst-types.cc`

 * *Files identical despite different names*

### Comparing `sosap-0.0.1/src/openfst/lib/fst.cc` & `sosap-0.1.0/src/openfst/lib/fst.cc`

 * *Files identical despite different names*

### Comparing `sosap-0.0.1/src/openfst/lib/mapped-file.cc` & `sosap-0.1.0/src/openfst/lib/mapped-file.cc`

 * *Files identical despite different names*

### Comparing `sosap-0.0.1/src/openfst/lib/symbol-table-ops.cc` & `sosap-0.1.0/src/openfst/lib/symbol-table-ops.cc`

 * *Files identical despite different names*

### Comparing `sosap-0.0.1/src/openfst/lib/util.cc` & `sosap-0.1.0/src/openfst/lib/util.cc`

 * *Files identical despite different names*

### Comparing `sosap-0.0.1/src/openfst/lib/weight.cc` & `sosap-0.1.0/src/openfst/lib/weight.cc`

 * *Files identical despite different names*

### Comparing `sosap-0.0.1/src/sosap.egg-info/PKG-INFO` & `sosap-0.1.0/src/sosap.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: sosap
-Version: 0.0.1
+Version: 0.1.0
 Summary: Python binding for Phonetisaurus
 Author-email: Seanghay Yath <seanghay.dev@gmail.com>
 Project-URL: repository, https://github.com/seanghay/sosap
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Cython
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
-## 🗣️ sosap / សូរសព្ទ
+<img width=144 src="https://github.com/seanghay/sosap/assets/15277233/25c2ae30-4dd6-4350-a387-c30353cb2a98">
 
-Python binding for Phonetisaurus
+Python binding for [Phonetisaurus](https://github.com/AdolfVonKleist/Phonetisaurus) using Cython.
 
 ### Install
 
 ```shell
 # pypi
 pip install sosap
 
@@ -29,15 +30,16 @@
 
 ### Usage
 
 ```python
 from sosap import Model
 
 model = Model("g2p.fst")
-
 model.phoneticize("hello")
 ```
 
+---
 
 ### License
 
-MIT
+`MIT`
+
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

