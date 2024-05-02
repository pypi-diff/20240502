# Comparing `tmp/BioSAK-1.87.0.tar.gz` & `tmp/BioSAK-1.87.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BioSAK-1.87.0.tar", last modified: Thu May  2 15:34:59 2024, max compression
+gzip compressed data, was "BioSAK-1.87.1.tar", last modified: Thu May  2 15:48:05 2024, max compression
```

## Comparing `BioSAK-1.87.0.tar` & `BioSAK-1.87.1.tar`

### file list

```diff
@@ -1,166 +1,166 @@
-drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2024-05-02 15:34:59.278595 BioSAK-1.87.0/
-drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2024-05-02 15:34:59.276949 BioSAK-1.87.0/BioSAK/
--rw-r--r--   0 songweizhi   (501) staff       (20)     3653 2024-01-16 05:10:59.000000 BioSAK-1.87.0/BioSAK/BLCA_op_parser.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2031 2023-05-31 05:26:00.000000 BioSAK-1.87.0/BioSAK/BioSAK_config.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)    39300 2024-03-22 00:45:31.000000 BioSAK-1.87.0/BioSAK/COG2020.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3615 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/COG_boxplot_last1row.R
--rw-r--r--   0 songweizhi   (501) staff       (20)     6974 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/COG_boxplot_last2row.R
--rwxr-xr-x   0 songweizhi   (501) staff       (20)     6067 2024-01-16 05:00:13.000000 BioSAK-1.87.0/BioSAK/CheckM.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     5891 2024-01-16 05:10:59.000000 BioSAK-1.87.0/BioSAK/ConvertMSA.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    16671 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/DnaFeaturesViewer.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2292 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/FastaSplitler_by_num.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2485 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/FastaSplitler_by_size.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2190 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/GTDB_for_BLCA.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1321 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/Gene2Ctg.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    45147 2024-03-23 14:54:03.000000 BioSAK-1.87.0/BioSAK/KEGG.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3484 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/KEGG_boxplot_last1row.R
--rw-r--r--   0 songweizhi   (501) staff       (20)      269 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/KEGG_get_eukaryotic_kos.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3077 2023-08-22 09:31:28.000000 BioSAK-1.87.0/BioSAK/KeepRemovingTmp.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2620 2024-01-16 05:10:59.000000 BioSAK-1.87.0/BioSAK/MeanMappingDepth.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3682 2024-01-16 12:39:58.000000 BioSAK-1.87.0/BioSAK/MetaBiosample.py
--rw-r--r--   0 songweizhi   (501) staff       (20)  3297822 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/MetaCHIP_phylo.hmm
--rw-r--r--   0 songweizhi   (501) staff       (20)  1206805 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/MetaCyc_reactions_with_ec.txt
--rw-r--r--   0 songweizhi   (501) staff       (20)    16960 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/NetEnzymes.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3713 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/Newick_tree_plotter.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1659 2024-01-16 05:10:59.000000 BioSAK-1.87.0/BioSAK/OneLineAln.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    10448 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/Prodigal.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     6048 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/Reads_simulator.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3573 2024-01-16 05:10:59.000000 BioSAK-1.87.0/BioSAK/RunGraphMB.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3833 2024-01-16 05:10:59.000000 BioSAK-1.87.0/BioSAK/SILVA_for_BLCA.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)     6255 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/SankeyTaxon.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     5678 2024-01-16 05:10:59.000000 BioSAK-1.87.0/BioSAK/SliceMSA.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3173 2024-01-16 05:10:59.000000 BioSAK-1.87.0/BioSAK/SubsampleLongReads.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)     1696 2024-01-16 05:10:59.000000 BioSAK-1.87.0/BioSAK/Tax4Fun2IndOTU.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3661 2024-05-02 15:34:57.000000 BioSAK-1.87.0/BioSAK/VERSION
--rw-r--r--   0 songweizhi   (501) staff       (20)      467 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/VisBlastOp.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     9944 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/VisGeneFlk.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/__init__.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2526 2024-03-25 14:00:14.000000 BioSAK-1.87.0/BioSAK/add_desc.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)    38577 2024-03-22 00:45:31.000000 BioSAK-1.87.0/BioSAK/arCOG.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     6985 2024-01-16 05:00:13.000000 BioSAK-1.87.0/BioSAK/bam2reads.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)     2630 2024-03-22 13:23:45.000000 BioSAK-1.87.0/BioSAK/boxplot.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3312 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/boxplot_last1row.R
--rw-r--r--   0 songweizhi   (501) staff       (20)     6104 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/boxplot_matrix_COG.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     5403 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/boxplot_matrix_COG_backup.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     6984 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/boxplot_matrix_KEGG.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     5747 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/boxplot_matrix_dbCAN.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1695 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/cat_fa.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    13440 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/cdd2cog.pl
--rw-r--r--   0 songweizhi   (501) staff       (20)     1186 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/checkm_marker.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1421 2024-05-02 15:31:51.000000 BioSAK-1.87.0/BioSAK/compare_sets.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1076 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/compare_trees.R
--rw-r--r--   0 songweizhi   (501) staff       (20)     9745 2024-01-16 05:10:59.000000 BioSAK-1.87.0/BioSAK/compare_trees.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     6592 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/cross_link_seqs.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    24033 2024-03-22 00:45:31.000000 BioSAK-1.87.0/BioSAK/dbCAN.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1936 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/download_GenBank_genome_subset_prokaryotes_csv.py
--rw-r--r--   0 songweizhi   (501) staff       (20)      767 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/dwnld_sra_reads.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)    13250 2024-03-22 08:01:22.000000 BioSAK-1.87.0/BioSAK/enrich.py
--rw-r--r--   0 songweizhi   (501) staff       (20)      929 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/exe_cmds.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1508 2023-12-05 01:06:39.000000 BioSAK-1.87.0/BioSAK/ezaai2mat.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1396 2023-12-05 01:02:55.000000 BioSAK-1.87.0/BioSAK/fa2id.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1195 2023-05-17 06:14:50.000000 BioSAK-1.87.0/BioSAK/fa2phy.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1363 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/fa2tree.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     6280 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/format_converter.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)     2861 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/format_leaf_name.py
--rw-r--r--   0 songweizhi   (501) staff       (20)      639 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/fq2fa.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3204 2024-04-19 15:04:59.000000 BioSAK-1.87.0/BioSAK/gapseq.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2846 2023-06-14 10:08:30.000000 BioSAK-1.87.0/BioSAK/gbk2faa.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3342 2023-06-14 10:14:13.000000 BioSAK-1.87.0/BioSAK/gbk2ffn.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2528 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/gbk2fna.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     6886 2024-04-29 03:23:48.000000 BioSAK-1.87.0/BioSAK/gbk2gff.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3726 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/gbk_to_ffn_faa.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1887 2024-04-15 02:59:40.000000 BioSAK-1.87.0/BioSAK/gc.py
--rw-r--r--   0 songweizhi   (501) staff       (20)      813 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/get_EC_from_ko_stats_D.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     7477 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/get_GTDB_taxon_gnm.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     5428 2023-06-15 03:03:02.000000 BioSAK-1.87.0/BioSAK/get_MAG_reads_long.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3991 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/get_Pfam_hmms.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    29246 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/get_SCG_tree.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1784 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/get_TopHits_taxonomy.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2247 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/get_aa_composition.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    12066 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/get_bin_abundance copy.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2139 2024-01-23 11:57:14.000000 BioSAK-1.87.0/BioSAK/get_data_matrix.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     5523 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/get_gene_depth.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3591 2024-01-16 05:10:59.000000 BioSAK-1.87.0/BioSAK/get_genome_GTDB.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     6070 2024-01-16 04:57:23.000000 BioSAK-1.87.0/BioSAK/get_genome_NCBI.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    11209 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/get_genome_NCBI_v1.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    12620 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/get_genome_NCBI_v2.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3048 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/get_gnm_size.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     4834 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/get_ko_gene_seqs.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1192 2023-09-21 08:44:42.000000 BioSAK-1.87.0/BioSAK/get_krona_plot.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1559 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/get_reads_from_sam.py
--rw-r--r--   0 songweizhi   (501) staff       (20)      792 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/get_reads_id_in_sam.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2386 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/get_sankey_plot.R
--rw-r--r--   0 songweizhi   (501) staff       (20)     4242 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/get_top_hit.py
--rw-r--r--   0 songweizhi   (501) staff       (20)      820 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/get_total_length.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1834 2024-04-29 04:11:58.000000 BioSAK-1.87.0/BioSAK/gff2chrom.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     4643 2023-05-18 01:37:58.000000 BioSAK-1.87.0/BioSAK/global_functions.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)     2910 2024-03-11 00:57:02.000000 BioSAK-1.87.0/BioSAK/hpc3.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    26872 2024-04-12 00:51:29.000000 BioSAK-1.87.0/BioSAK/iTOL.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3337 2024-03-07 03:01:35.000000 BioSAK-1.87.0/BioSAK/js_cmds.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3281 2024-04-08 09:48:49.000000 BioSAK-1.87.0/BioSAK/js_hpc3.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1643 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/keep_best_hit.py
--rw-r--r--   0 songweizhi   (501) staff       (20)  3361029 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/ko00001.keg
--rw-r--r--   0 songweizhi   (501) staff       (20)     1848 2024-03-10 15:18:30.000000 BioSAK-1.87.0/BioSAK/koala.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2772 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/label_tree.R
--rw-r--r--   0 songweizhi   (501) staff       (20)     4788 2024-01-16 05:10:59.000000 BioSAK-1.87.0/BioSAK/label_tree.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    35857 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/link_16S_MAG.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    12349 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/magabund.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    19855 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/magabund2.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1224 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/manipulator_fasta.py
--rw-r--r--   0 songweizhi   (501) staff       (20)        0 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/manipulator_msa.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3659 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/manipulator_newick.py
--rw-r--r--   0 songweizhi   (501) staff       (20)        0 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/manipulator_sam.py
--rw-r--r--   0 songweizhi   (501) staff       (20)      903 2024-04-17 08:12:49.000000 BioSAK-1.87.0/BioSAK/mannwhitneyu.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2433 2023-05-30 01:59:44.000000 BioSAK-1.87.0/BioSAK/mean_MAG_cov.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1880 2024-03-25 06:45:20.000000 BioSAK-1.87.0/BioSAK/merge_df.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2405 2024-01-16 05:10:59.000000 BioSAK-1.87.0/BioSAK/merge_seq.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     6742 2024-01-23 07:37:01.000000 BioSAK-1.87.0/BioSAK/metaAssembly.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1327 2023-06-11 13:56:21.000000 BioSAK-1.87.0/BioSAK/metabat2concoct.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1612 2023-06-11 16:00:51.000000 BioSAK-1.87.0/BioSAK/metabat2maxbin.py
--rw-r--r--   0 songweizhi   (501) staff       (20)        0 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/msa_to_distance_matrix.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1759 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/ncbi_dataset.py
--rw-r--r--   0 songweizhi   (501) staff       (20)        0 2024-03-03 11:00:02.000000 BioSAK-1.87.0/BioSAK/odp.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2820 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/parse_MetaCyc_RxnDB.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1460 2023-09-18 14:42:31.000000 BioSAK-1.87.0/BioSAK/parse_mmseqs_tsv.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     8633 2024-01-16 05:10:59.000000 BioSAK-1.87.0/BioSAK/plot_mag.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     7332 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/plot_sam_depth.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1638 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/plot_tree.R
--rw-r--r--   0 songweizhi   (501) staff       (20)     2256 2023-07-22 00:36:16.000000 BioSAK-1.87.0/BioSAK/prefix_file.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     4221 2024-01-16 05:10:59.000000 BioSAK-1.87.0/BioSAK/prokka.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     5057 2023-08-03 02:58:56.000000 BioSAK-1.87.0/BioSAK/reads2bam.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)     2534 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/rename_leaves.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2005 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/rename_reads_for_Reago.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     6801 2023-10-26 11:55:44.000000 BioSAK-1.87.0/BioSAK/rename_seq.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2210 2024-01-16 05:10:59.000000 BioSAK-1.87.0/BioSAK/rename_seqs.py
--rw-r--r--   0 songweizhi   (501) staff       (20)    15703 2024-04-29 07:37:26.000000 BioSAK-1.87.0/BioSAK/ribbon.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1996 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/sam2bam.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     6877 2023-05-13 11:01:19.000000 BioSAK-1.87.0/BioSAK/sampling_GTDB_gnms.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3603 2024-01-16 05:10:59.000000 BioSAK-1.87.0/BioSAK/select_seq.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3167 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/sep_reads_by_barcode.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2671 2024-01-16 05:10:59.000000 BioSAK-1.87.0/BioSAK/slice_seq.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     3788 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/split_fasta.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     1998 2024-01-16 05:10:59.000000 BioSAK-1.87.0/BioSAK/split_folder.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     4561 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/split_sam.py
--rwxr-xr-x   0 songweizhi   (501) staff       (20)     1204 2024-01-16 05:10:59.000000 BioSAK-1.87.0/BioSAK/submitHPC.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2011 2024-01-16 05:10:59.000000 BioSAK-1.87.0/BioSAK/subset_GTDB_meta.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     4585 2024-04-09 03:15:33.000000 BioSAK-1.87.0/BioSAK/subset_df.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     7296 2024-01-16 05:10:59.000000 BioSAK-1.87.0/BioSAK/subset_tree.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     7844 2024-01-16 05:10:59.000000 BioSAK-1.87.0/BioSAK/top_16S_hits.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2106 2023-05-09 01:09:35.000000 BioSAK-1.87.0/BioSAK/top_hits_in_a_group.py
--rw-r--r--   0 songweizhi   (501) staff       (20)      831 2024-04-09 06:05:51.000000 BioSAK-1.87.0/BioSAK/transpose.py
--rw-r--r--   0 songweizhi   (501) staff       (20)     2252 2024-01-16 05:10:59.000000 BioSAK-1.87.0/BioSAK/usearch_uc.py
--rw-r--r--   0 songweizhi   (501) staff       (20)      962 2024-04-17 08:12:49.000000 BioSAK-1.87.0/BioSAK/wilcox.py
-drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2024-05-02 15:34:59.278042 BioSAK-1.87.0/BioSAK.egg-info/
--rw-r--r--   0 songweizhi   (501) staff       (20)      508 2024-05-02 15:34:59.000000 BioSAK-1.87.0/BioSAK.egg-info/PKG-INFO
--rw-r--r--   0 songweizhi   (501) staff       (20)     3727 2024-05-02 15:34:59.000000 BioSAK-1.87.0/BioSAK.egg-info/SOURCES.txt
--rw-r--r--   0 songweizhi   (501) staff       (20)        1 2024-05-02 15:34:59.000000 BioSAK-1.87.0/BioSAK.egg-info/dependency_links.txt
--rw-r--r--   0 songweizhi   (501) staff       (20)       95 2024-05-02 15:34:59.000000 BioSAK-1.87.0/BioSAK.egg-info/requires.txt
--rw-r--r--   0 songweizhi   (501) staff       (20)        7 2024-05-02 15:34:59.000000 BioSAK-1.87.0/BioSAK.egg-info/top_level.txt
--rw-r--r--   0 songweizhi   (501) staff       (20)    35141 2023-05-09 01:09:36.000000 BioSAK-1.87.0/LICENSE
--rwxr-xr-x   0 songweizhi   (501) staff       (20)      300 2023-05-09 01:09:36.000000 BioSAK-1.87.0/MANIFEST.in
--rw-r--r--   0 songweizhi   (501) staff       (20)      508 2024-05-02 15:34:59.278341 BioSAK-1.87.0/PKG-INFO
--rw-r--r--   0 songweizhi   (501) staff       (20)     1533 2024-01-23 07:37:01.000000 BioSAK-1.87.0/README.md
-drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2024-05-02 15:34:59.277814 BioSAK-1.87.0/bin/
--rwxr-xr-x   0 songweizhi   (501) staff       (20)    78071 2024-05-02 15:34:57.000000 BioSAK-1.87.0/bin/BioSAK
--rw-r--r--   0 songweizhi   (501) staff       (20)       38 2024-05-02 15:34:59.278648 BioSAK-1.87.0/setup.cfg
--rw-r--r--   0 songweizhi   (501) staff       (20)      915 2024-01-15 11:41:11.000000 BioSAK-1.87.0/setup.py
+drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2024-05-02 15:48:05.231718 BioSAK-1.87.1/
+drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2024-05-02 15:48:05.230343 BioSAK-1.87.1/BioSAK/
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3653 2024-01-16 05:10:59.000000 BioSAK-1.87.1/BioSAK/BLCA_op_parser.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2031 2023-05-31 05:26:00.000000 BioSAK-1.87.1/BioSAK/BioSAK_config.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)    39300 2024-03-22 00:45:31.000000 BioSAK-1.87.1/BioSAK/COG2020.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3615 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/COG_boxplot_last1row.R
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6974 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/COG_boxplot_last2row.R
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)     6067 2024-01-16 05:00:13.000000 BioSAK-1.87.1/BioSAK/CheckM.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     5891 2024-01-16 05:10:59.000000 BioSAK-1.87.1/BioSAK/ConvertMSA.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    16671 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/DnaFeaturesViewer.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2292 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/FastaSplitler_by_num.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2485 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/FastaSplitler_by_size.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2190 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/GTDB_for_BLCA.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1321 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/Gene2Ctg.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    45147 2024-03-23 14:54:03.000000 BioSAK-1.87.1/BioSAK/KEGG.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3484 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/KEGG_boxplot_last1row.R
+-rw-r--r--   0 songweizhi   (501) staff       (20)      269 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/KEGG_get_eukaryotic_kos.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3077 2023-08-22 09:31:28.000000 BioSAK-1.87.1/BioSAK/KeepRemovingTmp.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2620 2024-01-16 05:10:59.000000 BioSAK-1.87.1/BioSAK/MeanMappingDepth.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3682 2024-01-16 12:39:58.000000 BioSAK-1.87.1/BioSAK/MetaBiosample.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)  3297822 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/MetaCHIP_phylo.hmm
+-rw-r--r--   0 songweizhi   (501) staff       (20)  1206805 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/MetaCyc_reactions_with_ec.txt
+-rw-r--r--   0 songweizhi   (501) staff       (20)    16960 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/NetEnzymes.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3713 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/Newick_tree_plotter.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1659 2024-01-16 05:10:59.000000 BioSAK-1.87.1/BioSAK/OneLineAln.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    10448 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/Prodigal.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6048 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/Reads_simulator.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3573 2024-01-16 05:10:59.000000 BioSAK-1.87.1/BioSAK/RunGraphMB.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3833 2024-01-16 05:10:59.000000 BioSAK-1.87.1/BioSAK/SILVA_for_BLCA.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)     6255 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/SankeyTaxon.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     5678 2024-01-16 05:10:59.000000 BioSAK-1.87.1/BioSAK/SliceMSA.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3173 2024-01-16 05:10:59.000000 BioSAK-1.87.1/BioSAK/SubsampleLongReads.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)     1696 2024-01-16 05:10:59.000000 BioSAK-1.87.1/BioSAK/Tax4Fun2IndOTU.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3661 2024-05-02 15:48:04.000000 BioSAK-1.87.1/BioSAK/VERSION
+-rw-r--r--   0 songweizhi   (501) staff       (20)      467 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/VisBlastOp.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     9944 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/VisGeneFlk.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/__init__.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2526 2024-03-25 14:00:14.000000 BioSAK-1.87.1/BioSAK/add_desc.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)    38577 2024-03-22 00:45:31.000000 BioSAK-1.87.1/BioSAK/arCOG.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6985 2024-01-16 05:00:13.000000 BioSAK-1.87.1/BioSAK/bam2reads.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)     2630 2024-03-22 13:23:45.000000 BioSAK-1.87.1/BioSAK/boxplot.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3312 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/boxplot_last1row.R
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6104 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/boxplot_matrix_COG.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     5403 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/boxplot_matrix_COG_backup.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6984 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/boxplot_matrix_KEGG.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     5747 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/boxplot_matrix_dbCAN.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1695 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/cat_fa.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    13440 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/cdd2cog.pl
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1186 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/checkm_marker.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1492 2024-05-02 15:48:04.000000 BioSAK-1.87.1/BioSAK/compare_sets.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1076 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/compare_trees.R
+-rw-r--r--   0 songweizhi   (501) staff       (20)     9745 2024-01-16 05:10:59.000000 BioSAK-1.87.1/BioSAK/compare_trees.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6592 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/cross_link_seqs.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    24033 2024-03-22 00:45:31.000000 BioSAK-1.87.1/BioSAK/dbCAN.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1936 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/download_GenBank_genome_subset_prokaryotes_csv.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)      767 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/dwnld_sra_reads.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)    13250 2024-03-22 08:01:22.000000 BioSAK-1.87.1/BioSAK/enrich.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)      929 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/exe_cmds.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1508 2023-12-05 01:06:39.000000 BioSAK-1.87.1/BioSAK/ezaai2mat.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1396 2023-12-05 01:02:55.000000 BioSAK-1.87.1/BioSAK/fa2id.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1195 2023-05-17 06:14:50.000000 BioSAK-1.87.1/BioSAK/fa2phy.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1363 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/fa2tree.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6280 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/format_converter.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)     2861 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/format_leaf_name.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)      639 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/fq2fa.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3204 2024-04-19 15:04:59.000000 BioSAK-1.87.1/BioSAK/gapseq.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2846 2023-06-14 10:08:30.000000 BioSAK-1.87.1/BioSAK/gbk2faa.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3342 2023-06-14 10:14:13.000000 BioSAK-1.87.1/BioSAK/gbk2ffn.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2528 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/gbk2fna.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6886 2024-04-29 03:23:48.000000 BioSAK-1.87.1/BioSAK/gbk2gff.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3726 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/gbk_to_ffn_faa.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1887 2024-04-15 02:59:40.000000 BioSAK-1.87.1/BioSAK/gc.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)      813 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/get_EC_from_ko_stats_D.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     7477 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/get_GTDB_taxon_gnm.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     5428 2023-06-15 03:03:02.000000 BioSAK-1.87.1/BioSAK/get_MAG_reads_long.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3991 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/get_Pfam_hmms.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    29246 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/get_SCG_tree.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1784 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/get_TopHits_taxonomy.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2247 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/get_aa_composition.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    12066 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/get_bin_abundance copy.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2139 2024-01-23 11:57:14.000000 BioSAK-1.87.1/BioSAK/get_data_matrix.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     5523 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/get_gene_depth.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3591 2024-01-16 05:10:59.000000 BioSAK-1.87.1/BioSAK/get_genome_GTDB.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6070 2024-01-16 04:57:23.000000 BioSAK-1.87.1/BioSAK/get_genome_NCBI.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    11209 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/get_genome_NCBI_v1.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    12620 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/get_genome_NCBI_v2.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3048 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/get_gnm_size.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     4834 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/get_ko_gene_seqs.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1192 2023-09-21 08:44:42.000000 BioSAK-1.87.1/BioSAK/get_krona_plot.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1559 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/get_reads_from_sam.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)      792 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/get_reads_id_in_sam.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2386 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/get_sankey_plot.R
+-rw-r--r--   0 songweizhi   (501) staff       (20)     4242 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/get_top_hit.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)      820 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/get_total_length.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1834 2024-04-29 04:11:58.000000 BioSAK-1.87.1/BioSAK/gff2chrom.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     4643 2023-05-18 01:37:58.000000 BioSAK-1.87.1/BioSAK/global_functions.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)     2910 2024-03-11 00:57:02.000000 BioSAK-1.87.1/BioSAK/hpc3.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    26872 2024-04-12 00:51:29.000000 BioSAK-1.87.1/BioSAK/iTOL.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3337 2024-03-07 03:01:35.000000 BioSAK-1.87.1/BioSAK/js_cmds.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3281 2024-04-08 09:48:49.000000 BioSAK-1.87.1/BioSAK/js_hpc3.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1643 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/keep_best_hit.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)  3361029 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/ko00001.keg
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1848 2024-03-10 15:18:30.000000 BioSAK-1.87.1/BioSAK/koala.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2772 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/label_tree.R
+-rw-r--r--   0 songweizhi   (501) staff       (20)     4788 2024-01-16 05:10:59.000000 BioSAK-1.87.1/BioSAK/label_tree.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    35857 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/link_16S_MAG.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    12349 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/magabund.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    19855 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/magabund2.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1224 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/manipulator_fasta.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)        0 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/manipulator_msa.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3659 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/manipulator_newick.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)        0 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/manipulator_sam.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)      903 2024-04-17 08:12:49.000000 BioSAK-1.87.1/BioSAK/mannwhitneyu.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2433 2023-05-30 01:59:44.000000 BioSAK-1.87.1/BioSAK/mean_MAG_cov.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1880 2024-03-25 06:45:20.000000 BioSAK-1.87.1/BioSAK/merge_df.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2405 2024-01-16 05:10:59.000000 BioSAK-1.87.1/BioSAK/merge_seq.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6742 2024-01-23 07:37:01.000000 BioSAK-1.87.1/BioSAK/metaAssembly.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1327 2023-06-11 13:56:21.000000 BioSAK-1.87.1/BioSAK/metabat2concoct.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1612 2023-06-11 16:00:51.000000 BioSAK-1.87.1/BioSAK/metabat2maxbin.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)        0 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/msa_to_distance_matrix.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1759 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/ncbi_dataset.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)        0 2024-03-03 11:00:02.000000 BioSAK-1.87.1/BioSAK/odp.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2820 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/parse_MetaCyc_RxnDB.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1460 2023-09-18 14:42:31.000000 BioSAK-1.87.1/BioSAK/parse_mmseqs_tsv.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     8633 2024-01-16 05:10:59.000000 BioSAK-1.87.1/BioSAK/plot_mag.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     7332 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/plot_sam_depth.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1638 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/plot_tree.R
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2256 2023-07-22 00:36:16.000000 BioSAK-1.87.1/BioSAK/prefix_file.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     4221 2024-01-16 05:10:59.000000 BioSAK-1.87.1/BioSAK/prokka.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     5057 2023-08-03 02:58:56.000000 BioSAK-1.87.1/BioSAK/reads2bam.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)     2534 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/rename_leaves.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2005 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/rename_reads_for_Reago.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6801 2023-10-26 11:55:44.000000 BioSAK-1.87.1/BioSAK/rename_seq.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2210 2024-01-16 05:10:59.000000 BioSAK-1.87.1/BioSAK/rename_seqs.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)    15703 2024-04-29 07:37:26.000000 BioSAK-1.87.1/BioSAK/ribbon.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1996 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/sam2bam.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     6877 2023-05-13 11:01:19.000000 BioSAK-1.87.1/BioSAK/sampling_GTDB_gnms.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3603 2024-01-16 05:10:59.000000 BioSAK-1.87.1/BioSAK/select_seq.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3167 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/sep_reads_by_barcode.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2671 2024-01-16 05:10:59.000000 BioSAK-1.87.1/BioSAK/slice_seq.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3788 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/split_fasta.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1998 2024-01-16 05:10:59.000000 BioSAK-1.87.1/BioSAK/split_folder.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     4561 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/split_sam.py
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)     1204 2024-01-16 05:10:59.000000 BioSAK-1.87.1/BioSAK/submitHPC.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2011 2024-01-16 05:10:59.000000 BioSAK-1.87.1/BioSAK/subset_GTDB_meta.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     4585 2024-04-09 03:15:33.000000 BioSAK-1.87.1/BioSAK/subset_df.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     7296 2024-01-16 05:10:59.000000 BioSAK-1.87.1/BioSAK/subset_tree.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     7844 2024-01-16 05:10:59.000000 BioSAK-1.87.1/BioSAK/top_16S_hits.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2106 2023-05-09 01:09:35.000000 BioSAK-1.87.1/BioSAK/top_hits_in_a_group.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)      831 2024-04-09 06:05:51.000000 BioSAK-1.87.1/BioSAK/transpose.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)     2252 2024-01-16 05:10:59.000000 BioSAK-1.87.1/BioSAK/usearch_uc.py
+-rw-r--r--   0 songweizhi   (501) staff       (20)      962 2024-04-17 08:12:49.000000 BioSAK-1.87.1/BioSAK/wilcox.py
+drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2024-05-02 15:48:05.231230 BioSAK-1.87.1/BioSAK.egg-info/
+-rw-r--r--   0 songweizhi   (501) staff       (20)      508 2024-05-02 15:48:05.000000 BioSAK-1.87.1/BioSAK.egg-info/PKG-INFO
+-rw-r--r--   0 songweizhi   (501) staff       (20)     3727 2024-05-02 15:48:05.000000 BioSAK-1.87.1/BioSAK.egg-info/SOURCES.txt
+-rw-r--r--   0 songweizhi   (501) staff       (20)        1 2024-05-02 15:48:05.000000 BioSAK-1.87.1/BioSAK.egg-info/dependency_links.txt
+-rw-r--r--   0 songweizhi   (501) staff       (20)       95 2024-05-02 15:48:05.000000 BioSAK-1.87.1/BioSAK.egg-info/requires.txt
+-rw-r--r--   0 songweizhi   (501) staff       (20)        7 2024-05-02 15:48:05.000000 BioSAK-1.87.1/BioSAK.egg-info/top_level.txt
+-rw-r--r--   0 songweizhi   (501) staff       (20)    35141 2023-05-09 01:09:36.000000 BioSAK-1.87.1/LICENSE
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)      300 2023-05-09 01:09:36.000000 BioSAK-1.87.1/MANIFEST.in
+-rw-r--r--   0 songweizhi   (501) staff       (20)      508 2024-05-02 15:48:05.231484 BioSAK-1.87.1/PKG-INFO
+-rw-r--r--   0 songweizhi   (501) staff       (20)     1533 2024-01-23 07:37:01.000000 BioSAK-1.87.1/README.md
+drwxr-xr-x   0 songweizhi   (501) staff       (20)        0 2024-05-02 15:48:05.231013 BioSAK-1.87.1/bin/
+-rwxr-xr-x   0 songweizhi   (501) staff       (20)    78071 2024-05-02 15:34:57.000000 BioSAK-1.87.1/bin/BioSAK
+-rw-r--r--   0 songweizhi   (501) staff       (20)       38 2024-05-02 15:48:05.231761 BioSAK-1.87.1/setup.cfg
+-rw-r--r--   0 songweizhi   (501) staff       (20)      915 2024-01-15 11:41:11.000000 BioSAK-1.87.1/setup.py
```

### Comparing `BioSAK-1.87.0/BioSAK/BLCA_op_parser.py` & `BioSAK-1.87.1/BioSAK/BLCA_op_parser.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/BioSAK_config.py` & `BioSAK-1.87.1/BioSAK/BioSAK_config.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/COG2020.py` & `BioSAK-1.87.1/BioSAK/COG2020.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/COG_boxplot_last1row.R` & `BioSAK-1.87.1/BioSAK/COG_boxplot_last1row.R`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/COG_boxplot_last2row.R` & `BioSAK-1.87.1/BioSAK/COG_boxplot_last2row.R`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/CheckM.py` & `BioSAK-1.87.1/BioSAK/CheckM.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/ConvertMSA.py` & `BioSAK-1.87.1/BioSAK/ConvertMSA.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/DnaFeaturesViewer.py` & `BioSAK-1.87.1/BioSAK/DnaFeaturesViewer.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/FastaSplitler_by_num.py` & `BioSAK-1.87.1/BioSAK/FastaSplitler_by_num.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/FastaSplitler_by_size.py` & `BioSAK-1.87.1/BioSAK/FastaSplitler_by_size.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/GTDB_for_BLCA.py` & `BioSAK-1.87.1/BioSAK/GTDB_for_BLCA.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/Gene2Ctg.py` & `BioSAK-1.87.1/BioSAK/Gene2Ctg.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/KEGG.py` & `BioSAK-1.87.1/BioSAK/KEGG.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/KEGG_boxplot_last1row.R` & `BioSAK-1.87.1/BioSAK/KEGG_boxplot_last1row.R`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/KeepRemovingTmp.py` & `BioSAK-1.87.1/BioSAK/KeepRemovingTmp.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/MeanMappingDepth.py` & `BioSAK-1.87.1/BioSAK/MeanMappingDepth.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/MetaBiosample.py` & `BioSAK-1.87.1/BioSAK/MetaBiosample.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/MetaCHIP_phylo.hmm` & `BioSAK-1.87.1/BioSAK/MetaCHIP_phylo.hmm`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/MetaCyc_reactions_with_ec.txt` & `BioSAK-1.87.1/BioSAK/MetaCyc_reactions_with_ec.txt`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/NetEnzymes.py` & `BioSAK-1.87.1/BioSAK/NetEnzymes.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/Newick_tree_plotter.py` & `BioSAK-1.87.1/BioSAK/Newick_tree_plotter.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/OneLineAln.py` & `BioSAK-1.87.1/BioSAK/OneLineAln.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/Prodigal.py` & `BioSAK-1.87.1/BioSAK/Prodigal.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/Reads_simulator.py` & `BioSAK-1.87.1/BioSAK/Reads_simulator.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/RunGraphMB.py` & `BioSAK-1.87.1/BioSAK/RunGraphMB.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/SILVA_for_BLCA.py` & `BioSAK-1.87.1/BioSAK/SILVA_for_BLCA.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/SankeyTaxon.py` & `BioSAK-1.87.1/BioSAK/SankeyTaxon.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/SliceMSA.py` & `BioSAK-1.87.1/BioSAK/SliceMSA.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/SubsampleLongReads.py` & `BioSAK-1.87.1/BioSAK/SubsampleLongReads.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/Tax4Fun2IndOTU.py` & `BioSAK-1.87.1/BioSAK/Tax4Fun2IndOTU.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/VERSION` & `BioSAK-1.87.1/BioSAK/VERSION`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
+1.87.1
+- fixed bugs
+
 1.87.0
 - new modules added: compare_sets
 
