# Comparing `tmp/multipie-1.2.8.tar.gz` & `tmp/multipie-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multipie-1.2.8.tar", last modified: Fri Nov 17 06:30:00 2023, max compression
+gzip compressed data, was "multipie-1.2.9.tar", last modified: Wed Nov 22 21:36:16 2023, max compression
```

## Comparing `multipie-1.2.8.tar` & `multipie-1.2.9.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-17 06:30:00.544550 multipie-1.2.8/
--rw-r--r--   0 hiro       (501) staff       (20)     1094 2023-05-09 15:21:28.000000 multipie-1.2.8/LICENSE
--rw-------   0 hiro       (501) staff       (20)       81 2023-05-15 22:16:08.000000 multipie-1.2.8/MANIFEST.in
--rw-r--r--   0 hiro       (501) staff       (20)     2568 2023-11-17 06:30:00.544448 multipie-1.2.8/PKG-INFO
--rw-r--r--   0 hiro       (501) staff       (20)     1799 2023-09-05 16:17:11.000000 multipie-1.2.8/README.md
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-17 06:30:00.460899 multipie-1.2.8/multipie/
--rw-r--r--   0 hiro       (501) staff       (20)     2308 2023-11-17 06:29:16.000000 multipie-1.2.8/multipie/__init__.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-17 06:30:00.498918 multipie-1.2.8/multipie/binary_data/
--rw-r--r--   0 hiro       (501) staff       (20)  5502948 2023-06-26 07:42:20.000000 multipie-1.2.8/multipie/binary_data/BaseAtomicMultipoleDataset.pkl
--rw-r--r--   0 hiro       (501) staff       (20)   163441 2023-05-15 15:35:55.000000 multipie-1.2.8/multipie/binary_data/CharacterPGSet.pkl
--rw-r--r--   0 hiro       (501) staff       (20)  6228253 2023-06-26 07:42:20.000000 multipie-1.2.8/multipie/binary_data/ClebschGordanPGSet.pkl
--rw-r--r--   0 hiro       (501) staff       (20)  6179284 2023-06-26 07:42:20.000000 multipie-1.2.8/multipie/binary_data/HarmonicsPGSet.pkl
--rw-r--r--   0 hiro       (501) staff       (20)   479036 2023-06-26 07:42:20.000000 multipie-1.2.8/multipie/binary_data/ResponseTensorPGSet.pkl
--rw-r--r--   0 hiro       (501) staff       (20)  1398892 2023-05-15 15:37:21.000000 multipie-1.2.8/multipie/binary_data/SymmetryOperationGSet.pkl
--rw-r--r--   0 hiro       (501) staff       (20)   173363 2023-05-15 15:37:24.000000 multipie-1.2.8/multipie/binary_data/VirtualClusterPGSet.pkl
--rw-r--r--   0 hiro       (501) staff       (20)   428610 2023-06-26 07:42:20.000000 multipie-1.2.8/multipie/binary_data/WyckoffGSet.pkl
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-17 06:30:00.501618 multipie-1.2.8/multipie/character/
--rwxr-xr-x   0 hiro       (501) staff       (20)     9784 2023-05-15 15:10:01.000000 multipie-1.2.8/multipie/character/character_pg.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     2009 2023-05-09 15:21:28.000000 multipie-1.2.8/multipie/character/character_pg_set.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-17 06:30:00.502155 multipie-1.2.8/multipie/clebsch_gordan/
--rwxr-xr-x   0 hiro       (501) staff       (20)     3189 2023-05-09 15:21:28.000000 multipie-1.2.8/multipie/clebsch_gordan/clebsch_gordan_pg.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1205 2023-05-09 15:21:28.000000 multipie-1.2.8/multipie/clebsch_gordan/clebsch_gordan_pg_set.py
--rw-r--r--   0 hiro       (501) staff       (20)     2609 2023-05-15 15:16:23.000000 multipie-1.2.8/multipie/const.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-17 06:30:00.531094 multipie-1.2.8/multipie/data/
--rwxr-xr-x   0 hiro       (501) staff       (20)  6306703 2023-05-09 15:21:28.000000 multipie-1.2.8/multipie/data/data_atomic_multipoles.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     8617 2023-05-09 15:21:28.000000 multipie-1.2.8/multipie/data/data_cartesian_to_ch_harmoncis.py
--rwxr-xr-x   0 hiro       (501) staff       (20)    12997 2023-05-09 15:21:28.000000 multipie-1.2.8/multipie/data/data_character_table.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     4838 2023-05-09 15:21:28.000000 multipie-1.2.8/multipie/data/data_compatibility_relation.py
--rwxr-xr-x   0 hiro       (501) staff       (20)  3154848 2023-05-09 15:21:28.000000 multipie-1.2.8/multipie/data/data_harmonics.py
--rwxr-xr-x   0 hiro       (501) staff       (20)   795507 2023-05-09 15:21:28.000000 multipie-1.2.8/multipie/data/data_harmonics_real.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     4044 2023-05-09 15:21:28.000000 multipie-1.2.8/multipie/data/data_no_space_group.py
--rwxr-xr-x   0 hiro       (501) staff       (20)    34367 2023-05-09 15:21:28.000000 multipie-1.2.8/multipie/data/data_product_decomp.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     7151 2023-05-09 15:21:28.000000 multipie-1.2.8/multipie/data/data_symmetry_operation_pg.py
--rwxr-xr-x   0 hiro       (501) staff       (20)    99525 2023-05-09 15:21:28.000000 multipie-1.2.8/multipie/data/data_symmetry_operation_sg.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1147 2023-09-27 15:25:52.000000 multipie-1.2.8/multipie/data/data_tag_harmonics_alias.py
--rwxr-xr-x   0 hiro       (501) staff       (20)      808 2023-05-09 15:21:28.000000 multipie-1.2.8/multipie/data/data_tag_irrep.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     3177 2023-05-09 15:21:28.000000 multipie-1.2.8/multipie/data/data_tag_point_group.py
--rwxr-xr-x   0 hiro       (501) staff       (20)    15738 2023-05-09 15:21:28.000000 multipie-1.2.8/multipie/data/data_tag_space_group.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1453 2023-10-04 11:55:57.000000 multipie-1.2.8/multipie/data/data_transform_matrix.py
--rwxr-xr-x   0 hiro       (501) staff       (20)   148045 2023-05-09 15:21:28.000000 multipie-1.2.8/multipie/data/data_virtual_cluster_real.py
--rwxr-xr-x   0 hiro       (501) staff       (20)    16423 2023-06-18 01:04:56.000000 multipie-1.2.8/multipie/data/data_wyckoff_pg.py
--rwxr-xr-x   0 hiro       (501) staff       (20)   174033 2023-06-18 06:26:28.000000 multipie-1.2.8/multipie/data/data_wyckoff_sg.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-17 06:30:00.532283 multipie-1.2.8/multipie/group/
--rwxr-xr-x   0 hiro       (501) staff       (20)    30277 2023-10-27 03:29:35.000000 multipie-1.2.8/multipie/group/point_group.py
--rwxr-xr-x   0 hiro       (501) staff       (20)    22747 2023-10-27 03:29:35.000000 multipie-1.2.8/multipie/group/space_group.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-17 06:30:00.533275 multipie-1.2.8/multipie/harmonics/
--rwxr-xr-x   0 hiro       (501) staff       (20)     4791 2023-05-15 15:10:01.000000 multipie-1.2.8/multipie/harmonics/harmonics.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     2888 2023-05-09 15:21:28.000000 multipie-1.2.8/multipie/harmonics/harmonics_complex_pg.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1415 2023-05-09 15:21:28.000000 multipie-1.2.8/multipie/harmonics/harmonics_complex_pg_set.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     3216 2023-05-09 15:21:28.000000 multipie-1.2.8/multipie/harmonics/harmonics_pg.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1393 2023-05-09 15:21:28.000000 multipie-1.2.8/multipie/harmonics/harmonics_pg_set.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-17 06:30:00.533436 multipie-1.2.8/multipie/harmonics/util/
--rwxr-xr-x   0 hiro       (501) staff       (20)     2287 2023-05-15 15:10:01.000000 multipie-1.2.8/multipie/harmonics/util/equivalent_operator.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-17 06:30:00.535065 multipie-1.2.8/multipie/model/
--rwxr-xr-x   0 hiro       (501) staff       (20)     3958 2023-10-25 00:59:23.000000 multipie-1.2.8/multipie/model/construct_model.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     3808 2023-10-27 05:31:44.000000 multipie-1.2.8/multipie/model/create_model.py
--rw-r--r--   0 hiro       (501) staff       (20)    36206 2023-11-17 06:29:16.000000 multipie-1.2.8/multipie/model/material_model.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     7555 2023-05-15 15:10:01.000000 multipie-1.2.8/multipie/model/multipie_manager.py
--rwxr-xr-x   0 hiro       (501) staff       (20)    32981 2023-10-27 06:00:02.000000 multipie-1.2.8/multipie/model/symmetry_adapted_model.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-17 06:30:00.536293 multipie-1.2.8/multipie/model/util/
--rwxr-xr-x   0 hiro       (501) staff       (20)      259 2023-05-15 15:10:01.000000 multipie-1.2.8/multipie/model/util/atomic_matrix_util.py
--rwxr-xr-x   0 hiro       (501) staff       (20)    27662 2023-09-27 15:25:52.000000 multipie-1.2.8/multipie/model/util/create_pdf.py
--rwxr-xr-x   0 hiro       (501) staff       (20)    24984 2023-10-25 01:05:51.000000 multipie-1.2.8/multipie/model/util/symmetry_adapted_model_util.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-17 06:30:00.457843 multipie-1.2.8/multipie/multipole/
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-17 06:30:00.538122 multipie-1.2.8/multipie/multipole/base/
--rwxr-xr-x   0 hiro       (501) staff       (20)     1132 2023-05-09 15:21:28.000000 multipie-1.2.8/multipie/multipole/base/base_atomic_multipole_dataset.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     2021 2023-06-26 07:42:20.000000 multipie-1.2.8/multipie/multipole/base/base_atomic_multipole_set.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-17 06:30:00.539560 multipie-1.2.8/multipie/multipole/util/
--rwxr-xr-x   0 hiro       (501) staff       (20)    14798 2023-09-27 15:25:52.000000 multipie-1.2.8/multipie/multipole/util/atomic_orbital_util.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     7452 2023-09-27 15:25:52.000000 multipie-1.2.8/multipie/multipole/util/atomic_samb_util.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1462 2023-05-15 15:10:01.000000 multipie-1.2.8/multipie/multipole/util/multipole_util.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1950 2023-05-09 15:21:28.000000 multipie-1.2.8/multipie/multipole/util/pauli.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     2891 2023-05-09 15:21:28.000000 multipie-1.2.8/multipie/multipole/util/spin_orbital_basis.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     5022 2023-09-27 15:25:52.000000 multipie-1.2.8/multipie/multipole/util/structure_samb_util.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     4908 2023-09-26 21:54:38.000000 multipie-1.2.8/multipie/multipole/util/z_samb_util.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-17 06:30:00.540129 multipie-1.2.8/multipie/response_tensor/
--rwxr-xr-x   0 hiro       (501) staff       (20)     6692 2023-05-15 15:10:01.000000 multipie-1.2.8/multipie/response_tensor/response_tensor_pg.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1406 2023-05-09 15:21:28.000000 multipie-1.2.8/multipie/response_tensor/response_tensor_pg_set.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-17 06:30:00.540295 multipie-1.2.8/multipie/response_tensor/util/
--rwxr-xr-x   0 hiro       (501) staff       (20)    22414 2023-05-09 15:21:28.000000 multipie-1.2.8/multipie/response_tensor/util/response_tensor_util.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-17 06:30:00.540649 multipie-1.2.8/multipie/scripts/
--rwxr-xr-x   0 hiro       (501) staff       (20)      567 2023-05-15 15:34:10.000000 multipie-1.2.8/multipie/scripts/create_binary.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1601 2023-06-04 14:31:58.000000 multipie-1.2.8/multipie/scripts/create_samb.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-17 06:30:00.541244 multipie-1.2.8/multipie/symmetry_operation/
--rwxr-xr-x   0 hiro       (501) staff       (20)     3037 2023-05-15 15:10:01.000000 multipie-1.2.8/multipie/symmetry_operation/symmetry_operation.py
--rwxr-xr-x   0 hiro       (501) staff       (20)    14963 2023-10-04 11:55:57.000000 multipie-1.2.8/multipie/symmetry_operation/symmetry_operation_g.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1584 2023-05-09 15:21:28.000000 multipie-1.2.8/multipie/symmetry_operation/symmetry_operation_g_set.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-17 06:30:00.541400 multipie-1.2.8/multipie/symmetry_operation/util/
--rwxr-xr-x   0 hiro       (501) staff       (20)     5769 2023-10-04 11:55:57.000000 multipie-1.2.8/multipie/symmetry_operation/util/symmetry_operation_util.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-17 06:30:00.543075 multipie-1.2.8/multipie/tag/
--rwxr-xr-x   0 hiro       (501) staff       (20)     1840 2023-05-09 15:21:28.000000 multipie-1.2.8/multipie/tag/tag.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     4830 2023-05-09 15:21:28.000000 multipie-1.2.8/multipie/tag/tag_group.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     2189 2023-05-09 15:21:28.000000 multipie-1.2.8/multipie/tag/tag_irrep.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     2859 2023-05-09 15:21:28.000000 multipie-1.2.8/multipie/tag/tag_list.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     8074 2023-05-09 15:21:28.000000 multipie-1.2.8/multipie/tag/tag_multipole.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     2783 2023-05-09 15:21:28.000000 multipie-1.2.8/multipie/tag/tag_response_tensor.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     4402 2023-05-09 15:21:28.000000 multipie-1.2.8/multipie/tag/tag_symmetry_operation.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1560 2023-05-09 15:21:28.000000 multipie-1.2.8/multipie/tag/tag_wyckoff.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-17 06:30:00.543398 multipie-1.2.8/multipie/virtual_cluster/
--rwxr-xr-x   0 hiro       (501) staff       (20)     2818 2023-05-15 15:10:01.000000 multipie-1.2.8/multipie/virtual_cluster/virtual_cluster_pg.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1440 2023-05-09 15:21:28.000000 multipie-1.2.8/multipie/virtual_cluster/virtual_cluster_pg_set.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-17 06:30:00.543815 multipie-1.2.8/multipie/wyckoff/
--rwxr-xr-x   0 hiro       (501) staff       (20)     3790 2023-06-18 00:29:54.000000 multipie-1.2.8/multipie/wyckoff/wyckoff_g.py
--rwxr-xr-x   0 hiro       (501) staff       (20)     1512 2023-05-09 15:21:28.000000 multipie-1.2.8/multipie/wyckoff/wyckoff_g_set.py
-drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-17 06:30:00.463032 multipie-1.2.8/multipie.egg-info/
--rw-r--r--   0 hiro       (501) staff       (20)     2568 2023-11-17 06:30:00.000000 multipie-1.2.8/multipie.egg-info/PKG-INFO
--rw-r--r--   0 hiro       (501) staff       (20)     3339 2023-11-17 06:30:00.000000 multipie-1.2.8/multipie.egg-info/SOURCES.txt
--rw-r--r--   0 hiro       (501) staff       (20)        1 2023-11-17 06:30:00.000000 multipie-1.2.8/multipie.egg-info/dependency_links.txt
--rw-r--r--   0 hiro       (501) staff       (20)      116 2023-11-17 06:30:00.000000 multipie-1.2.8/multipie.egg-info/entry_points.txt
--rw-r--r--   0 hiro       (501) staff       (20)       82 2023-11-17 06:30:00.000000 multipie-1.2.8/multipie.egg-info/requires.txt
--rw-r--r--   0 hiro       (501) staff       (20)        9 2023-11-17 06:30:00.000000 multipie-1.2.8/multipie.egg-info/top_level.txt
--rw-r--r--   0 hiro       (501) staff       (20)      888 2023-11-17 06:30:00.544846 multipie-1.2.8/setup.cfg
--rw-r--r--   0 hiro       (501) staff       (20)       38 2023-05-09 15:21:28.000000 multipie-1.2.8/setup.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-22 21:36:16.318023 multipie-1.2.9/
+-rw-r--r--   0 hiro       (501) staff       (20)     1094 2023-05-09 15:21:28.000000 multipie-1.2.9/LICENSE
+-rw-------   0 hiro       (501) staff       (20)       81 2023-05-15 22:16:08.000000 multipie-1.2.9/MANIFEST.in
+-rw-r--r--   0 hiro       (501) staff       (20)     2568 2023-11-22 21:36:16.317933 multipie-1.2.9/PKG-INFO
+-rw-r--r--   0 hiro       (501) staff       (20)     1799 2023-09-05 16:17:11.000000 multipie-1.2.9/README.md
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-22 21:36:16.217387 multipie-1.2.9/multipie/
+-rw-r--r--   0 hiro       (501) staff       (20)     2308 2023-11-22 21:35:47.000000 multipie-1.2.9/multipie/__init__.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-22 21:36:16.266087 multipie-1.2.9/multipie/binary_data/
+-rw-r--r--   0 hiro       (501) staff       (20)  5502948 2023-06-26 07:42:20.000000 multipie-1.2.9/multipie/binary_data/BaseAtomicMultipoleDataset.pkl
+-rw-r--r--   0 hiro       (501) staff       (20)   163441 2023-05-15 15:35:55.000000 multipie-1.2.9/multipie/binary_data/CharacterPGSet.pkl
+-rw-r--r--   0 hiro       (501) staff       (20)  6228253 2023-06-26 07:42:20.000000 multipie-1.2.9/multipie/binary_data/ClebschGordanPGSet.pkl
+-rw-r--r--   0 hiro       (501) staff       (20)  6179284 2023-06-26 07:42:20.000000 multipie-1.2.9/multipie/binary_data/HarmonicsPGSet.pkl
+-rw-r--r--   0 hiro       (501) staff       (20)   479036 2023-06-26 07:42:20.000000 multipie-1.2.9/multipie/binary_data/ResponseTensorPGSet.pkl
+-rw-r--r--   0 hiro       (501) staff       (20)  1398892 2023-05-15 15:37:21.000000 multipie-1.2.9/multipie/binary_data/SymmetryOperationGSet.pkl
+-rw-r--r--   0 hiro       (501) staff       (20)   173363 2023-05-15 15:37:24.000000 multipie-1.2.9/multipie/binary_data/VirtualClusterPGSet.pkl
+-rw-r--r--   0 hiro       (501) staff       (20)   428610 2023-06-26 07:42:20.000000 multipie-1.2.9/multipie/binary_data/WyckoffGSet.pkl
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-22 21:36:16.268641 multipie-1.2.9/multipie/character/
+-rwxr-xr-x   0 hiro       (501) staff       (20)     9784 2023-05-15 15:10:01.000000 multipie-1.2.9/multipie/character/character_pg.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     2009 2023-05-09 15:21:28.000000 multipie-1.2.9/multipie/character/character_pg_set.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-22 21:36:16.269191 multipie-1.2.9/multipie/clebsch_gordan/
+-rwxr-xr-x   0 hiro       (501) staff       (20)     3189 2023-05-09 15:21:28.000000 multipie-1.2.9/multipie/clebsch_gordan/clebsch_gordan_pg.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1205 2023-05-09 15:21:28.000000 multipie-1.2.9/multipie/clebsch_gordan/clebsch_gordan_pg_set.py
+-rw-r--r--   0 hiro       (501) staff       (20)     2609 2023-05-15 15:16:23.000000 multipie-1.2.9/multipie/const.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-22 21:36:16.304525 multipie-1.2.9/multipie/data/
+-rwxr-xr-x   0 hiro       (501) staff       (20)  6306703 2023-05-09 15:21:28.000000 multipie-1.2.9/multipie/data/data_atomic_multipoles.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     8617 2023-05-09 15:21:28.000000 multipie-1.2.9/multipie/data/data_cartesian_to_ch_harmoncis.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)    12997 2023-05-09 15:21:28.000000 multipie-1.2.9/multipie/data/data_character_table.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     4838 2023-05-09 15:21:28.000000 multipie-1.2.9/multipie/data/data_compatibility_relation.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)  3154848 2023-05-09 15:21:28.000000 multipie-1.2.9/multipie/data/data_harmonics.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)   795507 2023-05-09 15:21:28.000000 multipie-1.2.9/multipie/data/data_harmonics_real.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     4044 2023-05-09 15:21:28.000000 multipie-1.2.9/multipie/data/data_no_space_group.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)    34367 2023-05-09 15:21:28.000000 multipie-1.2.9/multipie/data/data_product_decomp.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     7151 2023-05-09 15:21:28.000000 multipie-1.2.9/multipie/data/data_symmetry_operation_pg.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)    99525 2023-05-09 15:21:28.000000 multipie-1.2.9/multipie/data/data_symmetry_operation_sg.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1147 2023-09-27 15:25:52.000000 multipie-1.2.9/multipie/data/data_tag_harmonics_alias.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)      808 2023-05-09 15:21:28.000000 multipie-1.2.9/multipie/data/data_tag_irrep.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     3177 2023-05-09 15:21:28.000000 multipie-1.2.9/multipie/data/data_tag_point_group.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)    15738 2023-05-09 15:21:28.000000 multipie-1.2.9/multipie/data/data_tag_space_group.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1453 2023-10-04 11:55:57.000000 multipie-1.2.9/multipie/data/data_transform_matrix.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)   148045 2023-05-09 15:21:28.000000 multipie-1.2.9/multipie/data/data_virtual_cluster_real.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)    16423 2023-06-18 01:04:56.000000 multipie-1.2.9/multipie/data/data_wyckoff_pg.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)   174033 2023-06-18 06:26:28.000000 multipie-1.2.9/multipie/data/data_wyckoff_sg.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-22 21:36:16.305755 multipie-1.2.9/multipie/group/
+-rwxr-xr-x   0 hiro       (501) staff       (20)    30277 2023-10-27 03:29:35.000000 multipie-1.2.9/multipie/group/point_group.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)    22747 2023-10-27 03:29:35.000000 multipie-1.2.9/multipie/group/space_group.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-22 21:36:16.306722 multipie-1.2.9/multipie/harmonics/
+-rwxr-xr-x   0 hiro       (501) staff       (20)     4791 2023-05-15 15:10:01.000000 multipie-1.2.9/multipie/harmonics/harmonics.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     2888 2023-05-09 15:21:28.000000 multipie-1.2.9/multipie/harmonics/harmonics_complex_pg.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1415 2023-05-09 15:21:28.000000 multipie-1.2.9/multipie/harmonics/harmonics_complex_pg_set.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     3216 2023-05-09 15:21:28.000000 multipie-1.2.9/multipie/harmonics/harmonics_pg.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1393 2023-05-09 15:21:28.000000 multipie-1.2.9/multipie/harmonics/harmonics_pg_set.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-22 21:36:16.306860 multipie-1.2.9/multipie/harmonics/util/
+-rwxr-xr-x   0 hiro       (501) staff       (20)     2287 2023-05-15 15:10:01.000000 multipie-1.2.9/multipie/harmonics/util/equivalent_operator.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-22 21:36:16.308233 multipie-1.2.9/multipie/model/
+-rwxr-xr-x   0 hiro       (501) staff       (20)     3958 2023-10-25 00:59:23.000000 multipie-1.2.9/multipie/model/construct_model.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     4418 2023-11-22 21:35:47.000000 multipie-1.2.9/multipie/model/create_model.py
+-rw-r--r--   0 hiro       (501) staff       (20)    35939 2023-11-22 21:35:47.000000 multipie-1.2.9/multipie/model/material_model.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     7555 2023-05-15 15:10:01.000000 multipie-1.2.9/multipie/model/multipie_manager.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)    32981 2023-10-27 06:00:02.000000 multipie-1.2.9/multipie/model/symmetry_adapted_model.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-22 21:36:16.309402 multipie-1.2.9/multipie/model/util/
+-rwxr-xr-x   0 hiro       (501) staff       (20)      259 2023-05-15 15:10:01.000000 multipie-1.2.9/multipie/model/util/atomic_matrix_util.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)    27662 2023-09-27 15:25:52.000000 multipie-1.2.9/multipie/model/util/create_pdf.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)    24984 2023-10-25 01:05:51.000000 multipie-1.2.9/multipie/model/util/symmetry_adapted_model_util.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-22 21:36:16.215804 multipie-1.2.9/multipie/multipole/
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-22 21:36:16.310085 multipie-1.2.9/multipie/multipole/base/
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1132 2023-05-09 15:21:28.000000 multipie-1.2.9/multipie/multipole/base/base_atomic_multipole_dataset.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     2021 2023-06-26 07:42:20.000000 multipie-1.2.9/multipie/multipole/base/base_atomic_multipole_set.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-22 21:36:16.311375 multipie-1.2.9/multipie/multipole/util/
+-rwxr-xr-x   0 hiro       (501) staff       (20)    14798 2023-09-27 15:25:52.000000 multipie-1.2.9/multipie/multipole/util/atomic_orbital_util.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     7452 2023-09-27 15:25:52.000000 multipie-1.2.9/multipie/multipole/util/atomic_samb_util.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1462 2023-05-15 15:10:01.000000 multipie-1.2.9/multipie/multipole/util/multipole_util.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1950 2023-05-09 15:21:28.000000 multipie-1.2.9/multipie/multipole/util/pauli.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     2891 2023-05-09 15:21:28.000000 multipie-1.2.9/multipie/multipole/util/spin_orbital_basis.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     5022 2023-09-27 15:25:52.000000 multipie-1.2.9/multipie/multipole/util/structure_samb_util.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     4908 2023-09-26 21:54:38.000000 multipie-1.2.9/multipie/multipole/util/z_samb_util.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-22 21:36:16.311883 multipie-1.2.9/multipie/response_tensor/
+-rwxr-xr-x   0 hiro       (501) staff       (20)     6692 2023-05-15 15:10:01.000000 multipie-1.2.9/multipie/response_tensor/response_tensor_pg.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1406 2023-05-09 15:21:28.000000 multipie-1.2.9/multipie/response_tensor/response_tensor_pg_set.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-22 21:36:16.312042 multipie-1.2.9/multipie/response_tensor/util/
+-rwxr-xr-x   0 hiro       (501) staff       (20)    22414 2023-05-09 15:21:28.000000 multipie-1.2.9/multipie/response_tensor/util/response_tensor_util.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-22 21:36:16.312384 multipie-1.2.9/multipie/scripts/
+-rwxr-xr-x   0 hiro       (501) staff       (20)      567 2023-05-15 15:34:10.000000 multipie-1.2.9/multipie/scripts/create_binary.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1601 2023-06-04 14:31:58.000000 multipie-1.2.9/multipie/scripts/create_samb.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-22 21:36:16.313004 multipie-1.2.9/multipie/symmetry_operation/
+-rwxr-xr-x   0 hiro       (501) staff       (20)     3037 2023-05-15 15:10:01.000000 multipie-1.2.9/multipie/symmetry_operation/symmetry_operation.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)    14963 2023-10-04 11:55:57.000000 multipie-1.2.9/multipie/symmetry_operation/symmetry_operation_g.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1584 2023-05-09 15:21:28.000000 multipie-1.2.9/multipie/symmetry_operation/symmetry_operation_g_set.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-22 21:36:16.313157 multipie-1.2.9/multipie/symmetry_operation/util/
+-rwxr-xr-x   0 hiro       (501) staff       (20)     5769 2023-10-04 11:55:57.000000 multipie-1.2.9/multipie/symmetry_operation/util/symmetry_operation_util.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-22 21:36:16.314681 multipie-1.2.9/multipie/tag/
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1840 2023-05-09 15:21:28.000000 multipie-1.2.9/multipie/tag/tag.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     4830 2023-05-09 15:21:28.000000 multipie-1.2.9/multipie/tag/tag_group.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     2189 2023-05-09 15:21:28.000000 multipie-1.2.9/multipie/tag/tag_irrep.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     2859 2023-05-09 15:21:28.000000 multipie-1.2.9/multipie/tag/tag_list.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     8074 2023-05-09 15:21:28.000000 multipie-1.2.9/multipie/tag/tag_multipole.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     2783 2023-05-09 15:21:28.000000 multipie-1.2.9/multipie/tag/tag_response_tensor.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     4402 2023-05-09 15:21:28.000000 multipie-1.2.9/multipie/tag/tag_symmetry_operation.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1560 2023-05-09 15:21:28.000000 multipie-1.2.9/multipie/tag/tag_wyckoff.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-22 21:36:16.314998 multipie-1.2.9/multipie/virtual_cluster/
+-rwxr-xr-x   0 hiro       (501) staff       (20)     2818 2023-05-15 15:10:01.000000 multipie-1.2.9/multipie/virtual_cluster/virtual_cluster_pg.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1440 2023-05-09 15:21:28.000000 multipie-1.2.9/multipie/virtual_cluster/virtual_cluster_pg_set.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-22 21:36:16.315456 multipie-1.2.9/multipie/wyckoff/
+-rwxr-xr-x   0 hiro       (501) staff       (20)     3790 2023-06-18 00:29:54.000000 multipie-1.2.9/multipie/wyckoff/wyckoff_g.py
+-rwxr-xr-x   0 hiro       (501) staff       (20)     1512 2023-05-09 15:21:28.000000 multipie-1.2.9/multipie/wyckoff/wyckoff_g_set.py
+drwxr-xr-x   0 hiro       (501) staff       (20)        0 2023-11-22 21:36:16.218217 multipie-1.2.9/multipie.egg-info/
+-rw-r--r--   0 hiro       (501) staff       (20)     2568 2023-11-22 21:36:16.000000 multipie-1.2.9/multipie.egg-info/PKG-INFO
+-rw-r--r--   0 hiro       (501) staff       (20)     3339 2023-11-22 21:36:16.000000 multipie-1.2.9/multipie.egg-info/SOURCES.txt
+-rw-r--r--   0 hiro       (501) staff       (20)        1 2023-11-22 21:36:16.000000 multipie-1.2.9/multipie.egg-info/dependency_links.txt
+-rw-r--r--   0 hiro       (501) staff       (20)      116 2023-11-22 21:36:16.000000 multipie-1.2.9/multipie.egg-info/entry_points.txt
+-rw-r--r--   0 hiro       (501) staff       (20)       82 2023-11-22 21:36:16.000000 multipie-1.2.9/multipie.egg-info/requires.txt
+-rw-r--r--   0 hiro       (501) staff       (20)        9 2023-11-22 21:36:16.000000 multipie-1.2.9/multipie.egg-info/top_level.txt
+-rw-r--r--   0 hiro       (501) staff       (20)      888 2023-11-22 21:36:16.318368 multipie-1.2.9/setup.cfg
+-rw-r--r--   0 hiro       (501) staff       (20)       38 2023-05-09 15:21:28.000000 multipie-1.2.9/setup.py
```

### Comparing `multipie-1.2.8/LICENSE` & `multipie-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/PKG-INFO` & `multipie-1.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multipie
-Version: 1.2.8
+Version: 1.2.9
 Summary: A python library for crystallographic symmetry operations and Symmetry-Adapted Multipole Basis (SAMB).
 Home-page: https://github.com/CMT-MU/MultiPie
 Author: Hiroaki Kusunose and Rikuto Oiwa
 Author-email: hiroaki.kusunose@gmail.com, ro.qp.07@gmail.com
 License: MIT
 Keywords: group theory,condensed matter,materials science,basis
 Requires-Python: >=3.9
