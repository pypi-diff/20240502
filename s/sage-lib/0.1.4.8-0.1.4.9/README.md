# Comparing `tmp/sage_lib-0.1.4.8.tar.gz` & `tmp/sage_lib-0.1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sage_lib-0.1.4.8.tar", last modified: Fri Feb 23 07:32:08 2024, max compression
+gzip compressed data, was "dist/sage_lib-0.1.4.9.tar", last modified: Thu Feb 29 10:29:26 2024, max compression
```

## Comparing `sage_lib-0.1.4.8.tar` & `sage_lib-0.1.4.9.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxrwxr-x   0 akaris    (1000) akaris    (1000)        0 2024-02-23 07:32:08.000000 sage_lib-0.1.4.8/
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)        7 2023-11-24 15:31:44.000000 sage_lib-0.1.4.8/README.md
-drwxrwxr-x   0 akaris    (1000) akaris    (1000)        0 2024-02-23 07:32:08.000000 sage_lib-0.1.4.8/sage_lib.egg-info/
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)       45 2024-02-23 07:32:08.000000 sage_lib-0.1.4.8/sage_lib.egg-info/entry_points.txt
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)       23 2024-02-23 07:32:08.000000 sage_lib-0.1.4.8/sage_lib.egg-info/requires.txt
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)        9 2024-02-23 07:32:08.000000 sage_lib-0.1.4.8/sage_lib.egg-info/top_level.txt
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)      184 2024-02-23 07:32:08.000000 sage_lib-0.1.4.8/sage_lib.egg-info/PKG-INFO
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)        1 2024-02-23 07:32:08.000000 sage_lib-0.1.4.8/sage_lib.egg-info/dependency_links.txt
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     3569 2024-02-23 07:32:08.000000 sage_lib-0.1.4.8/sage_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 akaris    (1000) akaris    (1000)       38 2024-02-23 07:32:08.000000 sage_lib-0.1.4.8/setup.cfg
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)      394 2024-02-23 07:32:02.000000 sage_lib-0.1.4.8/setup.py
--rw-rw-r--   0 akaris    (1000) akaris    (1000)      184 2024-02-23 07:32:08.000000 sage_lib-0.1.4.8/PKG-INFO
-drwxrwxr-x   0 akaris    (1000) akaris    (1000)        0 2024-02-23 07:32:08.000000 sage_lib-0.1.4.8/sage_lib/
-drwxrwxr-x   0 akaris    (1000) akaris    (1000)        0 2024-02-23 07:32:08.000000 sage_lib-0.1.4.8/sage_lib/descriptor/
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.4.8/sage_lib/descriptor/__init__.py
--rw-rw-r--   0 akaris    (1000) akaris    (1000)    22605 2024-01-30 14:35:03.000000 sage_lib-0.1.4.8/sage_lib/descriptor/MBTR.py
--rw-rw-r--   0 akaris    (1000) akaris    (1000)    12332 2024-01-26 13:40:44.000000 sage_lib-0.1.4.8/sage_lib/descriptor/MDTR_rev.py
-drwxrwxr-x   0 akaris    (1000) akaris    (1000)        0 2024-02-23 07:32:08.000000 sage_lib-0.1.4.8/sage_lib/IO/
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     9400 2023-11-30 16:58:50.000000 sage_lib-0.1.4.8/sage_lib/IO/EigenvalueFileManager.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.4.8/sage_lib/IO/__init__.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     8862 2023-11-30 09:14:10.000000 sage_lib-0.1.4.8/sage_lib/IO/KPointsManager.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)    16921 2024-01-17 11:53:21.000000 sage_lib-0.1.4.8/sage_lib/IO/OutFileManager.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     6402 2023-11-30 08:47:00.000000 sage_lib-0.1.4.8/sage_lib/IO/DOSManager.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     8151 2023-11-26 10:16:36.000000 sage_lib-0.1.4.8/sage_lib/IO/PotentialManager.py
-drwxrwxr-x   0 akaris    (1000) akaris    (1000)        0 2024-02-23 07:32:08.000000 sage_lib-0.1.4.8/sage_lib/IO/input_handling_tools/
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)    24368 2024-01-17 11:45:39.000000 sage_lib-0.1.4.8/sage_lib/IO/input_handling_tools/InputDFT.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.4.8/sage_lib/IO/input_handling_tools/__init__.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)      609 2024-01-17 11:45:45.000000 sage_lib-0.1.4.8/sage_lib/IO/input_handling_tools/InputClassic.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)      873 2023-11-26 10:17:02.000000 sage_lib-0.1.4.8/sage_lib/IO/input_handling_tools/InputFileManager.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     1168 2024-01-17 11:45:21.000000 sage_lib-0.1.4.8/sage_lib/IO/input_handling_tools/InputFile.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     4088 2023-11-26 10:15:54.000000 sage_lib-0.1.4.8/sage_lib/IO/BinaryDataHandler.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     5292 2023-11-26 10:15:38.000000 sage_lib-0.1.4.8/sage_lib/IO/PROFileManager.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     2756 2023-11-26 10:15:40.000000 sage_lib-0.1.4.8/sage_lib/IO/WaveFileManager.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     5213 2023-11-26 10:15:10.000000 sage_lib-0.1.4.8/sage_lib/IO/BashScriptManager.py
-drwxrwxr-x   0 akaris    (1000) akaris    (1000)        0 2024-02-23 07:32:08.000000 sage_lib-0.1.4.8/sage_lib/IO/structure_handling_tools/
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)    31331 2024-01-31 13:09:07.000000 sage_lib-0.1.4.8/sage_lib/IO/structure_handling_tools/PeriodicSystem.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.4.8/sage_lib/IO/structure_handling_tools/__init__.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     5924 2023-12-29 02:33:08.000000 sage_lib-0.1.4.8/sage_lib/IO/structure_handling_tools/AtomPositionMaker.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)    39615 2024-02-21 11:50:51.000000 sage_lib-0.1.4.8/sage_lib/IO/structure_handling_tools/AtomPositionOperator.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)    21000 2024-01-30 15:53:32.000000 sage_lib-0.1.4.8/sage_lib/IO/structure_handling_tools/AtomPositionManager.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     2622 2024-01-17 11:44:29.000000 sage_lib-0.1.4.8/sage_lib/IO/structure_handling_tools/AtomPosition.py
-drwxrwxr-x   0 akaris    (1000) akaris    (1000)        0 2024-02-23 07:32:08.000000 sage_lib-0.1.4.8/sage_lib/IO/structure_handling_tools/structural_file_readers/
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.4.8/sage_lib/IO/structure_handling_tools/structural_file_readers/__init__.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     4854 2024-01-17 15:22:16.000000 sage_lib-0.1.4.8/sage_lib/IO/structure_handling_tools/structural_file_readers/POSCAR.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     3458 2023-11-28 08:43:18.000000 sage_lib-0.1.4.8/sage_lib/IO/structure_handling_tools/structural_file_readers/CIF.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     2583 2023-11-28 07:46:02.000000 sage_lib-0.1.4.8/sage_lib/IO/structure_handling_tools/structural_file_readers/SI.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     8624 2024-02-08 11:15:50.000000 sage_lib-0.1.4.8/sage_lib/IO/structure_handling_tools/structural_file_readers/PDB.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)    10470 2024-02-09 13:45:47.000000 sage_lib-0.1.4.8/sage_lib/IO/structure_handling_tools/structural_file_readers/XYZ.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     5733 2023-12-12 15:25:04.000000 sage_lib-0.1.4.8/sage_lib/IO/structure_handling_tools/structural_file_readers/AIMS.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     6036 2024-01-17 16:13:47.000000 sage_lib-0.1.4.8/sage_lib/IO/structure_handling_tools/structural_file_readers/GEN.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     4702 2023-12-18 08:26:38.000000 sage_lib-0.1.4.8/sage_lib/IO/structure_handling_tools/structural_file_readers/ASE.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)      666 2024-01-30 15:22:44.000000 sage_lib-0.1.4.8/sage_lib/IO/structure_handling_tools/NonPeriodicSystem.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)    10187 2024-01-25 08:34:17.000000 sage_lib-0.1.4.8/sage_lib/IO/structure_handling_tools/plot.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     4991 2024-01-17 15:22:15.000000 sage_lib-0.1.4.8/sage_lib/IO/structure_handling_tools/AtomPositionLoader.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)      559 2023-11-26 11:22:04.000000 sage_lib-0.1.4.8/sage_lib/IO/ForceFieldManager.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     3145 2023-11-26 10:15:38.000000 sage_lib-0.1.4.8/sage_lib/IO/ChargeFileManager.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     5409 2024-01-17 14:07:15.000000 sage_lib-0.1.4.8/sage_lib/__init__.py
-drwxrwxr-x   0 akaris    (1000) akaris    (1000)        0 2024-02-23 07:32:08.000000 sage_lib-0.1.4.8/sage_lib/single_run/
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.4.8/sage_lib/single_run/__init__.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     1803 2024-01-17 15:01:44.000000 sage_lib-0.1.4.8/sage_lib/single_run/SingleRun.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     6596 2023-11-24 15:31:44.000000 sage_lib-0.1.4.8/sage_lib/single_run/FF_Gap.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)    14547 2024-01-17 14:56:21.000000 sage_lib-0.1.4.8/sage_lib/single_run/SingleRunDFT.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     3098 2024-01-17 14:12:18.000000 sage_lib-0.1.4.8/sage_lib/single_run/SingleRunManager.py
-drwxrwxr-x   0 akaris    (1000) akaris    (1000)        0 2024-02-23 07:32:08.000000 sage_lib-0.1.4.8/sage_lib/ensemble/
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.4.8/sage_lib/ensemble/__init__.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     1943 2023-11-30 08:04:04.000000 sage_lib-0.1.4.8/sage_lib/ensemble/FFEnsembleManager.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)      723 2023-11-30 08:05:18.000000 sage_lib-0.1.4.8/sage_lib/ensemble/DFTEnsemble.py
-drwxrwxr-x   0 akaris    (1000) akaris    (1000)        0 2024-02-23 07:32:08.000000 sage_lib-0.1.4.8/sage_lib/master/
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)    12789 2024-01-17 14:49:37.000000 sage_lib-0.1.4.8/sage_lib/master/FileManager.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.4.8/sage_lib/master/__init__.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)    53348 2024-01-26 15:57:17.000000 sage_lib-0.1.4.8/sage_lib/master/AtomicProperties.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)    54394 2024-02-23 07:15:35.000000 sage_lib-0.1.4.8/sage_lib/main.py
-drwxrwxr-x   0 akaris    (1000) akaris    (1000)        0 2024-02-23 07:32:08.000000 sage_lib-0.1.4.8/sage_lib/miscellaneous/
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.4.8/sage_lib/miscellaneous/__init__.py
--rw-rw-r--   0 akaris    (1000) akaris    (1000)    22279 2024-01-31 09:07:23.000000 sage_lib-0.1.4.8/sage_lib/miscellaneous/periodic_kdtree.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     7176 2024-01-17 14:09:09.000000 sage_lib-0.1.4.8/sage_lib/miscellaneous/BandPathGenerator.py
-drwxrwxr-x   0 akaris    (1000) akaris    (1000)        0 2024-02-23 07:32:08.000000 sage_lib-0.1.4.8/sage_lib/partition/
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.4.8/sage_lib/partition/__init__.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)    14943 2024-02-23 07:14:36.000000 sage_lib-0.1.4.8/sage_lib/partition/Partition.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)    22631 2024-02-09 08:58:32.000000 sage_lib-0.1.4.8/sage_lib/partition/PartitionManager.py
-drwxrwxr-x   0 akaris    (1000) akaris    (1000)        0 2024-02-23 07:32:08.000000 sage_lib-0.1.4.8/sage_lib/partition/partition_builder/
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)    12099 2024-01-31 09:40:59.000000 sage_lib-0.1.4.8/sage_lib/partition/partition_builder/MoleculeCluster_builder.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     6296 2024-02-23 07:14:15.000000 sage_lib-0.1.4.8/sage_lib/partition/partition_builder/VacuumStates_builder.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)      614 2023-11-26 10:15:36.000000 sage_lib-0.1.4.8/sage_lib/partition/partition_builder/Crystal_builder.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.4.8/sage_lib/partition/partition_builder/__init__.py
--rw-rw-r--   0 akaris    (1000) akaris    (1000)     7160 2024-02-21 16:05:45.000000 sage_lib-0.1.4.8/sage_lib/partition/partition_builder/AbInitioThermodynamics_builder.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     5375 2023-11-26 12:34:42.000000 sage_lib-0.1.4.8/sage_lib/partition/partition_builder/SurfaceStates_builder.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)    11331 2024-01-17 14:16:35.000000 sage_lib-0.1.4.8/sage_lib/partition/partition_builder/SupercellEmbedding_builder.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)    13697 2024-02-09 12:26:14.000000 sage_lib-0.1.4.8/sage_lib/partition/partition_builder/Filter_builder.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     6705 2023-12-26 16:23:08.000000 sage_lib-0.1.4.8/sage_lib/partition/partition_builder/Config_builder.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     2503 2023-11-26 11:03:08.000000 sage_lib-0.1.4.8/sage_lib/partition/partition_builder/BandStructure_builder.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     3749 2024-01-17 14:10:13.000000 sage_lib-0.1.4.8/sage_lib/partition/partition_builder/ForceField_builder.py
--rw-rw-r--   0 akaris    (1000) akaris    (1000)    34641 2024-02-21 16:01:38.000000 sage_lib-0.1.4.8/sage_lib/partition/partition_builder/MolecularDynamic_builder.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     2873 2024-01-30 12:38:27.000000 sage_lib-0.1.4.8/sage_lib/partition/partition_builder/PositionEditor_builder.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)     3669 2024-01-17 14:10:13.000000 sage_lib-0.1.4.8/sage_lib/partition/partition_builder/Molecule_builder.py
--rwxr-xr-x   0 akaris    (1000) akaris    (1000)    11764 2024-01-30 14:29:29.000000 sage_lib-0.1.4.8/sage_lib/partition/partition_builder/CrystalDefect_builder.py
+drwxrwxr-x   0 akaris    (1000) akaris    (1000)        0 2024-02-29 10:29:26.000000 sage_lib-0.1.4.9/
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)        7 2023-11-24 15:31:44.000000 sage_lib-0.1.4.9/README.md
+drwxrwxr-x   0 akaris    (1000) akaris    (1000)        0 2024-02-29 10:29:26.000000 sage_lib-0.1.4.9/sage_lib.egg-info/
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)       45 2024-02-29 10:29:26.000000 sage_lib-0.1.4.9/sage_lib.egg-info/entry_points.txt
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)       23 2024-02-29 10:29:26.000000 sage_lib-0.1.4.9/sage_lib.egg-info/requires.txt
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)        9 2024-02-29 10:29:26.000000 sage_lib-0.1.4.9/sage_lib.egg-info/top_level.txt
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)      184 2024-02-29 10:29:26.000000 sage_lib-0.1.4.9/sage_lib.egg-info/PKG-INFO
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)        1 2024-02-29 10:29:26.000000 sage_lib-0.1.4.9/sage_lib.egg-info/dependency_links.txt
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)     3566 2024-02-29 10:29:26.000000 sage_lib-0.1.4.9/sage_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 akaris    (1000) akaris    (1000)       38 2024-02-29 10:29:26.000000 sage_lib-0.1.4.9/setup.cfg
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)      394 2024-02-29 10:29:01.000000 sage_lib-0.1.4.9/setup.py
+-rw-rw-r--   0 akaris    (1000) akaris    (1000)      184 2024-02-29 10:29:26.000000 sage_lib-0.1.4.9/PKG-INFO
+drwxrwxr-x   0 akaris    (1000) akaris    (1000)        0 2024-02-29 10:29:26.000000 sage_lib-0.1.4.9/sage_lib/
+drwxrwxr-x   0 akaris    (1000) akaris    (1000)        0 2024-02-29 10:29:26.000000 sage_lib-0.1.4.9/sage_lib/descriptor/
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.4.9/sage_lib/descriptor/__init__.py
+-rw-rw-r--   0 akaris    (1000) akaris    (1000)    22605 2024-01-30 14:35:03.000000 sage_lib-0.1.4.9/sage_lib/descriptor/MBTR.py
+-rw-rw-r--   0 akaris    (1000) akaris    (1000)    12332 2024-01-26 13:40:44.000000 sage_lib-0.1.4.9/sage_lib/descriptor/MDTR_rev.py
+drwxrwxr-x   0 akaris    (1000) akaris    (1000)        0 2024-02-29 10:29:26.000000 sage_lib-0.1.4.9/sage_lib/IO/
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)     9400 2023-11-30 16:58:50.000000 sage_lib-0.1.4.9/sage_lib/IO/EigenvalueFileManager.py
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.4.9/sage_lib/IO/__init__.py
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)     8862 2023-11-30 09:14:10.000000 sage_lib-0.1.4.9/sage_lib/IO/KPointsManager.py
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)    16921 2024-01-17 11:53:21.000000 sage_lib-0.1.4.9/sage_lib/IO/OutFileManager.py
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)     6402 2023-11-30 08:47:00.000000 sage_lib-0.1.4.9/sage_lib/IO/DOSManager.py
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)     8151 2023-11-26 10:16:36.000000 sage_lib-0.1.4.9/sage_lib/IO/PotentialManager.py
+drwxrwxr-x   0 akaris    (1000) akaris    (1000)        0 2024-02-29 10:29:26.000000 sage_lib-0.1.4.9/sage_lib/IO/input_handling_tools/
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)    24368 2024-01-17 11:45:39.000000 sage_lib-0.1.4.9/sage_lib/IO/input_handling_tools/InputDFT.py
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.4.9/sage_lib/IO/input_handling_tools/__init__.py
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)      609 2024-01-17 11:45:45.000000 sage_lib-0.1.4.9/sage_lib/IO/input_handling_tools/InputClassic.py
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)      873 2023-11-26 10:17:02.000000 sage_lib-0.1.4.9/sage_lib/IO/input_handling_tools/InputFileManager.py
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)     1168 2024-01-17 11:45:21.000000 sage_lib-0.1.4.9/sage_lib/IO/input_handling_tools/InputFile.py
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)     4088 2023-11-26 10:15:54.000000 sage_lib-0.1.4.9/sage_lib/IO/BinaryDataHandler.py
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)     5292 2023-11-26 10:15:38.000000 sage_lib-0.1.4.9/sage_lib/IO/PROFileManager.py
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)     2756 2023-11-26 10:15:40.000000 sage_lib-0.1.4.9/sage_lib/IO/WaveFileManager.py
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)     5213 2023-11-26 10:15:10.000000 sage_lib-0.1.4.9/sage_lib/IO/BashScriptManager.py
+drwxrwxr-x   0 akaris    (1000) akaris    (1000)        0 2024-02-29 10:29:26.000000 sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)    31331 2024-01-31 13:09:07.000000 sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/PeriodicSystem.py
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/__init__.py
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)     5924 2023-12-29 02:33:08.000000 sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/AtomPositionMaker.py
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)    39615 2024-02-28 10:38:59.000000 sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/AtomPositionOperator.py
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)    21127 2024-02-27 16:53:39.000000 sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/AtomPositionManager.py
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)     2622 2024-01-17 11:44:29.000000 sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/AtomPosition.py
+drwxrwxr-x   0 akaris    (1000) akaris    (1000)        0 2024-02-29 10:29:26.000000 sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/structural_file_readers/
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/structural_file_readers/__init__.py
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)     4854 2024-01-17 15:22:16.000000 sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/structural_file_readers/POSCAR.py
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)     3458 2023-11-28 08:43:18.000000 sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/structural_file_readers/CIF.py
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)     2583 2023-11-28 07:46:02.000000 sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/structural_file_readers/SI.py
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)     8624 2024-02-08 11:15:50.000000 sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/structural_file_readers/PDB.py
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)    10566 2024-02-27 17:11:40.000000 sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/structural_file_readers/XYZ.py
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)     5733 2023-12-12 15:25:04.000000 sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/structural_file_readers/AIMS.py
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)     6036 2024-01-17 16:13:47.000000 sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/structural_file_readers/GEN.py
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)     4702 2023-12-18 08:26:38.000000 sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/structural_file_readers/ASE.py
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)      666 2024-01-30 15:22:44.000000 sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/NonPeriodicSystem.py
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)    10187 2024-01-25 08:34:17.000000 sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/plot.py
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)     4991 2024-01-17 15:22:15.000000 sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/AtomPositionLoader.py
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)      559 2023-11-26 11:22:04.000000 sage_lib-0.1.4.9/sage_lib/IO/ForceFieldManager.py
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)     3145 2023-11-26 10:15:38.000000 sage_lib-0.1.4.9/sage_lib/IO/ChargeFileManager.py
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)     5409 2024-01-17 14:07:15.000000 sage_lib-0.1.4.9/sage_lib/__init__.py
+drwxrwxr-x   0 akaris    (1000) akaris    (1000)        0 2024-02-29 10:29:26.000000 sage_lib-0.1.4.9/sage_lib/single_run/
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.4.9/sage_lib/single_run/__init__.py
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)     1803 2024-01-17 15:01:44.000000 sage_lib-0.1.4.9/sage_lib/single_run/SingleRun.py
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)     6596 2023-11-24 15:31:44.000000 sage_lib-0.1.4.9/sage_lib/single_run/FF_Gap.py
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)    14547 2024-01-17 14:56:21.000000 sage_lib-0.1.4.9/sage_lib/single_run/SingleRunDFT.py
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)     3098 2024-01-17 14:12:18.000000 sage_lib-0.1.4.9/sage_lib/single_run/SingleRunManager.py
+drwxrwxr-x   0 akaris    (1000) akaris    (1000)        0 2024-02-29 10:29:26.000000 sage_lib-0.1.4.9/sage_lib/ensemble/
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.4.9/sage_lib/ensemble/__init__.py
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)     1943 2023-11-30 08:04:04.000000 sage_lib-0.1.4.9/sage_lib/ensemble/FFEnsembleManager.py
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)      723 2023-11-30 08:05:18.000000 sage_lib-0.1.4.9/sage_lib/ensemble/DFTEnsemble.py
+drwxrwxr-x   0 akaris    (1000) akaris    (1000)        0 2024-02-29 10:29:26.000000 sage_lib-0.1.4.9/sage_lib/master/
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)    12789 2024-01-17 14:49:37.000000 sage_lib-0.1.4.9/sage_lib/master/FileManager.py
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.4.9/sage_lib/master/__init__.py
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)    53348 2024-01-26 15:57:17.000000 sage_lib-0.1.4.9/sage_lib/master/AtomicProperties.py
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)    56357 2024-02-28 10:38:17.000000 sage_lib-0.1.4.9/sage_lib/main.py
+drwxrwxr-x   0 akaris    (1000) akaris    (1000)        0 2024-02-29 10:29:26.000000 sage_lib-0.1.4.9/sage_lib/miscellaneous/
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.4.9/sage_lib/miscellaneous/__init__.py
+-rw-rw-r--   0 akaris    (1000) akaris    (1000)    22279 2024-01-31 09:07:23.000000 sage_lib-0.1.4.9/sage_lib/miscellaneous/periodic_kdtree.py
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)     7176 2024-01-17 14:09:09.000000 sage_lib-0.1.4.9/sage_lib/miscellaneous/BandPathGenerator.py
+drwxrwxr-x   0 akaris    (1000) akaris    (1000)        0 2024-02-29 10:29:26.000000 sage_lib-0.1.4.9/sage_lib/partition/
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.4.9/sage_lib/partition/__init__.py
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)    14976 2024-02-27 15:30:04.000000 sage_lib-0.1.4.9/sage_lib/partition/Partition.py
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)    22631 2024-02-28 09:20:51.000000 sage_lib-0.1.4.9/sage_lib/partition/PartitionManager.py
+drwxrwxr-x   0 akaris    (1000) akaris    (1000)        0 2024-02-29 10:29:26.000000 sage_lib-0.1.4.9/sage_lib/partition/partition_builder/
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)    12099 2024-01-31 09:40:59.000000 sage_lib-0.1.4.9/sage_lib/partition/partition_builder/MoleculeCluster_builder.py
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)     6358 2024-02-23 08:00:39.000000 sage_lib-0.1.4.9/sage_lib/partition/partition_builder/VacuumStates_builder.py
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)      614 2023-11-26 10:15:36.000000 sage_lib-0.1.4.9/sage_lib/partition/partition_builder/Crystal_builder.py
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)        0 2023-11-30 08:10:48.000000 sage_lib-0.1.4.9/sage_lib/partition/partition_builder/__init__.py
+-rw-rw-r--   0 akaris    (1000) akaris    (1000)     7189 2024-02-23 12:29:06.000000 sage_lib-0.1.4.9/sage_lib/partition/partition_builder/AbInitioThermodynamics_builder.py
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)     5375 2023-11-26 12:34:42.000000 sage_lib-0.1.4.9/sage_lib/partition/partition_builder/SurfaceStates_builder.py
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)    11331 2024-01-17 14:16:35.000000 sage_lib-0.1.4.9/sage_lib/partition/partition_builder/SupercellEmbedding_builder.py
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)    14023 2024-02-28 09:01:31.000000 sage_lib-0.1.4.9/sage_lib/partition/partition_builder/Filter_builder.py
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)     6705 2023-12-26 16:23:08.000000 sage_lib-0.1.4.9/sage_lib/partition/partition_builder/Config_builder.py
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)     2503 2023-11-26 11:03:08.000000 sage_lib-0.1.4.9/sage_lib/partition/partition_builder/BandStructure_builder.py
+-rw-rw-r--   0 akaris    (1000) akaris    (1000)    35959 2024-02-28 10:59:55.000000 sage_lib-0.1.4.9/sage_lib/partition/partition_builder/MolecularDynamic_builder.py
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)     2873 2024-01-30 12:38:27.000000 sage_lib-0.1.4.9/sage_lib/partition/partition_builder/PositionEditor_builder.py
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)     3669 2024-01-17 14:10:13.000000 sage_lib-0.1.4.9/sage_lib/partition/partition_builder/Molecule_builder.py
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)     2714 2024-02-28 10:50:31.000000 sage_lib-0.1.4.9/sage_lib/partition/partition_builder/Dataset_builder.py
+-rwxr-xr-x   0 akaris    (1000) akaris    (1000)    11764 2024-01-30 14:29:29.000000 sage_lib-0.1.4.9/sage_lib/partition/partition_builder/CrystalDefect_builder.py
```

### Comparing `sage_lib-0.1.4.8/sage_lib.egg-info/SOURCES.txt` & `sage_lib-0.1.4.9/sage_lib.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -59,16 +59,16 @@
 sage_lib/partition/PartitionManager.py
 sage_lib/partition/__init__.py
 sage_lib/partition/partition_builder/AbInitioThermodynamics_builder.py
 sage_lib/partition/partition_builder/BandStructure_builder.py
 sage_lib/partition/partition_builder/Config_builder.py
 sage_lib/partition/partition_builder/CrystalDefect_builder.py
 sage_lib/partition/partition_builder/Crystal_builder.py
