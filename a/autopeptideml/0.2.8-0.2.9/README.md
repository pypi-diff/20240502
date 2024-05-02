# Comparing `tmp/autopeptideml-0.2.8.tar.gz` & `tmp/autopeptideml-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autopeptideml-0.2.8.tar", last modified: Wed Jan 31 21:50:40 2024, max compression
+gzip compressed data, was "autopeptideml-0.2.9.tar", last modified: Thu Feb  1 22:52:34 2024, max compression
```

## Comparing `autopeptideml-0.2.8.tar` & `autopeptideml-0.2.9.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:50:40.676864 autopeptideml-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-01-31 21:50:30.000000 autopeptideml-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13873 2024-01-31 21:50:40.676864 autopeptideml-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13116 2024-01-31 21:50:30.000000 autopeptideml-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:50:40.604864 autopeptideml-0.2.8/autopeptideml/
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-01-31 21:50:30.000000 autopeptideml-0.2.8/autopeptideml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27209 2024-01-31 21:50:30.000000 autopeptideml-0.2.8/autopeptideml/autopeptideml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:50:40.608864 autopeptideml-0.2.8/autopeptideml/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-31 21:50:30.000000 autopeptideml-0.2.8/autopeptideml/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-01-31 21:50:30.000000 autopeptideml-0.2.8/autopeptideml/data/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-01-31 21:50:30.000000 autopeptideml-0.2.8/autopeptideml/data/bioactivities.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-01-31 21:50:30.000000 autopeptideml-0.2.8/autopeptideml/data/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:50:40.672864 autopeptideml-0.2.8/autopeptideml/data/peptipedia/
--rw-r--r--   0 runner    (1001) docker     (127)  1129879 2024-01-31 21:50:30.000000 autopeptideml-0.2.8/autopeptideml/data/peptipedia/peptipedia_0-5.csv
--rw-r--r--   0 runner    (1001) docker     (127)  7497305 2024-01-31 21:50:30.000000 autopeptideml-0.2.8/autopeptideml/data/peptipedia/peptipedia_10-15.csv
--rw-r--r--   0 runner    (1001) docker     (127)   613591 2024-01-31 21:50:30.000000 autopeptideml-0.2.8/autopeptideml/data/peptipedia/peptipedia_100-105.csv
--rw-r--r--   0 runner    (1001) docker     (127)   511998 2024-01-31 21:50:30.000000 autopeptideml-0.2.8/autopeptideml/data/peptipedia/peptipedia_105-110.csv
--rw-r--r--   0 runner    (1001) docker     (127)   660788 2024-01-31 21:50:30.000000 autopeptideml-0.2.8/autopeptideml/data/peptipedia/peptipedia_110-115.csv
--rw-r--r--   0 runner    (1001) docker     (127)   794732 2024-01-31 21:50:30.000000 autopeptideml-0.2.8/autopeptideml/data/peptipedia/peptipedia_115-120.csv
--rw-r--r--   0 runner    (1001) docker     (127)   596551 2024-01-31 21:50:30.000000 autopeptideml-0.2.8/autopeptideml/data/peptipedia/peptipedia_120-125.csv
--rw-r--r--   0 runner    (1001) docker     (127)   579273 2024-01-31 21:50:30.000000 autopeptideml-0.2.8/autopeptideml/data/peptipedia/peptipedia_125-130.csv
--rw-r--r--   0 runner    (1001) docker     (127)   678292 2024-01-31 21:50:30.000000 autopeptideml-0.2.8/autopeptideml/data/peptipedia/peptipedia_130-135.csv
--rw-r--r--   0 runner    (1001) docker     (127)   603678 2024-01-31 21:50:30.000000 autopeptideml-0.2.8/autopeptideml/data/peptipedia/peptipedia_135-140.csv
--rw-r--r--   0 runner    (1001) docker     (127)   610465 2024-01-31 21:50:30.000000 autopeptideml-0.2.8/autopeptideml/data/peptipedia/peptipedia_140-145.csv
--rw-r--r--   0 runner    (1001) docker     (127)   650744 2024-01-31 21:50:30.000000 autopeptideml-0.2.8/autopeptideml/data/peptipedia/peptipedia_145-150.csv
--rw-r--r--   0 runner    (1001) docker     (127)  5740974 2024-01-31 21:50:30.000000 autopeptideml-0.2.8/autopeptideml/data/peptipedia/peptipedia_15-20.csv
--rw-r--r--   0 runner    (1001) docker     (127)  4460975 2024-01-31 21:50:30.000000 autopeptideml-0.2.8/autopeptideml/data/peptipedia/peptipedia_20-25.csv
--rw-r--r--   0 runner    (1001) docker     (127)  2555702 2024-01-31 21:50:30.000000 autopeptideml-0.2.8/autopeptideml/data/peptipedia/peptipedia_25-30.csv
--rw-r--r--   0 runner    (1001) docker     (127)  2094302 2024-01-31 21:50:30.000000 autopeptideml-0.2.8/autopeptideml/data/peptipedia/peptipedia_30-35.csv
--rw-r--r--   0 runner    (1001) docker     (127)  1743696 2024-01-31 21:50:30.000000 autopeptideml-0.2.8/autopeptideml/data/peptipedia/peptipedia_35-40.csv
--rw-r--r--   0 runner    (1001) docker     (127)  1150257 2024-01-31 21:50:30.000000 autopeptideml-0.2.8/autopeptideml/data/peptipedia/peptipedia_40-45.csv
--rw-r--r--   0 runner    (1001) docker     (127)  1229426 2024-01-31 21:50:30.000000 autopeptideml-0.2.8/autopeptideml/data/peptipedia/peptipedia_45-50.csv
--rw-r--r--   0 runner    (1001) docker     (127)  6615499 2024-01-31 21:50:30.000000 autopeptideml-0.2.8/autopeptideml/data/peptipedia/peptipedia_5-10.csv
--rw-r--r--   0 runner    (1001) docker     (127)   697008 2024-01-31 21:50:30.000000 autopeptideml-0.2.8/autopeptideml/data/peptipedia/peptipedia_50-55.csv
--rw-r--r--   0 runner    (1001) docker     (127)   810597 2024-01-31 21:50:30.000000 autopeptideml-0.2.8/autopeptideml/data/peptipedia/peptipedia_55-60.csv
--rw-r--r--   0 runner    (1001) docker     (127)  2027222 2024-01-31 21:50:30.000000 autopeptideml-0.2.8/autopeptideml/data/peptipedia/peptipedia_60-65.csv
--rw-r--r--   0 runner    (1001) docker     (127)  1048517 2024-01-31 21:50:30.000000 autopeptideml-0.2.8/autopeptideml/data/peptipedia/peptipedia_65-70.csv
--rw-r--r--   0 runner    (1001) docker     (127)  1142783 2024-01-31 21:50:30.000000 autopeptideml-0.2.8/autopeptideml/data/peptipedia/peptipedia_70-75.csv
--rw-r--r--   0 runner    (1001) docker     (127)  1008565 2024-01-31 21:50:30.000000 autopeptideml-0.2.8/autopeptideml/data/peptipedia/peptipedia_75-80.csv
--rw-r--r--   0 runner    (1001) docker     (127)   959154 2024-01-31 21:50:30.000000 autopeptideml-0.2.8/autopeptideml/data/peptipedia/peptipedia_80-85.csv
--rw-r--r--   0 runner    (1001) docker     (127)   860343 2024-01-31 21:50:30.000000 autopeptideml-0.2.8/autopeptideml/data/peptipedia/peptipedia_85-90.csv
--rw-r--r--   0 runner    (1001) docker     (127)   768941 2024-01-31 21:50:30.000000 autopeptideml-0.2.8/autopeptideml/data/peptipedia/peptipedia_90-95.csv
--rw-r--r--   0 runner    (1001) docker     (127)   655388 2024-01-31 21:50:30.000000 autopeptideml-0.2.8/autopeptideml/data/peptipedia/peptipedia_95-100.csv
--rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-01-31 21:50:30.000000 autopeptideml-0.2.8/autopeptideml/data/preprocess_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     9199 2024-01-31 21:50:30.000000 autopeptideml-0.2.8/autopeptideml/data/readme_ex.md
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-01-31 21:50:30.000000 autopeptideml-0.2.8/autopeptideml/data/residues.py
--rw-r--r--   0 runner    (1001) docker     (127)     5876 2024-01-31 21:50:30.000000 autopeptideml-0.2.8/autopeptideml/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:50:40.676864 autopeptideml-0.2.8/autopeptideml/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-31 21:50:30.000000 autopeptideml-0.2.8/autopeptideml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5906 2024-01-31 21:50:30.000000 autopeptideml-0.2.8/autopeptideml/utils/dataset_split.py
--rw-r--r--   0 runner    (1001) docker     (127)     4515 2024-01-31 21:50:30.000000 autopeptideml-0.2.8/autopeptideml/utils/embeddings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:50:40.676864 autopeptideml-0.2.8/autopeptideml/utils/partitioning/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-31 21:50:30.000000 autopeptideml-0.2.8/autopeptideml/utils/partitioning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5096 2024-01-31 21:50:30.000000 autopeptideml-0.2.8/autopeptideml/utils/partitioning/mmseqs_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12140 2024-01-31 21:50:30.000000 autopeptideml-0.2.8/autopeptideml/utils/partitioning/needle_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10925 2024-01-31 21:50:30.000000 autopeptideml-0.2.8/autopeptideml/utils/training.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:50:40.676864 autopeptideml-0.2.8/autopeptideml/utils/unidl4biopep/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-31 21:50:30.000000 autopeptideml-0.2.8/autopeptideml/utils/unidl4biopep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-01-31 21:50:30.000000 autopeptideml-0.2.8/autopeptideml/utils/unidl4biopep/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-01-31 21:50:30.000000 autopeptideml-0.2.8/autopeptideml/utils/unidl4biopep/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     8306 2024-01-31 21:50:30.000000 autopeptideml-0.2.8/autopeptideml/utils/unidl4biopep/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-31 21:50:40.676864 autopeptideml-0.2.8/autopeptideml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13873 2024-01-31 21:50:40.000000 autopeptideml-0.2.8/autopeptideml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-01-31 21:50:40.000000 autopeptideml-0.2.8/autopeptideml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 21:50:40.000000 autopeptideml-0.2.8/autopeptideml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-01-31 21:50:40.000000 autopeptideml-0.2.8/autopeptideml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-31 21:50:40.000000 autopeptideml-0.2.8/autopeptideml.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-01-31 21:50:40.000000 autopeptideml-0.2.8/autopeptideml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-01-31 21:50:40.000000 autopeptideml-0.2.8/autopeptideml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-31 21:50:40.676864 autopeptideml-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-01-31 21:50:30.000000 autopeptideml-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:52:34.642939 autopeptideml-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-02-01 22:52:26.000000 autopeptideml-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13873 2024-02-01 22:52:34.642939 autopeptideml-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13116 2024-02-01 22:52:26.000000 autopeptideml-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:52:34.574939 autopeptideml-0.2.9/autopeptideml/
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-02-01 22:52:26.000000 autopeptideml-0.2.9/autopeptideml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27209 2024-02-01 22:52:26.000000 autopeptideml-0.2.9/autopeptideml/autopeptideml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:52:34.574939 autopeptideml-0.2.9/autopeptideml/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 22:52:26.000000 autopeptideml-0.2.9/autopeptideml/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-02-01 22:52:26.000000 autopeptideml-0.2.9/autopeptideml/data/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-02-01 22:52:26.000000 autopeptideml-0.2.9/autopeptideml/data/bioactivities.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-02-01 22:52:26.000000 autopeptideml-0.2.9/autopeptideml/data/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:52:34.638939 autopeptideml-0.2.9/autopeptideml/data/peptipedia/
+-rw-r--r--   0 runner    (1001) docker     (127)  1129879 2024-02-01 22:52:26.000000 autopeptideml-0.2.9/autopeptideml/data/peptipedia/peptipedia_0-5.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  7497305 2024-02-01 22:52:26.000000 autopeptideml-0.2.9/autopeptideml/data/peptipedia/peptipedia_10-15.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   613591 2024-02-01 22:52:26.000000 autopeptideml-0.2.9/autopeptideml/data/peptipedia/peptipedia_100-105.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   511998 2024-02-01 22:52:26.000000 autopeptideml-0.2.9/autopeptideml/data/peptipedia/peptipedia_105-110.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   660788 2024-02-01 22:52:26.000000 autopeptideml-0.2.9/autopeptideml/data/peptipedia/peptipedia_110-115.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   794732 2024-02-01 22:52:26.000000 autopeptideml-0.2.9/autopeptideml/data/peptipedia/peptipedia_115-120.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   596551 2024-02-01 22:52:26.000000 autopeptideml-0.2.9/autopeptideml/data/peptipedia/peptipedia_120-125.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   579273 2024-02-01 22:52:26.000000 autopeptideml-0.2.9/autopeptideml/data/peptipedia/peptipedia_125-130.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   678292 2024-02-01 22:52:26.000000 autopeptideml-0.2.9/autopeptideml/data/peptipedia/peptipedia_130-135.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   603678 2024-02-01 22:52:26.000000 autopeptideml-0.2.9/autopeptideml/data/peptipedia/peptipedia_135-140.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   610465 2024-02-01 22:52:26.000000 autopeptideml-0.2.9/autopeptideml/data/peptipedia/peptipedia_140-145.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   650744 2024-02-01 22:52:26.000000 autopeptideml-0.2.9/autopeptideml/data/peptipedia/peptipedia_145-150.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  5740974 2024-02-01 22:52:26.000000 autopeptideml-0.2.9/autopeptideml/data/peptipedia/peptipedia_15-20.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  4460975 2024-02-01 22:52:26.000000 autopeptideml-0.2.9/autopeptideml/data/peptipedia/peptipedia_20-25.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  2555702 2024-02-01 22:52:26.000000 autopeptideml-0.2.9/autopeptideml/data/peptipedia/peptipedia_25-30.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  2094302 2024-02-01 22:52:26.000000 autopeptideml-0.2.9/autopeptideml/data/peptipedia/peptipedia_30-35.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1743696 2024-02-01 22:52:26.000000 autopeptideml-0.2.9/autopeptideml/data/peptipedia/peptipedia_35-40.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1150257 2024-02-01 22:52:26.000000 autopeptideml-0.2.9/autopeptideml/data/peptipedia/peptipedia_40-45.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1229426 2024-02-01 22:52:26.000000 autopeptideml-0.2.9/autopeptideml/data/peptipedia/peptipedia_45-50.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  6615499 2024-02-01 22:52:26.000000 autopeptideml-0.2.9/autopeptideml/data/peptipedia/peptipedia_5-10.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   697008 2024-02-01 22:52:26.000000 autopeptideml-0.2.9/autopeptideml/data/peptipedia/peptipedia_50-55.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   810597 2024-02-01 22:52:26.000000 autopeptideml-0.2.9/autopeptideml/data/peptipedia/peptipedia_55-60.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  2027222 2024-02-01 22:52:26.000000 autopeptideml-0.2.9/autopeptideml/data/peptipedia/peptipedia_60-65.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1048517 2024-02-01 22:52:26.000000 autopeptideml-0.2.9/autopeptideml/data/peptipedia/peptipedia_65-70.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1142783 2024-02-01 22:52:26.000000 autopeptideml-0.2.9/autopeptideml/data/peptipedia/peptipedia_70-75.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1008565 2024-02-01 22:52:26.000000 autopeptideml-0.2.9/autopeptideml/data/peptipedia/peptipedia_75-80.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   959154 2024-02-01 22:52:26.000000 autopeptideml-0.2.9/autopeptideml/data/peptipedia/peptipedia_80-85.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   860343 2024-02-01 22:52:26.000000 autopeptideml-0.2.9/autopeptideml/data/peptipedia/peptipedia_85-90.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   768941 2024-02-01 22:52:26.000000 autopeptideml-0.2.9/autopeptideml/data/peptipedia/peptipedia_90-95.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   655388 2024-02-01 22:52:26.000000 autopeptideml-0.2.9/autopeptideml/data/peptipedia/peptipedia_95-100.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-02-01 22:52:26.000000 autopeptideml-0.2.9/autopeptideml/data/preprocess_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9199 2024-02-01 22:52:26.000000 autopeptideml-0.2.9/autopeptideml/data/readme_ex.md
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-02-01 22:52:26.000000 autopeptideml-0.2.9/autopeptideml/data/residues.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5876 2024-02-01 22:52:26.000000 autopeptideml-0.2.9/autopeptideml/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:52:34.642939 autopeptideml-0.2.9/autopeptideml/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 22:52:26.000000 autopeptideml-0.2.9/autopeptideml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5906 2024-02-01 22:52:26.000000 autopeptideml-0.2.9/autopeptideml/utils/dataset_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4515 2024-02-01 22:52:26.000000 autopeptideml-0.2.9/autopeptideml/utils/embeddings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:52:34.642939 autopeptideml-0.2.9/autopeptideml/utils/partitioning/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 22:52:26.000000 autopeptideml-0.2.9/autopeptideml/utils/partitioning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5096 2024-02-01 22:52:26.000000 autopeptideml-0.2.9/autopeptideml/utils/partitioning/mmseqs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12140 2024-02-01 22:52:26.000000 autopeptideml-0.2.9/autopeptideml/utils/partitioning/needle_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10925 2024-02-01 22:52:26.000000 autopeptideml-0.2.9/autopeptideml/utils/training.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:52:34.642939 autopeptideml-0.2.9/autopeptideml/utils/unidl4biopep/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 22:52:26.000000 autopeptideml-0.2.9/autopeptideml/utils/unidl4biopep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-02-01 22:52:26.000000 autopeptideml-0.2.9/autopeptideml/utils/unidl4biopep/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-02-01 22:52:26.000000 autopeptideml-0.2.9/autopeptideml/utils/unidl4biopep/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8306 2024-02-01 22:52:26.000000 autopeptideml-0.2.9/autopeptideml/utils/unidl4biopep/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 22:52:34.642939 autopeptideml-0.2.9/autopeptideml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13873 2024-02-01 22:52:34.000000 autopeptideml-0.2.9/autopeptideml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-02-01 22:52:34.000000 autopeptideml-0.2.9/autopeptideml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-01 22:52:34.000000 autopeptideml-0.2.9/autopeptideml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-02-01 22:52:34.000000 autopeptideml-0.2.9/autopeptideml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-01 22:52:34.000000 autopeptideml-0.2.9/autopeptideml.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-02-01 22:52:34.000000 autopeptideml-0.2.9/autopeptideml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-01 22:52:34.000000 autopeptideml-0.2.9/autopeptideml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-01 22:52:34.642939 autopeptideml-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-02-01 22:52:26.000000 autopeptideml-0.2.9/setup.py
```

### Comparing `autopeptideml-0.2.8/LICENSE` & `autopeptideml-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `autopeptideml-0.2.8/PKG-INFO` & `autopeptideml-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autopeptideml
-Version: 0.2.8
+Version: 0.2.9
 Summary: AutoML system for building trustworthy peptide bioactivity predictors
 Home-page: https://github.ibm.com/raulfd/autopeptideml
 Author: Raul Fernandez-Diaz
 Author-email: raulfd@ibm.com
 License: MIT
 Keywords: autopeptideml
 Requires-Python: >=3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: autopeptideml Version: 0.2.8 Summary: AutoML system
+Metadata-Version: 2.1 Name: autopeptideml Version: 0.2.9 Summary: AutoML system
 for building trustworthy peptide bioactivity predictors Home-page: https://
 github.ibm.com/raulfd/autopeptideml Author: Raul Fernandez-Diaz Author-email:
 raulfd@ibm.com License: MIT Keywords: autopeptideml Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 charset-normalizer Requires-Dist: gdown Requires-Dist: graph-part Requires-
 Dist: networkx Requires-Dist: optuna Requires-Dist: pandarallel Requires-Dist:
 scipy<=1.11.4 Requires-Dist: scikit-learn Requires-Dist: scikit-plot Requires-
```