```

### Comparing `multipie-1.2.8/README.md` & `multipie-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/__init__.py` & `multipie-1.2.9/multipie/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import sys
 
-__version__ = "1.2.8"
+__version__ = "1.2.9"
 __top_dir__ = os.path.normpath(os.path.dirname(__file__) + "/../") + "/"
 __bin_dir__ = __top_dir__ + "multipie/binary_data/"
 
 
 # ==================================================
 from gcoreutils.string_util import class_name
 from gcoreutils.binary_manager import BinaryManager
```

### Comparing `multipie-1.2.8/multipie/binary_data/BaseAtomicMultipoleDataset.pkl` & `multipie-1.2.9/multipie/binary_data/BaseAtomicMultipoleDataset.pkl`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/binary_data/CharacterPGSet.pkl` & `multipie-1.2.9/multipie/binary_data/CharacterPGSet.pkl`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/binary_data/ClebschGordanPGSet.pkl` & `multipie-1.2.9/multipie/binary_data/ClebschGordanPGSet.pkl`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/binary_data/HarmonicsPGSet.pkl` & `multipie-1.2.9/multipie/binary_data/HarmonicsPGSet.pkl`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/binary_data/ResponseTensorPGSet.pkl` & `multipie-1.2.9/multipie/binary_data/ResponseTensorPGSet.pkl`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/binary_data/SymmetryOperationGSet.pkl` & `multipie-1.2.9/multipie/binary_data/SymmetryOperationGSet.pkl`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/binary_data/VirtualClusterPGSet.pkl` & `multipie-1.2.9/multipie/binary_data/VirtualClusterPGSet.pkl`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/binary_data/WyckoffGSet.pkl` & `multipie-1.2.9/multipie/binary_data/WyckoffGSet.pkl`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/character/character_pg.py` & `multipie-1.2.9/multipie/character/character_pg.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/character/character_pg_set.py` & `multipie-1.2.9/multipie/character/character_pg_set.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/clebsch_gordan/clebsch_gordan_pg.py` & `multipie-1.2.9/multipie/clebsch_gordan/clebsch_gordan_pg.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/clebsch_gordan/clebsch_gordan_pg_set.py` & `multipie-1.2.9/multipie/clebsch_gordan/clebsch_gordan_pg_set.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/const.py` & `multipie-1.2.9/multipie/const.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/data/data_atomic_multipoles.py` & `multipie-1.2.9/multipie/data/data_atomic_multipoles.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/data/data_cartesian_to_ch_harmoncis.py` & `multipie-1.2.9/multipie/data/data_cartesian_to_ch_harmoncis.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/data/data_character_table.py` & `multipie-1.2.9/multipie/data/data_character_table.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/data/data_compatibility_relation.py` & `multipie-1.2.9/multipie/data/data_compatibility_relation.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/data/data_harmonics.py` & `multipie-1.2.9/multipie/data/data_harmonics.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/data/data_harmonics_real.py` & `multipie-1.2.9/multipie/data/data_harmonics_real.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/data/data_no_space_group.py` & `multipie-1.2.9/multipie/data/data_no_space_group.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/data/data_product_decomp.py` & `multipie-1.2.9/multipie/data/data_product_decomp.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/data/data_symmetry_operation_pg.py` & `multipie-1.2.9/multipie/data/data_symmetry_operation_pg.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/data/data_symmetry_operation_sg.py` & `multipie-1.2.9/multipie/data/data_symmetry_operation_sg.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/data/data_tag_harmonics_alias.py` & `multipie-1.2.9/multipie/data/data_tag_harmonics_alias.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/data/data_tag_irrep.py` & `multipie-1.2.9/multipie/data/data_tag_irrep.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/data/data_tag_point_group.py` & `multipie-1.2.9/multipie/data/data_tag_point_group.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/data/data_tag_space_group.py` & `multipie-1.2.9/multipie/data/data_tag_space_group.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/data/data_transform_matrix.py` & `multipie-1.2.9/multipie/data/data_transform_matrix.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/data/data_virtual_cluster_real.py` & `multipie-1.2.9/multipie/data/data_virtual_cluster_real.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/data/data_wyckoff_pg.py` & `multipie-1.2.9/multipie/data/data_wyckoff_pg.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/data/data_wyckoff_sg.py` & `multipie-1.2.9/multipie/data/data_wyckoff_sg.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/group/point_group.py` & `multipie-1.2.9/multipie/group/point_group.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/group/space_group.py` & `multipie-1.2.9/multipie/group/space_group.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/harmonics/harmonics.py` & `multipie-1.2.9/multipie/harmonics/harmonics.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/harmonics/harmonics_complex_pg.py` & `multipie-1.2.9/multipie/harmonics/harmonics_complex_pg.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/harmonics/harmonics_complex_pg_set.py` & `multipie-1.2.9/multipie/harmonics/harmonics_complex_pg_set.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/harmonics/harmonics_pg.py` & `multipie-1.2.9/multipie/harmonics/harmonics_pg.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/harmonics/harmonics_pg_set.py` & `multipie-1.2.9/multipie/harmonics/harmonics_pg_set.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/harmonics/util/equivalent_operator.py` & `multipie-1.2.9/multipie/harmonics/util/equivalent_operator.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/model/construct_model.py` & `multipie-1.2.9/multipie/model/construct_model.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/model/create_model.py` & `multipie-1.2.9/multipie/model/create_model.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """
 create model view, info, and basis.
 """
