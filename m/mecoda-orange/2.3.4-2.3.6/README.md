# Comparing `tmp/mecoda-orange-2.3.4.tar.gz` & `tmp/mecoda-orange-2.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mecoda-orange-2.3.4.tar", last modified: Mon Jan 22 11:03:10 2024, max compression
+gzip compressed data, was "mecoda-orange-2.3.6.tar", last modified: Thu May  2 15:34:52 2024, max compression
```

## Comparing `mecoda-orange-2.3.4.tar` & `mecoda-orange-2.3.6.tar`

### file list

```diff
@@ -1,85 +1,87 @@
-drwxr-xr-x   0 anomalia  (1000) anomalia  (1000)        0 2024-01-22 11:03:10.570943 mecoda-orange-2.3.4/
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)     3276 2024-01-22 11:03:10.570943 mecoda-orange-2.3.4/PKG-INFO
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)    16990 2024-01-03 11:30:01.000000 mecoda-orange-2.3.4/README.md
-drwxr-xr-x   0 anomalia  (1000) anomalia  (1000)        0 2024-01-22 11:03:10.566943 mecoda-orange-2.3.4/mecoda_orange/
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)      118 2022-12-22 11:43:28.000000 mecoda-orange-2.3.4/mecoda_orange/__init__.py
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)     9190 2024-01-22 09:26:55.000000 mecoda-orange-2.3.4/mecoda_orange/aire_ciudadano.py
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)     4831 2022-12-22 11:48:26.000000 mecoda-orange-2.3.4/mecoda_orange/canAIRio_fixed.py
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)     5149 2022-12-22 11:43:28.000000 mecoda-orange-2.3.4/mecoda_orange/canAIRio_fixed_extra_info.py
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)     3921 2022-12-22 11:48:26.000000 mecoda-orange-2.3.4/mecoda_orange/canAIRio_mobile.py
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)     3931 2022-12-22 11:43:28.000000 mecoda-orange-2.3.4/mecoda_orange/canAIRio_mobile_extra_info.py
-drwxr-xr-x   0 anomalia  (1000) anomalia  (1000)        0 2024-01-22 11:03:10.570943 mecoda-orange-2.3.4/mecoda_orange/icons/
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)     5308 2022-12-22 11:43:28.000000 mecoda-orange-2.3.4/mecoda_orange/icons/anchor-minka.png
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)     3788 2022-12-22 11:43:28.000000 mecoda-orange-2.3.4/mecoda_orange/icons/arrow-down-wide-short-solid-minka.png
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)    63603 2022-12-22 11:43:28.000000 mecoda-orange-2.3.4/mecoda_orange/icons/camera-minka.png
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)    62252 2022-12-22 11:43:28.000000 mecoda-orange-2.3.4/mecoda_orange/icons/camera-verde.png
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)   140085 2022-12-22 11:43:28.000000 mecoda-orange-2.3.4/mecoda_orange/icons/canairio_fixed_last_hour.png
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)    45017 2022-12-22 11:43:28.000000 mecoda-orange-2.3.4/mecoda_orange/icons/canairio_fixed_widget.png
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)    14592 2022-12-22 11:43:28.000000 mecoda-orange-2.3.4/mecoda_orange/icons/canairio_logo_gris.png
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)    14732 2022-12-22 11:43:28.000000 mecoda-orange-2.3.4/mecoda_orange/icons/canairio_logo_rosa.png
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)   206357 2022-12-22 11:43:28.000000 mecoda-orange-2.3.4/mecoda_orange/icons/canairio_mobile_total.png
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)   511527 2022-12-22 11:43:28.000000 mecoda-orange-2.3.4/mecoda_orange/icons/canairio_mobile_track.png
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)    24788 2022-12-22 11:43:28.000000 mecoda-orange-2.3.4/mecoda_orange/icons/canairio_mobile_widget.png
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)   141497 2022-12-22 11:43:28.000000 mecoda-orange-2.3.4/mecoda_orange/icons/canairio_workflow.png
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)     3973 2022-12-22 11:43:28.000000 mecoda-orange-2.3.4/mecoda_orange/icons/circle-info-solid-gris-oscuro.png
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)     3975 2022-12-22 11:43:28.000000 mecoda-orange-2.3.4/mecoda_orange/icons/circle-info-solid-gris.png
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)    12976 2022-12-22 11:43:28.000000 mecoda-orange-2.3.4/mecoda_orange/icons/circle-info-solid-minka.png
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)     3975 2022-12-22 11:43:28.000000 mecoda-orange-2.3.4/mecoda_orange/icons/circle-info-solid-rosa.png
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)     3969 2022-12-22 11:43:28.000000 mecoda-orange-2.3.4/mecoda_orange/icons/circle-info-solid-verde.png
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)    12025 2022-12-22 11:43:28.000000 mecoda-orange-2.3.4/mecoda_orange/icons/cos4cloud.png
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)    12025 2022-12-22 11:43:28.000000 mecoda-orange-2.3.4/mecoda_orange/icons/cos4cloud_color.png
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)    11936 2022-12-22 11:43:28.000000 mecoda-orange-2.3.4/mecoda_orange/icons/cos4cloud_v2.png
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)    10629 2022-12-22 11:43:28.000000 mecoda-orange-2.3.4/mecoda_orange/icons/filtrar.png
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)     4000 2022-12-22 11:43:28.000000 mecoda-orange-2.3.4/mecoda_orange/icons/fish-minka.png
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)     4272 2022-12-22 11:43:28.000000 mecoda-orange-2.3.4/mecoda_orange/icons/globe-minka.png
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)    22588 2022-12-22 11:43:28.000000 mecoda-orange-2.3.4/mecoda_orange/icons/ictio-circular.png
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)    21699 2022-12-22 11:43:28.000000 mecoda-orange-2.3.4/mecoda_orange/icons/ictio.png
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)    23513 2022-12-22 11:43:28.000000 mecoda-orange-2.3.4/mecoda_orange/icons/ictio_widget.png
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)    29338 2022-12-22 11:43:28.000000 mecoda-orange-2.3.4/mecoda_orange/icons/kduino.png
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)     4047 2022-12-22 11:43:28.000000 mecoda-orange-2.3.4/mecoda_orange/icons/leaf-solid-minka.png
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)    32797 2022-12-22 11:43:28.000000 mecoda-orange-2.3.4/mecoda_orange/icons/logo-aire-ciudadano.png
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)    12876 2022-12-22 11:43:28.000000 mecoda-orange-2.3.4/mecoda_orange/icons/logo-cos4cloud-middle.png
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)   292358 2022-12-22 11:43:28.000000 mecoda-orange-2.3.4/mecoda_orange/icons/map_filter_workflow.png
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)   107482 2022-12-22 11:43:28.000000 mecoda-orange-2.3.4/mecoda_orange/icons/map_filter_workflow2.png
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)    27586 2022-12-22 11:43:28.000000 mecoda-orange-2.3.4/mecoda_orange/icons/marine_filter_widget.png
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)     2497 2022-12-22 11:43:28.000000 mecoda-orange-2.3.4/mecoda_orange/icons/mecoda_share.png
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)    18983 2022-12-22 11:43:28.000000 mecoda-orange-2.3.4/mecoda_orange/icons/minka-logo.png
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)     4724 2023-10-30 12:22:52.000000 mecoda-orange-2.3.4/mecoda_orange/icons/minka-users.png
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)    36307 2022-12-22 11:43:28.000000 mecoda-orange-2.3.4/mecoda_orange/icons/minka-widget.png
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)    43844 2022-12-22 11:43:28.000000 mecoda-orange-2.3.4/mecoda_orange/icons/minka_taxon_filter_2.png
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)    31370 2022-12-22 11:43:28.000000 mecoda-orange-2.3.4/mecoda_orange/icons/minka_taxon_search_widget.png
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)    40361 2022-12-22 11:43:28.000000 mecoda-orange-2.3.4/mecoda_orange/icons/natusfera-widget-2.png
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)    40361 2022-12-22 11:43:28.000000 mecoda-orange-2.3.4/mecoda_orange/icons/natusfera-widget.png
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)    22976 2022-12-22 11:43:28.000000 mecoda-orange-2.3.4/mecoda_orange/icons/natusfera_v1.png
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)    50221 2022-12-22 11:43:28.000000 mecoda-orange-2.3.4/mecoda_orange/icons/odour-collect-widget-2.png
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)    47088 2022-12-22 11:43:28.000000 mecoda-orange-2.3.4/mecoda_orange/icons/odour-collect-widget.png
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)    11732 2022-12-22 11:43:28.000000 mecoda-orange-2.3.4/mecoda_orange/icons/odour_collect.png
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)     4754 2022-12-22 11:43:28.000000 mecoda-orange-2.3.4/mecoda_orange/icons/odourcollect-logo.png
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)    23329 2023-01-24 17:03:34.000000 mecoda-orange-2.3.4/mecoda_orange/icons/odourcollect-logo2.png
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)   194166 2023-10-18 14:05:47.000000 mecoda-orange-2.3.4/mecoda_orange/icons/plantnet.png
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)     3624 2022-12-22 11:43:28.000000 mecoda-orange-2.3.4/mecoda_orange/icons/seedling-solid-minka.png
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)    50866 2022-12-22 11:43:28.000000 mecoda-orange-2.3.4/mecoda_orange/icons/share.png
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)     9813 2022-12-22 11:43:28.000000 mecoda-orange-2.3.4/mecoda_orange/icons/share.svg
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)    22670 2022-12-22 11:43:28.000000 mecoda-orange-2.3.4/mecoda_orange/icons/smartcitizen.png
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)    10013 2022-12-22 11:43:28.000000 mecoda-orange-2.3.4/mecoda_orange/icons/smartcitizend.png
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)    10392 2022-12-22 11:43:28.000000 mecoda-orange-2.3.4/mecoda_orange/icons/taxon_tree.png
--rwxr-xr-x   0 anomalia  (1000) anomalia  (1000)    15659 2024-01-03 11:59:26.000000 mecoda-orange-2.3.4/mecoda_orange/minka.py
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)     2753 2022-12-22 11:43:28.000000 mecoda-orange-2.3.4/mecoda_orange/minka_get_images.py
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)     3462 2023-10-30 12:22:52.000000 mecoda-orange-2.3.4/mecoda_orange/minka_marine_filter.py
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)     1959 2023-11-05 15:47:03.000000 mecoda-orange-2.3.4/mecoda_orange/minka_mentions.py
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)    12259 2023-10-30 12:22:52.000000 mecoda-orange-2.3.4/mecoda_orange/minka_search_taxa.py
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)    11548 2022-12-22 11:43:28.000000 mecoda-orange-2.3.4/mecoda_orange/minka_taxa.py
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)    10142 2023-10-18 14:05:47.000000 mecoda-orange-2.3.4/mecoda_orange/odour_collect.py
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)     7591 2023-01-24 17:03:34.000000 mecoda-orange-2.3.4/mecoda_orange/odour_collect_events.py
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)     8176 2022-12-22 11:43:28.000000 mecoda-orange-2.3.4/mecoda_orange/smartcitizen_data.py
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)     7607 2022-12-22 11:43:28.000000 mecoda-orange-2.3.4/mecoda_orange/smartcitizen_search.py
-drwxr-xr-x   0 anomalia  (1000) anomalia  (1000)        0 2024-01-22 11:03:10.566943 mecoda-orange-2.3.4/mecoda_orange.egg-info/
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)     3276 2024-01-22 11:03:10.000000 mecoda-orange-2.3.4/mecoda_orange.egg-info/PKG-INFO
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)     3033 2024-01-22 11:03:10.000000 mecoda-orange-2.3.4/mecoda_orange.egg-info/SOURCES.txt
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)        1 2024-01-22 11:03:10.000000 mecoda-orange-2.3.4/mecoda_orange.egg-info/dependency_links.txt
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)       80 2024-01-22 11:03:10.000000 mecoda-orange-2.3.4/mecoda_orange.egg-info/entry_points.txt
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)        1 2024-01-22 11:03:05.000000 mecoda-orange-2.3.4/mecoda_orange.egg-info/not-zip-safe
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)      169 2024-01-22 11:03:10.000000 mecoda-orange-2.3.4/mecoda_orange.egg-info/requires.txt
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)       14 2024-01-22 11:03:10.000000 mecoda-orange-2.3.4/mecoda_orange.egg-info/top_level.txt
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)       38 2024-01-22 11:03:10.570943 mecoda-orange-2.3.4/setup.cfg
--rw-r--r--   0 anomalia  (1000) anomalia  (1000)     2279 2024-01-22 09:27:57.000000 mecoda-orange-2.3.4/setup.py
+drwxr-xr-x   0 anomalia  (1000) anomalia  (1000)        0 2024-05-02 15:34:52.965894 mecoda-orange-2.3.6/
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)     3638 2024-05-02 15:34:52.965894 mecoda-orange-2.3.6/PKG-INFO
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)    16996 2024-05-02 15:27:41.000000 mecoda-orange-2.3.6/README.md
+drwxr-xr-x   0 anomalia  (1000) anomalia  (1000)        0 2024-05-02 15:34:52.957894 mecoda-orange-2.3.6/mecoda_orange/
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)      118 2022-12-22 11:43:28.000000 mecoda-orange-2.3.6/mecoda_orange/__init__.py
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)     9190 2024-05-02 15:27:42.000000 mecoda-orange-2.3.6/mecoda_orange/aire_ciudadano.py
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)     4831 2024-05-02 15:27:42.000000 mecoda-orange-2.3.6/mecoda_orange/canAIRio_fixed.py
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)     5149 2022-12-22 11:43:28.000000 mecoda-orange-2.3.6/mecoda_orange/canAIRio_fixed_extra_info.py
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)     3921 2024-05-02 15:27:42.000000 mecoda-orange-2.3.6/mecoda_orange/canAIRio_mobile.py
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)     3931 2022-12-22 11:43:28.000000 mecoda-orange-2.3.6/mecoda_orange/canAIRio_mobile_extra_info.py
+drwxr-xr-x   0 anomalia  (1000) anomalia  (1000)        0 2024-05-02 15:34:52.965894 mecoda-orange-2.3.6/mecoda_orange/icons/
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)     5308 2022-12-22 11:43:28.000000 mecoda-orange-2.3.6/mecoda_orange/icons/anchor-minka.png
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)     3788 2022-12-22 11:43:28.000000 mecoda-orange-2.3.6/mecoda_orange/icons/arrow-down-wide-short-solid-minka.png
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)    63603 2022-12-22 11:43:28.000000 mecoda-orange-2.3.6/mecoda_orange/icons/camera-minka.png
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)    62252 2022-12-22 11:43:28.000000 mecoda-orange-2.3.6/mecoda_orange/icons/camera-verde.png
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)   140085 2022-12-22 11:43:28.000000 mecoda-orange-2.3.6/mecoda_orange/icons/canairio_fixed_last_hour.png
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)    45017 2022-12-22 11:43:28.000000 mecoda-orange-2.3.6/mecoda_orange/icons/canairio_fixed_widget.png
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)    14592 2022-12-22 11:43:28.000000 mecoda-orange-2.3.6/mecoda_orange/icons/canairio_logo_gris.png
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)    14732 2022-12-22 11:43:28.000000 mecoda-orange-2.3.6/mecoda_orange/icons/canairio_logo_rosa.png
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)   206357 2022-12-22 11:43:28.000000 mecoda-orange-2.3.6/mecoda_orange/icons/canairio_mobile_total.png
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)   511527 2022-12-22 11:43:28.000000 mecoda-orange-2.3.6/mecoda_orange/icons/canairio_mobile_track.png
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)    24788 2022-12-22 11:43:28.000000 mecoda-orange-2.3.6/mecoda_orange/icons/canairio_mobile_widget.png
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)   141497 2022-12-22 11:43:28.000000 mecoda-orange-2.3.6/mecoda_orange/icons/canairio_workflow.png
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)     3973 2022-12-22 11:43:28.000000 mecoda-orange-2.3.6/mecoda_orange/icons/circle-info-solid-gris-oscuro.png
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)     3975 2022-12-22 11:43:28.000000 mecoda-orange-2.3.6/mecoda_orange/icons/circle-info-solid-gris.png
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)    12976 2022-12-22 11:43:28.000000 mecoda-orange-2.3.6/mecoda_orange/icons/circle-info-solid-minka.png
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)     3975 2022-12-22 11:43:28.000000 mecoda-orange-2.3.6/mecoda_orange/icons/circle-info-solid-rosa.png
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)     3969 2022-12-22 11:43:28.000000 mecoda-orange-2.3.6/mecoda_orange/icons/circle-info-solid-verde.png
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)    12025 2022-12-22 11:43:28.000000 mecoda-orange-2.3.6/mecoda_orange/icons/cos4cloud.png
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)    12025 2022-12-22 11:43:28.000000 mecoda-orange-2.3.6/mecoda_orange/icons/cos4cloud_color.png
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)    11936 2022-12-22 11:43:28.000000 mecoda-orange-2.3.6/mecoda_orange/icons/cos4cloud_v2.png
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)    10629 2022-12-22 11:43:28.000000 mecoda-orange-2.3.6/mecoda_orange/icons/filtrar.png
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)     4000 2022-12-22 11:43:28.000000 mecoda-orange-2.3.6/mecoda_orange/icons/fish-minka.png
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)     4272 2022-12-22 11:43:28.000000 mecoda-orange-2.3.6/mecoda_orange/icons/globe-minka.png
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)    22588 2022-12-22 11:43:28.000000 mecoda-orange-2.3.6/mecoda_orange/icons/ictio-circular.png
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)    21699 2022-12-22 11:43:28.000000 mecoda-orange-2.3.6/mecoda_orange/icons/ictio.png
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)    23513 2022-12-22 11:43:28.000000 mecoda-orange-2.3.6/mecoda_orange/icons/ictio_widget.png
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)    29338 2022-12-22 11:43:28.000000 mecoda-orange-2.3.6/mecoda_orange/icons/kduino.png
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)     4047 2022-12-22 11:43:28.000000 mecoda-orange-2.3.6/mecoda_orange/icons/leaf-solid-minka.png
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)    32797 2024-05-02 15:27:42.000000 mecoda-orange-2.3.6/mecoda_orange/icons/logo-aire-ciudadano.png
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)    12876 2022-12-22 11:43:28.000000 mecoda-orange-2.3.6/mecoda_orange/icons/logo-cos4cloud-middle.png
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)   292358 2022-12-22 11:43:28.000000 mecoda-orange-2.3.6/mecoda_orange/icons/map_filter_workflow.png
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)   107482 2022-12-22 11:43:28.000000 mecoda-orange-2.3.6/mecoda_orange/icons/map_filter_workflow2.png
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)    27586 2022-12-22 11:43:28.000000 mecoda-orange-2.3.6/mecoda_orange/icons/marine_filter_widget.png
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)     2497 2022-12-22 11:43:28.000000 mecoda-orange-2.3.6/mecoda_orange/icons/mecoda_share.png
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)    18983 2022-12-22 11:43:28.000000 mecoda-orange-2.3.6/mecoda_orange/icons/minka-logo.png
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)     4724 2024-05-02 15:27:42.000000 mecoda-orange-2.3.6/mecoda_orange/icons/minka-users.png
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)    36307 2022-12-22 11:43:28.000000 mecoda-orange-2.3.6/mecoda_orange/icons/minka-widget.png
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)    43844 2022-12-22 11:43:28.000000 mecoda-orange-2.3.6/mecoda_orange/icons/minka_taxon_filter_2.png
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)    31370 2022-12-22 11:43:28.000000 mecoda-orange-2.3.6/mecoda_orange/icons/minka_taxon_search_widget.png
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)    40361 2022-12-22 11:43:28.000000 mecoda-orange-2.3.6/mecoda_orange/icons/natusfera-widget-2.png
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)    40361 2022-12-22 11:43:28.000000 mecoda-orange-2.3.6/mecoda_orange/icons/natusfera-widget.png
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)    22976 2022-12-22 11:43:28.000000 mecoda-orange-2.3.6/mecoda_orange/icons/natusfera_v1.png
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)    50221 2022-12-22 11:43:28.000000 mecoda-orange-2.3.6/mecoda_orange/icons/odour-collect-widget-2.png
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)    47088 2022-12-22 11:43:28.000000 mecoda-orange-2.3.6/mecoda_orange/icons/odour-collect-widget.png
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)    11732 2022-12-22 11:43:28.000000 mecoda-orange-2.3.6/mecoda_orange/icons/odour_collect.png
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)     4754 2022-12-22 11:43:28.000000 mecoda-orange-2.3.6/mecoda_orange/icons/odourcollect-logo.png
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)    23329 2024-05-02 15:27:42.000000 mecoda-orange-2.3.6/mecoda_orange/icons/odourcollect-logo2.png
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)   194166 2024-05-02 15:27:42.000000 mecoda-orange-2.3.6/mecoda_orange/icons/plantnet.png
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)     3624 2022-12-22 11:43:28.000000 mecoda-orange-2.3.6/mecoda_orange/icons/seedling-solid-minka.png
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)    50866 2022-12-22 11:43:28.000000 mecoda-orange-2.3.6/mecoda_orange/icons/share.png
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)     9813 2022-12-22 11:43:28.000000 mecoda-orange-2.3.6/mecoda_orange/icons/share.svg
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)    10013 2024-05-02 15:30:22.000000 mecoda-orange-2.3.6/mecoda_orange/icons/smartcitizen_data.png
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)    22670 2024-05-02 15:30:22.000000 mecoda-orange-2.3.6/mecoda_orange/icons/smartcitizen_search.png
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)    10392 2022-12-22 11:43:28.000000 mecoda-orange-2.3.6/mecoda_orange/icons/taxon_tree.png
+-rwxr-xr-x   0 anomalia  (1000) anomalia  (1000)    15659 2024-05-02 15:27:42.000000 mecoda-orange-2.3.6/mecoda_orange/minka.py
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)     2753 2022-12-22 11:43:28.000000 mecoda-orange-2.3.6/mecoda_orange/minka_get_images.py
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)     3462 2024-05-02 15:27:42.000000 mecoda-orange-2.3.6/mecoda_orange/minka_marine_filter.py
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)     1959 2024-05-02 15:27:42.000000 mecoda-orange-2.3.6/mecoda_orange/minka_mentions.py
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)    12259 2024-05-02 15:27:42.000000 mecoda-orange-2.3.6/mecoda_orange/minka_search_taxa.py
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)    11548 2022-12-22 11:43:28.000000 mecoda-orange-2.3.6/mecoda_orange/minka_taxa.py
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)    10142 2024-05-02 15:27:42.000000 mecoda-orange-2.3.6/mecoda_orange/odour_collect.py
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)     7591 2024-05-02 15:27:42.000000 mecoda-orange-2.3.6/mecoda_orange/odour_collect_events.py
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)     8474 2024-05-02 15:30:22.000000 mecoda-orange-2.3.6/mecoda_orange/smartcitizen_data.py
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)     9069 2024-05-02 15:30:22.000000 mecoda-orange-2.3.6/mecoda_orange/smartcitizen_search.py
+drwxr-xr-x   0 anomalia  (1000) anomalia  (1000)        0 2024-05-02 15:34:52.965894 mecoda-orange-2.3.6/mecoda_orange.egg-info/
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)     3638 2024-05-02 15:34:52.000000 mecoda-orange-2.3.6/mecoda_orange.egg-info/PKG-INFO
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)     3072 2024-05-02 15:34:52.000000 mecoda-orange-2.3.6/mecoda_orange.egg-info/SOURCES.txt
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)        1 2024-05-02 15:34:52.000000 mecoda-orange-2.3.6/mecoda_orange.egg-info/dependency_links.txt
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)       80 2024-05-02 15:34:52.000000 mecoda-orange-2.3.6/mecoda_orange.egg-info/entry_points.txt
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)        1 2024-05-02 15:34:26.000000 mecoda-orange-2.3.6/mecoda_orange.egg-info/not-zip-safe
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)      182 2024-05-02 15:34:52.000000 mecoda-orange-2.3.6/mecoda_orange.egg-info/requires.txt
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)       14 2024-05-02 15:34:52.000000 mecoda-orange-2.3.6/mecoda_orange.egg-info/top_level.txt
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)       38 2024-05-02 15:34:52.965894 mecoda-orange-2.3.6/setup.cfg
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)     2359 2024-05-02 15:32:00.000000 mecoda-orange-2.3.6/setup.py
+drwxr-xr-x   0 anomalia  (1000) anomalia  (1000)        0 2024-05-02 15:34:52.965894 mecoda-orange-2.3.6/tests/
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)     8620 2024-05-02 15:27:42.000000 mecoda-orange-2.3.6/tests/test_external_apis.py
```

### Comparing `mecoda-orange-2.3.4/PKG-INFO` & `mecoda-orange-2.3.6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mecoda-orange
-Version: 2.3.4
+Version: 2.3.6
 Summary: Orange Data Minining Add-on containing MECODA widgets to analyse data from citizen science observatories
 Home-page: https://github.com/eosc-cos4cloud/mecoda-orange
 Author: Ana Alvarez, ICM-CSIC
 Author-email: ana.alvarez@icm.csic.es
 License: BSD
 Keywords: orange3 add-on,orange,data mining
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
@@ -17,14 +17,26 @@
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Description-Content-Type: text/markdown
+Requires-Dist: mecoda-nat>=0.6.0
+Requires-Dist: pandas>=1.4.4
+Requires-Dist: Orange3>=3.31.1
+Requires-Dist: pyodcollect>=1.1.0
+Requires-Dist: mecoda-minka>=1.5.1
+Requires-Dist: smartcitizen-connector==1.0.4
+Requires-Dist: nest_asyncio
+Requires-Dist: pydantic>=2.4.2
+Requires-Dist: pytest
+Requires-Dist: tabulate
+Requires-Dist: PyQt5
+Requires-Dist: PyQtWebEngine
 
 # Mecoda-Orange
 Mecoda-Orange is an add-on developed on [Orange Data Mining Platform](https://orangedatamining.com/) to analyse data from science citizen observatories. 
 
 See [documentation](https://github.com/eosc-cos4cloud/mecoda-orange).
 
 [MECODA (ModulE for Citizen Observatory Data Analysis)](https://cos4cloud-eosc.eu/services/mecoda-data-analysis-package/) is a repository to facilitate analyzing and viewing all sorts of citizen science data. It allows users to make their own exploratory visual data analysis without the help of specialized analysts. It also enables observers to create their own reproducible visual dataflows and share and reuse them.
```

### Comparing `mecoda-orange-2.3.4/README.md` & `mecoda-orange-2.3.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # <img src="https://github.com/eosc-cos4cloud/mecoda-orange/blob/master/mecoda_orange/icons/share.png" alt="mecoda-logo" width="100"/> Mecoda-Orange 
 
 This repository includes different Orange Data Mining widgets to access data from [Minka](https://minka-sdg.org/), [Odour Collect](https://odourcollect.eu/), [canAIRio](https://canair.io/), [Ictio](https://ictio.org/), [Natusfera](https://natusfera.gbif.es/) or [Smart Citizen](https://smartcitizen.me).
 
-<img src="https://github.com/eosc-cos4cloud/mecoda-orange/blob/master/mecoda_orange/icons/cos4cloud.png" alt="cos4cloud-logo" width="75"/> MECODA is part of [Cos4Cloud](https://cos4cloud.eu/), a European Horizon 2020 project to boost citizen science technologies.
+<img src="https://github.com/eosc-cos4cloud/mecoda-orange/blob/master/mecoda_orange/icons/cos4cloud.png" alt="cos4cloud-logo" width="75"/> MECODA is part of [Cos4Cloud](https://cos4cloud-eosc.eu/)), a European Horizon 2020 project to boost citizen science technologies.
 
 To use MECODA package you need to install Orange Data Mining platform through https://orangedatamining.com/download
 
 Once Orange is installed, inside the Options menu, it's possible to get the package using the "Add-ons" category, clicking on "Add more" and searching by name "mecoda-orange". The last version of the package will be installed on the Orange platform.
 
 You can find also a ["Installation Guide"](https://github.com/eosc-cos4cloud/mecoda-orange/blob/master/docs/english/installation_guide.md), ["Orange Example of Use"](https://github.com/eosc-cos4cloud/mecoda-orange/blob/master/docs/english/orange_example_of_use.md) and ["MECODA example of use"]("https://github.com/eosc-cos4cloud/mecoda-orange/blob/master/docs/english/datathon_nov2023_eng.md").
```

### Comparing `mecoda-orange-2.3.4/mecoda_orange/aire_ciudadano.py` & `mecoda-orange-2.3.6/mecoda_orange/aire_ciudadano.py`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/canAIRio_fixed.py` & `mecoda-orange-2.3.6/mecoda_orange/canAIRio_fixed.py`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/canAIRio_fixed_extra_info.py` & `mecoda-orange-2.3.6/mecoda_orange/canAIRio_fixed_extra_info.py`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/canAIRio_mobile.py` & `mecoda-orange-2.3.6/mecoda_orange/canAIRio_mobile.py`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/canAIRio_mobile_extra_info.py` & `mecoda-orange-2.3.6/mecoda_orange/canAIRio_mobile_extra_info.py`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/icons/anchor-minka.png` & `mecoda-orange-2.3.6/mecoda_orange/icons/anchor-minka.png`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/icons/arrow-down-wide-short-solid-minka.png` & `mecoda-orange-2.3.6/mecoda_orange/icons/arrow-down-wide-short-solid-minka.png`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/icons/camera-minka.png` & `mecoda-orange-2.3.6/mecoda_orange/icons/camera-minka.png`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/icons/camera-verde.png` & `mecoda-orange-2.3.6/mecoda_orange/icons/camera-verde.png`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/icons/canairio_fixed_last_hour.png` & `mecoda-orange-2.3.6/mecoda_orange/icons/canairio_fixed_last_hour.png`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/icons/canairio_fixed_widget.png` & `mecoda-orange-2.3.6/mecoda_orange/icons/canairio_fixed_widget.png`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/icons/canairio_logo_gris.png` & `mecoda-orange-2.3.6/mecoda_orange/icons/canairio_logo_gris.png`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/icons/canairio_logo_rosa.png` & `mecoda-orange-2.3.6/mecoda_orange/icons/canairio_logo_rosa.png`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/icons/canairio_mobile_total.png` & `mecoda-orange-2.3.6/mecoda_orange/icons/canairio_mobile_total.png`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/icons/canairio_mobile_track.png` & `mecoda-orange-2.3.6/mecoda_orange/icons/canairio_mobile_track.png`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/icons/canairio_mobile_widget.png` & `mecoda-orange-2.3.6/mecoda_orange/icons/canairio_mobile_widget.png`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/icons/canairio_workflow.png` & `mecoda-orange-2.3.6/mecoda_orange/icons/canairio_workflow.png`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/icons/circle-info-solid-gris-oscuro.png` & `mecoda-orange-2.3.6/mecoda_orange/icons/circle-info-solid-gris-oscuro.png`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/icons/circle-info-solid-gris.png` & `mecoda-orange-2.3.6/mecoda_orange/icons/circle-info-solid-gris.png`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/icons/circle-info-solid-minka.png` & `mecoda-orange-2.3.6/mecoda_orange/icons/circle-info-solid-minka.png`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/icons/circle-info-solid-rosa.png` & `mecoda-orange-2.3.6/mecoda_orange/icons/circle-info-solid-rosa.png`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/icons/circle-info-solid-verde.png` & `mecoda-orange-2.3.6/mecoda_orange/icons/circle-info-solid-verde.png`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/icons/cos4cloud.png` & `mecoda-orange-2.3.6/mecoda_orange/icons/cos4cloud.png`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/icons/cos4cloud_color.png` & `mecoda-orange-2.3.6/mecoda_orange/icons/cos4cloud_color.png`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/icons/cos4cloud_v2.png` & `mecoda-orange-2.3.6/mecoda_orange/icons/cos4cloud_v2.png`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/icons/filtrar.png` & `mecoda-orange-2.3.6/mecoda_orange/icons/filtrar.png`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/icons/fish-minka.png` & `mecoda-orange-2.3.6/mecoda_orange/icons/fish-minka.png`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/icons/globe-minka.png` & `mecoda-orange-2.3.6/mecoda_orange/icons/globe-minka.png`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/icons/ictio-circular.png` & `mecoda-orange-2.3.6/mecoda_orange/icons/ictio-circular.png`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/icons/ictio.png` & `mecoda-orange-2.3.6/mecoda_orange/icons/ictio.png`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/icons/ictio_widget.png` & `mecoda-orange-2.3.6/mecoda_orange/icons/ictio_widget.png`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/icons/kduino.png` & `mecoda-orange-2.3.6/mecoda_orange/icons/kduino.png`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/icons/leaf-solid-minka.png` & `mecoda-orange-2.3.6/mecoda_orange/icons/leaf-solid-minka.png`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/icons/logo-aire-ciudadano.png` & `mecoda-orange-2.3.6/mecoda_orange/icons/logo-aire-ciudadano.png`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/icons/logo-cos4cloud-middle.png` & `mecoda-orange-2.3.6/mecoda_orange/icons/logo-cos4cloud-middle.png`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/icons/map_filter_workflow.png` & `mecoda-orange-2.3.6/mecoda_orange/icons/map_filter_workflow.png`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/icons/map_filter_workflow2.png` & `mecoda-orange-2.3.6/mecoda_orange/icons/map_filter_workflow2.png`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/icons/marine_filter_widget.png` & `mecoda-orange-2.3.6/mecoda_orange/icons/marine_filter_widget.png`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/icons/mecoda_share.png` & `mecoda-orange-2.3.6/mecoda_orange/icons/mecoda_share.png`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/icons/minka-logo.png` & `mecoda-orange-2.3.6/mecoda_orange/icons/minka-logo.png`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/icons/minka-users.png` & `mecoda-orange-2.3.6/mecoda_orange/icons/minka-users.png`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/icons/minka-widget.png` & `mecoda-orange-2.3.6/mecoda_orange/icons/minka-widget.png`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/icons/minka_taxon_filter_2.png` & `mecoda-orange-2.3.6/mecoda_orange/icons/minka_taxon_filter_2.png`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/icons/minka_taxon_search_widget.png` & `mecoda-orange-2.3.6/mecoda_orange/icons/minka_taxon_search_widget.png`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/icons/natusfera-widget-2.png` & `mecoda-orange-2.3.6/mecoda_orange/icons/natusfera-widget-2.png`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/icons/natusfera-widget.png` & `mecoda-orange-2.3.6/mecoda_orange/icons/natusfera-widget.png`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/icons/natusfera_v1.png` & `mecoda-orange-2.3.6/mecoda_orange/icons/natusfera_v1.png`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/icons/odour-collect-widget-2.png` & `mecoda-orange-2.3.6/mecoda_orange/icons/odour-collect-widget-2.png`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/icons/odour-collect-widget.png` & `mecoda-orange-2.3.6/mecoda_orange/icons/odour-collect-widget.png`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/icons/odour_collect.png` & `mecoda-orange-2.3.6/mecoda_orange/icons/odour_collect.png`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/icons/odourcollect-logo.png` & `mecoda-orange-2.3.6/mecoda_orange/icons/odourcollect-logo.png`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/icons/odourcollect-logo2.png` & `mecoda-orange-2.3.6/mecoda_orange/icons/odourcollect-logo2.png`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/icons/plantnet.png` & `mecoda-orange-2.3.6/mecoda_orange/icons/plantnet.png`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/icons/seedling-solid-minka.png` & `mecoda-orange-2.3.6/mecoda_orange/icons/seedling-solid-minka.png`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/icons/share.png` & `mecoda-orange-2.3.6/mecoda_orange/icons/share.png`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/icons/share.svg` & `mecoda-orange-2.3.6/mecoda_orange/icons/share.svg`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/icons/smartcitizen.png` & `mecoda-orange-2.3.6/mecoda_orange/icons/smartcitizen_search.png`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/icons/smartcitizend.png` & `mecoda-orange-2.3.6/mecoda_orange/icons/smartcitizen_data.png`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/icons/taxon_tree.png` & `mecoda-orange-2.3.6/mecoda_orange/icons/taxon_tree.png`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/minka.py` & `mecoda-orange-2.3.6/mecoda_orange/minka.py`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/minka_get_images.py` & `mecoda-orange-2.3.6/mecoda_orange/minka_get_images.py`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/minka_marine_filter.py` & `mecoda-orange-2.3.6/mecoda_orange/minka_marine_filter.py`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/minka_mentions.py` & `mecoda-orange-2.3.6/mecoda_orange/minka_mentions.py`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/minka_search_taxa.py` & `mecoda-orange-2.3.6/mecoda_orange/minka_search_taxa.py`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/minka_taxa.py` & `mecoda-orange-2.3.6/mecoda_orange/minka_taxa.py`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/odour_collect.py` & `mecoda-orange-2.3.6/mecoda_orange/odour_collect.py`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/odour_collect_events.py` & `mecoda-orange-2.3.6/mecoda_orange/odour_collect_events.py`

 * *Files identical despite different names*

### Comparing `mecoda-orange-2.3.4/mecoda_orange/smartcitizen_data.py` & `mecoda-orange-2.3.6/mecoda_orange/smartcitizen_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,42 +3,49 @@
 from orangewidget.settings import Setting
 from Orange.widgets.settings import DomainContextHandler, ContextSetting
 from orangewidget import gui
 from orangewidget.utils.widgetpreview import WidgetPreview
 import Orange.data
 from Orange.data.pandas_compat import table_from_frame, table_to_frame
 
-from smartcitizen_connector import ScApiDevice, rollup_table, localise_date
+from smartcitizen_connector import SCDevice
+from smartcitizen_connector.tools import freq_2_rollup_lut, localise_date
+import nest_asyncio
+import asyncio
+
+loop = asyncio.new_event_loop()
+nest_asyncio.apply(loop)
+asyncio.set_event_loop(loop)
 
 # Fixed stations
 class SmartcitizenDataWidget(OWBaseWidget):
 
     # Widget's name as displayed in the canvas
     name = "Smart Citizen Data"
 
     # Short widget description
     description = "Get data from environmental devices from the Smart Citizen API"
 
     # An icon resource file path for this widget
-    icon = "icons/smartcitizend.png"
+    icon = "icons/smartcitizen_data.png"
 
     # Priority in the section MECODA
     priority = 14
 
     # Basic (convenience) GUI definition:
     #   a simple 'single column' GUI layout
     want_main_area = False
 
     #   with a fixed non resizable geometry.
     resizing_enabled = True
 
     # Defining settings
     device = Setting("", schema_only=True)
     rollup_number = Setting("10", schema_only=True)
-    rollup_text = Setting("m", schema_only=True)
+    rollup_text = Setting("Min", schema_only=True)
     resample = Setting(True, schema_only=True)
     min_date_text = Setting("", schema_only=True)
     max_date_text = Setting("", schema_only=True)
 
     # Widget's outputs; here, a single output named "Observations", of type Table
     class Inputs:
         devices = Input("Devices", Orange.data.Table, auto_summary = False)
@@ -72,24 +79,26 @@
         )
 
         self.rollup_text_line = gui.comboBox(
             self.rollupBox,
             self,
             "rollup_text",
             label="Rollup units:",
-            items=tuple(rollup_table.keys()),
+            items=tuple([item[0] for item in freq_2_rollup_lut]),
             sendSelectedValue=True,
             emptyString=False,
             editable=False,
             contentsLength=None,
             searchable=True,
             orientation=1
         )
 
-        self.dateBox = gui.widgetBox(self.controlArea, "Filter by date (YYYY-MM-DD)")
+        self.dateBox = gui.widgetBox(self.controlArea,
+            "Filter by date (YYYY-MM-DD)"
+        )
 
         self.date_init_line = gui.lineEdit(
             self.dateBox,
             self,
             "min_date_text",
             label="Initial Date:",
             orientation=1,
@@ -212,27 +221,30 @@
                 return
 
             if self.rollup is None:
                 self.infoa.setText(f'Input a valid rollup.')
                 self.info.set_output_summary(self.info.NoOutput)
                 return
 
-            d = ScApiDevice(self.device)
-            timezone = d.get_device_timezone()
+            d = SCDevice(self.device)
+            timezone = d.timezone
             progress = gui.ProgressBar(self, 4)
             progress.advance()
 
-            data = d.get_device_data(
+            # loop = asyncio.get_event_loop()
+            loop.run_until_complete(d.get_data(
                         min_date = localise_date(self.min_date, timezone),
                         max_date = localise_date(self.max_date, timezone),
-                        rollup = self.rollup,
+                        frequency = self.rollup,
                         clean_na = None,
                         resample = self.resample
                     )
+                )
 
+            data = d.data
             progress.advance()
 
             if data is not None:
                 table = table_from_frame(data)
                 progress.advance()
                 self.Outputs.readings.send(table)
                 progress.advance()
```

### Comparing `mecoda-orange-2.3.4/mecoda_orange/smartcitizen_search.py` & `mecoda-orange-2.3.6/mecoda_orange/smartcitizen_search.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 from orangewidget.widget import OWBaseWidget, Output
 from orangewidget.settings import Setting
 from orangewidget import gui
 from orangewidget.utils.widgetpreview import WidgetPreview
 import Orange.data
 from Orange.data.pandas_compat import table_from_frame
 
-from smartcitizen_connector import ScApiDevice
+from smartcitizen_connector import SCDevice, search_by_query
+from smartcitizen_connector.tools import dict_unpack
 from pandas import DataFrame
 
+unhashable_columns = ['notify', 'data', 'owner', 'kit', 'location', 'hardware_info', 'postprocessing', 'device_token', 'hardware']
+
 # Fixed stations
 class SmartcitizenSearchWidget(OWBaseWidget):
 
     # Widget's name as displayed in the canvas
     name = "Smart Citizen Search"
 
     # Short widget description
     description = "Search environmental devices from the Smart Citizen API"
 
     # An icon resource file path for this widget
-    icon = "icons/smartcitizen.png"
+    icon = "icons/smartcitizen_search.png"
 
     # Priority in the section MECODA
     priority = 13
 
     # Basic (convenience) GUI definition:
     #   a simple 'single column' GUI layout
     want_main_area = False
@@ -31,19 +34,14 @@
     resizing_enabled = True
 
     # Defining settings
     city = Setting("", schema_only=True)
     user = Setting("", schema_only=True)
     tags = Setting("", schema_only=True)
     device_id = Setting("", schema_only=True)
-    kit_id = Setting("", schema_only=True)
-
-    blueprints = ScApiDevice.get_kits()
-    # descriptive_blueprints = ('',) + tuple(blueprints['item_descr'].values,)
-    descriptive_blueprints = blueprints = ('', ) + tuple(sorted("{0:0=2d}".format(kit.id) + ': ' + kit.name for kit in blueprints),)
 
     # Widget's outputs; here, a single output named "Observations", of type Table
     class Outputs:
         deviceTable = Output("Devices", Orange.data.Table, auto_summary=False)
 
     def __init__(self):
         # use the init method from the class OWBaseWidget
@@ -83,31 +81,14 @@
             "user",
             label="User name:",
             orientation=1,
             controlWidth=200,
             # callback=self.device_id_disable,
             )
 
-        self.kit_id_line = gui.comboBox(
-            self.searchBox,
-            self,
-            "kit_id",
-            box=None,
-            label="Kit ID:",
-            # labelWidth=None,
-            items=self.descriptive_blueprints,
-            # callback=self.kit_id_edit,
-            sendSelectedValue=True,
-            emptyString=False,
-            editable=False,
-            contentsLength=None,
-            searchable=True,
-            orientation=1,
-            )
-
         gui.separator(self.controlArea)
 
         self.deviceBox = gui.widgetBox(self.controlArea, "Or directly find device")
         self.device_id_line = gui.lineEdit(
             self.deviceBox,
             self,
             'device_id',
@@ -121,60 +102,67 @@
 
         # commit area
         self.commitBox = gui.widgetBox(self.controlArea, "", spacing=2)
         gui.button(self.commitBox, self, "Search devices", callback=self.commit)
 
     def device_id_edit(self):
         if self.device_id_line != "":
-            self.kit_id_line.setDisabled(True)
+            # self.kit_id_line.setDisabled(True)
             self.city_line.setDisabled(True)
             self.tags_line.setDisabled(True)
             self.user_line.setDisabled(True)
 
-            self.kit_id = ""
+            # self.kit_id = ""
             self.city = ""
             self.tags = ""
             self.user = ""
 
         else:
-            self.kit_id_line.setDisabled(False)
+            # self.kit_id_line.setDisabled(False)
             self.city_line.setDisabled(False)
             self.tags_line.setDisabled(False)
             self.user_line.setDisabled(False)
 
     def tags_edit(self):
         if "," in self.tags:
             t = self.tags.split(",")
             self.tags_tokenized = [x.strip() for x in t]
         else:
-            self.tags_tokenized = [self.tags]
+            if self.tags:
+                self.tags_tokenized = [self.tags]
+            else:
+                self.tags_tokenized = None
 
     def commit(self):
         progress = gui.ProgressBar(self, 3)
         progress.advance()
 
         if self.device_id != "":
 
-            if self.user != "" or self.kit_id != "" or self.city != "":
+            if self.user != "" or self.city != "":
                 self.infoa.setText(f'Ignoring search filters')
             self.infoa.setText(f'Collecting device...')
 
-            d = ScApiDevice.get_device_info(self.device_id)
+            d = SCDevice(self.device_id)
 
             if d is not None:
-                df = DataFrame(list(d.dict().items())).set_index(0).T.set_index('id')
-                df['kit_id'] = df['kit_id'].astype('int')
-                df['owner_id'] = df['owner_id'].astype('float')
-                df['latitude'] = df['latitude'].astype('float')
-                df['longitude'] = df['longitude'].astype('float')
+                df = DataFrame(list(d.json.model_dump().items())).set_index(0).T.set_index('id')
+
+                df['owner_id'] = df.loc[int(self.device_id), 'owner']['id']
+                df['owner_username'] = df.loc[int(self.device_id), 'owner']['username']
+                df['latitude'] = df.loc[int(self.device_id), 'location']['latitude']
+                df['longitude'] = df.loc[int(self.device_id), 'location']['longitude']
+                df['city'] = df.loc[int(self.device_id), 'location']['city']
+                df['country_code'] = df.loc[int(self.device_id), 'location']['country_code']
                 df['device_id'] = int(self.device_id)
 
                 df['system_tags'] = df['system_tags'].astype('str')
                 df['user_tags'] = df['user_tags'].astype('str')
 
+                df.drop(columns = unhashable_columns, errors='ignore', inplace=True)
                 table = table_from_frame(df)
 
                 progress.advance()
                 self.Outputs.deviceTable.send(table)
                 self.infoa.setText(f'Device {self.device_id} gathered')
                 self.info.set_output_summary(1)
 
@@ -182,49 +170,82 @@
                 self.infoa.setText(f'Device {self.device_id} not found. Check again')
                 self.info.set_output_summary(self.info.NoOutput)
 
         else:
 
             if self.user == "": owner_username = None
             else: owner_username = self.user
-            if self.kit_id == "": kit_id = None
-            else: kit_id = int(self.kit_id.split(':')[0])
             if self.city == "": city = None
             else: city = self.city
 
             self.infoa.setText(f'Looking for devices...')
             self.infoa.setText(f'')
 
-            devices = ScApiDevice.get_devices(
-                owner_username=owner_username,
-                kit_id = kit_id,
-                city = city,
-                tags = self.tags_tokenized,
-                full = True)
+            # Query list for different devices
+            query_list = []
+            if owner_username is not None:
+                query_list.append({
+                        'key': 'owner_username',
+                        'value': owner_username,
+                        'search_matcher': 'eq'
+                    })
+
+            if city is not None:
+                    query_list.append({
+                        'key': 'tags_name',
+                        'value': city,
+                        'search_matcher': 'in'
+                    })
+
+            if self.tags_tokenized is not None:
+                    query_list.append({
+                        'key': 'tags_name',
+                        'value': self.tags_tokenized,
+                        'search_matcher': 'in'
+                    } )
+
+            if len(query_list):
+                devices = search_by_query(
+                    endpoint= 'devices',
+                    search_items= query_list)
+            else:
+                self.infoa.setText(f'At least one field is required.')
+                self.info.set_output_summary(self.info.NoOutput)
+                progress.finish()
+                return
+
+            if devices is None:
+                self.infoa.setText(f'Nothing found.')
+                self.info.set_output_summary(self.info.NoOutput)
+                progress.finish()
+                return
 
-            if len(devices) > 0:
-                df = DataFrame([device.__dict__ for device in devices])
+            if len(devices):
+                devices['owner_id'] = devices.apply(dict_unpack, column='owner', key='id', axis=1)
+                devices['owner_username'] = devices.apply(dict_unpack, column='owner', key='username', axis=1)
+                devices['latitude'] = devices.apply(dict_unpack, column='location', key='latitude', axis=1)
+                devices['longitude'] = devices.apply(dict_unpack, column='location', key='longitude', axis=1)
+                devices['city'] = devices.apply(dict_unpack, column='location', key='city', axis=1)
+                devices['country_code'] = devices.apply(dict_unpack, column='location', key='country_code', axis=1)
 
-                df['system_tags'] = df['system_tags'].astype('str')
-                df['user_tags'] = df['user_tags'].astype('str')
+                devices['system_tags'] = devices['system_tags'].astype('str')
+                devices['user_tags'] = devices['user_tags'].astype('str')
 
-                table = table_from_frame(df)
+                devices.drop(columns = unhashable_columns, errors='ignore', inplace=True)
+
+                table = table_from_frame(devices)
                 progress.advance()
                 self.infoa.setText(f'{len(devices)} devices gathered')
                 self.info.set_output_summary(len(devices))
                 self.Outputs.deviceTable.send(table)
 
             else:
                 self.infoa.setText(f'Nothing found.')
                 self.info.set_output_summary(self.info.NoOutput)
-
-        # except ValueError:
-        #     self.infoa.setText(f'Nothing found.')
-
-        # except Exception as error:
-        #     self.infoa.setText(f'ERROR: \n{error}')
+                progress.finish()
+                return
 
         progress.finish()
 
 # For developer purpose, allow running the widget directly with python
 if __name__ == "__main__":
     WidgetPreview(SmartcitizenSearchWidget).run()
```

### Comparing `mecoda-orange-2.3.4/mecoda_orange.egg-info/PKG-INFO` & `mecoda-orange-2.3.6/mecoda_orange.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mecoda-orange
-Version: 2.3.4
+Version: 2.3.6
 Summary: Orange Data Minining Add-on containing MECODA widgets to analyse data from citizen science observatories
 Home-page: https://github.com/eosc-cos4cloud/mecoda-orange
 Author: Ana Alvarez, ICM-CSIC
 Author-email: ana.alvarez@icm.csic.es
 License: BSD
 Keywords: orange3 add-on,orange,data mining
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
@@ -17,14 +17,26 @@
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Description-Content-Type: text/markdown
+Requires-Dist: mecoda-nat>=0.6.0
+Requires-Dist: pandas>=1.4.4
+Requires-Dist: Orange3>=3.31.1
+Requires-Dist: pyodcollect>=1.1.0
+Requires-Dist: mecoda-minka>=1.5.1
+Requires-Dist: smartcitizen-connector==1.0.4
+Requires-Dist: nest_asyncio
+Requires-Dist: pydantic>=2.4.2
+Requires-Dist: pytest
+Requires-Dist: tabulate
+Requires-Dist: PyQt5
+Requires-Dist: PyQtWebEngine
 
 # Mecoda-Orange
 Mecoda-Orange is an add-on developed on [Orange Data Mining Platform](https://orangedatamining.com/) to analyse data from science citizen observatories. 
 
 See [documentation](https://github.com/eosc-cos4cloud/mecoda-orange).
 
 [MECODA (ModulE for Citizen Observatory Data Analysis)](https://cos4cloud-eosc.eu/services/mecoda-data-analysis-package/) is a repository to facilitate analyzing and viewing all sorts of citizen science data. It allows users to make their own exploratory visual data analysis without the help of specialized analysts. It also enables observers to create their own reproducible visual dataflows and share and reuse them.
```

### Comparing `mecoda-orange-2.3.4/mecoda_orange.egg-info/SOURCES.txt` & `mecoda-orange-2.3.6/mecoda_orange.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -70,10 +70,11 @@
 mecoda_orange/icons/odour_collect.png
 mecoda_orange/icons/odourcollect-logo.png
 mecoda_orange/icons/odourcollect-logo2.png
 mecoda_orange/icons/plantnet.png
 mecoda_orange/icons/seedling-solid-minka.png
 mecoda_orange/icons/share.png
 mecoda_orange/icons/share.svg
-mecoda_orange/icons/smartcitizen.png
-mecoda_orange/icons/smartcitizend.png
-mecoda_orange/icons/taxon_tree.png
+mecoda_orange/icons/smartcitizen_data.png
+mecoda_orange/icons/smartcitizen_search.png
+mecoda_orange/icons/taxon_tree.png
+tests/test_external_apis.py
```

### Comparing `mecoda-orange-2.3.4/setup.py` & `mecoda-orange-2.3.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 # incluir documentación de https://github.com/biolab/orange3-example-addon/blob/master/setup.py
 
 NAME = "Orange3-MECODA"
 DOCUMENTATION_NAME = "Orange MECODA"
 
-VERSION = "2.3.4"
+VERSION = "2.3.6"
 
 AUTHOR = "Ana Alvarez, ICM-CSIC"
 AUTHOR_EMAIL = "ana.alvarez@icm.csic.es"
 
 URL = "https://github.com/eosc-cos4cloud/mecoda-orange"
 
 DESCRIPTION = "Orange Data Minining Add-on containing MECODA widgets to analyse data from citizen science observatories"
@@ -58,16 +58,17 @@
         "orange.addons": "MECODA = mecoda_orange",
     },
     install_requires=[
         "mecoda-nat >= 0.6.0",
         "pandas >= 1.4.4",
         "Orange3 >= 3.31.1",
         "pyodcollect >= 1.1.0",
-        "mecoda-minka >= 1.3.1",
-        "smartcitizen-connector == 0.2.0",
+        "mecoda-minka >= 1.5.1",
+        "smartcitizen-connector == 1.0.4",  # Smart Citizen connector should be fixed at a version
+        "nest_asyncio",
         "pydantic >= 2.4.2",
         "pytest",
         "tabulate",
         "PyQt5",
         "PyQtWebEngine",
     ],
     keywords=KEYWORDS,
```