+sage_lib/partition/partition_builder/Dataset_builder.py
 sage_lib/partition/partition_builder/Filter_builder.py
-sage_lib/partition/partition_builder/ForceField_builder.py
 sage_lib/partition/partition_builder/MolecularDynamic_builder.py
 sage_lib/partition/partition_builder/MoleculeCluster_builder.py
 sage_lib/partition/partition_builder/Molecule_builder.py
 sage_lib/partition/partition_builder/PositionEditor_builder.py
 sage_lib/partition/partition_builder/SupercellEmbedding_builder.py
 sage_lib/partition/partition_builder/SurfaceStates_builder.py
 sage_lib/partition/partition_builder/VacuumStates_builder.py
```

### Comparing `sage_lib-0.1.4.8/sage_lib/descriptor/MBTR.py` & `sage_lib-0.1.4.9/sage_lib/descriptor/MBTR.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.8/sage_lib/descriptor/MDTR_rev.py` & `sage_lib-0.1.4.9/sage_lib/descriptor/MDTR_rev.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.8/sage_lib/IO/EigenvalueFileManager.py` & `sage_lib-0.1.4.9/sage_lib/IO/EigenvalueFileManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.8/sage_lib/IO/KPointsManager.py` & `sage_lib-0.1.4.9/sage_lib/IO/KPointsManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.8/sage_lib/IO/OutFileManager.py` & `sage_lib-0.1.4.9/sage_lib/IO/OutFileManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.8/sage_lib/IO/DOSManager.py` & `sage_lib-0.1.4.9/sage_lib/IO/DOSManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.8/sage_lib/IO/PotentialManager.py` & `sage_lib-0.1.4.9/sage_lib/IO/PotentialManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.8/sage_lib/IO/input_handling_tools/InputDFT.py` & `sage_lib-0.1.4.9/sage_lib/IO/input_handling_tools/InputDFT.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.8/sage_lib/IO/input_handling_tools/InputClassic.py` & `sage_lib-0.1.4.9/sage_lib/IO/input_handling_tools/InputClassic.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.8/sage_lib/IO/input_handling_tools/InputFileManager.py` & `sage_lib-0.1.4.9/sage_lib/IO/input_handling_tools/InputFileManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.8/sage_lib/IO/input_handling_tools/InputFile.py` & `sage_lib-0.1.4.9/sage_lib/IO/input_handling_tools/InputFile.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.8/sage_lib/IO/BinaryDataHandler.py` & `sage_lib-0.1.4.9/sage_lib/IO/BinaryDataHandler.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.8/sage_lib/IO/PROFileManager.py` & `sage_lib-0.1.4.9/sage_lib/IO/PROFileManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.8/sage_lib/IO/WaveFileManager.py` & `sage_lib-0.1.4.9/sage_lib/IO/WaveFileManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.8/sage_lib/IO/BashScriptManager.py` & `sage_lib-0.1.4.9/sage_lib/IO/BashScriptManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.8/sage_lib/IO/structure_handling_tools/PeriodicSystem.py` & `sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/PeriodicSystem.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.8/sage_lib/IO/structure_handling_tools/AtomPositionMaker.py` & `sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/AtomPositionMaker.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.8/sage_lib/IO/structure_handling_tools/AtomPositionOperator.py` & `sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/AtomPositionOperator.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.8/sage_lib/IO/structure_handling_tools/AtomPositionManager.py` & `sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/AtomPositionManager.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,16 +167,20 @@
         # == == Molecular / atomistic representations == == #
         self._MBTR = None
         self._MBTR_representation, self._MBTR_representation_dev = None, None
         self._graph_representation, self._similarity_matrix = None, None
 
         # Properties related to atomic calculations
         self._total_charge = None  # Total charge. Type: float or None
