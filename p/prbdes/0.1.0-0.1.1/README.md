# Comparing `tmp/prbdes-0.1.0.tar.gz` & `tmp/prbdes-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prbdes-0.1.0.tar", max compression
+gzip compressed data, was "prbdes-0.1.1.tar", max compression
```

## Comparing `prbdes-0.1.0.tar` & `prbdes-0.1.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0     1027 2024-04-25 16:21:04.594233 prbdes-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0    11235 2024-04-25 15:49:16.124698 prbdes-0.1.0/README.md
--rw-r--r--   0        0        0       82 2024-04-25 15:49:16.124698 prbdes-0.1.0/prbdes/data/exclude/excl_roi_1.bed
--rw-r--r--   0        0        0       97 2024-04-25 15:49:16.124698 prbdes-0.1.0/prbdes/data/exclude/excl_roi_10.bed
--rw-r--r--   0        0        0       96 2024-04-25 15:49:16.124698 prbdes-0.1.0/prbdes/data/exclude/excl_roi_11.bed
--rw-r--r--   0        0        0       99 2024-04-25 15:49:16.124698 prbdes-0.1.0/prbdes/data/exclude/excl_roi_12.bed
--rw-r--r--   0        0        0       96 2024-04-25 15:49:16.124698 prbdes-0.1.0/prbdes/data/exclude/excl_roi_2.bed
--rw-r--r--   0        0        0       98 2024-04-25 15:49:16.124698 prbdes-0.1.0/prbdes/data/exclude/excl_roi_3.bed
--rw-r--r--   0        0        0       96 2024-04-25 15:49:16.124698 prbdes-0.1.0/prbdes/data/exclude/excl_roi_4.bed
--rw-r--r--   0        0        0       96 2024-04-25 15:49:16.124698 prbdes-0.1.0/prbdes/data/exclude/excl_roi_5.bed
--rw-r--r--   0        0        0       98 2024-04-25 15:49:16.124698 prbdes-0.1.0/prbdes/data/exclude/excl_roi_6.bed
--rw-r--r--   0        0        0       97 2024-04-25 15:49:16.124698 prbdes-0.1.0/prbdes/data/exclude/excl_roi_7.bed
--rw-r--r--   0        0        0       97 2024-04-25 15:49:16.124698 prbdes-0.1.0/prbdes/data/exclude/excl_roi_8.bed
--rw-r--r--   0        0        0       96 2024-04-25 15:49:16.124698 prbdes-0.1.0/prbdes/data/exclude/excl_roi_9.bed
--rw-r--r--   0        0        0    21733 2024-04-25 15:49:16.124698 prbdes-0.1.0/prbdes/data/rois/DNA_FISH_template.ods
--rw-r--r--   0        0        0    17661 2024-04-25 15:49:16.124698 prbdes-0.1.0/prbdes/data/rois/DNA_RNA_FISH_template.ods
--rw-r--r--   0        0        0    30029 2024-04-25 15:49:16.124698 prbdes-0.1.0/prbdes/data/rois/RNA_FISH_template.ods
--rw-r--r--   0        0        0      515 2024-04-25 15:49:16.124698 prbdes-0.1.0/prbdes/data/rois/all_regions.tsv
--rw-r--r--   0        0        0       62 2024-04-25 15:49:16.124698 prbdes-0.1.0/prbdes/data/rois/df_DNA_FISH.txt
--rw-r--r--   0        0        0      154 2024-04-25 15:49:16.124698 prbdes-0.1.0/prbdes/data/rois/df_DNA_RNA_FISH.txt
--rw-r--r--   0        0        0      247 2024-04-25 15:49:16.124698 prbdes-0.1.0/prbdes/data/rois/df_RNA_FISH.txt
--rw-r--r--   0        0        0     3199 2024-04-25 15:56:53.904588 prbdes-0.1.0/prbdes/main.py
--rw-r--r--   0        0        0   198113 2024-04-25 15:49:16.134698 prbdes-0.1.0/prbdes/notebooks/plot_oligos.ipynb
--rw-r--r--   0        0        0  8848869 2024-04-25 15:49:16.214698 prbdes-0.1.0/prbdes/notebooks/plot_probe_candidates.ipynb
--rw-r--r--   0        0        0    60626 2024-04-25 15:49:16.214698 prbdes-0.1.0/prbdes/notebooks/plot_probes.ipynb
--rw-r--r--   0        0        0     1619 2024-04-25 15:49:16.124698 prbdes-0.1.0/prbdes/shell/apply_blacklist.sh
--rw-r--r--   0        0        0     1810 2024-04-25 15:59:57.854541 prbdes-0.1.0/prbdes/shell/build-db.sh
--rw-r--r--   0        0        0     3523 2024-04-25 15:59:01.174555 prbdes-0.1.0/prbdes/shell/build-db_BL.sh
--rw-r--r--   0        0        0     1454 2024-04-25 16:13:01.234343 prbdes-0.1.0/prbdes/shell/build-db_cc.sh
--rw-r--r--   0        0        0     1201 2024-04-25 15:49:16.124698 prbdes-0.1.0/prbdes/shell/generate_blacklist.sh
--rw-r--r--   0        0        0      857 2024-04-25 15:49:16.124698 prbdes-0.1.0/prbdes/shell/get_ref_genome.sh
--rw-r--r--   0        0        0      719 2024-04-25 15:49:16.134698 prbdes-0.1.0/prbdes/shell/melt_secs_parallel.sh
--rw-r--r--   0        0        0     2240 2024-04-25 15:49:16.134698 prbdes-0.1.0/prbdes/shell/pipeline.sh
--rw-r--r--   0        0        0     2570 2024-04-25 15:49:16.134698 prbdes-0.1.0/prbdes/shell/pipeline_exclude.sh
--rw-r--r--   0        0        0     2826 2024-04-25 15:49:16.214698 prbdes-0.1.0/prbdes/shell/probe-query.sh
--rw-r--r--   0        0        0     4418 2024-04-25 15:49:16.214698 prbdes-0.1.0/prbdes/shell/run_nHUSH.sh
--rw-r--r--   0        0        0     5167 2024-04-25 15:49:16.214698 prbdes-0.1.0/prbdes/shell/run_nHUSH_excl.sh
--rw-r--r--   0        0        0      735 2024-04-25 15:49:16.214698 prbdes-0.1.0/prbdes/shell/unfinished_HUSH.sh
--rw-r--r--   0        0        0     3548 2024-04-25 15:49:16.214698 prbdes-0.1.0/prbdes/shell/validation_oldHUSH_BLAST.sh
--rw-r--r--   0        0        0     3093 2024-04-25 15:49:16.124698 prbdes-0.1.0/prbdes/src/HUSH_feedback.py
--rw-r--r--   0        0        0    23353 2024-04-25 16:16:42.854294 prbdes-0.1.0/prbdes/src/cycling_query.py
--rw-r--r--   0        0        0     8497 2024-04-25 15:49:16.124698 prbdes-0.1.0/prbdes/src/escafish_score.py
--rw-r--r--   0        0        0     3038 2024-04-25 16:07:27.484434 prbdes-0.1.0/prbdes/src/exclude_region.py
--rw-r--r--   0        0        0     1362 2024-04-25 15:49:16.124698 prbdes-0.1.0/prbdes/src/generate_exclude.py
--rw-r--r--   0        0        0     3567 2024-04-25 16:07:43.094431 prbdes-0.1.0/prbdes/src/get_oligos.py
--rw-r--r--   0        0        0     3331 2024-04-25 15:49:16.214698 prbdes-0.1.0/prbdes/src/prepare_input.r
--rw-r--r--   0        0        0     3890 2024-04-25 15:49:16.214698 prbdes-0.1.0/prbdes/src/reform_hush.py
--rw-r--r--   0        0        0     5134 2024-04-25 15:49:16.214698 prbdes-0.1.0/prbdes/src/reform_hush_combined.py
--rw-r--r--   0        0        0     6161 2024-04-25 15:49:16.214698 prbdes-0.1.0/prbdes/src/reform_hush_consec.py
--rw-r--r--   0        0        0     4856 2024-04-25 15:49:16.214698 prbdes-0.1.0/prbdes/src/select_probe.py
--rw-r--r--   0        0        0      511 2024-04-25 16:10:26.674391 prbdes-0.1.0/prbdes/src/split_fasta.py
--rw-r--r--   0        0        0     3690 2024-04-25 15:49:16.214698 prbdes-0.1.0/prbdes/src/summarize-probes-cumul.py
--rw-r--r--   0        0        0     3722 2024-04-25 15:49:16.214698 prbdes-0.1.0/prbdes/src/summarize-probes-final.py
--rw-r--r--   0        0        0     3219 2024-04-25 15:49:16.214698 prbdes-0.1.0/prbdes/src/summarize-probes.py
--rw-r--r--   0        0        0      686 2024-04-25 15:56:28.524594 prbdes-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    12107 1970-01-01 00:00:00.000000 prbdes-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1027 2024-05-02 08:51:58.248826 prbdes-0.1.1/LICENSE.txt
+-rw-r--r--   0        0        0    11235 2024-05-02 08:51:58.249604 prbdes-0.1.1/README.md
+-rw-r--r--   0        0        0       82 2024-05-02 08:51:58.315733 prbdes-0.1.1/prbdes/data/exclude/excl_roi_1.bed
+-rw-r--r--   0        0        0       97 2024-05-02 08:51:58.316003 prbdes-0.1.1/prbdes/data/exclude/excl_roi_10.bed
+-rw-r--r--   0        0        0       96 2024-05-02 08:51:58.316244 prbdes-0.1.1/prbdes/data/exclude/excl_roi_11.bed
+-rw-r--r--   0        0        0       99 2024-05-02 08:51:58.316469 prbdes-0.1.1/prbdes/data/exclude/excl_roi_12.bed
+-rw-r--r--   0        0        0       96 2024-05-02 08:51:58.316687 prbdes-0.1.1/prbdes/data/exclude/excl_roi_2.bed
+-rw-r--r--   0        0        0       98 2024-05-02 08:51:58.316950 prbdes-0.1.1/prbdes/data/exclude/excl_roi_3.bed
+-rw-r--r--   0        0        0       96 2024-05-02 08:51:58.317173 prbdes-0.1.1/prbdes/data/exclude/excl_roi_4.bed
+-rw-r--r--   0        0        0       96 2024-05-02 08:51:58.317378 prbdes-0.1.1/prbdes/data/exclude/excl_roi_5.bed
+-rw-r--r--   0        0        0       98 2024-05-02 08:51:58.317570 prbdes-0.1.1/prbdes/data/exclude/excl_roi_6.bed
+-rw-r--r--   0        0        0       97 2024-05-02 08:51:58.317751 prbdes-0.1.1/prbdes/data/exclude/excl_roi_7.bed
+-rw-r--r--   0        0        0       97 2024-05-02 08:51:58.317960 prbdes-0.1.1/prbdes/data/exclude/excl_roi_8.bed
+-rw-r--r--   0        0        0       96 2024-05-02 08:51:58.318210 prbdes-0.1.1/prbdes/data/exclude/excl_roi_9.bed
+-rw-r--r--   0        0        0    21733 2024-05-02 08:51:58.318649 prbdes-0.1.1/prbdes/data/rois/DNA_FISH_template.ods
+-rw-r--r--   0        0        0    17661 2024-05-02 08:51:58.319115 prbdes-0.1.1/prbdes/data/rois/DNA_RNA_FISH_template.ods
+-rw-r--r--   0        0        0    30029 2024-05-02 08:51:58.319580 prbdes-0.1.1/prbdes/data/rois/RNA_FISH_template.ods
+-rw-r--r--   0        0        0      515 2024-05-02 08:51:58.319893 prbdes-0.1.1/prbdes/data/rois/all_regions.tsv
+-rw-r--r--   0        0        0       62 2024-05-02 08:51:58.320190 prbdes-0.1.1/prbdes/data/rois/df_DNA_FISH.txt
+-rw-r--r--   0        0        0      154 2024-05-02 08:51:58.320467 prbdes-0.1.1/prbdes/data/rois/df_DNA_RNA_FISH.txt
+-rw-r--r--   0        0        0      247 2024-05-02 08:51:58.320795 prbdes-0.1.1/prbdes/data/rois/df_RNA_FISH.txt
+-rw-r--r--   0        0        0     3199 2024-05-02 08:51:58.321796 prbdes-0.1.1/prbdes/main.py
+-rw-r--r--   0        0        0   198113 2024-05-02 08:51:58.323235 prbdes-0.1.1/prbdes/notebooks/plot_oligos.ipynb
+-rw-r--r--   0        0        0  8848869 2024-05-02 08:51:58.391017 prbdes-0.1.1/prbdes/notebooks/plot_probe_candidates.ipynb
+-rw-r--r--   0        0        0    60626 2024-05-02 08:51:58.391645 prbdes-0.1.1/prbdes/notebooks/plot_probes.ipynb
+-rw-r--r--   0        0        0     1619 2024-05-02 08:51:58.392253 prbdes-0.1.1/prbdes/shell/apply_blacklist.sh
+-rw-r--r--   0        0        0     1810 2024-05-02 08:51:58.394784 prbdes-0.1.1/prbdes/shell/build-db.sh
+-rw-r--r--   0        0        0     3523 2024-05-02 08:51:58.395808 prbdes-0.1.1/prbdes/shell/build-db_BL.sh
+-rw-r--r--   0        0        0     1454 2024-05-02 08:51:58.396729 prbdes-0.1.1/prbdes/shell/build-db_cc.sh
+-rw-r--r--   0        0        0     1201 2024-05-02 08:51:58.397158 prbdes-0.1.1/prbdes/shell/generate_blacklist.sh
+-rw-r--r--   0        0        0      857 2024-05-02 08:51:58.397466 prbdes-0.1.1/prbdes/shell/get_ref_genome.sh
+-rw-r--r--   0        0        0      719 2024-05-02 08:51:58.397780 prbdes-0.1.1/prbdes/shell/melt_secs_parallel.sh
+-rw-r--r--   0        0        0     2240 2024-05-02 08:51:58.398025 prbdes-0.1.1/prbdes/shell/pipeline.sh
+-rw-r--r--   0        0        0     2570 2024-05-02 08:51:58.398315 prbdes-0.1.1/prbdes/shell/pipeline_exclude.sh
+-rw-r--r--   0        0        0     2826 2024-05-02 08:51:58.398632 prbdes-0.1.1/prbdes/shell/probe-query.sh
+-rw-r--r--   0        0        0     4418 2024-05-02 08:51:58.399497 prbdes-0.1.1/prbdes/shell/run_nHUSH.sh
+-rw-r--r--   0        0        0     5167 2024-05-02 08:51:58.400054 prbdes-0.1.1/prbdes/shell/run_nHUSH_excl.sh
+-rw-r--r--   0        0        0      735 2024-05-02 08:51:58.400410 prbdes-0.1.1/prbdes/shell/unfinished_HUSH.sh
+-rw-r--r--   0        0        0     3548 2024-05-02 08:51:58.400712 prbdes-0.1.1/prbdes/shell/validation_oldHUSH_BLAST.sh
+-rw-r--r--   0        0        0     3093 2024-05-02 08:51:58.401371 prbdes-0.1.1/prbdes/src/HUSH_feedback.py
+-rw-r--r--   0        0        0    23353 2024-05-02 08:51:58.402408 prbdes-0.1.1/prbdes/src/cycling_query.py
+-rw-r--r--   0        0        0     8497 2024-05-02 08:51:58.402904 prbdes-0.1.1/prbdes/src/escafish_score.py
+-rw-r--r--   0        0        0     3038 2024-05-02 08:51:58.403712 prbdes-0.1.1/prbdes/src/exclude_region.py
+-rw-r--r--   0        0        0     1362 2024-05-02 08:51:58.404074 prbdes-0.1.1/prbdes/src/generate_exclude.py
+-rw-r--r--   0        0        0     3567 2024-05-02 08:51:58.404889 prbdes-0.1.1/prbdes/src/get_oligos.py
+-rw-r--r--   0        0        0     3331 2024-05-02 08:51:58.405313 prbdes-0.1.1/prbdes/src/prepare_input.r
+-rw-r--r--   0        0        0     3890 2024-05-02 08:51:58.405698 prbdes-0.1.1/prbdes/src/reform_hush.py
+-rw-r--r--   0        0        0     5134 2024-05-02 08:51:58.406116 prbdes-0.1.1/prbdes/src/reform_hush_combined.py
+-rw-r--r--   0        0        0     6161 2024-05-02 08:51:58.406503 prbdes-0.1.1/prbdes/src/reform_hush_consec.py
+-rw-r--r--   0        0        0     4856 2024-05-02 08:51:58.406906 prbdes-0.1.1/prbdes/src/select_probe.py
+-rw-r--r--   0        0        0      511 2024-05-02 08:51:58.407666 prbdes-0.1.1/prbdes/src/split_fasta.py
+-rw-r--r--   0        0        0     3690 2024-05-02 08:51:58.408141 prbdes-0.1.1/prbdes/src/summarize-probes-cumul.py
+-rw-r--r--   0        0        0     3722 2024-05-02 08:51:58.408499 prbdes-0.1.1/prbdes/src/summarize-probes-final.py
+-rw-r--r--   0        0        0     3219 2024-05-02 08:51:58.408832 prbdes-0.1.1/prbdes/src/summarize-probes.py
+-rw-r--r--   0        0        0      678 2024-05-02 08:54:12.904787 prbdes-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    12107 1970-01-01 00:00:00.000000 prbdes-0.1.1/PKG-INFO
```

### Comparing `prbdes-0.1.0/LICENSE.txt` & `prbdes-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `prbdes-0.1.0/README.md` & `prbdes-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `prbdes-0.1.0/prbdes/data/rois/DNA_FISH_template.ods` & `prbdes-0.1.1/prbdes/data/rois/DNA_FISH_template.ods`

 * *Files identical despite different names*

### Comparing `prbdes-0.1.0/prbdes/data/rois/DNA_RNA_FISH_template.ods` & `prbdes-0.1.1/prbdes/data/rois/DNA_RNA_FISH_template.ods`

 * *Files identical despite different names*

### Comparing `prbdes-0.1.0/prbdes/data/rois/RNA_FISH_template.ods` & `prbdes-0.1.1/prbdes/data/rois/RNA_FISH_template.ods`

 * *Files identical despite different names*

### Comparing `prbdes-0.1.0/prbdes/data/rois/all_regions.tsv` & `prbdes-0.1.1/prbdes/data/rois/all_regions.tsv`

 * *Files identical despite different names*

### Comparing `prbdes-0.1.0/prbdes/main.py` & `prbdes-0.1.1/prbdes/main.py`

 * *Files identical despite different names*

### Comparing `prbdes-0.1.0/prbdes/notebooks/plot_oligos.ipynb` & `prbdes-0.1.1/prbdes/notebooks/plot_oligos.ipynb`

 * *Files identical despite different names*

### Comparing `prbdes-0.1.0/prbdes/notebooks/plot_probe_candidates.ipynb` & `prbdes-0.1.1/prbdes/notebooks/plot_probe_candidates.ipynb`

 * *Files identical despite different names*

### Comparing `prbdes-0.1.0/prbdes/notebooks/plot_probes.ipynb` & `prbdes-0.1.1/prbdes/notebooks/plot_probes.ipynb`

 * *Files identical despite different names*

### Comparing `prbdes-0.1.0/prbdes/shell/apply_blacklist.sh` & `prbdes-0.1.1/prbdes/shell/apply_blacklist.sh`

 * *Files identical despite different names*

### Comparing `prbdes-0.1.0/prbdes/shell/build-db.sh` & `prbdes-0.1.1/prbdes/shell/build-db.sh`

 * *Files identical despite different names*

### Comparing `prbdes-0.1.0/prbdes/shell/build-db_BL.sh` & `prbdes-0.1.1/prbdes/shell/build-db_BL.sh`

 * *Files identical despite different names*

### Comparing `prbdes-0.1.0/prbdes/shell/build-db_cc.sh` & `prbdes-0.1.1/prbdes/shell/build-db_cc.sh`

 * *Files identical despite different names*

### Comparing `prbdes-0.1.0/prbdes/shell/generate_blacklist.sh` & `prbdes-0.1.1/prbdes/shell/generate_blacklist.sh`

 * *Files identical despite different names*

### Comparing `prbdes-0.1.0/prbdes/shell/get_ref_genome.sh` & `prbdes-0.1.1/prbdes/shell/get_ref_genome.sh`

 * *Files identical despite different names*

### Comparing `prbdes-0.1.0/prbdes/shell/melt_secs_parallel.sh` & `prbdes-0.1.1/prbdes/shell/melt_secs_parallel.sh`

 * *Files identical despite different names*

### Comparing `prbdes-0.1.0/prbdes/shell/pipeline.sh` & `prbdes-0.1.1/prbdes/shell/pipeline.sh`

 * *Files identical despite different names*

### Comparing `prbdes-0.1.0/prbdes/shell/pipeline_exclude.sh` & `prbdes-0.1.1/prbdes/shell/pipeline_exclude.sh`

 * *Files identical despite different names*

### Comparing `prbdes-0.1.0/prbdes/shell/probe-query.sh` & `prbdes-0.1.1/prbdes/shell/probe-query.sh`

 * *Files identical despite different names*

### Comparing `prbdes-0.1.0/prbdes/shell/run_nHUSH.sh` & `prbdes-0.1.1/prbdes/shell/run_nHUSH.sh`

 * *Files identical despite different names*

### Comparing `prbdes-0.1.0/prbdes/shell/run_nHUSH_excl.sh` & `prbdes-0.1.1/prbdes/shell/run_nHUSH_excl.sh`

 * *Files identical despite different names*

### Comparing `prbdes-0.1.0/prbdes/shell/unfinished_HUSH.sh` & `prbdes-0.1.1/prbdes/shell/unfinished_HUSH.sh`

 * *Files identical despite different names*

### Comparing `prbdes-0.1.0/prbdes/shell/validation_oldHUSH_BLAST.sh` & `prbdes-0.1.1/prbdes/shell/validation_oldHUSH_BLAST.sh`

 * *Files identical despite different names*

### Comparing `prbdes-0.1.0/prbdes/src/HUSH_feedback.py` & `prbdes-0.1.1/prbdes/src/HUSH_feedback.py`

 * *Files identical despite different names*

### Comparing `prbdes-0.1.0/prbdes/src/cycling_query.py` & `prbdes-0.1.1/prbdes/src/cycling_query.py`

 * *Files identical despite different names*

### Comparing `prbdes-0.1.0/prbdes/src/escafish_score.py` & `prbdes-0.1.1/prbdes/src/escafish_score.py`

 * *Files identical despite different names*

### Comparing `prbdes-0.1.0/prbdes/src/exclude_region.py` & `prbdes-0.1.1/prbdes/src/exclude_region.py`

 * *Files identical despite different names*

### Comparing `prbdes-0.1.0/prbdes/src/generate_exclude.py` & `prbdes-0.1.1/prbdes/src/generate_exclude.py`

 * *Files identical despite different names*

### Comparing `prbdes-0.1.0/prbdes/src/get_oligos.py` & `prbdes-0.1.1/prbdes/src/get_oligos.py`

 * *Files identical despite different names*

### Comparing `prbdes-0.1.0/prbdes/src/prepare_input.r` & `prbdes-0.1.1/prbdes/src/prepare_input.r`

 * *Files identical despite different names*

### Comparing `prbdes-0.1.0/prbdes/src/reform_hush.py` & `prbdes-0.1.1/prbdes/src/reform_hush.py`

 * *Files identical despite different names*

### Comparing `prbdes-0.1.0/prbdes/src/reform_hush_combined.py` & `prbdes-0.1.1/prbdes/src/reform_hush_combined.py`

 * *Files identical despite different names*

### Comparing `prbdes-0.1.0/prbdes/src/reform_hush_consec.py` & `prbdes-0.1.1/prbdes/src/reform_hush_consec.py`

 * *Files identical despite different names*

### Comparing `prbdes-0.1.0/prbdes/src/select_probe.py` & `prbdes-0.1.1/prbdes/src/select_probe.py`

 * *Files identical despite different names*

### Comparing `prbdes-0.1.0/prbdes/src/summarize-probes-cumul.py` & `prbdes-0.1.1/prbdes/src/summarize-probes-cumul.py`

 * *Files identical despite different names*

### Comparing `prbdes-0.1.0/prbdes/src/summarize-probes-final.py` & `prbdes-0.1.1/prbdes/src/summarize-probes-final.py`

 * *Files identical despite different names*

### Comparing `prbdes-0.1.0/prbdes/src/summarize-probes.py` & `prbdes-0.1.1/prbdes/src/summarize-probes.py`

 * *Files identical despite different names*

### Comparing `prbdes-0.1.0/pyproject.toml` & `prbdes-0.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "prbdes"
-version = "0.1.0"
+version = "0.1.1"
 description = "Probe design originails for FISH by Quentin Verron"
 authors = ["Quentin Verron"]
 maintainers = [
     "Quentin Verron",
     "Zafer Kosar <zafermolbio.gmail.com>"]
 license = "CC NC BY 4.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 numpy = "^1.20"
-pandas = ">=1.2.2,<3.0.0"
+pandas = "^1.2.2"
 tabulate = "^0.9.0"
 biopython = "^1.82"
 tqdm = "^4"
 joblib = "^1"
 click = "^8.1.0"
 poetry = "^1.5"
 requests = "^2.31.0"
```

### Comparing `prbdes-0.1.0/PKG-INFO` & `prbdes-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prbdes
-Version: 0.1.0
+Version: 0.1.1
 Summary: Probe design originails for FISH by Quentin Verron
 License: CC NC BY 4.0
 Author: Quentin Verron
 Maintainer: Quentin Verron
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: biopython (>=1.82,<2.0)
 Requires-Dist: click (>=8.1.0,<9.0.0)
 Requires-Dist: ifpd2q (>=1.0.3,<2.0.0)
 Requires-Dist: joblib (>=1,<2)
 Requires-Dist: numpy (>=1.20,<2.0)
-Requires-Dist: pandas (>=1.2.2,<3.0.0)
+Requires-Dist: pandas (>=1.2.2,<2.0.0)
 Requires-Dist: poetry (>=1.5,<2.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: tqdm (>=4,<5)
 Description-Content-Type: text/markdown
 
 # Instructions for probe design
```

