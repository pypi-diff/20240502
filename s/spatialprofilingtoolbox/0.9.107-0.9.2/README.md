# Comparing `tmp/spatialprofilingtoolbox-0.9.107.tar.gz` & `tmp/spatialprofilingtoolbox-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spatialprofilingtoolbox-0.9.107.tar", last modified: Fri Apr 15 21:19:48 2022, max compression
+gzip compressed data, was "spatialprofilingtoolbox-0.9.2.tar", last modified: Fri Mar 18 16:55:03 2022, max compression
```

## Comparing `spatialprofilingtoolbox-0.9.107.tar` & `spatialprofilingtoolbox-0.9.2.tar`

### file list

```diff
@@ -1,108 +1,97 @@
-drwxr-xr-x   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)        0 2022-04-15 21:19:48.077950 spatialprofilingtoolbox-0.9.107/
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)      950 2021-08-09 23:10:18.000000 spatialprofilingtoolbox-0.9.107/LICENSE.md
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)      836 2022-04-15 21:19:48.077697 spatialprofilingtoolbox-0.9.107/PKG-INFO
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)    12279 2022-04-07 21:57:54.000000 spatialprofilingtoolbox-0.9.107/README.md
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)      104 2021-08-09 23:10:18.000000 spatialprofilingtoolbox-0.9.107/pyproject.toml
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)       38 2022-04-15 21:19:48.078042 spatialprofilingtoolbox-0.9.107/setup.cfg
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     3408 2022-04-07 19:59:46.000000 spatialprofilingtoolbox-0.9.107/setup.py
-drwxr-xr-x   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)        0 2022-04-15 21:19:48.039507 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     3848 2022-04-08 18:36:26.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/__init__.py
-drwxr-xr-x   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)        0 2022-04-15 21:19:48.040885 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/applications/
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)      174 2021-08-09 23:10:18.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/applications/__init__.py
-drwxr-xr-x   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)        0 2022-04-15 21:19:48.042727 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/applications/cell_cartoons/
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)      391 2021-08-09 23:10:18.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/applications/cell_cartoons/__init__.py
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)      673 2021-08-09 23:10:18.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/applications/cell_cartoons/application.py
-drwxr-xr-x   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)        0 2022-04-15 21:19:48.044131 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/applications/configuration_ui/
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)       84 2021-11-15 05:46:02.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/applications/configuration_ui/__init__.py
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     7921 2022-04-07 19:59:46.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/applications/configuration_ui/ui.py
-drwxr-xr-x   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)        0 2022-04-15 21:19:48.045128 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/applications/diffusion_graphs_viz/
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)      143 2021-08-09 23:10:18.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/applications/diffusion_graphs_viz/__init__.py
--rwxr-xr-x   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     6785 2021-08-09 23:10:18.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/applications/diffusion_graphs_viz/diffusion_graphs_viz.py
-drwxr-xr-x   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)        0 2022-04-15 21:19:48.046022 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/applications/diffusion_tests_viz/
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)      171 2021-08-09 23:10:18.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/applications/diffusion_tests_viz/__init__.py
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)    11629 2021-09-17 21:18:07.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/applications/diffusion_tests_viz/diffusion_tests_viz.py
-drwxr-xr-x   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)        0 2022-04-15 21:19:48.047018 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/applications/front_proximity_viz/
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)      156 2021-08-09 23:10:18.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/applications/front_proximity_viz/__init__.py
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)    11479 2021-08-09 23:10:18.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/applications/front_proximity_viz/front_proximity_viz.py
-drwxr-xr-x   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)        0 2022-04-15 21:19:48.047650 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/dataset_designs/
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)      196 2021-08-09 23:10:18.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/dataset_designs/__init__.py
-drwxr-xr-x   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)        0 2022-04-15 21:19:48.049934 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/dataset_designs/multiplexed_imaging/
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)      776 2021-08-09 23:10:18.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/dataset_designs/multiplexed_imaging/__init__.py
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)    15729 2022-04-15 20:32:23.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/dataset_designs/multiplexed_imaging/halo_cell_metadata_design.py
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)    13119 2021-11-15 05:46:02.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/dataset_designs/multiplexed_imaging/halo_cell_metadata_provider.py
-drwxr-xr-x   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)        0 2022-04-15 21:19:48.058406 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/environment/
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)      254 2021-08-09 23:10:18.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/environment/__init__.py
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     2533 2022-04-07 19:59:46.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/environment/calculator.py
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     5570 2021-09-17 21:18:07.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/environment/cell_metadata.py
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     1620 2021-11-15 05:46:02.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/environment/computational_design.py
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     2537 2022-04-15 18:57:33.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/environment/configuration.py
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)      708 2022-04-07 19:59:46.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/environment/configuration_settings.py
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     2830 2021-09-17 21:18:07.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/environment/database_context_utility.py
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     3115 2021-11-15 05:46:02.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/environment/dichotomization.py
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     1419 2022-04-15 20:45:48.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/environment/extract_compartments.py
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     3699 2022-04-15 18:35:07.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/environment/file_io.py
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     6007 2022-04-15 19:49:41.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/environment/job_generator.py
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     2473 2022-04-07 19:59:46.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/environment/log_formats.py
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     2500 2022-04-07 19:59:46.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/environment/performance_timer.py
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)      631 2022-04-15 18:11:25.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/environment/settings_wrappers.py
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     3240 2021-11-15 05:46:02.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/environment/single_job_analyzer.py
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     4147 2022-04-07 19:59:46.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/environment/skimmer.py
-drwxr-xr-x   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)        0 2022-04-15 21:19:48.060899 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/environment/source_file_parsers/
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)      212 2022-04-07 19:59:46.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/environment/source_file_parsers/__init__.py
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)    12886 2022-04-07 19:59:46.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/environment/source_file_parsers/cellmanifests.py
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     5403 2022-04-07 19:59:46.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/environment/source_file_parsers/cellmanifestset.py
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     7268 2022-04-07 19:59:46.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/environment/source_file_parsers/channels.py
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     1893 2022-04-07 19:59:46.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/environment/source_file_parsers/outcomes.py
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     3795 2022-04-07 19:59:46.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/environment/source_file_parsers/parser.py
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)      461 2021-11-15 05:46:02.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/environment/workflow_modules.py
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     8316 2022-04-07 19:59:46.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/fields.tsv
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)      355 2022-04-07 19:59:46.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/nextflow.config.local
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)      419 2022-04-15 20:48:14.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/nextflow.config.lsf
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     4999 2022-04-07 19:59:46.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/pathology_schema.sql
-drwxr-xr-x   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)        0 2022-04-15 21:19:48.063895 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/scripts/
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     1843 2021-11-15 05:46:02.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/scripts/spt-aggregate-cell-data
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     1249 2022-04-07 19:59:46.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/scripts/spt-diffusion-graphs-viz
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)      771 2022-04-07 19:59:46.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/scripts/spt-diffusion-viz
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)      889 2022-04-07 19:59:46.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/scripts/spt-front-proximity-viz
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     2437 2021-11-15 05:46:02.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/scripts/spt-merge-sqlite-dbs
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     5664 2022-04-15 19:02:13.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/scripts/spt-pipeline
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)      877 2022-04-07 19:59:46.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/scripts/spt-print
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     5174 2022-04-15 20:44:22.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/spt_pipeline.nf
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)        7 2022-04-15 21:19:40.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/version.txt
-drwxr-xr-x   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)        0 2022-04-15 21:19:48.064464 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/workflows/
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)      874 2021-08-09 23:10:18.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/workflows/__init__.py
-drwxr-xr-x   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)        0 2022-04-15 21:19:48.068472 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/workflows/density/
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)      752 2021-11-15 05:46:02.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/workflows/density/__init__.py
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     2609 2022-04-15 18:36:51.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/workflows/density/analyzer.py
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     5970 2022-04-07 19:59:46.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/workflows/density/computational_design.py
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)    11261 2022-04-14 20:16:26.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/workflows/density/core.py
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     4842 2022-04-07 19:59:46.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/workflows/density/data_logging.py
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)    22951 2022-04-14 20:30:25.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/workflows/density/integrator.py
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)      548 2022-04-07 19:59:46.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/workflows/density/job_generator.py
-drwxr-xr-x   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)        0 2022-04-15 21:19:48.071534 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/workflows/diffusion/
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     1072 2021-11-15 05:46:02.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/workflows/diffusion/__init__.py
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     7446 2021-11-15 05:46:02.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/workflows/diffusion/analyzer.py
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     2891 2021-11-15 05:46:02.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/workflows/diffusion/computational_design.py
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)    14889 2021-11-15 05:46:02.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/workflows/diffusion/core.py
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)    20856 2021-11-15 05:46:02.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/workflows/diffusion/integrator.py
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)      412 2021-11-15 05:46:02.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/workflows/diffusion/job_generator.py
-drwxr-xr-x   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)        0 2022-04-15 21:19:48.074051 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/workflows/front_proximity/
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)      967 2021-11-15 05:46:02.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/workflows/front_proximity/__init__.py
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     1995 2021-11-15 05:46:02.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/workflows/front_proximity/analyzer.py
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     2027 2021-11-15 05:46:02.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/workflows/front_proximity/computational_design.py
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     8655 2022-04-07 19:59:46.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/workflows/front_proximity/core.py
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     1003 2021-11-15 05:46:02.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/workflows/front_proximity/integrator.py
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)      422 2021-11-15 05:46:02.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/workflows/front_proximity/job_generator.py
-drwxr-xr-x   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)        0 2022-04-15 21:19:48.077053 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/workflows/phenotype_proximity/
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     1275 2021-11-15 05:46:02.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/workflows/phenotype_proximity/__init__.py
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     1958 2022-04-14 19:24:13.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/workflows/phenotype_proximity/analyzer.py
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     4141 2021-11-15 05:46:02.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/workflows/phenotype_proximity/computational_design.py
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)    18907 2022-04-14 19:20:24.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/workflows/phenotype_proximity/core.py
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)    10911 2021-11-15 05:46:02.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/workflows/phenotype_proximity/integrator.py
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)      523 2021-11-15 05:46:02.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/workflows/phenotype_proximity/job_generator.py
-drwxr-xr-x   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)        0 2022-04-15 21:19:48.040660 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox.egg-info/
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)      836 2022-04-15 21:19:47.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox.egg-info/PKG-INFO
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     4919 2022-04-15 21:19:48.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox.egg-info/SOURCES.txt
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)        1 2022-04-15 21:19:47.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox.egg-info/dependency_links.txt
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)      285 2022-04-15 21:19:47.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox.egg-info/requires.txt
--rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)       24 2022-04-15 21:19:47.000000 spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox.egg-info/top_level.txt
+drwxr-xr-x   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)        0 2022-03-18 16:55:03.358274 spatialprofilingtoolbox-0.9.2/
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)      950 2021-08-09 23:10:18.000000 spatialprofilingtoolbox-0.9.2/LICENSE.md
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)      834 2022-03-18 16:55:03.357993 spatialprofilingtoolbox-0.9.2/PKG-INFO
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)    11235 2022-03-18 16:19:54.000000 spatialprofilingtoolbox-0.9.2/README.md
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)      104 2021-08-09 23:10:18.000000 spatialprofilingtoolbox-0.9.2/pyproject.toml
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)       38 2022-03-18 16:55:03.358388 spatialprofilingtoolbox-0.9.2/setup.cfg
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     3206 2022-03-18 15:58:37.000000 spatialprofilingtoolbox-0.9.2/setup.py
+drwxr-xr-x   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)        0 2022-03-18 16:55:03.335457 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     3582 2022-03-18 16:08:11.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/__init__.py
+drwxr-xr-x   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)        0 2022-03-18 16:55:03.337851 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/applications/
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)      174 2021-08-09 23:10:18.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/applications/__init__.py
+drwxr-xr-x   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)        0 2022-03-18 16:55:03.338481 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/applications/cell_cartoons/
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)      391 2021-08-09 23:10:18.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/applications/cell_cartoons/__init__.py
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)      673 2021-08-09 23:10:18.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/applications/cell_cartoons/application.py
+drwxr-xr-x   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)        0 2022-03-18 16:55:03.339239 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/applications/configuration_ui/
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)       84 2021-11-15 05:46:02.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/applications/configuration_ui/__init__.py
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     7400 2021-11-15 05:46:02.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/applications/configuration_ui/ui.py
+drwxr-xr-x   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)        0 2022-03-18 16:55:03.339990 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/applications/diffusion_graphs_viz/
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)      143 2021-08-09 23:10:18.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/applications/diffusion_graphs_viz/__init__.py
+-rwxr-xr-x   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     6785 2021-08-09 23:10:18.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/applications/diffusion_graphs_viz/diffusion_graphs_viz.py
+drwxr-xr-x   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)        0 2022-03-18 16:55:03.340691 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/applications/diffusion_tests_viz/
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)      171 2021-08-09 23:10:18.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/applications/diffusion_tests_viz/__init__.py
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)    11629 2021-09-17 21:18:07.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/applications/diffusion_tests_viz/diffusion_tests_viz.py
+drwxr-xr-x   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)        0 2022-03-18 16:55:03.341258 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/applications/front_proximity_viz/
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)      156 2021-08-09 23:10:18.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/applications/front_proximity_viz/__init__.py
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)    11479 2021-08-09 23:10:18.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/applications/front_proximity_viz/front_proximity_viz.py
+drwxr-xr-x   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)        0 2022-03-18 16:55:03.341563 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/dataset_designs/
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)      196 2021-08-09 23:10:18.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/dataset_designs/__init__.py
+drwxr-xr-x   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)        0 2022-03-18 16:55:03.343106 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/dataset_designs/multiplexed_imaging/
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)      776 2021-08-09 23:10:18.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/dataset_designs/multiplexed_imaging/__init__.py
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     2874 2021-11-15 05:46:02.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/dataset_designs/multiplexed_imaging/halo_areas_provider.py
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)    15651 2022-03-10 18:45:34.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/dataset_designs/multiplexed_imaging/halo_cell_metadata_design.py
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)    13119 2021-11-15 05:46:02.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/dataset_designs/multiplexed_imaging/halo_cell_metadata_provider.py
+drwxr-xr-x   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)        0 2022-03-18 16:55:03.347348 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/environment/
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)      254 2021-08-09 23:10:18.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/environment/__init__.py
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     2533 2021-11-15 21:33:15.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/environment/calculator.py
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     5570 2021-09-17 21:18:07.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/environment/cell_metadata.py
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     1620 2021-11-15 05:46:02.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/environment/computational_design.py
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     2229 2022-03-18 16:37:18.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/environment/configuration.py
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)      708 2021-11-15 05:46:02.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/environment/configuration_settings.py
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     2830 2021-09-17 21:18:07.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/environment/database_context_utility.py
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     3115 2021-11-15 05:46:02.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/environment/dichotomization.py
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     4334 2021-11-15 05:46:02.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/environment/file_io.py
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     4797 2021-11-15 05:46:02.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/environment/job_generator.py
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     2473 2022-03-15 18:36:28.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/environment/log_formats.py
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)      546 2021-11-15 05:46:02.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/environment/settings_wrappers.py
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     3240 2021-11-15 05:46:02.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/environment/single_job_analyzer.py
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)      461 2021-11-15 05:46:02.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/environment/workflow_modules.py
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)      318 2022-03-18 15:57:25.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/nextflow.config.local
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)      316 2022-03-18 15:57:19.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/nextflow.config.lsf
+drwxr-xr-x   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)        0 2022-03-18 16:55:03.349461 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/scripts/
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     1843 2021-11-15 05:46:02.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/scripts/spt-aggregate-cell-data
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     1249 2021-11-15 21:33:15.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/scripts/spt-diffusion-graphs-viz
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)      771 2021-11-15 21:33:15.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/scripts/spt-diffusion-viz
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)      889 2021-11-15 21:33:15.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/scripts/spt-front-proximity-viz
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     2437 2021-11-15 05:46:02.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/scripts/spt-merge-sqlite-dbs
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     3713 2022-03-18 16:08:18.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/scripts/spt-pipeline
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)      877 2022-03-18 15:33:41.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/scripts/spt-print
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     3319 2022-03-18 15:33:04.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/spt_pipeline.nf
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)        5 2022-03-18 16:38:27.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/version.txt
+drwxr-xr-x   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)        0 2022-03-18 16:55:03.349808 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/workflows/
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)      874 2021-08-09 23:10:18.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/workflows/__init__.py
+drwxr-xr-x   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)        0 2022-03-18 16:55:03.351829 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/workflows/density/
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)      752 2021-11-15 05:46:02.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/workflows/density/__init__.py
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     2645 2021-11-15 20:00:32.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/workflows/density/analyzer.py
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     5970 2022-03-10 18:45:44.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/workflows/density/computational_design.py
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)    11200 2022-03-10 18:45:44.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/workflows/density/core.py
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     4842 2022-03-10 18:45:44.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/workflows/density/data_logging.py
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)    22951 2022-03-10 18:45:44.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/workflows/density/integrator.py
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)      548 2021-11-15 20:00:32.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/workflows/density/job_generator.py
+drwxr-xr-x   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)        0 2022-03-18 16:55:03.353638 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/workflows/diffusion/
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     1072 2021-11-15 05:46:02.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/workflows/diffusion/__init__.py
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     7446 2021-11-15 05:46:02.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/workflows/diffusion/analyzer.py
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     2891 2021-11-15 05:46:02.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/workflows/diffusion/computational_design.py
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)    14889 2021-11-15 05:46:02.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/workflows/diffusion/core.py
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)    20856 2021-11-15 05:46:02.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/workflows/diffusion/integrator.py
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)      412 2021-11-15 05:46:02.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/workflows/diffusion/job_generator.py
+drwxr-xr-x   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)        0 2022-03-18 16:55:03.355481 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/workflows/front_proximity/
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)      967 2021-11-15 05:46:02.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/workflows/front_proximity/__init__.py
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     1995 2021-11-15 05:46:02.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/workflows/front_proximity/analyzer.py
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     2027 2021-11-15 05:46:02.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/workflows/front_proximity/computational_design.py
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     8655 2021-11-15 23:52:18.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/workflows/front_proximity/core.py
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     1003 2021-11-15 05:46:02.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/workflows/front_proximity/integrator.py
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)      422 2021-11-15 05:46:02.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/workflows/front_proximity/job_generator.py
+drwxr-xr-x   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)        0 2022-03-18 16:55:03.357651 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/workflows/phenotype_proximity/
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     1275 2021-11-15 05:46:02.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/workflows/phenotype_proximity/__init__.py
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     2354 2021-11-15 05:46:02.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/workflows/phenotype_proximity/analyzer.py
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     4141 2021-11-15 05:46:02.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/workflows/phenotype_proximity/computational_design.py
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)    20080 2022-03-15 18:36:28.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/workflows/phenotype_proximity/core.py
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)    10911 2021-11-15 05:46:02.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/workflows/phenotype_proximity/integrator.py
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)      523 2021-11-15 05:46:02.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/workflows/phenotype_proximity/job_generator.py
+drwxr-xr-x   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)        0 2022-03-18 16:55:03.337452 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox.egg-info/
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)      834 2022-03-18 16:55:02.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox.egg-info/PKG-INFO
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)     4340 2022-03-18 16:55:03.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)        1 2022-03-18 16:55:02.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)      233 2022-03-18 16:55:03.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox.egg-info/requires.txt
+-rw-r--r--   0 mathewj2 (925913212) MSKCC\Domain Users (9696963)       24 2022-03-18 16:55:03.000000 spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox.egg-info/top_level.txt
```

### Comparing `spatialprofilingtoolbox-0.9.107/LICENSE.md` & `spatialprofilingtoolbox-0.9.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `spatialprofilingtoolbox-0.9.107/PKG-INFO` & `spatialprofilingtoolbox-0.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spatialprofilingtoolbox
-Version: 0.9.107
+Version: 0.9.2
 Summary: Toolbox for spatial analysis of pathology images.
 Home-page: https://spatialprofilingtoolbox.readthedocs.io/en/prerelease/readme.html
 Author: Rami Vanguri, James Mathews
 Author-email: mathewj2@mskcc.org
 License: UNKNOWN
 Project-URL: Documentation, https://spatialprofilingtoolbox.readthedocs.io/en/prerelease/readme.html
 Project-URL: Source code, https://github.com/nadeemlab/SPT
```