+import pickle
+
 from multipie.model.material_model import MaterialModel
 from multipie.model.multipie_manager import MultiPieManager
 from multipie.model.symmetry_adapted_model import SymmetryAdaptedModel
 from multipie.model.util.create_pdf import ModelPDF
 
 
 # ==================================================
@@ -48,21 +50,39 @@
     samb = SymmetryAdaptedModel(cmodel, mpm=mpm, head=head)
     samb_dict = samb.create_dict()
     mpm.write(model_name + "_samb.py", samb_dict, SymmetryAdaptedModel._header(), model_name)
 
     # create matrix (real space)
     mpm.log("creating SAMB matrix (real space) ... ", None)
     samb_matrix_real = samb.create_matrix(fmt="sympy")
-    mpm.write(model_name + "_matrix.py", samb_matrix_real, SymmetryAdaptedModel._matrix_header(), model_name)
+
+    if model_dict["option"]["binary_output"]:
+        filename = model_name + "_matrix.pkl"
+        full = mpm.filename(filename)
+        f = open(full, "wb")
+        pickle.dump(samb_matrix_real, f)
+        f.close()
+        mpm.log(f"  * wrote '{filename}'.", None)
+    else:
+        mpm.write(model_name + "_matrix.py", samb_matrix_real, SymmetryAdaptedModel._matrix_header(), model_name)
 
     # create matrix (momentum space)
     if not cmodel["info"]["molecule"] and cmodel["info"]["generate"]["fourier_transform"]:
         mpm.log("creating SAMB matrix (momentum space) ... ", None)
         samb_matrix = samb.create_matrix_k(full=True, fmt="sympy")