+        self._charge = None  # charge. Type: float or None
+
         self._magnetization = None  # Magnetization. Type: float or None
         self._total_force = None  # Total force. Type: np.array or None
+        self._force = None  # Total force. Type: np.array or None
+
         self._E = None  # Total energy. Type: float or None
         self._Edisp = None  # Dispersion energy. Type: float or None
         self._IRdisplacement = None  # IR displacement. Type: np.array or None
 
         self._mass = None # 
         self._mass_list = None #
```

### Comparing `sage_lib-0.1.4.8/sage_lib/IO/structure_handling_tools/AtomPosition.py` & `sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/AtomPosition.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.8/sage_lib/IO/structure_handling_tools/structural_file_readers/POSCAR.py` & `sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/structural_file_readers/POSCAR.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.8/sage_lib/IO/structure_handling_tools/structural_file_readers/CIF.py` & `sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/structural_file_readers/CIF.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.8/sage_lib/IO/structure_handling_tools/structural_file_readers/SI.py` & `sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/structural_file_readers/SI.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.8/sage_lib/IO/structure_handling_tools/structural_file_readers/PDB.py` & `sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/structural_file_readers/PDB.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.8/sage_lib/IO/structure_handling_tools/structural_file_readers/XYZ.py` & `sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/structural_file_readers/XYZ.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         energy = hasattr(self, 'E') and energy and self.E is not None and energy
         pbc = hasattr(self, 'latticeVectors') and self.latticeVectors is not None and pbc
         time = hasattr(self, 'time') and self.time is not None and time 
 
         # Constructing the header information dynamically
         properties_list = [
             f'Lattice="{ " ".join(map(str, self.latticeVectors.flatten())) }"' if lattice else '',
-            f'Properties={":".join(filter(None, [f"species:S:1" if species else "", f"{position_tag}:R:3" if position else "", f"{forces_tag}:R:3" if forces else "", f"{charge_tag}:R:3" if charge else "", f"{magnetization_tag}:R:3" if magnetization else ""]))}',
+            f'Properties={":".join(filter(None, [f"species:S:1" if species else "", f"{position_tag}:R:3" if position else "", f"{forces_tag}:R:3" if forces else "", f"{charge_tag}:R:{self.charge.shape[1]}" if charge else "", f"{magnetization_tag}:R:{self.magnetization.shape[1]}" if magnetization else ""]))}',
             f'{energy_tag}={self.E}' if energy else '',
             f'{pbc_tag}="T T T"' if pbc else '',
             f'{time_tag}={self.time}' if time else ''
         ]
         properties_str = ' '.join(filter(None, properties_list))
 
         # Preparing atom data lines
