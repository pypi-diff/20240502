# Comparing `tmp/deeplake-3.9.2.tar.gz` & `tmp/deeplake-3.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deeplake-3.9.2.tar", last modified: Mon Apr 29 17:57:39 2024, max compression
+gzip compressed data, was "deeplake-3.9.3.tar", last modified: Thu May  2 21:43:24 2024, max compression
```

## Comparing `deeplake-3.9.2.tar` & `deeplake-3.9.3.tar`

### file list

```diff
@@ -1,423 +1,423 @@
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:57:39.958538 deeplake-3.9.2/
--rw-r--r--   0 nvoxland   (501) wheel        (0)    15975 2024-04-29 17:54:31.000000 deeplake-3.9.2/LICENSE
--rw-r--r--   0 nvoxland   (501) wheel        (0)       36 2024-04-29 17:54:31.000000 deeplake-3.9.2/MANIFEST.in
--rw-r--r--   0 nvoxland   (501) wheel        (0)    21937 2024-04-29 17:57:39.958678 deeplake-3.9.2/PKG-INFO
--rw-r--r--   0 nvoxland   (501) wheel        (0)    21247 2024-04-29 17:54:31.000000 deeplake-3.9.2/README.md
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:57:39.855837 deeplake-3.9.2/deeplake/
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2812 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/__init__.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:57:39.859866 deeplake-3.9.2/deeplake/api/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/api/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)   109063 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/api/dataset.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4693 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/api/info.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1203 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/api/link.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1698 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/api/link_tiled.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2908 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/api/read.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:57:39.871270 deeplake-3.9.2/deeplake/api/tests/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/api/tests/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4250 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/api/tests/test_access_method.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1867 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/api/tests/test_agreement.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    97680 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/api/tests/test_api.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7076 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/api/tests/test_api_tiling.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    11734 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/api/tests/test_api_with_compression.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2654 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/api/tests/test_chunk_sizes.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2562 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/api/tests/test_connect_datasets.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2959 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/api/tests/test_dataset.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1500 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/api/tests/test_dicom.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     6210 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/api/tests/test_downsample.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1040 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/api/tests/test_events.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5056 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/api/tests/test_grayscale.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      298 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/api/tests/test_hosted_datasets.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     6482 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/api/tests/test_info.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     6911 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/api/tests/test_insertion_out_of_order.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7044 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/api/tests/test_json.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    26194 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/api/tests/test_link.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3329 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/api/tests/test_link_tiled.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1789 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/api/tests/test_linking.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1024 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/api/tests/test_mesh.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1204 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/api/tests/test_meta.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4109 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/api/tests/test_nifti.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7900 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/api/tests/test_none.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      970 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/api/tests/test_partial_upload.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2108 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/api/tests/test_pickle.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5680 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/api/tests/test_point_cloud.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4249 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/api/tests/test_polygons.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    12455 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/api/tests/test_pop.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1595 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/api/tests/test_readonly.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    18930 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/api/tests/test_rechunk.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     8958 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/api/tests/test_reset.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4596 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/api/tests/test_sample_info.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      526 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/api/tests/test_tag.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3149 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/api/tests/test_text.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    26508 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/api/tests/test_update_samples.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     8127 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/api/tests/test_video.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7035 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/api/tests/test_views.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1368 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/api/tiled.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:57:39.871403 deeplake-3.9.2/deeplake/auto/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/auto/__init__.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:57:39.871686 deeplake-3.9.2/deeplake/auto/structured/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/auto/structured/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      635 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/auto/structured/base.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7308 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/auto/structured/dataframe.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:57:39.872465 deeplake-3.9.2/deeplake/auto/tests/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/auto/tests/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7975 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/auto/tests/test_coco_template.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    13527 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/auto/tests/test_ingestion.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5371 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/auto/tests/test_kaggle.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5519 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/auto/tests/test_yolo_template.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:57:39.873810 deeplake-3.9.2/deeplake/auto/unstructured/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/auto/unstructured/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      537 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/auto/unstructured/base.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:57:39.874704 deeplake-3.9.2/deeplake/auto/unstructured/coco/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/auto/unstructured/coco/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7093 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/auto/unstructured/coco/coco.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      669 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/auto/unstructured/coco/constants.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1709 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/auto/unstructured/coco/convert.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5237 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/auto/unstructured/coco/utils.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     6701 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/auto/unstructured/image_classification.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3533 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/auto/unstructured/kaggle.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4514 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/auto/unstructured/util.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:57:39.875775 deeplake-3.9.2/deeplake/auto/unstructured/yolo/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/auto/unstructured/yolo/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      278 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/auto/unstructured/yolo/constants.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7394 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/auto/unstructured/yolo/utils.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    12933 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/auto/unstructured/yolo/yolo.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:57:39.877601 deeplake-3.9.2/deeplake/client/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/client/__init__.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:57:39.878591 deeplake-3.9.2/deeplake/client/auth/
--rw-r--r--   0 nvoxland   (501) wheel        (0)      578 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/client/auth/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      886 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/client/auth/activeloop.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      933 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/client/auth/auth_context.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2407 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/client/auth/azure.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1603 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/client/auth/test_auth_context.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    21451 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/client/client.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1436 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/client/config.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      690 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/client/log.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    10650 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/client/test_client.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    12996 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/client/utils.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3876 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/compression.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    10287 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/constants.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:57:39.889635 deeplake-3.9.2/deeplake/core/
--rw-r--r--   0 nvoxland   (501) wheel        (0)       23 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/__init__.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:57:39.891644 deeplake-3.9.2/deeplake/core/chunk/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/chunk/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    24544 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/chunk/base_chunk.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    26270 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/chunk/chunk_compressed_chunk.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     6748 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/chunk/sample_compressed_chunk.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4944 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/chunk/test_chunk_compressed.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4512 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/chunk/test_sample_compressed.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5464 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/chunk/test_uncompressed.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    10139 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/chunk/uncompressed_chunk.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)   137699 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/chunk_engine.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    39331 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/compression.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:57:39.893450 deeplake-3.9.2/deeplake/core/compute/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/compute/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      911 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/compute/process.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2332 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/compute/provider.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      640 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/compute/ray.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      806 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/compute/serial.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      576 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/compute/thread.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:57:39.896062 deeplake-3.9.2/deeplake/core/dataset/
--rw-r--r--   0 nvoxland   (501) wheel        (0)      903 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/dataset/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)   197018 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/dataset/dataset.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    16167 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/dataset/deeplake_cloud_dataset.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    12670 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/dataset/indra_dataset_view.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     6249 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/dataset/indra_tensor_view.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      760 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/dataset/invalid_view.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4666 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/dataset/view_entry.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      118 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/distance_type.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4348 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/fast_forwarding.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:57:39.896508 deeplake-3.9.2/deeplake/core/index/
--rw-r--r--   0 nvoxland   (501) wheel        (0)      138 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/index/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    17988 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/index/index.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     9539 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/index_maintenance.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    20531 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/io.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4121 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/ipc.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    13074 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/link_creds.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    16646 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/linked_chunk_engine.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2277 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/linked_sample.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2597 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/linked_tiled_sample.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     9946 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/lock.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:57:39.898959 deeplake-3.9.2/deeplake/core/meta/
--rw-r--r--   0 nvoxland   (501) wheel        (0)       97 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/meta/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4043 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/meta/dataset_meta.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:57:39.901801 deeplake-3.9.2/deeplake/core/meta/encode/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/meta/encode/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    25591 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/meta/encode/base_encoder.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3915 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/meta/encode/byte_positions.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    13848 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/meta/encode/chunk_id.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1551 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/meta/encode/creds.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3972 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/meta/encode/pad.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      941 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/meta/encode/sequence.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      683 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/meta/encode/shape.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:57:39.903022 deeplake-3.9.2/deeplake/core/meta/encode/tests/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/meta/encode/tests/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      226 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/meta/encode/tests/common.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2237 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1452 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2114 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3673 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/meta/encode/tests/test_shape_encoder.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2810 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7627 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/meta/encode/tile.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      503 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/meta/meta.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    14862 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/meta/tensor_meta.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      906 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/partial_reader.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      971 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/partial_sample.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5269 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/polygon.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:57:39.904592 deeplake-3.9.2/deeplake/core/query/
--rw-r--r--   0 nvoxland   (501) wheel        (0)       82 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/query/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    12021 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/query/autocomplete.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    15253 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/query/filter.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     8905 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/query/query.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    21165 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/sample.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2506 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/seed.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    23415 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/serialize.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:57:39.908141 deeplake-3.9.2/deeplake/core/storage/
--rw-r--r--   0 nvoxland   (501) wheel        (0)      495 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/storage/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    15471 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/storage/azure.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1053 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/storage/deeplake_memory_object.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    19256 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/storage/gcs.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    13455 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/storage/google_drive.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3114 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/storage/indra.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     9604 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/storage/local.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    20308 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/storage/lru_cache.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3705 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/storage/memory.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7292 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/storage/provider.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    29048 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/storage/s3.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    65084 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/tensor.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7571 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/tensor_link.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5185 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/test_serialize.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:57:39.912615 deeplake-3.9.2/deeplake/core/tests/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/tests/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7674 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/tests/test_compression.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      729 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/tests/test_compute.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2181 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/tests/test_dataset.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    16372 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/tests/test_indra_dataset.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      913 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/tests/test_io.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4811 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/tests/test_locking.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1833 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/tests/test_query.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      676 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/tests/test_readonly.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      377 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/tests/test_seed.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1944 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/tests/test_serialize.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    10543 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/tests/test_vdb_indexes.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:57:39.913857 deeplake-3.9.2/deeplake/core/tiling/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/tiling/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4790 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/tiling/deserialize.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1701 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/tiling/optimizer.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4827 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/tiling/sample_tiles.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2893 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/tiling/serialize.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1968 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/tiling/test_optimizer.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2367 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/tiling/test_serialize.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:57:39.915981 deeplake-3.9.2/deeplake/core/transform/
--rw-r--r--   0 nvoxland   (501) wheel        (0)      111 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/transform/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    56175 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/transform/test_transform.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    30619 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/transform/transform.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    11143 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/transform/transform_dataset.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     6049 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/transform/transform_tensor.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:57:39.916466 deeplake-3.9.2/deeplake/core/vectorstore/
--rw-r--r--   0 nvoxland   (501) wheel        (0)      638 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/vectorstore/__init__.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:57:39.918025 deeplake-3.9.2/deeplake/core/vectorstore/dataset_handlers/
--rw-r--r--   0 nvoxland   (501) wheel        (0)      100 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/vectorstore/dataset_handlers/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    13355 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/vectorstore/dataset_handlers/client_side_dataset_handler.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      450 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/vectorstore/dataset_handlers/dataset_handler.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     6152 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/vectorstore/dataset_handlers/dataset_handler_base.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:57:39.918532 deeplake-3.9.2/deeplake/core/vectorstore/deep_memory/
--rw-r--r--   0 nvoxland   (501) wheel        (0)       73 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/vectorstore/deep_memory/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    26733 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/vectorstore/deep_memory/deep_memory.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    24999 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/vectorstore/deep_memory/test_deepmemory.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    32155 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/vectorstore/deeplake_vectorstore.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:57:39.919020 deeplake-3.9.2/deeplake/core/vectorstore/embeddings/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/vectorstore/embeddings/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3777 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/vectorstore/embeddings/embedder.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3131 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/vectorstore/embeddings/test_embedder.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    90371 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/vectorstore/test_deeplake_vectorstore.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:57:39.919601 deeplake-3.9.2/deeplake/core/vectorstore/vector_search/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/vectorstore/vector_search/__init__.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:57:39.920152 deeplake-3.9.2/deeplake/core/vectorstore/vector_search/dataset/
--rw-r--r--   0 nvoxland   (501) wheel        (0)      392 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/vectorstore/vector_search/dataset/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    18849 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/vectorstore/vector_search/dataset/dataset.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    14233 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/vectorstore/vector_search/dataset/test_dataset.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:57:39.920779 deeplake-3.9.2/deeplake/core/vectorstore/vector_search/filter/
--rw-r--r--   0 nvoxland   (501) wheel        (0)      286 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/vectorstore/vector_search/filter/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4396 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/vectorstore/vector_search/filter/filter.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4223 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/vectorstore/vector_search/filter/test_filter.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:57:39.921681 deeplake-3.9.2/deeplake/core/vectorstore/vector_search/indra/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/vectorstore/vector_search/indra/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5190 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/vectorstore/vector_search/indra/query.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7363 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/vectorstore/vector_search/indra/search_algorithm.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3657 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/vectorstore/vector_search/indra/test_indra.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:57:39.922861 deeplake-3.9.2/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/
--rw-r--r--   0 nvoxland   (501) wheel        (0)      275 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      956 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/distance_metric.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      221 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/order.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1406 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/vectorstore/vector_search/indra/vector_search.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:57:39.923636 deeplake-3.9.2/deeplake/core/vectorstore/vector_search/ingestion/
--rw-r--r--   0 nvoxland   (501) wheel        (0)       93 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/vectorstore/vector_search/ingestion/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5839 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/vectorstore/vector_search/ingestion/data_ingestion.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2047 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/vectorstore/vector_search/ingestion/ingest_data.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5205 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/vectorstore/vector_search/ingestion/test_data_ingestion.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:57:39.924830 deeplake-3.9.2/deeplake/core/vectorstore/vector_search/python/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/vectorstore/vector_search/python/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1924 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/vectorstore/vector_search/python/search_algorithm.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2371 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/vectorstore/vector_search/python/test_vector_search.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1734 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/vectorstore/vector_search/python/vector_search.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    21909 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/vectorstore/vector_search/utils.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3912 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/vectorstore/vector_search/vector_search.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:57:39.926048 deeplake-3.9.2/deeplake/core/version_control/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/version_control/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1954 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/version_control/commit_chunk_map.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     6337 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/version_control/commit_diff.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3127 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/version_control/commit_node.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5006 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/version_control/dataset_diff.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    19869 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/version_control/test_merge.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    91907 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/core/version_control/test_version_control.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:57:39.929168 deeplake-3.9.2/deeplake/enterprise/
--rw-r--r--   0 nvoxland   (501) wheel        (0)      145 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/enterprise/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     8422 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/enterprise/convert_to_libdeeplake.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    37913 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/enterprise/dataloader.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5967 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/enterprise/dummy_dataloader.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     6276 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/enterprise/libdeeplake_query.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    28963 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/enterprise/test_pytorch.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3432 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/enterprise/test_query.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    22675 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/enterprise/test_tensorflow.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1819 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/enterprise/util.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1590 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/hooks.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     8558 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/htype.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:57:39.929344 deeplake-3.9.2/deeplake/integrations/
--rw-r--r--   0 nvoxland   (501) wheel        (0)       99 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/integrations/__init__.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:57:39.930080 deeplake-3.9.2/deeplake/integrations/huggingface/
--rw-r--r--   0 nvoxland   (501) wheel        (0)       44 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/integrations/huggingface/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5503 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/integrations/huggingface/huggingface.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:57:39.930888 deeplake-3.9.2/deeplake/integrations/mmdet/
--rw-r--r--   0 nvoxland   (501) wheel        (0)      118 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/integrations/mmdet/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    62719 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/integrations/mmdet/mmdet_.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4740 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/integrations/mmdet/mmdet_runners.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    19652 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/integrations/mmdet/mmdet_utils.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:57:39.931896 deeplake-3.9.2/deeplake/integrations/pytorch/
--rw-r--r--   0 nvoxland   (501) wheel        (0)       40 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/integrations/pytorch/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    10179 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/integrations/pytorch/common.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7317 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/integrations/pytorch/dataset.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4367 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/integrations/pytorch/pytorch.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7282 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/integrations/pytorch/shuffle_buffer.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:57:39.932977 deeplake-3.9.2/deeplake/integrations/tf/
--rw-r--r--   0 nvoxland   (501) wheel        (0)      136 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/integrations/tf/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1270 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/integrations/tf/common.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2454 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/integrations/tf/datasettotensorflow.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5331 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/integrations/tf/deeplake_tensorflow_dataset.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:57:39.933333 deeplake-3.9.2/deeplake/integrations/wandb/
--rw-r--r--   0 nvoxland   (501) wheel        (0)       21 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/integrations/wandb/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    12089 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/integrations/wandb/wandb.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:57:39.934404 deeplake-3.9.2/deeplake/requirements/
--rw-r--r--   0 nvoxland   (501) wheel        (0)      487 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/requirements/common.txt
--rw-r--r--   0 nvoxland   (501) wheel        (0)       71 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/requirements/docs.txt
--rw-r--r--   0 nvoxland   (501) wheel        (0)      381 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/requirements/plugins.txt
--rw-r--r--   0 nvoxland   (501) wheel        (0)      416 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/requirements/tests.txt
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:57:39.936331 deeplake-3.9.2/deeplake/tests/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/tests/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1404 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/tests/cache_fixtures.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2721 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/tests/client_fixtures.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4218 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/tests/common.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4386 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/tests/dataset_fixtures.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    25709 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/tests/path_fixtures.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2811 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/tests/storage_fixtures.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:57:39.950158 deeplake-3.9.2/deeplake/util/
--rw-r--r--   0 nvoxland   (501) wheel        (0)       86 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7370 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/access_method.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1130 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/agreement.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1567 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/array_list.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      619 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/assert_byte_indexes.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2961 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/auto.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5919 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/bugout_reporter.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)       54 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/bugout_token.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3623 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/cache_chain.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4612 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/casting.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      310 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/check_installation.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1213 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/check_latest_version.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3151 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/chunk_engine.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4597 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/class_label.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      231 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/compression.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1197 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/compute.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5706 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/connect_dataset.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1170 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/dataset.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      443 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/delete_entry.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    15906 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/diff.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     5181 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/downsample.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)       84 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/empty_sample.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    15642 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/encoder.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    37198 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/exceptions.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2026 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/exif.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1803 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/from_tfds.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      136 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/generate_id.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      306 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/hash.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2901 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/htype.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1517 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/image.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      873 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/invalid_view_op.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      135 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/iterable_ordered_dict.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1001 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/iteration_warning.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      507 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/join_chunks.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     6422 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/json.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7804 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/keys.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3071 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/link.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1646 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/logging.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    37936 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/merge.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2426 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/modified.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      903 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/notebook.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:57:39.953737 deeplake-3.9.2/deeplake/util/object_3d/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        1 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/object_3d/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3374 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/object_3d/mesh.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      185 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/object_3d/mesh_parser.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      185 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/object_3d/mesh_reader.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1021 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/object_3d/object_base_3d.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      695 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/object_3d/ply_parser.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1323 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/object_3d/ply_parser_base.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     6188 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/object_3d/ply_parsers.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1663 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/object_3d/ply_reader.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3221 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/object_3d/ply_reader_base.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    10435 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/object_3d/ply_readers.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     7113 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/object_3d/point_cloud.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1087 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/object_3d/read_3d_data.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4600 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/path.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3220 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/pretty_print.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2844 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/remove_cache.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4511 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/scheduling.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3140 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/shape_interval.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      351 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/shuffle.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     4784 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/spinner.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1153 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/split.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    10033 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/storage.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1131 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/tag.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1425 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/tensor_db.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      951 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/testing.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:57:39.957685 deeplake-3.9.2/deeplake/util/tests/
--rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/tests/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1476 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/tests/test_auto.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1795 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/tests/test_connect_dataset.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1239 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/tests/test_iterable_ordered_dict.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      628 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/tests/test_keys.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      892 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/tests/test_read.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1071 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/tests/test_shape_interval.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      429 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/tests/test_shuffle.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      698 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/tests/test_split.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      974 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/tests/test_tensor_db.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      299 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/tests/test_token.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     2452 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/tests/test_version_control.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      559 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/tests/test_video.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      276 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/threading.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      381 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/token.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    27435 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/transform.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)    41390 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/version_control.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1284 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/video.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)      167 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/util/warnings.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:57:39.958334 deeplake-3.9.2/deeplake/visualizer/
--rw-r--r--   0 nvoxland   (501) wheel        (0)       34 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/visualizer/__init__.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     6466 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/visualizer/video_streaming.py
--rw-r--r--   0 nvoxland   (501) wheel        (0)     6764 2024-04-29 17:54:31.000000 deeplake-3.9.2/deeplake/visualizer/visualizer.py
-drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-04-29 17:57:39.857136 deeplake-3.9.2/deeplake.egg-info/
--rw-r--r--   0 nvoxland   (501) wheel        (0)    21937 2024-04-29 17:57:39.000000 deeplake-3.9.2/deeplake.egg-info/PKG-INFO
--rw-r--r--   0 nvoxland   (501) wheel        (0)    13651 2024-04-29 17:57:39.000000 deeplake-3.9.2/deeplake.egg-info/SOURCES.txt
--rw-r--r--   0 nvoxland   (501) wheel        (0)        1 2024-04-29 17:57:39.000000 deeplake-3.9.2/deeplake.egg-info/dependency_links.txt
--rw-r--r--   0 nvoxland   (501) wheel        (0)        1 2024-04-29 17:57:39.000000 deeplake-3.9.2/deeplake.egg-info/not-zip-safe
--rw-r--r--   0 nvoxland   (501) wheel        (0)     1109 2024-04-29 17:57:39.000000 deeplake-3.9.2/deeplake.egg-info/requires.txt
--rw-r--r--   0 nvoxland   (501) wheel        (0)        9 2024-04-29 17:57:39.000000 deeplake-3.9.2/deeplake.egg-info/top_level.txt
--rw-r--r--   0 nvoxland   (501) wheel        (0)       63 2024-04-29 17:54:31.000000 deeplake-3.9.2/pyproject.toml
--rw-r--r--   0 nvoxland   (501) wheel        (0)      311 2024-04-29 17:57:39.959139 deeplake-3.9.2/setup.cfg
--rw-r--r--   0 nvoxland   (501) wheel        (0)     3339 2024-04-29 17:54:31.000000 deeplake-3.9.2/setup.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:43:24.456086 deeplake-3.9.3/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    15975 2024-05-02 21:40:11.000000 deeplake-3.9.3/LICENSE
+-rw-r--r--   0 nvoxland   (501) wheel        (0)       36 2024-05-02 21:40:11.000000 deeplake-3.9.3/MANIFEST.in
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    21937 2024-05-02 21:43:24.456366 deeplake-3.9.3/PKG-INFO
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    21247 2024-05-02 21:40:11.000000 deeplake-3.9.3/README.md
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:43:24.364375 deeplake-3.9.3/deeplake/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2812 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/__init__.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:43:24.368237 deeplake-3.9.3/deeplake/api/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/api/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)   109063 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/api/dataset.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4693 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/api/info.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1203 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/api/link.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1698 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/api/link_tiled.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2908 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/api/read.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:43:24.377903 deeplake-3.9.3/deeplake/api/tests/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/api/tests/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4250 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/api/tests/test_access_method.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1867 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/api/tests/test_agreement.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    97680 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/api/tests/test_api.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7076 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/api/tests/test_api_tiling.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    11734 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/api/tests/test_api_with_compression.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2654 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/api/tests/test_chunk_sizes.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2562 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/api/tests/test_connect_datasets.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2959 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/api/tests/test_dataset.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1500 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/api/tests/test_dicom.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     6210 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/api/tests/test_downsample.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1040 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/api/tests/test_events.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5056 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/api/tests/test_grayscale.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      298 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/api/tests/test_hosted_datasets.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     6482 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/api/tests/test_info.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     6911 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/api/tests/test_insertion_out_of_order.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7044 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/api/tests/test_json.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    26194 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/api/tests/test_link.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3329 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/api/tests/test_link_tiled.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1789 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/api/tests/test_linking.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1024 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/api/tests/test_mesh.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1204 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/api/tests/test_meta.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4109 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/api/tests/test_nifti.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7900 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/api/tests/test_none.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      970 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/api/tests/test_partial_upload.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2108 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/api/tests/test_pickle.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5680 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/api/tests/test_point_cloud.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4249 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/api/tests/test_polygons.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    12455 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/api/tests/test_pop.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1595 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/api/tests/test_readonly.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    18930 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/api/tests/test_rechunk.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     8958 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/api/tests/test_reset.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4596 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/api/tests/test_sample_info.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      526 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/api/tests/test_tag.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3149 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/api/tests/test_text.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    26508 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/api/tests/test_update_samples.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     8127 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/api/tests/test_video.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7035 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/api/tests/test_views.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1368 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/api/tiled.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:43:24.378214 deeplake-3.9.3/deeplake/auto/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/auto/__init__.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:43:24.378517 deeplake-3.9.3/deeplake/auto/structured/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/auto/structured/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      635 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/auto/structured/base.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7308 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/auto/structured/dataframe.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:43:24.379873 deeplake-3.9.3/deeplake/auto/tests/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/auto/tests/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7975 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/auto/tests/test_coco_template.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    13527 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/auto/tests/test_ingestion.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5371 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/auto/tests/test_kaggle.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5519 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/auto/tests/test_yolo_template.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:43:24.380978 deeplake-3.9.3/deeplake/auto/unstructured/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/auto/unstructured/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      537 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/auto/unstructured/base.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:43:24.382292 deeplake-3.9.3/deeplake/auto/unstructured/coco/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/auto/unstructured/coco/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7093 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/auto/unstructured/coco/coco.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      669 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/auto/unstructured/coco/constants.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1709 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/auto/unstructured/coco/convert.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5237 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/auto/unstructured/coco/utils.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     6701 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/auto/unstructured/image_classification.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3533 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/auto/unstructured/kaggle.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4514 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/auto/unstructured/util.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:43:24.383071 deeplake-3.9.3/deeplake/auto/unstructured/yolo/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/auto/unstructured/yolo/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      278 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/auto/unstructured/yolo/constants.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7394 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/auto/unstructured/yolo/utils.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    12933 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/auto/unstructured/yolo/yolo.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:43:24.384683 deeplake-3.9.3/deeplake/client/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/client/__init__.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:43:24.385857 deeplake-3.9.3/deeplake/client/auth/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      578 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/client/auth/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      886 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/client/auth/activeloop.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      933 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/client/auth/auth_context.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2407 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/client/auth/azure.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1603 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/client/auth/test_auth_context.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    21451 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/client/client.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1436 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/client/config.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      690 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/client/log.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    10650 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/client/test_client.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    12996 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/client/utils.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3876 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/compression.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    10287 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/constants.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:43:24.393874 deeplake-3.9.3/deeplake/core/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)       23 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/__init__.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:43:24.396423 deeplake-3.9.3/deeplake/core/chunk/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/chunk/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    24544 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/chunk/base_chunk.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    26270 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/chunk/chunk_compressed_chunk.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     6748 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/chunk/sample_compressed_chunk.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4944 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/chunk/test_chunk_compressed.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4512 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/chunk/test_sample_compressed.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5464 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/chunk/test_uncompressed.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    10139 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/chunk/uncompressed_chunk.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)   137699 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/chunk_engine.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    39331 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/compression.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:43:24.398097 deeplake-3.9.3/deeplake/core/compute/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/compute/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      911 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/compute/process.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2332 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/compute/provider.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      640 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/compute/ray.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      806 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/compute/serial.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      576 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/compute/thread.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:43:24.400532 deeplake-3.9.3/deeplake/core/dataset/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      903 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/dataset/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)   197018 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/dataset/dataset.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    16167 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/dataset/deeplake_cloud_dataset.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    12670 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/dataset/indra_dataset_view.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     6249 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/dataset/indra_tensor_view.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      760 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/dataset/invalid_view.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4666 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/dataset/view_entry.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      118 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/distance_type.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4348 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/fast_forwarding.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:43:24.400864 deeplake-3.9.3/deeplake/core/index/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      138 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/index/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    17988 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/index/index.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     9539 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/index_maintenance.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    20531 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/io.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4121 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/ipc.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    13074 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/link_creds.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    16646 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/linked_chunk_engine.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2277 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/linked_sample.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2597 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/linked_tiled_sample.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     9946 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/lock.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:43:24.401968 deeplake-3.9.3/deeplake/core/meta/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)       97 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/meta/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4043 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/meta/dataset_meta.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:43:24.404232 deeplake-3.9.3/deeplake/core/meta/encode/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/meta/encode/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    25591 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/meta/encode/base_encoder.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3915 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/meta/encode/byte_positions.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    13848 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/meta/encode/chunk_id.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1551 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/meta/encode/creds.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3972 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/meta/encode/pad.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      941 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/meta/encode/sequence.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      683 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/meta/encode/shape.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:43:24.405513 deeplake-3.9.3/deeplake/core/meta/encode/tests/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/meta/encode/tests/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      226 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/meta/encode/tests/common.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2237 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1452 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2114 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3673 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/meta/encode/tests/test_shape_encoder.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2810 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7627 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/meta/encode/tile.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      503 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/meta/meta.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    14862 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/meta/tensor_meta.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      906 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/partial_reader.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      971 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/partial_sample.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5269 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/polygon.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:43:24.406528 deeplake-3.9.3/deeplake/core/query/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)       82 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/query/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    12021 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/query/autocomplete.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    15253 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/query/filter.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     8905 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/query/query.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    21165 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/sample.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2506 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/seed.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    23415 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/serialize.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:43:24.409387 deeplake-3.9.3/deeplake/core/storage/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      495 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/storage/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    15471 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/storage/azure.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1053 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/storage/deeplake_memory_object.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    19256 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/storage/gcs.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    13455 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/storage/google_drive.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3114 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/storage/indra.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     9604 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/storage/local.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    20308 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/storage/lru_cache.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3705 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/storage/memory.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7292 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/storage/provider.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    29048 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/storage/s3.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    65084 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/tensor.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7571 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/tensor_link.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5185 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/test_serialize.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:43:24.412164 deeplake-3.9.3/deeplake/core/tests/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/tests/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7674 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/tests/test_compression.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      729 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/tests/test_compute.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2181 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/tests/test_dataset.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    16372 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/tests/test_indra_dataset.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      913 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/tests/test_io.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4811 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/tests/test_locking.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1833 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/tests/test_query.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      676 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/tests/test_readonly.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      377 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/tests/test_seed.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1944 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/tests/test_serialize.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    10543 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/tests/test_vdb_indexes.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:43:24.413745 deeplake-3.9.3/deeplake/core/tiling/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/tiling/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4790 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/tiling/deserialize.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1701 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/tiling/optimizer.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4827 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/tiling/sample_tiles.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2893 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/tiling/serialize.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1968 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/tiling/test_optimizer.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2367 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/tiling/test_serialize.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:43:24.415440 deeplake-3.9.3/deeplake/core/transform/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      111 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/transform/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    56175 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/transform/test_transform.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    30619 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/transform/transform.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    11143 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/transform/transform_dataset.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     6049 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/transform/transform_tensor.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:43:24.416102 deeplake-3.9.3/deeplake/core/vectorstore/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      638 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/vectorstore/__init__.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:43:24.417800 deeplake-3.9.3/deeplake/core/vectorstore/dataset_handlers/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      100 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/vectorstore/dataset_handlers/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    13355 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/vectorstore/dataset_handlers/client_side_dataset_handler.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      450 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/vectorstore/dataset_handlers/dataset_handler.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     6152 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/vectorstore/dataset_handlers/dataset_handler_base.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:43:24.418730 deeplake-3.9.3/deeplake/core/vectorstore/deep_memory/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)       73 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/vectorstore/deep_memory/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    26733 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/vectorstore/deep_memory/deep_memory.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    24999 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/vectorstore/deep_memory/test_deepmemory.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    32155 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/vectorstore/deeplake_vectorstore.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:43:24.419360 deeplake-3.9.3/deeplake/core/vectorstore/embeddings/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/vectorstore/embeddings/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3777 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/vectorstore/embeddings/embedder.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3131 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/vectorstore/embeddings/test_embedder.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    90371 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/vectorstore/test_deeplake_vectorstore.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:43:24.420017 deeplake-3.9.3/deeplake/core/vectorstore/vector_search/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/vectorstore/vector_search/__init__.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:43:24.420657 deeplake-3.9.3/deeplake/core/vectorstore/vector_search/dataset/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      392 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/vectorstore/vector_search/dataset/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    18849 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/vectorstore/vector_search/dataset/dataset.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    14233 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/vectorstore/vector_search/dataset/test_dataset.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:43:24.421469 deeplake-3.9.3/deeplake/core/vectorstore/vector_search/filter/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      286 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/vectorstore/vector_search/filter/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4396 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/vectorstore/vector_search/filter/filter.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4223 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/vectorstore/vector_search/filter/test_filter.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:43:24.422521 deeplake-3.9.3/deeplake/core/vectorstore/vector_search/indra/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/vectorstore/vector_search/indra/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5190 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/vectorstore/vector_search/indra/query.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7363 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/vectorstore/vector_search/indra/search_algorithm.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3657 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/vectorstore/vector_search/indra/test_indra.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:43:24.422992 deeplake-3.9.3/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      275 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      956 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/distance_metric.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      221 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/order.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1406 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/vectorstore/vector_search/indra/vector_search.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:43:24.423663 deeplake-3.9.3/deeplake/core/vectorstore/vector_search/ingestion/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)       93 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/vectorstore/vector_search/ingestion/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5839 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/vectorstore/vector_search/ingestion/data_ingestion.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2047 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/vectorstore/vector_search/ingestion/ingest_data.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5205 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/vectorstore/vector_search/ingestion/test_data_ingestion.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:43:24.424352 deeplake-3.9.3/deeplake/core/vectorstore/vector_search/python/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/vectorstore/vector_search/python/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1924 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/vectorstore/vector_search/python/search_algorithm.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2371 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/vectorstore/vector_search/python/test_vector_search.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1734 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/vectorstore/vector_search/python/vector_search.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    21909 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/vectorstore/vector_search/utils.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3912 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/vectorstore/vector_search/vector_search.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:43:24.425718 deeplake-3.9.3/deeplake/core/version_control/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/version_control/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1954 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/version_control/commit_chunk_map.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     6337 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/version_control/commit_diff.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3127 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/version_control/commit_node.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5006 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/version_control/dataset_diff.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    19869 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/version_control/test_merge.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    91907 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/core/version_control/test_version_control.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:43:24.428939 deeplake-3.9.3/deeplake/enterprise/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      145 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/enterprise/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     8422 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/enterprise/convert_to_libdeeplake.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    37913 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/enterprise/dataloader.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5967 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/enterprise/dummy_dataloader.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     6276 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/enterprise/libdeeplake_query.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    28963 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/enterprise/test_pytorch.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3432 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/enterprise/test_query.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    22675 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/enterprise/test_tensorflow.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1819 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/enterprise/util.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1590 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/hooks.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     8558 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/htype.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:43:24.429139 deeplake-3.9.3/deeplake/integrations/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)       99 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/integrations/__init__.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:43:24.429755 deeplake-3.9.3/deeplake/integrations/huggingface/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)       44 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/integrations/huggingface/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5503 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/integrations/huggingface/huggingface.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:43:24.431128 deeplake-3.9.3/deeplake/integrations/mmdet/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      118 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/integrations/mmdet/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    62719 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/integrations/mmdet/mmdet_.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4740 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/integrations/mmdet/mmdet_runners.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    19652 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/integrations/mmdet/mmdet_utils.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:43:24.432355 deeplake-3.9.3/deeplake/integrations/pytorch/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)       40 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/integrations/pytorch/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    10179 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/integrations/pytorch/common.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7317 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/integrations/pytorch/dataset.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4367 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/integrations/pytorch/pytorch.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7282 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/integrations/pytorch/shuffle_buffer.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:43:24.433009 deeplake-3.9.3/deeplake/integrations/tf/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      136 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/integrations/tf/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1270 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/integrations/tf/common.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2454 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/integrations/tf/datasettotensorflow.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5331 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/integrations/tf/deeplake_tensorflow_dataset.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:43:24.433468 deeplake-3.9.3/deeplake/integrations/wandb/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)       21 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/integrations/wandb/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    12089 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/integrations/wandb/wandb.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:43:24.434089 deeplake-3.9.3/deeplake/requirements/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      487 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/requirements/common.txt
+-rw-r--r--   0 nvoxland   (501) wheel        (0)       71 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/requirements/docs.txt
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      381 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/requirements/plugins.txt
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      416 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/requirements/tests.txt
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:43:24.435356 deeplake-3.9.3/deeplake/tests/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/tests/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1404 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/tests/cache_fixtures.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2721 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/tests/client_fixtures.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4218 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/tests/common.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4386 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/tests/dataset_fixtures.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    25709 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/tests/path_fixtures.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2811 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/tests/storage_fixtures.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:43:24.450704 deeplake-3.9.3/deeplake/util/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)       86 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7370 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/access_method.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1130 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/agreement.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1567 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/array_list.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      619 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/assert_byte_indexes.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2961 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/auto.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5919 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/bugout_reporter.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)       54 2024-05-02 21:40:12.000000 deeplake-3.9.3/deeplake/util/bugout_token.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3623 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/cache_chain.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4612 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/casting.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      310 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/check_installation.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1213 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/check_latest_version.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3151 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/chunk_engine.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4597 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/class_label.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      231 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/compression.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1197 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/compute.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5706 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/connect_dataset.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1170 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/dataset.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      443 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/delete_entry.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    15906 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/diff.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     5181 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/downsample.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)       84 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/empty_sample.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    15642 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/encoder.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    37198 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/exceptions.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2026 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/exif.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1803 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/from_tfds.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      136 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/generate_id.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      306 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/hash.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2901 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/htype.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1517 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/image.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      873 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/invalid_view_op.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      135 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/iterable_ordered_dict.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1001 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/iteration_warning.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      507 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/join_chunks.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     6422 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/json.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7804 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/keys.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3071 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/link.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1646 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/logging.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    37936 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/merge.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2426 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/modified.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      903 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/notebook.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:43:24.453383 deeplake-3.9.3/deeplake/util/object_3d/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        1 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/object_3d/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3374 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/object_3d/mesh.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      185 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/object_3d/mesh_parser.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      185 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/object_3d/mesh_reader.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1021 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/object_3d/object_base_3d.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      695 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/object_3d/ply_parser.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1323 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/object_3d/ply_parser_base.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     6188 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/object_3d/ply_parsers.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1663 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/object_3d/ply_reader.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3221 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/object_3d/ply_reader_base.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    10435 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/object_3d/ply_readers.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     7113 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/object_3d/point_cloud.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1087 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/object_3d/read_3d_data.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4600 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/path.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3220 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/pretty_print.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2844 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/remove_cache.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4511 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/scheduling.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3140 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/shape_interval.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      351 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/shuffle.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     4784 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/spinner.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1153 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/split.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    10033 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/storage.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1131 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/tag.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1425 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/tensor_db.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      951 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/testing.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:43:24.455149 deeplake-3.9.3/deeplake/util/tests/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/tests/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1476 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/tests/test_auto.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1795 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/tests/test_connect_dataset.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1239 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/tests/test_iterable_ordered_dict.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      628 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/tests/test_keys.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      892 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/tests/test_read.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1071 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/tests/test_shape_interval.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      429 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/tests/test_shuffle.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      698 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/tests/test_split.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      974 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/tests/test_tensor_db.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      299 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/tests/test_token.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     2452 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/tests/test_version_control.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      559 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/tests/test_video.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      276 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/threading.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      381 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/token.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    27435 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/transform.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    41390 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/version_control.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1284 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/video.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      167 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/util/warnings.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:43:24.455764 deeplake-3.9.3/deeplake/visualizer/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)       34 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/visualizer/__init__.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     6466 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/visualizer/video_streaming.py
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     6764 2024-05-02 21:40:11.000000 deeplake-3.9.3/deeplake/visualizer/visualizer.py
+drwxr-xr-x   0 nvoxland   (501) wheel        (0)        0 2024-05-02 21:43:24.365765 deeplake-3.9.3/deeplake.egg-info/
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    21937 2024-05-02 21:43:24.000000 deeplake-3.9.3/deeplake.egg-info/PKG-INFO
+-rw-r--r--   0 nvoxland   (501) wheel        (0)    13651 2024-05-02 21:43:24.000000 deeplake-3.9.3/deeplake.egg-info/SOURCES.txt
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        1 2024-05-02 21:43:24.000000 deeplake-3.9.3/deeplake.egg-info/dependency_links.txt
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        1 2024-05-02 21:43:24.000000 deeplake-3.9.3/deeplake.egg-info/not-zip-safe
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     1109 2024-05-02 21:43:24.000000 deeplake-3.9.3/deeplake.egg-info/requires.txt
+-rw-r--r--   0 nvoxland   (501) wheel        (0)        9 2024-05-02 21:43:24.000000 deeplake-3.9.3/deeplake.egg-info/top_level.txt
+-rw-r--r--   0 nvoxland   (501) wheel        (0)       63 2024-05-02 21:40:12.000000 deeplake-3.9.3/pyproject.toml
+-rw-r--r--   0 nvoxland   (501) wheel        (0)      311 2024-05-02 21:43:24.456661 deeplake-3.9.3/setup.cfg
+-rw-r--r--   0 nvoxland   (501) wheel        (0)     3339 2024-05-02 21:40:12.000000 deeplake-3.9.3/setup.py
```

### Comparing `deeplake-3.9.2/LICENSE` & `deeplake-3.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/PKG-INFO` & `deeplake-3.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deeplake
-Version: 3.9.2
+Version: 3.9.3
 Summary: Activeloop Deep Lake
 Author: activeloop.ai
 Author-email: support@activeloop.ai
 License: MPL-2.0
 Project-URL: Documentation, https://docs.activeloop.ai/
 Project-URL: Source, https://github.com/activeloopai/deeplake
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: deeplake Version: 3.9.2 Summary: Activeloop Deep
+Metadata-Version: 2.1 Name: deeplake Version: 3.9.3 Summary: Activeloop Deep
 Lake Author: activeloop.ai Author-email: support@activeloop.ai License: MPL-2.0
 Project-URL: Documentation, https://docs.activeloop.ai/ Project-URL: Source,
 https://github.com/activeloopai/deeplake Classifier: License :: OSI Approved ::
 Mozilla Public License 2.0 (MPL 2.0) Description-Content-Type: text/markdown
 Provides-Extra: audio Provides-Extra: video Provides-Extra: av Provides-Extra:
 gcp Provides-Extra: azure Provides-Extra: dicom Provides-Extra: medical
 Provides-Extra: visualizer Provides-Extra: gdrive Provides-Extra: point_cloud