### Comparing `autopeptideml-0.2.8/README.md` & `autopeptideml-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `autopeptideml-0.2.8/autopeptideml/autopeptideml.py` & `autopeptideml-0.2.9/autopeptideml/autopeptideml.py`

 * *Files identical despite different names*

### Comparing `autopeptideml-0.2.8/autopeptideml/data/algorithms.py` & `autopeptideml-0.2.9/autopeptideml/data/algorithms.py`

 * *Files identical despite different names*

### Comparing `autopeptideml-0.2.8/autopeptideml/data/bioactivities.txt` & `autopeptideml-0.2.9/autopeptideml/data/bioactivities.txt`

 * *Files identical despite different names*

### Comparing `autopeptideml-0.2.8/autopeptideml/data/metrics.py` & `autopeptideml-0.2.9/autopeptideml/data/metrics.py`

 * *Files identical despite different names*

### Comparing `autopeptideml-0.2.8/autopeptideml/data/peptipedia/peptipedia_0-5.csv` & `autopeptideml-0.2.9/autopeptideml/data/peptipedia/peptipedia_0-5.csv`

 * *Files identical despite different names*

### Comparing `autopeptideml-0.2.8/autopeptideml/data/peptipedia/peptipedia_10-15.csv` & `autopeptideml-0.2.9/autopeptideml/data/peptipedia/peptipedia_10-15.csv`

 * *Files identical despite different names*