@@ -95,15 +95,16 @@
 
         Returns:
             bool: True if the file is successfully read and parsed, False otherwise.
         """ 
 
         # Default tags for properties if not provided
         default_tags = {
-            'energy': 'E',
+            'energy': 'energy',
+            'E': 'E',
             'mass': 'masses',
             'forces': 'forces',
             'position': 'pos',
             'species': 'species',
             'pbc': 'pbc',
             'time': 'time',
             'Lattice': 'Lattice',
@@ -170,15 +171,15 @@
         if key == tags['Lattice']:
             self._latticeVectors = np.array([[float(value[1:-1].strip().split()[i * 3 + j]) for j in range(3)] for i in range(3)])
             self._atomCoordinateType = 'C'
 
         elif key == tags['Properties']:
             self._parse_properties(value, body, dtype_map, property_to_attr)
 
-        elif key == tags['energy']:
+        elif key == tags['energy'] or key == tags['E']:
             self._E = float(value)
 
         elif key == tags['pbc']:
             self._pbc = ['T' in v for v in value.split()]
 
         elif key == tags['time']:
             self._time = float(value)
```

### Comparing `sage_lib-0.1.4.8/sage_lib/IO/structure_handling_tools/structural_file_readers/AIMS.py` & `sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/structural_file_readers/AIMS.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.8/sage_lib/IO/structure_handling_tools/structural_file_readers/GEN.py` & `sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/structural_file_readers/GEN.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.8/sage_lib/IO/structure_handling_tools/structural_file_readers/ASE.py` & `sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/structural_file_readers/ASE.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.8/sage_lib/IO/structure_handling_tools/NonPeriodicSystem.py` & `sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/NonPeriodicSystem.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.8/sage_lib/IO/structure_handling_tools/plot.py` & `sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/plot.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.8/sage_lib/IO/structure_handling_tools/AtomPositionLoader.py` & `sage_lib-0.1.4.9/sage_lib/IO/structure_handling_tools/AtomPositionLoader.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.8/sage_lib/IO/ForceFieldManager.py` & `sage_lib-0.1.4.9/sage_lib/IO/ForceFieldManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.8/sage_lib/IO/ChargeFileManager.py` & `sage_lib-0.1.4.9/sage_lib/IO/ChargeFileManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.8/sage_lib/__init__.py` & `sage_lib-0.1.4.9/sage_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.8/sage_lib/single_run/SingleRun.py` & `sage_lib-0.1.4.9/sage_lib/single_run/SingleRun.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.8/sage_lib/single_run/FF_Gap.py` & `sage_lib-0.1.4.9/sage_lib/single_run/FF_Gap.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.8/sage_lib/single_run/SingleRunDFT.py` & `sage_lib-0.1.4.9/sage_lib/single_run/SingleRunDFT.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.8/sage_lib/single_run/SingleRunManager.py` & `sage_lib-0.1.4.9/sage_lib/single_run/SingleRunManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.8/sage_lib/ensemble/FFEnsembleManager.py` & `sage_lib-0.1.4.9/sage_lib/ensemble/FFEnsembleManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.8/sage_lib/ensemble/DFTEnsemble.py` & `sage_lib-0.1.4.9/sage_lib/ensemble/DFTEnsemble.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.8/sage_lib/master/FileManager.py` & `sage_lib-0.1.4.9/sage_lib/master/FileManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.8/sage_lib/master/AtomicProperties.py` & `sage_lib-0.1.4.9/sage_lib/master/AtomicProperties.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.8/sage_lib/main.py` & `sage_lib-0.1.4.9/sage_lib/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -260,15 +260,15 @@
             for conteiner_index, conteiner in enumerate(PT.containers):
                 file_location = output_path+f'/frame{conteiner_index}'
                 PT.create_directories_for_path(file_location)
                 conteiner.AtomPositionManager.plot_RBF(periodic_image=0, cutoff=cutoff, number_of_bins=number_of_bins, output_path=file_location,
                                                         bin_volume_normalize=True, number_of_atoms_normalize=True, density_normalize=True)
 
 def generate_MD(path:str, source:str=None, subfolders:bool=False, forces_tag:str=None, energy_tag:str=None, output_path:str=None, 
-                    plot:str=None, reference:str=None, ff_energy_tag:str=None, ff_forces_tag:str=None,
+                    plot:str=None, reference:str=None, ff_energy_tag:str=None, ff_forces_tag:str=None, sigma:float=None,
                     verbose:bool=False, conteiner_index:int=None):
     """
     Generate plots from simulation data.
 
     This function processes simulation data and generates plots, such as band structure or molecular structures, based on the data and specified plot type.
 
     Parameters:
@@ -279,31 +279,35 @@
     plot (str, optional): Type of plot to generate (e.g., 'band').
     verbose (bool, optional): If True, provides detailed output during execution.
     fermi (float, optional): Fermi level energy, important for certain types of plots.
 
     Returns:
     None
     """
+    # 'count_species', 'displacements', 'RBF', 'evaluate_ff', 'bond_distance_tracking', 'molecule_formation_tracking'
     output_path = output_path if output_path is not None else '.'
     PT = Partition(path)
     PT.read_files( file_location=path, source=source, energy_tag=energy_tag, forces_tag=forces_tag, subfolders=subfolders, verbose=verbose)
-    if plot.upper() == 'COUNT':
-        PT.handleMDAnalysis( values= {'count':{'output_path':output_path, 'verbose':verbose} }  )
+    if plot.upper() == 'COUNT_SPECIES':
+        PT.handleMDAnalysis( values= {'COUNT_SPECIES':{'output_path':output_path, 'verbose':verbose} }  )
 
-    if plot.upper() == 'DISPLACEMENTS':
-        PT.handleMDAnalysis( values= {'displacements':{'reference':reference, 'verbose':verbose} }  )
+    elif plot.upper() == 'DISPLACEMENTS':
+        PT.handleMDAnalysis( values= {'DISPLACEMENTS':{'reference':reference, 'verbose':verbose} }  )
 
-    if plot.upper() == 'RBF':
+    elif plot.upper() == 'RBF':
         PT.handleMDAnalysis( values= {'RBF':{'output_path':output_path, 'verbose':verbose} }  )
 
-    if plot.upper() == 'EVALUATE_FF':
+    elif plot.upper() == 'EVALUATE_FF':
         PT.handleMDAnalysis( values= {'EVALUATE_FF':{'output_path':output_path, 'ff_energy_tag':ff_energy_tag, 'ff_forces_tag':ff_forces_tag, 'verbose':verbose} }  )
 
-    if plot.upper() == 'BOND_TRACKING':
-        PT.handleMDAnalysis( values= {'BOND_TRACKING':{'reference':reference,'output_path':output_path, 'verbose':verbose} }  )
+    elif plot.upper() == 'BOND_DISTANCE_TRACKING':
+        PT.handleMDAnalysis( values= {'BOND_DISTANCE_TRACKING':{'reference':reference, 'sigma':sigma, 'output_path':output_path, 'verbose':verbose} }  )
+    
+    elif plot.upper() == 'MOLECULE_FORMATION_TRACKING':
+        PT.handleMDAnalysis( values= {'MOLECULE_FORMATION_TRACKING':{'sigma':sigma, 'output_path':output_path, 'verbose':verbose} }  )
    
 def generate_AbInitioThermodynamics(path:str, source:str=None, subfolders:bool=False, forces_tag:str=None, energy_tag:str=None, output_path:str=None, 
                 plot:str=None, reference_ID:list=None, especie:str=None, mu_max:float=None, mu_min:float=None,
                 verbose:bool=False, conteiner_index:int=None):
     """
     .
     """
@@ -455,14 +459,30 @@
     PT.read_files(file_location=path, source=source, energy_tag=energy_tag, forces_tag=forces_tag, subfolders=subfolders, verbose=verbose)
     PT.filter_conteiners(filter_class=filter_class, container_property=container_property, filter_type=filter_type, 
                         value=value, traj=traj, selection_number=N, ID=ID, verbosity=verbose)
 
     # Export the filtered files
     PT.export_files(file_location=output_path, source=source, label='enumerate', verbose=verbose)
 
+def generate_dataset(path:str, source:str=None, forces_tag:str=None, energy_tag:str=None, subfolders:bool=False, output_path:str=None, output_source:str=None, verbose:bool=False, conteiner_index:int=None, 
+                    operation:str=None, ):
+    """
+    """
+    # Initialize the DFTPartition object
+    PT = Partition(path)
+
+    # Read files and apply filters
+    PT.read_files(file_location=path, source=source, energy_tag=energy_tag, forces_tag=forces_tag, subfolders=subfolders, verbose=verbose)
+    if operation.upper() == 'SORT':
+        PT.handleDataset( values= {'sort':{'verbose':verbose} }  )
+    print( [n.AtomPositionManager.E for n in PT.containers] )
+    # Export the filtered files
+    PT.export_files(file_location=output_path, source=source, label='enumerate', verbose=verbose)
+
+
 def generate_supercell_embedding(
                         unitcell_path:str=None,              unitcell_source:str=None, forces_tag:str=None, energy_tag:str=None,
                         relax_supercell_path:str=None,       relax_supercell_source:str=None, 
                         unrelax_supercell_path:str=None,     unrelax_supercell_source:str=None, 
                         output_path:str=None,                output_source:str=None, verbose:bool=False, ):
     """
     Generates a supercell embedding from given unitcell and supercell structures and exports the result.
@@ -637,16 +657,17 @@
     parser_plot.add_argument('--emax', type=float, help='Specifies the maximum energy (in eV) for the plot range. Similar to --emin, it allows focusing on a specific energy interval in the plot.')
     parser_plot.add_argument('--cutoff', type=float, default=6.0, help='Defines the cutoff distance (in Ångströms) for RBF plots. This parameter is crucial for determining the extent of spatial interactions to be considered in the plot.')
     parser_plot.add_argument('--number_of_bins', type=int, default=100, help='Sets the number of bins for the histogram in RBF plots. A higher number of bins can lead to finer details in the plot, but may also increase computational load.')
 
     # =========== MD analisis ===========
     parser_MD = subparsers.add_parser('MD', help='')
     add_arguments(parser_MD)