```

### Comparing `deeplake-3.9.2/README.md` & `deeplake-3.9.3/README.md`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/__init__.py` & `deeplake-3.9.3/deeplake/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
     "copy",
     "query",
     "rename",
     "random",
 ]
 
 
-__version__ = "3.9.2"
+__version__ = "3.9.3"
 warn_if_update_required(__version__)
 __encoded_version__ = np.array(__version__)
 config = {"s3": Config(max_pool_connections=50, connect_timeout=300, read_timeout=300)}
 
 
 deeplake_reporter.tags.append(f"version:{__version__}")
```

### Comparing `deeplake-3.9.2/deeplake/api/dataset.py` & `deeplake-3.9.3/deeplake/api/dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/api/info.py` & `deeplake-3.9.3/deeplake/api/info.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/api/link.py` & `deeplake-3.9.3/deeplake/api/link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/api/link_tiled.py` & `deeplake-3.9.3/deeplake/api/link_tiled.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/api/read.py` & `deeplake-3.9.3/deeplake/api/read.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/api/tests/test_access_method.py` & `deeplake-3.9.3/deeplake/api/tests/test_access_method.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/api/tests/test_agreement.py` & `deeplake-3.9.3/deeplake/api/tests/test_agreement.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/api/tests/test_api.py` & `deeplake-3.9.3/deeplake/api/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/api/tests/test_api_tiling.py` & `deeplake-3.9.3/deeplake/api/tests/test_api_tiling.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/api/tests/test_api_with_compression.py` & `deeplake-3.9.3/deeplake/api/tests/test_api_with_compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/api/tests/test_chunk_sizes.py` & `deeplake-3.9.3/deeplake/api/tests/test_chunk_sizes.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/api/tests/test_connect_datasets.py` & `deeplake-3.9.3/deeplake/api/tests/test_connect_datasets.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/api/tests/test_dataset.py` & `deeplake-3.9.3/deeplake/api/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/api/tests/test_dicom.py` & `deeplake-3.9.3/deeplake/api/tests/test_dicom.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/api/tests/test_downsample.py` & `deeplake-3.9.3/deeplake/api/tests/test_downsample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/api/tests/test_events.py` & `deeplake-3.9.3/deeplake/api/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/api/tests/test_grayscale.py` & `deeplake-3.9.3/deeplake/api/tests/test_grayscale.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/api/tests/test_info.py` & `deeplake-3.9.3/deeplake/api/tests/test_info.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/api/tests/test_insertion_out_of_order.py` & `deeplake-3.9.3/deeplake/api/tests/test_insertion_out_of_order.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/api/tests/test_json.py` & `deeplake-3.9.3/deeplake/api/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/api/tests/test_link.py` & `deeplake-3.9.3/deeplake/api/tests/test_link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/api/tests/test_link_tiled.py` & `deeplake-3.9.3/deeplake/api/tests/test_link_tiled.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/api/tests/test_linking.py` & `deeplake-3.9.3/deeplake/api/tests/test_linking.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/api/tests/test_mesh.py` & `deeplake-3.9.3/deeplake/api/tests/test_mesh.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/api/tests/test_meta.py` & `deeplake-3.9.3/deeplake/api/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/api/tests/test_nifti.py` & `deeplake-3.9.3/deeplake/api/tests/test_nifti.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/api/tests/test_none.py` & `deeplake-3.9.3/deeplake/api/tests/test_none.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/api/tests/test_partial_upload.py` & `deeplake-3.9.3/deeplake/api/tests/test_partial_upload.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/api/tests/test_pickle.py` & `deeplake-3.9.3/deeplake/api/tests/test_pickle.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/api/tests/test_point_cloud.py` & `deeplake-3.9.3/deeplake/api/tests/test_point_cloud.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/api/tests/test_polygons.py` & `deeplake-3.9.3/deeplake/api/tests/test_polygons.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/api/tests/test_pop.py` & `deeplake-3.9.3/deeplake/api/tests/test_pop.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/api/tests/test_readonly.py` & `deeplake-3.9.3/deeplake/api/tests/test_readonly.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/api/tests/test_rechunk.py` & `deeplake-3.9.3/deeplake/api/tests/test_rechunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/api/tests/test_reset.py` & `deeplake-3.9.3/deeplake/api/tests/test_reset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/api/tests/test_sample_info.py` & `deeplake-3.9.3/deeplake/api/tests/test_sample_info.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/api/tests/test_tag.py` & `deeplake-3.9.3/deeplake/api/tests/test_tag.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/api/tests/test_text.py` & `deeplake-3.9.3/deeplake/api/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/api/tests/test_update_samples.py` & `deeplake-3.9.3/deeplake/api/tests/test_update_samples.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/api/tests/test_video.py` & `deeplake-3.9.3/deeplake/api/tests/test_video.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/api/tests/test_views.py` & `deeplake-3.9.3/deeplake/api/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/api/tiled.py` & `deeplake-3.9.3/deeplake/api/tiled.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/auto/structured/base.py` & `deeplake-3.9.3/deeplake/auto/structured/base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/auto/structured/dataframe.py` & `deeplake-3.9.3/deeplake/auto/structured/dataframe.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/auto/tests/test_coco_template.py` & `deeplake-3.9.3/deeplake/auto/tests/test_coco_template.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/auto/tests/test_ingestion.py` & `deeplake-3.9.3/deeplake/auto/tests/test_ingestion.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/auto/tests/test_kaggle.py` & `deeplake-3.9.3/deeplake/auto/tests/test_kaggle.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/auto/tests/test_yolo_template.py` & `deeplake-3.9.3/deeplake/auto/tests/test_yolo_template.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/auto/unstructured/base.py` & `deeplake-3.9.3/deeplake/auto/unstructured/base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/auto/unstructured/coco/coco.py` & `deeplake-3.9.3/deeplake/auto/unstructured/coco/coco.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/auto/unstructured/coco/constants.py` & `deeplake-3.9.3/deeplake/auto/unstructured/coco/constants.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/auto/unstructured/coco/convert.py` & `deeplake-3.9.3/deeplake/auto/unstructured/coco/convert.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/auto/unstructured/coco/utils.py` & `deeplake-3.9.3/deeplake/auto/unstructured/coco/utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/auto/unstructured/image_classification.py` & `deeplake-3.9.3/deeplake/auto/unstructured/image_classification.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/auto/unstructured/kaggle.py` & `deeplake-3.9.3/deeplake/auto/unstructured/kaggle.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/auto/unstructured/util.py` & `deeplake-3.9.3/deeplake/auto/unstructured/util.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/auto/unstructured/yolo/utils.py` & `deeplake-3.9.3/deeplake/auto/unstructured/yolo/utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/auto/unstructured/yolo/yolo.py` & `deeplake-3.9.3/deeplake/auto/unstructured/yolo/yolo.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/client/auth/__init__.py` & `deeplake-3.9.3/deeplake/client/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/client/auth/activeloop.py` & `deeplake-3.9.3/deeplake/client/auth/activeloop.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/client/auth/auth_context.py` & `deeplake-3.9.3/deeplake/client/auth/auth_context.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/client/auth/azure.py` & `deeplake-3.9.3/deeplake/client/auth/azure.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/client/auth/test_auth_context.py` & `deeplake-3.9.3/deeplake/client/auth/test_auth_context.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/client/client.py` & `deeplake-3.9.3/deeplake/client/client.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/client/config.py` & `deeplake-3.9.3/deeplake/client/config.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/client/log.py` & `deeplake-3.9.3/deeplake/client/log.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/client/test_client.py` & `deeplake-3.9.3/deeplake/client/test_client.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/client/utils.py` & `deeplake-3.9.3/deeplake/client/utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/compression.py` & `deeplake-3.9.3/deeplake/compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/constants.py` & `deeplake-3.9.3/deeplake/constants.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/chunk/base_chunk.py` & `deeplake-3.9.3/deeplake/core/chunk/base_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/chunk/chunk_compressed_chunk.py` & `deeplake-3.9.3/deeplake/core/chunk/chunk_compressed_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/chunk/sample_compressed_chunk.py` & `deeplake-3.9.3/deeplake/core/chunk/sample_compressed_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/chunk/test_chunk_compressed.py` & `deeplake-3.9.3/deeplake/core/chunk/test_chunk_compressed.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/chunk/test_sample_compressed.py` & `deeplake-3.9.3/deeplake/core/chunk/test_sample_compressed.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/chunk/test_uncompressed.py` & `deeplake-3.9.3/deeplake/core/chunk/test_uncompressed.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/chunk/uncompressed_chunk.py` & `deeplake-3.9.3/deeplake/core/chunk/uncompressed_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/chunk_engine.py` & `deeplake-3.9.3/deeplake/core/chunk_engine.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/compression.py` & `deeplake-3.9.3/deeplake/core/compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/compute/process.py` & `deeplake-3.9.3/deeplake/core/compute/process.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/compute/provider.py` & `deeplake-3.9.3/deeplake/core/compute/provider.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/compute/ray.py` & `deeplake-3.9.3/deeplake/core/compute/ray.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/compute/serial.py` & `deeplake-3.9.3/deeplake/core/compute/serial.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/compute/thread.py` & `deeplake-3.9.3/deeplake/core/compute/thread.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/dataset/__init__.py` & `deeplake-3.9.3/deeplake/core/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/dataset/dataset.py` & `deeplake-3.9.3/deeplake/core/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/dataset/deeplake_cloud_dataset.py` & `deeplake-3.9.3/deeplake/core/dataset/deeplake_cloud_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/dataset/indra_dataset_view.py` & `deeplake-3.9.3/deeplake/core/dataset/indra_dataset_view.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/dataset/indra_tensor_view.py` & `deeplake-3.9.3/deeplake/core/dataset/indra_tensor_view.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/dataset/invalid_view.py` & `deeplake-3.9.3/deeplake/core/dataset/invalid_view.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/dataset/view_entry.py` & `deeplake-3.9.3/deeplake/core/dataset/view_entry.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/fast_forwarding.py` & `deeplake-3.9.3/deeplake/core/fast_forwarding.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/index/index.py` & `deeplake-3.9.3/deeplake/core/index/index.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/index_maintenance.py` & `deeplake-3.9.3/deeplake/core/index_maintenance.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/io.py` & `deeplake-3.9.3/deeplake/core/io.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/ipc.py` & `deeplake-3.9.3/deeplake/core/ipc.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/link_creds.py` & `deeplake-3.9.3/deeplake/core/link_creds.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/linked_chunk_engine.py` & `deeplake-3.9.3/deeplake/core/linked_chunk_engine.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/linked_sample.py` & `deeplake-3.9.3/deeplake/core/linked_sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/linked_tiled_sample.py` & `deeplake-3.9.3/deeplake/core/linked_tiled_sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/lock.py` & `deeplake-3.9.3/deeplake/core/lock.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/meta/dataset_meta.py` & `deeplake-3.9.3/deeplake/core/meta/dataset_meta.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/meta/encode/base_encoder.py` & `deeplake-3.9.3/deeplake/core/meta/encode/base_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/meta/encode/byte_positions.py` & `deeplake-3.9.3/deeplake/core/meta/encode/byte_positions.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/meta/encode/chunk_id.py` & `deeplake-3.9.3/deeplake/core/meta/encode/chunk_id.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/meta/encode/creds.py` & `deeplake-3.9.3/deeplake/core/meta/encode/creds.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/meta/encode/pad.py` & `deeplake-3.9.3/deeplake/core/meta/encode/pad.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/meta/encode/sequence.py` & `deeplake-3.9.3/deeplake/core/meta/encode/sequence.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/meta/encode/shape.py` & `deeplake-3.9.3/deeplake/core/meta/encode/shape.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py` & `deeplake-3.9.3/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py` & `deeplake-3.9.3/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py` & `deeplake-3.9.3/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/meta/encode/tests/test_shape_encoder.py` & `deeplake-3.9.3/deeplake/core/meta/encode/tests/test_shape_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py` & `deeplake-3.9.3/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/meta/encode/tile.py` & `deeplake-3.9.3/deeplake/core/meta/encode/tile.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/meta/tensor_meta.py` & `deeplake-3.9.3/deeplake/core/meta/tensor_meta.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/partial_reader.py` & `deeplake-3.9.3/deeplake/core/partial_reader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/partial_sample.py` & `deeplake-3.9.3/deeplake/core/partial_sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/polygon.py` & `deeplake-3.9.3/deeplake/core/polygon.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/query/autocomplete.py` & `deeplake-3.9.3/deeplake/core/query/autocomplete.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/query/filter.py` & `deeplake-3.9.3/deeplake/core/query/filter.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/query/query.py` & `deeplake-3.9.3/deeplake/core/query/query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/sample.py` & `deeplake-3.9.3/deeplake/core/sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/seed.py` & `deeplake-3.9.3/deeplake/core/seed.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/serialize.py` & `deeplake-3.9.3/deeplake/core/serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/storage/azure.py` & `deeplake-3.9.3/deeplake/core/storage/azure.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/storage/deeplake_memory_object.py` & `deeplake-3.9.3/deeplake/core/storage/deeplake_memory_object.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/storage/gcs.py` & `deeplake-3.9.3/deeplake/core/storage/gcs.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/storage/google_drive.py` & `deeplake-3.9.3/deeplake/core/storage/google_drive.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/storage/indra.py` & `deeplake-3.9.3/deeplake/core/storage/indra.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/storage/local.py` & `deeplake-3.9.3/deeplake/core/storage/local.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/storage/lru_cache.py` & `deeplake-3.9.3/deeplake/core/storage/lru_cache.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/storage/memory.py` & `deeplake-3.9.3/deeplake/core/storage/memory.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/storage/provider.py` & `deeplake-3.9.3/deeplake/core/storage/provider.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/storage/s3.py` & `deeplake-3.9.3/deeplake/core/storage/s3.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/tensor.py` & `deeplake-3.9.3/deeplake/core/tensor.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/tensor_link.py` & `deeplake-3.9.3/deeplake/core/tensor_link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/test_serialize.py` & `deeplake-3.9.3/deeplake/core/test_serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/tests/test_compression.py` & `deeplake-3.9.3/deeplake/core/tests/test_compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/tests/test_compute.py` & `deeplake-3.9.3/deeplake/core/tests/test_compute.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/tests/test_dataset.py` & `deeplake-3.9.3/deeplake/core/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/tests/test_indra_dataset.py` & `deeplake-3.9.3/deeplake/core/tests/test_indra_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/tests/test_io.py` & `deeplake-3.9.3/deeplake/core/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/tests/test_locking.py` & `deeplake-3.9.3/deeplake/core/tests/test_locking.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/tests/test_query.py` & `deeplake-3.9.3/deeplake/core/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/tests/test_readonly.py` & `deeplake-3.9.3/deeplake/core/tests/test_readonly.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/tests/test_serialize.py` & `deeplake-3.9.3/deeplake/core/tests/test_serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/tests/test_vdb_indexes.py` & `deeplake-3.9.3/deeplake/core/tests/test_vdb_indexes.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/tiling/deserialize.py` & `deeplake-3.9.3/deeplake/core/tiling/deserialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/tiling/optimizer.py` & `deeplake-3.9.3/deeplake/core/tiling/optimizer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/tiling/sample_tiles.py` & `deeplake-3.9.3/deeplake/core/tiling/sample_tiles.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/tiling/serialize.py` & `deeplake-3.9.3/deeplake/core/tiling/serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/tiling/test_optimizer.py` & `deeplake-3.9.3/deeplake/core/tiling/test_optimizer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/tiling/test_serialize.py` & `deeplake-3.9.3/deeplake/core/tiling/test_serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/transform/test_transform.py` & `deeplake-3.9.3/deeplake/core/transform/test_transform.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/transform/transform.py` & `deeplake-3.9.3/deeplake/core/transform/transform.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/transform/transform_dataset.py` & `deeplake-3.9.3/deeplake/core/transform/transform_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/transform/transform_tensor.py` & `deeplake-3.9.3/deeplake/core/transform/transform_tensor.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/vectorstore/__init__.py` & `deeplake-3.9.3/deeplake/core/vectorstore/__init__.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/vectorstore/dataset_handlers/client_side_dataset_handler.py` & `deeplake-3.9.3/deeplake/core/vectorstore/dataset_handlers/client_side_dataset_handler.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/vectorstore/dataset_handlers/dataset_handler_base.py` & `deeplake-3.9.3/deeplake/core/vectorstore/dataset_handlers/dataset_handler_base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/vectorstore/deep_memory/deep_memory.py` & `deeplake-3.9.3/deeplake/core/vectorstore/deep_memory/deep_memory.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/vectorstore/deep_memory/test_deepmemory.py` & `deeplake-3.9.3/deeplake/core/vectorstore/deep_memory/test_deepmemory.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/vectorstore/deeplake_vectorstore.py` & `deeplake-3.9.3/deeplake/core/vectorstore/deeplake_vectorstore.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/vectorstore/embeddings/embedder.py` & `deeplake-3.9.3/deeplake/core/vectorstore/embeddings/embedder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/vectorstore/embeddings/test_embedder.py` & `deeplake-3.9.3/deeplake/core/vectorstore/embeddings/test_embedder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/vectorstore/test_deeplake_vectorstore.py` & `deeplake-3.9.3/deeplake/core/vectorstore/test_deeplake_vectorstore.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/vectorstore/vector_search/dataset/dataset.py` & `deeplake-3.9.3/deeplake/core/vectorstore/vector_search/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/vectorstore/vector_search/dataset/test_dataset.py` & `deeplake-3.9.3/deeplake/core/vectorstore/vector_search/dataset/test_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/vectorstore/vector_search/filter/filter.py` & `deeplake-3.9.3/deeplake/core/vectorstore/vector_search/filter/filter.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/vectorstore/vector_search/filter/test_filter.py` & `deeplake-3.9.3/deeplake/core/vectorstore/vector_search/filter/test_filter.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/vectorstore/vector_search/indra/query.py` & `deeplake-3.9.3/deeplake/core/vectorstore/vector_search/indra/query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/vectorstore/vector_search/indra/search_algorithm.py` & `deeplake-3.9.3/deeplake/core/vectorstore/vector_search/indra/search_algorithm.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/vectorstore/vector_search/indra/test_indra.py` & `deeplake-3.9.3/deeplake/core/vectorstore/vector_search/indra/test_indra.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/distance_metric.py` & `deeplake-3.9.3/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/distance_metric.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/vectorstore/vector_search/indra/vector_search.py` & `deeplake-3.9.3/deeplake/core/vectorstore/vector_search/indra/vector_search.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/vectorstore/vector_search/ingestion/data_ingestion.py` & `deeplake-3.9.3/deeplake/core/vectorstore/vector_search/ingestion/data_ingestion.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/vectorstore/vector_search/ingestion/ingest_data.py` & `deeplake-3.9.3/deeplake/core/vectorstore/vector_search/ingestion/ingest_data.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/vectorstore/vector_search/ingestion/test_data_ingestion.py` & `deeplake-3.9.3/deeplake/core/vectorstore/vector_search/ingestion/test_data_ingestion.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/vectorstore/vector_search/python/search_algorithm.py` & `deeplake-3.9.3/deeplake/core/vectorstore/vector_search/python/search_algorithm.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/vectorstore/vector_search/python/test_vector_search.py` & `deeplake-3.9.3/deeplake/core/vectorstore/vector_search/python/test_vector_search.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/vectorstore/vector_search/python/vector_search.py` & `deeplake-3.9.3/deeplake/core/vectorstore/vector_search/python/vector_search.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/vectorstore/vector_search/utils.py` & `deeplake-3.9.3/deeplake/core/vectorstore/vector_search/utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/vectorstore/vector_search/vector_search.py` & `deeplake-3.9.3/deeplake/core/vectorstore/vector_search/vector_search.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/version_control/commit_chunk_map.py` & `deeplake-3.9.3/deeplake/core/version_control/commit_chunk_map.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/version_control/commit_diff.py` & `deeplake-3.9.3/deeplake/core/version_control/commit_diff.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/version_control/commit_node.py` & `deeplake-3.9.3/deeplake/core/version_control/commit_node.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/version_control/dataset_diff.py` & `deeplake-3.9.3/deeplake/core/version_control/dataset_diff.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/version_control/test_merge.py` & `deeplake-3.9.3/deeplake/core/version_control/test_merge.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/core/version_control/test_version_control.py` & `deeplake-3.9.3/deeplake/core/version_control/test_version_control.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/enterprise/convert_to_libdeeplake.py` & `deeplake-3.9.3/deeplake/enterprise/convert_to_libdeeplake.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/enterprise/dataloader.py` & `deeplake-3.9.3/deeplake/enterprise/dataloader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/enterprise/dummy_dataloader.py` & `deeplake-3.9.3/deeplake/enterprise/dummy_dataloader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/enterprise/libdeeplake_query.py` & `deeplake-3.9.3/deeplake/enterprise/libdeeplake_query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/enterprise/test_pytorch.py` & `deeplake-3.9.3/deeplake/enterprise/test_pytorch.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/enterprise/test_query.py` & `deeplake-3.9.3/deeplake/enterprise/test_query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/enterprise/test_tensorflow.py` & `deeplake-3.9.3/deeplake/enterprise/test_tensorflow.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/enterprise/util.py` & `deeplake-3.9.3/deeplake/enterprise/util.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/hooks.py` & `deeplake-3.9.3/deeplake/hooks.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/htype.py` & `deeplake-3.9.3/deeplake/htype.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/integrations/huggingface/huggingface.py` & `deeplake-3.9.3/deeplake/integrations/huggingface/huggingface.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/integrations/mmdet/mmdet_.py` & `deeplake-3.9.3/deeplake/integrations/mmdet/mmdet_.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/integrations/mmdet/mmdet_runners.py` & `deeplake-3.9.3/deeplake/integrations/mmdet/mmdet_runners.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/integrations/mmdet/mmdet_utils.py` & `deeplake-3.9.3/deeplake/integrations/mmdet/mmdet_utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/integrations/pytorch/common.py` & `deeplake-3.9.3/deeplake/integrations/pytorch/common.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/integrations/pytorch/dataset.py` & `deeplake-3.9.3/deeplake/integrations/pytorch/dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/integrations/pytorch/pytorch.py` & `deeplake-3.9.3/deeplake/integrations/pytorch/pytorch.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/integrations/pytorch/shuffle_buffer.py` & `deeplake-3.9.3/deeplake/integrations/pytorch/shuffle_buffer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/integrations/tf/common.py` & `deeplake-3.9.3/deeplake/integrations/tf/common.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/integrations/tf/datasettotensorflow.py` & `deeplake-3.9.3/deeplake/integrations/tf/datasettotensorflow.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/integrations/tf/deeplake_tensorflow_dataset.py` & `deeplake-3.9.3/deeplake/integrations/tf/deeplake_tensorflow_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/integrations/wandb/wandb.py` & `deeplake-3.9.3/deeplake/integrations/wandb/wandb.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/tests/cache_fixtures.py` & `deeplake-3.9.3/deeplake/tests/cache_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/tests/client_fixtures.py` & `deeplake-3.9.3/deeplake/tests/client_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/tests/common.py` & `deeplake-3.9.3/deeplake/tests/common.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/tests/dataset_fixtures.py` & `deeplake-3.9.3/deeplake/tests/dataset_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/tests/path_fixtures.py` & `deeplake-3.9.3/deeplake/tests/path_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/tests/storage_fixtures.py` & `deeplake-3.9.3/deeplake/tests/storage_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/util/access_method.py` & `deeplake-3.9.3/deeplake/util/access_method.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/util/agreement.py` & `deeplake-3.9.3/deeplake/util/agreement.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/util/array_list.py` & `deeplake-3.9.3/deeplake/util/array_list.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/util/assert_byte_indexes.py` & `deeplake-3.9.3/deeplake/util/assert_byte_indexes.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/util/auto.py` & `deeplake-3.9.3/deeplake/util/auto.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/util/bugout_reporter.py` & `deeplake-3.9.3/deeplake/util/bugout_reporter.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/util/cache_chain.py` & `deeplake-3.9.3/deeplake/util/cache_chain.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/util/casting.py` & `deeplake-3.9.3/deeplake/util/casting.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/util/check_latest_version.py` & `deeplake-3.9.3/deeplake/util/check_latest_version.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/util/chunk_engine.py` & `deeplake-3.9.3/deeplake/util/chunk_engine.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/util/class_label.py` & `deeplake-3.9.3/deeplake/util/class_label.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/util/compute.py` & `deeplake-3.9.3/deeplake/util/compute.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/util/connect_dataset.py` & `deeplake-3.9.3/deeplake/util/connect_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/util/dataset.py` & `deeplake-3.9.3/deeplake/util/dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/util/diff.py` & `deeplake-3.9.3/deeplake/util/diff.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/util/downsample.py` & `deeplake-3.9.3/deeplake/util/downsample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/util/encoder.py` & `deeplake-3.9.3/deeplake/util/encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/util/exceptions.py` & `deeplake-3.9.3/deeplake/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/util/exif.py` & `deeplake-3.9.3/deeplake/util/exif.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/util/from_tfds.py` & `deeplake-3.9.3/deeplake/util/from_tfds.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/util/htype.py` & `deeplake-3.9.3/deeplake/util/htype.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/util/image.py` & `deeplake-3.9.3/deeplake/util/image.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/util/invalid_view_op.py` & `deeplake-3.9.3/deeplake/util/invalid_view_op.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/util/iteration_warning.py` & `deeplake-3.9.3/deeplake/util/iteration_warning.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/util/json.py` & `deeplake-3.9.3/deeplake/util/json.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/util/keys.py` & `deeplake-3.9.3/deeplake/util/keys.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/util/link.py` & `deeplake-3.9.3/deeplake/util/link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/util/logging.py` & `deeplake-3.9.3/deeplake/util/logging.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/util/merge.py` & `deeplake-3.9.3/deeplake/util/merge.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/util/modified.py` & `deeplake-3.9.3/deeplake/util/modified.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/util/notebook.py` & `deeplake-3.9.3/deeplake/util/notebook.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/util/object_3d/mesh.py` & `deeplake-3.9.3/deeplake/util/object_3d/mesh.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/util/object_3d/object_base_3d.py` & `deeplake-3.9.3/deeplake/util/object_3d/object_base_3d.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/util/object_3d/ply_parser.py` & `deeplake-3.9.3/deeplake/util/object_3d/ply_parser.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/util/object_3d/ply_parser_base.py` & `deeplake-3.9.3/deeplake/util/object_3d/ply_parser_base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/util/object_3d/ply_parsers.py` & `deeplake-3.9.3/deeplake/util/object_3d/ply_parsers.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/util/object_3d/ply_reader.py` & `deeplake-3.9.3/deeplake/util/object_3d/ply_reader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/util/object_3d/ply_reader_base.py` & `deeplake-3.9.3/deeplake/util/object_3d/ply_reader_base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/util/object_3d/ply_readers.py` & `deeplake-3.9.3/deeplake/util/object_3d/ply_readers.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/util/object_3d/point_cloud.py` & `deeplake-3.9.3/deeplake/util/object_3d/point_cloud.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/util/object_3d/read_3d_data.py` & `deeplake-3.9.3/deeplake/util/object_3d/read_3d_data.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/util/path.py` & `deeplake-3.9.3/deeplake/util/path.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/util/pretty_print.py` & `deeplake-3.9.3/deeplake/util/pretty_print.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/util/remove_cache.py` & `deeplake-3.9.3/deeplake/util/remove_cache.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/util/scheduling.py` & `deeplake-3.9.3/deeplake/util/scheduling.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/util/shape_interval.py` & `deeplake-3.9.3/deeplake/util/shape_interval.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/util/spinner.py` & `deeplake-3.9.3/deeplake/util/spinner.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/util/split.py` & `deeplake-3.9.3/deeplake/util/split.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/util/storage.py` & `deeplake-3.9.3/deeplake/util/storage.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/util/tag.py` & `deeplake-3.9.3/deeplake/util/tag.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/util/tensor_db.py` & `deeplake-3.9.3/deeplake/util/tensor_db.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/util/testing.py` & `deeplake-3.9.3/deeplake/util/testing.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/util/tests/test_auto.py` & `deeplake-3.9.3/deeplake/util/tests/test_auto.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/util/tests/test_connect_dataset.py` & `deeplake-3.9.3/deeplake/util/tests/test_connect_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/util/tests/test_iterable_ordered_dict.py` & `deeplake-3.9.3/deeplake/util/tests/test_iterable_ordered_dict.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/util/tests/test_keys.py` & `deeplake-3.9.3/deeplake/util/tests/test_keys.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/util/tests/test_read.py` & `deeplake-3.9.3/deeplake/util/tests/test_read.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/util/tests/test_shape_interval.py` & `deeplake-3.9.3/deeplake/util/tests/test_shape_interval.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/util/tests/test_split.py` & `deeplake-3.9.3/deeplake/util/tests/test_split.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/util/tests/test_tensor_db.py` & `deeplake-3.9.3/deeplake/util/tests/test_tensor_db.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/util/tests/test_version_control.py` & `deeplake-3.9.3/deeplake/util/tests/test_version_control.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/util/tests/test_video.py` & `deeplake-3.9.3/deeplake/util/tests/test_video.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/util/transform.py` & `deeplake-3.9.3/deeplake/util/transform.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/util/version_control.py` & `deeplake-3.9.3/deeplake/util/version_control.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/util/video.py` & `deeplake-3.9.3/deeplake/util/video.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/visualizer/video_streaming.py` & `deeplake-3.9.3/deeplake/visualizer/video_streaming.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake/visualizer/visualizer.py` & `deeplake-3.9.3/deeplake/visualizer/visualizer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake.egg-info/PKG-INFO` & `deeplake-3.9.3/deeplake.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deeplake
-Version: 3.9.2
+Version: 3.9.3
 Summary: Activeloop Deep Lake
 Author: activeloop.ai
 Author-email: support@activeloop.ai
 License: MPL-2.0
 Project-URL: Documentation, https://docs.activeloop.ai/
 Project-URL: Source, https://github.com/activeloopai/deeplake
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: deeplake Version: 3.9.2 Summary: Activeloop Deep
+Metadata-Version: 2.1 Name: deeplake Version: 3.9.3 Summary: Activeloop Deep
 Lake Author: activeloop.ai Author-email: support@activeloop.ai License: MPL-2.0
 Project-URL: Documentation, https://docs.activeloop.ai/ Project-URL: Source,
 https://github.com/activeloopai/deeplake Classifier: License :: OSI Approved ::
 Mozilla Public License 2.0 (MPL 2.0) Description-Content-Type: text/markdown
 Provides-Extra: audio Provides-Extra: video Provides-Extra: av Provides-Extra:
 gcp Provides-Extra: azure Provides-Extra: dicom Provides-Extra: medical
 Provides-Extra: visualizer Provides-Extra: gdrive Provides-Extra: point_cloud