### Comparing `autopeptideml-0.2.8/autopeptideml/data/peptipedia/peptipedia_100-105.csv` & `autopeptideml-0.2.9/autopeptideml/data/peptipedia/peptipedia_100-105.csv`

 * *Files identical despite different names*

### Comparing `autopeptideml-0.2.8/autopeptideml/data/peptipedia/peptipedia_105-110.csv` & `autopeptideml-0.2.9/autopeptideml/data/peptipedia/peptipedia_105-110.csv`

 * *Files identical despite different names*

### Comparing `autopeptideml-0.2.8/autopeptideml/data/peptipedia/peptipedia_110-115.csv` & `autopeptideml-0.2.9/autopeptideml/data/peptipedia/peptipedia_110-115.csv`

 * *Files identical despite different names*

### Comparing `autopeptideml-0.2.8/autopeptideml/data/peptipedia/peptipedia_115-120.csv` & `autopeptideml-0.2.9/autopeptideml/data/peptipedia/peptipedia_115-120.csv`

 * *Files identical despite different names*

### Comparing `autopeptideml-0.2.8/autopeptideml/data/peptipedia/peptipedia_120-125.csv` & `autopeptideml-0.2.9/autopeptideml/data/peptipedia/peptipedia_120-125.csv`

 * *Files identical despite different names*