-1.86.4
-- fixed bugs
-
 1.86.0
 - new modules added: ribbon
 
 1.85.0
 - new modules added: wilcox and mannwhitneyu
 
 1.84.0
```

### Comparing `BioSAK-1.87.0/BioSAK/VisGeneFlk.py` & `BioSAK-1.87.1/BioSAK/VisGeneFlk.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/add_desc.py` & `BioSAK-1.87.1/BioSAK/add_desc.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/arCOG.py` & `BioSAK-1.87.1/BioSAK/arCOG.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/bam2reads.py` & `BioSAK-1.87.1/BioSAK/bam2reads.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/boxplot.py` & `BioSAK-1.87.1/BioSAK/boxplot.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/boxplot_last1row.R` & `BioSAK-1.87.1/BioSAK/boxplot_last1row.R`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/boxplot_matrix_COG.py` & `BioSAK-1.87.1/BioSAK/boxplot_matrix_COG.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/boxplot_matrix_COG_backup.py` & `BioSAK-1.87.1/BioSAK/boxplot_matrix_COG_backup.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/boxplot_matrix_KEGG.py` & `BioSAK-1.87.1/BioSAK/boxplot_matrix_KEGG.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/boxplot_matrix_dbCAN.py` & `BioSAK-1.87.1/BioSAK/boxplot_matrix_dbCAN.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/cat_fa.py` & `BioSAK-1.87.1/BioSAK/cat_fa.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/cdd2cog.pl` & `BioSAK-1.87.1/BioSAK/cdd2cog.pl`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/checkm_marker.py` & `BioSAK-1.87.1/BioSAK/checkm_marker.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/compare_sets.py` & `BioSAK-1.87.1/BioSAK/compare_sets.py`

 * *Files 12% similar despite different names*

```diff
@@ -35,17 +35,17 @@
     for e2 in set_2:
         if e2 not in shared_id_set:
             set_2_uniq.add(e2)
 
     if len(shared_id_set) == 0:
         print('No id shared between %s and %s' % (file_1, file_2))
     else:
-        print('Shared IDs\n%s\n' % '.'.join(shared_id_set))
-        print('IDs uniq to %s\n%s\n' % (file_1, '.'.join(sorted(list(set_1_uniq)))))
-        print('IDs uniq to %s\n%s\n' % (file_2, '.'.join(sorted(list(set_2_uniq)))))
+        print('Shared IDs (%s)\n%s\n' % (len(shared_id_set), '.'.join(shared_id_set)))
+        print('IDs uniq to %s (%s)\n%s\n' % (file_1, len(set_1_uniq), '.'.join(sorted(list(set_1_uniq)))))
+        print('IDs uniq to %s (%s)\n%s\n' % (file_2, len(set_2_uniq), '.'.join(sorted(list(set_2_uniq)))))
 
 
 if __name__ == '__main__':
 
     compare_sets_parser = argparse.ArgumentParser(usage=compare_sets_usage)
     compare_sets_parser.add_argument('-1', required=True, help='file 1')
     compare_sets_parser.add_argument('-2', required=True, help='file 2')
```

### Comparing `BioSAK-1.87.0/BioSAK/compare_trees.R` & `BioSAK-1.87.1/BioSAK/compare_trees.R`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/compare_trees.py` & `BioSAK-1.87.1/BioSAK/compare_trees.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/cross_link_seqs.py` & `BioSAK-1.87.1/BioSAK/cross_link_seqs.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/dbCAN.py` & `BioSAK-1.87.1/BioSAK/dbCAN.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/download_GenBank_genome_subset_prokaryotes_csv.py` & `BioSAK-1.87.1/BioSAK/download_GenBank_genome_subset_prokaryotes_csv.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/dwnld_sra_reads.py` & `BioSAK-1.87.1/BioSAK/dwnld_sra_reads.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/enrich.py` & `BioSAK-1.87.1/BioSAK/enrich.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/exe_cmds.py` & `BioSAK-1.87.1/BioSAK/exe_cmds.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/ezaai2mat.py` & `BioSAK-1.87.1/BioSAK/ezaai2mat.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/fa2id.py` & `BioSAK-1.87.1/BioSAK/fa2id.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/fa2phy.py` & `BioSAK-1.87.1/BioSAK/fa2phy.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/fa2tree.py` & `BioSAK-1.87.1/BioSAK/fa2tree.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/format_converter.py` & `BioSAK-1.87.1/BioSAK/format_converter.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/format_leaf_name.py` & `BioSAK-1.87.1/BioSAK/format_leaf_name.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/fq2fa.py` & `BioSAK-1.87.1/BioSAK/fq2fa.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/gapseq.py` & `BioSAK-1.87.1/BioSAK/gapseq.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/gbk2faa.py` & `BioSAK-1.87.1/BioSAK/gbk2faa.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/gbk2ffn.py` & `BioSAK-1.87.1/BioSAK/gbk2ffn.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/gbk2fna.py` & `BioSAK-1.87.1/BioSAK/gbk2fna.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/gbk2gff.py` & `BioSAK-1.87.1/BioSAK/gbk2gff.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/gbk_to_ffn_faa.py` & `BioSAK-1.87.1/BioSAK/gbk_to_ffn_faa.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/gc.py` & `BioSAK-1.87.1/BioSAK/gc.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/get_EC_from_ko_stats_D.py` & `BioSAK-1.87.1/BioSAK/get_EC_from_ko_stats_D.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/get_GTDB_taxon_gnm.py` & `BioSAK-1.87.1/BioSAK/get_GTDB_taxon_gnm.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/get_MAG_reads_long.py` & `BioSAK-1.87.1/BioSAK/get_MAG_reads_long.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/get_Pfam_hmms.py` & `BioSAK-1.87.1/BioSAK/get_Pfam_hmms.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/get_SCG_tree.py` & `BioSAK-1.87.1/BioSAK/get_SCG_tree.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/get_TopHits_taxonomy.py` & `BioSAK-1.87.1/BioSAK/get_TopHits_taxonomy.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/get_aa_composition.py` & `BioSAK-1.87.1/BioSAK/get_aa_composition.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/get_bin_abundance copy.py` & `BioSAK-1.87.1/BioSAK/get_bin_abundance copy.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/get_data_matrix.py` & `BioSAK-1.87.1/BioSAK/get_data_matrix.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/get_gene_depth.py` & `BioSAK-1.87.1/BioSAK/get_gene_depth.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/get_genome_GTDB.py` & `BioSAK-1.87.1/BioSAK/get_genome_GTDB.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/get_genome_NCBI.py` & `BioSAK-1.87.1/BioSAK/get_genome_NCBI.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/get_genome_NCBI_v1.py` & `BioSAK-1.87.1/BioSAK/get_genome_NCBI_v1.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/get_genome_NCBI_v2.py` & `BioSAK-1.87.1/BioSAK/get_genome_NCBI_v2.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/get_gnm_size.py` & `BioSAK-1.87.1/BioSAK/get_gnm_size.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/get_ko_gene_seqs.py` & `BioSAK-1.87.1/BioSAK/get_ko_gene_seqs.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/get_krona_plot.py` & `BioSAK-1.87.1/BioSAK/get_krona_plot.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/get_reads_from_sam.py` & `BioSAK-1.87.1/BioSAK/get_reads_from_sam.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/get_reads_id_in_sam.py` & `BioSAK-1.87.1/BioSAK/get_reads_id_in_sam.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/get_sankey_plot.R` & `BioSAK-1.87.1/BioSAK/get_sankey_plot.R`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/get_top_hit.py` & `BioSAK-1.87.1/BioSAK/get_top_hit.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/get_total_length.py` & `BioSAK-1.87.1/BioSAK/get_total_length.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/gff2chrom.py` & `BioSAK-1.87.1/BioSAK/gff2chrom.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/global_functions.py` & `BioSAK-1.87.1/BioSAK/global_functions.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/hpc3.py` & `BioSAK-1.87.1/BioSAK/hpc3.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/iTOL.py` & `BioSAK-1.87.1/BioSAK/iTOL.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/js_cmds.py` & `BioSAK-1.87.1/BioSAK/js_cmds.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/js_hpc3.py` & `BioSAK-1.87.1/BioSAK/js_hpc3.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/keep_best_hit.py` & `BioSAK-1.87.1/BioSAK/keep_best_hit.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/ko00001.keg` & `BioSAK-1.87.1/BioSAK/ko00001.keg`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/koala.py` & `BioSAK-1.87.1/BioSAK/koala.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/label_tree.R` & `BioSAK-1.87.1/BioSAK/label_tree.R`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/label_tree.py` & `BioSAK-1.87.1/BioSAK/label_tree.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/link_16S_MAG.py` & `BioSAK-1.87.1/BioSAK/link_16S_MAG.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/magabund.py` & `BioSAK-1.87.1/BioSAK/magabund.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/magabund2.py` & `BioSAK-1.87.1/BioSAK/magabund2.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/manipulator_fasta.py` & `BioSAK-1.87.1/BioSAK/manipulator_fasta.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/manipulator_newick.py` & `BioSAK-1.87.1/BioSAK/manipulator_newick.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/mannwhitneyu.py` & `BioSAK-1.87.1/BioSAK/mannwhitneyu.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/mean_MAG_cov.py` & `BioSAK-1.87.1/BioSAK/mean_MAG_cov.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/merge_df.py` & `BioSAK-1.87.1/BioSAK/merge_df.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/merge_seq.py` & `BioSAK-1.87.1/BioSAK/merge_seq.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/metaAssembly.py` & `BioSAK-1.87.1/BioSAK/metaAssembly.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/metabat2concoct.py` & `BioSAK-1.87.1/BioSAK/metabat2concoct.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/metabat2maxbin.py` & `BioSAK-1.87.1/BioSAK/metabat2maxbin.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/ncbi_dataset.py` & `BioSAK-1.87.1/BioSAK/ncbi_dataset.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/parse_MetaCyc_RxnDB.py` & `BioSAK-1.87.1/BioSAK/parse_MetaCyc_RxnDB.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/parse_mmseqs_tsv.py` & `BioSAK-1.87.1/BioSAK/parse_mmseqs_tsv.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/plot_mag.py` & `BioSAK-1.87.1/BioSAK/plot_mag.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/plot_sam_depth.py` & `BioSAK-1.87.1/BioSAK/plot_sam_depth.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/plot_tree.R` & `BioSAK-1.87.1/BioSAK/plot_tree.R`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/prefix_file.py` & `BioSAK-1.87.1/BioSAK/prefix_file.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/prokka.py` & `BioSAK-1.87.1/BioSAK/prokka.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/reads2bam.py` & `BioSAK-1.87.1/BioSAK/reads2bam.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/rename_leaves.py` & `BioSAK-1.87.1/BioSAK/rename_leaves.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/rename_reads_for_Reago.py` & `BioSAK-1.87.1/BioSAK/rename_reads_for_Reago.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/rename_seq.py` & `BioSAK-1.87.1/BioSAK/rename_seq.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/rename_seqs.py` & `BioSAK-1.87.1/BioSAK/rename_seqs.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/ribbon.py` & `BioSAK-1.87.1/BioSAK/ribbon.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/sam2bam.py` & `BioSAK-1.87.1/BioSAK/sam2bam.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/sampling_GTDB_gnms.py` & `BioSAK-1.87.1/BioSAK/sampling_GTDB_gnms.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/select_seq.py` & `BioSAK-1.87.1/BioSAK/select_seq.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/sep_reads_by_barcode.py` & `BioSAK-1.87.1/BioSAK/sep_reads_by_barcode.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/slice_seq.py` & `BioSAK-1.87.1/BioSAK/slice_seq.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/split_fasta.py` & `BioSAK-1.87.1/BioSAK/split_fasta.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/split_folder.py` & `BioSAK-1.87.1/BioSAK/split_folder.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/split_sam.py` & `BioSAK-1.87.1/BioSAK/split_sam.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/submitHPC.py` & `BioSAK-1.87.1/BioSAK/submitHPC.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/subset_GTDB_meta.py` & `BioSAK-1.87.1/BioSAK/subset_GTDB_meta.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/subset_df.py` & `BioSAK-1.87.1/BioSAK/subset_df.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/subset_tree.py` & `BioSAK-1.87.1/BioSAK/subset_tree.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/top_16S_hits.py` & `BioSAK-1.87.1/BioSAK/top_16S_hits.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/top_hits_in_a_group.py` & `BioSAK-1.87.1/BioSAK/top_hits_in_a_group.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/transpose.py` & `BioSAK-1.87.1/BioSAK/transpose.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/usearch_uc.py` & `BioSAK-1.87.1/BioSAK/usearch_uc.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK/wilcox.py` & `BioSAK-1.87.1/BioSAK/wilcox.py`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/BioSAK.egg-info/SOURCES.txt` & `BioSAK-1.87.1/BioSAK.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/LICENSE` & `BioSAK-1.87.1/LICENSE`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/README.md` & `BioSAK-1.87.1/README.md`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/bin/BioSAK` & `BioSAK-1.87.1/bin/BioSAK`

 * *Files identical despite different names*

### Comparing `BioSAK-1.87.0/setup.py` & `BioSAK-1.87.1/setup.py`

 * *Files identical despite different names*