-        mpm.write(model_name + "_matrix_k.py", samb_matrix, SymmetryAdaptedModel._matrix_header_k(), model_name)
+
+        if model_dict["option"]["binary_output"]:
+            filename = model_name + "_matrix_k.pkl"
+            full = mpm.filename(filename)
+            f = open(full, "wb")
+            pickle.dump(samb_matrix, f)
+            f.close()
+            mpm.log(f"  * wrote '{filename}'.", None)
+        else:
+            mpm.write(model_name + "_matrix_k.py", samb_matrix, SymmetryAdaptedModel._matrix_header_k(), model_name)
 
     # create LaTeX and PDF.
     if mpm.pdf:
         mpm.log("creating LaTeX and PDF ... ", None)
         ModelPDF(cmodel, samb_dict, mpm)
 
     mpm.formatter()
```

### Comparing `multipie-1.2.8/multipie/model/material_model.py` & `multipie-1.2.9/multipie/model/material_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 - spinful* : spinful basis ? (bool), [False].
 - cell* : unit-cell constants (dict) { "a", "b", "c", "alpha", "beta", "gamma" }, [a=b=c=1,alpha=beta=gamma=90].
 - option*
   - view* : view point (int list), [None].
   - view_mode* : mode for QtDraw file (str) ("standard"/"arrow"/"debug"), ["standard"].
   - output* : output folder (str), [model name].
   - minimal_samb* (bool) : minimal output in _samb.pdf ? [True].
