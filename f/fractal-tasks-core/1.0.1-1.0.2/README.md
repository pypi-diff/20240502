# Comparing `tmp/fractal_tasks_core-1.0.1.tar.gz` & `tmp/fractal_tasks_core-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractal_tasks_core-1.0.1.tar", max compression
+gzip compressed data, was "fractal_tasks_core-1.0.2.tar", max compression
```

## Comparing `fractal_tasks_core-1.0.1.tar` & `fractal_tasks_core-1.0.2.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0     1584 2024-04-30 10:58:01.120479 fractal_tasks_core-1.0.1/LICENSE
--rw-r--r--   0        0        0     6042 2024-04-30 10:58:01.120479 fractal_tasks_core-1.0.1/README.md
--rw-r--r--   0        0        0       32 2024-04-30 10:58:01.124479 fractal_tasks_core-1.0.1/fractal_tasks_core/.gitignore
--rw-r--r--   0        0        0    64149 2024-04-30 10:58:01.124479 fractal_tasks_core-1.0.1/fractal_tasks_core/__FRACTAL_MANIFEST__.json
--rw-r--r--   0        0        0      198 2024-04-30 10:58:01.124479 fractal_tasks_core-1.0.1/fractal_tasks_core/__init__.py
--rw-r--r--   0        0        0       87 2024-04-30 10:58:01.124479 fractal_tasks_core-1.0.1/fractal_tasks_core/cellvoyager/__init__.py
--rw-r--r--   0        0        0     4552 2024-04-30 10:58:01.124479 fractal_tasks_core-1.0.1/fractal_tasks_core/cellvoyager/filenames.py
--rw-r--r--   0        0        0    15388 2024-04-30 10:58:01.124479 fractal_tasks_core-1.0.1/fractal_tasks_core/cellvoyager/metadata.py
--rw-r--r--   0        0        0     3289 2024-04-30 10:58:01.124479 fractal_tasks_core-1.0.1/fractal_tasks_core/cellvoyager/wells.py
--rw-r--r--   0        0        0    16713 2024-04-30 10:58:01.124479 fractal_tasks_core-1.0.1/fractal_tasks_core/channels.py
--rw-r--r--   0        0        0      108 2024-04-30 10:58:01.124479 fractal_tasks_core-1.0.1/fractal_tasks_core/dev/README.md
--rw-r--r--   0        0        0       98 2024-04-30 10:58:01.124479 fractal_tasks_core-1.0.1/fractal_tasks_core/dev/__init__.py
--rw-r--r--   0        0        0     4607 2024-04-30 10:58:01.124479 fractal_tasks_core-1.0.1/fractal_tasks_core/dev/check_manifest.py
--rw-r--r--   0        0        0     5368 2024-04-30 10:58:01.124479 fractal_tasks_core-1.0.1/fractal_tasks_core/dev/create_manifest.py
--rw-r--r--   0        0        0     8166 2024-04-30 10:58:01.124479 fractal_tasks_core-1.0.1/fractal_tasks_core/dev/lib_args_schemas.py
--rw-r--r--   0        0        0     6406 2024-04-30 10:58:01.124479 fractal_tasks_core-1.0.1/fractal_tasks_core/dev/lib_descriptions.py
--rw-r--r--   0        0        0     3260 2024-04-30 10:58:01.124479 fractal_tasks_core-1.0.1/fractal_tasks_core/dev/lib_signature_constraints.py
--rw-r--r--   0        0        0     2827 2024-04-30 10:58:01.124479 fractal_tasks_core-1.0.1/fractal_tasks_core/dev/lib_task_docs.py
--rw-r--r--   0        0        0     2273 2024-04-30 10:58:01.124479 fractal_tasks_core-1.0.1/fractal_tasks_core/dev/lib_titles.py
--rw-r--r--   0        0        0     3624 2024-04-30 10:58:01.124479 fractal_tasks_core-1.0.1/fractal_tasks_core/dev/task_list.py
--rw-r--r--   0        0        0     2660 2024-04-30 10:58:01.124479 fractal_tasks_core-1.0.1/fractal_tasks_core/dev/task_models.py
--rw-r--r--   0        0        0     5189 2024-04-30 10:58:01.124479 fractal_tasks_core-1.0.1/fractal_tasks_core/labels.py
--rw-r--r--   0        0        0     9005 2024-04-30 10:58:01.124479 fractal_tasks_core-1.0.1/fractal_tasks_core/masked_loading.py
--rw-r--r--   0        0        0      508 2024-04-30 10:58:01.124479 fractal_tasks_core-1.0.1/fractal_tasks_core/ngff/__init__.py
--rw-r--r--   0        0        0    12849 2024-04-30 10:58:01.124479 fractal_tasks_core-1.0.1/fractal_tasks_core/ngff/specs.py
--rw-r--r--   0        0        0     3974 2024-04-30 10:58:01.124479 fractal_tasks_core-1.0.1/fractal_tasks_core/ngff/zarr_utils.py
--rw-r--r--   0        0        0     3788 2024-04-30 10:58:01.124479 fractal_tasks_core-1.0.1/fractal_tasks_core/pyramids.py
--rw-r--r--   0        0        0      185 2024-04-30 10:58:01.124479 fractal_tasks_core-1.0.1/fractal_tasks_core/roi/__init__.py
--rw-r--r--   0        0        0     4501 2024-04-30 10:58:01.124479 fractal_tasks_core-1.0.1/fractal_tasks_core/roi/_overlaps_common.py
--rw-r--r--   0        0        0     1327 2024-04-30 10:58:01.124479 fractal_tasks_core-1.0.1/fractal_tasks_core/roi/load_region.py
--rw-r--r--   0        0        0    18609 2024-04-30 10:58:01.128479 fractal_tasks_core-1.0.1/fractal_tasks_core/roi/v1.py
--rw-r--r--   0        0        0     4910 2024-04-30 10:58:01.128479 fractal_tasks_core-1.0.1/fractal_tasks_core/roi/v1_checks.py
--rw-r--r--   0        0        0    13273 2024-04-30 10:58:01.128479 fractal_tasks_core-1.0.1/fractal_tasks_core/roi/v1_overlaps.py
--rw-r--r--   0        0        0     3394 2024-04-30 10:58:01.128479 fractal_tasks_core-1.0.1/fractal_tasks_core/tables/__init__.py
--rw-r--r--   0        0        0    11579 2024-04-30 10:58:01.128479 fractal_tasks_core-1.0.1/fractal_tasks_core/tables/v1.py
--rw-r--r--   0        0        0       72 2024-04-30 10:58:01.128479 fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/__init__.py
--rw-r--r--   0        0        0     8178 2024-04-30 10:58:01.128479 fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/_registration_utils.py
--rw-r--r--   0        0        0     2407 2024-04-30 10:58:01.128479 fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/_utils.py
--rw-r--r--   0        0        0     7545 2024-04-30 10:58:01.128479 fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/_zarr_utils.py
--rw-r--r--   0        0        0    14906 2024-04-30 10:58:01.128479 fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/apply_registration_to_image.py
--rw-r--r--   0        0        0     9394 2024-04-30 10:58:01.128479 fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/calculate_registration_image_based.py
--rw-r--r--   0        0        0    27516 2024-04-30 10:58:01.128479 fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/cellpose_segmentation.py
--rw-r--r--   0        0        0     8458 2024-04-30 10:58:01.128479 fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/cellpose_transforms.py
--rw-r--r--   0        0        0     7384 2024-04-30 10:58:01.128479 fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/cellvoyager_to_ome_zarr_compute.py
--rw-r--r--   0        0        0    18564 2024-04-30 10:58:01.128479 fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/cellvoyager_to_ome_zarr_init.py
--rw-r--r--   0        0        0    21248 2024-04-30 10:58:01.128479 fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/cellvoyager_to_ome_zarr_init_multiplex.py
--rw-r--r--   0        0        0    11258 2024-04-30 10:58:01.128479 fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/copy_ome_zarr_hcs_plate.py
--rw-r--r--   0        0        0     6421 2024-04-30 10:58:01.128479 fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/find_registration_consensus.py
--rw-r--r--   0        0        0    10735 2024-04-30 10:58:01.128479 fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/illumination_correction.py
--rw-r--r--   0        0        0     3686 2024-04-30 10:58:01.128479 fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/image_based_registration_hcs_init.py
--rw-r--r--   0        0        0    11752 2024-04-30 10:58:01.128479 fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/import_ome_zarr.py
--rw-r--r--   0        0        0     3066 2024-04-30 10:58:01.128479 fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/init_group_by_well_for_multiplexing.py
--rw-r--r--   0        0        0     4903 2024-04-30 10:58:01.128479 fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/io_models.py
--rw-r--r--   0        0        0     6239 2024-04-30 10:58:01.128479 fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/maximum_intensity_projection.py
--rw-r--r--   0        0        0    24816 2024-04-30 10:58:01.128479 fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/napari_workflows_wrapper.py
--rw-r--r--   0        0        0     7136 2024-04-30 10:58:01.128479 fractal_tasks_core-1.0.1/fractal_tasks_core/upscale_array.py
--rw-r--r--   0        0        0     6101 2024-04-30 10:58:01.128479 fractal_tasks_core-1.0.1/fractal_tasks_core/utils.py
--rw-r--r--   0        0        0     3890 2024-04-30 10:58:01.128479 fractal_tasks_core-1.0.1/fractal_tasks_core/zarr_utils.py
--rw-r--r--   0        0        0     3403 2024-04-30 10:58:01.132479 fractal_tasks_core-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     8096 1970-01-01 00:00:00.000000 fractal_tasks_core-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1584 2024-05-02 14:41:52.040443 fractal_tasks_core-1.0.2/LICENSE
+-rw-r--r--   0        0        0     6042 2024-05-02 14:41:52.040443 fractal_tasks_core-1.0.2/README.md
+-rw-r--r--   0        0        0       32 2024-05-02 14:41:52.044443 fractal_tasks_core-1.0.2/fractal_tasks_core/.gitignore
+-rw-r--r--   0        0        0    64149 2024-05-02 14:41:52.044443 fractal_tasks_core-1.0.2/fractal_tasks_core/__FRACTAL_MANIFEST__.json
+-rw-r--r--   0        0        0      198 2024-05-02 14:41:52.044443 fractal_tasks_core-1.0.2/fractal_tasks_core/__init__.py
+-rw-r--r--   0        0        0       87 2024-05-02 14:41:52.044443 fractal_tasks_core-1.0.2/fractal_tasks_core/cellvoyager/__init__.py
+-rw-r--r--   0        0        0     4552 2024-05-02 14:41:52.044443 fractal_tasks_core-1.0.2/fractal_tasks_core/cellvoyager/filenames.py
+-rw-r--r--   0        0        0    15388 2024-05-02 14:41:52.044443 fractal_tasks_core-1.0.2/fractal_tasks_core/cellvoyager/metadata.py
+-rw-r--r--   0        0        0     3289 2024-05-02 14:41:52.044443 fractal_tasks_core-1.0.2/fractal_tasks_core/cellvoyager/wells.py
+-rw-r--r--   0        0        0    16713 2024-05-02 14:41:52.044443 fractal_tasks_core-1.0.2/fractal_tasks_core/channels.py
+-rw-r--r--   0        0        0      108 2024-05-02 14:41:52.044443 fractal_tasks_core-1.0.2/fractal_tasks_core/dev/README.md
+-rw-r--r--   0        0        0       98 2024-05-02 14:41:52.044443 fractal_tasks_core-1.0.2/fractal_tasks_core/dev/__init__.py
+-rw-r--r--   0        0        0     4607 2024-05-02 14:41:52.044443 fractal_tasks_core-1.0.2/fractal_tasks_core/dev/check_manifest.py
+-rw-r--r--   0        0        0     5368 2024-05-02 14:41:52.044443 fractal_tasks_core-1.0.2/fractal_tasks_core/dev/create_manifest.py
+-rw-r--r--   0        0        0     8166 2024-05-02 14:41:52.044443 fractal_tasks_core-1.0.2/fractal_tasks_core/dev/lib_args_schemas.py
+-rw-r--r--   0        0        0     6406 2024-05-02 14:41:52.044443 fractal_tasks_core-1.0.2/fractal_tasks_core/dev/lib_descriptions.py
+-rw-r--r--   0        0        0     3260 2024-05-02 14:41:52.044443 fractal_tasks_core-1.0.2/fractal_tasks_core/dev/lib_signature_constraints.py
+-rw-r--r--   0        0        0     2827 2024-05-02 14:41:52.044443 fractal_tasks_core-1.0.2/fractal_tasks_core/dev/lib_task_docs.py
+-rw-r--r--   0        0        0     2273 2024-05-02 14:41:52.044443 fractal_tasks_core-1.0.2/fractal_tasks_core/dev/lib_titles.py
+-rw-r--r--   0        0        0     3624 2024-05-02 14:41:52.044443 fractal_tasks_core-1.0.2/fractal_tasks_core/dev/task_list.py
+-rw-r--r--   0        0        0     2660 2024-05-02 14:41:52.044443 fractal_tasks_core-1.0.2/fractal_tasks_core/dev/task_models.py
+-rw-r--r--   0        0        0     5189 2024-05-02 14:41:52.044443 fractal_tasks_core-1.0.2/fractal_tasks_core/labels.py
+-rw-r--r--   0        0        0     9005 2024-05-02 14:41:52.044443 fractal_tasks_core-1.0.2/fractal_tasks_core/masked_loading.py
+-rw-r--r--   0        0        0      508 2024-05-02 14:41:52.044443 fractal_tasks_core-1.0.2/fractal_tasks_core/ngff/__init__.py
+-rw-r--r--   0        0        0    12849 2024-05-02 14:41:52.044443 fractal_tasks_core-1.0.2/fractal_tasks_core/ngff/specs.py
+-rw-r--r--   0        0        0     3974 2024-05-02 14:41:52.044443 fractal_tasks_core-1.0.2/fractal_tasks_core/ngff/zarr_utils.py
+-rw-r--r--   0        0        0     3788 2024-05-02 14:41:52.044443 fractal_tasks_core-1.0.2/fractal_tasks_core/pyramids.py
+-rw-r--r--   0        0        0      185 2024-05-02 14:41:52.044443 fractal_tasks_core-1.0.2/fractal_tasks_core/roi/__init__.py
+-rw-r--r--   0        0        0     4501 2024-05-02 14:41:52.044443 fractal_tasks_core-1.0.2/fractal_tasks_core/roi/_overlaps_common.py
+-rw-r--r--   0        0        0     1327 2024-05-02 14:41:52.044443 fractal_tasks_core-1.0.2/fractal_tasks_core/roi/load_region.py
+-rw-r--r--   0        0        0    18609 2024-05-02 14:41:52.044443 fractal_tasks_core-1.0.2/fractal_tasks_core/roi/v1.py
+-rw-r--r--   0        0        0     4910 2024-05-02 14:41:52.044443 fractal_tasks_core-1.0.2/fractal_tasks_core/roi/v1_checks.py
+-rw-r--r--   0        0        0    13273 2024-05-02 14:41:52.044443 fractal_tasks_core-1.0.2/fractal_tasks_core/roi/v1_overlaps.py
+-rw-r--r--   0        0        0     3394 2024-05-02 14:41:52.044443 fractal_tasks_core-1.0.2/fractal_tasks_core/tables/__init__.py
+-rw-r--r--   0        0        0    11579 2024-05-02 14:41:52.044443 fractal_tasks_core-1.0.2/fractal_tasks_core/tables/v1.py
+-rw-r--r--   0        0        0       72 2024-05-02 14:41:52.044443 fractal_tasks_core-1.0.2/fractal_tasks_core/tasks/__init__.py
+-rw-r--r--   0        0        0     8178 2024-05-02 14:41:52.044443 fractal_tasks_core-1.0.2/fractal_tasks_core/tasks/_registration_utils.py
+-rw-r--r--   0        0        0     2407 2024-05-02 14:41:52.044443 fractal_tasks_core-1.0.2/fractal_tasks_core/tasks/_utils.py
+-rw-r--r--   0        0        0     7545 2024-05-02 14:41:52.044443 fractal_tasks_core-1.0.2/fractal_tasks_core/tasks/_zarr_utils.py
+-rw-r--r--   0        0        0    14906 2024-05-02 14:41:52.044443 fractal_tasks_core-1.0.2/fractal_tasks_core/tasks/apply_registration_to_image.py
+-rw-r--r--   0        0        0     9394 2024-05-02 14:41:52.044443 fractal_tasks_core-1.0.2/fractal_tasks_core/tasks/calculate_registration_image_based.py
+-rw-r--r--   0        0        0    27516 2024-05-02 14:41:52.044443 fractal_tasks_core-1.0.2/fractal_tasks_core/tasks/cellpose_segmentation.py
+-rw-r--r--   0        0        0     8458 2024-05-02 14:41:52.044443 fractal_tasks_core-1.0.2/fractal_tasks_core/tasks/cellpose_transforms.py
+-rw-r--r--   0        0        0     7384 2024-05-02 14:41:52.044443 fractal_tasks_core-1.0.2/fractal_tasks_core/tasks/cellvoyager_to_ome_zarr_compute.py
+-rw-r--r--   0        0        0    18564 2024-05-02 14:41:52.044443 fractal_tasks_core-1.0.2/fractal_tasks_core/tasks/cellvoyager_to_ome_zarr_init.py
+-rw-r--r--   0        0        0    21248 2024-05-02 14:41:52.044443 fractal_tasks_core-1.0.2/fractal_tasks_core/tasks/cellvoyager_to_ome_zarr_init_multiplex.py
+-rw-r--r--   0        0        0    11258 2024-05-02 14:41:52.044443 fractal_tasks_core-1.0.2/fractal_tasks_core/tasks/copy_ome_zarr_hcs_plate.py
+-rw-r--r--   0        0        0     6421 2024-05-02 14:41:52.044443 fractal_tasks_core-1.0.2/fractal_tasks_core/tasks/find_registration_consensus.py
+-rw-r--r--   0        0        0    10735 2024-05-02 14:41:52.044443 fractal_tasks_core-1.0.2/fractal_tasks_core/tasks/illumination_correction.py
+-rw-r--r--   0        0        0     3686 2024-05-02 14:41:52.044443 fractal_tasks_core-1.0.2/fractal_tasks_core/tasks/image_based_registration_hcs_init.py
+-rw-r--r--   0        0        0    11752 2024-05-02 14:41:52.044443 fractal_tasks_core-1.0.2/fractal_tasks_core/tasks/import_ome_zarr.py
+-rw-r--r--   0        0        0     3066 2024-05-02 14:41:52.044443 fractal_tasks_core-1.0.2/fractal_tasks_core/tasks/init_group_by_well_for_multiplexing.py
+-rw-r--r--   0        0        0     4903 2024-05-02 14:41:52.048442 fractal_tasks_core-1.0.2/fractal_tasks_core/tasks/io_models.py
+-rw-r--r--   0        0        0     6239 2024-05-02 14:41:52.048442 fractal_tasks_core-1.0.2/fractal_tasks_core/tasks/maximum_intensity_projection.py
+-rw-r--r--   0        0        0    24816 2024-05-02 14:41:52.048442 fractal_tasks_core-1.0.2/fractal_tasks_core/tasks/napari_workflows_wrapper.py
+-rw-r--r--   0        0        0     7136 2024-05-02 14:41:52.048442 fractal_tasks_core-1.0.2/fractal_tasks_core/upscale_array.py
+-rw-r--r--   0        0        0     6101 2024-05-02 14:41:52.048442 fractal_tasks_core-1.0.2/fractal_tasks_core/utils.py
+-rw-r--r--   0        0        0     3890 2024-05-02 14:41:52.048442 fractal_tasks_core-1.0.2/fractal_tasks_core/zarr_utils.py
+-rw-r--r--   0        0        0     3403 2024-05-02 14:41:52.048442 fractal_tasks_core-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     8096 1970-01-01 00:00:00.000000 fractal_tasks_core-1.0.2/PKG-INFO
```

### Comparing `fractal_tasks_core-1.0.1/LICENSE` & `fractal_tasks_core-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.1/README.md` & `fractal_tasks_core-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.1/fractal_tasks_core/__FRACTAL_MANIFEST__.json` & `fractal_tasks_core-1.0.2/fractal_tasks_core/__FRACTAL_MANIFEST__.json`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.1/fractal_tasks_core/cellvoyager/filenames.py` & `fractal_tasks_core-1.0.2/fractal_tasks_core/cellvoyager/filenames.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.1/fractal_tasks_core/cellvoyager/metadata.py` & `fractal_tasks_core-1.0.2/fractal_tasks_core/cellvoyager/metadata.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.1/fractal_tasks_core/cellvoyager/wells.py` & `fractal_tasks_core-1.0.2/fractal_tasks_core/cellvoyager/wells.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.1/fractal_tasks_core/channels.py` & `fractal_tasks_core-1.0.2/fractal_tasks_core/channels.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.1/fractal_tasks_core/dev/check_manifest.py` & `fractal_tasks_core-1.0.2/fractal_tasks_core/dev/check_manifest.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.1/fractal_tasks_core/dev/create_manifest.py` & `fractal_tasks_core-1.0.2/fractal_tasks_core/dev/create_manifest.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.1/fractal_tasks_core/dev/lib_args_schemas.py` & `fractal_tasks_core-1.0.2/fractal_tasks_core/dev/lib_args_schemas.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.1/fractal_tasks_core/dev/lib_descriptions.py` & `fractal_tasks_core-1.0.2/fractal_tasks_core/dev/lib_descriptions.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.1/fractal_tasks_core/dev/lib_signature_constraints.py` & `fractal_tasks_core-1.0.2/fractal_tasks_core/dev/lib_signature_constraints.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.1/fractal_tasks_core/dev/lib_task_docs.py` & `fractal_tasks_core-1.0.2/fractal_tasks_core/dev/lib_task_docs.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.1/fractal_tasks_core/dev/lib_titles.py` & `fractal_tasks_core-1.0.2/fractal_tasks_core/dev/lib_titles.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.1/fractal_tasks_core/dev/task_list.py` & `fractal_tasks_core-1.0.2/fractal_tasks_core/dev/task_list.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.1/fractal_tasks_core/dev/task_models.py` & `fractal_tasks_core-1.0.2/fractal_tasks_core/dev/task_models.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.1/fractal_tasks_core/labels.py` & `fractal_tasks_core-1.0.2/fractal_tasks_core/labels.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.1/fractal_tasks_core/masked_loading.py` & `fractal_tasks_core-1.0.2/fractal_tasks_core/masked_loading.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.1/fractal_tasks_core/ngff/specs.py` & `fractal_tasks_core-1.0.2/fractal_tasks_core/ngff/specs.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.1/fractal_tasks_core/ngff/zarr_utils.py` & `fractal_tasks_core-1.0.2/fractal_tasks_core/ngff/zarr_utils.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.1/fractal_tasks_core/pyramids.py` & `fractal_tasks_core-1.0.2/fractal_tasks_core/pyramids.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.1/fractal_tasks_core/roi/_overlaps_common.py` & `fractal_tasks_core-1.0.2/fractal_tasks_core/roi/_overlaps_common.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.1/fractal_tasks_core/roi/load_region.py` & `fractal_tasks_core-1.0.2/fractal_tasks_core/roi/load_region.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.1/fractal_tasks_core/roi/v1.py` & `fractal_tasks_core-1.0.2/fractal_tasks_core/roi/v1.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.1/fractal_tasks_core/roi/v1_checks.py` & `fractal_tasks_core-1.0.2/fractal_tasks_core/roi/v1_checks.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.1/fractal_tasks_core/roi/v1_overlaps.py` & `fractal_tasks_core-1.0.2/fractal_tasks_core/roi/v1_overlaps.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.1/fractal_tasks_core/tables/__init__.py` & `fractal_tasks_core-1.0.2/fractal_tasks_core/tables/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.1/fractal_tasks_core/tables/v1.py` & `fractal_tasks_core-1.0.2/fractal_tasks_core/tables/v1.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/_registration_utils.py` & `fractal_tasks_core-1.0.2/fractal_tasks_core/tasks/_registration_utils.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/_utils.py` & `fractal_tasks_core-1.0.2/fractal_tasks_core/tasks/_utils.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/_zarr_utils.py` & `fractal_tasks_core-1.0.2/fractal_tasks_core/tasks/_zarr_utils.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/apply_registration_to_image.py` & `fractal_tasks_core-1.0.2/fractal_tasks_core/tasks/apply_registration_to_image.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/calculate_registration_image_based.py` & `fractal_tasks_core-1.0.2/fractal_tasks_core/tasks/calculate_registration_image_based.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/cellpose_segmentation.py` & `fractal_tasks_core-1.0.2/fractal_tasks_core/tasks/cellpose_segmentation.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/cellpose_transforms.py` & `fractal_tasks_core-1.0.2/fractal_tasks_core/tasks/cellpose_transforms.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/cellvoyager_to_ome_zarr_compute.py` & `fractal_tasks_core-1.0.2/fractal_tasks_core/tasks/cellvoyager_to_ome_zarr_compute.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/cellvoyager_to_ome_zarr_init.py` & `fractal_tasks_core-1.0.2/fractal_tasks_core/tasks/cellvoyager_to_ome_zarr_init.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/cellvoyager_to_ome_zarr_init_multiplex.py` & `fractal_tasks_core-1.0.2/fractal_tasks_core/tasks/cellvoyager_to_ome_zarr_init_multiplex.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/copy_ome_zarr_hcs_plate.py` & `fractal_tasks_core-1.0.2/fractal_tasks_core/tasks/copy_ome_zarr_hcs_plate.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,15 +159,15 @@
         ]
         new_well_image_attrs[old_plate_url][
             well_sub_url
         ] += curr_well_image_list
 
     # Fill in the plate metadata based on all available wells
     for old_plate_url in plate_metadata_dicts:
-        well_list, column_list, row_list = _generate_wells_rows_columns(
+        well_list, row_list, column_list = _generate_wells_rows_columns(
             plate_wells[old_plate_url]
         )
         plate_metadata_dicts[old_plate_url]["plate"]["columns"] = []
         for column in column_list:
             plate_metadata_dicts[old_plate_url]["plate"]["columns"].append(
                 {"name": column}
             )
```

