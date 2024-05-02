# Comparing `tmp/bio2zarr-0.0.8.tar.gz` & `tmp/bio2zarr-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bio2zarr-0.0.8.tar", last modified: Wed May  1 07:42:27 2024, max compression
+gzip compressed data, was "bio2zarr-0.0.9.tar", last modified: Thu May  2 10:27:54 2024, max compression
```

## Comparing `bio2zarr-0.0.8.tar` & `bio2zarr-0.0.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2024-05-01 07:42:27.195027 bio2zarr-0.0.8/
-drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2024-05-01 07:42:27.179027 bio2zarr-0.0.8/.github/
-drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2024-05-01 07:42:27.183027 bio2zarr-0.0.8/.github/workflows/
--rw-r--r--   0 jk        (1000) jk        (1000)      789 2024-05-01 07:41:12.000000 bio2zarr-0.0.8/.github/workflows/ci.yml
--rw-r--r--   0 jk        (1000) jk        (1000)     1181 2024-04-24 11:39:12.000000 bio2zarr-0.0.8/.github/workflows/docs.yml
--rw-r--r--   0 jk        (1000) jk        (1000)     2827 2024-05-01 07:41:12.000000 bio2zarr-0.0.8/.gitignore
--rw-r--r--   0 jk        (1000) jk        (1000)      384 2024-05-01 07:41:12.000000 bio2zarr-0.0.8/.pre-commit-config.yaml
--rw-r--r--   0 jk        (1000) jk        (1000)     1280 2024-05-01 07:41:12.000000 bio2zarr-0.0.8/CHANGELOG.md
--rw-r--r--   0 jk        (1000) jk        (1000)    11357 2024-02-14 18:08:29.000000 bio2zarr-0.0.8/LICENSE
--rw-r--r--   0 jk        (1000) jk        (1000)       12 2024-03-27 16:08:22.000000 bio2zarr-0.0.8/MANIFEST.in
--rw-r--r--   0 jk        (1000) jk        (1000)    17401 2024-05-01 07:42:27.195027 bio2zarr-0.0.8/PKG-INFO
--rw-r--r--   0 jk        (1000) jk        (1000)     3075 2024-05-01 07:41:12.000000 bio2zarr-0.0.8/README.md
-drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2024-05-01 07:42:27.187027 bio2zarr-0.0.8/bio2zarr/
--rw-r--r--   0 jk        (1000) jk        (1000)       49 2024-04-17 09:15:58.000000 bio2zarr-0.0.8/bio2zarr/__init__.py
--rw-r--r--   0 jk        (1000) jk        (1000)      527 2024-04-17 09:15:58.000000 bio2zarr-0.0.8/bio2zarr/__main__.py
--rw-r--r--   0 jk        (1000) jk        (1000)      411 2024-05-01 07:42:27.000000 bio2zarr-0.0.8/bio2zarr/_version.py
--rw-r--r--   0 jk        (1000) jk        (1000)    14397 2024-04-24 11:39:37.000000 bio2zarr-0.0.8/bio2zarr/cli.py
--rw-r--r--   0 jk        (1000) jk        (1000)     9006 2024-04-24 22:27:00.000000 bio2zarr-0.0.8/bio2zarr/core.py
--rw-r--r--   0 jk        (1000) jk        (1000)     6768 2024-04-17 09:15:58.000000 bio2zarr-0.0.8/bio2zarr/plink.py
--rw-r--r--   0 jk        (1000) jk        (1000)      142 2024-03-22 09:36:59.000000 bio2zarr-0.0.8/bio2zarr/provenance.py
--rw-r--r--   0 jk        (1000) jk        (1000)       79 2024-04-17 09:15:58.000000 bio2zarr-0.0.8/bio2zarr/typing.py
--rw-r--r--   0 jk        (1000) jk        (1000)    83878 2024-05-01 07:41:12.000000 bio2zarr-0.0.8/bio2zarr/vcf.py
--rw-r--r--   0 jk        (1000) jk        (1000)    17328 2024-05-01 07:41:12.000000 bio2zarr-0.0.8/bio2zarr/vcf_utils.py
-drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2024-05-01 07:42:27.191027 bio2zarr-0.0.8/bio2zarr.egg-info/
--rw-r--r--   0 jk        (1000) jk        (1000)    17401 2024-05-01 07:42:27.000000 bio2zarr-0.0.8/bio2zarr.egg-info/PKG-INFO
--rw-r--r--   0 jk        (1000) jk        (1000)      754 2024-05-01 07:42:27.000000 bio2zarr-0.0.8/bio2zarr.egg-info/SOURCES.txt
--rw-r--r--   0 jk        (1000) jk        (1000)        1 2024-05-01 07:42:27.000000 bio2zarr-0.0.8/bio2zarr.egg-info/dependency_links.txt
--rw-r--r--   0 jk        (1000) jk        (1000)      131 2024-05-01 07:42:27.000000 bio2zarr-0.0.8/bio2zarr.egg-info/entry_points.txt
--rw-r--r--   0 jk        (1000) jk        (1000)      137 2024-05-01 07:42:27.000000 bio2zarr-0.0.8/bio2zarr.egg-info/requires.txt
--rw-r--r--   0 jk        (1000) jk        (1000)        9 2024-05-01 07:42:27.000000 bio2zarr-0.0.8/bio2zarr.egg-info/top_level.txt
-drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2024-05-01 07:42:27.191027 bio2zarr-0.0.8/docs/
--rw-r--r--   0 jk        (1000) jk        (1000)      489 2024-04-19 14:33:24.000000 bio2zarr-0.0.8/docs/Makefile
--rw-r--r--   0 jk        (1000) jk        (1000)     1041 2024-04-19 14:33:24.000000 bio2zarr-0.0.8/docs/_config.yml
--rw-r--r--   0 jk        (1000) jk        (1000)       50 2024-04-19 14:33:24.000000 bio2zarr-0.0.8/docs/_toc.yml
--rwxr-xr-x   0 jk        (1000) jk        (1000)      505 2024-04-19 14:33:24.000000 bio2zarr-0.0.8/docs/build.sh
--rw-r--r--   0 jk        (1000) jk        (1000)      182 2024-04-19 14:33:24.000000 bio2zarr-0.0.8/docs/cli.md
--rw-r--r--   0 jk        (1000) jk        (1000)     1947 2024-04-19 14:33:24.000000 bio2zarr-0.0.8/docs/intro.md
--rw-r--r--   0 jk        (1000) jk        (1000)   107441 2024-04-19 14:33:24.000000 bio2zarr-0.0.8/docs/logo.png
--rw-r--r--   0 jk        (1000) jk        (1000)        9 2024-04-19 14:33:24.000000 bio2zarr-0.0.8/docs/references.bib
--rw-r--r--   0 jk        (1000) jk        (1000)       94 2024-04-19 14:51:51.000000 bio2zarr-0.0.8/docs/requirements.txt
--rw-r--r--   0 jk        (1000) jk        (1000)     2098 2024-05-01 07:41:12.000000 bio2zarr-0.0.8/pyproject.toml
--rw-r--r--   0 jk        (1000) jk        (1000)       38 2024-05-01 07:42:27.195027 bio2zarr-0.0.8/setup.cfg
-drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2024-05-01 07:42:27.191027 bio2zarr-0.0.8/validation-data/
--rw-r--r--   0 jk        (1000) jk        (1000)     2985 2024-02-29 11:43:51.000000 bio2zarr-0.0.8/validation-data/Makefile
--rwxr-xr-x   0 jk        (1000) jk        (1000)      323 2024-02-29 11:43:51.000000 bio2zarr-0.0.8/validation-data/split.sh
--rw-r--r--   0 jk        (1000) jk        (1000)     2323 2024-04-17 09:15:58.000000 bio2zarr-0.0.8/validation.py
--rw-r--r--   0 jk        (1000) jk        (1000)      959 2024-04-17 09:17:44.000000 bio2zarr-0.0.8/vcf_generator.py
+drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2024-05-02 10:27:54.473099 bio2zarr-0.0.9/
+drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2024-05-02 10:27:54.441098 bio2zarr-0.0.9/.github/
+drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2024-05-02 10:27:54.445098 bio2zarr-0.0.9/.github/workflows/
+-rw-r--r--   0 jk        (1000) jk        (1000)      789 2024-05-01 07:41:12.000000 bio2zarr-0.0.9/.github/workflows/ci.yml
+-rw-r--r--   0 jk        (1000) jk        (1000)     1181 2024-04-24 11:39:12.000000 bio2zarr-0.0.9/.github/workflows/docs.yml
+-rw-r--r--   0 jk        (1000) jk        (1000)     2827 2024-05-01 07:41:12.000000 bio2zarr-0.0.9/.gitignore
+-rw-r--r--   0 jk        (1000) jk        (1000)      384 2024-05-01 07:41:12.000000 bio2zarr-0.0.9/.pre-commit-config.yaml
+-rw-r--r--   0 jk        (1000) jk        (1000)     1406 2024-05-02 10:27:41.000000 bio2zarr-0.0.9/CHANGELOG.md
+-rw-r--r--   0 jk        (1000) jk        (1000)    11357 2024-02-14 18:08:29.000000 bio2zarr-0.0.9/LICENSE
+-rw-r--r--   0 jk        (1000) jk        (1000)       12 2024-03-27 16:08:22.000000 bio2zarr-0.0.9/MANIFEST.in
+-rw-r--r--   0 jk        (1000) jk        (1000)    17408 2024-05-02 10:27:54.473099 bio2zarr-0.0.9/PKG-INFO
+-rw-r--r--   0 jk        (1000) jk        (1000)     3075 2024-05-01 07:41:12.000000 bio2zarr-0.0.9/README.md
+drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2024-05-02 10:27:54.453098 bio2zarr-0.0.9/bio2zarr/
+-rw-r--r--   0 jk        (1000) jk        (1000)       49 2024-04-17 09:15:58.000000 bio2zarr-0.0.9/bio2zarr/__init__.py
+-rw-r--r--   0 jk        (1000) jk        (1000)      527 2024-04-17 09:15:58.000000 bio2zarr-0.0.9/bio2zarr/__main__.py
+-rw-r--r--   0 jk        (1000) jk        (1000)      411 2024-05-02 10:27:54.000000 bio2zarr-0.0.9/bio2zarr/_version.py
+-rw-r--r--   0 jk        (1000) jk        (1000)    14376 2024-05-01 22:40:11.000000 bio2zarr-0.0.9/bio2zarr/cli.py
+-rw-r--r--   0 jk        (1000) jk        (1000)     9006 2024-04-24 22:27:00.000000 bio2zarr-0.0.9/bio2zarr/core.py
+-rw-r--r--   0 jk        (1000) jk        (1000)     6768 2024-04-17 09:15:58.000000 bio2zarr-0.0.9/bio2zarr/plink.py
+-rw-r--r--   0 jk        (1000) jk        (1000)      142 2024-03-22 09:36:59.000000 bio2zarr-0.0.9/bio2zarr/provenance.py
+-rw-r--r--   0 jk        (1000) jk        (1000)       79 2024-04-17 09:15:58.000000 bio2zarr-0.0.9/bio2zarr/typing.py
+-rw-r--r--   0 jk        (1000) jk        (1000)    84757 2024-05-02 09:57:34.000000 bio2zarr-0.0.9/bio2zarr/vcf.py
+-rw-r--r--   0 jk        (1000) jk        (1000)    17777 2024-05-01 22:40:18.000000 bio2zarr-0.0.9/bio2zarr/vcf_utils.py
+drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2024-05-02 10:27:54.469099 bio2zarr-0.0.9/bio2zarr.egg-info/
+-rw-r--r--   0 jk        (1000) jk        (1000)    17408 2024-05-02 10:27:54.000000 bio2zarr-0.0.9/bio2zarr.egg-info/PKG-INFO
+-rw-r--r--   0 jk        (1000) jk        (1000)      754 2024-05-02 10:27:54.000000 bio2zarr-0.0.9/bio2zarr.egg-info/SOURCES.txt
+-rw-r--r--   0 jk        (1000) jk        (1000)        1 2024-05-02 10:27:54.000000 bio2zarr-0.0.9/bio2zarr.egg-info/dependency_links.txt
+-rw-r--r--   0 jk        (1000) jk        (1000)      131 2024-05-02 10:27:54.000000 bio2zarr-0.0.9/bio2zarr.egg-info/entry_points.txt
+-rw-r--r--   0 jk        (1000) jk        (1000)      144 2024-05-02 10:27:54.000000 bio2zarr-0.0.9/bio2zarr.egg-info/requires.txt
+-rw-r--r--   0 jk        (1000) jk        (1000)        9 2024-05-02 10:27:54.000000 bio2zarr-0.0.9/bio2zarr.egg-info/top_level.txt
+drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2024-05-02 10:27:54.465099 bio2zarr-0.0.9/docs/
+-rw-r--r--   0 jk        (1000) jk        (1000)      489 2024-04-19 14:33:24.000000 bio2zarr-0.0.9/docs/Makefile
+-rw-r--r--   0 jk        (1000) jk        (1000)     1041 2024-04-19 14:33:24.000000 bio2zarr-0.0.9/docs/_config.yml
+-rw-r--r--   0 jk        (1000) jk        (1000)       50 2024-04-19 14:33:24.000000 bio2zarr-0.0.9/docs/_toc.yml
+-rwxr-xr-x   0 jk        (1000) jk        (1000)      505 2024-04-19 14:33:24.000000 bio2zarr-0.0.9/docs/build.sh
+-rw-r--r--   0 jk        (1000) jk        (1000)      182 2024-04-19 14:33:24.000000 bio2zarr-0.0.9/docs/cli.md
+-rw-r--r--   0 jk        (1000) jk        (1000)     1947 2024-04-19 14:33:24.000000 bio2zarr-0.0.9/docs/intro.md
+-rw-r--r--   0 jk        (1000) jk        (1000)   107441 2024-04-19 14:33:24.000000 bio2zarr-0.0.9/docs/logo.png
+-rw-r--r--   0 jk        (1000) jk        (1000)        9 2024-04-19 14:33:24.000000 bio2zarr-0.0.9/docs/references.bib
+-rw-r--r--   0 jk        (1000) jk        (1000)       94 2024-04-19 14:51:51.000000 bio2zarr-0.0.9/docs/requirements.txt
+-rw-r--r--   0 jk        (1000) jk        (1000)     2105 2024-05-01 22:40:11.000000 bio2zarr-0.0.9/pyproject.toml
+-rw-r--r--   0 jk        (1000) jk        (1000)       38 2024-05-02 10:27:54.473099 bio2zarr-0.0.9/setup.cfg
+drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2024-05-02 10:27:54.469099 bio2zarr-0.0.9/validation-data/
+-rw-r--r--   0 jk        (1000) jk        (1000)     3121 2024-05-02 09:45:38.000000 bio2zarr-0.0.9/validation-data/Makefile
+-rwxr-xr-x   0 jk        (1000) jk        (1000)      323 2024-02-29 11:43:51.000000 bio2zarr-0.0.9/validation-data/split.sh
+-rw-r--r--   0 jk        (1000) jk        (1000)     2323 2024-04-17 09:15:58.000000 bio2zarr-0.0.9/validation.py
+-rw-r--r--   0 jk        (1000) jk        (1000)      959 2024-04-17 09:17:44.000000 bio2zarr-0.0.9/vcf_generator.py
```

### Comparing `bio2zarr-0.0.8/.github/workflows/ci.yml` & `bio2zarr-0.0.9/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `bio2zarr-0.0.8/.github/workflows/docs.yml` & `bio2zarr-0.0.9/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `bio2zarr-0.0.8/.gitignore` & `bio2zarr-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `bio2zarr-0.0.8/CHANGELOG.md` & `bio2zarr-0.0.9/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,15 @@
-# 0.0.7 2024-04-30
+# 0.0.9 2024-05-02
+
+- Change on-disk format for explode and schema
+- Support older tabix indexes
+- Fix some bugs in explode
+
+# 0.0.8 2024-04-30
+
 - Change on-disk format of distributed encode and simplify
 - Check for all partitions nominally completed encoding before doing
   anything destructive in dencode-finalise
 
 # 0.0.6 2024-04-24
 
 - Only use NOSHUFFLE by default on ``call_genotype`` and bool arrays.
```