+  - binary_output* (bool) : output matrix data in binary format ? [False].
 - generate*
   - model_type* : model type (str), ("tight_binding"/"phonon"), ["tight_binding"].
   - time_reversal_type* : time-reversal type (str), ("electric"/"magnetic"/"both"), ["electric"].
   - irrep* : irrep. (str list), [identity irrep.] (empty list is for all irreps.), [None].
   - fourier_transform* : create fourier transformed SAMB ? [False].
   - toroidal_priority* : create toroidal multipoles (G,T) in high priority ? [False].
 - k_point* : k-point (dict) {name: "position"}, [{ "Γ": "[0,0,0]", "X": "[1/2,0,0]" }].
@@ -66,14 +67,15 @@
     - a2* : unit cell a2 vector
     - a3* : unit cell a3 vector
     - option :
         - view : view index
         - view_mode : QtDraw mode, standard/arrow/debug
         - output : output directory.
         - minimal_samb : output minimal SAMB ?
+        - binary_output : output matrix data in binary format ?
     - generate :
         - model_type : tight_binding/phonon
         - time_reversal_type : electric/magnetic/both
         - irrep : irrep list
         - fourier_transform* : create fourier transformed SAMB ?
         - toroidal_priority : create toroidal multipoles (G,T) in high priority ?
     - k_point* : representative k points