### Comparing `autopeptideml-0.2.8/autopeptideml/data/peptipedia/peptipedia_125-130.csv` & `autopeptideml-0.2.9/autopeptideml/data/peptipedia/peptipedia_125-130.csv`

 * *Files identical despite different names*

### Comparing `autopeptideml-0.2.8/autopeptideml/data/peptipedia/peptipedia_130-135.csv` & `autopeptideml-0.2.9/autopeptideml/data/peptipedia/peptipedia_130-135.csv`

 * *Files identical despite different names*

### Comparing `autopeptideml-0.2.8/autopeptideml/data/peptipedia/peptipedia_135-140.csv` & `autopeptideml-0.2.9/autopeptideml/data/peptipedia/peptipedia_135-140.csv`

 * *Files identical despite different names*

### Comparing `autopeptideml-0.2.8/autopeptideml/data/peptipedia/peptipedia_140-145.csv` & `autopeptideml-0.2.9/autopeptideml/data/peptipedia/peptipedia_140-145.csv`

 * *Files identical despite different names*

### Comparing `autopeptideml-0.2.8/autopeptideml/data/peptipedia/peptipedia_145-150.csv` & `autopeptideml-0.2.9/autopeptideml/data/peptipedia/peptipedia_145-150.csv`

 * *Files identical despite different names*