### Comparing `spatialprofilingtoolbox-0.9.107/README.md` & `spatialprofilingtoolbox-0.9.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 <p align="center">
 <a href="https://github.com/nadeemlab/SPT#Supported-workflows">Supported workflows</a>
  | <a href="https://github.com/nadeemlab/SPT#Preparing-your-data">Preparing your data</a>
  | <a href="https://github.com/nadeemlab/SPT#Prerequisites">Prerequisites</a>
  | <a href="https://github.com/nadeemlab/SPT#Getting-started">Getting started</a>
  | <a href="https://github.com/nadeemlab/SPT#Examples">Examples</a>
  | <a href="https://spatialprofilingtoolbox.readthedocs.io">Read the Docs</a>
- | <a href="https://nadeemlab.github.io/SPT/maintenance.html">Maintenance</a>
 </p>
 
 The SPT modules do image analysis computation in the context of histopathology. For the convenience of automatic usage in different runtime contexts, the pipelines are orchestrated with [Nextflow](https://www.nextflow.io/).
 
 Supported workflows
 -------------------
 - **Phenotype proximity workflow**. The core module takes as input two collections of points, and calculates the average density with which a point of one set appears within a specified distance from a given point of the other set. In a balanced/symmetric mode, it calculates instead the density of occurence of a pair of points from the respective sets within the specified distance range.
@@ -36,88 +35,45 @@
 ---------------
 Install the SPT tools from [PyPI](https://pypi.org/project/spatialprofilingtoolbox/):
 
 ```sh
 pip install spatialprofilingtoolbox
 ```
 
-Now run
-
-```sh
-spt-pipeline configure
-```
-
-in a clean directory. You will be prompted to choose which computations to do, where the input data is stored, etc.
-
-Then:
-
-```sh
-spt-pipeline run
-```
+Now you just do `spt-pipeline` in the directory where you want all of the outputs to be created. On the first run, you will be prompted to choose which computations to do, where the input data is stored, etc.
 
 If you just want to try this out, without [preparing your own input data](#Preparing-your-data) as described above, you can clone this repository, do `cd tests/`, and use the test data in `tests/data/` by answering the prompts as shown:
 
 <p align="center">
 <img src="docs/_static/dialog_example.png" alt="config dialog">
 </p>
 
-You can also **skip the configuration dialog** by creating `.spt_pipeline.json` in your working directory before running `spt-pipeline`, for example copied from a previous run. Moreover if you prefer a more "Nextflow native" deployment, you can just copy the script [`spt_pipeline.nf`](spatialprofilingtoolbox/spt_pipeline.nf) and to your working directory and use Nextflow directly:
+You can also skip the dialog by creating the configuration file `.spt_pipeline.json` in your working directory before running `spt-pipeline`. Moreover if you prefer a more "Nextflow native" deployment, you can just copy the script [`spt_pipeline.nf`](spatialprofilingtoolbox/spt_pipeline.nf) and to your working directory and then use Nextflow directly:
 
 ```
 nextflow spt_pipeline.nf
 ```
 
-### LSF
+#### LSF
 The pipeline seamlessly supports High-Performance Clusters (HPCs) running [Platform LSF](https://www.ibm.com/products/hpc-workload-management) on which [Singularity](https://sylabs.io/singularity/) is installed. However every HPC is configured differently with respect to shared file system resources, and few HPCs allow the Docker daemon that would permit automatic container usage. For this reason it is currently necessary to manually pull the Docker container "as" a singularity container from our public registry,
 
 ```sh
 singularity pull docker://nadeemlab/spt:latest
 ```
 
 and move the resulting `.sif` file to a shared area accessible to the nodes in your cluster.
 
-Now run `spt-pipeline configure` and supply the path to your SIF file.
+Then use `spt-pipeline write-nextflow-script` to generate `nextflow.config.lsf`, in which you should add the path to your `.sif` file.
 
-Finally, use `spt-pipeline run`, or, more explicitly:
+Finally, run `spt-pipeline`, or, more explicitly:
 
 ```sh
 nextflow -c nextflow.config.lsf run spt_pipeline.nf
 ```
 
-### Monitoring output
-SPT generates verbose logs, which Nextflow sends to files `work/*/*/.command.log` .
-
-A convenient way to monitor these is:
-
-```sh
-tail -f $(find work/*/*/\.command.log)
-```
-
-Since new log files are created as the workflow progresses, you may need to run this command multiple times.
-
-Another way monitor the log files is to use [`multitail`](https://github.com/halturin/multitail). `multitail` can be used from a local `make` build of its source code.
-Monitor the logs from each process deployed by Nextflow:
-
-```sh
-multitail -cT ANSI $(find work/*/*/\.command.log | tr '\n' 'X' | sed 's/X/ -cT ANSI /g')
-```
-
-Common `multitail` commands:
-- `d` brings up a list of the windows, to be deleted on `<ENTER>`. Helpful when there are lots of windows.
-- `q` quits.
-- `ctrl-h` brings up a list of other commands.
-
-Note: If there are many user applications running, you may need to increase certain file-monitoring limits:
-
-```sh
-sudo sysctl fs.inotify.max_user_instances=8192
-sudo sysctl -p
-```
-
-
 Examples
 --------
 The dataset analyzed in the following examples is imaging mass cytometry of breast cancer tissue microarrays, published [here](https://doi.org/10.5281/zenodo.3518283). For the purpose of phenotyping, continuous intensity values were dichotomized using a [log transformation and 2-population Gaussian mixture model](https://github.com/nadeemlab/SPT/blob/main/spatialprofilingtoolbox/environment/dichotomization.py).
 
 ### Phenotype proximity workflow
 
 A basic question concerning the spatial information provided by cell imaging is: What characterizes the spatial relationship between the arrangements of cells belonging to two given phenotypes?
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
                 [docs/_static/SPT_logo_blue_on_transparent.png]
  _S_u_p_p_o_r_t_e_d_ _w_o_r_k_f_l_o_w_s | _P_r_e_p_a_r_i_n_g_ _y_o_u_r_ _d_a_t_a | _P_r_e_r_e_q_u_i_s_i_t_e_s | _G_e_t_t_i_n_g_ _s_t_a_r_t_e_d |
-                    _E_x_a_m_p_l_e_s | _R_e_a_d_ _t_h_e_ _D_o_c_s | _M_a_i_n_t_e_n_a_n_c_e
+                           _E_x_a_m_p_l_e_s | _R_e_a_d_ _t_h_e_ _D_o_c_s
 The SPT modules do image analysis computation in the context of histopathology.
 For the convenience of automatic usage in different runtime contexts, the
 pipelines are orchestrated with [Nextflow](https://www.nextflow.io/). Supported
 workflows ------------------- - **Phenotype proximity workflow**. The core
 module takes as input two collections of points, and calculates the average
 density with which a point of one set appears within a specified distance from
 a given point of the other set. In a balanced/symmetric mode, it calculates
@@ -30,58 +30,47 @@
 slight differences noted where applicable. 1. Ensure a Linux/Unix-style
 environment (though a Windows deployment may work using [WSL](https://
 docs.microsoft.com/en-us/windows/wsl/about)). 2. Install Java 8+, if it is not
 already installed. This is needed for Nextflow. If you do not already have
 Nextflow installed, it will be installed by the first invocation of `spt-
 pipeline`. Getting started --------------- Install the SPT tools from [PyPI]
 (https://pypi.org/project/spatialprofilingtoolbox/): ```sh pip install
-spatialprofilingtoolbox ``` Now run ```sh spt-pipeline configure ``` in a clean
-directory. You will be prompted to choose which computations to do, where the
-input data is stored, etc. Then: ```sh spt-pipeline run ``` If you just want to
-try this out, without [preparing your own input data](#Preparing-your-data) as
-described above, you can clone this repository, do `cd tests/`, and use the
-test data in `tests/data/` by answering the prompts as shown:
+spatialprofilingtoolbox ``` Now you just do `spt-pipeline` in the directory
+where you want all of the outputs to be created. On the first run, you will be
+prompted to choose which computations to do, where the input data is stored,
+etc. If you just want to try this out, without [preparing your own input data]
+(#Preparing-your-data) as described above, you can clone this repository, do
+`cd tests/`, and use the test data in `tests/data/` by answering the prompts as
+shown:
                                 [config dialog]
-You can also **skip the configuration dialog** by creating `.spt_pipeline.json`
-in your working directory before running `spt-pipeline`, for example copied
-from a previous run. Moreover if you prefer a more "Nextflow native"
-deployment, you can just copy the script [`spt_pipeline.nf`]
-(spatialprofilingtoolbox/spt_pipeline.nf) and to your working directory and use
-Nextflow directly: ``` nextflow spt_pipeline.nf ``` ### LSF The pipeline
-seamlessly supports High-Performance Clusters (HPCs) running [Platform LSF]
-(https://www.ibm.com/products/hpc-workload-management) on which [Singularity]
-(https://sylabs.io/singularity/) is installed. However every HPC is configured
-differently with respect to shared file system resources, and few HPCs allow
-the Docker daemon that would permit automatic container usage. For this reason
-it is currently necessary to manually pull the Docker container "as" a
-singularity container from our public registry, ```sh singularity pull docker:/
-/nadeemlab/spt:latest ``` and move the resulting `.sif` file to a shared area
-accessible to the nodes in your cluster. Now run `spt-pipeline configure` and
-supply the path to your SIF file. Finally, use `spt-pipeline run`, or, more
-explicitly: ```sh nextflow -c nextflow.config.lsf run spt_pipeline.nf ``` ###
-Monitoring output SPT generates verbose logs, which Nextflow sends to files
-`work/*/*/.command.log` . A convenient way to monitor these is: ```sh tail -f $
-(find work/*/*/\.command.log) ``` Since new log files are created as the
-workflow progresses, you may need to run this command multiple times. Another
-way monitor the log files is to use [`multitail`](https://github.com/halturin/
-multitail). `multitail` can be used from a local `make` build of its source
-code. Monitor the logs from each process deployed by Nextflow: ```sh multitail
--cT ANSI $(find work/*/*/\.command.log | tr '\n' 'X' | sed 's/X/ -cT ANSI /g')
-``` Common `multitail` commands: - `d` brings up a list of the windows, to be
-deleted on ``. Helpful when there are lots of windows. - `q` quits. - `ctrl-h`
-brings up a list of other commands. Note: If there are many user applications
-running, you may need to increase certain file-monitoring limits: ```sh sudo
-sysctl fs.inotify.max_user_instances=8192 sudo sysctl -p ``` Examples -------
-- The dataset analyzed in the following examples is imaging mass cytometry of
-breast cancer tissue microarrays, published [here](https://doi.org/10.5281/
-zenodo.3518283). For the purpose of phenotyping, continuous intensity values
-were dichotomized using a [log transformation and 2-population Gaussian mixture
-model](https://github.com/nadeemlab/SPT/blob/main/spatialprofilingtoolbox/
-environment/dichotomization.py). ### Phenotype proximity workflow A basic
-question concerning the spatial information provided by cell imaging is: What
+You can also skip the dialog by creating the configuration file
+`.spt_pipeline.json` in your working directory before running `spt-pipeline`.
+Moreover if you prefer a more "Nextflow native" deployment, you can just copy
+the script [`spt_pipeline.nf`](spatialprofilingtoolbox/spt_pipeline.nf) and to
+your working directory and then use Nextflow directly: ``` nextflow
+spt_pipeline.nf ``` #### LSF The pipeline seamlessly supports High-Performance
+Clusters (HPCs) running [Platform LSF](https://www.ibm.com/products/hpc-
+workload-management) on which [Singularity](https://sylabs.io/singularity/) is
+installed. However every HPC is configured differently with respect to shared
+file system resources, and few HPCs allow the Docker daemon that would permit
+automatic container usage. For this reason it is currently necessary to
+manually pull the Docker container "as" a singularity container from our public
+registry, ```sh singularity pull docker://nadeemlab/spt:latest ``` and move the
+resulting `.sif` file to a shared area accessible to the nodes in your cluster.
+Then use `spt-pipeline write-nextflow-script` to generate
+`nextflow.config.lsf`, in which you should add the path to your `.sif` file.
+Finally, run `spt-pipeline`, or, more explicitly: ```sh nextflow -
+c nextflow.config.lsf run spt_pipeline.nf ``` Examples -------- The dataset
+analyzed in the following examples is imaging mass cytometry of breast cancer
+tissue microarrays, published [here](https://doi.org/10.5281/zenodo.3518283).
+For the purpose of phenotyping, continuous intensity values were dichotomized
+using a [log transformation and 2-population Gaussian mixture model](https://
+github.com/nadeemlab/SPT/blob/main/spatialprofilingtoolbox/environment/
+dichotomization.py). ### Phenotype proximity workflow A basic question
+concerning the spatial information provided by cell imaging is: What
 characterizes the spatial relationship between the arrangements of cells
 belonging to two given phenotypes? As an answer to this question, here we
 calculate: **(unbalanced) phenotype proximity metric**: *The average number of
 cells of a given target phenotype which occur within a prescribed (pixel)
 distance of a given cell of a given source phenotype, the average being over
 all such cells, i.e. those of the source phenotype*. High values for this
 metric may be due to overall higher counts for the target phenotype, as opposed
```

### Comparing `spatialprofilingtoolbox-0.9.107/setup.py` & `spatialprofilingtoolbox-0.9.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,17 +22,14 @@
     'seaborn==0.11.1',
     'plotly==5.1.0',
     'kaleido==0.2.1',
     'numpy==1.21.0',
     'pandas>=1.1.5',
     'scipy==1.7.1',
     'scikit-learn==0.24.1',
-    'psycopg2-binary==2.9.3',
-    'pyshp==2.2.0',
-    'tabulate==0.8.9',
 ]
 version = get_file_contents(join('spatialprofilingtoolbox', 'version.txt'))
 
 setuptools.setup(
     name='spatialprofilingtoolbox',
     version=version,
     author='Rami Vanguri, James Mathews',
@@ -46,15 +43,14 @@
         'spatialprofilingtoolbox.dataset_designs.multiplexed_imaging',
         'spatialprofilingtoolbox.workflows',
         'spatialprofilingtoolbox.workflows.diffusion',
         'spatialprofilingtoolbox.workflows.phenotype_proximity',
         'spatialprofilingtoolbox.workflows.front_proximity',
         'spatialprofilingtoolbox.workflows.density',
         'spatialprofilingtoolbox.environment',
-        'spatialprofilingtoolbox.environment.source_file_parsers',
         'spatialprofilingtoolbox.applications',
         'spatialprofilingtoolbox.applications.configuration_ui',
         'spatialprofilingtoolbox.applications.cell_cartoons',
         'spatialprofilingtoolbox.applications.diffusion_tests_viz',
         'spatialprofilingtoolbox.applications.diffusion_graphs_viz',
         'spatialprofilingtoolbox.applications.front_proximity_viz',
     ],
@@ -65,16 +61,14 @@
         'Intended Audience :: Science/Research',
     ],
     package_data={'spatialprofilingtoolbox': [
             'version.txt',
             'spt_pipeline.nf',
             'nextflow.config.lsf',
             'nextflow.config.local',
-            'fields.tsv',
-            'pathology_schema.sql',
         ]},
     python_requires='>=3.7',
     scripts=[
         'spatialprofilingtoolbox/scripts/spt-pipeline',
         'spatialprofilingtoolbox/scripts/spt-merge-sqlite-dbs',
         'spatialprofilingtoolbox/scripts/spt-diffusion-viz',
         'spatialprofilingtoolbox/scripts/spt-diffusion-graphs-viz',
```

### Comparing `spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/__init__.py` & `spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from .environment.configuration import get_config_parameters
 from .environment.configuration import write_out_nextflow_script
 from .environment.configuration import nf_script_file
 from .environment.configuration import nf_config_file
 from .applications.configuration_ui.ui import configuration_dialog
 
 from .environment.settings_wrappers import DatasetSettings
-from .environment.skimmer import DataSkimmer
 from .environment.log_formats import colorized_logger
 __logger = colorized_logger(__name__)
 
 __version__ = get_version()
 
 def get_job_generator(workflow=None, **kwargs):
     """
@@ -32,20 +31,14 @@
             dataset_design_class = dataset_design_class,
             **kwargs,
         )
     else:
         __logger.error('Workflow "%s" not supported.', str(workflow))
         raise TypeError
 
-def get_semantic_source_parser(workflow=None, **kwargs):
-    return DataSkimmer(
-        dataset_settings = get_dataset_settings(**kwargs),
-        dataset_design = get_dataset_design(workflow=workflow, **kwargs),
-    )
-
 def get_dataset_design_class(workflow=None, **kwargs):
     return workflows[workflow].dataset_design
 
 def get_dataset_design(workflow=None, **kwargs):
     """
     Exposes design parameters to scripts.
     """
```

### Comparing `spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/applications/cell_cartoons/application.py` & `spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/applications/cell_cartoons/application.py`

 * *Files identical despite different names*

### Comparing `spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/applications/configuration_ui/ui.py` & `spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/applications/configuration_ui/ui.py`

 * *Files 7% similar despite different names*

```diff
@@ -195,27 +195,14 @@
         )
         if re.match(yes_pattern, save_graphml):
             save_graphml = True
         else:
             save_graphml = False
         parameters['save_graphml'] = save_graphml
 
-    sif_file = pp.prompt(
-        'If using singularity container SIF file, supply the path to it here (otherwise enter the empty string):'
-    )
-    if not sif_file in [None, '']:
-        if exists(sif_file):
-            parameters['sif_file'] = sif_file
-
-    excluded_host_name = pp.prompt(
-        'If using a cluster, if desired supply the name of a host to exclude (otherwise enter the empty string):'
-    )
-    if not excluded_host_name in [None, '']:
-        parameters['excluded_host_name'] = excluded_host_name
-
     skip_integrity_check = pp.prompt(
         'Skip file integrity check?',
         validator = bool_validator,
     )
     if re.match(yes_pattern, skip_integrity_check):
         skip_integrity_check = True
     else:
```

### Comparing `spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/applications/diffusion_graphs_viz/diffusion_graphs_viz.py` & `spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/applications/diffusion_graphs_viz/diffusion_graphs_viz.py`

 * *Files identical despite different names*

### Comparing `spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/applications/diffusion_tests_viz/diffusion_tests_viz.py` & `spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/applications/diffusion_tests_viz/diffusion_tests_viz.py`

 * *Files identical despite different names*

### Comparing `spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/applications/front_proximity_viz/front_proximity_viz.py` & `spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/applications/front_proximity_viz/front_proximity_viz.py`

 * *Files identical despite different names*

### Comparing `spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/dataset_designs/multiplexed_imaging/__init__.py` & `spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/dataset_designs/multiplexed_imaging/__init__.py`

 * *Files identical despite different names*

### Comparing `spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/dataset_designs/multiplexed_imaging/halo_cell_metadata_design.py` & `spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/dataset_designs/multiplexed_imaging/halo_cell_metadata_design.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import pathlib
 import os
 from os.path import join
-from os.path import exists
 
 import pandas as pd
 
+from .halo_areas_provider import HALORegionalAreasProvider
 from ...environment.file_io import get_input_filename_by_identifier
 from ...environment.settings_wrappers import DatasetSettings
 from ...environment.log_formats import colorized_logger
-from ...environment.extract_compartments import extract_compartments
 
 logger = colorized_logger(__name__)
 
 
 class HALOCellMetadataDesign:
     """
     This class provides the schema necessary to interpret cell metadata manifests
@@ -49,28 +48,16 @@
             file_metadata = pd.read_csv(self.dataset_settings.file_manifest_file, sep='\t'),
             input_file_identifier = 'Elementary phenotypes file',
         )
         self.elementary_phenotypes = pd.read_csv(
             elementary_phenotypes_file,
             keep_default_na=False,
         )
-        if compartments:
-            self.compartments = compartments
-        else:
-            if not 'compartments_file' in kwargs:
-                compartments_file = 'compartments.txt'
-            else:
-                compartments_file = kwargs['compartments_file']
-            if not exists(compartments_file):
-                self.compartments = extract_compartments(
-                    self.dataset_settings,
-                    HALOCellMetadataDesign.get_cell_manifest_descriptor(),
-                )
-            else:
-                self.compartments = open(compartments_file, 'rt').read().strip('\n').split('\n')
+        self.compartments = compartments
+        self.areas_provider = HALORegionalAreasProvider
 
     def get_FOV_column(self):
         """
         Returns:
             str:
                 The column name for the column in the HALO-exported CSV which indicates
                 the field of view in which the cell corresponding to a table record
@@ -115,26 +102,39 @@
         :rtype: str
         """
         if r'\\' in fov:
             return pathlib.PureWindowsPath(fov).name
         else:
             return fov
 
+    def get_regional_areas_file_identifier(self):
+        """
+        Returns:
+            str:
+                The name of the file identifier (as it would appear in the file
+                manifest) that identifies the file providing areas for each compartment
+                appearing in some field of view of some sample.
+        """
+        return 'Regional areas file'
+
     @staticmethod
     def get_cell_manifest_descriptor():
         return 'HALO software cell manifest'
 
     @staticmethod
     def validate_cell_manifest_descriptor(descriptor):
         return descriptor in [
             HALOCellMetadataDesign.get_cell_manifest_descriptor(),
             'simulated HALO-exported cell manifest',
         ]
         return 'HALO software cell manifest'
 
+    def get_regional_areas_table_descriptor(self):
+        return 'HALO software regional/compartment areas'
+
     def get_compartments(self):
         """
         Returns:
             list:
                 A list of the expected compartment names (i.e. "Classifier Label"
                 values). This method may need to be migrated to a more specific
                 dataset design module, or else obtain its values from a separate
```

### Comparing `spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/dataset_designs/multiplexed_imaging/halo_cell_metadata_provider.py` & `spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/dataset_designs/multiplexed_imaging/halo_cell_metadata_provider.py`

 * *Files identical despite different names*

### Comparing `spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/environment/calculator.py` & `spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/environment/calculator.py`

 * *Files identical despite different names*

### Comparing `spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/environment/cell_metadata.py` & `spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/environment/cell_metadata.py`

 * *Files identical despite different names*

### Comparing `spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/environment/computational_design.py` & `spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/environment/computational_design.py`

 * *Files identical despite different names*

### Comparing `spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/environment/configuration.py` & `spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/environment/configuration.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,45 +4,36 @@
 """
 import importlib.resources
 import os
 from os.path import abspath
 from os.path import exists
 from os.path import join
 import json
-import re
 
 from ..applications.configuration_ui.ui import configuration_dialog
 from .configuration_settings import config_filename
 from .configuration_settings import get_version
-from .extract_compartments import extract_compartments
-from .settings_wrappers import DatasetSettings
 
 from .log_formats import colorized_logger
 logger = colorized_logger(__name__)
 
 nf_script_file = 'spt_pipeline.nf'
 nf_config_file = {
     'lsf' : 'nextflow.config.lsf',
     'local' : 'nextflow.config.local',
 }
 
-def write_out_nextflow_script(sif_file, excluded_host_name=None):
+def write_out_nextflow_script():
     for filename in [nf_script_file] + list(nf_config_file.values()):
         contents = None
         with importlib.resources.path('spatialprofilingtoolbox', filename) as path:
             with open(path, 'rt') as file:
                 contents = file.read().rstrip('\n')
         if contents:
             if not exists(join(os.getcwd(), filename)):
-                if sif_file:
-                    contents = re.sub("'spt_latest\.sif'", "'" + sif_file + "'", contents)
-                if filename == 'nextflow.config.lsf':
-                    if not excluded_host_name is None:
-                        contents = re.sub('{{ host_to_exclude }}', excluded_host_name, contents)
-                        contents = re.sub('// process {', 'process {', contents)
                 with open(join(os.getcwd(), filename), 'wt') as file:
                     file.write(contents)
         else:
             logger.error('Could not load %s', filename)
 
 def get_config_parameters(json_string=None):
     supplied_json_string = not json_string is None
@@ -59,12 +50,17 @@
         configuration_dialog()
         json_string = open(config_filename, 'rt').read()
 
     if (not supplied_json_string) and has_config_file:
         json_string = open(config_filename, 'rt').read()
 
     parameters = json.loads(json_string)
-
-    if not 'file_manifest_file' in parameters:
-        parameters['file_manifest_file'] = 'file_manifest.tsv'
+    version_specifier = 'spt_version'
+    if version_specifier in parameters:
+        if parameters[version_specifier] != get_version():
+            logger.debug(
+                'Version mentioned in configuration file is %s, but running version of SPT is %s.',
+                parameters[version_specifier],
+                get_version(),
+            )
 
     return parameters
```

### Comparing `spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/environment/configuration_settings.py` & `spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/environment/configuration_settings.py`

 * *Files identical despite different names*

### Comparing `spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/environment/database_context_utility.py` & `spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/environment/database_context_utility.py`

 * *Files identical despite different names*

### Comparing `spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/environment/dichotomization.py` & `spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/environment/dichotomization.py`

 * *Files identical despite different names*

### Comparing `spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/environment/log_formats.py` & `spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/environment/log_formats.py`

 * *Files identical despite different names*

### Comparing `spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/environment/settings_wrappers.py` & `spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/environment/settings_wrappers.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import os
 from os.path import join
 FIND_FILES_USING_PATH = ('FIND_FILES_USING_PATH' in os.environ)
-# When running under Nextflow, dependence on files via absolute paths are prohibited
 
 
 class DatasetSettings:
     """
     A convenience bundle object to store information about an input dataset's
     location on the file system.
     """
```

### Comparing `spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/environment/single_job_analyzer.py` & `spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/environment/single_job_analyzer.py`

 * *Files identical despite different names*

### Comparing `spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/scripts/spt-aggregate-cell-data` & `spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/scripts/spt-aggregate-cell-data`

 * *Files identical despite different names*

### Comparing `spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/scripts/spt-diffusion-graphs-viz` & `spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/scripts/spt-diffusion-graphs-viz`

 * *Files identical despite different names*

### Comparing `spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/scripts/spt-diffusion-viz` & `spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/scripts/spt-diffusion-viz`

 * *Files identical despite different names*

### Comparing `spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/scripts/spt-front-proximity-viz` & `spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/scripts/spt-front-proximity-viz`

 * *Files identical despite different names*

### Comparing `spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/scripts/spt-merge-sqlite-dbs` & `spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/scripts/spt-merge-sqlite-dbs`

 * *Files identical despite different names*

### Comparing `spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/scripts/spt-print` & `spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/scripts/spt-print`

 * *Files identical despite different names*

### Comparing `spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/spt_pipeline.nf` & `spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/spt_pipeline.nf`

 * *Files 24% similar despite different names*

```diff
@@ -13,18 +13,15 @@
     #!/usr/bin/env python3
     import os
     from os.path import join
     import json
 
     parameters = json.load(open('$config_file', 'rt'))
     input_path = parameters['input_path']
-    if 'file_manifest_file' in parameters:
-        manifest = parameters['file_manifest_file']
-    else:
-        manifest = 'file_manifest.tsv'
+    manifest = parameters['file_manifest_file']
     file_manifest_file = join(input_path, manifest)
     print(file_manifest_file, end='')
     """
 }
 
 process list_auxiliary_job_inputs {
     input:
@@ -50,73 +47,20 @@
 
     script:
     """
     spt-pipeline generate-jobs
     """
 }
 
-process list_all_jobs_inputs {
-    input:
-    path config_file
-    path file_manifest_file
-
-    output:
-    path 'all_jobs_input_files.txt'
-
-    script:
-    """
-    spt-pipeline list-all-jobs-inputs --all-jobs-inputs=all_jobs_input_files.txt
-    """
-}
-
-process list_all_compartments {
-    input:
-    path config_file
-    path file_manifest_file
-    path extra_dependencies
-
-    output:
-    path 'compartments.txt'
-
-    script:
-    """
-    spt-pipeline list-all-compartments --compartments-file=compartments.txt
-    """
-}
-
-process semantic_parsing {
-    publishDir 'results'
-
-    input:
-    path config_file
-    path file_manifest_file
-    path extra_dependencies
-    path compartments
-
-    output:
-    path 'normalized_source_data.db'
-
-    script:
-    """
-    spt-pipeline semantic-parse
-    """
-}
-
 process single_job {
-    memory { 2.GB * task.attempt }
-
-    errorStrategy { task.exitStatus in 137..140 ? 'retry' : 'terminate' }
-    maxRetries 4
-
     input:
     path config_file
     path file_manifest_file
     tuple val(input_file_identifier), file(input_filename), val(job_index)
     path extra_dependencies
-    path compartments
 
     output:
     file "intermediate${job_index}.db"
 
     script:
     """
     spt-pipeline single-job --input-file-identifier="$input_file_identifier" --intermediate-database-filename=intermediate${job_index}.db
@@ -134,27 +78,21 @@
     script:
     """
     spt-merge-sqlite-dbs $all_database_filenames --output=merged.db
     """
 }
 
 process aggregate_results {
-    memory { 2.GB * task.attempt }
-
-    errorStrategy { task.exitStatus in 137..140 ? 'retry' : 'terminate' }
-    maxRetries 6
-
     publishDir 'results'
 
     input:
     path config_file
     path file_manifest_file
     path 'intermediate.0.db'
     path extra_dependencies
-    path compartments
 
     output:
     file 'intermediate.db'
     file 'stats_tests.csv'
 
     script:
     """
@@ -193,48 +131,19 @@
     )
         .map{ file(it) }
         .splitText(by: 1)
         .map{ file(it.trim()) }
         .collect()
         .set{ auxiliary_job_input_files_ch }
 
-    list_all_jobs_inputs(
-        config_file_ch,
-        file_manifest_ch,
-    )
-        .map{ file(it) }
-        .splitText(by: 1)
-        .map{ file(it.trim()) }
-        .collect()
-        .set{ all_job_input_files_ch }
-
-    list_all_compartments(
-        config_file_ch,
-        file_manifest_ch,
-        all_job_input_files_ch,
-    )
-        .map{ file(it) }
-        .splitText(by: 1)
-        .map{ file(it.trim()) }
-        .collect()
-        .set{ compartments_ch }
-
-    semantic_parsing(
-        config_file_ch,
-        file_manifest_ch,
-        all_job_input_files_ch,
-        compartments_ch,
-    )
-
     single_job(
         config_file_ch,
         file_manifest_ch,
         jobs_ch,
         auxiliary_job_input_files_ch,
-        compartments_ch,
     )
         .collect()
         .set{ all_intermediate_databases }
 
     merge_databases(
         all_intermediate_databases,
         all_intermediate_database_filenames,
@@ -242,10 +151,9 @@
         .set{ merged_database_ch }
 
     aggregate_results(
         config_file_ch,
         file_manifest_ch,
         merged_database_ch,
         auxiliary_job_input_files_ch,
-        compartments_ch,
     )
 }
```

### Comparing `spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/workflows/__init__.py` & `spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/workflows/density/__init__.py` & `spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/workflows/density/__init__.py`

 * *Files identical despite different names*

### Comparing `spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/workflows/density/analyzer.py` & `spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/workflows/density/analyzer.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 
 class DensityAnalyzer(SingleJobAnalyzer):
     """
     The main class of the job.
     """
     def __init__(self,
+        skip_integrity_check=False,
         **kwargs,
     ):
         super(DensityAnalyzer, self).__init__(**kwargs)
         self.retrieve_input_filename()
         self.retrieve_sample_identifier()
         self.calculator = DensityCalculator(
             input_filename = self.get_input_filename(),
```

### Comparing `spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/workflows/density/computational_design.py` & `spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/workflows/density/computational_design.py`

 * *Files identical despite different names*

### Comparing `spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/workflows/density/core.py` & `spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/workflows/density/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,17 +169,15 @@
             nearest_cell_columns = ['distance to nearest cell ' + compartment for compartment in all_compartments]
 
             table['sample_identifier'] = sample_identifier
             table['outcome_assignment'] = outcomes_dict[sample_identifier]
 
             if self.computational_design.use_intensities:
                 self.overlay_intensities(table)
-                intensity_columns = self.computational_design.get_intensity_columns(values_only=True)
-            else:
-                intensity_columns = []
+            intensity_columns = self.computational_design.get_intensity_columns(values_only=True)
 
             pertinent_columns = [
                 'sample_identifier',
                 self.dataset_design.get_FOV_column(),
                 'outcome_assignment',
                 'compartment',
                 self.dataset_design.get_cell_area_column(),
```

### Comparing `spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/workflows/density/data_logging.py` & `spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/workflows/density/data_logging.py`

 * *Files identical despite different names*

### Comparing `spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/workflows/density/integrator.py` & `spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/workflows/density/integrator.py`

 * *Files identical despite different names*

### Comparing `spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/workflows/density/job_generator.py` & `spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/workflows/density/job_generator.py`

 * *Files identical despite different names*

### Comparing `spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/workflows/diffusion/__init__.py` & `spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/workflows/diffusion/__init__.py`

 * *Files identical despite different names*

### Comparing `spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/workflows/diffusion/analyzer.py` & `spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/workflows/diffusion/analyzer.py`

 * *Files identical despite different names*

### Comparing `spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/workflows/diffusion/computational_design.py` & `spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/workflows/diffusion/computational_design.py`

 * *Files identical despite different names*

### Comparing `spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/workflows/diffusion/core.py` & `spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/workflows/diffusion/core.py`

 * *Files identical despite different names*

### Comparing `spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/workflows/diffusion/integrator.py` & `spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/workflows/diffusion/integrator.py`

 * *Files identical despite different names*

### Comparing `spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/workflows/front_proximity/__init__.py` & `spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/workflows/front_proximity/__init__.py`

 * *Files identical despite different names*

### Comparing `spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/workflows/front_proximity/analyzer.py` & `spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/workflows/front_proximity/analyzer.py`

 * *Files identical despite different names*

### Comparing `spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/workflows/front_proximity/computational_design.py` & `spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/workflows/front_proximity/computational_design.py`

 * *Files identical despite different names*

### Comparing `spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/workflows/front_proximity/core.py` & `spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/workflows/front_proximity/core.py`

 * *Files identical despite different names*

### Comparing `spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/workflows/front_proximity/integrator.py` & `spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/workflows/front_proximity/integrator.py`

 * *Files identical despite different names*

### Comparing `spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/workflows/phenotype_proximity/__init__.py` & `spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/workflows/phenotype_proximity/__init__.py`

 * *Files identical despite different names*

### Comparing `spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/workflows/phenotype_proximity/analyzer.py` & `spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/workflows/phenotype_proximity/analyzer.py`

 * *Files 20% similar despite different names*

```diff
@@ -21,21 +21,28 @@
     The main class of the single job.
     """
     def __init__(self, **kwargs):
         super(PhenotypeProximityAnalyzer, self).__init__(**kwargs)
 
         self.retrieve_input_filename()
         self.retrieve_sample_identifier()
+        file_id = self.dataset_design.get_regional_areas_file_identifier()
+        regional_areas_file = get_input_filename_by_identifier(
+            dataset_settings = self.dataset_settings,
+            file_metadata = pd.read_csv(self.dataset_settings.file_manifest_file, sep='\t'),
+            input_file_identifier = file_id,
+        )
 
         self.calculator = PhenotypeProximityCalculator(
             input_filename = self.get_input_filename(),
             sample_identifier = self.get_sample_identifier(),
             dataset_settings = self.dataset_settings,
             dataset_design = self.dataset_design,
             computational_design = self.computational_design,
+            regional_areas_file = regional_areas_file,
         )
 
     def _calculate(self):
         self.calculator.calculate_proximity()
 
     def initialize_intermediate_database(self):
         cell_pair_counts_header = self.computational_design.get_cell_pair_counts_table_header()
```

### Comparing `spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/workflows/phenotype_proximity/computational_design.py` & `spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/workflows/phenotype_proximity/computational_design.py`

 * *Files identical despite different names*

### Comparing `spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/workflows/phenotype_proximity/core.py` & `spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/workflows/phenotype_proximity/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     radius_pixels_upper_limit = 100
     radius_number_increments = 4
 
     def __init__(self,
         input_filename: str=None,
         sample_identifier: str=None,
         dataset_settings: DatasetSettings=None,
+        regional_areas_file: str=None,
         **kwargs,
     ):
         """
         :param input_filename: The filename for the source file with cell data.
         :type input_filename: str
 
         :param sample_identifier: The sample associated with this source file.
@@ -47,22 +48,30 @@
 
         :param dataset_settings: Dataset-specific paths and settings.
         :type dataset_settings: DatasetSettings
 
         :param dataset_design: The design object for the input dataset.
 
         :param computational_design: The design object for the proximity workflow.
+
+        :param regional_areas_file: The file containing total areas of classified
+            regions.
+        :type regional_areas_file: str
         """
         super(PhenotypeProximityCalculator, self).__init__(**kwargs)
         self.input_filename = input_filename
         self.sample_identifier = sample_identifier
         outcomes_file = get_outcomes_files(dataset_settings)[0]
         self.outcome = self.pull_in_outcome_data(outcomes_file)[
             sample_identifier
         ]
+        self.areas = self.dataset_design.areas_provider(
+            dataset_design=self.dataset_design,
+            regional_areas_file=regional_areas_file,
+        )
         self.fov_lookup = {}
 
     def calculate_proximity(self):
         """
         The main exposed entrypoint into the calculation.
 
         Aggregates and writes counts to database.
@@ -148,15 +157,15 @@
         intensity_column_names = self.dataset_design.get_intensity_column_names()
         inverse = {value:key for key, value in intensity_column_names.items()}
         source_columns = list(intensity_column_names.values())
         pertinent_columns = [
             'regional compartment',
             'x value',
             'y value',
-        ] + source_columns + phenotype_membership_columns + [self.dataset_design.get_cell_area_column()]
+        ] + source_columns + phenotype_membership_columns
         table.drop(
             [column for column in table.columns if not column in pertinent_columns],
             axis=1,
             inplace=True,
         )
         table.rename(columns = inverse, inplace=True)
         table.rename(columns = {
@@ -397,20 +406,37 @@
                         continue
 
                     count += additional
                     count -= sum(rows & cols)
                     source_count += sum(rows)
 
                 if balanced:
-                    area = sum(table.loc[compartment_indices[fov_index][compartment]][
-                        self.dataset_design.get_cell_area_column()
-                    ])
+                    area = 0
+                    for _, (fov_index, table) in enumerate(cells.items()):
+                        fov = self.fov_lookup[fov_index]
+                        if compartment == 'all':
+                            area0 = self.areas.get_total_compartmental_area(fov=fov)
+                        else:
+                            area0 = self.areas.get_area(fov=fov, compartment=compartment)
+                        if area0 is None:
+                            logger.warning(
+                                ''.join([
+                                    'Did not find area for "%s" compartment in field of view "%s".',
+                                    ' Skipping field of view "%s" in "%s".',
+                                ]),
+                                compartment,
+                                fov_index,
+                                fov_index,
+                                self.sample_identifier,
+                            )
+                            continue
+                        area += area0
                     if area == 0:
                         logger.warning(
-                            'Area computation failed for compartment "%s" in "%s".',
+                            'Did not find ANY area for "%s" compartment in "%s".',
                             compartment,
                             self.sample_identifier,
                         )
 
                 if source_count == 0:
                     logger.warning(
                         'No cells of "source" phenotype %s in %s, %s, within %s .',
```

### Comparing `spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/workflows/phenotype_proximity/integrator.py` & `spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/workflows/phenotype_proximity/integrator.py`

 * *Files identical despite different names*

### Comparing `spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox/workflows/phenotype_proximity/job_generator.py` & `spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox/workflows/phenotype_proximity/job_generator.py`

 * *Files identical despite different names*

### Comparing `spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox.egg-info/PKG-INFO` & `spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spatialprofilingtoolbox
-Version: 0.9.107
+Version: 0.9.2
 Summary: Toolbox for spatial analysis of pathology images.
 Home-page: https://spatialprofilingtoolbox.readthedocs.io/en/prerelease/readme.html
 Author: Rami Vanguri, James Mathews
 Author-email: mathewj2@mskcc.org
 License: UNKNOWN
 Project-URL: Documentation, https://spatialprofilingtoolbox.readthedocs.io/en/prerelease/readme.html
 Project-URL: Source code, https://github.com/nadeemlab/SPT
```

### Comparing `spatialprofilingtoolbox-0.9.107/spatialprofilingtoolbox.egg-info/SOURCES.txt` & `spatialprofilingtoolbox-0.9.2/spatialprofilingtoolbox.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 LICENSE.md
 README.md
 pyproject.toml
 setup.py
 spatialprofilingtoolbox/__init__.py
-spatialprofilingtoolbox/fields.tsv
 spatialprofilingtoolbox/nextflow.config.local
 spatialprofilingtoolbox/nextflow.config.lsf
-spatialprofilingtoolbox/pathology_schema.sql
 spatialprofilingtoolbox/spt_pipeline.nf
 spatialprofilingtoolbox/version.txt
 spatialprofilingtoolbox.egg-info/PKG-INFO
 spatialprofilingtoolbox.egg-info/SOURCES.txt
 spatialprofilingtoolbox.egg-info/dependency_links.txt
 spatialprofilingtoolbox.egg-info/requires.txt
 spatialprofilingtoolbox.egg-info/top_level.txt
@@ -23,39 +21,31 @@
 spatialprofilingtoolbox/applications/diffusion_graphs_viz/diffusion_graphs_viz.py
 spatialprofilingtoolbox/applications/diffusion_tests_viz/__init__.py
 spatialprofilingtoolbox/applications/diffusion_tests_viz/diffusion_tests_viz.py
 spatialprofilingtoolbox/applications/front_proximity_viz/__init__.py
 spatialprofilingtoolbox/applications/front_proximity_viz/front_proximity_viz.py
 spatialprofilingtoolbox/dataset_designs/__init__.py
 spatialprofilingtoolbox/dataset_designs/multiplexed_imaging/__init__.py
+spatialprofilingtoolbox/dataset_designs/multiplexed_imaging/halo_areas_provider.py
 spatialprofilingtoolbox/dataset_designs/multiplexed_imaging/halo_cell_metadata_design.py
 spatialprofilingtoolbox/dataset_designs/multiplexed_imaging/halo_cell_metadata_provider.py
 spatialprofilingtoolbox/environment/__init__.py
 spatialprofilingtoolbox/environment/calculator.py
 spatialprofilingtoolbox/environment/cell_metadata.py
 spatialprofilingtoolbox/environment/computational_design.py
 spatialprofilingtoolbox/environment/configuration.py
 spatialprofilingtoolbox/environment/configuration_settings.py
 spatialprofilingtoolbox/environment/database_context_utility.py
 spatialprofilingtoolbox/environment/dichotomization.py
-spatialprofilingtoolbox/environment/extract_compartments.py
 spatialprofilingtoolbox/environment/file_io.py
 spatialprofilingtoolbox/environment/job_generator.py
 spatialprofilingtoolbox/environment/log_formats.py
-spatialprofilingtoolbox/environment/performance_timer.py
 spatialprofilingtoolbox/environment/settings_wrappers.py
 spatialprofilingtoolbox/environment/single_job_analyzer.py
-spatialprofilingtoolbox/environment/skimmer.py
 spatialprofilingtoolbox/environment/workflow_modules.py
-spatialprofilingtoolbox/environment/source_file_parsers/__init__.py
-spatialprofilingtoolbox/environment/source_file_parsers/cellmanifests.py
-spatialprofilingtoolbox/environment/source_file_parsers/cellmanifestset.py
-spatialprofilingtoolbox/environment/source_file_parsers/channels.py
-spatialprofilingtoolbox/environment/source_file_parsers/outcomes.py
-spatialprofilingtoolbox/environment/source_file_parsers/parser.py
 spatialprofilingtoolbox/scripts/spt-aggregate-cell-data
 spatialprofilingtoolbox/scripts/spt-diffusion-graphs-viz
 spatialprofilingtoolbox/scripts/spt-diffusion-viz
 spatialprofilingtoolbox/scripts/spt-front-proximity-viz
 spatialprofilingtoolbox/scripts/spt-merge-sqlite-dbs
 spatialprofilingtoolbox/scripts/spt-pipeline
 spatialprofilingtoolbox/scripts/spt-print
```