-    parser_MD.add_argument('--plot', type=str, required=True, choices=['count', 'displacements', 'RBF', 'evaluate_ff', 'bond_tracking'], help='')
+    parser_MD.add_argument('--plot', type=str, required=True, choices=['count_species', 'displacements', 'RBF', 'evaluate_ff', 'bond_distance_tracking', 'molecule_formation_tracking'], help='')
     parser_MD.add_argument('--specie', type=str, required=False, help='')
+    parser_MD.add_argument('--sigma', type=float, required=False, help=' bonda factor')
     parser_MD.add_argument('--reference', type=str, required=False, help='')
     parser_MD.add_argument('--ff-forces-tag', type=str, required=False, help='')
     parser_MD.add_argument('--ff-energy-tag', type=str, required=False, help='')
 
     # ========== Sub-command: edit_positions ===========
     parser_edit = subparsers.add_parser('edit_positions', help='Modify atomic positions in the input files, allowing operations like "rattling" to introduce small random displacements.')
     add_arguments(parser_edit)
@@ -670,21 +691,26 @@
     parser_edit_config.add_argument('--weights', type=float, nargs='+', required=False, help='')
     parser_edit_config.add_argument('--N', default=1, type=int, help='.')
 
     # ========== Sub-command: filter ===========
     parser_filter = subparsers.add_parser('filter', help='Apply filters to select specific data based on various criteria.')
     add_arguments(parser_filter)
     parser_filter.add_argument('--filter', choices=['random', 'flat_histogram', 'binary', 'index'], type=str, help='Type of filter to apply: random, flat_histogram, or binary.')
-    parser_filter.add_argument('--property', choices=['E', 'forces', 'has_ID', 'has_not_ID'], type=str, help='Property to use for filtering: Energy (E), forces, or atom IDs.')
+    parser_filter.add_argument('--property', choices=['E', 'E/N', 'forces', 'has_ID', 'has_not_ID'], type=str, help='Property to use for filtering: Energy (E), forces, or atom IDs.')
     parser_filter.add_argument('--type', choices=['max', 'min', 'equipartition', 'tail', 'uniform'], type=str, help='Filter type: max (maximum value) or min (minimum value).')
     parser_filter.add_argument('--value', type=float, required=False, help='Value to compare against for the filter.')
     parser_filter.add_argument('--ID', type=str, required=False, help='Atom ID for filtering, if applicable.')
     parser_filter.add_argument('--traj', default=False, action='store_true', help='Enable trajectory-based filtering.')
     parser_filter.add_argument('--N', default=1, type=float, help='Number of elements to select when filtering.')
 
+    # ========== Sub-command: dataset ===========
+    parser_dataset = subparsers.add_parser('dataset', help='Apply filters to select specific data based on various criteria.')
+    add_arguments(parser_dataset)
+    parser_dataset.add_argument('--operation', choices=['sort'], type=str, help='')
+
     # ========== Sub-command: supercell_embedding ===========
     parser_supercell_embedding = subparsers.add_parser('supercell_embedding', help='Embed a unit cell into a supercell for large-scale calculations or visualizations.')
     add_arguments(parser_supercell_embedding)
     parser_supercell_embedding.add_argument('--unitcell_path', type=str, default='.', help='Path to the unit cell file. (default: .)')
     parser_supercell_embedding.add_argument('--unitcell_source', type=str, choices=['VASP', 'OUTCAR', 'xyz', 'traj', 'cif', 'AIMS'], default='VASP', help='Source format of the unit cell file: VASP, OUTCAR, xyz, etc. (default: VASP)')
     parser_supercell_embedding.add_argument('--notrelax_supercell_path', type=str, default='.', help='Path to the non-relaxed supercell file.')
     parser_supercell_embedding.add_argument('--notrelax_supercell_source', type=str, choices=['VASP', 'OUTCAR', 'xyz', 'traj', 'cif', 'AIMS'], default='VASP', help='Source format of the non-relaxed supercell file.')
@@ -750,15 +776,15 @@
     elif args.command == 'plot':
         generate_plot(path=args.path, source=args.source, forces_tag=args.forces_tag, energy_tag=args.energy_tag, subfolders=args.subfolders, conteiner_index=args.conteiner_index,
             verbose=args.verbose, output_path=args.output_path, plot=args.plot, fermi=args.fermi,
             emin=args.emin, emax=args.emax, cutoff=args.cutoff, number_of_bins=args.number_of_bins)
 
     elif args.command == 'MD':
         generate_MD(path=args.path, source=args.source, forces_tag=args.forces_tag, energy_tag=args.energy_tag, subfolders=args.subfolders, conteiner_index=args.conteiner_index,
-            verbose=args.verbose, output_path=args.output_path, plot=args.plot, 
+            verbose=args.verbose, output_path=args.output_path, plot=args.plot,  sigma=args.sigma, 
             reference=args.reference, ff_energy_tag=args.ff_energy_tag, ff_forces_tag=args.ff_forces_tag)
 
     elif args.command == 'edit_positions':
         generate_edit_positions(path=args.path, source=args.source, forces_tag=args.forces_tag, energy_tag=args.energy_tag, subfolders=args.subfolders, verbose=args.verbose, 
             output_path=args.output_path, output_source=args.output_source, 
             edit=args.edit, std=args.std, N=args.N, direction=args.direction, repeat=args.repeat, compress_min=args.compress_min, compress_max=args.compress_max,
             init_index=args.init_index, mid_index=args.mid_index, end_index=args.end_index)
@@ -768,14 +794,18 @@
             output_path=args.output_path, output_source=args.output_source, 
             edit=args.edit, atom_ID=args.ID, new_atom_ID=args.new_ID, weights=args.weights, N=args.N )
 
     elif args.command == 'filter':
         generate_filter(path=args.path, source=args.source, forces_tag=args.forces_tag, energy_tag=args.energy_tag, subfolders=args.subfolders, verbose=args.verbose, output_path=args.output_path, output_source=args.output_source,
                 filter_class=args.filter, container_property=args.property, filter_type=args.type, value=args.value, traj=args.traj, N=args.N, ID=args.ID)
 
+    elif args.command == 'dataset':
+        generate_dataset(path=args.path, source=args.source, forces_tag=args.forces_tag, energy_tag=args.energy_tag, subfolders=args.subfolders, conteiner_index=args.conteiner_index,
+            verbose=args.verbose, output_path=args.output_path, operation=args.operation, )
+
     elif args.command == 'supercell_embedding':
         generate_supercell_embedding(
                         relax_supercell_path=args.path,     relax_supercell_source=args.source, forces_tag=args.forces_tag, energy_tag=args.energy_tag, 
                         unrelax_supercell_path=args.notrelax_supercell_path,   unrelax_supercell_source=args.notrelax_supercell_source, 
                         unitcell_path=args.unitcell_path,            unitcell_source=args.unitcell_source, 
                         output_path=args.output_path,       output_source=args.output_source,
                         verbose=args.verbose )
```

### Comparing `sage_lib-0.1.4.8/sage_lib/miscellaneous/periodic_kdtree.py` & `sage_lib-0.1.4.9/sage_lib/miscellaneous/periodic_kdtree.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.8/sage_lib/miscellaneous/BandPathGenerator.py` & `sage_lib-0.1.4.9/sage_lib/miscellaneous/BandPathGenerator.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.8/sage_lib/partition/Partition.py` & `sage_lib-0.1.4.9/sage_lib/partition/Partition.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,18 +23,18 @@
     from sage_lib.partition.partition_builder.CrystalDefect_builder import CrystalDefect_builder
 except ImportError as e:
     import sys
     sys.stderr.write(f"An error occurred while importing CrystalDefect_builder: {str(e)}\n")
     del sys
 
 try:
-    from sage_lib.partition.partition_builder.ForceField_builder import ForceField_builder
+    from sage_lib.partition.partition_builder.Dataset_builder import Dataset_builder
 except ImportError as e:
     import sys
-    sys.stderr.write(f"An error occurred while importing ForceField_builder: {str(e)}\n")
+    sys.stderr.write(f"An error occurred while importing Dataset_builder: {str(e)}\n")
     del sys
 
 try:
     from sage_lib.partition.partition_builder.Molecule_builder import Molecule_builder
 except ImportError as e:
     import sys
     sys.stderr.write(f"An error occurred while importing Molecule_builder: {str(e)}\n")
@@ -107,15 +107,15 @@
 try:
     import numpy as np
 except ImportError as e:
     import sys
     sys.stderr.write(f"An error occurred while importing numpy: {str(e)}\n")
     del sys
 
