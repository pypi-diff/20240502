# Comparing `tmp/eotdl-2024.4.25.tar.gz` & `tmp/eotdl-2024.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eotdl-2024.4.25.tar", max compression
+gzip compressed data, was "eotdl-2024.5.2.tar", max compression
```

## Comparing `eotdl-2024.4.25.tar` & `eotdl-2024.5.2.tar`

### file list

```diff
@@ -1,77 +1,78 @@
--rwxr-xr-x   0        0        0     2849 2024-04-25 07:56:54.008592 eotdl-2024.4.25/README.md
--rwxr-xr-x   0        0        0       27 2024-04-25 10:44:50.799369 eotdl-2024.4.25/eotdl/__init__.py
--rwxr-xr-x   0        0        0      231 2024-04-25 07:56:54.008592 eotdl-2024.4.25/eotdl/access/__init__.py
--rwxr-xr-x   0        0        0      107 2024-04-25 07:56:54.008592 eotdl-2024.4.25/eotdl/access/airbus/__init__.py
--rwxr-xr-x   0        0        0    12018 2024-04-25 07:56:54.008592 eotdl-2024.4.25/eotdl/access/airbus/client.py
--rwxr-xr-x   0        0        0     1009 2024-04-25 07:56:54.008592 eotdl-2024.4.25/eotdl/access/airbus/parameters.py
--rwxr-xr-x   0        0        0      652 2024-04-25 07:56:54.008592 eotdl-2024.4.25/eotdl/access/airbus/utils.py
--rwxr-xr-x   0        0        0     1568 2024-04-25 07:56:54.008592 eotdl-2024.4.25/eotdl/access/download.py
--rwxr-xr-x   0        0        0      633 2024-04-25 07:56:54.008592 eotdl-2024.4.25/eotdl/access/search.py
--rwxr-xr-x   0        0        0      238 2024-04-25 07:56:54.008592 eotdl-2024.4.25/eotdl/access/sentinelhub/__init__.py
--rwxr-xr-x   0        0        0     4098 2024-04-25 07:56:54.008592 eotdl-2024.4.25/eotdl/access/sentinelhub/client.py
--rwxr-xr-x   0        0        0     4142 2024-04-25 07:56:54.008592 eotdl-2024.4.25/eotdl/access/sentinelhub/evalscripts.py
--rwxr-xr-x   0        0        0     2061 2024-04-25 07:56:54.008592 eotdl-2024.4.25/eotdl/access/sentinelhub/parameters.py
--rwxr-xr-x   0        0        0     3295 2024-04-25 07:56:54.008592 eotdl-2024.4.25/eotdl/access/sentinelhub/utils.py
--rwxr-xr-x   0        0        0       99 2024-04-25 07:56:54.008592 eotdl-2024.4.25/eotdl/auth/__init__.py
--rwxr-xr-x   0        0        0     2029 2024-04-25 07:56:54.008592 eotdl-2024.4.25/eotdl/auth/auth.py
--rwxr-xr-x   0        0        0      308 2024-04-25 07:56:54.008592 eotdl-2024.4.25/eotdl/auth/errors.py
--rwxr-xr-x   0        0        0      115 2024-04-25 07:56:54.008592 eotdl-2024.4.25/eotdl/auth/is_logged.py
--rwxr-xr-x   0        0        0      161 2024-04-25 07:56:54.008592 eotdl-2024.4.25/eotdl/auth/logout.py
--rwxr-xr-x   0        0        0      660 2024-04-25 07:56:54.008592 eotdl-2024.4.25/eotdl/cli.py
--rwxr-xr-x   0        0        0        0 2024-04-25 07:56:54.008592 eotdl-2024.4.25/eotdl/commands/__init__.py
--rwxr-xr-x   0        0        0     1544 2024-04-25 07:56:54.008592 eotdl-2024.4.25/eotdl/commands/auth.py
--rwxr-xr-x   0        0        0     5205 2024-04-25 08:14:02.237444 eotdl-2024.4.25/eotdl/commands/datasets.py
--rwxr-xr-x   0        0        0     4873 2024-04-25 07:56:54.008592 eotdl-2024.4.25/eotdl/commands/models.py
--rwxr-xr-x   0        0        0      269 2024-04-25 07:56:54.008592 eotdl-2024.4.25/eotdl/curation/__init__.py
--rwxr-xr-x   0        0        0      220 2024-04-25 07:56:54.008592 eotdl-2024.4.25/eotdl/curation/stac/__init__.py
--rwxr-xr-x   0        0        0     3347 2024-04-25 07:56:54.008592 eotdl-2024.4.25/eotdl/curation/stac/assets.py
--rwxr-xr-x   0        0        0     5503 2024-04-25 10:24:33.763860 eotdl-2024.4.25/eotdl/curation/stac/dataframe.py
--rwxr-xr-x   0        0        0     8493 2024-04-25 07:56:54.008592 eotdl-2024.4.25/eotdl/curation/stac/dataframe_bck.py
--rwxr-xr-x   0        0        0     1520 2024-04-25 07:56:54.008592 eotdl-2024.4.25/eotdl/curation/stac/dataframe_labeling.py
--rwxr-xr-x   0        0        0      629 2024-04-25 07:56:54.008592 eotdl-2024.4.25/eotdl/curation/stac/extensions/__init__.py
--rwxr-xr-x   0        0        0      671 2024-04-25 07:56:54.008592 eotdl-2024.4.25/eotdl/curation/stac/extensions/base.py
--rwxr-xr-x   0        0        0      370 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/curation/stac/extensions/dem.py
--rwxr-xr-x   0        0        0     4004 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/curation/stac/extensions/eo.py
--rwxr-xr-x   0        0        0      159 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/curation/stac/extensions/label/__init__.py
--rwxr-xr-x   0        0        0     4069 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/curation/stac/extensions/label/base.py
--rwxr-xr-x   0        0        0     8074 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/curation/stac/extensions/label/image_name_labeler.py
--rwxr-xr-x   0        0        0     8787 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/curation/stac/extensions/label/scaneo.py
--rwxr-xr-x   0        0        0    21429 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/curation/stac/extensions/ml_dataset.py
--rwxr-xr-x   0        0        0     1236 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/curation/stac/extensions/projection.py
--rwxr-xr-x   0        0        0     1540 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/curation/stac/extensions/raster.py
--rwxr-xr-x   0        0        0     1633 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/curation/stac/extensions/sar.py
--rwxr-xr-x   0        0        0     5108 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/curation/stac/extent.py
--rwxr-xr-x   0        0        0     1529 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/curation/stac/parsers.py
--rwxr-xr-x   0        0        0    13180 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/curation/stac/stac.py
--rwxr-xr-x   0        0        0      170 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/datasets/__init__.py
--rwxr-xr-x   0        0        0     3667 2024-04-25 10:24:33.763860 eotdl-2024.4.25/eotdl/datasets/download.py
--rwxr-xr-x   0        0        0     5806 2024-04-25 10:24:33.763860 eotdl-2024.4.25/eotdl/datasets/ingest.py
--rwxr-xr-x   0        0        0     1457 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/datasets/metadata.py
--rwxr-xr-x   0        0        0     1041 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/datasets/retrieve.py
--rw-r--r--   0        0        0      386 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/datasets/update.py
--rwxr-xr-x   0        0        0       53 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/files/__init__.py
--rwxr-xr-x   0        0        0     6185 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/files/ingest.py
--rwxr-xr-x   0        0        0      108 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/models/__init__.py
--rwxr-xr-x   0        0        0     4119 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/models/download.py
--rwxr-xr-x   0        0        0     3381 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/models/ingest.py
--rwxr-xr-x   0        0        0     1443 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/models/metadata.py
--rwxr-xr-x   0        0        0      664 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/models/retrieve.py
--rw-r--r--   0        0        0      374 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/models/update.py
--rwxr-xr-x   0        0        0      791 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/repos/APIRepo.py
--rwxr-xr-x   0        0        0      957 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/repos/AuthAPIRepo.py
--rwxr-xr-x   0        0        0     1154 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/repos/AuthRepo.py
--rwxr-xr-x   0        0        0     2660 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/repos/DatasetsAPIRepo.py
--rwxr-xr-x   0        0        0     6768 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/repos/FilesAPIRepo.py
--rwxr-xr-x   0        0        0     1677 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/repos/ModelsAPIRepo.py
--rwxr-xr-x   0        0        0      222 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/repos/__init__.py
--rwxr-xr-x   0        0        0       41 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/shared/__init__.py
--rwxr-xr-x   0        0        0      479 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/shared/checksum.py
--rwxr-xr-x   0        0        0      178 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/tools/__init__.py
--rwxr-xr-x   0        0        0     7320 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/tools/geo_utils.py
--rwxr-xr-x   0        0        0     1664 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/tools/metadata.py
--rwxr-xr-x   0        0        0     1152 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/tools/paths.py
--rwxr-xr-x   0        0        0     5763 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/tools/stac.py
--rwxr-xr-x   0        0        0     4691 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/tools/time_utils.py
--rwxr-xr-x   0        0        0     6354 2024-04-25 07:56:54.012591 eotdl-2024.4.25/eotdl/tools/tools.py
--rwxr-xr-x   0        0        0      944 2024-04-25 10:44:50.795369 eotdl-2024.4.25/pyproject.toml
--rw-r--r--   0        0        0     4052 1970-01-01 00:00:00.000000 eotdl-2024.4.25/PKG-INFO
+-rwxr-xr-x   0        0        0     2849 2024-04-25 07:56:54.008592 eotdl-2024.5.2/README.md
+-rwxr-xr-x   0        0        0       27 2024-05-02 13:54:59.689017 eotdl-2024.5.2/eotdl/__init__.py
+-rwxr-xr-x   0        0        0      231 2024-04-25 07:56:54.008592 eotdl-2024.5.2/eotdl/access/__init__.py
+-rwxr-xr-x   0        0        0      107 2024-04-25 07:56:54.008592 eotdl-2024.5.2/eotdl/access/airbus/__init__.py
+-rwxr-xr-x   0        0        0    12018 2024-04-25 07:56:54.008592 eotdl-2024.5.2/eotdl/access/airbus/client.py
+-rwxr-xr-x   0        0        0     1009 2024-04-25 07:56:54.008592 eotdl-2024.5.2/eotdl/access/airbus/parameters.py
+-rwxr-xr-x   0        0        0      652 2024-04-25 07:56:54.008592 eotdl-2024.5.2/eotdl/access/airbus/utils.py
+-rwxr-xr-x   0        0        0     1845 2024-05-02 08:47:51.838648 eotdl-2024.5.2/eotdl/access/download.py
+-rwxr-xr-x   0        0        0      633 2024-04-25 07:56:54.008592 eotdl-2024.5.2/eotdl/access/search.py
+-rwxr-xr-x   0        0        0      238 2024-04-25 07:56:54.008592 eotdl-2024.5.2/eotdl/access/sentinelhub/__init__.py
+-rwxr-xr-x   0        0        0     4098 2024-04-25 07:56:54.008592 eotdl-2024.5.2/eotdl/access/sentinelhub/client.py
+-rwxr-xr-x   0        0        0     4142 2024-04-25 07:56:54.008592 eotdl-2024.5.2/eotdl/access/sentinelhub/evalscripts.py
+-rwxr-xr-x   0        0        0     2061 2024-04-25 07:56:54.008592 eotdl-2024.5.2/eotdl/access/sentinelhub/parameters.py
+-rwxr-xr-x   0        0        0     3560 2024-05-02 08:47:51.838648 eotdl-2024.5.2/eotdl/access/sentinelhub/utils.py
+-rwxr-xr-x   0        0        0       99 2024-04-25 07:56:54.008592 eotdl-2024.5.2/eotdl/auth/__init__.py
+-rwxr-xr-x   0        0        0     2029 2024-04-25 07:56:54.008592 eotdl-2024.5.2/eotdl/auth/auth.py
+-rwxr-xr-x   0        0        0      308 2024-04-25 07:56:54.008592 eotdl-2024.5.2/eotdl/auth/errors.py
+-rwxr-xr-x   0        0        0      115 2024-04-25 07:56:54.008592 eotdl-2024.5.2/eotdl/auth/is_logged.py
+-rwxr-xr-x   0        0        0      161 2024-04-25 07:56:54.008592 eotdl-2024.5.2/eotdl/auth/logout.py
+-rwxr-xr-x   0        0        0      660 2024-04-25 07:56:54.008592 eotdl-2024.5.2/eotdl/cli.py
+-rwxr-xr-x   0        0        0        0 2024-04-25 07:56:54.008592 eotdl-2024.5.2/eotdl/commands/__init__.py
+-rwxr-xr-x   0        0        0     1544 2024-04-25 07:56:54.008592 eotdl-2024.5.2/eotdl/commands/auth.py
+-rwxr-xr-x   0        0        0     5205 2024-04-25 08:14:02.237444 eotdl-2024.5.2/eotdl/commands/datasets.py
+-rwxr-xr-x   0        0        0     4873 2024-04-25 07:56:54.008592 eotdl-2024.5.2/eotdl/commands/models.py
+-rwxr-xr-x   0        0        0      269 2024-04-25 07:56:54.008592 eotdl-2024.5.2/eotdl/curation/__init__.py
+-rwxr-xr-x   0        0        0      220 2024-04-25 07:56:54.008592 eotdl-2024.5.2/eotdl/curation/stac/__init__.py
+-rwxr-xr-x   0        0        0     3347 2024-04-25 07:56:54.008592 eotdl-2024.5.2/eotdl/curation/stac/assets.py
+-rwxr-xr-x   0        0        0     5503 2024-04-25 10:24:33.763860 eotdl-2024.5.2/eotdl/curation/stac/dataframe.py
+-rwxr-xr-x   0        0        0     8493 2024-04-25 07:56:54.008592 eotdl-2024.5.2/eotdl/curation/stac/dataframe_bck.py
+-rwxr-xr-x   0        0        0     1520 2024-04-25 07:56:54.008592 eotdl-2024.5.2/eotdl/curation/stac/dataframe_labeling.py
+-rwxr-xr-x   0        0        0      629 2024-04-25 07:56:54.008592 eotdl-2024.5.2/eotdl/curation/stac/extensions/__init__.py
+-rwxr-xr-x   0        0        0      671 2024-04-25 07:56:54.008592 eotdl-2024.5.2/eotdl/curation/stac/extensions/base.py
+-rwxr-xr-x   0        0        0      370 2024-04-25 07:56:54.012591 eotdl-2024.5.2/eotdl/curation/stac/extensions/dem.py
+-rwxr-xr-x   0        0        0     4004 2024-04-25 07:56:54.012591 eotdl-2024.5.2/eotdl/curation/stac/extensions/eo.py
+-rwxr-xr-x   0        0        0      159 2024-04-25 07:56:54.012591 eotdl-2024.5.2/eotdl/curation/stac/extensions/label/__init__.py
+-rwxr-xr-x   0        0        0     4069 2024-04-25 07:56:54.012591 eotdl-2024.5.2/eotdl/curation/stac/extensions/label/base.py
+-rwxr-xr-x   0        0        0     8074 2024-04-25 07:56:54.012591 eotdl-2024.5.2/eotdl/curation/stac/extensions/label/image_name_labeler.py
+-rwxr-xr-x   0        0        0     8787 2024-04-25 07:56:54.012591 eotdl-2024.5.2/eotdl/curation/stac/extensions/label/scaneo.py
+-rwxr-xr-x   0        0        0    21429 2024-04-25 07:56:54.012591 eotdl-2024.5.2/eotdl/curation/stac/extensions/ml_dataset.py
+-rwxr-xr-x   0        0        0     1236 2024-04-25 07:56:54.012591 eotdl-2024.5.2/eotdl/curation/stac/extensions/projection.py
+-rwxr-xr-x   0        0        0     1540 2024-04-25 07:56:54.012591 eotdl-2024.5.2/eotdl/curation/stac/extensions/raster.py
+-rwxr-xr-x   0        0        0     1633 2024-04-25 07:56:54.012591 eotdl-2024.5.2/eotdl/curation/stac/extensions/sar.py
+-rwxr-xr-x   0        0        0     5108 2024-04-25 07:56:54.012591 eotdl-2024.5.2/eotdl/curation/stac/extent.py
+-rwxr-xr-x   0        0        0     1529 2024-04-25 07:56:54.012591 eotdl-2024.5.2/eotdl/curation/stac/parsers.py
+-rwxr-xr-x   0        0        0    13180 2024-04-25 07:56:54.012591 eotdl-2024.5.2/eotdl/curation/stac/stac.py
+-rwxr-xr-x   0        0        0      175 2024-05-02 13:36:26.868161 eotdl-2024.5.2/eotdl/datasets/__init__.py
+-rwxr-xr-x   0        0        0     3667 2024-04-25 10:24:33.763860 eotdl-2024.5.2/eotdl/datasets/download.py
+-rwxr-xr-x   0        0        0     5806 2024-04-25 10:24:33.763860 eotdl-2024.5.2/eotdl/datasets/ingest.py
+-rwxr-xr-x   0        0        0     1457 2024-04-25 07:56:54.012591 eotdl-2024.5.2/eotdl/datasets/metadata.py
+-rwxr-xr-x   0        0        0     1041 2024-04-25 07:56:54.012591 eotdl-2024.5.2/eotdl/datasets/retrieve.py
+-rw-r--r--   0        0        0      386 2024-04-25 07:56:54.012591 eotdl-2024.5.2/eotdl/datasets/update.py
+-rwxr-xr-x   0        0        0       87 2024-05-02 13:36:26.868161 eotdl-2024.5.2/eotdl/files/__init__.py
+-rwxr-xr-x   0        0        0     6185 2024-04-25 07:56:54.012591 eotdl-2024.5.2/eotdl/files/ingest.py
+-rw-r--r--   0        0        0      519 2024-05-02 13:36:26.868161 eotdl-2024.5.2/eotdl/files/list_files.py
+-rwxr-xr-x   0        0        0      146 2024-05-02 13:36:26.868161 eotdl-2024.5.2/eotdl/models/__init__.py
+-rwxr-xr-x   0        0        0     4119 2024-04-25 07:56:54.012591 eotdl-2024.5.2/eotdl/models/download.py
+-rwxr-xr-x   0        0        0     3381 2024-04-25 07:56:54.012591 eotdl-2024.5.2/eotdl/models/ingest.py
+-rwxr-xr-x   0        0        0     1443 2024-04-25 07:56:54.012591 eotdl-2024.5.2/eotdl/models/metadata.py
+-rwxr-xr-x   0        0        0      664 2024-04-25 07:56:54.012591 eotdl-2024.5.2/eotdl/models/retrieve.py
+-rw-r--r--   0        0        0      374 2024-04-25 07:56:54.012591 eotdl-2024.5.2/eotdl/models/update.py
+-rwxr-xr-x   0        0        0      791 2024-04-25 07:56:54.012591 eotdl-2024.5.2/eotdl/repos/APIRepo.py
+-rwxr-xr-x   0        0        0      957 2024-04-25 07:56:54.012591 eotdl-2024.5.2/eotdl/repos/AuthAPIRepo.py
+-rwxr-xr-x   0        0        0     1154 2024-04-25 07:56:54.012591 eotdl-2024.5.2/eotdl/repos/AuthRepo.py
+-rwxr-xr-x   0        0        0     2660 2024-04-25 07:56:54.012591 eotdl-2024.5.2/eotdl/repos/DatasetsAPIRepo.py
+-rwxr-xr-x   0        0        0     7171 2024-05-02 13:36:26.868161 eotdl-2024.5.2/eotdl/repos/FilesAPIRepo.py
+-rwxr-xr-x   0        0        0     1677 2024-04-25 07:56:54.012591 eotdl-2024.5.2/eotdl/repos/ModelsAPIRepo.py
+-rwxr-xr-x   0        0        0      222 2024-04-25 07:56:54.012591 eotdl-2024.5.2/eotdl/repos/__init__.py
+-rwxr-xr-x   0        0        0       41 2024-04-25 07:56:54.012591 eotdl-2024.5.2/eotdl/shared/__init__.py
+-rwxr-xr-x   0        0        0      479 2024-04-25 07:56:54.012591 eotdl-2024.5.2/eotdl/shared/checksum.py
+-rwxr-xr-x   0        0        0      178 2024-04-25 07:56:54.012591 eotdl-2024.5.2/eotdl/tools/__init__.py
+-rwxr-xr-x   0        0        0     7320 2024-04-25 07:56:54.012591 eotdl-2024.5.2/eotdl/tools/geo_utils.py
+-rwxr-xr-x   0        0        0     1664 2024-04-25 07:56:54.012591 eotdl-2024.5.2/eotdl/tools/metadata.py
+-rwxr-xr-x   0        0        0     1152 2024-04-25 07:56:54.012591 eotdl-2024.5.2/eotdl/tools/paths.py
+-rwxr-xr-x   0        0        0     5763 2024-04-25 07:56:54.012591 eotdl-2024.5.2/eotdl/tools/stac.py
+-rwxr-xr-x   0        0        0     4691 2024-04-25 07:56:54.012591 eotdl-2024.5.2/eotdl/tools/time_utils.py
+-rwxr-xr-x   0        0        0     6354 2024-04-25 07:56:54.012591 eotdl-2024.5.2/eotdl/tools/tools.py
+-rwxr-xr-x   0        0        0      944 2024-05-02 13:54:59.685018 eotdl-2024.5.2/pyproject.toml
+-rw-r--r--   0        0        0     4102 1970-01-01 00:00:00.000000 eotdl-2024.5.2/PKG-INFO
```

### Comparing `eotdl-2024.4.25/README.md` & `eotdl-2024.5.2/README.md`

 * *Files identical despite different names*

### Comparing `eotdl-2024.4.25/eotdl/access/airbus/client.py` & `eotdl-2024.5.2/eotdl/access/airbus/client.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.4.25/eotdl/access/airbus/parameters.py` & `eotdl-2024.5.2/eotdl/access/airbus/parameters.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.4.25/eotdl/access/airbus/utils.py` & `eotdl-2024.5.2/eotdl/access/airbus/utils.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.4.25/eotdl/access/download.py` & `eotdl-2024.5.2/eotdl/access/download.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Download imagery
 """
 
 from datetime import datetime
-from typing import Union, List
+from typing import Union, List, Optional
 
 from .sentinelhub import (
     SHClient,
     SH_PARAMETERS_DICT,
     evaluate_sentinel_parameters,
     imagery_from_tmp_to_dir,
 )
@@ -15,43 +15,49 @@
 
 
 def download_sentinel_imagery(
     output: str,
     time_interval: Union[str, datetime, List[Union[str, datetime]]],
     bounding_box: List[Union[int, float]],
     sensor: str,
+    name: Optional[str] = None,
 ) -> None:
     """
     Download Sentinel imagery
     """
     evaluate_sentinel_parameters(sensor, time_interval, bounding_box, output)
 
     client = SHClient()
     parameters = SH_PARAMETERS_DICT[sensor]()
 
-    request = client.request_data(time_interval, bounding_box, parameters)
-    client.download_data(request)
-    imagery_from_tmp_to_dir(output)
+    results = search_sentinel_imagery(time_interval, bounding_box, sensor)
+    timestamps = [date.strftime("%Y-%m-%d") for date in results.get_timestamps()]
+
+    requests_list = []
+    for date in timestamps:
+        requests_list.append(client.request_data(date, bounding_box, parameters))
+    if len(requests_list) == 0:
+        print(f"No images found for {sensor} in the specified time: {time_interval}")
+        return
+    elif len(requests_list) <= 2:
+        bulk = False
+    else:
+        bulk = True
+    client.download_data(requests_list)
+    imagery_from_tmp_to_dir(output, name=name, bulk=bulk)
 
 
 def search_and_download_sentinel_imagery(
     output: str,
     time_interval: Union[str, datetime, List[Union[str, datetime]]],
     bounding_box: List[Union[int, float]],
     sensor: str,
 ) -> None:
     """
     Search and download Sentinel imagery
     """
-    evaluate_sentinel_parameters(sensor, time_interval, bounding_box, output)
-
-    client = SHClient()
-    parameters = SH_PARAMETERS_DICT[sensor]()
-
-    results = search_sentinel_imagery(time_interval, bounding_box, sensor)
-    timestamps = [date.strftime("%Y-%m-%d") for date in results.get_timestamps()]
+    from warnings import warn
 
-    requests_list = []
-    for date in timestamps:
-        requests_list.append(client.request_data(date, bounding_box, parameters))
-    client.download_data(requests_list)
-    imagery_from_tmp_to_dir(output)
+    warn(
+        "The function `search_and_download_sentinel_imagery` has been deprecated and will be removed in future updates. Please use download_satellite_imagery instead."
+    )
+    download_sentinel_imagery(output, time_interval, bounding_box, sensor)
```

### Comparing `eotdl-2024.4.25/eotdl/access/search.py` & `eotdl-2024.5.2/eotdl/access/search.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.4.25/eotdl/access/sentinelhub/client.py` & `eotdl-2024.5.2/eotdl/access/sentinelhub/client.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.4.25/eotdl/access/sentinelhub/evalscripts.py` & `eotdl-2024.5.2/eotdl/access/sentinelhub/evalscripts.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.4.25/eotdl/access/sentinelhub/parameters.py` & `eotdl-2024.5.2/eotdl/access/sentinelhub/parameters.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.4.25/eotdl/access/sentinelhub/utils.py` & `eotdl-2024.5.2/eotdl/access/sentinelhub/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,32 +45,40 @@
         if not is_bounding_box(bounding_box):
             raise ValueError(
                 "Bounding box must be a list or tuple with four elements in format (lon_min, lat_min, lon_max, lat_max)."
             )
 
 
 def imagery_from_tmp_to_dir(
-    output_dir: str, tmp_dir: Optional[str] = "/tmp/sentinelhub"
+    output_dir: str,
+    tmp_dir: Optional[str] = "/tmp/sentinelhub",
+    name: Optional[str] = None,
+    bulk: Optional[bool] = False,
 ) -> None:
     """
     Copy imagery from tmp to output dir
     """
     downloaded_files = glob(f"{tmp_dir}/**/response.tiff")
     if len(downloaded_files) == 0:
         return
 
     makedirs(output_dir, exist_ok=True)
 
     for downloaded_file in downloaded_files:
         request_json = downloaded_file.replace("response.tiff", "request.json")
         metadata = generate_raster_metadata(downloaded_file, request_json)
-        if metadata["acquisition-date"]:
-            output_filename = f"{metadata['type']}_{metadata['acquisition-date']}"
+        if name and not bulk:
+            output_filename = name
+        elif name and bulk:
+            output_filename = f"{name}_{metadata['acquisition-date']}"
         else:
-            output_filename = metadata["type"]
+            if metadata["acquisition-date"]:
+                output_filename = f"{metadata['type']}_{metadata['acquisition-date']}"
+            else:
+                output_filename = metadata["type"]
 
         copyfile(downloaded_file, f"{output_dir}/{output_filename}.tif")
         with open(f"{output_dir}/{output_filename}.json", "w", encoding="utf-8") as f:
             json.dump(metadata, f)
 
     rmtree(tmp_dir)
```

### Comparing `eotdl-2024.4.25/eotdl/auth/auth.py` & `eotdl-2024.5.2/eotdl/auth/auth.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.4.25/eotdl/cli.py` & `eotdl-2024.5.2/eotdl/cli.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.4.25/eotdl/commands/auth.py` & `eotdl-2024.5.2/eotdl/commands/auth.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.4.25/eotdl/commands/datasets.py` & `eotdl-2024.5.2/eotdl/commands/datasets.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.4.25/eotdl/commands/models.py` & `eotdl-2024.5.2/eotdl/commands/models.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.4.25/eotdl/curation/stac/assets.py` & `eotdl-2024.5.2/eotdl/curation/stac/assets.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.4.25/eotdl/curation/stac/dataframe.py` & `eotdl-2024.5.2/eotdl/curation/stac/dataframe.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.4.25/eotdl/curation/stac/dataframe_bck.py` & `eotdl-2024.5.2/eotdl/curation/stac/dataframe_bck.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.4.25/eotdl/curation/stac/dataframe_labeling.py` & `eotdl-2024.5.2/eotdl/curation/stac/dataframe_labeling.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.4.25/eotdl/curation/stac/extensions/__init__.py` & `eotdl-2024.5.2/eotdl/curation/stac/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.4.25/eotdl/curation/stac/extensions/base.py` & `eotdl-2024.5.2/eotdl/curation/stac/extensions/base.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.4.25/eotdl/curation/stac/extensions/eo.py` & `eotdl-2024.5.2/eotdl/curation/stac/extensions/eo.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.4.25/eotdl/curation/stac/extensions/label/base.py` & `eotdl-2024.5.2/eotdl/curation/stac/extensions/label/base.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.4.25/eotdl/curation/stac/extensions/label/image_name_labeler.py` & `eotdl-2024.5.2/eotdl/curation/stac/extensions/label/image_name_labeler.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.4.25/eotdl/curation/stac/extensions/label/scaneo.py` & `eotdl-2024.5.2/eotdl/curation/stac/extensions/label/scaneo.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.4.25/eotdl/curation/stac/extensions/ml_dataset.py` & `eotdl-2024.5.2/eotdl/curation/stac/extensions/ml_dataset.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.4.25/eotdl/curation/stac/extensions/projection.py` & `eotdl-2024.5.2/eotdl/curation/stac/extensions/projection.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.4.25/eotdl/curation/stac/extensions/raster.py` & `eotdl-2024.5.2/eotdl/curation/stac/extensions/raster.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.4.25/eotdl/curation/stac/extensions/sar.py` & `eotdl-2024.5.2/eotdl/curation/stac/extensions/sar.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.4.25/eotdl/curation/stac/extent.py` & `eotdl-2024.5.2/eotdl/curation/stac/extent.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.4.25/eotdl/curation/stac/parsers.py` & `eotdl-2024.5.2/eotdl/curation/stac/parsers.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.4.25/eotdl/curation/stac/stac.py` & `eotdl-2024.5.2/eotdl/curation/stac/stac.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.4.25/eotdl/datasets/download.py` & `eotdl-2024.5.2/eotdl/datasets/download.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.4.25/eotdl/datasets/ingest.py` & `eotdl-2024.5.2/eotdl/datasets/ingest.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.4.25/eotdl/datasets/metadata.py` & `eotdl-2024.5.2/eotdl/datasets/metadata.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.4.25/eotdl/datasets/retrieve.py` & `eotdl-2024.5.2/eotdl/datasets/retrieve.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.4.25/eotdl/files/ingest.py` & `eotdl-2024.5.2/eotdl/files/ingest.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.4.25/eotdl/models/download.py` & `eotdl-2024.5.2/eotdl/models/download.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.4.25/eotdl/models/ingest.py` & `eotdl-2024.5.2/eotdl/models/ingest.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.4.25/eotdl/models/metadata.py` & `eotdl-2024.5.2/eotdl/models/metadata.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.4.25/eotdl/models/retrieve.py` & `eotdl-2024.5.2/eotdl/models/retrieve.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.4.25/eotdl/repos/APIRepo.py` & `eotdl-2024.5.2/eotdl/repos/APIRepo.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.4.25/eotdl/repos/AuthAPIRepo.py` & `eotdl-2024.5.2/eotdl/repos/AuthAPIRepo.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.4.25/eotdl/repos/AuthRepo.py` & `eotdl-2024.5.2/eotdl/repos/AuthRepo.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.4.25/eotdl/repos/DatasetsAPIRepo.py` & `eotdl-2024.5.2/eotdl/repos/DatasetsAPIRepo.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.4.25/eotdl/repos/FilesAPIRepo.py` & `eotdl-2024.5.2/eotdl/repos/FilesAPIRepo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import requests
 import os
 from tqdm import tqdm
 import hashlib
+from io import BytesIO
 
 from ..repos import APIRepo
 
 
 class FilesAPIRepo(APIRepo):
     def __init__(self, url=None):
         super().__init__(url)
@@ -185,7 +186,15 @@
 
     def complete_upload(self, user, upload_id, version, endpoint):
         r = requests.post(
             f"{self.url}{endpoint}/complete/{upload_id}?version={version}",
             headers=self.generate_headers(user),
         )
         return self.format_response(r)
+    
+    def get_file_stream(self, dataset_id, filename, user, version=None):
+        url = self.url + f"datasets/{dataset_id}/download/{filename}"
+        if version is not None:
+            url += "?version=" + str(version)
+        headers = self.generate_headers(user)
+        response = requests.get(url, headers=headers, stream=True)
+        return BytesIO(response.content)
```

### Comparing `eotdl-2024.4.25/eotdl/repos/ModelsAPIRepo.py` & `eotdl-2024.5.2/eotdl/repos/ModelsAPIRepo.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.4.25/eotdl/tools/geo_utils.py` & `eotdl-2024.5.2/eotdl/tools/geo_utils.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.4.25/eotdl/tools/metadata.py` & `eotdl-2024.5.2/eotdl/tools/metadata.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.4.25/eotdl/tools/paths.py` & `eotdl-2024.5.2/eotdl/tools/paths.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.4.25/eotdl/tools/stac.py` & `eotdl-2024.5.2/eotdl/tools/stac.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.4.25/eotdl/tools/time_utils.py` & `eotdl-2024.5.2/eotdl/tools/time_utils.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.4.25/eotdl/tools/tools.py` & `eotdl-2024.5.2/eotdl/tools/tools.py`

 * *Files identical despite different names*

### Comparing `eotdl-2024.4.25/pyproject.toml` & `eotdl-2024.5.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eotdl"
-version = "2024.04.25"
+version = "2024.05.02"
 description = "Earth Observation Training Data Lab"
 authors = ["EarthPulse <it@earthpulse.es>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "eotdl"}]
 
 [tool.poetry.scripts]
```

### Comparing `eotdl-2024.4.25/PKG-INFO` & `eotdl-2024.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: eotdl
-Version: 2024.4.25
+Version: 2024.5.2
 Summary: Earth Observation Training Data Lab
 License: MIT
 Author: EarthPulse
 Author-email: it@earthpulse.es
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: black (>=23.10.1,<24.0.0)
 Requires-Dist: geomet (>=1.0.0,<2.0.0)
 Requires-Dist: geopandas (>=0.13.2,<0.14.0)
 Requires-Dist: markdown (>=3.5.2,<4.0.0)
 Requires-Dist: markdownify (>=0.11.6,<0.12.0)
 Requires-Dist: mypy (>=1.6.1,<2.0.0)
 Requires-Dist: pydantic (>=1.10.6,<2.0.0)
```

#### html2text {}

```diff
@@ -1,23 +1,24 @@
-Metadata-Version: 2.1 Name: eotdl Version: 2024.4.25 Summary: Earth Observation
+Metadata-Version: 2.1 Name: eotdl Version: 2024.5.2 Summary: Earth Observation
 Training Data Lab License: MIT Author: EarthPulse Author-email:
 it@earthpulse.es Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Requires-Dist: black
-(>=23.10.1,<24.0.0) Requires-Dist: geomet (>=1.0.0,<2.0.0) Requires-Dist:
-geopandas (>=0.13.2,<0.14.0) Requires-Dist: markdown (>=3.5.2,<4.0.0) Requires-
-Dist: markdownify (>=0.11.6,<0.12.0) Requires-Dist: mypy (>=1.6.1,<2.0.0)
-Requires-Dist: pydantic (>=1.10.6,<2.0.0) Requires-Dist: pyjwt (>=2.6.0,<3.0.0)
-Requires-Dist: pystac[validation] (==1.8.2) Requires-Dist: python-frontmatter
-(>=1.1.0,<2.0.0) Requires-Dist: pyyaml (>=6.0.1,<7.0.0) Requires-Dist: rasterio
-(>=1.3.9,<2.0.0) Requires-Dist: requests (>=2.28.2,<3.0.0) Requires-Dist:
-sentinelhub (>=3.9.1,<4.0.0) Requires-Dist: tqdm (>=4.65.0,<5.0.0) Requires-
-Dist: typer[all] (>=0.9.0,<0.10.0) Description-Content-Type: text/markdown
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3.12 Requires-Dist: black (>=23.10.1,<24.0.0) Requires-
+Dist: geomet (>=1.0.0,<2.0.0) Requires-Dist: geopandas (>=0.13.2,<0.14.0)
+Requires-Dist: markdown (>=3.5.2,<4.0.0) Requires-Dist: markdownify
+(>=0.11.6,<0.12.0) Requires-Dist: mypy (>=1.6.1,<2.0.0) Requires-Dist: pydantic
+(>=1.10.6,<2.0.0) Requires-Dist: pyjwt (>=2.6.0,<3.0.0) Requires-Dist: pystac
+[validation] (==1.8.2) Requires-Dist: python-frontmatter (>=1.1.0,<2.0.0)
+Requires-Dist: pyyaml (>=6.0.1,<7.0.0) Requires-Dist: rasterio (>=1.3.9,<2.0.0)
+Requires-Dist: requests (>=2.28.2,<3.0.0) Requires-Dist: sentinelhub
+(>=3.9.1,<4.0.0) Requires-Dist: tqdm (>=4.65.0,<5.0.0) Requires-Dist: typer
+[all] (>=0.9.0,<0.10.0) Description-Content-Type: text/markdown
                                     _[_E_O_T_D_L_]
   Explore, download, create and share your own Training Datasets and Machine
                      Learning models for Earth Observation
                  _W_e_b_s_i_t_e Â· _D_o_c_u_m_e_n_t_a_t_i_o_n Â· _D_a_t_a_s_e_t_s Â· _B_l_o_g
                                  _[_N_P_M_ _V_e_r_s_i_o_n_]
 This is the main library and CLI for the **Earth Observation Training Data
 Lab** (EOTDL), a complete environment that allows you, among other things, to:
```