@@ -155,14 +157,15 @@
             "a2": "[0.0, 1.0, 0.0]",
             "a3": "[0.0, 0.0, 1.0]",
             "option": {
                 "view": [0, 0, 1],
                 "view_mode": "standard",
                 "output": "material_model",
                 "minimal_samb": True,
+                "binary_output": False,
             },
             "generate": {
                 "model_type": "tight_binding",
                 "time_reversal_type": "electric",
                 "irrep": ["A"],
                 "fourier_transform": False,
                 "toroidal_priority": False,
@@ -211,17 +214,15 @@
 
         info["spinful"] = dic["spinful"]
         info["option"] = dic["option"]
         info["model"] = dic["model"]
         info["group"] = (str(self._mpm.group), self._group_str(info["molecule"]))
         info["crystal"] = self._mpm.group.tag.crystal
 
-        cell_info = cell_transform_matrix(
-            cell=dic["cell"], crystal=info["crystal"], translation=False
-        )
+        cell_info = cell_transform_matrix(cell=dic["cell"], crystal=info["crystal"], translation=False)
         self._cell = cell_info[0]
         self._volume = cell_info[1]
         self._A = cell_info[2]
         self._G = cell_info[3]
         self._A_norm = cell_info[4]
         if not info["molecule"]:
             info["cell"] = self._cell
@@ -335,17 +336,15 @@
         cluster_site_n = len(default_style["site"])
         cluster_bond_n = len(default_style["bond"])
 
         # plot sites.
         for pos, (site_name, pset) in name["site_name"].items():
             head, idx = name["site"][site_name]
             cluster_no = int(name["alias"][head].split("_")[1])
-            prop_no = (
-                cluster_no - 1 if cluster_no < cluster_site_n else cluster_site_n - 1
-            )
+            prop_no = cluster_no - 1 if cluster_no < cluster_site_n else cluster_site_n - 1
             color, size, opacity = default_style["site"][prop_no]
             if n_pset > 1:
                 cluster_name = f"S{cluster_no}({pset})"
             else:
                 cluster_name = f"S{cluster_no}"
             mp = data["site"][site_name][1]
             if mode == "debug":
@@ -371,17 +370,15 @@
                     opacity=0.3,
                 )
 
         # plot bonds.
         for bond, (bond_name, pset) in name["bond_name"].items():
             head, idx = name["bond"][bond_name]
             cluster_no = int(name["alias"][head].split("_")[1])