-class Partition(BandStructure_builder, Config_builder, Crystal_builder, CrystalDefect_builder, ForceField_builder, 
+class Partition(BandStructure_builder, Config_builder, Crystal_builder, CrystalDefect_builder, Dataset_builder, 
                  Molecule_builder, PositionEditor_builder, SurfaceStates_builder, VacuumStates_builder, Filter_builder, 
                  SupercellEmbedding_builder, MoleculeCluster_builder,MolecularDynamic_builder,AbInitioThermodynamics_builder):
     """
     The Partition class is designed to handle various operations related to different types
     of crystal structure manipulations. It inherits from multiple builder classes, each
     specialized in a specific aspect of crystal structure and simulation setup.
     """
@@ -141,17 +141,17 @@
         Config_builder.__init__(self, name=name, file_location=file_location, **kwargs)
         # Crystal_builder: Likely used for creating or manipulating crystal structures. This class might 
         # handle tasks like generating crystal lattices, defining unit cells, or applying crystallographic transformations.
         Crystal_builder.__init__(self, name=name, file_location=file_location, **kwargs)
         # CrystalDefect_builder: Probably focused on introducing and managing defects within crystal structures, 
         # such as vacancies, interstitials, or dislocations. Useful in studies of material properties influenced by imperfections.
         CrystalDefect_builder.__init__(self, name=name, file_location=file_location, **kwargs)
-        # ForceField_builder: Likely used for defining or constructing force fields in molecular dynamics simulations. 
-        # This could involve setting up parameters like bond strengths, angles, and torsional forces.
-        ForceField_builder.__init__(self, name=name, file_location=file_location, **kwargs)
+        # 
+        # 
+        Dataset_builder.__init__(self, name=name, file_location=file_location, **kwargs)
         # Molecule_builder: Presumably used for creating and manipulating molecular structures. This may include 
         # tasks like building molecular models, adding or removing atoms or groups, and setting molecular geometries.
         Molecule_builder.__init__(self, name=name, file_location=file_location, **kwargs)
         # PositionEditor_builder: Probably designed for editing and manipulating atomic positions. This could 
         # involve tasks like translating, rotating, or scaling atomic structures.
         PositionEditor_builder.__init__(self, name=name, file_location=file_location, **kwargs)
         # SurfaceStates_builder: Likely focuses on the properties and states of material surfaces. This might include 
@@ -165,14 +165,20 @@
         Filter_builder.__init__(self, name=name, file_location=file_location, **kwargs)
         # SupercellEmbedding_builder: Likely used in the context of supercell models in crystallography or materials science. 
         # This class might handle the creation or manipulation of supercells for periodic boundary condition simulations.
         SupercellEmbedding_builder.__init__(self, name=name, file_location=file_location, **kwargs)
         #
         #
         MoleculeCluster_builder.__init__(self, name=name, file_location=file_location, **kwargs)
+        #
+        #
+        MolecularDynamic_builder.__init__(self, name=name, file_location=file_location, **kwargs)
+        #
+        #
+        AbInitioThermodynamics_builder.__init__(self, name=name, file_location=file_location, **kwargs)
 
     def generate_variants(self, parameter: str, values:np.array=None, file_location: str = None) -> bool:
         """
         Generates variants of the current container set based on the specified parameter and its range of values.
 
         This method iterates over the existing containers and applies different modifications
         according to the specified parameter (e.g., KPOINTS, VACANCY). The result is a new set
```

### Comparing `sage_lib-0.1.4.8/sage_lib/partition/PartitionManager.py` & `sage_lib-0.1.4.9/sage_lib/partition/PartitionManager.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.8/sage_lib/partition/partition_builder/MoleculeCluster_builder.py` & `sage_lib-0.1.4.9/sage_lib/partition/partition_builder/MoleculeCluster_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.8/sage_lib/partition/partition_builder/VacuumStates_builder.py` & `sage_lib-0.1.4.9/sage_lib/partition/partition_builder/VacuumStates_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         - file_location (str, optional): Path to the directory containing initial data files.
         - name (str, optional): Name identifier for this instance of VacuumStatesBuilder.
         - **kwargs: Additional keyword arguments.
         """
         super().__init__(name=name, file_location=file_location)
         
     def generate_dimers(self, container, steps: int = None, atomlabel_A: str = None, atomlabel_B: str = None, 
-                        initial_distance: float = None, final_distance: float = None, 
+                        initial_distance: float = None, final_distance: float = None, factor:float=None,
                         vacuum_tolerance: float = 6.0, file_location: str = None):
         """
         Generates a series of dimer configurations with varying distances.
 
         Parameters:
         - container (object): The container where the dimer configurations will be stored.
         - steps (int, optional): Number of steps between initial and final distance.
@@ -59,14 +59,15 @@
 
         Returns:
         - tuple: A pair of lists, one containing containers with dimer configurations, and the other containing subdirectories for these containers.
 
         Raises:
         - ValueError: If required parameters are not provided or invalid.
         """
+        factor = factor if factor else 0.8 
         initial_distance = initial_distance if initial_distance is not None else (self.covalent_radii[atomlabel_A]+self.covalent_radii[atomlabel_B])*0.85
         final_distance = final_distance if final_distance is not None else 5
         delta_distance =  (final_distance-initial_distance)/steps
         sub_directories, containers = [], []
         lattice_distance =  np.array([ [final_distance+vacuum_tolerance,0,0], [0,vacuum_tolerance,0], [0,0,vacuum_tolerance] ]) 
 
         for step in range(steps):
```

### Comparing `sage_lib-0.1.4.8/sage_lib/partition/partition_builder/Crystal_builder.py` & `sage_lib-0.1.4.9/sage_lib/partition/partition_builder/Crystal_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.8/sage_lib/partition/partition_builder/AbInitioThermodynamics_builder.py` & `sage_lib-0.1.4.9/sage_lib/partition/partition_builder/AbInitioThermodynamics_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,14 +137,15 @@
             x_values = np.linspace(pd_min, pd_max, 100)
             # Calculate y values based on the line equation
             y_values = m * x_values + b
             
             # Plot each line
             plt.plot(x_values, y_values, alpha=0.5, label=f'Line {index}')
 
+        opt_estructures = []
         # TODO: Identify and plot the lower envelope
         # This requires a custom implementation based on your criteria for the lower envelope.
         
         # Customize the plot
         plt.legend()
         plt.xlabel('X Axis')
         plt.ylabel('Y Axis')
```

### Comparing `sage_lib-0.1.4.8/sage_lib/partition/partition_builder/SurfaceStates_builder.py` & `sage_lib-0.1.4.9/sage_lib/partition/partition_builder/SurfaceStates_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.8/sage_lib/partition/partition_builder/SupercellEmbedding_builder.py` & `sage_lib-0.1.4.9/sage_lib/partition/partition_builder/SupercellEmbedding_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.8/sage_lib/partition/partition_builder/Filter_builder.py` & `sage_lib-0.1.4.9/sage_lib/partition/partition_builder/Filter_builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -186,14 +186,19 @@
             mask = np.array([compare(force) for force in forces_magnitude], dtype=int)
 
         elif container_property.upper() == 'E':
             # Calculate the magnitude of the total force for each container
             energies = [ c.AtomPositionManager.E for c in self.containers ]
             mask = np.array([compare(energy) for energy in energies], dtype=int)
 
+        elif container_property.upper() == 'E/N':
+            # Calculate the magnitude of the total force for each container
+            energies_atom = [ c.AtomPositionManager.E/c.AtomPositionManager.atomCount for c in self.containers ]
+            mask = np.array([compare(energy) for energy in energies_atom], dtype=int)
+
         elif container_property.upper() == 'HAS_ID':
             # 
             ID_amount = [ c.AtomPositionManager.atom_ID_amount(ID) for c in self.containers ]
             mask = np.array([ compare(ida) for ida in ID_amount], dtype=int)
 
         return mask
```

### Comparing `sage_lib-0.1.4.8/sage_lib/partition/partition_builder/Config_builder.py` & `sage_lib-0.1.4.9/sage_lib/partition/partition_builder/Config_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.8/sage_lib/partition/partition_builder/BandStructure_builder.py` & `sage_lib-0.1.4.9/sage_lib/partition/partition_builder/BandStructure_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.8/sage_lib/partition/partition_builder/MolecularDynamic_builder.py` & `sage_lib-0.1.4.9/sage_lib/partition/partition_builder/MolecularDynamic_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,20 +109,40 @@
         """
         super().__init__(name=name, file_location=file_location)
 
         self._molecule_template = {}
         self._density = None
         self._cluster_lattice_vectors = None
 
-    def get_count_species(self,):
+    def get_count_species(self, sigma:float=None) -> list:
         """
         """
         count_species = []
         for container_i, container in enumerate(self.containers):
-            count_species.append( container.AtomPositionManager.count_species() )
+            count_species.append( container.AtomPositionManager.count_species(sigma) )
+
+        return count_species
+
+    def get_molecular_graph_tracking(self, sigma:float=None ) -> list:
+        count_species = []
+        for container_i, container in enumerate(self.containers):
+            count_species.append( container.AtomPositionManager.get_molecular_graph(sigma=sigma) )
+
+        for i, n in enumerate(count_species[1:]):
+            print('iter', i)
+            for j, m in enumerate(n):
+                if len(m) < 10 and not m in count_species[i]:
+                    print('MOL', j)                    
+                    for o in count_species[i]:
+                        for p in o:
+
+                            if p in m:
+                                print( [ self.containers[0].AtomPositionManager.atomLabelsList[oo] for oo in o ], [ self.containers[0].AtomPositionManager.atomLabelsList[oo] for oo in m ] )
+                                print( o, m )
+
 
         return count_species
 
     def get_displacement(self, reference:str=None):
         """
         Calculate the displacement of atoms based on a reference point.
 
@@ -248,14 +268,15 @@
         for c_i, c in enumerate(self.containers):
             reference_pos = self._calculate_reference_values(c, reference='Z')
             for n_i, n in enumerate(initial_bonds):
                 data[c_i, n_i, 0] = reference_pos[n[0]]
                 data[c_i, n_i, 1] = c.AtomPositionManager.distance( c.AtomPositionManager.atomPositions[n[0]], c.AtomPositionManager.atomPositions[n[1]] )
 
         return {'initial_bonds_index':initial_bonds, 'bonds_data':data}
+        
 
     def _plot_RBF_for_container(self, container, container_i, output_path, verbose:bool=True):
         """
         Función para trazar RBF para un contenedor específico.
         """
         if verbose: print(f'Plot container {container_i}')
         output_path_container = os.path.join(output_path, f'MD_RBF/{container_i}')
@@ -471,51 +492,50 @@
             cuartil1 = np.percentile(error, 25)
             cuartil3 = np.percentile(error, 75)
             coef_variacion = desviacion_std / media if media != 0 else 0  # Prevenir división por cero
             mae = np.mean(np.abs(data_x - data_y))
             rmsd = np.sqrt(np.mean(np.square(data_x - data_y)))
             nrmsd = rmsd / (np.max(data_x) - np.min(data_x))
 
-            # Agregamos las estadísticas como texto en el plot
             textstr = '\n'.join((
-                f'Mínimo: {minimo:.2f}',
-                f'Máximo: {maximo:.2f}',
-                f'Media: {media:.2f}',
-                f'Mediana: {mediana:.2f}',
-                f'Desv. Estándar: {desviacion_std:.2f}',
-                f'Varianza: {varianza:.2f}',
-                f'Rango IQR: {rango_iqr:.2f}',
-                f'1er Cuartil: {cuartil1:.2f}',
-                f'3er Cuartil: {cuartil3:.2f}',
-                f'Coef. Variación: {coef_variacion:.2f}', 
+                f'Minimum: {minimo:.2f}',
+                f'Maximum: {maximo:.2f}',
+                f'Mean: {media:.2f}',
+                f'Median: {mediana:.2f}',
+                f'Standard Deviation: {desviacion_std:.2f}',
+                f'Variance: {varianza:.2f}',
+                f'IQR Range: {rango_iqr:.2f}',
+                f'1st Quartile: {cuartil1:.2f}',
+                f'3rd Quartile: {cuartil3:.2f}',
+                f'Coefficient of Variation: {coef_variacion:.2f}', 
                 f'MAE: {mae:.2f}',
                 f'RMSD: {rmsd:.2f}',
                 f'NRMSD: {nrmsd:.2f}' ))
 
             # Posicionamos el texto en el plot
             props = dict(boxstyle='round', facecolor='wheat', alpha=0.5)
             plt.text(0.65, 0.95, textstr, transform=plt.gca().transAxes, fontsize=12,
                      verticalalignment='top', bbox=props)
 
             plt.tight_layout()
             if save:
                 plt.savefig(f'{data_output_path}/evaluation_error_{data_label}_plot.png', dpi=100)
             plt.clf()
 
+            if verbose:
+                print(f' >> Plot :: Evaluation {n} - data shape: {data["F"]["train"][n].shape}')
+                print(f' >> Plot :: Error Distribution {n} - data shape: {error.shape}')
 
 
         for n in data['F']['train']:
 
             _plot(  data_x=np.linalg.norm(data['F']['train'][n],axis=1), 
                     data_y=np.linalg.norm(data['F']['validation'][n],axis=1), 
                     data_color=self.element_colors[n], 
                     data_label=n, data_output_path=output_path, data_max=10, data_min=0)
-            if verbose:
-                print(f' >> Plot :: Evaluation {n} - data shape: {data["F"]["train"][n].shape}')
-                print(f' >> Plot :: Error Distribution {n} - data shape: {error.shape}')
 
         data_x= data['E']['train']/data['N']['train']
         data_y= data['E']['validation']/data['N']['validation']
 
         _plot(  data_x=data_x, 
                 data_y=data_y, 
                 data_color=(0.2, 0.2, 0.2), 
@@ -635,37 +655,41 @@
         Args:
             values (list): List of analysis types to perform.
             file_location (str, optional): File location for output data.
         """
         MDA_data = {}
 
         for plot in values:
-            if plot.upper() == 'displacements':
+            if plot.upper() == 'DISPLACEMENTS':
                 MDA_data['displacement'] = self.get_displacement(reference=values[plot].get('reference', None))
                 self.plot_displacement( data_displacement=MDA_data['displacement'], output_path=values[plot].get('output_path', '.'), verbose=values[plot].get('verbose', False) )
 
             if plot.upper() == 'RBF':
                 MDA_data['RBF'] = self.plot_RBF()
                 self.animated_RBF( output_path=values[plot].get('output_path', '.'), duration=0.1, save=True, verbose=values[plot].get('verbose', False) )
 
-            if plot.upper() == 'COUNT':
-                MDA_data['count'] = self.get_count_species()
+            if plot.upper() == 'COUNT_SPECIES':
+                MDA_data['count'] = self.get_count_species(sigma=values[plot].get('sigma', None))
                 self.plot_count( count_dict=MDA_data['count'], output_path=values[plot].get('output_path', '.'), save=True, verbose=values[plot].get('verbose', False) )
 
             if plot.upper() == 'EVALUATE_FF':
                 MDA_data['evaluation'] = self.get_evaluation(
                                                     ff_energy_tag=values[plot].get('ff_energy_tag', 'ff-energy'),
                                                     ff_forces_tag=values[plot].get('ff_forces_tag', 'ff-forces'),
                                                             )
                 self.plot_evaluation(data=MDA_data['evaluation'], output_path=values[plot].get('output_path', '.'), save=True, verbose=values[plot].get('verbose', False) )
 
-            if plot.upper() == 'BOND_TRACKING':
+            if plot.upper() == 'BOND_DISTANCE_TRACKING':
                 MDA_data['bond_tracking'] = self.get_bond_tracking(sigma=values[plot].get('sigma', None), reference=values[plot].get('reference', None))
                 self.plot_bond_tracking( bond_tracking_dict=MDA_data['bond_tracking'], output_path=values[plot].get('output_path', '.'), save=True, verbose=values[plot].get('verbose', False) )
 
+            if plot.upper() == 'MOLECULE_FORMATION_TRACKING':
+                MDA_data['molecule_formation_tracking'] = self.get_molecular_graph_tracking(sigma=values[plot].get('sigma', None))
+                #self.plot_bond_tracking( bond_tracking_dict=MDA_data['bond_tracking'], output_path=values[plot].get('output_path', '.'), save=True, verbose=values[plot].get('verbose', False) )
+
                 #self.plot_count( count_dict=MDA_data['count'], output_path=values[plot].get('output_path', '.'), save=True, verbose=values[plot].get('verbose', False) )
 
 
 
 '''
 import numpy as np
 import ase.io
```

### Comparing `sage_lib-0.1.4.8/sage_lib/partition/partition_builder/PositionEditor_builder.py` & `sage_lib-0.1.4.9/sage_lib/partition/partition_builder/PositionEditor_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.8/sage_lib/partition/partition_builder/Molecule_builder.py` & `sage_lib-0.1.4.9/sage_lib/partition/partition_builder/Molecule_builder.py`

 * *Files identical despite different names*

### Comparing `sage_lib-0.1.4.8/sage_lib/partition/partition_builder/CrystalDefect_builder.py` & `sage_lib-0.1.4.9/sage_lib/partition/partition_builder/CrystalDefect_builder.py`

 * *Files identical despite different names*