### Comparing `autopeptideml-0.2.8/autopeptideml/data/peptipedia/peptipedia_15-20.csv` & `autopeptideml-0.2.9/autopeptideml/data/peptipedia/peptipedia_15-20.csv`

 * *Files identical despite different names*

### Comparing `autopeptideml-0.2.8/autopeptideml/data/peptipedia/peptipedia_20-25.csv` & `autopeptideml-0.2.9/autopeptideml/data/peptipedia/peptipedia_20-25.csv`

 * *Files identical despite different names*

### Comparing `autopeptideml-0.2.8/autopeptideml/data/peptipedia/peptipedia_25-30.csv` & `autopeptideml-0.2.9/autopeptideml/data/peptipedia/peptipedia_25-30.csv`

 * *Files identical despite different names*

### Comparing `autopeptideml-0.2.8/autopeptideml/data/peptipedia/peptipedia_30-35.csv` & `autopeptideml-0.2.9/autopeptideml/data/peptipedia/peptipedia_30-35.csv`

 * *Files identical despite different names*

### Comparing `autopeptideml-0.2.8/autopeptideml/data/peptipedia/peptipedia_35-40.csv` & `autopeptideml-0.2.9/autopeptideml/data/peptipedia/peptipedia_35-40.csv`

 * *Files identical despite different names*