-            prop_no = (
-                cluster_no - 1 if cluster_no < cluster_bond_n else cluster_bond_n - 1
-            )
+            prop_no = cluster_no - 1 if cluster_no < cluster_bond_n else cluster_bond_n - 1
             (c1, c2), width, opacity = default_style["bond"][prop_no]
             if n_pset > 1:
                 cluster_name = f"B{cluster_no}({pset})"
             else:
                 cluster_name = f"B{cluster_no}"
             _, mp, ij, _, _ = data["bond"][bond_name]
 
@@ -435,17 +432,15 @@
         crystal = info["crystal"]
 
         rep_site = {}
         for name, (pos, orb_list) in info["site"].items():
             wp = str(self._mpm.group.find_wyckoff_position(str(pos)))
             pos = str(NSArray(pos))
             orb_list = split_orb_list_rank_block(
-                sort_orb_list(
-                    parse_orb_list(orb_list, spinful, crystal), spinful, crystal
-                ),
+                sort_orb_list(parse_orb_list(orb_list, spinful, crystal), spinful, crystal),
                 spinful,
                 crystal,
             )
             sym = self._mpm.group.wyckoff.site_symmetry(wp)
             if not info["molecule"]:
                 pos = str(self._mpm.group.shift_home_unit_cell(pos))
             rep_site[name] = (pos, wp, orb_list, sym)
@@ -502,17 +497,15 @@
                             ss,
                             self._mapping_str(mp),
                         )
                 else:
                     cell_site[f"{site}_{rsite_no+1}"] = (s, self._mapping_str(mp))
                 name_site[sname] = (site, rsite_no + 1)
                 orbital[sname] = orb_list
-            assert (
-                data_site[f"site_{site_no+1:03d}"][1][0] == 0
-            ), f"first SO is not identity operation, {mp}"
+            assert data_site[f"site_{site_no+1:03d}"][1][0] == 0, f"first SO is not identity operation, {mp}"
             for rsite_no in range(basic_num):
                 s_no = site_no + rsite_no
                 sname = f"site_{s_no+1:03d}"
                 for pset in range(n_pset):
                     s = position[pset * basic_num + rsite_no]
                     site_to_name[s] = (sname, pset + 1)
             site_no = site_no + basic_num
@@ -532,17 +525,15 @@
         for l, lst in d.items():
             sname, orbs = lst[0]
             if len(lst) > 1:
                 for sname_, orbs_ in lst[1:]:
                     if orbs != orbs_:
                         s1 = name_site[sname][0]
                         s2 = name_site[sname_][0]
-                        raise Exception(
-                            f"invalid orbitals are given, {s1} {orbs} != {s2} {orbs_}."
-                        )
+                        raise Exception(f"invalid orbitals are given, {s1} {orbs} != {s2} {orbs_}.")
 
         info["cell_site"].update(cell_site)
 
         name["alias"].update(alias),
         name["site"].update(name_site)
         name["site_name"].update(site_to_name)
 
@@ -717,35 +708,29 @@
                 assert ht_no[0] >= ht_no[1], f"site indices are wrong, {ht_no}"
                 vc = f"{v}@{c}"
                 data_bond[bname] = (vc, mp, ht_no, str(v), b)
                 br = str(NSArray(vc).regular_direction()).split("@")[0]
                 b_vector[br] = b_vector.get(br, []) + [bname]
                 if n_pset > 1:
                     for pset in range(n_pset):
-                        v, c = NSArray(bonds[pset * basic_num + rbond_no]).convert_bond(
-                            "bond"
-                        )
+                        v, c = NSArray(bonds[pset * basic_num + rbond_no]).convert_bond("bond")
                         vc1 = f"{v}@{c}"
                         cell_bond[f"{rbname}_{rbond_no+1}({pset+1})"] = (
                             vc1,
                             self._mapping_str(mp),
                         )
                 else:
                     cell_bond[f"{rbname}_{rbond_no+1}"] = (vc, self._mapping_str(mp))
                 name_bond[bname] = (rbname, rbond_no + 1)
-            assert (
-                data_bond[f"bond_{bond_no:03d}"][1][0] == 0
-            ), f"first SO is not identity operation, {mp}"
+            assert data_bond[f"bond_{bond_no:03d}"][1][0] == 0, f"first SO is not identity operation, {mp}"
             for rbond_no in range(basic_num):
                 b_no = bond_no + rbond_no
                 bname = f"bond_{b_no:03d}"
                 for pset in range(n_pset):
-                    v, c = NSArray(bonds[pset * basic_num + rbond_no]).convert_bond(
-                        "bond"
-                    )
+                    v, c = NSArray(bonds[pset * basic_num + rbond_no]).convert_bond("bond")
                     b = f"{v}@{c}"
                     bond_to_name[b] = (bname, pset + 1)
             bond_no = bond_no + basic_num
 
             # replace same bond vector.
             for lst in b_vector.values():
                 top = lst[0]
@@ -766,41 +751,34 @@
         data["bond"].update(data_bond)
 
     # ==================================================
     def _set_matrix(self, name, data, orbital, ket_dict):
         cluster_atomic = {}
         atomic_braket = {}
 
-        ij_list = [v[2] for v in data["site"].values()] + [
-            v[2] for v in data["bond"].values()
-        ]
+        ij_list = [v[2] for v in data["site"].values()] + [v[2] for v in data["bond"].values()]
 
         for ij in ij_list:
             i, j = ij
             site_i = f"site_{i+1:03d}"
             site_j = f"site_{j+1:03d}"
             Si = name["site"][list(data["site"].keys())[i]][0]
             Sj = name["site"][list(data["site"].keys())[j]][0]
             if Si == Sj:
                 orbs_i = orbital[site_i]
                 orbs_j = orbs_i
                 braket = sum(
-                    [
-                        [(orb, orbs_j[j]) for j in range(i, len(orbs_i))]
-                        for i, orb in enumerate(orbs_i)
-                    ],
+                    [[(orb, orbs_j[j]) for j in range(i, len(orbs_i))] for i, orb in enumerate(orbs_i)],
                     [],
                 )
             else:
                 orbs_i = orbital[site_i]
                 orbs_j = orbital[site_j]
                 braket = sum([[(orbi, orbj) for orbj in orbs_j] for orbi in orbs_i], [])