```

### Comparing `deeplake-3.9.2/deeplake.egg-info/SOURCES.txt` & `deeplake-3.9.3/deeplake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deeplake-3.9.2/deeplake.egg-info/requires.txt` & `deeplake-3.9.3/deeplake.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -4,35 +4,35 @@
 click
 pathos
 humbug>=0.3.1
 tqdm
 lz4
 pyjwt
 pydantic
-libdeeplake==0.0.123
+libdeeplake==0.0.124
 
 [:python_version >= "3.7" and sys_platform != "win32"]
 aioboto3>=10.4.0
 nest_asyncio
 
 [all]
-laspy
-google-api-python-client~=2.31.0
-azure-storage-blob
-pydicom
-IPython
-google-auth~=2.0.1
+google-auth-oauthlib~=0.4.5
 azure-identity
-azure-cli
+google-auth~=2.0.1
+IPython
 oauth2client~=4.1.3
 google-cloud-storage~=1.42.0
+google-api-python-client~=2.31.0
+pydicom
+azure-storage-blob
+laspy
 nibabel
 flask
-google-auth-oauthlib~=0.4.5
-libdeeplake==0.0.123
+azure-cli
+libdeeplake==0.0.124
 
 [all:python_version >= "3.7" or sys_platform != "win32"]
 av>=8.1.0
 
 [audio]
 
 [audio:python_version >= "3.7" or sys_platform != "win32"]
@@ -49,15 +49,15 @@
 azure-storage-blob
 
 [dicom]
 pydicom
 nibabel
 
 [enterprise]
-libdeeplake==0.0.123
+libdeeplake==0.0.124
 pyjwt
 
 [gcp]
 google-cloud-storage~=1.42.0
 google-auth~=2.0.1
 google-auth-oauthlib~=0.4.5
```

### Comparing `deeplake-3.9.2/setup.py` & `deeplake-3.9.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 all_extras = {r for v in extras.values() for r in v}
 install_requires = [req_map[r] for r in req_map if r not in all_extras]
 extras_require = {k: [req_map[r] for r in v] for k, v in extras.items()}
 
 extras_require["all"] = [req_map[r] for r in all_extras]
 
 if libdeeplake_available():
-    libdeeplake = "libdeeplake==0.0.123"
+    libdeeplake = "libdeeplake==0.0.124"
     extras_require["enterprise"] = [libdeeplake, "pyjwt"]
     extras_require["all"].append(libdeeplake)
     install_requires.append(libdeeplake)
 
 init_file = os.path.join(project_name, "__init__.py")
```