### Comparing `autopeptideml-0.2.8/autopeptideml/data/peptipedia/peptipedia_40-45.csv` & `autopeptideml-0.2.9/autopeptideml/data/peptipedia/peptipedia_40-45.csv`

 * *Files identical despite different names*

### Comparing `autopeptideml-0.2.8/autopeptideml/data/peptipedia/peptipedia_45-50.csv` & `autopeptideml-0.2.9/autopeptideml/data/peptipedia/peptipedia_45-50.csv`

 * *Files identical despite different names*

### Comparing `autopeptideml-0.2.8/autopeptideml/data/peptipedia/peptipedia_5-10.csv` & `autopeptideml-0.2.9/autopeptideml/data/peptipedia/peptipedia_5-10.csv`

 * *Files identical despite different names*

### Comparing `autopeptideml-0.2.8/autopeptideml/data/peptipedia/peptipedia_50-55.csv` & `autopeptideml-0.2.9/autopeptideml/data/peptipedia/peptipedia_50-55.csv`

 * *Files identical despite different names*

### Comparing `autopeptideml-0.2.8/autopeptideml/data/peptipedia/peptipedia_55-60.csv` & `autopeptideml-0.2.9/autopeptideml/data/peptipedia/peptipedia_55-60.csv`

 * *Files identical despite different names*