### Comparing `bio2zarr-0.0.8/LICENSE` & `bio2zarr-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bio2zarr-0.0.8/PKG-INFO` & `bio2zarr-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bio2zarr
-Version: 0.0.8
+Version: 0.0.9
 Summary: Convert bioinformatics data to Zarr
 Author-email: sgkit Developers <project@sgkit.dev>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -230,15 +230,15 @@
 Requires-Dist: bed_reader
 Provides-Extra: dev
 Requires-Dist: msprime; extra == "dev"
 Requires-Dist: pysam; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-coverage; extra == "dev"
 Requires-Dist: pytest-xdist; extra == "dev"
-Requires-Dist: sgkit; extra == "dev"
+Requires-Dist: sgkit>=0.8.0; extra == "dev"
 Requires-Dist: tqdm; extra == "dev"
 
 [![CI](https://github.com/sgkit-dev/bio2zarr/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/sgkit-dev/bio2zarr/actions/workflows/ci.yml)
 
 # bio2zarr
 Convert bioinformatics file formats to Zarr
```

### Comparing `bio2zarr-0.0.8/README.md` & `bio2zarr-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `bio2zarr-0.0.8/bio2zarr/__main__.py` & `bio2zarr-0.0.9/bio2zarr/__main__.py`

 * *Files identical despite different names*

### Comparing `bio2zarr-0.0.8/bio2zarr/cli.py` & `bio2zarr-0.0.9/bio2zarr/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -229,15 +229,15 @@
 def dexplode_partition(icf_path, partition, verbose):
     """
     Convert a VCF partition to intermediate columnar format. Must be called *after*
     the ICF path has been initialised with dexplode_init. Partition indexes must be
     from 0 (inclusive) to the number of paritions returned by dexplode_init (exclusive).
     """
     setup_logging(verbose)
-    vcf.explode_partition(icf_path, partition, show_progress=False)
+    vcf.explode_partition(icf_path, partition)
 
 
 @click.command
 @icf_path
 @verbose
 def dexplode_finalise(icf_path, verbose):
     """
```

### Comparing `bio2zarr-0.0.8/bio2zarr/core.py` & `bio2zarr-0.0.9/bio2zarr/core.py`

 * *Files identical despite different names*

### Comparing `bio2zarr-0.0.8/bio2zarr/plink.py` & `bio2zarr-0.0.9/bio2zarr/plink.py`

 * *Files identical despite different names*

### Comparing `bio2zarr-0.0.8/bio2zarr/vcf.py` & `bio2zarr-0.0.9/bio2zarr/vcf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import collections
 import contextlib
 import dataclasses
-import functools
 import json
 import logging
 import math
 import os
 import os.path
 import pathlib
 import pickle
@@ -141,37 +140,49 @@
 @dataclasses.dataclass
 class VcfPartition:
     vcf_path: str
     region: str
     num_records: int = -1
 
 
-ICF_METADATA_FORMAT_VERSION = "0.2"
+ICF_METADATA_FORMAT_VERSION = "0.3"
 ICF_DEFAULT_COMPRESSOR = numcodecs.Blosc(
     cname="zstd", clevel=7, shuffle=numcodecs.Blosc.NOSHUFFLE
 )
 
-# TODO refactor this to have embedded Contig dataclass, Filters
-# and Samples dataclasses to allow for more information to be
-# retained and forward compatibility.
+
+@dataclasses.dataclass
+class Contig:
+    id: str
+    length: int = None
+
+
+@dataclasses.dataclass
+class Sample:
+    id: str
+
+
+@dataclasses.dataclass
+class Filter:
+    id: str
+    description: str = ""
 
 
 @dataclasses.dataclass
 class IcfMetadata:
     samples: list
-    contig_names: list
-    contig_record_counts: dict
+    contigs: list
     filters: list
     fields: list
     partitions: list = None
-    contig_lengths: list = None
     format_version: str = None
     compressor: dict = None
     column_chunk_size: int = None
     provenance: dict = None
+    num_records: int = -1
 
     @property
     def info_fields(self):
         fields = []
         for field in self.fields:
             if field.category == "INFO":
                 fields.append(field)
@@ -183,43 +194,44 @@
         for field in self.fields:
             if field.category == "FORMAT":
                 fields.append(field)
         return fields
 
     @property
     def num_contigs(self):
-        return len(self.contig_names)
+        return len(self.contigs)
 
     @property
     def num_filters(self):
         return len(self.filters)
 
-    @property
-    def num_records(self):
-        return sum(self.contig_record_counts.values())
-
     @staticmethod
     def fromdict(d):
         if d["format_version"] != ICF_METADATA_FORMAT_VERSION:
             raise ValueError(
                 "Intermediate columnar metadata format version mismatch: "
                 f"{d['format_version']} != {ICF_METADATA_FORMAT_VERSION}"
             )
-        fields = [VcfField.fromdict(fd) for fd in d["fields"]]
         partitions = [VcfPartition(**pd) for pd in d["partitions"]]
         for p in partitions:
             p.region = vcf_utils.Region(**p.region)
         d = d.copy()
-        d["fields"] = fields
         d["partitions"] = partitions
+        d["fields"] = [VcfField.fromdict(fd) for fd in d["fields"]]
+        d["samples"] = [Sample(**sd) for sd in d["samples"]]
+        d["filters"] = [Filter(**fd) for fd in d["filters"]]
+        d["contigs"] = [Contig(**cd) for cd in d["contigs"]]
         return IcfMetadata(**d)
 
     def asdict(self):
         return dataclasses.asdict(self)
 
+    def asjson(self):
+        return json.dumps(self.asdict(), indent=4)
+
 
 def fixed_vcf_field_definitions():
     def make_field_def(name, vcf_type, vcf_number):
         return VcfField(
             category="fixed",
             name=name,
             vcf_type=vcf_type,
@@ -239,45 +251,56 @@
     ]
     return fields
 
 
 def scan_vcf(path, target_num_partitions):
     with vcf_utils.IndexedVcf(path) as indexed_vcf:
         vcf = indexed_vcf.vcf
-        filters = [
-            h["ID"]
-            for h in vcf.header_iter()
-            if h["HeaderType"] == "FILTER" and isinstance(h["ID"], str)
-        ]
+        filters = []
+        pass_index = -1
+        for h in vcf.header_iter():
+            if h["HeaderType"] == "FILTER" and isinstance(h["ID"], str):
+                try:
+                    description = h["Description"].strip('"')
+                except KeyError:
+                    description = ""
+                if h["ID"] == "PASS":
+                    pass_index = len(filters)
+                filters.append(Filter(h["ID"], description))
+
         # Ensure PASS is the first filter if present
-        if "PASS" in filters:
-            filters.remove("PASS")
-            filters.insert(0, "PASS")
+        if pass_index > 0:
+            pass_filter = filters.pop(pass_index)
+            filters.insert(0, pass_filter)
 
         fields = fixed_vcf_field_definitions()
         for h in vcf.header_iter():
             if h["HeaderType"] in ["INFO", "FORMAT"]:
                 field = VcfField.from_header(h)
                 if field.name == "GT":
                     field.vcf_type = "Integer"
                     field.vcf_number = "."
                 fields.append(field)
 
+        try:
+            contig_lengths = vcf.seqlens
+        except AttributeError:
+            contig_lengths = [None for _ in vcf.seqnames]
+
         metadata = IcfMetadata(
-            samples=vcf.samples,
-            contig_names=vcf.seqnames,
-            contig_record_counts=indexed_vcf.contig_record_counts(),
+            samples=[Sample(sample_id) for sample_id in vcf.samples],
+            contigs=[
+                Contig(contig_id, length)
+                for contig_id, length in zip(vcf.seqnames, contig_lengths)
+            ],
             filters=filters,
             fields=fields,
             partitions=[],
+            num_records=sum(indexed_vcf.contig_record_counts().values()),
         )
-        try:
-            metadata.contig_lengths = vcf.seqlens
-        except AttributeError:
-            pass
 
         regions = indexed_vcf.partition_into_regions(num_parts=target_num_partitions)
         logger.info(
             f"Split {path} into {len(regions)} regions (target={target_num_partitions})"
         )
         for region in regions:
             metadata.partitions.append(
@@ -288,30 +311,14 @@
                     region=region,
                 )
             )
         core.update_progress(1)
         return metadata, vcf.raw_header
 
 
-def check_overlap(partitions):
-    for i in range(1, len(partitions)):
-        prev_region = partitions[i - 1].region
-        current_region = partitions[i].region
-        if prev_region.contig == current_region.contig:
-            if prev_region.end is None:
-                logger.warning("Cannot check overlaps; issue #146")
-                continue
-            if prev_region.end > current_region.start:
-                raise ValueError(
-                    f"Multiple VCFs have the region "
-                    f"{prev_region.contig}:{prev_region.start}-"
-                    f"{current_region.end}"
-                )
-
-
 def scan_vcfs(paths, show_progress, target_num_partitions, worker_processes=1):
     logger.info(
         f"Scanning {len(paths)} VCFs attempting to split into {target_num_partitions}"
         f" partitions."
     )
     # An easy mistake to make is to pass the same file twice. Check this early on.
     for path, count in collections.Counter(paths).items():
@@ -332,35 +339,38 @@
         results = list(pwm.results_as_completed())
 
     # Sort to make the ordering deterministic
     results.sort(key=lambda t: t[0].partitions[0].vcf_path)
     # We just take the first header, assuming the others
     # are compatible.
     all_partitions = []
-    contig_record_counts = collections.Counter()
+    total_records = 0
     for metadata, _ in results:
-        all_partitions.extend(metadata.partitions)
-        metadata.partitions.clear()
-        contig_record_counts += metadata.contig_record_counts
-        metadata.contig_record_counts.clear()
+        for partition in metadata.partitions:
+            logger.debug(f"Scanned partition {partition}")
+            all_partitions.append(partition)
+        total_records += metadata.num_records
+        metadata.num_records = 0
+        metadata.partitions = []
 
     icf_metadata, header = results[0]
     for metadata, _ in results[1:]:
         if metadata != icf_metadata:
             raise ValueError("Incompatible VCF chunks")
 
-    icf_metadata.contig_record_counts = dict(contig_record_counts)
+    # Note: this will be infinity here if any of the chunks has an index
+    # that doesn't keep track of the number of records per-contig
+    icf_metadata.num_records = total_records
 
     # Sort by contig (in the order they appear in the header) first,
     # then by start coordinate
-    contig_index_map = {contig: j for j, contig in enumerate(metadata.contig_names)}
+    contig_index_map = {contig.id: j for j, contig in enumerate(metadata.contigs)}
     all_partitions.sort(
         key=lambda x: (contig_index_map[x.region.contig], x.region.start)
     )
-    check_overlap(all_partitions)
     icf_metadata.partitions = all_partitions
     logger.info(f"Scan complete, resulting in {len(all_partitions)} partitions.")
     return icf_metadata, header
 
 
 def sanitise_value_bool(buff, j, value):
     x = True
@@ -849,48 +859,47 @@
         self.path = pathlib.Path(path)
         # TODO raise a more informative error here telling people this
         # directory is either a WIP or the wrong format.
         with open(self.path / "metadata.json") as f:
             self.metadata = IcfMetadata.fromdict(json.load(f))
         with open(self.path / "header.txt") as f:
             self.vcf_header = f.read()
-
         self.compressor = numcodecs.get_codec(self.metadata.compressor)
-        self.columns = {}
+        self.fields = {}
         partition_num_records = [
             partition.num_records for partition in self.metadata.partitions
         ]
         # Allow us to find which partition a given record is in
         self.partition_record_index = np.cumsum([0, *partition_num_records])
         for field in self.metadata.fields:
-            self.columns[field.full_name] = IntermediateColumnarFormatField(self, field)
+            self.fields[field.full_name] = IntermediateColumnarFormatField(self, field)
         logger.info(
             f"Loaded IntermediateColumnarFormat(partitions={self.num_partitions}, "
-            f"records={self.num_records}, columns={self.num_columns})"
+            f"records={self.num_records}, fields={self.num_fields})"
         )
 
     def __repr__(self):
         return (
             f"IntermediateColumnarFormat(fields={len(self)}, "
             f"partitions={self.num_partitions}, "
             f"records={self.num_records}, path={self.path})"
         )
 
     def __getitem__(self, key):
-        return self.columns[key]
+        return self.fields[key]
 
     def __iter__(self):
-        return iter(self.columns)
+        return iter(self.fields)
 
     def __len__(self):
-        return len(self.columns)
+        return len(self.fields)
 
     def summary_table(self):
         data = []
-        for name, col in self.columns.items():
+        for name, col in self.fields.items():
             summary = col.vcf_field.summary
             d = {
                 "name": name,
                 "type": col.vcf_field.vcf_type,
                 "chunks": summary.num_chunks,
                 "size": display_size(summary.uncompressed_size),
                 "compressed": display_size(summary.compressed_size),
@@ -898,29 +907,63 @@
                 "min_val": display_number(summary.min_value),
                 "max_val": display_number(summary.max_value),
             }
 
             data.append(d)
         return data
 
-    @functools.cached_property
+    @property
     def num_records(self):
-        return sum(self.metadata.contig_record_counts.values())
+        return self.metadata.num_records
 
     @property
     def num_partitions(self):
         return len(self.metadata.partitions)
 
     @property
     def num_samples(self):
         return len(self.metadata.samples)
 
     @property
-    def num_columns(self):
-        return len(self.columns)
+    def num_fields(self):
+        return len(self.fields)
+
+
+@dataclasses.dataclass
+class IcfPartitionMetadata:
+    num_records: int
+    last_position: int
+    field_summaries: dict
+
+    def asdict(self):
+        return dataclasses.asdict(self)
+
+    def asjson(self):
+        return json.dumps(self.asdict(), indent=4)
+
+    @staticmethod
+    def fromdict(d):
+        md = IcfPartitionMetadata(**d)
+        for k, v in md.field_summaries.items():
+            md.field_summaries[k] = VcfFieldSummary.fromdict(v)
+        return md
+
+
+def check_overlapping_partitions(partitions):
+    for i in range(1, len(partitions)):
+        prev_region = partitions[i - 1].region
+        current_region = partitions[i].region
+        if prev_region.contig == current_region.contig:
+            assert prev_region.end is not None
+            # Regions are *inclusive*
+            if prev_region.end >= current_region.start:
+                raise ValueError(
+                    f"Overlapping VCF regions in partitions {i - 1} and {i}: "
+                    f"{prev_region} and {current_region}"
+                )
 
 
 class IntermediateColumnarFormatWriter:
     def __init__(self, path):
         self.path = pathlib.Path(path)
         self.wip_path = self.path / "wip"
         self.metadata = None
@@ -986,19 +1029,16 @@
             col_path.mkdir(parents=True)
 
     def load_partition_summaries(self):
         summaries = []
         not_found = []
         for j in range(self.num_partitions):
             try:
-                with open(self.wip_path / f"p{j}_summary.json") as f:
-                    summary = json.load(f)
-                    for k, v in summary["field_summaries"].items():
-                        summary["field_summaries"][k] = VcfFieldSummary.fromdict(v)
-                    summaries.append(summary)
+                with open(self.wip_path / f"p{j}.json") as f:
+                    summaries.append(IcfPartitionMetadata.fromdict(json.load(f)))
             except FileNotFoundError:
                 not_found.append(j)
         if len(not_found) > 0:
             raise FileNotFoundError(
                 f"Partition metadata not found for {len(not_found)}"
                 f" partitions: {not_found}"
             )
@@ -1007,15 +1047,15 @@
     def load_metadata(self):
         if self.metadata is None:
             with open(self.wip_path / "metadata.json") as f:
                 self.metadata = IcfMetadata.fromdict(json.load(f))
 
     def process_partition(self, partition_index):
         self.load_metadata()
-        summary_path = self.wip_path / f"p{partition_index}_summary.json"
+        summary_path = self.wip_path / f"p{partition_index}.json"
         # If someone is rewriting a summary path (for whatever reason), make sure it
         # doesn't look like it's already been completed.
         # NOTE to do this properly we probably need to take a lock on this file - but
         # this simple approach will catch the vast majority of problems.
         if summary_path.exists():
             summary_path.unlink()
 
@@ -1028,23 +1068,25 @@
         has_gt = False
         for field in self.metadata.format_fields:
             if field.name == "GT":
                 has_gt = True
             else:
                 format_fields.append(field)
 
+        last_position = None
         with IcfPartitionWriter(
             self.metadata,
             self.path,
             partition_index,
         ) as tcw:
             with vcf_utils.IndexedVcf(partition.vcf_path) as ivcf:
                 num_records = 0
                 for variant in ivcf.variants(partition.region):
                     num_records += 1
+                    last_position = variant.POS
                     tcw.append("CHROM", variant.CHROM)
                     tcw.append("POS", variant.POS)
                     tcw.append("QUAL", variant.QUAL)
                     tcw.append("ID", variant.ID)
                     tcw.append("FILTERS", variant.FILTERS)
                     tcw.append("REF", variant.REF)
                     tcw.append("ALT", variant.ALT)
@@ -1061,96 +1103,86 @@
                     # done about it.
                     core.update_progress(1)
             logger.info(
                 f"Finished reading VCF for partition {partition_index}, "
                 f"flushing buffers"
             )
 
-        partition_metadata = {
-            "num_records": num_records,
-            "field_summaries": {k: v.asdict() for k, v in tcw.field_summaries.items()},
-        }
+        partition_metadata = IcfPartitionMetadata(
+            num_records=num_records,
+            last_position=last_position,
+            field_summaries=tcw.field_summaries,
+        )
         with open(summary_path, "w") as f:
-            json.dump(partition_metadata, f, indent=4)
+            f.write(partition_metadata.asjson())
         logger.info(
-            f"Finish p{partition_index} {partition.vcf_path}__{partition.region}="
-            f"{num_records} records"
+            f"Finish p{partition_index} {partition.vcf_path}__{partition.region} "
+            f"{num_records} records last_pos={last_position}"
         )
 
-    def process_partition_slice(
-        self,
-        start,
-        stop,
-        *,
-        worker_processes=1,
-        show_progress=False,
-    ):
+    def explode(self, *, worker_processes=1, show_progress=False):
         self.load_metadata()
-        if start == 0 and stop == self.num_partitions:
-            num_records = self.metadata.num_records
-        else:
-            # We only know the number of records if all partitions are done at once,
-            # and we signal this to tqdm by passing None as the total.
+        num_records = self.metadata.num_records
+        if np.isinf(num_records):
+            logger.warning(
+                "Total records unknown, cannot show progress; "
+                "reindex VCFs with bcftools index to fix"
+            )
             num_records = None
-        num_columns = len(self.metadata.fields)
+        num_fields = len(self.metadata.fields)
         num_samples = len(self.metadata.samples)
         logger.info(
-            f"Exploding columns={num_columns} samples={num_samples}; "
-            f"partitions={stop - start} "
+            f"Exploding fields={num_fields} samples={num_samples}; "
+            f"partitions={self.num_partitions} "
             f"variants={'unknown' if num_records is None else num_records}"
         )
         progress_config = core.ProgressConfig(
             total=num_records,
             units="vars",
             title="Explode",
             show=show_progress,
         )
         with core.ParallelWorkManager(worker_processes, progress_config) as pwm:
-            for j in range(start, stop):
+            for j in range(self.num_partitions):
                 pwm.submit(self.process_partition, j)
 
-    def explode(self, *, worker_processes=1, show_progress=False):
-        self.load_metadata()
-        return self.process_partition_slice(
-            0,
-            self.num_partitions,
-            worker_processes=worker_processes,
-            show_progress=show_progress,
-        )
-
-    def explode_partition(self, partition, *, show_progress=False, worker_processes=1):
+    def explode_partition(self, partition):
         self.load_metadata()
         if partition < 0 or partition >= self.num_partitions:
             raise ValueError(
                 "Partition index must be in the range 0 <= index < num_partitions"
             )
-        return self.process_partition_slice(
-            partition,
-            partition + 1,
-            worker_processes=worker_processes,
-            show_progress=show_progress,
-        )
+        self.process_partition(partition)
 
     def finalise(self):
         self.load_metadata()
         partition_summaries = self.load_partition_summaries()
         total_records = 0
         for index, summary in enumerate(partition_summaries):
-            partition_records = summary["num_records"]
+            partition_records = summary.num_records
             self.metadata.partitions[index].num_records = partition_records
+            self.metadata.partitions[index].region.end = summary.last_position
             total_records += partition_records
-        assert total_records == self.metadata.num_records
+        if not np.isinf(self.metadata.num_records):
+            # Note: this is just telling us that there's a bug in the
+            # index based record counting code, but it doesn't actually
+            # matter much. We may want to just make this a warning if
+            # we hit regular problems.
+            assert total_records == self.metadata.num_records
+        self.metadata.num_records = total_records
+
+        check_overlapping_partitions(self.metadata.partitions)
 
         for field in self.metadata.fields:
             for summary in partition_summaries:
-                field.summary.update(summary["field_summaries"][field.full_name])
+                field.summary.update(summary.field_summaries[field.full_name])
 
         logger.info("Finalising metadata")
         with open(self.path / "metadata.json", "w") as f:
-            json.dump(self.metadata.asdict(), f, indent=4)
+            f.write(self.metadata.asjson())
 
         logger.debug("Removing WIP directory")
         shutil.rmtree(self.wip_path)
 
 
 def explode(
     icf_path,
@@ -1193,22 +1225,17 @@
         worker_processes=worker_processes,
         show_progress=show_progress,
         column_chunk_size=column_chunk_size,
         compressor=compressor,
     )
 
 
-# NOTE only including worker_processes here so we can use the 0 option to get the
-# work done syncronously and so we can get test coverage on it. Should find a
-# better way to do this.
-def explode_partition(icf_path, partition, *, show_progress=False, worker_processes=1):
+def explode_partition(icf_path, partition):
     writer = IntermediateColumnarFormatWriter(icf_path)
-    writer.explode_partition(
-        partition, show_progress=show_progress, worker_processes=worker_processes
-    )
+    writer.explode_partition(partition)
 
 
 def explode_finalise(icf_path):
     writer = IntermediateColumnarFormatWriter(icf_path)
     writer.finalise()
 
 
@@ -1328,28 +1355,27 @@
         chunk_items = self.chunks[0]
         for size in self.shape[1:]:
             chunk_items *= size
         dt = np.dtype(self.dtype)
         return chunk_items * dt.itemsize
 
 
-ZARR_SCHEMA_FORMAT_VERSION = "0.2"
+ZARR_SCHEMA_FORMAT_VERSION = "0.3"
 
 
 @dataclasses.dataclass
 class VcfZarrSchema:
     format_version: str
     samples_chunk_size: int
     variants_chunk_size: int
     dimensions: list
-    sample_id: list
-    contig_id: list
-    contig_length: list
-    filter_id: list
-    columns: dict
+    samples: list
+    contigs: list
+    filters: list
+    fields: dict
 
     def asdict(self):
         return dataclasses.asdict(self)
 
     def asjson(self):
         return json.dumps(self.asdict(), indent=4)
 
@@ -1357,16 +1383,19 @@
     def fromdict(d):
         if d["format_version"] != ZARR_SCHEMA_FORMAT_VERSION:
             raise ValueError(
                 "Zarr schema format version mismatch: "
                 f"{d['format_version']} != {ZARR_SCHEMA_FORMAT_VERSION}"
             )
         ret = VcfZarrSchema(**d)
-        ret.columns = {
-            key: ZarrColumnSpec(**value) for key, value in d["columns"].items()
+        ret.samples = [Sample(**sd) for sd in d["samples"]]
+        ret.contigs = [Contig(**sd) for sd in d["contigs"]]
+        ret.filters = [Filter(**sd) for sd in d["filters"]]
+        ret.fields = {
+            key: ZarrColumnSpec(**value) for key, value in d["fields"].items()
         }
         return ret
 
     @staticmethod
     def fromjson(s):
         return VcfZarrSchema.fromdict(json.loads(s))
 
@@ -1402,15 +1431,15 @@
                 dtype=dtype,
                 shape=shape,
                 description="",
                 dimensions=dimensions,
                 chunks=[variants_chunk_size],
             )
 
-        alt_col = icf.columns["ALT"]
+        alt_col = icf.fields["ALT"]
         max_alleles = alt_col.vcf_field.summary.max_number + 1
 
         colspecs = [
             fixed_field_spec(
                 name="variant_contig",
                 dtype=core.min_int_dtype(0, icf.metadata.num_contigs),
             ),
@@ -1494,20 +1523,19 @@
                 )
             )
 
         return VcfZarrSchema(
             format_version=ZARR_SCHEMA_FORMAT_VERSION,
             samples_chunk_size=samples_chunk_size,
             variants_chunk_size=variants_chunk_size,
-            columns={col.name: col for col in colspecs},
+            fields={col.name: col for col in colspecs},
             dimensions=["variants", "samples", "ploidy", "alleles", "filters"],
-            sample_id=icf.metadata.samples,
-            contig_id=icf.metadata.contig_names,
-            contig_length=icf.metadata.contig_lengths,
-            filter_id=icf.metadata.filters,
+            samples=icf.metadata.samples,
+            contigs=icf.metadata.contigs,
+            filters=icf.metadata.filters,
         )
 
 
 class VcfZarr:
     def __init__(self, path):
         if not (path / ".zmetadata").exists():
             raise ValueError("Not in VcfZarr format")  # NEEDS TEST
@@ -1667,58 +1695,60 @@
 
         self.wip_path.mkdir()
         self.arrays_path.mkdir()
         self.partitions_path.mkdir()
         store = zarr.DirectoryStore(self.arrays_path)
         root = zarr.group(store=store)
 
-        for column in self.schema.columns.values():
+        for column in self.schema.fields.values():
             self.init_array(root, column, partitions[-1].stop)
 
         logger.info("Writing WIP metadata")
         with open(self.wip_path / "metadata.json", "w") as f:
             json.dump(self.metadata.asdict(), f, indent=4)
         return len(partitions)
 
     def encode_samples(self, root):
-        if not np.array_equal(self.schema.sample_id, self.icf.metadata.samples):
+        if self.schema.samples != self.icf.metadata.samples:
             raise ValueError(
                 "Subsetting or reordering samples not supported currently"
             )  # NEEDS TEST
         array = root.array(
             "sample_id",
-            self.schema.sample_id,
+            [sample.id for sample in self.schema.samples],
             dtype="str",
             compressor=DEFAULT_ZARR_COMPRESSOR,
             chunks=(self.schema.samples_chunk_size,),
         )
         array.attrs["_ARRAY_DIMENSIONS"] = ["samples"]
         logger.debug("Samples done")
 
     def encode_contig_id(self, root):
         array = root.array(
             "contig_id",
-            self.schema.contig_id,
+            [contig.id for contig in self.schema.contigs],
             dtype="str",
             compressor=DEFAULT_ZARR_COMPRESSOR,
         )
         array.attrs["_ARRAY_DIMENSIONS"] = ["contigs"]
-        if self.schema.contig_length is not None:
+        if all(contig.length is not None for contig in self.schema.contigs):
             array = root.array(
                 "contig_length",
-                self.schema.contig_length,
+                [contig.length for contig in self.schema.contigs],
                 dtype=np.int64,
                 compressor=DEFAULT_ZARR_COMPRESSOR,
             )
             array.attrs["_ARRAY_DIMENSIONS"] = ["contigs"]
 
     def encode_filter_id(self, root):
+        # TODO need a way to store description also
+        # https://github.com/sgkit-dev/vcf-zarr-spec/issues/19
         array = root.array(
             "filter_id",
-            self.schema.filter_id,
+            [filt.id for filt in self.schema.filters],
             dtype="str",
             compressor=DEFAULT_ZARR_COMPRESSOR,
         )
         array.attrs["_ARRAY_DIMENSIONS"] = ["filters"]
 
     def init_array(self, root, variable, variants_dim_size):
         object_codec = None
@@ -1778,24 +1808,24 @@
         partition_path.mkdir(exist_ok=True)
         logger.info(f"Encoding partition {partition_index} to {partition_path}")
 
         self.encode_id_partition(partition_index)
         self.encode_filters_partition(partition_index)
         self.encode_contig_partition(partition_index)
         self.encode_alleles_partition(partition_index)
-        for col in self.schema.columns.values():
+        for col in self.schema.fields.values():
             if col.vcf_field is not None:
                 self.encode_array_partition(col, partition_index)
-        if "call_genotype" in self.schema.columns:
+        if "call_genotype" in self.schema.fields:
             self.encode_genotypes_partition(partition_index)
 
         final_path = self.partition_path(partition_index)
         logger.info(f"Finalising {partition_index} at {final_path}")
         if final_path.exists():
-            logger.warning("Removing existing partition at {final_path}")
+            logger.warning(f"Removing existing partition at {final_path}")
             shutil.rmtree(final_path)
         os.rename(partition_path, final_path)
 
     def init_partition_array(self, partition_index, name):
         wip_path = self.wip_partition_array_path(partition_index, name)
         # Create an empty array like the definition
         src = self.arrays_path / name
@@ -1809,15 +1839,15 @@
         logger.debug(f"Encoded {name} partition {partition_index}")
 
     def encode_array_partition(self, column, partition_index):
         array = self.init_partition_array(partition_index, column.name)
 
         partition = self.metadata.partitions[partition_index]
         ba = core.BufferedArray(array, partition.start)
-        source_col = self.icf.columns[column.vcf_field]
+        source_col = self.icf.fields[column.vcf_field]
         sanitiser = source_col.sanitiser_factory(ba.buff.shape)
 
         for value in source_col.iter_values(partition.start, partition.stop):
             # We write directly into the buffer in the sanitiser function
             # to make it easier to reason about dimension padding
             j = ba.next_buffer_row()
             sanitiser(ba.buff, j, value)
@@ -1832,15 +1862,15 @@
         )
 
         partition = self.metadata.partitions[partition_index]
         gt = core.BufferedArray(gt_array, partition.start)
         gt_mask = core.BufferedArray(gt_mask_array, partition.start)
         gt_phased = core.BufferedArray(gt_phased_array, partition.start)
 
-        source_col = self.icf.columns["FORMAT/GT"]
+        source_col = self.icf.fields["FORMAT/GT"]
         for value in source_col.iter_values(partition.start, partition.stop):
             j = gt.next_buffer_row()
             sanitise_value_int_2d(gt.buff, j, value[:, :-1])
             j = gt_phased.next_buffer_row()
             sanitise_value_int_1d(gt_phased.buff, j, value[:, -1])
             # TODO check is this the correct semantics when we are padding
             # with mixed ploidies?
@@ -1855,16 +1885,16 @@
         self.finalise_partition_array(partition_index, "call_genotype_phased")
 
     def encode_alleles_partition(self, partition_index):
         array_name = "variant_allele"
         alleles_array = self.init_partition_array(partition_index, array_name)
         partition = self.metadata.partitions[partition_index]
         alleles = core.BufferedArray(alleles_array, partition.start)
-        ref_col = self.icf.columns["REF"]
-        alt_col = self.icf.columns["ALT"]
+        ref_col = self.icf.fields["REF"]
+        alt_col = self.icf.fields["ALT"]
 
         for ref, alt in zip(
             ref_col.iter_values(partition.start, partition.stop),
             alt_col.iter_values(partition.start, partition.stop),
         ):
             j = alleles.next_buffer_row()
             alleles.buff[j, :] = STR_FILL
@@ -1876,15 +1906,15 @@
 
     def encode_id_partition(self, partition_index):
         vid_array = self.init_partition_array(partition_index, "variant_id")
         vid_mask_array = self.init_partition_array(partition_index, "variant_id_mask")
         partition = self.metadata.partitions[partition_index]
         vid = core.BufferedArray(vid_array, partition.start)
         vid_mask = core.BufferedArray(vid_mask_array, partition.start)
-        col = self.icf.columns["ID"]
+        col = self.icf.fields["ID"]
 
         for value in col.iter_values(partition.start, partition.stop):
             j = vid.next_buffer_row()
             k = vid_mask.next_buffer_row()
             assert j == k
             if value is not None:
                 vid.buff[j] = value[0]
@@ -1895,21 +1925,21 @@
         vid.flush()
         vid_mask.flush()
 
         self.finalise_partition_array(partition_index, "variant_id")
         self.finalise_partition_array(partition_index, "variant_id_mask")
 
     def encode_filters_partition(self, partition_index):
-        lookup = {filt: index for index, filt in enumerate(self.schema.filter_id)}
+        lookup = {filt.id: index for index, filt in enumerate(self.schema.filters)}
         array_name = "variant_filter"
         array = self.init_partition_array(partition_index, array_name)
         partition = self.metadata.partitions[partition_index]
         var_filter = core.BufferedArray(array, partition.start)
 
-        col = self.icf.columns["FILTERS"]
+        col = self.icf.fields["FILTERS"]
         for value in col.iter_values(partition.start, partition.stop):
             j = var_filter.next_buffer_row()
             var_filter.buff[j] = False
             for f in value:
                 try:
                     var_filter.buff[j, lookup[f]] = True
                 except KeyError:
@@ -1917,20 +1947,20 @@
                         f"Filter '{f}' was not defined in the header."
                     ) from None
         var_filter.flush()
 
         self.finalise_partition_array(partition_index, array_name)
 
     def encode_contig_partition(self, partition_index):
-        lookup = {contig: index for index, contig in enumerate(self.schema.contig_id)}
+        lookup = {contig.id: index for index, contig in enumerate(self.schema.contigs)}
         array_name = "variant_contig"
         array = self.init_partition_array(partition_index, array_name)
         partition = self.metadata.partitions[partition_index]
         contig = core.BufferedArray(array, partition.start)
-        col = self.icf.columns["CHROM"]
+        col = self.icf.fields["CHROM"]
 
         for value in col.iter_values(partition.start, partition.stop):
             j = contig.next_buffer_row()
             # Note: because we are using the indexes to define the lookups
             # and we always have an index, it seems that we the contig lookup
             # will always succeed. However, if anyone ever does hit a KeyError
             # here, please do open an issue with a reproducible example!
@@ -1982,29 +2012,29 @@
         for partition_id in range(self.num_partitions):
             if not self.partition_path(partition_id).exists():
                 missing.append(partition_id)
         if len(missing) > 0:
             raise FileNotFoundError(f"Partitions not encoded: {missing}")
 
         progress_config = core.ProgressConfig(
-            total=len(self.schema.columns),
+            total=len(self.schema.fields),
             title="Finalise",
             units="array",
             show=show_progress,
         )
         # NOTE: it's not clear that adding more workers will make this quicker,
         # as it's just going to be causing contention on the file system.
         # Something to check empirically in some deployments.
         # FIXME we're just using worker_processes=0 here to hook into the
         # SynchronousExecutor which is intended for testing purposes so
         # that we get test coverage. Should fix this either by allowing
         # for multiple workers, or making a standard wrapper for tqdm
         # that allows us to have a consistent look and feel.
         with core.ParallelWorkManager(0, progress_config) as pwm:
-            for name in self.schema.columns:
+            for name in self.schema.fields:
                 pwm.submit(self.finalise_array, name)
         logger.debug(f"Removing {self.wip_path}")
         shutil.rmtree(self.wip_path)
         logger.info("Consolidating Zarr metadata")
         zarr.consolidate_metadata(self.path)
 
     ######################
@@ -2012,26 +2042,25 @@
     ######################
 
     def get_max_encoding_memory(self):
         """
         Return the approximate maximum memory used to encode a variant chunk.
         """
         max_encoding_mem = max(
-            col.variant_chunk_nbytes for col in self.schema.columns.values()
+            col.variant_chunk_nbytes for col in self.schema.fields.values()
         )
         gt_mem = 0
-        if "call_genotype" in self.schema.columns:
+        if "call_genotype" in self.schema.fields:
             encoded_together = [
                 "call_genotype",
                 "call_genotype_phased",
                 "call_genotype_mask",
             ]
             gt_mem = sum(
-                self.schema.columns[col].variant_chunk_nbytes
-                for col in encoded_together
+                self.schema.fields[col].variant_chunk_nbytes for col in encoded_together
             )
         return max(max_encoding_mem, gt_mem)
 
     def encode_all_partitions(
         self, *, worker_processes=1, show_progress=False, max_memory=None
     ):
         max_memory = parse_max_memory(max_memory)
@@ -2055,15 +2084,15 @@
             raise ValueError(
                 f"Insufficient memory to encode a partition:"
                 f"{display_size(per_worker_memory)} > {display_size(max_memory)}"
             )
         num_workers = min(max_num_workers, worker_processes)
 
         total_bytes = 0
-        for col in self.schema.columns.values():
+        for col in self.schema.fields.values():
             # Open the array definition to get the total size
             total_bytes += zarr.open(self.arrays_path / col.name).nbytes
 
         progress_config = core.ProgressConfig(
             total=total_bytes,
             title="Encode",
             units="B",
```

### Comparing `bio2zarr-0.0.8/bio2zarr/vcf_utils.py` & `bio2zarr-0.0.9/bio2zarr/vcf_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,25 +72,29 @@
     """
     data = f.read(struct.calcsize(fmt))
     return struct.Struct(fmt).unpack(data)
 
 
 @dataclass
 class Region:
+    """
+    A htslib style region, where coordinates are 1-based and inclusive.
+    """
+
     contig: str
     start: Optional[int] = None
     end: Optional[int] = None
 
     def __post_init__(self):
         if self.start is not None:
             self.start = int(self.start)
             assert self.start > 0
         if self.end is not None:
             self.end = int(self.end)
-            assert self.end > self.start
+            assert self.end >= self.start
 
     def __str__(self):
         s = f"{self.contig}"
         if self.start is not None:
             s += f":{self.start}-"
         if self.end is not None:
             s += str(self.end)
@@ -109,14 +113,17 @@
 @dataclass
 class CSIBin:
     bin: int
     loffset: int
     chunks: Sequence[Chunk]
 
 
+RECORD_COUNT_UNKNOWN = np.inf
+
+
 @dataclass
 class CSIIndex:
     min_shift: int
     depth: int
     aux: str
     bins: Sequence[Sequence[CSIBin]]
     record_counts: Sequence[int]
@@ -217,15 +224,17 @@
         bins = []
         record_counts = []
 
         if n_ref > 0:
             for _ in range(n_ref):
                 n_bin = read_bytes_as_value(f, "<i")
                 seq_bins = []
-                record_count = -1
+                # Distinguish between counts that are zero because the sequence
+                # isn't there, vs counts that aren't in the index.
+                record_count = 0 if n_bin == 0 else RECORD_COUNT_UNKNOWN
                 for _ in range(n_bin):
                     bin, loffset, n_chunk = read_bytes_as_tuple(f, "<IQi")
                     chunks = []
                     for _ in range(n_chunk):
                         chunk = Chunk(*read_bytes_as_tuple(f, "<QQ"))
                         chunks.append(chunk)
                     seq_bins.append(CSIBin(bin, loffset, chunks))
@@ -333,15 +342,17 @@
             names = read_bytes_as_value(f, f"<{header.l_nm}s")
             # Convert \0-terminated names to strings
             sequence_names = [str(name, "utf-8") for name in names.split(b"\x00")[:-1]]
 
             for _ in range(header.n_ref):
                 n_bin = read_bytes_as_value(f, "<i")
                 seq_bins = []
-                record_count = -1
+                # Distinguish between counts that are zero because the sequence
+                # isn't there, vs counts that aren't in the index.
+                record_count = 0 if n_bin == 0 else RECORD_COUNT_UNKNOWN
                 for _ in range(n_bin):
                     bin, n_chunk = read_bytes_as_tuple(f, "<Ii")
                     chunks = []
                     for _ in range(n_chunk):
                         chunk = Chunk(*read_bytes_as_tuple(f, "<QQ"))
                         chunks.append(chunk)
                     seq_bins.append(TabixBin(bin, chunks))
@@ -432,27 +443,24 @@
     def variants(self, region):
         # Need to filter because of indels overlapping the region
         start = 1 if region.start is None else region.start
         for var in self.vcf(str(region)):
             if var.POS >= start:
                 yield var
 
-    def _filter_empty(self, regions):
+    def _filter_empty_and_refine(self, regions):
         """
-        Return all regions in the specified list that have one or more records.
-
-        Sometimes with Tabix indexes these seem to crop up:
-
-        - https://github.com/sgkit-dev/bio2zarr/issues/45
-        - https://github.com/sgkit-dev/bio2zarr/issues/120
+        Return all regions in the specified list that have one or more records,
+        and refine the start coordinate of the region to be the actual first coord
         """
         ret = []
         for region in regions:
-            variants = self.variants(region)
-            if next(variants, None) is not None:
+            var = next(self.variants(region), None)
+            if var is not None:
+                region.start = var.POS
                 ret.append(region)
         return ret
 
     def partition_into_regions(
         self,
         num_parts: Optional[int] = None,
         target_part_size: Union[None, int, str] = None,
@@ -524,8 +532,8 @@
                         regions.append(Region(next_contig, 1, end))
 
         # Add any sequences at the end that were not skipped
         for ri in range(region_contigs[-1] + 1, len(self.sequence_names)):
             if self.index.record_counts[ri] > 0:
                 regions.append(Region(self.sequence_names[ri]))
 
-        return self._filter_empty(regions)
+        return self._filter_empty_and_refine(regions)
```

### Comparing `bio2zarr-0.0.8/bio2zarr.egg-info/PKG-INFO` & `bio2zarr-0.0.9/bio2zarr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bio2zarr
-Version: 0.0.8
+Version: 0.0.9
 Summary: Convert bioinformatics data to Zarr
 Author-email: sgkit Developers <project@sgkit.dev>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -230,15 +230,15 @@
 Requires-Dist: bed_reader
 Provides-Extra: dev
 Requires-Dist: msprime; extra == "dev"
 Requires-Dist: pysam; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-coverage; extra == "dev"
 Requires-Dist: pytest-xdist; extra == "dev"
-Requires-Dist: sgkit; extra == "dev"
+Requires-Dist: sgkit>=0.8.0; extra == "dev"
 Requires-Dist: tqdm; extra == "dev"
 
 [![CI](https://github.com/sgkit-dev/bio2zarr/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/sgkit-dev/bio2zarr/actions/workflows/ci.yml)
 
 # bio2zarr
 Convert bioinformatics file formats to Zarr
```

### Comparing `bio2zarr-0.0.8/bio2zarr.egg-info/SOURCES.txt` & `bio2zarr-0.0.9/bio2zarr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bio2zarr-0.0.8/docs/_config.yml` & `bio2zarr-0.0.9/docs/_config.yml`

 * *Files identical despite different names*

### Comparing `bio2zarr-0.0.8/docs/intro.md` & `bio2zarr-0.0.9/docs/intro.md`

 * *Files identical despite different names*

### Comparing `bio2zarr-0.0.8/docs/logo.png` & `bio2zarr-0.0.9/docs/logo.png`

 * *Files identical despite different names*

### Comparing `bio2zarr-0.0.8/pyproject.toml` & `bio2zarr-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 [project.optional-dependencies]
 dev = [
   "msprime",
   "pysam",
   "pytest",
   "pytest-coverage",
   "pytest-xdist",
-  "sgkit",
+  "sgkit>=0.8.0",
   "tqdm"
 ]
 
 [tool.setuptools]
 packages = ["bio2zarr"]
 
 [tool.setuptools_scm]
```

### Comparing `bio2zarr-0.0.8/validation-data/Makefile` & `bio2zarr-0.0.9/validation-data/Makefile`

 * *Files 8% similar despite different names*

```diff
@@ -35,17 +35,22 @@
 # 1000 genomes phase 3
 1KG_P3_ALL_URL=http://ftp.1000genomes.ebi.ac.uk/vol1/ftp/data_collections/1000_genomes_project/release/20190312_biallelic_SNV_and_INDEL/ALL.chr1.shapeit2_integrated_snvindels_v2a_27022019.GRCh38.phased.vcf.gz
 1KG_P3_SNP_URL=http://ftp.1000genomes.ebi.ac.uk/vol1/ftp/data_collections/1000_genomes_project/release/20181203_biallelic_SNV/ALL.chr1.shapeit2_integrated_v1a.GRCh38.20181129.phased.vcf.gz
 
 # 1000 genomes phase 1
 1KG_P1_ALL_URL=http://ftp.1000genomes.ebi.ac.uk/vol1/ftp/phase1/analysis_results/integrated_call_sets/ALL.chr6.integrated_phase1_v3.20101123.snps_indels_svs.genotypes.vcf.gz
 
+old_tabix:
+	rm -fR tabix old_tabix
+	git clone https://github.com/samtools/tabix.git
+	cd tabix && make
+	cp tabix/tabix ./old_tabix
 
 %.vcf.gz.tbi: %.vcf.gz
-	tabix $<
+	./old_tabix $<
 
 %.2.split: %
 	./split.sh $< 2
 
 %.5.split: %
 	./split.sh $< 5
```

### Comparing `bio2zarr-0.0.8/validation.py` & `bio2zarr-0.0.9/validation.py`

 * *Files identical despite different names*

### Comparing `bio2zarr-0.0.8/vcf_generator.py` & `bio2zarr-0.0.9/vcf_generator.py`

 * *Files identical despite different names*