-            cluster_atomic[ij] = [
-                (f"{bra}:{ket}", (bra[0], i), (ket[0], j)) for bra, ket in braket
-            ]
+            cluster_atomic[ij] = [(f"{bra}:{ket}", (bra[0], i), (ket[0], j)) for bra, ket in braket]
             for bra, ket in braket:
                 atomic_braket[f"{bra}:{ket}"] = (bra, ket)
 
         rs = {k: f"M_{i+1:03d}" for i, k in enumerate(atomic_braket.keys())}
         d = {rs[k]: v for k, v in atomic_braket.items()}
         atomic_braket = d
 
@@ -865,17 +843,15 @@
         Returns:
             NSArray: all sites for given grid.
         """
         if info["molecule"]:
             site = self._mpm.group.transform_site(site, remove_duplicate=True)
             return site
 
-        site = self._mpm.group.transform_site(
-            site, shift=True, remove_duplicate=True, plus_set=True
-        )
+        site = self._mpm.group.transform_site(site, shift=True, remove_duplicate=True, plus_set=True)
 
         if repeat:
             offset = detail["cell_range"][::2]
             N = [i - j for i, j in zip(detail["cell_range"][1::2], offset)]
             ns = N[0] * N[1] * N[2]
 
             igrid = NSArray.igrid(N, offset)
@@ -956,14 +932,15 @@
 
         if "option" not in d.keys():
             d["option"] = {
                 "view": None,
                 "view_mode": "standard",
                 "output": model,
                 "minimal_samb": True,
+                "binary_output": False,
             }
         else:
             if "view" not in d["option"].keys():
                 d["option"]["view"] = None
             if "view_mode" not in d["option"].keys():
                 d["option"]["view_mode"] = "standard"
             if "output" not in d["option"].keys():
```

### Comparing `multipie-1.2.8/multipie/model/multipie_manager.py` & `multipie-1.2.9/multipie/model/multipie_manager.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/model/symmetry_adapted_model.py` & `multipie-1.2.9/multipie/model/symmetry_adapted_model.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/model/util/create_pdf.py` & `multipie-1.2.9/multipie/model/util/create_pdf.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/model/util/symmetry_adapted_model_util.py` & `multipie-1.2.9/multipie/model/util/symmetry_adapted_model_util.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/multipole/base/base_atomic_multipole_dataset.py` & `multipie-1.2.9/multipie/multipole/base/base_atomic_multipole_dataset.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/multipole/base/base_atomic_multipole_set.py` & `multipie-1.2.9/multipie/multipole/base/base_atomic_multipole_set.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/multipole/util/atomic_orbital_util.py` & `multipie-1.2.9/multipie/multipole/util/atomic_orbital_util.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/multipole/util/atomic_samb_util.py` & `multipie-1.2.9/multipie/multipole/util/atomic_samb_util.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/multipole/util/multipole_util.py` & `multipie-1.2.9/multipie/multipole/util/multipole_util.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/multipole/util/pauli.py` & `multipie-1.2.9/multipie/multipole/util/pauli.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/multipole/util/spin_orbital_basis.py` & `multipie-1.2.9/multipie/multipole/util/spin_orbital_basis.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/multipole/util/structure_samb_util.py` & `multipie-1.2.9/multipie/multipole/util/structure_samb_util.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/multipole/util/z_samb_util.py` & `multipie-1.2.9/multipie/multipole/util/z_samb_util.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/response_tensor/response_tensor_pg.py` & `multipie-1.2.9/multipie/response_tensor/response_tensor_pg.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/response_tensor/response_tensor_pg_set.py` & `multipie-1.2.9/multipie/response_tensor/response_tensor_pg_set.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/response_tensor/util/response_tensor_util.py` & `multipie-1.2.9/multipie/response_tensor/util/response_tensor_util.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/scripts/create_binary.py` & `multipie-1.2.9/multipie/scripts/create_binary.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/scripts/create_samb.py` & `multipie-1.2.9/multipie/scripts/create_samb.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/symmetry_operation/symmetry_operation.py` & `multipie-1.2.9/multipie/symmetry_operation/symmetry_operation.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/symmetry_operation/symmetry_operation_g.py` & `multipie-1.2.9/multipie/symmetry_operation/symmetry_operation_g.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/symmetry_operation/symmetry_operation_g_set.py` & `multipie-1.2.9/multipie/symmetry_operation/symmetry_operation_g_set.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/symmetry_operation/util/symmetry_operation_util.py` & `multipie-1.2.9/multipie/symmetry_operation/util/symmetry_operation_util.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/tag/tag.py` & `multipie-1.2.9/multipie/tag/tag.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/tag/tag_group.py` & `multipie-1.2.9/multipie/tag/tag_group.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/tag/tag_irrep.py` & `multipie-1.2.9/multipie/tag/tag_irrep.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/tag/tag_list.py` & `multipie-1.2.9/multipie/tag/tag_list.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/tag/tag_multipole.py` & `multipie-1.2.9/multipie/tag/tag_multipole.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/tag/tag_response_tensor.py` & `multipie-1.2.9/multipie/tag/tag_response_tensor.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/tag/tag_symmetry_operation.py` & `multipie-1.2.9/multipie/tag/tag_symmetry_operation.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/tag/tag_wyckoff.py` & `multipie-1.2.9/multipie/tag/tag_wyckoff.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/virtual_cluster/virtual_cluster_pg.py` & `multipie-1.2.9/multipie/virtual_cluster/virtual_cluster_pg.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/virtual_cluster/virtual_cluster_pg_set.py` & `multipie-1.2.9/multipie/virtual_cluster/virtual_cluster_pg_set.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/wyckoff/wyckoff_g.py` & `multipie-1.2.9/multipie/wyckoff/wyckoff_g.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie/wyckoff/wyckoff_g_set.py` & `multipie-1.2.9/multipie/wyckoff/wyckoff_g_set.py`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/multipie.egg-info/PKG-INFO` & `multipie-1.2.9/multipie.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multipie
-Version: 1.2.8
+Version: 1.2.9
 Summary: A python library for crystallographic symmetry operations and Symmetry-Adapted Multipole Basis (SAMB).
 Home-page: https://github.com/CMT-MU/MultiPie
 Author: Hiroaki Kusunose and Rikuto Oiwa
 Author-email: hiroaki.kusunose@gmail.com, ro.qp.07@gmail.com
 License: MIT
 Keywords: group theory,condensed matter,materials science,basis
 Requires-Python: >=3.9
```

### Comparing `multipie-1.2.8/multipie.egg-info/SOURCES.txt` & `multipie-1.2.9/multipie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `multipie-1.2.8/setup.cfg` & `multipie-1.2.9/setup.cfg`

 * *Files identical despite different names*