### Comparing `autopeptideml-0.2.8/autopeptideml/data/peptipedia/peptipedia_60-65.csv` & `autopeptideml-0.2.9/autopeptideml/data/peptipedia/peptipedia_60-65.csv`

 * *Files identical despite different names*

### Comparing `autopeptideml-0.2.8/autopeptideml/data/peptipedia/peptipedia_65-70.csv` & `autopeptideml-0.2.9/autopeptideml/data/peptipedia/peptipedia_65-70.csv`

 * *Files identical despite different names*

### Comparing `autopeptideml-0.2.8/autopeptideml/data/peptipedia/peptipedia_70-75.csv` & `autopeptideml-0.2.9/autopeptideml/data/peptipedia/peptipedia_70-75.csv`

 * *Files identical despite different names*

### Comparing `autopeptideml-0.2.8/autopeptideml/data/peptipedia/peptipedia_75-80.csv` & `autopeptideml-0.2.9/autopeptideml/data/peptipedia/peptipedia_75-80.csv`

 * *Files identical despite different names*

### Comparing `autopeptideml-0.2.8/autopeptideml/data/peptipedia/peptipedia_80-85.csv` & `autopeptideml-0.2.9/autopeptideml/data/peptipedia/peptipedia_80-85.csv`

 * *Files identical despite different names*

### Comparing `autopeptideml-0.2.8/autopeptideml/data/peptipedia/peptipedia_85-90.csv` & `autopeptideml-0.2.9/autopeptideml/data/peptipedia/peptipedia_85-90.csv`

 * *Files identical despite different names*

### Comparing `autopeptideml-0.2.8/autopeptideml/data/peptipedia/peptipedia_90-95.csv` & `autopeptideml-0.2.9/autopeptideml/data/peptipedia/peptipedia_90-95.csv`

 * *Files identical despite different names*

### Comparing `autopeptideml-0.2.8/autopeptideml/data/peptipedia/peptipedia_95-100.csv` & `autopeptideml-0.2.9/autopeptideml/data/peptipedia/peptipedia_95-100.csv`

 * *Files identical despite different names*

### Comparing `autopeptideml-0.2.8/autopeptideml/data/preprocess_db.py` & `autopeptideml-0.2.9/autopeptideml/data/preprocess_db.py`

 * *Files identical despite different names*

### Comparing `autopeptideml-0.2.8/autopeptideml/data/readme_ex.md` & `autopeptideml-0.2.9/autopeptideml/data/readme_ex.md`

 * *Files identical despite different names*

### Comparing `autopeptideml-0.2.8/autopeptideml/main.py` & `autopeptideml-0.2.9/autopeptideml/main.py`

 * *Files identical despite different names*

