# Comparing `tmp/trimnami-0.1.3.tar.gz` & `tmp/trimnami-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trimnami-0.1.3.tar", last modified: Thu Feb  8 02:54:18 2024, max compression
+gzip compressed data, was "trimnami-0.1.4.tar", last modified: Thu May  2 06:23:15 2024, max compression
```

## Comparing `trimnami-0.1.3.tar` & `trimnami-0.1.4.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 02:54:18.030753 trimnami-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-02-08 02:54:07.000000 trimnami-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7247 2024-02-08 02:54:18.030753 trimnami-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-02-08 02:54:07.000000 trimnami-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-08 02:54:18.030753 trimnami-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-02-08 02:54:07.000000 trimnami-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 02:54:18.010753 trimnami-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-02-08 02:54:07.000000 trimnami-0.1.3/tests/test_copyOrGzip.py
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-02-08 02:54:07.000000 trimnami-0.1.3/tests/test_trimnami.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 02:54:18.010753 trimnami-0.1.3/trimnami/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 02:54:07.000000 trimnami-0.1.3/trimnami/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9480 2024-02-08 02:54:07.000000 trimnami-0.1.3/trimnami/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 02:54:18.010753 trimnami-0.1.3/trimnami/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-02-08 02:54:07.000000 trimnami-0.1.3/trimnami/config/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 02:54:18.010753 trimnami-0.1.3/trimnami/config/profile/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-02-08 02:54:07.000000 trimnami-0.1.3/trimnami/config/profile/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-02-08 02:54:07.000000 trimnami-0.1.3/trimnami/config/system_config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 02:54:18.010753 trimnami-0.1.3/trimnami/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-08 02:54:07.000000 trimnami-0.1.3/trimnami/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-02-08 02:54:07.000000 trimnami-0.1.3/trimnami/scripts/copyOrGzip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 02:54:18.018753 trimnami-0.1.3/trimnami/test_data/
--rw-r--r--   0 runner    (1001) docker     (127)   950550 2024-02-08 02:54:07.000000 trimnami-0.1.3/trimnami/test_data/A13-04-182-06_TAGCTT_R1.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (127)  1016766 2024-02-08 02:54:07.000000 trimnami-0.1.3/trimnami/test_data/A13-04-182-06_TAGCTT_R2.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (127)  1018716 2024-02-08 02:54:07.000000 trimnami-0.1.3/trimnami/test_data/A13-12-250-06_GGCTAC_R1_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (127)  1019116 2024-02-08 02:54:07.000000 trimnami-0.1.3/trimnami/test_data/A13-12-250-06_GGCTAC_R2_001.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (127)  1418720 2024-02-08 02:54:07.000000 trimnami-0.1.3/trimnami/test_data/A13-135-177-06_AGTTCC.fastq
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 02:54:18.022753 trimnami-0.1.3/trimnami/test_data/nanopore/
--rw-r--r--   0 runner    (1001) docker     (127)   350434 2024-02-08 02:54:07.000000 trimnami-0.1.3/trimnami/test_data/nanopore/SRR7947171.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (127)   840483 2024-02-08 02:54:07.000000 trimnami-0.1.3/trimnami/test_data/nanopore/SRR7947176.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (127)  1942970 2024-02-08 02:54:07.000000 trimnami-0.1.3/trimnami/test_data/ref.fna
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-02-08 02:54:07.000000 trimnami-0.1.3/trimnami/trimnami.CITATION
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-02-08 02:54:07.000000 trimnami-0.1.3/trimnami/trimnami.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-08 02:54:07.000000 trimnami-0.1.3/trimnami/trimnami.VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 02:54:18.022753 trimnami-0.1.3/trimnami/workflow/
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-02-08 02:54:07.000000 trimnami-0.1.3/trimnami/workflow/Snakefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 02:54:18.026753 trimnami-0.1.3/trimnami/workflow/databases/
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-02-08 02:54:07.000000 trimnami-0.1.3/trimnami/workflow/databases/IlluminaAdapters.fa
--rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-02-08 02:54:07.000000 trimnami-0.1.3/trimnami/workflow/databases/nebnext_adapters.fa
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-02-08 02:54:07.000000 trimnami-0.1.3/trimnami/workflow/databases/primerB.fa
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-02-08 02:54:07.000000 trimnami-0.1.3/trimnami/workflow/databases/rc_primerB_ad6.fa
--rw-r--r--   0 runner    (1001) docker     (127)   911854 2024-02-08 02:54:07.000000 trimnami-0.1.3/trimnami/workflow/databases/vector_contaminants.fa
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 02:54:18.026753 trimnami-0.1.3/trimnami/workflow/envs/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-02-08 02:54:07.000000 trimnami-0.1.3/trimnami/workflow/envs/bbmap.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-02-08 02:54:07.000000 trimnami-0.1.3/trimnami/workflow/envs/cutadapt.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-02-08 02:54:07.000000 trimnami-0.1.3/trimnami/workflow/envs/fastp.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-02-08 02:54:07.000000 trimnami-0.1.3/trimnami/workflow/envs/fastqc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-02-08 02:54:07.000000 trimnami-0.1.3/trimnami/workflow/envs/filtlong.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-02-08 02:54:07.000000 trimnami-0.1.3/trimnami/workflow/envs/minimap2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-02-08 02:54:07.000000 trimnami-0.1.3/trimnami/workflow/envs/multiqc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-02-08 02:54:07.000000 trimnami-0.1.3/trimnami/workflow/envs/pigz.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-02-08 02:54:07.000000 trimnami-0.1.3/trimnami/workflow/envs/prinseq.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-02-08 02:54:07.000000 trimnami-0.1.3/trimnami/workflow/envs/rasusa.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-08 02:54:07.000000 trimnami-0.1.3/trimnami/workflow/envs/seqtk.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 02:54:18.030753 trimnami-0.1.3/trimnami/workflow/rules/
--rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-02-08 02:54:07.000000 trimnami-0.1.3/trimnami/workflow/rules/cutadapt.smk
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-02-08 02:54:07.000000 trimnami-0.1.3/trimnami/workflow/rules/fasta.smk
--rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-02-08 02:54:07.000000 trimnami-0.1.3/trimnami/workflow/rules/fastp.smk
--rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-02-08 02:54:07.000000 trimnami-0.1.3/trimnami/workflow/rules/fastqc.smk
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-02-08 02:54:07.000000 trimnami-0.1.3/trimnami/workflow/rules/filtlong.smk
--rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-02-08 02:54:07.000000 trimnami-0.1.3/trimnami/workflow/rules/hostRemoval.smk
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-02-08 02:54:07.000000 trimnami-0.1.3/trimnami/workflow/rules/notrim.smk
--rw-r--r--   0 runner    (1001) docker     (127)     4961 2024-02-08 02:54:07.000000 trimnami-0.1.3/trimnami/workflow/rules/preflight.smk
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-02-08 02:54:07.000000 trimnami-0.1.3/trimnami/workflow/rules/prinseq.smk
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-02-08 02:54:07.000000 trimnami-0.1.3/trimnami/workflow/rules/rasusa.smk
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-02-08 02:54:07.000000 trimnami-0.1.3/trimnami/workflow/rules/reports.smk
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-02-08 02:54:07.000000 trimnami-0.1.3/trimnami/workflow/rules/results.smk
--rw-r--r--   0 runner    (1001) docker     (127)    13472 2024-02-08 02:54:07.000000 trimnami-0.1.3/trimnami/workflow/rules/roundAB.smk
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 02:54:18.030753 trimnami-0.1.3/trimnami.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7247 2024-02-08 02:54:17.000000 trimnami-0.1.3/trimnami.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-02-08 02:54:18.000000 trimnami-0.1.3/trimnami.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-08 02:54:17.000000 trimnami-0.1.3/trimnami.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-08 02:54:17.000000 trimnami-0.1.3/trimnami.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-02-08 02:54:17.000000 trimnami-0.1.3/trimnami.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-08 02:54:17.000000 trimnami-0.1.3/trimnami.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:23:15.812973 trimnami-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-02 06:23:08.000000 trimnami-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7247 2024-05-02 06:23:15.812973 trimnami-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-05-02 06:23:08.000000 trimnami-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 06:23:15.812973 trimnami-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-02 06:23:08.000000 trimnami-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:23:15.792973 trimnami-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-02 06:23:08.000000 trimnami-0.1.4/tests/test_copyOrGzip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-02 06:23:08.000000 trimnami-0.1.4/tests/test_trimnami.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:23:15.792973 trimnami-0.1.4/trimnami/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 06:23:08.000000 trimnami-0.1.4/trimnami/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9480 2024-05-02 06:23:08.000000 trimnami-0.1.4/trimnami/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:23:15.792973 trimnami-0.1.4/trimnami/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-02 06:23:08.000000 trimnami-0.1.4/trimnami/config/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:23:15.792973 trimnami-0.1.4/trimnami/config/profile/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-02 06:23:08.000000 trimnami-0.1.4/trimnami/config/profile/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-02 06:23:08.000000 trimnami-0.1.4/trimnami/config/system_config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:23:15.792973 trimnami-0.1.4/trimnami/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 06:23:08.000000 trimnami-0.1.4/trimnami/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-02 06:23:08.000000 trimnami-0.1.4/trimnami/scripts/copyOrGzip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:23:15.800973 trimnami-0.1.4/trimnami/test_data/
+-rw-r--r--   0 runner    (1001) docker     (127)   950550 2024-05-02 06:23:08.000000 trimnami-0.1.4/trimnami/test_data/A13-04-182-06_TAGCTT_R1.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (127)  1016766 2024-05-02 06:23:08.000000 trimnami-0.1.4/trimnami/test_data/A13-04-182-06_TAGCTT_R2.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (127)  1018716 2024-05-02 06:23:08.000000 trimnami-0.1.4/trimnami/test_data/A13-12-250-06_GGCTAC_R1_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (127)  1019116 2024-05-02 06:23:08.000000 trimnami-0.1.4/trimnami/test_data/A13-12-250-06_GGCTAC_R2_001.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (127)  1418720 2024-05-02 06:23:08.000000 trimnami-0.1.4/trimnami/test_data/A13-135-177-06_AGTTCC.fastq
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:23:15.804973 trimnami-0.1.4/trimnami/test_data/nanopore/
+-rw-r--r--   0 runner    (1001) docker     (127)   350434 2024-05-02 06:23:08.000000 trimnami-0.1.4/trimnami/test_data/nanopore/SRR7947171.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   840483 2024-05-02 06:23:08.000000 trimnami-0.1.4/trimnami/test_data/nanopore/SRR7947176.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (127)  1942970 2024-05-02 06:23:08.000000 trimnami-0.1.4/trimnami/test_data/ref.fna
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-02 06:23:08.000000 trimnami-0.1.4/trimnami/trimnami.CITATION
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-02 06:23:08.000000 trimnami-0.1.4/trimnami/trimnami.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-02 06:23:08.000000 trimnami-0.1.4/trimnami/trimnami.VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:23:15.804973 trimnami-0.1.4/trimnami/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-02 06:23:08.000000 trimnami-0.1.4/trimnami/workflow/Snakefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:23:15.804973 trimnami-0.1.4/trimnami/workflow/databases/
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-02 06:23:08.000000 trimnami-0.1.4/trimnami/workflow/databases/IlluminaAdapters.fa
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-05-02 06:23:08.000000 trimnami-0.1.4/trimnami/workflow/databases/nebnext_adapters.fa
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-02 06:23:08.000000 trimnami-0.1.4/trimnami/workflow/databases/primerB.fa
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-02 06:23:08.000000 trimnami-0.1.4/trimnami/workflow/databases/rc_primerB_ad6.fa
+-rw-r--r--   0 runner    (1001) docker     (127)   911854 2024-05-02 06:23:08.000000 trimnami-0.1.4/trimnami/workflow/databases/vector_contaminants.fa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:23:15.808973 trimnami-0.1.4/trimnami/workflow/envs/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-02 06:23:08.000000 trimnami-0.1.4/trimnami/workflow/envs/bbmap.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-02 06:23:08.000000 trimnami-0.1.4/trimnami/workflow/envs/cutadapt.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-02 06:23:08.000000 trimnami-0.1.4/trimnami/workflow/envs/fastp.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-02 06:23:08.000000 trimnami-0.1.4/trimnami/workflow/envs/fastqc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-02 06:23:08.000000 trimnami-0.1.4/trimnami/workflow/envs/filtlong.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-02 06:23:08.000000 trimnami-0.1.4/trimnami/workflow/envs/minimap2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-02 06:23:08.000000 trimnami-0.1.4/trimnami/workflow/envs/multiqc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-02 06:23:08.000000 trimnami-0.1.4/trimnami/workflow/envs/pigz.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-02 06:23:08.000000 trimnami-0.1.4/trimnami/workflow/envs/prinseq.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-02 06:23:08.000000 trimnami-0.1.4/trimnami/workflow/envs/rasusa.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-02 06:23:08.000000 trimnami-0.1.4/trimnami/workflow/envs/seqtk.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:23:15.812973 trimnami-0.1.4/trimnami/workflow/rules/
+-rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-05-02 06:23:08.000000 trimnami-0.1.4/trimnami/workflow/rules/cutadapt.smk
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-02 06:23:08.000000 trimnami-0.1.4/trimnami/workflow/rules/fasta.smk
+-rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-05-02 06:23:08.000000 trimnami-0.1.4/trimnami/workflow/rules/fastp.smk
+-rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-05-02 06:23:08.000000 trimnami-0.1.4/trimnami/workflow/rules/fastqc.smk
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-02 06:23:08.000000 trimnami-0.1.4/trimnami/workflow/rules/filtlong.smk
+-rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-05-02 06:23:08.000000 trimnami-0.1.4/trimnami/workflow/rules/hostRemoval.smk
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-02 06:23:08.000000 trimnami-0.1.4/trimnami/workflow/rules/notrim.smk
+-rw-r--r--   0 runner    (1001) docker     (127)     4961 2024-05-02 06:23:08.000000 trimnami-0.1.4/trimnami/workflow/rules/preflight.smk
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-05-02 06:23:08.000000 trimnami-0.1.4/trimnami/workflow/rules/prinseq.smk
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-02 06:23:08.000000 trimnami-0.1.4/trimnami/workflow/rules/rasusa.smk
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-02 06:23:08.000000 trimnami-0.1.4/trimnami/workflow/rules/reports.smk
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-02 06:23:08.000000 trimnami-0.1.4/trimnami/workflow/rules/results.smk
+-rw-r--r--   0 runner    (1001) docker     (127)    13472 2024-05-02 06:23:08.000000 trimnami-0.1.4/trimnami/workflow/rules/roundAB.smk
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:23:15.812973 trimnami-0.1.4/trimnami.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7247 2024-05-02 06:23:15.000000 trimnami-0.1.4/trimnami.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-05-02 06:23:15.000000 trimnami-0.1.4/trimnami.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 06:23:15.000000 trimnami-0.1.4/trimnami.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-02 06:23:15.000000 trimnami-0.1.4/trimnami.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-02 06:23:15.000000 trimnami-0.1.4/trimnami.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-02 06:23:15.000000 trimnami-0.1.4/trimnami.egg-info/top_level.txt
```

### Comparing `trimnami-0.1.3/PKG-INFO` & `trimnami-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trimnami
-Version: 0.1.3
+Version: 0.1.4
 Summary: Trim lots of metagenomics samples all at once.
 Home-page: https://github.com/beardymcjohnface/Trimnami
 Author: Michael Roach
 Author-email: beardymcjohnface@gmail.com
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: snaketool-utils>=0.0.5
```

### Comparing `trimnami-0.1.3/README.md` & `trimnami-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `trimnami-0.1.3/setup.py` & `trimnami-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `trimnami-0.1.3/tests/test_copyOrGzip.py` & `trimnami-0.1.4/tests/test_copyOrGzip.py`

 * *Files identical despite different names*

### Comparing `trimnami-0.1.3/tests/test_trimnami.py` & `trimnami-0.1.4/tests/test_trimnami.py`

 * *Files identical despite different names*

### Comparing `trimnami-0.1.3/trimnami/__main__.py` & `trimnami-0.1.4/trimnami/__main__.py`

 * *Files identical despite different names*

### Comparing `trimnami-0.1.3/trimnami/config/config.yaml` & `trimnami-0.1.4/trimnami/config/config.yaml`

 * *Files identical despite different names*

### Comparing `trimnami-0.1.3/trimnami/config/system_config.yaml` & `trimnami-0.1.4/trimnami/config/system_config.yaml`

 * *Files identical despite different names*

### Comparing `trimnami-0.1.3/trimnami/scripts/copyOrGzip.py` & `trimnami-0.1.4/trimnami/scripts/copyOrGzip.py`

 * *Files identical despite different names*

### Comparing `trimnami-0.1.3/trimnami/test_data/A13-04-182-06_TAGCTT_R1.fastq.gz` & `trimnami-0.1.4/trimnami/test_data/A13-04-182-06_TAGCTT_R1.fastq.gz`

 * *Files identical despite different names*

### Comparing `trimnami-0.1.3/trimnami/test_data/A13-04-182-06_TAGCTT_R2.fastq.gz` & `trimnami-0.1.4/trimnami/test_data/A13-04-182-06_TAGCTT_R2.fastq.gz`

 * *Files identical despite different names*

### Comparing `trimnami-0.1.3/trimnami/test_data/A13-12-250-06_GGCTAC_R1_001.fastq.gz` & `trimnami-0.1.4/trimnami/test_data/A13-12-250-06_GGCTAC_R1_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `trimnami-0.1.3/trimnami/test_data/A13-12-250-06_GGCTAC_R2_001.fastq.gz` & `trimnami-0.1.4/trimnami/test_data/A13-12-250-06_GGCTAC_R2_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `trimnami-0.1.3/trimnami/test_data/A13-135-177-06_AGTTCC.fastq` & `trimnami-0.1.4/trimnami/test_data/A13-135-177-06_AGTTCC.fastq`

 * *Files identical despite different names*

### Comparing `trimnami-0.1.3/trimnami/test_data/nanopore/SRR7947171.fastq.gz` & `trimnami-0.1.4/trimnami/test_data/nanopore/SRR7947171.fastq.gz`

 * *Files identical despite different names*

### Comparing `trimnami-0.1.3/trimnami/test_data/nanopore/SRR7947176.fastq.gz` & `trimnami-0.1.4/trimnami/test_data/nanopore/SRR7947176.fastq.gz`

 * *Files identical despite different names*

### Comparing `trimnami-0.1.3/trimnami/test_data/ref.fna` & `trimnami-0.1.4/trimnami/test_data/ref.fna`

 * *Files identical despite different names*

### Comparing `trimnami-0.1.3/trimnami/trimnami.LICENSE` & `trimnami-0.1.4/trimnami/trimnami.LICENSE`

 * *Files identical despite different names*

### Comparing `trimnami-0.1.3/trimnami/workflow/Snakefile` & `trimnami-0.1.4/trimnami/workflow/Snakefile`

 * *Files identical despite different names*

### Comparing `trimnami-0.1.3/trimnami/workflow/databases/IlluminaAdapters.fa` & `trimnami-0.1.4/trimnami/workflow/databases/IlluminaAdapters.fa`

 * *Files identical despite different names*

### Comparing `trimnami-0.1.3/trimnami/workflow/databases/nebnext_adapters.fa` & `trimnami-0.1.4/trimnami/workflow/databases/nebnext_adapters.fa`

 * *Files identical despite different names*

### Comparing `trimnami-0.1.3/trimnami/workflow/databases/primerB.fa` & `trimnami-0.1.4/trimnami/workflow/databases/primerB.fa`

 * *Files identical despite different names*

### Comparing `trimnami-0.1.3/trimnami/workflow/databases/rc_primerB_ad6.fa` & `trimnami-0.1.4/trimnami/workflow/databases/rc_primerB_ad6.fa`

 * *Files identical despite different names*

### Comparing `trimnami-0.1.3/trimnami/workflow/databases/vector_contaminants.fa` & `trimnami-0.1.4/trimnami/workflow/databases/vector_contaminants.fa`

 * *Files identical despite different names*

### Comparing `trimnami-0.1.3/trimnami/workflow/rules/cutadapt.smk` & `trimnami-0.1.4/trimnami/workflow/rules/cutadapt.smk`

 * *Files identical despite different names*

### Comparing `trimnami-0.1.3/trimnami/workflow/rules/fastp.smk` & `trimnami-0.1.4/trimnami/workflow/rules/fastp.smk`

 * *Files identical despite different names*

### Comparing `trimnami-0.1.3/trimnami/workflow/rules/fastqc.smk` & `trimnami-0.1.4/trimnami/workflow/rules/fastqc.smk`

 * *Files identical despite different names*

### Comparing `trimnami-0.1.3/trimnami/workflow/rules/filtlong.smk` & `trimnami-0.1.4/trimnami/workflow/rules/filtlong.smk`

 * *Files identical despite different names*

### Comparing `trimnami-0.1.3/trimnami/workflow/rules/hostRemoval.smk` & `trimnami-0.1.4/trimnami/workflow/rules/hostRemoval.smk`

 * *Files identical despite different names*

### Comparing `trimnami-0.1.3/trimnami/workflow/rules/notrim.smk` & `trimnami-0.1.4/trimnami/workflow/rules/notrim.smk`

 * *Files identical despite different names*

### Comparing `trimnami-0.1.3/trimnami/workflow/rules/preflight.smk` & `trimnami-0.1.4/trimnami/workflow/rules/preflight.smk`

 * *Files identical despite different names*

### Comparing `trimnami-0.1.3/trimnami/workflow/rules/prinseq.smk` & `trimnami-0.1.4/trimnami/workflow/rules/prinseq.smk`

 * *Files identical despite different names*

### Comparing `trimnami-0.1.3/trimnami/workflow/rules/rasusa.smk` & `trimnami-0.1.4/trimnami/workflow/rules/rasusa.smk`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,16 @@
         config["qc"]["subsample"]
     benchmark:
         os.path.join(dir["bench"], "rasusa_single.{dir}.{file}.txt")
     log:
         os.path.join(dir["log"], "rasusa_single.{dir}.{file}.log")
     shell:
         ("if (( $(wc -c {input} | awk '{{print$1}}') > 200 ))\n then "
-            "rasusa "
-                "-i {input} "
+            "rasusa reads "
                 "-o {output} "
                 "-O g "
                 "{params} "
+                "{input} "
                 "2> {log}\n "
          "else "
             "touch {output}\n "
          "fi\n\n ")
```

### Comparing `trimnami-0.1.3/trimnami/workflow/rules/reports.smk` & `trimnami-0.1.4/trimnami/workflow/rules/reports.smk`

 * *Files identical despite different names*

### Comparing `trimnami-0.1.3/trimnami/workflow/rules/roundAB.smk` & `trimnami-0.1.4/trimnami/workflow/rules/roundAB.smk`

 * *Files identical despite different names*

### Comparing `trimnami-0.1.3/trimnami.egg-info/PKG-INFO` & `trimnami-0.1.4/trimnami.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trimnami
-Version: 0.1.3
+Version: 0.1.4
 Summary: Trim lots of metagenomics samples all at once.
 Home-page: https://github.com/beardymcjohnface/Trimnami
 Author: Michael Roach
 Author-email: beardymcjohnface@gmail.com
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: snaketool-utils>=0.0.5
```

### Comparing `trimnami-0.1.3/trimnami.egg-info/SOURCES.txt` & `trimnami-0.1.4/trimnami.egg-info/SOURCES.txt`

 * *Files identical despite different names*

