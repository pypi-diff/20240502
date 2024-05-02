# Comparing `tmp/probe_design-0.2.8.tar.gz` & `tmp/probe_design-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "probe_design-0.2.8.tar", max compression
+gzip compressed data, was "probe_design-0.2.9.tar", max compression
```

## Comparing `probe_design-0.2.8.tar` & `probe_design-0.2.9.tar`

### file list

```diff
@@ -1,64 +1,65 @@
--rw-r--r--   0        0        0     1027 2023-12-27 11:04:31.964287 probe_design-0.2.8/LICENSE
--rw-r--r--   0        0        0    10758 2024-03-04 17:08:35.580527 probe_design-0.2.8/README.md
--rw-r--r--   0        0        0     1439 2024-01-29 09:13:22.868827 probe_design-0.2.8/probe_design/__init__.py
--rw-r--r--   0        0        0       82 2023-12-27 11:04:31.994619 probe_design-0.2.8/probe_design/data/exclude/excl_roi_1.bed
--rw-r--r--   0        0        0       97 2023-12-27 11:04:31.995005 probe_design-0.2.8/probe_design/data/exclude/excl_roi_10.bed
--rw-r--r--   0        0        0       96 2023-12-27 11:04:31.995340 probe_design-0.2.8/probe_design/data/exclude/excl_roi_11.bed
--rw-r--r--   0        0        0       99 2023-12-27 11:04:31.995677 probe_design-0.2.8/probe_design/data/exclude/excl_roi_12.bed
--rw-r--r--   0        0        0       96 2023-12-27 11:04:31.996162 probe_design-0.2.8/probe_design/data/exclude/excl_roi_2.bed
--rw-r--r--   0        0        0       98 2023-12-27 11:04:31.996466 probe_design-0.2.8/probe_design/data/exclude/excl_roi_3.bed
--rw-r--r--   0        0        0       96 2023-12-27 11:04:31.996749 probe_design-0.2.8/probe_design/data/exclude/excl_roi_4.bed
--rw-r--r--   0        0        0       96 2023-12-27 11:04:31.997073 probe_design-0.2.8/probe_design/data/exclude/excl_roi_5.bed
--rw-r--r--   0        0        0       98 2023-12-27 11:04:31.997375 probe_design-0.2.8/probe_design/data/exclude/excl_roi_6.bed
--rw-r--r--   0        0        0       97 2023-12-27 11:04:31.997734 probe_design-0.2.8/probe_design/data/exclude/excl_roi_7.bed
--rw-r--r--   0        0        0       97 2023-12-27 11:04:31.998055 probe_design-0.2.8/probe_design/data/exclude/excl_roi_8.bed
--rw-r--r--   0        0        0       96 2023-12-27 11:04:31.998471 probe_design-0.2.8/probe_design/data/exclude/excl_roi_9.bed
--rw-r--r--   0        0        0    21733 2023-12-27 11:04:31.999411 probe_design-0.2.8/probe_design/data/rois/DNA_FISH_template.ods
--rw-r--r--   0        0        0    17661 2023-12-27 11:04:32.000083 probe_design-0.2.8/probe_design/data/rois/DNA_RNA_FISH_template.ods
--rw-r--r--   0        0        0    30029 2023-12-27 11:04:32.000635 probe_design-0.2.8/probe_design/data/rois/RNA_FISH_template.ods
--rw-r--r--   0        0        0      515 2023-12-27 11:04:32.001141 probe_design-0.2.8/probe_design/data/rois/all_regions.tsv
--rw-r--r--   0        0        0       62 2023-12-27 11:04:32.001655 probe_design-0.2.8/probe_design/data/rois/df_DNA_FISH.txt
--rw-r--r--   0        0        0      154 2023-12-27 11:04:32.002115 probe_design-0.2.8/probe_design/data/rois/df_DNA_RNA_FISH.txt
--rw-r--r--   0        0        0      247 2023-12-27 11:04:32.002541 probe_design-0.2.8/probe_design/data/rois/df_RNA_FISH.txt
--rw-r--r--   0        0        0     2949 2024-02-22 11:09:10.840678 probe_design-0.2.8/probe_design/main.py
--rw-r--r--   0        0        0     5076 2023-12-27 11:04:32.036740 probe_design-0.2.8/probe_design/notebooks/plot_oligos.ipynb
--rw-r--r--   0        0        0    15318 2023-12-27 11:04:32.037331 probe_design-0.2.8/probe_design/notebooks/plot_probe_candidates.ipynb
--rw-r--r--   0        0        0     5086 2023-12-27 11:04:32.037940 probe_design-0.2.8/probe_design/notebooks/plot_probes.ipynb
--rw-r--r--   0        0        0     1619 2023-12-27 11:04:32.038806 probe_design-0.2.8/probe_design/shell/apply_blacklist.sh
--rw-r--r--   0        0        0     1807 2024-02-22 12:31:56.143592 probe_design-0.2.8/probe_design/shell/build-db.sh
--rw-r--r--   0        0        0     3520 2024-02-22 12:31:16.514067 probe_design-0.2.8/probe_design/shell/build-db_BL.sh
--rw-r--r--   0        0        0     1451 2024-02-22 12:31:43.215584 probe_design-0.2.8/probe_design/shell/build-db_cc.sh
--rw-r--r--   0        0        0     1201 2023-12-27 11:04:32.040735 probe_design-0.2.8/probe_design/shell/generate_blacklist.sh
--rw-r--r--   0        0        0      857 2023-12-27 11:04:32.041184 probe_design-0.2.8/probe_design/shell/get_ref_genome.sh
--rw-r--r--   0        0        0       97 2024-02-22 11:09:10.841735 probe_design-0.2.8/probe_design/shell/makedirs.sh
--rw-r--r--   0        0        0      720 2024-02-22 11:09:10.842306 probe_design-0.2.8/probe_design/shell/melt_secs_parallel.sh
--rw-r--r--   0        0        0     2362 2023-12-27 11:04:32.042486 probe_design-0.2.8/probe_design/shell/pipeline.sh
--rw-r--r--   0        0        0     2745 2023-12-27 11:04:32.042976 probe_design-0.2.8/probe_design/shell/pipeline_exclude.sh
--rw-r--r--   0        0        0     2826 2023-12-27 11:04:32.043433 probe_design-0.2.8/probe_design/shell/probe-query.sh
--rw-r--r--   0        0        0     4422 2024-02-05 10:18:01.859852 probe_design-0.2.8/probe_design/shell/run_nHUSH.sh
--rw-r--r--   0        0        0     5171 2024-02-05 10:17:03.523669 probe_design-0.2.8/probe_design/shell/run_nHUSH_excl.sh
--rw-r--r--   0        0        0      338 2023-12-29 15:06:22.909485 probe_design-0.2.8/probe_design/shell/show.sh
--rw-r--r--   0        0        0       22 2024-01-29 14:30:38.732109 probe_design-0.2.8/probe_design/shell/test_shell.sh
--rw-r--r--   0        0        0      735 2023-12-27 11:04:32.045065 probe_design-0.2.8/probe_design/shell/unfinished_HUSH.sh
--rw-r--r--   0        0        0     3552 2024-02-05 10:16:36.206369 probe_design-0.2.8/probe_design/shell/validation_oldHUSH_BLAST.sh
--rw-r--r--   0        0        0     3560 2024-01-08 11:24:09.444010 probe_design-0.2.8/probe_design/src/HUSH_feedback.py
--rw-r--r--   0        0        0     1827 2024-03-04 17:37:19.708500 probe_design-0.2.8/probe_design/src/__init__.py
--rw-r--r--   0        0        0    23845 2024-02-22 11:09:10.842932 probe_design-0.2.8/probe_design/src/cycling_query.py
--rw-r--r--   0        0        0     8046 2024-01-11 14:36:50.223140 probe_design-0.2.8/probe_design/src/download_chromosomes.py
--rw-r--r--   0        0        0     9275 2024-03-04 17:08:35.582944 probe_design-0.2.8/probe_design/src/escafish_score.py
--rw-r--r--   0        0        0     3163 2024-03-04 17:08:35.583496 probe_design-0.2.8/probe_design/src/exclude_region.py
--rw-r--r--   0        0        0     1446 2024-01-02 10:41:11.267835 probe_design-0.2.8/probe_design/src/generate_exclude.py
--rw-r--r--   0        0        0     4314 2024-03-04 17:08:35.584658 probe_design-0.2.8/probe_design/src/get_oligos.py
--rw-r--r--   0        0        0     3331 2023-12-27 11:04:32.050271 probe_design-0.2.8/probe_design/src/prepare_input.r
--rw-r--r--   0        0        0     4177 2024-01-08 11:39:19.105676 probe_design-0.2.8/probe_design/src/reform_hush.py
--rw-r--r--   0        0        0     5134 2024-03-04 17:37:42.432020 probe_design-0.2.8/probe_design/src/reform_hush_combined.py
--rw-r--r--   0        0        0     5598 2024-01-08 11:29:55.409099 probe_design-0.2.8/probe_design/src/reform_hush_combined_new.py
--rw-r--r--   0        0        0     6620 2024-01-08 11:42:47.175118 probe_design-0.2.8/probe_design/src/reform_hush_consec.py
--rw-r--r--   0        0        0     5167 2024-01-02 11:59:24.604027 probe_design-0.2.8/probe_design/src/select_probe.py
--rw-r--r--   0        0        0      785 2024-03-04 17:08:35.585612 probe_design-0.2.8/probe_design/src/split_fasta.py
--rw-r--r--   0        0        0     3546 2024-01-02 12:38:28.314063 probe_design-0.2.8/probe_design/src/summarize_probes.py
--rw-r--r--   0        0        0     4050 2024-01-02 12:38:28.313904 probe_design-0.2.8/probe_design/src/summarize_probes_cumul.py
--rw-r--r--   0        0        0     4081 2023-12-27 11:04:32.054742 probe_design-0.2.8/probe_design/src/summarize_probes_final.py
--rw-r--r--   0        0        0      796 2024-01-30 09:02:49.166937 probe_design-0.2.8/probe_design/src/test.py
--rw-r--r--   0        0        0      732 2024-03-04 17:38:21.313577 probe_design-0.2.8/pyproject.toml
--rw-r--r--   0        0        0    11665 1970-01-01 00:00:00.000000 probe_design-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1027 2023-12-27 11:04:31.964287 probe_design-0.2.9/LICENSE
+-rw-r--r--   0        0        0    10758 2024-03-04 17:08:35.580527 probe_design-0.2.9/README.md
+-rw-r--r--   0        0        0     1439 2024-01-29 09:13:22.868827 probe_design-0.2.9/probe_design/__init__.py
+-rw-r--r--   0        0        0       82 2023-12-27 11:04:31.994619 probe_design-0.2.9/probe_design/data/exclude/excl_roi_1.bed
+-rw-r--r--   0        0        0       97 2023-12-27 11:04:31.995005 probe_design-0.2.9/probe_design/data/exclude/excl_roi_10.bed
+-rw-r--r--   0        0        0       96 2023-12-27 11:04:31.995340 probe_design-0.2.9/probe_design/data/exclude/excl_roi_11.bed
+-rw-r--r--   0        0        0       99 2023-12-27 11:04:31.995677 probe_design-0.2.9/probe_design/data/exclude/excl_roi_12.bed
+-rw-r--r--   0        0        0       96 2023-12-27 11:04:31.996162 probe_design-0.2.9/probe_design/data/exclude/excl_roi_2.bed
+-rw-r--r--   0        0        0       98 2023-12-27 11:04:31.996466 probe_design-0.2.9/probe_design/data/exclude/excl_roi_3.bed
+-rw-r--r--   0        0        0       96 2023-12-27 11:04:31.996749 probe_design-0.2.9/probe_design/data/exclude/excl_roi_4.bed
+-rw-r--r--   0        0        0       96 2023-12-27 11:04:31.997073 probe_design-0.2.9/probe_design/data/exclude/excl_roi_5.bed
+-rw-r--r--   0        0        0       98 2023-12-27 11:04:31.997375 probe_design-0.2.9/probe_design/data/exclude/excl_roi_6.bed
+-rw-r--r--   0        0        0       97 2023-12-27 11:04:31.997734 probe_design-0.2.9/probe_design/data/exclude/excl_roi_7.bed
+-rw-r--r--   0        0        0       97 2023-12-27 11:04:31.998055 probe_design-0.2.9/probe_design/data/exclude/excl_roi_8.bed
+-rw-r--r--   0        0        0       96 2023-12-27 11:04:31.998471 probe_design-0.2.9/probe_design/data/exclude/excl_roi_9.bed
+-rw-r--r--   0        0        0    21733 2023-12-27 11:04:31.999411 probe_design-0.2.9/probe_design/data/rois/DNA_FISH_template.ods
+-rw-r--r--   0        0        0    17661 2023-12-27 11:04:32.000083 probe_design-0.2.9/probe_design/data/rois/DNA_RNA_FISH_template.ods
+-rw-r--r--   0        0        0    30029 2023-12-27 11:04:32.000635 probe_design-0.2.9/probe_design/data/rois/RNA_FISH_template.ods
+-rw-r--r--   0        0        0      515 2023-12-27 11:04:32.001141 probe_design-0.2.9/probe_design/data/rois/all_regions.tsv
+-rw-r--r--   0        0        0       62 2023-12-27 11:04:32.001655 probe_design-0.2.9/probe_design/data/rois/df_DNA_FISH.txt
+-rw-r--r--   0        0        0      154 2023-12-27 11:04:32.002115 probe_design-0.2.9/probe_design/data/rois/df_DNA_RNA_FISH.txt
+-rw-r--r--   0        0        0      247 2023-12-27 11:04:32.002541 probe_design-0.2.9/probe_design/data/rois/df_RNA_FISH.txt
+-rw-r--r--   0        0        0     2949 2024-02-22 11:09:10.840678 probe_design-0.2.9/probe_design/main.py
+-rw-r--r--   0        0        0     5076 2023-12-27 11:04:32.036740 probe_design-0.2.9/probe_design/notebooks/plot_oligos.ipynb
+-rw-r--r--   0        0        0    15318 2023-12-27 11:04:32.037331 probe_design-0.2.9/probe_design/notebooks/plot_probe_candidates.ipynb
+-rw-r--r--   0        0        0     5086 2023-12-27 11:04:32.037940 probe_design-0.2.9/probe_design/notebooks/plot_probes.ipynb
+-rw-r--r--   0        0        0     1619 2023-12-27 11:04:32.038806 probe_design-0.2.9/probe_design/shell/apply_blacklist.sh
+-rw-r--r--   0        0        0     1807 2024-02-22 12:31:56.143592 probe_design-0.2.9/probe_design/shell/build-db.sh
+-rw-r--r--   0        0        0     3520 2024-02-22 12:31:16.514067 probe_design-0.2.9/probe_design/shell/build-db_BL.sh
+-rw-r--r--   0        0        0     1451 2024-02-22 12:31:43.215584 probe_design-0.2.9/probe_design/shell/build-db_cc.sh
+-rw-r--r--   0        0        0     1201 2023-12-27 11:04:32.040735 probe_design-0.2.9/probe_design/shell/generate_blacklist.sh
+-rw-r--r--   0        0        0      857 2023-12-27 11:04:32.041184 probe_design-0.2.9/probe_design/shell/get_ref_genome.sh
+-rw-r--r--   0        0        0       97 2024-02-22 11:09:10.841735 probe_design-0.2.9/probe_design/shell/makedirs.sh
+-rw-r--r--   0        0        0      720 2024-02-22 11:09:10.842306 probe_design-0.2.9/probe_design/shell/melt_secs_parallel.sh
+-rw-r--r--   0        0        0     2362 2023-12-27 11:04:32.042486 probe_design-0.2.9/probe_design/shell/pipeline.sh
+-rw-r--r--   0        0        0     2745 2023-12-27 11:04:32.042976 probe_design-0.2.9/probe_design/shell/pipeline_exclude.sh
+-rw-r--r--   0        0        0     2826 2023-12-27 11:04:32.043433 probe_design-0.2.9/probe_design/shell/probe-query.sh
+-rw-r--r--   0        0        0     4422 2024-02-05 10:18:01.859852 probe_design-0.2.9/probe_design/shell/run_nHUSH.sh
+-rw-r--r--   0        0        0     5171 2024-02-05 10:17:03.523669 probe_design-0.2.9/probe_design/shell/run_nHUSH_excl.sh
+-rw-r--r--   0        0        0      338 2023-12-29 15:06:22.909485 probe_design-0.2.9/probe_design/shell/show.sh
+-rw-r--r--   0        0        0       22 2024-01-29 14:30:38.732109 probe_design-0.2.9/probe_design/shell/test_shell.sh
+-rw-r--r--   0        0        0      735 2023-12-27 11:04:32.045065 probe_design-0.2.9/probe_design/shell/unfinished_HUSH.sh
+-rw-r--r--   0        0        0     3552 2024-02-05 10:16:36.206369 probe_design-0.2.9/probe_design/shell/validation_oldHUSH_BLAST.sh
+-rw-r--r--   0        0        0     3560 2024-01-08 11:24:09.444010 probe_design-0.2.9/probe_design/src/HUSH_feedback.py
+-rw-r--r--   0        0        0     1827 2024-03-04 17:37:19.708500 probe_design-0.2.9/probe_design/src/__init__.py
+-rw-r--r--   0        0        0    23845 2024-02-22 11:09:10.842932 probe_design-0.2.9/probe_design/src/cycling_query.py
+-rw-r--r--   0        0        0     8046 2024-01-11 14:36:50.223140 probe_design-0.2.9/probe_design/src/download_chromosomes.py
+-rw-r--r--   0        0        0     9275 2024-03-04 17:08:35.582944 probe_design-0.2.9/probe_design/src/escafish_score.py
+-rw-r--r--   0        0        0     8497 2024-03-04 18:28:27.540344 probe_design-0.2.9/probe_design/src/escafish_score_old.py
+-rw-r--r--   0        0        0     3163 2024-03-04 17:08:35.583496 probe_design-0.2.9/probe_design/src/exclude_region.py
+-rw-r--r--   0        0        0     1446 2024-01-02 10:41:11.267835 probe_design-0.2.9/probe_design/src/generate_exclude.py
+-rw-r--r--   0        0        0     4314 2024-03-04 17:08:35.584658 probe_design-0.2.9/probe_design/src/get_oligos.py
+-rw-r--r--   0        0        0     3331 2023-12-27 11:04:32.050271 probe_design-0.2.9/probe_design/src/prepare_input.r
+-rw-r--r--   0        0        0     4177 2024-01-08 11:39:19.105676 probe_design-0.2.9/probe_design/src/reform_hush.py
+-rw-r--r--   0        0        0     5134 2024-03-04 17:37:42.432020 probe_design-0.2.9/probe_design/src/reform_hush_combined.py
+-rw-r--r--   0        0        0     5598 2024-01-08 11:29:55.409099 probe_design-0.2.9/probe_design/src/reform_hush_combined_new.py
+-rw-r--r--   0        0        0     6620 2024-01-08 11:42:47.175118 probe_design-0.2.9/probe_design/src/reform_hush_consec.py
+-rw-r--r--   0        0        0     5167 2024-01-02 11:59:24.604027 probe_design-0.2.9/probe_design/src/select_probe.py
+-rw-r--r--   0        0        0      785 2024-03-04 17:08:35.585612 probe_design-0.2.9/probe_design/src/split_fasta.py
+-rw-r--r--   0        0        0     3546 2024-01-02 12:38:28.314063 probe_design-0.2.9/probe_design/src/summarize_probes.py
+-rw-r--r--   0        0        0     4050 2024-01-02 12:38:28.313904 probe_design-0.2.9/probe_design/src/summarize_probes_cumul.py
+-rw-r--r--   0        0        0     4081 2023-12-27 11:04:32.054742 probe_design-0.2.9/probe_design/src/summarize_probes_final.py
+-rw-r--r--   0        0        0      796 2024-01-30 09:02:49.166937 probe_design-0.2.9/probe_design/src/test.py
+-rw-r--r--   0        0        0      732 2024-03-04 18:28:43.756627 probe_design-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0    11665 1970-01-01 00:00:00.000000 probe_design-0.2.9/PKG-INFO
```

### Comparing `probe_design-0.2.8/LICENSE` & `probe_design-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `probe_design-0.2.8/README.md` & `probe_design-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `probe_design-0.2.8/probe_design/__init__.py` & `probe_design-0.2.9/probe_design/__init__.py`

 * *Files identical despite different names*

### Comparing `probe_design-0.2.8/probe_design/data/rois/DNA_FISH_template.ods` & `probe_design-0.2.9/probe_design/data/rois/DNA_FISH_template.ods`

 * *Files identical despite different names*

### Comparing `probe_design-0.2.8/probe_design/data/rois/DNA_RNA_FISH_template.ods` & `probe_design-0.2.9/probe_design/data/rois/DNA_RNA_FISH_template.ods`

 * *Files identical despite different names*

### Comparing `probe_design-0.2.8/probe_design/data/rois/RNA_FISH_template.ods` & `probe_design-0.2.9/probe_design/data/rois/RNA_FISH_template.ods`

 * *Files identical despite different names*

### Comparing `probe_design-0.2.8/probe_design/data/rois/all_regions.tsv` & `probe_design-0.2.9/probe_design/data/rois/all_regions.tsv`

 * *Files identical despite different names*

### Comparing `probe_design-0.2.8/probe_design/main.py` & `probe_design-0.2.9/probe_design/main.py`

 * *Files identical despite different names*

### Comparing `probe_design-0.2.8/probe_design/notebooks/plot_oligos.ipynb` & `probe_design-0.2.9/probe_design/notebooks/plot_oligos.ipynb`

 * *Files identical despite different names*

### Comparing `probe_design-0.2.8/probe_design/notebooks/plot_probe_candidates.ipynb` & `probe_design-0.2.9/probe_design/notebooks/plot_probe_candidates.ipynb`

 * *Files identical despite different names*

### Comparing `probe_design-0.2.8/probe_design/notebooks/plot_probes.ipynb` & `probe_design-0.2.9/probe_design/notebooks/plot_probes.ipynb`

 * *Files identical despite different names*

### Comparing `probe_design-0.2.8/probe_design/shell/apply_blacklist.sh` & `probe_design-0.2.9/probe_design/shell/apply_blacklist.sh`

 * *Files identical despite different names*

### Comparing `probe_design-0.2.8/probe_design/shell/build-db.sh` & `probe_design-0.2.9/probe_design/shell/build-db.sh`

 * *Files identical despite different names*

### Comparing `probe_design-0.2.8/probe_design/shell/build-db_BL.sh` & `probe_design-0.2.9/probe_design/shell/build-db_BL.sh`

 * *Files identical despite different names*

### Comparing `probe_design-0.2.8/probe_design/shell/build-db_cc.sh` & `probe_design-0.2.9/probe_design/shell/build-db_cc.sh`

 * *Files identical despite different names*

### Comparing `probe_design-0.2.8/probe_design/shell/generate_blacklist.sh` & `probe_design-0.2.9/probe_design/shell/generate_blacklist.sh`

 * *Files identical despite different names*

### Comparing `probe_design-0.2.8/probe_design/shell/get_ref_genome.sh` & `probe_design-0.2.9/probe_design/shell/get_ref_genome.sh`

 * *Files identical despite different names*

### Comparing `probe_design-0.2.8/probe_design/shell/melt_secs_parallel.sh` & `probe_design-0.2.9/probe_design/shell/melt_secs_parallel.sh`

 * *Files identical despite different names*

### Comparing `probe_design-0.2.8/probe_design/shell/pipeline.sh` & `probe_design-0.2.9/probe_design/shell/pipeline.sh`

 * *Files identical despite different names*

### Comparing `probe_design-0.2.8/probe_design/shell/pipeline_exclude.sh` & `probe_design-0.2.9/probe_design/shell/pipeline_exclude.sh`

 * *Files identical despite different names*

### Comparing `probe_design-0.2.8/probe_design/shell/probe-query.sh` & `probe_design-0.2.9/probe_design/shell/probe-query.sh`

 * *Files identical despite different names*

### Comparing `probe_design-0.2.8/probe_design/shell/run_nHUSH.sh` & `probe_design-0.2.9/probe_design/shell/run_nHUSH.sh`

 * *Files identical despite different names*

### Comparing `probe_design-0.2.8/probe_design/shell/run_nHUSH_excl.sh` & `probe_design-0.2.9/probe_design/shell/run_nHUSH_excl.sh`

 * *Files identical despite different names*

### Comparing `probe_design-0.2.8/probe_design/shell/unfinished_HUSH.sh` & `probe_design-0.2.9/probe_design/shell/unfinished_HUSH.sh`

 * *Files identical despite different names*

### Comparing `probe_design-0.2.8/probe_design/shell/validation_oldHUSH_BLAST.sh` & `probe_design-0.2.9/probe_design/shell/validation_oldHUSH_BLAST.sh`

 * *Files identical despite different names*

### Comparing `probe_design-0.2.8/probe_design/src/HUSH_feedback.py` & `probe_design-0.2.9/probe_design/src/HUSH_feedback.py`

 * *Files identical despite different names*

### Comparing `probe_design-0.2.8/probe_design/src/__init__.py` & `probe_design-0.2.9/probe_design/src/__init__.py`

 * *Files identical despite different names*

### Comparing `probe_design-0.2.8/probe_design/src/cycling_query.py` & `probe_design-0.2.9/probe_design/src/cycling_query.py`

 * *Files identical despite different names*

### Comparing `probe_design-0.2.8/probe_design/src/download_chromosomes.py` & `probe_design-0.2.9/probe_design/src/download_chromosomes.py`

 * *Files identical despite different names*

### Comparing `probe_design-0.2.8/probe_design/src/escafish_score.py` & `probe_design-0.2.9/probe_design/src/escafish_score.py`

 * *Files identical despite different names*

### Comparing `probe_design-0.2.8/probe_design/src/exclude_region.py` & `probe_design-0.2.9/probe_design/src/exclude_region.py`

 * *Files identical despite different names*

### Comparing `probe_design-0.2.8/probe_design/src/generate_exclude.py` & `probe_design-0.2.9/probe_design/src/generate_exclude.py`

 * *Files identical despite different names*

### Comparing `probe_design-0.2.8/probe_design/src/get_oligos.py` & `probe_design-0.2.9/probe_design/src/get_oligos.py`

 * *Files identical despite different names*

### Comparing `probe_design-0.2.8/probe_design/src/prepare_input.r` & `probe_design-0.2.9/probe_design/src/prepare_input.r`

 * *Files identical despite different names*

### Comparing `probe_design-0.2.8/probe_design/src/reform_hush.py` & `probe_design-0.2.9/probe_design/src/reform_hush.py`

 * *Files identical despite different names*

### Comparing `probe_design-0.2.8/probe_design/src/reform_hush_combined.py` & `probe_design-0.2.9/probe_design/src/reform_hush_combined.py`

 * *Files identical despite different names*

### Comparing `probe_design-0.2.8/probe_design/src/reform_hush_combined_new.py` & `probe_design-0.2.9/probe_design/src/reform_hush_combined_new.py`

 * *Files identical despite different names*

### Comparing `probe_design-0.2.8/probe_design/src/reform_hush_consec.py` & `probe_design-0.2.9/probe_design/src/reform_hush_consec.py`

 * *Files identical despite different names*

### Comparing `probe_design-0.2.8/probe_design/src/select_probe.py` & `probe_design-0.2.9/probe_design/src/select_probe.py`

 * *Files identical despite different names*

### Comparing `probe_design-0.2.8/probe_design/src/split_fasta.py` & `probe_design-0.2.9/probe_design/src/split_fasta.py`

 * *Files identical despite different names*

### Comparing `probe_design-0.2.8/probe_design/src/summarize_probes.py` & `probe_design-0.2.9/probe_design/src/summarize_probes.py`

 * *Files identical despite different names*

### Comparing `probe_design-0.2.8/probe_design/src/summarize_probes_cumul.py` & `probe_design-0.2.9/probe_design/src/summarize_probes_cumul.py`

 * *Files identical despite different names*

### Comparing `probe_design-0.2.8/probe_design/src/summarize_probes_final.py` & `probe_design-0.2.9/probe_design/src/summarize_probes_final.py`

 * *Files identical despite different names*

### Comparing `probe_design-0.2.8/probe_design/src/test.py` & `probe_design-0.2.9/probe_design/src/test.py`

 * *Files identical despite different names*

### Comparing `probe_design-0.2.8/pyproject.toml` & `probe_design-0.2.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "probe-design"
-version = "0.2.8"
+version = "0.2.9"
 description = "Probe design for FISH by Quentin Verron"
 authors = ["Quentin Verron"]
 maintainers = [
     "Quentin Verron",
     "Zafer Kosar <zafermolbio.gmail.com>"]
 license = "CC NC BY 4.0"
 readme = "README.md"
```

### Comparing `probe_design-0.2.8/PKG-INFO` & `probe_design-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: probe-design
-Version: 0.2.8
+Version: 0.2.9
 Summary: Probe design for FISH by Quentin Verron
 License: CC NC BY 4.0
 Author: Quentin Verron
 Maintainer: Quentin Verron
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