### Comparing `autopeptideml-0.2.8/autopeptideml/utils/dataset_split.py` & `autopeptideml-0.2.9/autopeptideml/utils/dataset_split.py`

 * *Files identical despite different names*

### Comparing `autopeptideml-0.2.8/autopeptideml/utils/embeddings.py` & `autopeptideml-0.2.9/autopeptideml/utils/embeddings.py`

 * *Files identical despite different names*

### Comparing `autopeptideml-0.2.8/autopeptideml/utils/partitioning/mmseqs_utils.py` & `autopeptideml-0.2.9/autopeptideml/utils/partitioning/mmseqs_utils.py`

 * *Files identical despite different names*

### Comparing `autopeptideml-0.2.8/autopeptideml/utils/partitioning/needle_utils.py` & `autopeptideml-0.2.9/autopeptideml/utils/partitioning/needle_utils.py`

 * *Files identical despite different names*

### Comparing `autopeptideml-0.2.8/autopeptideml/utils/training.py` & `autopeptideml-0.2.9/autopeptideml/utils/training.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 
 from ..data.metrics import METRIC2FUNCTION, METRICS
 from ..data.algorithms import SUPPORTED_MODELS, SYNONYMS
 
 
 NO_N_JOBS = []
 NO_N_JOBS.extend(SYNONYMS['svm'])
-NO_N_JOBS.extend(SYNPNYMS['mlp'])
-NO_N_JOBS.extend(SYNPNYMS['xgboost'])
+NO_N_JOBS.extend(SYNONYMS['mlp'])
+NO_N_JOBS.extend(SYNONYMS['xgboost'])
 
 
 class FlexibleObjective:
     def __init__(
         self,
         config,
         train_df: pd.DataFrame,
```

### Comparing `autopeptideml-0.2.8/autopeptideml/utils/unidl4biopep/dataset.py` & `autopeptideml-0.2.9/autopeptideml/utils/unidl4biopep/dataset.py`

 * *Files identical despite different names*

### Comparing `autopeptideml-0.2.8/autopeptideml/utils/unidl4biopep/loss.py` & `autopeptideml-0.2.9/autopeptideml/utils/unidl4biopep/loss.py`

 * *Files identical despite different names*

### Comparing `autopeptideml-0.2.8/autopeptideml/utils/unidl4biopep/model.py` & `autopeptideml-0.2.9/autopeptideml/utils/unidl4biopep/model.py`

 * *Files identical despite different names*

### Comparing `autopeptideml-0.2.8/autopeptideml.egg-info/PKG-INFO` & `autopeptideml-0.2.9/autopeptideml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autopeptideml
-Version: 0.2.8
+Version: 0.2.9
 Summary: AutoML system for building trustworthy peptide bioactivity predictors
 Home-page: https://github.ibm.com/raulfd/autopeptideml
 Author: Raul Fernandez-Diaz
 Author-email: raulfd@ibm.com
 License: MIT
 Keywords: autopeptideml
 Requires-Python: >=3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: autopeptideml Version: 0.2.8 Summary: AutoML system
+Metadata-Version: 2.1 Name: autopeptideml Version: 0.2.9 Summary: AutoML system
 for building trustworthy peptide bioactivity predictors Home-page: https://
 github.ibm.com/raulfd/autopeptideml Author: Raul Fernandez-Diaz Author-email:
 raulfd@ibm.com License: MIT Keywords: autopeptideml Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 charset-normalizer Requires-Dist: gdown Requires-Dist: graph-part Requires-
 Dist: networkx Requires-Dist: optuna Requires-Dist: pandarallel Requires-Dist:
 scipy<=1.11.4 Requires-Dist: scikit-learn Requires-Dist: scikit-plot Requires-
```

### Comparing `autopeptideml-0.2.8/autopeptideml.egg-info/SOURCES.txt` & `autopeptideml-0.2.9/autopeptideml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autopeptideml-0.2.8/setup.py` & `autopeptideml-0.2.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,10 +52,10 @@
     long_description_content_type='text/markdown',
     data_files=[('', files)],
     include_package_data=True,
     keywords='autopeptideml',
     name='autopeptideml',
     packages=find_packages(exclude=['examples']),
     url='https://github.ibm.com/raulfd/autopeptideml',
-    version='0.2.8',
+    version='0.2.9',
     zip_safe=False,
 )
```