### Comparing `fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/find_registration_consensus.py` & `fractal_tasks_core-1.0.2/fractal_tasks_core/tasks/find_registration_consensus.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/illumination_correction.py` & `fractal_tasks_core-1.0.2/fractal_tasks_core/tasks/illumination_correction.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/image_based_registration_hcs_init.py` & `fractal_tasks_core-1.0.2/fractal_tasks_core/tasks/image_based_registration_hcs_init.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/import_ome_zarr.py` & `fractal_tasks_core-1.0.2/fractal_tasks_core/tasks/import_ome_zarr.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/init_group_by_well_for_multiplexing.py` & `fractal_tasks_core-1.0.2/fractal_tasks_core/tasks/init_group_by_well_for_multiplexing.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/io_models.py` & `fractal_tasks_core-1.0.2/fractal_tasks_core/tasks/io_models.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/maximum_intensity_projection.py` & `fractal_tasks_core-1.0.2/fractal_tasks_core/tasks/maximum_intensity_projection.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.1/fractal_tasks_core/tasks/napari_workflows_wrapper.py` & `fractal_tasks_core-1.0.2/fractal_tasks_core/tasks/napari_workflows_wrapper.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.1/fractal_tasks_core/upscale_array.py` & `fractal_tasks_core-1.0.2/fractal_tasks_core/upscale_array.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.1/fractal_tasks_core/utils.py` & `fractal_tasks_core-1.0.2/fractal_tasks_core/utils.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.1/fractal_tasks_core/zarr_utils.py` & `fractal_tasks_core-1.0.2/fractal_tasks_core/zarr_utils.py`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-1.0.1/pyproject.toml` & `fractal_tasks_core-1.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fractal-tasks-core"
-version = "1.0.1"
+version = "1.0.2"
 description = "Core bioimage-analysis library and tasks of the Fractal analytics platform"
 authors = [
     "Joel Lüthi  <joel.luethi@fmi.ch>",
     "Tommaso Comparin <tommaso.comparin@exact-lab.it>",
     "Marco Franzon <marco.franzon@exact-lab.it>",
     "Jacopo Nespolo <jacopo.nespolo@exact-lab.it>",
 ]
@@ -86,15 +86,15 @@
 branch = true
 parallel = true
 relative_files = true
 source = ["fractal_tasks_core"]
 omit = ["tests/*", "examples/*", "fractal_tasks_core/dev/*"]
 
 [tool.bumpver]
-current_version = "1.0.1"
+current_version = "1.0.2"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `fractal_tasks_core-1.0.1/PKG-INFO` & `fractal_tasks_core-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fractal-tasks-core
-Version: 1.0.1
+Version: 1.0.2
 Summary: Core bioimage-analysis library and tasks of the Fractal analytics platform
 Home-page: https://github.com/fractal-analytics-platform/fractal-tasks-core
 License: BSD-3-Clause
 Author: Joel Lüthi 
 Author-email: joel.luethi@fmi.ch
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
```

