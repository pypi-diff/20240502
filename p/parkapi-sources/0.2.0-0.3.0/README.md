# Comparing `tmp/parkapi_sources-0.2.0.tar.gz` & `tmp/parkapi_sources-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parkapi_sources-0.2.0.tar", last modified: Thu Apr 18 18:44:35 2024, max compression
+gzip compressed data, was "parkapi_sources-0.3.0.tar", last modified: Thu May  2 13:18:48 2024, max compression
```

## Comparing `parkapi_sources-0.2.0.tar` & `parkapi_sources-0.3.0.tar`

### file list

```diff
@@ -1,209 +1,236 @@
-drwxrwxr-x   0 ernesto-ruge  (1000) ernesto-ruge  (1000)        0 2024-04-18 18:44:35.609994 parkapi_sources-0.2.0/
-drwxrwxr-x   0 ernesto-ruge  (1000) ernesto-ruge  (1000)        0 2024-04-18 18:44:35.561994 parkapi_sources-0.2.0/.github/
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)      283 2023-10-05 11:46:16.000000 parkapi_sources-0.2.0/.github/dependabot.yml
-drwxrwxr-x   0 ernesto-ruge  (1000) ernesto-ruge  (1000)        0 2024-04-18 18:44:35.561994 parkapi_sources-0.2.0/.github/workflows/
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     2297 2024-04-18 18:40:04.000000 parkapi_sources-0.2.0/.github/workflows/build-publish.yml
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     1116 2024-04-06 12:51:03.000000 parkapi_sources-0.2.0/.github/workflows/lint.yml
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)      167 2024-04-06 12:51:03.000000 parkapi_sources-0.2.0/.gitignore
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     1079 2024-04-06 12:51:03.000000 parkapi_sources-0.2.0/LICENCE.txt
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)      381 2024-04-06 12:51:03.000000 parkapi_sources-0.2.0/Makefile
--rw-r--r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)    13292 2024-04-18 18:44:35.609994 parkapi_sources-0.2.0/PKG-INFO
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)    11759 2024-04-17 11:50:30.000000 parkapi_sources-0.2.0/README.md
-drwxrwxr-x   0 ernesto-ruge  (1000) ernesto-ruge  (1000)        0 2024-04-18 18:44:35.561994 parkapi_sources-0.2.0/data/
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)    11453 2024-02-22 21:14:08.000000 parkapi_sources-0.2.0/data/freiburg.geojson
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)    11994 2024-02-18 18:32:29.000000 parkapi_sources-0.2.0/data/heidelberg.geojson
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)    10851 2024-02-18 12:45:48.000000 parkapi_sources-0.2.0/data/mannheim.geojson
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     5300 2024-02-18 12:13:28.000000 parkapi_sources-0.2.0/data/ulm.geojson
-drwxrwxr-x   0 ernesto-ruge  (1000) ernesto-ruge  (1000)        0 2024-04-18 18:44:35.561994 parkapi_sources-0.2.0/dev/
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)      369 2024-03-03 08:55:46.000000 parkapi_sources-0.2.0/dev/parkapi.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     3147 2024-03-10 13:09:04.000000 parkapi_sources-0.2.0/dev/test-pull-converter.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     4282 2024-03-10 13:09:12.000000 parkapi_sources-0.2.0/dev/test-push-converter.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     3279 2024-04-18 18:39:03.000000 parkapi_sources-0.2.0/pyproject.toml
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)       92 2024-04-06 12:51:03.000000 parkapi_sources-0.2.0/requirements-dev.txt
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)      103 2024-04-06 12:51:03.000000 parkapi_sources-0.2.0/requirements.txt
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)       38 2024-04-18 18:44:35.613994 parkapi_sources-0.2.0/setup.cfg
-drwxrwxr-x   0 ernesto-ruge  (1000) ernesto-ruge  (1000)        0 2024-04-18 18:44:35.557994 parkapi_sources-0.2.0/src/
-drwxrwxr-x   0 ernesto-ruge  (1000) ernesto-ruge  (1000)        0 2024-04-18 18:44:35.561994 parkapi_sources-0.2.0/src/parkapi_sources/
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)      188 2024-02-22 16:56:21.000000 parkapi_sources-0.2.0/src/parkapi_sources/__init__.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)      411 2024-04-18 18:44:35.000000 parkapi_sources-0.2.0/src/parkapi_sources/_version.py
-drwxrwxr-x   0 ernesto-ruge  (1000) ernesto-ruge  (1000)        0 2024-04-18 18:44:35.561994 parkapi_sources-0.2.0/src/parkapi_sources/converters/
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)      850 2024-04-18 18:25:23.000000 parkapi_sources-0.2.0/src/parkapi_sources/converters/__init__.py
-drwxrwxr-x   0 ernesto-ruge  (1000) ernesto-ruge  (1000)        0 2024-04-18 18:44:35.565994 parkapi_sources-0.2.0/src/parkapi_sources/converters/bahn_v2/
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)      187 2024-01-23 12:08:24.000000 parkapi_sources-0.2.0/src/parkapi_sources/converters/bahn_v2/__init__.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     3117 2024-03-13 09:18:11.000000 parkapi_sources-0.2.0/src/parkapi_sources/converters/bahn_v2/converter.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     1823 2024-02-24 10:13:25.000000 parkapi_sources-0.2.0/src/parkapi_sources/converters/bahn_v2/mapper.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     3885 2024-03-10 14:01:49.000000 parkapi_sources-0.2.0/src/parkapi_sources/converters/bahn_v2/validators.py
-drwxrwxr-x   0 ernesto-ruge  (1000) ernesto-ruge  (1000)        0 2024-04-18 18:44:35.565994 parkapi_sources-0.2.0/src/parkapi_sources/converters/base_converter/
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)      186 2024-02-18 08:16:51.000000 parkapi_sources-0.2.0/src/parkapi_sources/converters/base_converter/__init__.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)      829 2024-02-24 10:13:25.000000 parkapi_sources-0.2.0/src/parkapi_sources/converters/base_converter/base_converter.py
-drwxrwxr-x   0 ernesto-ruge  (1000) ernesto-ruge  (1000)        0 2024-04-18 18:44:35.565994 parkapi_sources-0.2.0/src/parkapi_sources/converters/base_converter/pull/
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)      340 2024-02-24 10:13:25.000000 parkapi_sources-0.2.0/src/parkapi_sources/converters/base_converter/pull/__init__.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)      729 2024-02-22 17:53:59.000000 parkapi_sources-0.2.0/src/parkapi_sources/converters/base_converter/pull/pull_converter.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     2809 2024-02-24 10:18:03.000000 parkapi_sources-0.2.0/src/parkapi_sources/converters/base_converter/pull/pull_scraper_mixin.py
-drwxrwxr-x   0 ernesto-ruge  (1000) ernesto-ruge  (1000)        0 2024-04-18 18:44:35.565994 parkapi_sources-0.2.0/src/parkapi_sources/converters/base_converter/pull/static_geojson_data_mixin/
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)      248 2024-02-24 10:13:25.000000 parkapi_sources-0.2.0/src/parkapi_sources/converters/base_converter/pull/static_geojson_data_mixin/__init__.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     3302 2024-02-24 10:18:03.000000 parkapi_sources-0.2.0/src/parkapi_sources/converters/base_converter/pull/static_geojson_data_mixin/mixin.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     2207 2024-03-10 14:01:49.000000 parkapi_sources-0.2.0/src/parkapi_sources/converters/base_converter/pull/static_geojson_data_mixin/models.py
-drwxrwxr-x   0 ernesto-ruge  (1000) ernesto-ruge  (1000)        0 2024-04-18 18:44:35.569994 parkapi_sources-0.2.0/src/parkapi_sources/converters/base_converter/push/
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)      428 2024-03-03 09:26:43.000000 parkapi_sources-0.2.0/src/parkapi_sources/converters/base_converter/push/__init__.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     1478 2024-03-03 09:23:45.000000 parkapi_sources-0.2.0/src/parkapi_sources/converters/base_converter/push/csv_converter.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)      649 2024-03-03 09:24:01.000000 parkapi_sources-0.2.0/src/parkapi_sources/converters/base_converter/push/json_converter.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     4937 2024-03-03 09:26:51.000000 parkapi_sources-0.2.0/src/parkapi_sources/converters/base_converter/push/normalized_xlsx_converter.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)      270 2024-03-03 09:23:17.000000 parkapi_sources-0.2.0/src/parkapi_sources/converters/base_converter/push/push_converter.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     1659 2024-03-03 09:26:51.000000 parkapi_sources-0.2.0/src/parkapi_sources/converters/base_converter/push/xlsx_converter.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)      725 2024-03-03 09:24:24.000000 parkapi_sources-0.2.0/src/parkapi_sources/converters/base_converter/push/xml_converter.py
-drwxrwxr-x   0 ernesto-ruge  (1000) ernesto-ruge  (1000)        0 2024-04-18 18:44:35.569994 parkapi_sources-0.2.0/src/parkapi_sources/converters/bfrk_bw/
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)      313 2024-04-06 12:51:03.000000 parkapi_sources-0.2.0/src/parkapi_sources/converters/bfrk_bw/__init__.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     2061 2024-04-06 12:51:03.000000 parkapi_sources-0.2.0/src/parkapi_sources/converters/bfrk_bw/base_converter.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     2026 2024-04-06 12:51:03.000000 parkapi_sources-0.2.0/src/parkapi_sources/converters/bfrk_bw/base_models.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     1644 2024-04-06 12:51:03.000000 parkapi_sources-0.2.0/src/parkapi_sources/converters/bfrk_bw/bike_converter.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     2039 2024-04-07 08:08:33.000000 parkapi_sources-0.2.0/src/parkapi_sources/converters/bfrk_bw/bike_models.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     1628 2024-04-06 12:51:03.000000 parkapi_sources-0.2.0/src/parkapi_sources/converters/bfrk_bw/car_converter.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     1763 2024-04-06 12:51:03.000000 parkapi_sources-0.2.0/src/parkapi_sources/converters/bfrk_bw/car_models.py
-drwxrwxr-x   0 ernesto-ruge  (1000) ernesto-ruge  (1000)        0 2024-04-18 18:44:35.569994 parkapi_sources-0.2.0/src/parkapi_sources/converters/freiburg/
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)      189 2024-02-20 06:26:13.000000 parkapi_sources-0.2.0/src/parkapi_sources/converters/freiburg/__init__.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     3061 2024-04-06 12:51:03.000000 parkapi_sources-0.2.0/src/parkapi_sources/converters/freiburg/converter.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     1688 2024-03-12 18:24:31.000000 parkapi_sources-0.2.0/src/parkapi_sources/converters/freiburg/models.py
-drwxrwxr-x   0 ernesto-ruge  (1000) ernesto-ruge  (1000)        0 2024-04-18 18:44:35.569994 parkapi_sources-0.2.0/src/parkapi_sources/converters/heidelberg/
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)      191 2024-02-18 18:24:58.000000 parkapi_sources-0.2.0/src/parkapi_sources/converters/heidelberg/__init__.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     3399 2024-04-06 12:51:03.000000 parkapi_sources-0.2.0/src/parkapi_sources/converters/heidelberg/converter.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     1970 2024-03-10 14:02:52.000000 parkapi_sources-0.2.0/src/parkapi_sources/converters/heidelberg/validators.py
-drwxrwxr-x   0 ernesto-ruge  (1000) ernesto-ruge  (1000)        0 2024-04-18 18:44:35.569994 parkapi_sources-0.2.0/src/parkapi_sources/converters/karlsruhe/
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)      190 2024-02-23 19:57:04.000000 parkapi_sources-0.2.0/src/parkapi_sources/converters/karlsruhe/__init__.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     4312 2024-04-06 12:51:03.000000 parkapi_sources-0.2.0/src/parkapi_sources/converters/karlsruhe/converter.py
-drwxrwxr-x   0 ernesto-ruge  (1000) ernesto-ruge  (1000)        0 2024-04-18 18:44:35.573994 parkapi_sources-0.2.0/src/parkapi_sources/converters/karlsruhe/files/
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     2933 2024-02-24 07:37:42.000000 parkapi_sources-0.2.0/src/parkapi_sources/converters/karlsruhe/files/ca.crt.pem
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     4253 2024-03-11 20:05:21.000000 parkapi_sources-0.2.0/src/parkapi_sources/converters/karlsruhe/models.py
-drwxrwxr-x   0 ernesto-ruge  (1000) ernesto-ruge  (1000)        0 2024-04-18 18:44:35.573994 parkapi_sources-0.2.0/src/parkapi_sources/converters/mannheim/
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)      189 2024-03-13 10:23:57.000000 parkapi_sources-0.2.0/src/parkapi_sources/converters/mannheim/__init__.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     2512 2024-04-06 12:51:03.000000 parkapi_sources-0.2.0/src/parkapi_sources/converters/mannheim/converter.py
-drwxrwxr-x   0 ernesto-ruge  (1000) ernesto-ruge  (1000)        0 2024-04-18 18:44:35.573994 parkapi_sources-0.2.0/src/parkapi_sources/converters/neckarsulm/
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)      191 2024-02-22 20:49:31.000000 parkapi_sources-0.2.0/src/parkapi_sources/converters/neckarsulm/__init__.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     2698 2024-03-13 09:19:34.000000 parkapi_sources-0.2.0/src/parkapi_sources/converters/neckarsulm/converter.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     3263 2024-03-10 14:01:49.000000 parkapi_sources-0.2.0/src/parkapi_sources/converters/neckarsulm/models.py
-drwxrwxr-x   0 ernesto-ruge  (1000) ernesto-ruge  (1000)        0 2024-04-18 18:44:35.573994 parkapi_sources-0.2.0/src/parkapi_sources/converters/pbw/
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)      184 2024-01-11 19:30:18.000000 parkapi_sources-0.2.0/src/parkapi_sources/converters/pbw/__init__.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     4889 2024-04-06 12:51:03.000000 parkapi_sources-0.2.0/src/parkapi_sources/converters/pbw/converter.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     2554 2024-02-24 10:13:25.000000 parkapi_sources-0.2.0/src/parkapi_sources/converters/pbw/mapper.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)    11699 2024-03-10 14:01:49.000000 parkapi_sources-0.2.0/src/parkapi_sources/converters/pbw/validation.py
-drwxrwxr-x   0 ernesto-ruge  (1000) ernesto-ruge  (1000)        0 2024-04-18 18:44:35.573994 parkapi_sources-0.2.0/src/parkapi_sources/converters/pforzheim/
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)      190 2024-04-06 12:51:03.000000 parkapi_sources-0.2.0/src/parkapi_sources/converters/pforzheim/__init__.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     2669 2024-04-06 12:51:03.000000 parkapi_sources-0.2.0/src/parkapi_sources/converters/pforzheim/converter.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     1836 2024-04-06 12:51:03.000000 parkapi_sources-0.2.0/src/parkapi_sources/converters/pforzheim/validation.py
-drwxrwxr-x   0 ernesto-ruge  (1000) ernesto-ruge  (1000)        0 2024-04-18 18:44:35.573994 parkapi_sources-0.2.0/src/parkapi_sources/converters/reutlingen/
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)      191 2024-04-06 12:51:03.000000 parkapi_sources-0.2.0/src/parkapi_sources/converters/reutlingen/__init__.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     2975 2024-04-06 12:51:03.000000 parkapi_sources-0.2.0/src/parkapi_sources/converters/reutlingen/converter.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     1903 2024-04-06 12:51:03.000000 parkapi_sources-0.2.0/src/parkapi_sources/converters/reutlingen/validation.py
-drwxrwxr-x   0 ernesto-ruge  (1000) ernesto-ruge  (1000)        0 2024-04-18 18:44:35.573994 parkapi_sources-0.2.0/src/parkapi_sources/converters/stuttgart/
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)      190 2024-02-22 20:49:25.000000 parkapi_sources-0.2.0/src/parkapi_sources/converters/stuttgart/__init__.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     6424 2024-04-06 12:51:03.000000 parkapi_sources-0.2.0/src/parkapi_sources/converters/stuttgart/converter.py
-drwxrwxr-x   0 ernesto-ruge  (1000) ernesto-ruge  (1000)        0 2024-04-18 18:44:35.573994 parkapi_sources-0.2.0/src/parkapi_sources/converters/ulm/
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)      184 2024-02-18 09:36:16.000000 parkapi_sources-0.2.0/src/parkapi_sources/converters/ulm/__init__.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     2316 2024-04-06 12:51:03.000000 parkapi_sources-0.2.0/src/parkapi_sources/converters/ulm/converter.py
-drwxrwxr-x   0 ernesto-ruge  (1000) ernesto-ruge  (1000)        0 2024-04-18 18:44:35.573994 parkapi_sources-0.2.0/src/parkapi_sources/converters/vrs_p_r/
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)      193 2024-02-20 06:27:14.000000 parkapi_sources-0.2.0/src/parkapi_sources/converters/vrs_p_r/__init__.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     2276 2024-03-13 09:19:56.000000 parkapi_sources-0.2.0/src/parkapi_sources/converters/vrs_p_r/vrs_p_r.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     1288 2024-02-22 17:14:04.000000 parkapi_sources-0.2.0/src/parkapi_sources/exceptions.py
-drwxrwxr-x   0 ernesto-ruge  (1000) ernesto-ruge  (1000)        0 2024-04-18 18:44:35.577994 parkapi_sources-0.2.0/src/parkapi_sources/models/
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)      338 2024-02-24 07:50:48.000000 parkapi_sources-0.2.0/src/parkapi_sources/models/__init__.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     1176 2024-03-12 08:54:31.000000 parkapi_sources-0.2.0/src/parkapi_sources/models/enums.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     7197 2024-04-06 12:51:03.000000 parkapi_sources-0.2.0/src/parkapi_sources/models/parking_site_inputs.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)      661 2024-03-13 09:17:44.000000 parkapi_sources-0.2.0/src/parkapi_sources/models/source_info.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     4413 2024-02-27 09:38:16.000000 parkapi_sources-0.2.0/src/parkapi_sources/models/xlsx_inputs.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     3088 2024-04-18 18:25:23.000000 parkapi_sources-0.2.0/src/parkapi_sources/parkapi_sources.py
-drwxrwxr-x   0 ernesto-ruge  (1000) ernesto-ruge  (1000)        0 2024-04-18 18:44:35.577994 parkapi_sources-0.2.0/src/parkapi_sources/scripts/
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     9093 2024-03-03 12:12:23.000000 parkapi_sources-0.2.0/src/parkapi_sources/scripts/parkapi.py
-drwxrwxr-x   0 ernesto-ruge  (1000) ernesto-ruge  (1000)        0 2024-04-18 18:44:35.577994 parkapi_sources-0.2.0/src/parkapi_sources/util/
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)      259 2024-02-18 08:11:12.000000 parkapi_sources-0.2.0/src/parkapi_sources/util/__init__.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)      373 2024-02-17 12:41:11.000000 parkapi_sources-0.2.0/src/parkapi_sources/util/config_helper.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     1060 2024-02-24 10:13:25.000000 parkapi_sources-0.2.0/src/parkapi_sources/util/encoding.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)    10420 2023-12-13 06:17:03.000000 parkapi_sources-0.2.0/src/parkapi_sources/util/xml_helper.py
-drwxrwxr-x   0 ernesto-ruge  (1000) ernesto-ruge  (1000)        0 2024-04-18 18:44:35.581994 parkapi_sources-0.2.0/src/parkapi_sources/validators/
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)      617 2024-02-26 20:02:59.000000 parkapi_sources-0.2.0/src/parkapi_sources/validators/__init__.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)      704 2024-02-24 09:14:30.000000 parkapi_sources-0.2.0/src/parkapi_sources/validators/boolean_validators.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)      899 2024-02-24 10:16:07.000000 parkapi_sources-0.2.0/src/parkapi_sources/validators/date_validator.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     1130 2024-02-26 19:19:11.000000 parkapi_sources-0.2.0/src/parkapi_sources/validators/datetime_validator.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)      511 2024-03-03 12:05:09.000000 parkapi_sources-0.2.0/src/parkapi_sources/validators/decimal_validators.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     1371 2024-02-24 09:41:47.000000 parkapi_sources-0.2.0/src/parkapi_sources/validators/integer_validators.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)      743 2023-11-10 09:25:05.000000 parkapi_sources-0.2.0/src/parkapi_sources/validators/noneable.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)      994 2024-02-26 20:06:19.000000 parkapi_sources-0.2.0/src/parkapi_sources/validators/string_validators.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)      473 2024-02-24 11:30:26.000000 parkapi_sources-0.2.0/src/parkapi_sources/validators/time_validators.py
-drwxrwxr-x   0 ernesto-ruge  (1000) ernesto-ruge  (1000)        0 2024-04-18 18:44:35.609994 parkapi_sources-0.2.0/src/parkapi_sources.egg-info/
--rw-r--r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)    13292 2024-04-18 18:44:35.000000 parkapi_sources-0.2.0/src/parkapi_sources.egg-info/PKG-INFO
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     7490 2024-04-18 18:44:35.000000 parkapi_sources-0.2.0/src/parkapi_sources.egg-info/SOURCES.txt
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)        1 2024-04-18 18:44:35.000000 parkapi_sources-0.2.0/src/parkapi_sources.egg-info/dependency_links.txt
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)      194 2024-04-18 18:44:35.000000 parkapi_sources-0.2.0/src/parkapi_sources.egg-info/requires.txt
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)       16 2024-04-18 18:44:35.000000 parkapi_sources-0.2.0/src/parkapi_sources.egg-info/top_level.txt
-drwxrwxr-x   0 ernesto-ruge  (1000) ernesto-ruge  (1000)        0 2024-04-18 18:44:35.581994 parkapi_sources-0.2.0/tests/
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)      320 2024-02-24 10:57:25.000000 parkapi_sources-0.2.0/tests/conftest.py
-drwxrwxr-x   0 ernesto-ruge  (1000) ernesto-ruge  (1000)        0 2024-04-18 18:44:35.585994 parkapi_sources-0.2.0/tests/converters/
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     1744 2024-03-10 13:12:22.000000 parkapi_sources-0.2.0/tests/converters/bahn_v2_test.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     2053 2024-04-06 12:51:03.000000 parkapi_sources-0.2.0/tests/converters/bfrk_bw_test.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)      823 2024-02-26 19:50:57.000000 parkapi_sources-0.2.0/tests/converters/conftest.py
-drwxrwxr-x   0 ernesto-ruge  (1000) ernesto-ruge  (1000)        0 2024-04-18 18:44:35.597994 parkapi_sources-0.2.0/tests/converters/data/
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)   947589 2024-02-27 10:13:50.000000 parkapi_sources-0.2.0/tests/converters/data/bahn_v2.json
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)   552854 2024-04-06 12:51:03.000000 parkapi_sources-0.2.0/tests/converters/data/bfrk_bw_bike.csv
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)   617384 2024-04-06 12:51:03.000000 parkapi_sources-0.2.0/tests/converters/data/bfrk_bw_car.csv
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)    12651 2024-02-22 20:57:47.000000 parkapi_sources-0.2.0/tests/converters/data/freiburg.json
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     3681 2024-02-18 18:19:28.000000 parkapi_sources-0.2.0/tests/converters/data/heidelberg.json
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)    63706 2024-02-23 19:52:35.000000 parkapi_sources-0.2.0/tests/converters/data/karlsruhe.json
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)   119042 2024-02-18 13:19:30.000000 parkapi_sources-0.2.0/tests/converters/data/mannheim.html
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)    20667 2024-01-24 12:53:39.000000 parkapi_sources-0.2.0/tests/converters/data/neckarsulm.csv
-drwxrwxr-x   0 ernesto-ruge  (1000) ernesto-ruge  (1000)        0 2024-04-18 18:44:35.605994 parkapi_sources-0.2.0/tests/converters/data/pbw/
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     1251 2024-02-27 10:48:03.000000 parkapi_sources-0.2.0/tests/converters/data/pbw/catalog-city.json
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)   114816 2024-02-27 10:48:22.000000 parkapi_sources-0.2.0/tests/converters/data/pbw/object-by-city-10.json
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     5061 2024-02-27 10:48:24.000000 parkapi_sources-0.2.0/tests/converters/data/pbw/object-by-city-11.json
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)    36083 2024-02-27 10:48:31.000000 parkapi_sources-0.2.0/tests/converters/data/pbw/object-by-city-12.json
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     1784 2024-02-27 10:48:32.000000 parkapi_sources-0.2.0/tests/converters/data/pbw/object-by-city-15.json
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     6859 2024-02-27 10:48:35.000000 parkapi_sources-0.2.0/tests/converters/data/pbw/object-by-city-17.json
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     7122 2024-02-27 10:48:36.000000 parkapi_sources-0.2.0/tests/converters/data/pbw/object-by-city-18.json
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     5812 2024-02-27 10:48:38.000000 parkapi_sources-0.2.0/tests/converters/data/pbw/object-by-city-19.json
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     5795 2024-02-27 10:48:40.000000 parkapi_sources-0.2.0/tests/converters/data/pbw/object-by-city-31.json
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     1622 2024-02-27 10:48:41.000000 parkapi_sources-0.2.0/tests/converters/data/pbw/object-by-city-32.json
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     6650 2024-02-27 10:48:43.000000 parkapi_sources-0.2.0/tests/converters/data/pbw/object-by-city-33.json
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     1622 2024-02-27 10:48:45.000000 parkapi_sources-0.2.0/tests/converters/data/pbw/object-by-city-34.json
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     3225 2024-02-27 10:48:04.000000 parkapi_sources-0.2.0/tests/converters/data/pbw/object-by-city-4.json
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     3187 2024-02-27 10:48:46.000000 parkapi_sources-0.2.0/tests/converters/data/pbw/object-by-city-42.json
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     3296 2024-02-27 10:48:48.000000 parkapi_sources-0.2.0/tests/converters/data/pbw/object-by-city-48.json
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     1597 2024-02-27 10:48:50.000000 parkapi_sources-0.2.0/tests/converters/data/pbw/object-by-city-49.json
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     3241 2024-02-27 10:48:51.000000 parkapi_sources-0.2.0/tests/converters/data/pbw/object-by-city-51.json
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     1635 2024-02-27 10:48:53.000000 parkapi_sources-0.2.0/tests/converters/data/pbw/object-by-city-52.json
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     1640 2024-02-27 10:48:54.000000 parkapi_sources-0.2.0/tests/converters/data/pbw/object-by-city-60.json
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     1557 2024-02-27 10:48:55.000000 parkapi_sources-0.2.0/tests/converters/data/pbw/object-by-city-61.json
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)    14227 2024-02-27 10:48:08.000000 parkapi_sources-0.2.0/tests/converters/data/pbw/object-by-city-7.json
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     3149 2024-02-27 10:48:57.000000 parkapi_sources-0.2.0/tests/converters/data/pbw/object-by-city-71.json
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     7071 2024-02-27 10:48:10.000000 parkapi_sources-0.2.0/tests/converters/data/pbw/object-by-city-9.json
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     6685 2024-02-27 10:48:58.000000 parkapi_sources-0.2.0/tests/converters/data/pbw/object-dynamic-all.json
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)    18956 2024-04-06 12:51:03.000000 parkapi_sources-0.2.0/tests/converters/data/pforzheim.json
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     9387 2024-04-06 12:51:03.000000 parkapi_sources-0.2.0/tests/converters/data/reutlingen.csv
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)    35423 2023-12-10 17:32:25.000000 parkapi_sources-0.2.0/tests/converters/data/stuttgart-realtime.xml
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)   218959 2023-12-12 19:06:24.000000 parkapi_sources-0.2.0/tests/converters/data/stuttgart-static.xml
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)    62841 2024-02-18 11:33:57.000000 parkapi_sources-0.2.0/tests/converters/data/ulm.html
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)   136171 2024-02-09 10:04:51.000000 parkapi_sources-0.2.0/tests/converters/data/vrs_p_r.xlsx
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     1859 2024-03-10 14:03:12.000000 parkapi_sources-0.2.0/tests/converters/freiburg_test.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     2226 2024-03-10 14:03:12.000000 parkapi_sources-0.2.0/tests/converters/heidelberg_test.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     2439 2024-04-06 12:51:03.000000 parkapi_sources-0.2.0/tests/converters/helper.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     1926 2024-03-10 13:13:39.000000 parkapi_sources-0.2.0/tests/converters/karlsruhe_test.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     1845 2024-03-10 14:03:12.000000 parkapi_sources-0.2.0/tests/converters/mannheim_test.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     1190 2024-04-06 12:51:03.000000 parkapi_sources-0.2.0/tests/converters/neckarsulm_test.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     2880 2024-03-10 14:03:16.000000 parkapi_sources-0.2.0/tests/converters/pbw_test.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     1165 2024-04-06 12:51:03.000000 parkapi_sources-0.2.0/tests/converters/pforzheim_test.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     1201 2024-04-06 12:51:03.000000 parkapi_sources-0.2.0/tests/converters/reutlingen_test.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     1949 2024-03-10 14:03:12.000000 parkapi_sources-0.2.0/tests/converters/stuttgart_test.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     1777 2024-03-10 13:17:24.000000 parkapi_sources-0.2.0/tests/converters/ulm_test.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     1162 2024-03-10 13:17:24.000000 parkapi_sources-0.2.0/tests/converters/vrs_p_r_test.py
-drwxrwxr-x   0 ernesto-ruge  (1000) ernesto-ruge  (1000)        0 2024-04-18 18:44:35.609994 parkapi_sources-0.2.0/tests/models/
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     2183 2024-02-24 10:57:48.000000 parkapi_sources-0.2.0/tests/models/xlsx_inputs_test.py
-drwxrwxr-x   0 ernesto-ruge  (1000) ernesto-ruge  (1000)        0 2024-04-18 18:44:35.609994 parkapi_sources-0.2.0/tests/util/
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     4105 2024-02-24 11:00:31.000000 parkapi_sources-0.2.0/tests/util/data_xml_helper.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     1706 2024-02-24 10:57:48.000000 parkapi_sources-0.2.0/tests/util/encoding_test.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     4039 2024-02-24 10:57:48.000000 parkapi_sources-0.2.0/tests/util/xml_helper_test.py
-drwxrwxr-x   0 ernesto-ruge  (1000) ernesto-ruge  (1000)        0 2024-04-18 18:44:35.609994 parkapi_sources-0.2.0/tests/validators/
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     1255 2024-02-24 10:57:48.000000 parkapi_sources-0.2.0/tests/validators/boolean_validators_test.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     1071 2024-02-24 10:57:48.000000 parkapi_sources-0.2.0/tests/validators/date_validators_test.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     2108 2024-02-24 10:57:48.000000 parkapi_sources-0.2.0/tests/validators/datetime_validators_test.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     1081 2024-02-24 10:57:48.000000 parkapi_sources-0.2.0/tests/validators/integer_validators_test.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)     1213 2024-02-24 10:57:48.000000 parkapi_sources-0.2.0/tests/validators/noneable_tests.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)      585 2024-02-24 10:57:48.000000 parkapi_sources-0.2.0/tests/validators/string_validators_test.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)      567 2024-02-24 10:57:48.000000 parkapi_sources-0.2.0/tests/validators/time_validators_test.py
--rw-rw-r--   0 ernesto-ruge  (1000) ernesto-ruge  (1000)      640 2024-02-27 09:07:05.000000 parkapi_sources-0.2.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.646194 parkapi_sources-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.610194 parkapi_sources-0.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.614194 parkapi_sources-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/.github/workflows/build-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/.github/workflows/lint-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/LICENCE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    16246 2024-05-02 13:18:48.646194 parkapi_sources-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14713 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.614194 parkapi_sources-0.3.0/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    11453 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/data/freiburg.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)    11994 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/data/heidelberg.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)    10851 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/data/mannheim.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/data/ulm.geojson
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.614194 parkapi_sources-0.3.0/dev/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/dev/parkapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/dev/test-pull-converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/dev/test-push-converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 13:18:48.646194 parkapi_sources-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.606194 parkapi_sources-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.614194 parkapi_sources-0.3.0/src/parkapi_sources/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-02 13:18:48.000000 parkapi_sources-0.3.0/src/parkapi_sources/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.614194 parkapi_sources-0.3.0/src/parkapi_sources/converters/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.614194 parkapi_sources-0.3.0/src/parkapi_sources/converters/bahn_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/bahn_v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/bahn_v2/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/bahn_v2/mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/bahn_v2/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.618194 parkapi_sources-0.3.0/src/parkapi_sources/converters/base_converter/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/base_converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/base_converter/base_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.618194 parkapi_sources-0.3.0/src/parkapi_sources/converters/base_converter/pull/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/base_converter/pull/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/base_converter/pull/pull_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/base_converter/pull/pull_scraper_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.618194 parkapi_sources-0.3.0/src/parkapi_sources/converters/base_converter/pull/static_geojson_data_mixin/
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/base_converter/pull/static_geojson_data_mixin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/base_converter/pull/static_geojson_data_mixin/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/base_converter/pull/static_geojson_data_mixin/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.618194 parkapi_sources-0.3.0/src/parkapi_sources/converters/base_converter/push/
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/base_converter/push/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/base_converter/push/csv_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/base_converter/push/json_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/base_converter/push/normalized_xlsx_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/base_converter/push/parkapi_json_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/base_converter/push/push_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/base_converter/push/xlsx_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/base_converter/push/xml_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.618194 parkapi_sources-0.3.0/src/parkapi_sources/converters/bfrk_bw/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/bfrk_bw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/bfrk_bw/base_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/bfrk_bw/base_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/bfrk_bw/bike_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/bfrk_bw/bike_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/bfrk_bw/car_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/bfrk_bw/car_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.622194 parkapi_sources-0.3.0/src/parkapi_sources/converters/freiburg/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/freiburg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/freiburg/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/freiburg/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.622194 parkapi_sources-0.3.0/src/parkapi_sources/converters/heidelberg/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/heidelberg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/heidelberg/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/heidelberg/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.622194 parkapi_sources-0.3.0/src/parkapi_sources/converters/karlsruhe/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/karlsruhe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/karlsruhe/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.622194 parkapi_sources-0.3.0/src/parkapi_sources/converters/karlsruhe/files/
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/karlsruhe/files/ca.crt.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/karlsruhe/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.622194 parkapi_sources-0.3.0/src/parkapi_sources/converters/kienzler/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/kienzler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/kienzler/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/kienzler/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.622194 parkapi_sources-0.3.0/src/parkapi_sources/converters/mannheim_buchen/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/mannheim_buchen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/mannheim_buchen/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/mannheim_buchen/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.622194 parkapi_sources-0.3.0/src/parkapi_sources/converters/neckarsulm/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/neckarsulm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/neckarsulm/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/neckarsulm/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.622194 parkapi_sources-0.3.0/src/parkapi_sources/converters/neckarsulm_bike/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/neckarsulm_bike/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/neckarsulm_bike/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.626194 parkapi_sources-0.3.0/src/parkapi_sources/converters/pbw/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/pbw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4889 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/pbw/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/pbw/mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11699 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/pbw/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.626194 parkapi_sources-0.3.0/src/parkapi_sources/converters/pforzheim/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/pforzheim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/pforzheim/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/pforzheim/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.626194 parkapi_sources-0.3.0/src/parkapi_sources/converters/pum_bw/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/pum_bw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/pum_bw/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.626194 parkapi_sources-0.3.0/src/parkapi_sources/converters/reutlingen/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/reutlingen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/reutlingen/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/reutlingen/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.626194 parkapi_sources-0.3.0/src/parkapi_sources/converters/reutlingen_bike/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/reutlingen_bike/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/reutlingen_bike/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/reutlingen_bike/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.626194 parkapi_sources-0.3.0/src/parkapi_sources/converters/stuttgart/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/stuttgart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6424 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/stuttgart/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.626194 parkapi_sources-0.3.0/src/parkapi_sources/converters/ulm/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/ulm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/ulm/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.626194 parkapi_sources-0.3.0/src/parkapi_sources/converters/vrs_p_r/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/vrs_p_r/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/converters/vrs_p_r/vrs_p_r.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.626194 parkapi_sources-0.3.0/src/parkapi_sources/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/models/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7717 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/models/parking_site_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/models/source_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/models/xlsx_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3322 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/parkapi_sources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.630194 parkapi_sources-0.3.0/src/parkapi_sources/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     9093 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/scripts/parkapi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.630194 parkapi_sources-0.3.0/src/parkapi_sources/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/util/config_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/util/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10420 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/util/xml_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.630194 parkapi_sources-0.3.0/src/parkapi_sources/validators/
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/validators/boolean_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/validators/date_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/validators/datetime_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/validators/decimal_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/validators/integer_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/validators/list_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/validators/noneable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/validators/string_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/src/parkapi_sources/validators/time_validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.646194 parkapi_sources-0.3.0/src/parkapi_sources.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16246 2024-05-02 13:18:48.000000 parkapi_sources-0.3.0/src/parkapi_sources.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8603 2024-05-02 13:18:48.000000 parkapi_sources-0.3.0/src/parkapi_sources.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 13:18:48.000000 parkapi_sources-0.3.0/src/parkapi_sources.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-02 13:18:48.000000 parkapi_sources-0.3.0/src/parkapi_sources.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-02 13:18:48.000000 parkapi_sources-0.3.0/src/parkapi_sources.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.630194 parkapi_sources-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.634194 parkapi_sources-0.3.0/tests/converters/
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/bahn_v2_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/bfrk_bw_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.638194 parkapi_sources-0.3.0/tests/converters/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   947589 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/bahn_v2.json
+-rw-r--r--   0 runner    (1001) docker     (127)   552854 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/bfrk_bw_bike.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   617384 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/bfrk_bw_car.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/buchen.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12651 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/freiburg.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/heidelberg.json
+-rw-r--r--   0 runner    (1001) docker     (127)    63706 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/karlsruhe.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/kienzler.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18474 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/mannheim.json
+-rw-r--r--   0 runner    (1001) docker     (127)    20667 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/neckarsulm.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    18115 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/neckarsulm_bike.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.642194 parkapi_sources-0.3.0/tests/converters/data/pbw/
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/pbw/catalog-city.json
+-rw-r--r--   0 runner    (1001) docker     (127)   114816 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-10.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-11.json
+-rw-r--r--   0 runner    (1001) docker     (127)    36083 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-12.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-15.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6859 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-17.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7122 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-18.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5812 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-19.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-31.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-32.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6650 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-33.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-34.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-4.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-42.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-48.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-49.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-51.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-52.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-60.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-61.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14227 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-7.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-71.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7071 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-9.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/pbw/object-dynamic-all.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18956 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/pforzheim.json
+-rw-r--r--   0 runner    (1001) docker     (127)    30849 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/pum_bw.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)     9387 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/reutlingen.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    27295 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/reutlingen_bike.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    35423 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/stuttgart-realtime.xml
+-rw-r--r--   0 runner    (1001) docker     (127)   218959 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/stuttgart-static.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    62841 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/ulm.html
+-rw-r--r--   0 runner    (1001) docker     (127)   136171 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/data/vrs_p_r.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/freiburg_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/heidelberg_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/karlsruhe_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/kienzler_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/mannheim_buchen_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/neckarsulm_bike_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/neckarsulm_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/pbw_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/pforzheim_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/pum_bw_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/reutlingen_bike_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/reutlingen_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/stuttgart_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/ulm_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/converters/vrs_p_r_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.642194 parkapi_sources-0.3.0/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/models/xlsx_inputs_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.646194 parkapi_sources-0.3.0/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     4105 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/util/data_xml_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/util/encoding_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/util/xml_helper_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:18:48.646194 parkapi_sources-0.3.0/tests/validators/
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/validators/boolean_validators_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/validators/date_validators_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/validators/datetime_validators_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/validators/integer_validators_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/validators/noneable_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/validators/string_validators_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tests/validators/time_validators_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-02 13:18:42.000000 parkapi_sources-0.3.0/tox.ini
```

### Comparing `parkapi_sources-0.2.0/.github/workflows/build-publish.yml` & `parkapi_sources-0.3.0/.github/workflows/build-publish.yml`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/.github/workflows/lint.yml` & `parkapi_sources-0.3.0/.github/workflows/lint-test.yml`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,28 @@
 name: lint
 
 on:
-  push:
-    branches:
-      - '*'
   pull_request:
     branches:
       - '*'
   # make workflow "callable" by others
   workflow_call:
 
 jobs:
   lint:
     runs-on: ubuntu-latest
-    strategy:
-      matrix:
-        python-version:
-          - '3'
+
     steps:
     - name: checkout
       uses: actions/checkout@v4
-    - name: setup Python v${{ matrix.python-version }}
+
+    - name: setup Python v3.10
       uses: actions/setup-python@v5
       with:
-        python-version: ${{ matrix.python-version }}
+        python-version: '3.10'
         cache: 'pip'
 
     - name: pip install
       run: pip install -r requirements.txt -r requirements-dev.txt
 
     - name: lint using ruff
       # We could also use the official GitHub Actions integration.
@@ -37,7 +32,32 @@
 
     - name: format using black
       # We could also use the official GitHub Actions integration.
       # https://black.readthedocs.io/en/stable/integrations/github_actions.html
       # uses: uses: psf/black@stable
       run: |
         black -S --check --diff ./src ./tests
+
+  test:
+    runs-on: ubuntu-latest
+
+    steps:
+
+    - name: set timezone
+      uses: szenius/set-timezone@v2.0
+      with:
+        timezoneLinux: "Europe/Berlin"
+
+    - name: checkout
+      uses: actions/checkout@v4
+
+    - name: setup Python v3.10
+      uses: actions/setup-python@v5
+      with:
+        python-version: '3.10'
+        cache: 'pip'
+
+    - name: pip install
+      run: pip install -r requirements.txt -r requirements-dev.txt
+
+    - name: run pytest
+      run: python -m pytest tests
```

### Comparing `parkapi_sources-0.2.0/LICENCE.txt` & `parkapi_sources-0.3.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/PKG-INFO` & `parkapi_sources-0.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parkapi_sources
-Version: 0.2.0
+Version: 0.3.0
 Summary: ParkAPI Sources is a collection of converters from several different data sources to normalized ParkAPI data.
 Author-email: "Ernesto Ruge, binary butterfly GmbH" <ernesto.ruge@binary-butterfly.de>
 Maintainer-email: "Ernesto Ruge, binary butterfly GmbH" <ernesto.ruge@binary-butterfly.de>
 Keywords: data,parking,converter,mobility,car,bike
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -43,22 +43,28 @@
 | name                                                                              | purpose | type        | uid                  | realtime |
 |-----------------------------------------------------------------------------------|---------|-------------|----------------------|----------|
 | Deutsche Bahn                                                                     | car     | pull        | `bahn_v2`            | no       |
 | Barrierefreie Reisekette Baden-Württemberg: PKW-Parkplätze an Bahnhöfen           | car     | push (csv)  | `bfrk_bw_oepnv_car`  | no       |
 | Barrierefreie Reisekette Baden-Württemberg: PKW-Parkplätze an Bushaltestellen     | car     | push (csv)  | `bfrk_bw_spnv_car`   | no       |
 | Barrierefreie Reisekette Baden-Württemberg: Fahrrad-Parkplätze an Bahnhöfen       | bike    | push (csv)  | `bfrk_bw_oepnv_bike` | no       |
 | Barrierefreie Reisekette Baden-Württemberg: Fahrrad-Parkplätze an Bushaltestellen | bike    | push (csv)  | `bfrk_bw_spnv_bike`  | no       |
+| Stadt Buchen                                                                      | car     | push (json) | `buchen`             | yes      |
 | Stadt Freiburg                                                                    | car     | pull        | `freiburg`           | yes      |
 | Stadt Heidelberg                                                                  | car     | pull        | `heidelberg`         | yes      |
 | Stadt Karlsruhe                                                                   | car     | pull        | `karlsruhe`          | yes      |
-| Stadt Mannheim                                                                    | car     | pull        | `mannheim`           | yes      |
+| Kienzler                                                                          | bike    | pull        | `kienzler`           | yes      |
+| Stadt Mannheim                                                                    | car     | push (json) | `mannheim`           | yes      |
+| Stadt Neckarsulm: PKW-Parkplätze                                                  | car     | pull        | `neckarsulm`         | no       |
+| Stadt Neckarsulm: Fahrrad-Abstellanlagen                                          | bike    | pull        | `neckarsulm_bike`    | no       |
 | Stadt Karlsruhe                                                                   | car     | push (csv)  | `neckarsulm`         | no       |
+| Baden-Württemberg: Parken und Mitfahren                                           | car     | push (xlsx) | `pum_bw`             | no       |
 | Parkraumgesellschaft Baden-Württemberg                                            | car     | pull        | `pbw`                | yes      |
 | Stadt Pforzheim                                                                   | car     | push (csv)  | `pforzheim`          | no       |
-| Stadt Reutlingen                                                                  | car     | push (csv)  | `reutlingen`         | no       |
+| Stadt Reutlingen: PKW-Parkplätze                                                  | car     | push (csv)  | `reutlingen`         | no       |
+| Stadt Reutlingen: Fahrrad-Abstellanlagen                                          | bike    | push (csv)  | `reutlingen_bike`    | no       |
 | Stadt Stuttgart                                                                   | car     | push (json) | `stuttgart`          | yes      |
 | Stadt Ulm                                                                         | car     | pull        | `ulm`                | yes      |
 | Verband Region Stuttgart: Park and Ride                                           | car     | pull        | `vrs_p_r`            | yes      |
 
 New converters for new sources are always welcome, please have a look at "Contribute" below.
 
 
@@ -212,14 +218,56 @@
 
 If you test a `PullConverter`, you will need no mock requests. This can be done using the fantastic
 [`requests_mock`](https://pypi.org/project/requests-mock/) library.
 
 If you created new validators, these should be tested with different inputs. Usually, `pytest.parametrize` is a nice approach to do this.
 
 
+### Migrate a converter
+
+If you want to migrate a v1 or v2 converter, you can re-use some of the code. There is a paradigm change, though: `parkapi-source-v3` 
+enforces a strict validation after transforming the data, while v1 and v2 converters don't. ParkAPI v1 / v2 converters are always pull
+converters, so the base class is always `PullConverter`.
+
+Instead of defining `POOL`, you will set `source_info` at the same place. Attributes are almost the same, except for `id` was renamed to 
+`uid`, and there is the new attribute `has_realtime_data`, which has to be set.
+
+ParkAPI v1 and v2 used two methods for static and realtime data, just as `parkapi-sources-v3`:
+
+- the old static data handling `def get_lot_infos(self) -> List[LotInfo]:` is
+  `get_static_parking_sites(self) -> tuple[list[StaticParkingSiteInput], list[ImportParkingSiteException]]:` in `parkapi-sources-v3`.
+- the old realtime data handling`def get_lot_data(self) -> List[LotData]:` is
+  `def get_realtime_parking_sites(self) -> tuple[list[RealtimeParkingSiteInput], list[ImportParkingSiteException]]:` in 
+  `parkapi-sources-v3`.
+
+The result objects have quite the same idea, too:
+
+- `LotInfo` gets `StaticParkingSiteInput`
+- `LotData` gets `RealtimeParkingSiteInput`
+
+There's also a helper for scraped content: before, there was `self.request_soup(self.POOL.public_url)` in order to get a `BeautifulSoup`
+element. Now, there is a helper mixin called `PullScraperMixin`. You can use it this way: 
+
+```
+class MyPullConverter(PullConverter, PullScraperMixin):
+```
+
+Additionally, there is another mixin for the GeoJSON files you already know from v1 and v2 converters: `StaticGeojsonDataMixin`. Using this,
+you can just define the static data method this way:
+
+```
+    def get_static_parking_sites(self) -> tuple[list[StaticParkingSiteInput], list[ImportParkingSiteException]]:
+        return self._get_static_parking_site_inputs_and_exceptions(source_uid=self.source_info.uid)
+```
+
+Afterwards, you can put the GeoJSON file to `/data`.
+
+Please keep in mind that you will have to add tests for the migrated scraper.
+
+
 ### Linting
 
 As we try to keep a consistent code style, please lint your code before creating the merge request. We use `black` and `ruff` for linting.
 There is Makefile target to do both: `make lint`. It runs the following commands:
 
 ```bash
 black ./src ./tests
```

### Comparing `parkapi_sources-0.2.0/README.md` & `parkapi_sources-0.3.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -9,22 +9,28 @@
 | name                                                                              | purpose | type        | uid                  | realtime |
 |-----------------------------------------------------------------------------------|---------|-------------|----------------------|----------|
 | Deutsche Bahn                                                                     | car     | pull        | `bahn_v2`            | no       |
 | Barrierefreie Reisekette Baden-Württemberg: PKW-Parkplätze an Bahnhöfen           | car     | push (csv)  | `bfrk_bw_oepnv_car`  | no       |
 | Barrierefreie Reisekette Baden-Württemberg: PKW-Parkplätze an Bushaltestellen     | car     | push (csv)  | `bfrk_bw_spnv_car`   | no       |
 | Barrierefreie Reisekette Baden-Württemberg: Fahrrad-Parkplätze an Bahnhöfen       | bike    | push (csv)  | `bfrk_bw_oepnv_bike` | no       |
 | Barrierefreie Reisekette Baden-Württemberg: Fahrrad-Parkplätze an Bushaltestellen | bike    | push (csv)  | `bfrk_bw_spnv_bike`  | no       |
+| Stadt Buchen                                                                      | car     | push (json) | `buchen`             | yes      |
 | Stadt Freiburg                                                                    | car     | pull        | `freiburg`           | yes      |
 | Stadt Heidelberg                                                                  | car     | pull        | `heidelberg`         | yes      |
 | Stadt Karlsruhe                                                                   | car     | pull        | `karlsruhe`          | yes      |
-| Stadt Mannheim                                                                    | car     | pull        | `mannheim`           | yes      |
+| Kienzler                                                                          | bike    | pull        | `kienzler`           | yes      |
+| Stadt Mannheim                                                                    | car     | push (json) | `mannheim`           | yes      |
+| Stadt Neckarsulm: PKW-Parkplätze                                                  | car     | pull        | `neckarsulm`         | no       |
+| Stadt Neckarsulm: Fahrrad-Abstellanlagen                                          | bike    | pull        | `neckarsulm_bike`    | no       |
 | Stadt Karlsruhe                                                                   | car     | push (csv)  | `neckarsulm`         | no       |
+| Baden-Württemberg: Parken und Mitfahren                                           | car     | push (xlsx) | `pum_bw`             | no       |
 | Parkraumgesellschaft Baden-Württemberg                                            | car     | pull        | `pbw`                | yes      |
 | Stadt Pforzheim                                                                   | car     | push (csv)  | `pforzheim`          | no       |
-| Stadt Reutlingen                                                                  | car     | push (csv)  | `reutlingen`         | no       |
+| Stadt Reutlingen: PKW-Parkplätze                                                  | car     | push (csv)  | `reutlingen`         | no       |
+| Stadt Reutlingen: Fahrrad-Abstellanlagen                                          | bike    | push (csv)  | `reutlingen_bike`    | no       |
 | Stadt Stuttgart                                                                   | car     | push (json) | `stuttgart`          | yes      |
 | Stadt Ulm                                                                         | car     | pull        | `ulm`                | yes      |
 | Verband Region Stuttgart: Park and Ride                                           | car     | pull        | `vrs_p_r`            | yes      |
 
 New converters for new sources are always welcome, please have a look at "Contribute" below.
 
 
@@ -178,14 +184,56 @@
 
 If you test a `PullConverter`, you will need no mock requests. This can be done using the fantastic
 [`requests_mock`](https://pypi.org/project/requests-mock/) library.
 
 If you created new validators, these should be tested with different inputs. Usually, `pytest.parametrize` is a nice approach to do this.
 
 
+### Migrate a converter
+
+If you want to migrate a v1 or v2 converter, you can re-use some of the code. There is a paradigm change, though: `parkapi-source-v3` 
+enforces a strict validation after transforming the data, while v1 and v2 converters don't. ParkAPI v1 / v2 converters are always pull
+converters, so the base class is always `PullConverter`.
+
+Instead of defining `POOL`, you will set `source_info` at the same place. Attributes are almost the same, except for `id` was renamed to 
+`uid`, and there is the new attribute `has_realtime_data`, which has to be set.
+
+ParkAPI v1 and v2 used two methods for static and realtime data, just as `parkapi-sources-v3`:
+
+- the old static data handling `def get_lot_infos(self) -> List[LotInfo]:` is
+  `get_static_parking_sites(self) -> tuple[list[StaticParkingSiteInput], list[ImportParkingSiteException]]:` in `parkapi-sources-v3`.
+- the old realtime data handling`def get_lot_data(self) -> List[LotData]:` is
+  `def get_realtime_parking_sites(self) -> tuple[list[RealtimeParkingSiteInput], list[ImportParkingSiteException]]:` in 
+  `parkapi-sources-v3`.
+
+The result objects have quite the same idea, too:
+
+- `LotInfo` gets `StaticParkingSiteInput`
+- `LotData` gets `RealtimeParkingSiteInput`
+
+There's also a helper for scraped content: before, there was `self.request_soup(self.POOL.public_url)` in order to get a `BeautifulSoup`
+element. Now, there is a helper mixin called `PullScraperMixin`. You can use it this way: 
+
+```
+class MyPullConverter(PullConverter, PullScraperMixin):
+```
+
+Additionally, there is another mixin for the GeoJSON files you already know from v1 and v2 converters: `StaticGeojsonDataMixin`. Using this,
+you can just define the static data method this way:
+
+```
+    def get_static_parking_sites(self) -> tuple[list[StaticParkingSiteInput], list[ImportParkingSiteException]]:
+        return self._get_static_parking_site_inputs_and_exceptions(source_uid=self.source_info.uid)
+```
+
+Afterwards, you can put the GeoJSON file to `/data`.
+
+Please keep in mind that you will have to add tests for the migrated scraper.
+
+
 ### Linting
 
 As we try to keep a consistent code style, please lint your code before creating the merge request. We use `black` and `ruff` for linting.
 There is Makefile target to do both: `make lint`. It runs the following commands:
 
 ```bash
 black ./src ./tests
```

### Comparing `parkapi_sources-0.2.0/data/freiburg.geojson` & `parkapi_sources-0.3.0/data/freiburg.geojson`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/data/heidelberg.geojson` & `parkapi_sources-0.3.0/data/heidelberg.geojson`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/data/mannheim.geojson` & `parkapi_sources-0.3.0/data/mannheim.geojson`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/data/ulm.geojson` & `parkapi_sources-0.3.0/data/ulm.geojson`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/dev/test-pull-converter.py` & `parkapi_sources-0.3.0/dev/test-pull-converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/dev/test-push-converter.py` & `parkapi_sources-0.3.0/dev/test-push-converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/pyproject.toml` & `parkapi_sources-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/src/parkapi_sources/converters/__init__.py` & `parkapi_sources-0.3.0/src/parkapi_sources/converters/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,15 +5,19 @@
 
 from .bahn_v2 import BahnV2PullConverter
 from .base_converter import BaseConverter
 from .bfrk_bw import BfrkBwOepnvBikePushConverter, BfrkBwOepnvCarPushConverter, BfrkBwSpnvBikePushConverter, BfrkBwSpnvCarPushConverter
 from .freiburg import FreiburgPullConverter
 from .heidelberg import HeidelbergPullConverter
 from .karlsruhe import KarlsruhePullConverter
-from .mannheim import MannheimPullConverter
+from .kienzler import KienzlerPullConverter
+from .mannheim_buchen import BuchenPushConverter, MannheimPushConverter
 from .neckarsulm import NeckarsulmPushConverter
+from .neckarsulm_bike import NeckarsulmBikePushConverter
 from .pbw import PbwPullConverter
 from .pforzheim import PforzheimPushConverter
+from .pum_bw import PumBwPushConverter
 from .reutlingen import ReutlingenPushConverter
+from .reutlingen_bike import ReutlingenBikePushConverter
 from .stuttgart import StuttgartPushConverter
 from .ulm import UlmPullConverter
 from .vrs_p_r import VrsParkAndRidePushConverter
```

### Comparing `parkapi_sources-0.2.0/src/parkapi_sources/converters/bahn_v2/converter.py` & `parkapi_sources-0.3.0/src/parkapi_sources/converters/bahn_v2/converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/src/parkapi_sources/converters/bahn_v2/mapper.py` & `parkapi_sources-0.3.0/src/parkapi_sources/converters/bahn_v2/mapper.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/src/parkapi_sources/converters/bahn_v2/validators.py` & `parkapi_sources-0.3.0/src/parkapi_sources/converters/bahn_v2/validators.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/src/parkapi_sources/converters/base_converter/base_converter.py` & `parkapi_sources-0.3.0/src/parkapi_sources/converters/base_converter/base_converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/src/parkapi_sources/converters/base_converter/pull/pull_converter.py` & `parkapi_sources-0.3.0/src/parkapi_sources/converters/base_converter/pull/pull_converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/src/parkapi_sources/converters/base_converter/pull/pull_scraper_mixin.py` & `parkapi_sources-0.3.0/src/parkapi_sources/converters/base_converter/pull/pull_scraper_mixin.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/src/parkapi_sources/converters/base_converter/pull/static_geojson_data_mixin/mixin.py` & `parkapi_sources-0.3.0/src/parkapi_sources/converters/base_converter/pull/static_geojson_data_mixin/mixin.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/src/parkapi_sources/converters/base_converter/pull/static_geojson_data_mixin/models.py` & `parkapi_sources-0.3.0/src/parkapi_sources/converters/base_converter/pull/static_geojson_data_mixin/models.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/src/parkapi_sources/converters/base_converter/push/csv_converter.py` & `parkapi_sources-0.3.0/src/parkapi_sources/converters/base_converter/push/csv_converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/src/parkapi_sources/converters/base_converter/push/json_converter.py` & `parkapi_sources-0.3.0/src/parkapi_sources/converters/base_converter/push/json_converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/src/parkapi_sources/converters/base_converter/push/normalized_xlsx_converter.py` & `parkapi_sources-0.3.0/src/parkapi_sources/converters/base_converter/push/normalized_xlsx_converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/src/parkapi_sources/converters/base_converter/push/xlsx_converter.py` & `parkapi_sources-0.3.0/src/parkapi_sources/converters/base_converter/push/xlsx_converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/src/parkapi_sources/converters/base_converter/push/xml_converter.py` & `parkapi_sources-0.3.0/src/parkapi_sources/converters/base_converter/push/xml_converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/src/parkapi_sources/converters/bfrk_bw/base_converter.py` & `parkapi_sources-0.3.0/src/parkapi_sources/converters/bfrk_bw/base_converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/src/parkapi_sources/converters/bfrk_bw/base_models.py` & `parkapi_sources-0.3.0/src/parkapi_sources/converters/bfrk_bw/base_models.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/src/parkapi_sources/converters/bfrk_bw/bike_converter.py` & `parkapi_sources-0.3.0/src/parkapi_sources/converters/bfrk_bw/bike_converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/src/parkapi_sources/converters/bfrk_bw/bike_models.py` & `parkapi_sources-0.3.0/src/parkapi_sources/converters/bfrk_bw/bike_models.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/src/parkapi_sources/converters/bfrk_bw/car_converter.py` & `parkapi_sources-0.3.0/src/parkapi_sources/converters/bfrk_bw/car_converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/src/parkapi_sources/converters/bfrk_bw/car_models.py` & `parkapi_sources-0.3.0/src/parkapi_sources/converters/bfrk_bw/car_models.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/src/parkapi_sources/converters/freiburg/converter.py` & `parkapi_sources-0.3.0/src/parkapi_sources/converters/freiburg/converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/src/parkapi_sources/converters/freiburg/models.py` & `parkapi_sources-0.3.0/src/parkapi_sources/converters/freiburg/models.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/src/parkapi_sources/converters/heidelberg/converter.py` & `parkapi_sources-0.3.0/src/parkapi_sources/converters/heidelberg/converter.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from parkapi_sources.exceptions import ImportParkingSiteException, ImportSourceException
 from parkapi_sources.models import RealtimeParkingSiteInput, SourceInfo, StaticParkingSiteInput
 
 from .validators import HeidelbergRealtimeInput, HeidelbergRealtimeUpdateInput
 
 
 class HeidelbergPullConverter(PullConverter, StaticGeojsonDataMixin):
+    required_config_keys = ['PARK_API_HEIDELBERG_API_KEY']
     heidelberg_realtime_validator = DataclassValidator(HeidelbergRealtimeInput)
     heidelberg_realtime_update_validator = DataclassValidator(HeidelbergRealtimeUpdateInput)
     source_info = SourceInfo(
         uid='heidelberg',
         name='Stadt Heidelberg',
         public_url='https://parken.heidelberg.de',
         source_url='https://parken.heidelberg.de/v1',
```

### Comparing `parkapi_sources-0.2.0/src/parkapi_sources/converters/heidelberg/validators.py` & `parkapi_sources-0.3.0/src/parkapi_sources/converters/heidelberg/validators.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/src/parkapi_sources/converters/karlsruhe/converter.py` & `parkapi_sources-0.3.0/src/parkapi_sources/converters/karlsruhe/converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/src/parkapi_sources/converters/karlsruhe/files/ca.crt.pem` & `parkapi_sources-0.3.0/src/parkapi_sources/converters/karlsruhe/files/ca.crt.pem`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/src/parkapi_sources/converters/karlsruhe/models.py` & `parkapi_sources-0.3.0/src/parkapi_sources/converters/karlsruhe/models.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/src/parkapi_sources/converters/mannheim/converter.py` & `parkapi_sources-0.3.0/src/parkapi_sources/converters/ulm/converter.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,54 +1,52 @@
 """
 Copyright 2024 binary butterfly GmbH
 Use of this source code is governed by an MIT-style license that can be found in the LICENSE.txt.
 """
 
-from datetime import datetime
+from datetime import datetime, timezone
 from typing import Optional
 
 from bs4.element import Tag
 
 from parkapi_sources.converters.base_converter.pull import PullConverter, PullScraperMixin, StaticGeojsonDataMixin
 from parkapi_sources.exceptions import ImportParkingSiteException
 from parkapi_sources.models import RealtimeParkingSiteInput, SourceInfo, StaticParkingSiteInput
 
 
-class MannheimPullConverter(PullConverter, StaticGeojsonDataMixin, PullScraperMixin):
+class UlmPullConverter(PullConverter, StaticGeojsonDataMixin, PullScraperMixin):
     source_info = SourceInfo(
-        uid='mannheim',
-        name='Stadt Mannheim',
-        public_url='https://www.parken-mannheim.de',
+        uid='ulm',
+        name='Stadt Ulm',
+        public_url='https://www.parken-in-ulm.de',
         timezone='Europe/Berlin',
-        attribution_contributor='Mannheimer Parkhausbetriebe GmbH',
-        attribution_url='https://www.parken-mannheim.de/impressum',
+        attribution_contributor='Ulmer Parkbetriebs-GmbH',
+        attribution_url='https://www.parken-in-ulm.de/impressum.php',
         has_realtime_data=True,
     )
-    _parking_site_uids_to_ignore: list[str] = ['b8874acd-39d9-424c-9405-1fc3307b7df8']
 
     def get_static_parking_sites(self) -> tuple[list[StaticParkingSiteInput], list[ImportParkingSiteException]]:
         return self._get_static_parking_site_inputs_and_exceptions(source_uid=self.source_info.uid)
 
     def get_realtime_parking_sites(self) -> tuple[list[RealtimeParkingSiteInput], list[ImportParkingSiteException]]:
         return self._get_scraped_realtime_parking_site_inputs_and_exceptions()
 
     def get_realtime_tags_and_params(self) -> tuple[list[Tag], dict]:
         root = self.load_url_in_soup()
 
-        realtime_data_updated_at_text = root.find_all('div', id='parkhausliste-ct')[-1].find('p').text
-        realtime_data_updated_at = datetime.strptime(realtime_data_updated_at_text, 'zuletzt aktualisiert am %d.%m.%Y, %H:%M Uhr')
+        section = root.find('section', class_='s_live_counter')
+        return section.find_all('div', class_='card-container'), {}
 
-        tags = root.find_all(class_='parkhaus-lnk')
-
-        return tags, {'realtime_data_updated_at': realtime_data_updated_at}
-
-    def realtime_tag_to_dict(self, tag: Tag, realtime_data_updated_at: Optional[datetime] = None, **kwargs) -> Optional[dict]:
-        realtime_parking_site_dict = {'realtime_data_updated_at': realtime_data_updated_at.isoformat()}
-        parking_site_uid = tag.attrs.get('href').split('/')[-1]
-
-        if parking_site_uid in self._parking_site_uids_to_ignore:
-            return None
-
-        realtime_parking_site_dict['uid'] = parking_site_uid
-        realtime_parking_site_dict['realtime_free_capacity'] = int(tag.parent.find_next_sibling().text)
+    def realtime_tag_to_dict(self, tag: Tag, **kwargs) -> Optional[dict]:
+        realtime_parking_site_dict = {
+            'realtime_data_updated_at': datetime.now(tz=timezone.utc).isoformat(),
+            'uid': tag.find('a', class_='stretched-link').attrs.get('href').split('/')[-1],
+        }
+
+        parking_data = tag.find('div', class_='counter-text').get_text().strip().split(' / ')
+        realtime_parking_site_dict['realtime_capacity'] = int(parking_data[1])
+        if parking_data[0].strip() == '?':
+            realtime_parking_site_dict['realtime_free_capacity'] = None
+        else:
+            realtime_parking_site_dict['realtime_free_capacity'] = int(parking_data[0])
 
         return realtime_parking_site_dict
```

### Comparing `parkapi_sources-0.2.0/src/parkapi_sources/converters/neckarsulm/converter.py` & `parkapi_sources-0.3.0/src/parkapi_sources/converters/neckarsulm/converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 class NeckarsulmPushConverter(CsvConverter):
     neckarsulm_row_validator = DataclassValidator(NeckarsulmRowInput)
 
     source_info = SourceInfo(
         uid='neckarsulm',
-        name='Stadt Neckarsulm',
+        name='Stadt Neckarsulm: PKW-Parkplätze',
         public_url='https://www.neckarsulm.de',
         has_realtime_data=False,
     )
 
     header_mapping: dict[str, str] = {
         'id': 'uid',
         'name': 'name',
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `parkapi_sources-0.2.0/src/parkapi_sources/converters/neckarsulm/models.py` & `parkapi_sources-0.3.0/src/parkapi_sources/converters/neckarsulm/models.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/src/parkapi_sources/converters/pbw/converter.py` & `parkapi_sources-0.3.0/src/parkapi_sources/converters/pbw/converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/src/parkapi_sources/converters/pbw/mapper.py` & `parkapi_sources-0.3.0/src/parkapi_sources/converters/pbw/mapper.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/src/parkapi_sources/converters/pbw/validation.py` & `parkapi_sources-0.3.0/src/parkapi_sources/converters/pbw/validation.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/src/parkapi_sources/converters/pforzheim/converter.py` & `parkapi_sources-0.3.0/src/parkapi_sources/converters/pforzheim/converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/src/parkapi_sources/converters/pforzheim/validation.py` & `parkapi_sources-0.3.0/src/parkapi_sources/converters/pforzheim/validation.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/src/parkapi_sources/converters/reutlingen/converter.py` & `parkapi_sources-0.3.0/src/parkapi_sources/converters/reutlingen/converter.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """
 Copyright 2024 binary butterfly GmbH
 Use of this source code is governed by an MIT-style license that can be found in the LICENSE.txt.
 """
 
 import csv
-from datetime import datetime, timezone
 from io import StringIO
 
 from validataclass.exceptions import ValidationError
 from validataclass.validators import DataclassValidator
 
 from parkapi_sources.converters.base_converter.push import CsvConverter
 from parkapi_sources.exceptions import ImportParkingSiteException
@@ -18,15 +17,15 @@
 
 
 class ReutlingenPushConverter(CsvConverter):
     reutlingen_row_validator = DataclassValidator(ReutlingenRowInput)
 
     source_info = SourceInfo(
         uid='reutlingen',
-        name='Stadt Reutlingen',
+        name='Stadt Reutlingen: PKW-Parkplätze',
         public_url='https://www.reutlingen.de',
         has_realtime_data=False,
     )
 
     header_mapping: dict[str, str] = {'id': 'uid', 'ort': 'name', 'Kapazität': 'capacity', 'GEOM': 'coordinates', 'type': 'type'}
 
     def handle_csv_string(
@@ -44,30 +43,21 @@
         # We start at row 2, as the first one is our header
         for row in data[1:]:
             input_dict: dict[str, str] = {}
             for field in self.header_mapping.values():
                 input_dict[field] = row[mapping[field]]
 
             try:
-                input_data: ReutlingenRowInput = self.reutlingen_row_validator.validate(input_dict)
+                reutlingen_row_input: ReutlingenRowInput = self.reutlingen_row_validator.validate(input_dict)
             except ValidationError as e:
                 static_parking_site_errors.append(
                     ImportParkingSiteException(
-                        uid=input_dict.get('uid'),
+                        source_uid=self.source_info.uid,
+                        parking_site_uid=input_dict.get('uid'),
                         message=f'validation error for {input_dict}: {e.to_dict()}',
                     ),
                 )
                 continue
 
-            parking_site_input = StaticParkingSiteInput(
-                uid=str(input_data.uid),
-                name=input_data.name,
-                address=f'{input_data.name}, Reutlingen',
-                lat=input_data.coordinates[1],
-                lon=input_data.coordinates[0],
-                type=input_data.type.to_parking_site_type_input(),
-                capacity=input_data.capacity,
-                static_data_updated_at=datetime.now(tz=timezone.utc),
-            )
-            static_parking_site_inputs.append(parking_site_input)
+            static_parking_site_inputs.append(reutlingen_row_input.to_parking_site_input())
 
         return static_parking_site_inputs, static_parking_site_errors
```

### Comparing `parkapi_sources-0.2.0/src/parkapi_sources/converters/reutlingen/validation.py` & `parkapi_sources-0.3.0/src/parkapi_sources/converters/reutlingen/validation.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 """
 Copyright 2024 binary butterfly GmbH
 Use of this source code is governed by an MIT-style license that can be found in the LICENSE.txt.
 """
 
-import re
+from datetime import datetime, timezone
 from enum import Enum
-from typing import Any
 
 from validataclass.dataclasses import validataclass
-from validataclass.exceptions import ValidationError
-from validataclass.validators import DecimalValidator, EnumValidator, IntegerValidator, ListValidator, StringValidator
+from validataclass.validators import DecimalValidator, EnumValidator, IntegerValidator, StringValidator
 
+from parkapi_sources.models import StaticParkingSiteInput
 from parkapi_sources.models.enums import ParkingSiteType
-from parkapi_sources.validators import ExcelNoneable
+from parkapi_sources.validators import PointCoordinateTupleValidator
 
 
 class ReutlingenParkingSiteType(Enum):
     PARKHAUS = 'parkhaus'
     TIEFGARAGE = 'tiefgarage'
     PARKFLAECHE = 'parkfläche'
     P_R = 'p+r'
@@ -25,29 +24,26 @@
         return {
             self.PARKHAUS: ParkingSiteType.CAR_PARK,
             self.TIEFGARAGE: ParkingSiteType.UNDERGROUND,
             self.PARKFLAECHE: ParkingSiteType.OFF_STREET_PARKING_GROUND,
         }.get(self, ParkingSiteType.OTHER)
 
 
-class PointCoordinateTupleValidator(ListValidator):
-    PATTERN = re.compile(r'POINT \(([-+]?\d+\.\d+) ([-+]?\d+\.\d+)\)')
-
-    def validate(self, input_data: Any, **kwargs) -> list:
-        self._ensure_type(input_data, str)
-        input_match = re.match(self.PATTERN, input_data)
-
-        if input_match is None:
-            raise ValidationError(code='invalid_tuple_input', reason='invalid point coordinate tuple input')
-
-        input_data = [input_match.group(1), input_match.group(2)]
-
-        return super().validate(input_data, **kwargs)
-
-
 @validataclass
 class ReutlingenRowInput:
     uid: int = IntegerValidator(allow_strings=True)
     type: ReutlingenParkingSiteType = EnumValidator(ReutlingenParkingSiteType)
     coordinates: list = PointCoordinateTupleValidator(DecimalValidator())
-    capacity: str = ExcelNoneable(IntegerValidator(allow_strings=True))
+    capacity: int = IntegerValidator(allow_strings=True)
     name: str = StringValidator(max_length=255)
+
+    def to_parking_site_input(self) -> StaticParkingSiteInput:
+        return StaticParkingSiteInput(
+            uid=str(self.uid),
+            name=self.name,
+            address=f'{self.name}, Reutlingen',
+            lat=self.coordinates[1],
+            lon=self.coordinates[0],
+            type=self.type.to_parking_site_type_input(),
+            capacity=self.capacity,
+            static_data_updated_at=datetime.now(tz=timezone.utc),
+        )
```

### Comparing `parkapi_sources-0.2.0/src/parkapi_sources/converters/stuttgart/converter.py` & `parkapi_sources-0.3.0/src/parkapi_sources/converters/stuttgart/converter.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/src/parkapi_sources/converters/ulm/converter.py` & `parkapi_sources-0.3.0/src/parkapi_sources/converters/pum_bw/converter.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,52 +1,73 @@
 """
 Copyright 2024 binary butterfly GmbH
 Use of this source code is governed by an MIT-style license that can be found in the LICENSE.txt.
 """
 
 from datetime import datetime, timezone
-from typing import Optional
+from typing import Any
 
-from bs4.element import Tag
+from openpyxl.cell import Cell
+from openpyxl.workbook.workbook import Workbook
+from validataclass.exceptions import ValidationError
 
-from parkapi_sources.converters.base_converter.pull import PullConverter, PullScraperMixin, StaticGeojsonDataMixin
+from parkapi_sources.converters.base_converter.push import XlsxConverter
 from parkapi_sources.exceptions import ImportParkingSiteException
-from parkapi_sources.models import RealtimeParkingSiteInput, SourceInfo, StaticParkingSiteInput
+from parkapi_sources.models import SourceInfo, StaticParkingSiteInput
 
 
-class UlmPullConverter(PullConverter, StaticGeojsonDataMixin, PullScraperMixin):
+class PumBwPushConverter(XlsxConverter):
     source_info = SourceInfo(
-        uid='ulm',
-        name='Stadt Ulm',
-        public_url='https://www.parken-in-ulm.de',
-        timezone='Europe/Berlin',
-        attribution_contributor='Ulmer Parkbetriebs-GmbH',
-        attribution_url='https://www.parken-in-ulm.de/impressum.php',
-        has_realtime_data=True,
+        uid='pum_bw',
+        name='Baden-Württemberg: Parken und Mitfahren',
+        public_url='https://mobidata-bw.de/dataset/p-m-parkplatze-baden-wurttemberg',
+        has_realtime_data=False,
     )
 
-    def get_static_parking_sites(self) -> tuple[list[StaticParkingSiteInput], list[ImportParkingSiteException]]:
-        return self._get_static_parking_site_inputs_and_exceptions(source_uid=self.source_info.uid)
+    header_row: dict[str, str] = {
+        'AS-Nummer': 'uid',
+        'Bezeichnung Parkplatz': 'name',
+        'Straße': 'street',
+        'Längengrad': 'lat',
+        'Breitengrad': 'lon',
+        'Zufahrt': 'description',
+        'Anzahl Plätze': 'capacity',
+    }
+
+    def handle_xlsx(self, workbook: Workbook) -> tuple[list[StaticParkingSiteInput], list[ImportParkingSiteException]]:
+        static_parking_site_inputs: list[StaticParkingSiteInput] = []
+        static_parking_site_errors: list[ImportParkingSiteException] = []
+
+        worksheet = workbook.active
+        mapping: dict[str, int] = self.get_mapping_by_header(next(worksheet.rows))
+
+        # We start at row 2, as the first one is our header
+        for row in worksheet.iter_rows(min_row=2):
+            # ignore empty lines as LibreOffice sometimes adds empty rows at the end of a file
+            if row[0].value is None:
+                continue
+            parking_site_dict = self.map_row_to_parking_site_dict(mapping, row)
+
+            try:
+                static_parking_site_inputs.append(self.static_parking_site_validator.validate(parking_site_dict))
+            except ValidationError as e:
+                static_parking_site_errors.append(
+                    ImportParkingSiteException(
+                        uid=parking_site_dict.get('uid'),
+                        message=f'invalid static parking site data: {e.to_dict()}',
+                    )
+                )
+                continue
+
+        return static_parking_site_inputs, static_parking_site_errors
+
+    @staticmethod
+    def map_row_to_parking_site_dict(mapping: dict[str, int], row: list[Cell]) -> dict[str, Any]:
+        parking_site_dict: dict[str, str] = {}
+        for field in mapping.keys():
+            parking_site_dict[field] = row[mapping[field]].value
+
+        parking_site_dict['uid'] = f"{parking_site_dict['uid']}-{parking_site_dict['name']}"
+        parking_site_dict['name'] = f"{parking_site_dict['street']} {parking_site_dict['name']}"
+        parking_site_dict['static_data_updated_at'] = datetime.now(tz=timezone.utc).isoformat()
 
-    def get_realtime_parking_sites(self) -> tuple[list[RealtimeParkingSiteInput], list[ImportParkingSiteException]]:
-        return self._get_scraped_realtime_parking_site_inputs_and_exceptions()
-
-    def get_realtime_tags_and_params(self) -> tuple[list[Tag], dict]:
-        root = self.load_url_in_soup()
-
-        section = root.find('section', class_='s_live_counter')
-        return section.find_all('div', class_='card-container'), {}
-
-    def realtime_tag_to_dict(self, tag: Tag, **kwargs) -> Optional[dict]:
-        realtime_parking_site_dict = {
-            'realtime_data_updated_at': datetime.now(tz=timezone.utc).isoformat(),
-            'uid': tag.find('a', class_='stretched-link').attrs.get('href').split('/')[-1],
-        }
-
-        parking_data = tag.find('div', class_='counter-text').get_text().strip().split(' / ')
-        realtime_parking_site_dict['realtime_capacity'] = int(parking_data[1])
-        if parking_data[0].strip() == '?':
-            realtime_parking_site_dict['realtime_free_capacity'] = None
-        else:
-            realtime_parking_site_dict['realtime_free_capacity'] = int(parking_data[0])
-
-        return realtime_parking_site_dict
+        return parking_site_dict
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `parkapi_sources-0.2.0/src/parkapi_sources/converters/vrs_p_r/vrs_p_r.py` & `parkapi_sources-0.3.0/src/parkapi_sources/converters/vrs_p_r/vrs_p_r.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/src/parkapi_sources/exceptions.py` & `parkapi_sources-0.3.0/src/parkapi_sources/exceptions.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/src/parkapi_sources/models/enums.py` & `parkapi_sources-0.3.0/src/parkapi_sources/models/enums.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/src/parkapi_sources/models/parking_site_inputs.py` & `parkapi_sources-0.3.0/src/parkapi_sources/models/parking_site_inputs.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,16 +42,16 @@
     purpose: PurposeType = EnumValidator(PurposeType), Default(PurposeType.CAR)
     operator_name: OptionalUnsetNone[str] = StringValidator(max_length=256), DefaultUnset
     public_url: OptionalUnsetNone[str] = Noneable(UrlValidator(max_length=4096)), DefaultUnset
     address: OptionalUnsetNone[str] = Noneable(StringValidator(max_length=512)), DefaultUnset
     description: OptionalUnsetNone[str] = Noneable(StringValidator(max_length=4096)), DefaultUnset
     type: OptionalUnsetNone[ParkingSiteType] = Noneable(EnumValidator(ParkingSiteType)), DefaultUnset
 
-    max_stay: OptionalUnsetNone[int] = Noneable(IntegerValidator(min_value=0)), DefaultUnset
-    max_height: OptionalUnsetNone[int] = Noneable(IntegerValidator(min_value=0)), DefaultUnset
+    max_stay: OptionalUnsetNone[int] = Noneable(IntegerValidator(min_value=0, allow_strings=True)), DefaultUnset
+    max_height: OptionalUnsetNone[int] = Noneable(IntegerValidator(min_value=0, allow_strings=True)), DefaultUnset
     has_lighting: OptionalUnsetNone[bool] = Noneable(BooleanValidator()), DefaultUnset
     fee_description: OptionalUnsetNone[str] = Noneable(StringValidator(max_length=4096)), DefaultUnset
     has_fee: OptionalUnsetNone[bool] = Noneable(BooleanValidator()), DefaultUnset
     park_and_ride_type: OptionalUnsetNone[list[ParkAndRideType]] = (
         Noneable(
             ListValidator(EnumValidator(ParkAndRideType)),
         ),
@@ -69,22 +69,22 @@
         ),
         DefaultUnset,
     )
 
     lat: Decimal = NumericValidator(min_value=-90, max_value=90)
     lon: Decimal = NumericValidator(min_value=-180, max_value=180)
 
-    capacity: OptionalUnsetNone[int] = Noneable(IntegerValidator(min_value=0)), DefaultUnset
-    capacity_disabled: OptionalUnsetNone[int] = Noneable(IntegerValidator(min_value=0)), DefaultUnset
-    capacity_woman: OptionalUnsetNone[int] = Noneable(IntegerValidator(min_value=0)), DefaultUnset
-    capacity_family: OptionalUnsetNone[int] = Noneable(IntegerValidator(min_value=0)), DefaultUnset
-    capacity_charging: OptionalUnsetNone[int] = Noneable(IntegerValidator(min_value=0)), DefaultUnset
-    capacity_carsharing: OptionalUnsetNone[int] = Noneable(IntegerValidator(min_value=0)), DefaultUnset
-    capacity_truck: OptionalUnsetNone[int] = Noneable(IntegerValidator(min_value=0)), DefaultUnset
-    capacity_bus: OptionalUnsetNone[int] = Noneable(IntegerValidator(min_value=0)), DefaultUnset
+    capacity: OptionalUnsetNone[int] = Noneable(IntegerValidator(min_value=0, allow_strings=True)), DefaultUnset
+    capacity_disabled: OptionalUnsetNone[int] = Noneable(IntegerValidator(min_value=0, allow_strings=True)), DefaultUnset
+    capacity_woman: OptionalUnsetNone[int] = Noneable(IntegerValidator(min_value=0, allow_strings=True)), DefaultUnset
+    capacity_family: OptionalUnsetNone[int] = Noneable(IntegerValidator(min_value=0, allow_strings=True)), DefaultUnset
+    capacity_charging: OptionalUnsetNone[int] = Noneable(IntegerValidator(min_value=0, allow_strings=True)), DefaultUnset
+    capacity_carsharing: OptionalUnsetNone[int] = Noneable(IntegerValidator(min_value=0, allow_strings=True)), DefaultUnset
+    capacity_truck: OptionalUnsetNone[int] = Noneable(IntegerValidator(min_value=0, allow_strings=True)), DefaultUnset
+    capacity_bus: OptionalUnsetNone[int] = Noneable(IntegerValidator(min_value=0, allow_strings=True)), DefaultUnset
 
     opening_hours: OptionalUnsetNone[str] = Noneable(StringValidator(max_length=512)), DefaultUnset
 
     external_identifiers: OptionalUnsetNone[list[ExternalIdentifierInput]] = (
         Noneable(ListValidator(DataclassValidator(ExternalIdentifierInput))),
         DefaultUnset,
     )
@@ -113,24 +113,24 @@
         target_timezone=timezone.utc,
         discard_milliseconds=True,
     )
     realtime_opening_status: OptionalUnsetNone[OpeningStatus] = (
         Noneable(EnumValidator(OpeningStatus), default=OpeningStatus.UNKNOWN),
         Default(OpeningStatus.UNKNOWN),
     )
-    realtime_capacity: OptionalUnsetNone[int] = Noneable(IntegerValidator(min_value=0)), DefaultUnset
-    realtime_capacity_disabled: OptionalUnsetNone[int] = Noneable(IntegerValidator(min_value=0)), DefaultUnset
-    realtime_capacity_woman: OptionalUnsetNone[int] = Noneable(IntegerValidator(min_value=0)), DefaultUnset
-    realtime_capacity_family: OptionalUnsetNone[int] = Noneable(IntegerValidator(min_value=0)), DefaultUnset
-    realtime_capacity_charging: OptionalUnsetNone[int] = Noneable(IntegerValidator(min_value=0)), DefaultUnset
-    realtime_capacity_carsharing: OptionalUnsetNone[int] = Noneable(IntegerValidator(min_value=0)), DefaultUnset
-    realtime_capacity_truck: OptionalUnsetNone[int] = Noneable(IntegerValidator(min_value=0)), DefaultUnset
-    realtime_capacity_bus: OptionalUnsetNone[int] = Noneable(IntegerValidator(min_value=0)), DefaultUnset
-
-    realtime_free_capacity: OptionalUnsetNone[int] = Noneable(IntegerValidator(min_value=0)), DefaultUnset
-    realtime_free_capacity_disabled: OptionalUnsetNone[int] = Noneable(IntegerValidator(min_value=0)), DefaultUnset
-    realtime_free_capacity_woman: OptionalUnsetNone[int] = Noneable(IntegerValidator(min_value=0)), DefaultUnset
-    realtime_free_capacity_family: OptionalUnsetNone[int] = Noneable(IntegerValidator(min_value=0)), DefaultUnset
-    realtime_free_capacity_charging: OptionalUnsetNone[int] = Noneable(IntegerValidator(min_value=0)), DefaultUnset
-    realtime_free_capacity_carsharing: OptionalUnsetNone[int] = Noneable(IntegerValidator(min_value=0)), DefaultUnset
-    realtime_free_capacity_truck: OptionalUnsetNone[int] = Noneable(IntegerValidator(min_value=0)), DefaultUnset
-    realtime_free_capacity_bus: OptionalUnsetNone[int] = Noneable(IntegerValidator(min_value=0)), DefaultUnset
+    realtime_capacity: OptionalUnsetNone[int] = Noneable(IntegerValidator(min_value=0, allow_strings=True)), DefaultUnset
+    realtime_capacity_disabled: OptionalUnsetNone[int] = Noneable(IntegerValidator(min_value=0, allow_strings=True)), DefaultUnset
+    realtime_capacity_woman: OptionalUnsetNone[int] = Noneable(IntegerValidator(min_value=0, allow_strings=True)), DefaultUnset
+    realtime_capacity_family: OptionalUnsetNone[int] = Noneable(IntegerValidator(min_value=0, allow_strings=True)), DefaultUnset
+    realtime_capacity_charging: OptionalUnsetNone[int] = Noneable(IntegerValidator(min_value=0, allow_strings=True)), DefaultUnset
+    realtime_capacity_carsharing: OptionalUnsetNone[int] = Noneable(IntegerValidator(min_value=0, allow_strings=True)), DefaultUnset
+    realtime_capacity_truck: OptionalUnsetNone[int] = Noneable(IntegerValidator(min_value=0, allow_strings=True)), DefaultUnset
+    realtime_capacity_bus: OptionalUnsetNone[int] = Noneable(IntegerValidator(min_value=0, allow_strings=True)), DefaultUnset
+
+    realtime_free_capacity: OptionalUnsetNone[int] = Noneable(IntegerValidator(min_value=0, allow_strings=True)), DefaultUnset
+    realtime_free_capacity_disabled: OptionalUnsetNone[int] = Noneable(IntegerValidator(min_value=0, allow_strings=True)), DefaultUnset
+    realtime_free_capacity_woman: OptionalUnsetNone[int] = Noneable(IntegerValidator(min_value=0, allow_strings=True)), DefaultUnset
+    realtime_free_capacity_family: OptionalUnsetNone[int] = Noneable(IntegerValidator(min_value=0, allow_strings=True)), DefaultUnset
+    realtime_free_capacity_charging: OptionalUnsetNone[int] = Noneable(IntegerValidator(min_value=0, allow_strings=True)), DefaultUnset
+    realtime_free_capacity_carsharing: OptionalUnsetNone[int] = Noneable(IntegerValidator(min_value=0, allow_strings=True)), DefaultUnset
+    realtime_free_capacity_truck: OptionalUnsetNone[int] = Noneable(IntegerValidator(min_value=0, allow_strings=True)), DefaultUnset
+    realtime_free_capacity_bus: OptionalUnsetNone[int] = Noneable(IntegerValidator(min_value=0, allow_strings=True)), DefaultUnset
```

### Comparing `parkapi_sources-0.2.0/src/parkapi_sources/models/source_info.py` & `parkapi_sources-0.3.0/src/parkapi_sources/models/source_info.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/src/parkapi_sources/models/xlsx_inputs.py` & `parkapi_sources-0.3.0/src/parkapi_sources/models/xlsx_inputs.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/src/parkapi_sources/parkapi_sources.py` & `parkapi_sources-0.3.0/src/parkapi_sources/parkapi_sources.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,21 +8,25 @@
 from .converters import (
     BahnV2PullConverter,
     BaseConverter,
     BfrkBwOepnvBikePushConverter,
     BfrkBwOepnvCarPushConverter,
     BfrkBwSpnvBikePushConverter,
     BfrkBwSpnvCarPushConverter,
+    BuchenPushConverter,
     FreiburgPullConverter,
     HeidelbergPullConverter,
     KarlsruhePullConverter,
-    MannheimPullConverter,
+    KienzlerPullConverter,
+    MannheimPushConverter,
+    NeckarsulmBikePushConverter,
     NeckarsulmPushConverter,
     PbwPullConverter,
     PforzheimPushConverter,
+    PumBwPushConverter,
     ReutlingenPushConverter,
     StuttgartPushConverter,
     UlmPullConverter,
     VrsParkAndRidePushConverter,
 )
 from .converters.base_converter.pull import PullConverter
 from .converters.base_converter.push import PushConverter
@@ -33,21 +37,25 @@
 class ParkAPISources:
     converter_classes: list[Type[BaseConverter]] = [
         BahnV2PullConverter,
         BfrkBwOepnvBikePushConverter,
         BfrkBwOepnvCarPushConverter,
         BfrkBwSpnvBikePushConverter,
         BfrkBwSpnvCarPushConverter,
+        BuchenPushConverter,
         FreiburgPullConverter,
         HeidelbergPullConverter,
         KarlsruhePullConverter,
-        MannheimPullConverter,
+        KienzlerPullConverter,
+        MannheimPushConverter,
+        NeckarsulmBikePushConverter,
         NeckarsulmPushConverter,
-        PforzheimPushConverter,
         PbwPullConverter,
+        PforzheimPushConverter,
+        PumBwPushConverter,
         ReutlingenPushConverter,
         StuttgartPushConverter,
         UlmPullConverter,
         VrsParkAndRidePushConverter,
     ]
     config_helper: ConfigHelper
     converter_by_uid: dict[str, BaseConverter]
```

### Comparing `parkapi_sources-0.2.0/src/parkapi_sources/scripts/parkapi.py` & `parkapi_sources-0.3.0/src/parkapi_sources/scripts/parkapi.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/src/parkapi_sources/util/encoding.py` & `parkapi_sources-0.3.0/src/parkapi_sources/util/encoding.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/src/parkapi_sources/util/xml_helper.py` & `parkapi_sources-0.3.0/src/parkapi_sources/util/xml_helper.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/src/parkapi_sources/validators/__init__.py` & `parkapi_sources-0.3.0/src/parkapi_sources/validators/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,10 +4,11 @@
 """
 
 from .boolean_validators import MappedBooleanValidator
 from .date_validator import ParsedDateValidator
 from .datetime_validator import Rfc1123DateTimeValidator, SpacedDateTimeValidator
 from .decimal_validators import GermanDecimalValidator
 from .integer_validators import GermanDurationIntegerValidator
+from .list_validator import PointCoordinateTupleValidator
 from .noneable import ExcelNoneable
 from .string_validators import NumberCastingStringValidator, ReplacingStringValidator
 from .time_validators import ExcelTimeValidator
```

### Comparing `parkapi_sources-0.2.0/src/parkapi_sources/validators/boolean_validators.py` & `parkapi_sources-0.3.0/src/parkapi_sources/validators/boolean_validators.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/src/parkapi_sources/validators/date_validator.py` & `parkapi_sources-0.3.0/src/parkapi_sources/validators/date_validator.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/src/parkapi_sources/validators/datetime_validator.py` & `parkapi_sources-0.3.0/src/parkapi_sources/validators/datetime_validator.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/src/parkapi_sources/validators/integer_validators.py` & `parkapi_sources-0.3.0/src/parkapi_sources/validators/integer_validators.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/src/parkapi_sources/validators/noneable.py` & `parkapi_sources-0.3.0/src/parkapi_sources/validators/noneable.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/src/parkapi_sources/validators/string_validators.py` & `parkapi_sources-0.3.0/src/parkapi_sources/validators/string_validators.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/src/parkapi_sources.egg-info/PKG-INFO` & `parkapi_sources-0.3.0/src/parkapi_sources.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parkapi_sources
-Version: 0.2.0
+Version: 0.3.0
 Summary: ParkAPI Sources is a collection of converters from several different data sources to normalized ParkAPI data.
 Author-email: "Ernesto Ruge, binary butterfly GmbH" <ernesto.ruge@binary-butterfly.de>
 Maintainer-email: "Ernesto Ruge, binary butterfly GmbH" <ernesto.ruge@binary-butterfly.de>
 Keywords: data,parking,converter,mobility,car,bike
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -43,22 +43,28 @@
 | name                                                                              | purpose | type        | uid                  | realtime |
 |-----------------------------------------------------------------------------------|---------|-------------|----------------------|----------|
 | Deutsche Bahn                                                                     | car     | pull        | `bahn_v2`            | no       |
 | Barrierefreie Reisekette Baden-Württemberg: PKW-Parkplätze an Bahnhöfen           | car     | push (csv)  | `bfrk_bw_oepnv_car`  | no       |
 | Barrierefreie Reisekette Baden-Württemberg: PKW-Parkplätze an Bushaltestellen     | car     | push (csv)  | `bfrk_bw_spnv_car`   | no       |
 | Barrierefreie Reisekette Baden-Württemberg: Fahrrad-Parkplätze an Bahnhöfen       | bike    | push (csv)  | `bfrk_bw_oepnv_bike` | no       |
 | Barrierefreie Reisekette Baden-Württemberg: Fahrrad-Parkplätze an Bushaltestellen | bike    | push (csv)  | `bfrk_bw_spnv_bike`  | no       |
+| Stadt Buchen                                                                      | car     | push (json) | `buchen`             | yes      |
 | Stadt Freiburg                                                                    | car     | pull        | `freiburg`           | yes      |
 | Stadt Heidelberg                                                                  | car     | pull        | `heidelberg`         | yes      |
 | Stadt Karlsruhe                                                                   | car     | pull        | `karlsruhe`          | yes      |
-| Stadt Mannheim                                                                    | car     | pull        | `mannheim`           | yes      |
+| Kienzler                                                                          | bike    | pull        | `kienzler`           | yes      |
+| Stadt Mannheim                                                                    | car     | push (json) | `mannheim`           | yes      |
+| Stadt Neckarsulm: PKW-Parkplätze                                                  | car     | pull        | `neckarsulm`         | no       |
+| Stadt Neckarsulm: Fahrrad-Abstellanlagen                                          | bike    | pull        | `neckarsulm_bike`    | no       |
 | Stadt Karlsruhe                                                                   | car     | push (csv)  | `neckarsulm`         | no       |
+| Baden-Württemberg: Parken und Mitfahren                                           | car     | push (xlsx) | `pum_bw`             | no       |
 | Parkraumgesellschaft Baden-Württemberg                                            | car     | pull        | `pbw`                | yes      |
 | Stadt Pforzheim                                                                   | car     | push (csv)  | `pforzheim`          | no       |
-| Stadt Reutlingen                                                                  | car     | push (csv)  | `reutlingen`         | no       |
+| Stadt Reutlingen: PKW-Parkplätze                                                  | car     | push (csv)  | `reutlingen`         | no       |
+| Stadt Reutlingen: Fahrrad-Abstellanlagen                                          | bike    | push (csv)  | `reutlingen_bike`    | no       |
 | Stadt Stuttgart                                                                   | car     | push (json) | `stuttgart`          | yes      |
 | Stadt Ulm                                                                         | car     | pull        | `ulm`                | yes      |
 | Verband Region Stuttgart: Park and Ride                                           | car     | pull        | `vrs_p_r`            | yes      |
 
 New converters for new sources are always welcome, please have a look at "Contribute" below.
 
 
@@ -212,14 +218,56 @@
 
 If you test a `PullConverter`, you will need no mock requests. This can be done using the fantastic
 [`requests_mock`](https://pypi.org/project/requests-mock/) library.
 
 If you created new validators, these should be tested with different inputs. Usually, `pytest.parametrize` is a nice approach to do this.
 
 
+### Migrate a converter
+
+If you want to migrate a v1 or v2 converter, you can re-use some of the code. There is a paradigm change, though: `parkapi-source-v3` 
+enforces a strict validation after transforming the data, while v1 and v2 converters don't. ParkAPI v1 / v2 converters are always pull
+converters, so the base class is always `PullConverter`.
+
+Instead of defining `POOL`, you will set `source_info` at the same place. Attributes are almost the same, except for `id` was renamed to 
+`uid`, and there is the new attribute `has_realtime_data`, which has to be set.
+
+ParkAPI v1 and v2 used two methods for static and realtime data, just as `parkapi-sources-v3`:
+
+- the old static data handling `def get_lot_infos(self) -> List[LotInfo]:` is
+  `get_static_parking_sites(self) -> tuple[list[StaticParkingSiteInput], list[ImportParkingSiteException]]:` in `parkapi-sources-v3`.
+- the old realtime data handling`def get_lot_data(self) -> List[LotData]:` is
+  `def get_realtime_parking_sites(self) -> tuple[list[RealtimeParkingSiteInput], list[ImportParkingSiteException]]:` in 
+  `parkapi-sources-v3`.
+
+The result objects have quite the same idea, too:
+
+- `LotInfo` gets `StaticParkingSiteInput`
+- `LotData` gets `RealtimeParkingSiteInput`
+
+There's also a helper for scraped content: before, there was `self.request_soup(self.POOL.public_url)` in order to get a `BeautifulSoup`
+element. Now, there is a helper mixin called `PullScraperMixin`. You can use it this way: 
+
+```
+class MyPullConverter(PullConverter, PullScraperMixin):
+```
+
+Additionally, there is another mixin for the GeoJSON files you already know from v1 and v2 converters: `StaticGeojsonDataMixin`. Using this,
+you can just define the static data method this way:
+
+```
+    def get_static_parking_sites(self) -> tuple[list[StaticParkingSiteInput], list[ImportParkingSiteException]]:
+        return self._get_static_parking_site_inputs_and_exceptions(source_uid=self.source_info.uid)
+```
+
+Afterwards, you can put the GeoJSON file to `/data`.
+
+Please keep in mind that you will have to add tests for the migrated scraper.
+
+
 ### Linting
 
 As we try to keep a consistent code style, please lint your code before creating the merge request. We use `black` and `ruff` for linting.
 There is Makefile target to do both: `make lint`. It runs the following commands:
 
 ```bash
 black ./src ./tests
```

### Comparing `parkapi_sources-0.2.0/src/parkapi_sources.egg-info/SOURCES.txt` & `parkapi_sources-0.3.0/src/parkapi_sources.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 .gitignore
+CHANGELOG.md
 LICENCE.txt
 Makefile
 README.md
 pyproject.toml
 requirements-dev.txt
 requirements.txt
 tox.ini
 .github/dependabot.yml
 .github/workflows/build-publish.yml
-.github/workflows/lint.yml
+.github/workflows/lint-test.yml
 data/freiburg.geojson
 data/heidelberg.geojson
 data/mannheim.geojson
 data/ulm.geojson
 dev/parkapi.py
 dev/test-pull-converter.py
 dev/test-push-converter.py
@@ -38,14 +39,15 @@
 src/parkapi_sources/converters/base_converter/pull/static_geojson_data_mixin/__init__.py
 src/parkapi_sources/converters/base_converter/pull/static_geojson_data_mixin/mixin.py
 src/parkapi_sources/converters/base_converter/pull/static_geojson_data_mixin/models.py
 src/parkapi_sources/converters/base_converter/push/__init__.py
 src/parkapi_sources/converters/base_converter/push/csv_converter.py
 src/parkapi_sources/converters/base_converter/push/json_converter.py
 src/parkapi_sources/converters/base_converter/push/normalized_xlsx_converter.py
+src/parkapi_sources/converters/base_converter/push/parkapi_json_converter.py
 src/parkapi_sources/converters/base_converter/push/push_converter.py
 src/parkapi_sources/converters/base_converter/push/xlsx_converter.py
 src/parkapi_sources/converters/base_converter/push/xml_converter.py
 src/parkapi_sources/converters/bfrk_bw/__init__.py
 src/parkapi_sources/converters/bfrk_bw/base_converter.py
 src/parkapi_sources/converters/bfrk_bw/base_models.py
 src/parkapi_sources/converters/bfrk_bw/bike_converter.py
@@ -58,29 +60,40 @@
 src/parkapi_sources/converters/heidelberg/__init__.py
 src/parkapi_sources/converters/heidelberg/converter.py
 src/parkapi_sources/converters/heidelberg/validators.py
 src/parkapi_sources/converters/karlsruhe/__init__.py
 src/parkapi_sources/converters/karlsruhe/converter.py
 src/parkapi_sources/converters/karlsruhe/models.py
 src/parkapi_sources/converters/karlsruhe/files/ca.crt.pem
-src/parkapi_sources/converters/mannheim/__init__.py
-src/parkapi_sources/converters/mannheim/converter.py
+src/parkapi_sources/converters/kienzler/__init__.py
+src/parkapi_sources/converters/kienzler/converter.py
+src/parkapi_sources/converters/kienzler/models.py
+src/parkapi_sources/converters/mannheim_buchen/__init__.py
+src/parkapi_sources/converters/mannheim_buchen/converter.py
+src/parkapi_sources/converters/mannheim_buchen/models.py
 src/parkapi_sources/converters/neckarsulm/__init__.py
 src/parkapi_sources/converters/neckarsulm/converter.py
 src/parkapi_sources/converters/neckarsulm/models.py
+src/parkapi_sources/converters/neckarsulm_bike/__init__.py
+src/parkapi_sources/converters/neckarsulm_bike/converter.py
 src/parkapi_sources/converters/pbw/__init__.py
 src/parkapi_sources/converters/pbw/converter.py
 src/parkapi_sources/converters/pbw/mapper.py
 src/parkapi_sources/converters/pbw/validation.py
 src/parkapi_sources/converters/pforzheim/__init__.py
 src/parkapi_sources/converters/pforzheim/converter.py
 src/parkapi_sources/converters/pforzheim/validation.py
+src/parkapi_sources/converters/pum_bw/__init__.py
+src/parkapi_sources/converters/pum_bw/converter.py
 src/parkapi_sources/converters/reutlingen/__init__.py
 src/parkapi_sources/converters/reutlingen/converter.py
 src/parkapi_sources/converters/reutlingen/validation.py
+src/parkapi_sources/converters/reutlingen_bike/__init__.py
+src/parkapi_sources/converters/reutlingen_bike/converter.py
+src/parkapi_sources/converters/reutlingen_bike/validation.py
 src/parkapi_sources/converters/stuttgart/__init__.py
 src/parkapi_sources/converters/stuttgart/converter.py
 src/parkapi_sources/converters/ulm/__init__.py
 src/parkapi_sources/converters/ulm/converter.py
 src/parkapi_sources/converters/vrs_p_r/__init__.py
 src/parkapi_sources/converters/vrs_p_r/vrs_p_r.py
 src/parkapi_sources/models/__init__.py
@@ -95,43 +108,53 @@
 src/parkapi_sources/util/xml_helper.py
 src/parkapi_sources/validators/__init__.py
 src/parkapi_sources/validators/boolean_validators.py
 src/parkapi_sources/validators/date_validator.py
 src/parkapi_sources/validators/datetime_validator.py
 src/parkapi_sources/validators/decimal_validators.py
 src/parkapi_sources/validators/integer_validators.py
+src/parkapi_sources/validators/list_validator.py
 src/parkapi_sources/validators/noneable.py
 src/parkapi_sources/validators/string_validators.py
 src/parkapi_sources/validators/time_validators.py
 tests/conftest.py
 tests/converters/bahn_v2_test.py
 tests/converters/bfrk_bw_test.py
 tests/converters/conftest.py
 tests/converters/freiburg_test.py
 tests/converters/heidelberg_test.py
 tests/converters/helper.py
 tests/converters/karlsruhe_test.py
-tests/converters/mannheim_test.py
+tests/converters/kienzler_test.py
+tests/converters/mannheim_buchen_test.py
+tests/converters/neckarsulm_bike_test.py
 tests/converters/neckarsulm_test.py
 tests/converters/pbw_test.py
 tests/converters/pforzheim_test.py
+tests/converters/pum_bw_test.py
+tests/converters/reutlingen_bike_test.py
 tests/converters/reutlingen_test.py
 tests/converters/stuttgart_test.py
 tests/converters/ulm_test.py
 tests/converters/vrs_p_r_test.py
 tests/converters/data/bahn_v2.json
 tests/converters/data/bfrk_bw_bike.csv
 tests/converters/data/bfrk_bw_car.csv
+tests/converters/data/buchen.json
 tests/converters/data/freiburg.json
 tests/converters/data/heidelberg.json
 tests/converters/data/karlsruhe.json
-tests/converters/data/mannheim.html
+tests/converters/data/kienzler.json
+tests/converters/data/mannheim.json
 tests/converters/data/neckarsulm.csv
+tests/converters/data/neckarsulm_bike.csv
 tests/converters/data/pforzheim.json
+tests/converters/data/pum_bw.xlsx
 tests/converters/data/reutlingen.csv
+tests/converters/data/reutlingen_bike.csv
 tests/converters/data/stuttgart-realtime.xml
 tests/converters/data/stuttgart-static.xml
 tests/converters/data/ulm.html
 tests/converters/data/vrs_p_r.xlsx
 tests/converters/data/pbw/catalog-city.json
 tests/converters/data/pbw/object-by-city-10.json
 tests/converters/data/pbw/object-by-city-11.json
```

### Comparing `parkapi_sources-0.2.0/tests/converters/bahn_v2_test.py` & `parkapi_sources-0.3.0/tests/converters/bahn_v2_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/tests/converters/bfrk_bw_test.py` & `parkapi_sources-0.3.0/tests/converters/bfrk_bw_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/tests/converters/conftest.py` & `parkapi_sources-0.3.0/tests/converters/conftest.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/tests/converters/data/bahn_v2.json` & `parkapi_sources-0.3.0/tests/converters/data/bahn_v2.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/tests/converters/data/bfrk_bw_bike.csv` & `parkapi_sources-0.3.0/tests/converters/data/bfrk_bw_bike.csv`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/tests/converters/data/bfrk_bw_car.csv` & `parkapi_sources-0.3.0/tests/converters/data/bfrk_bw_car.csv`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/tests/converters/data/freiburg.json` & `parkapi_sources-0.3.0/tests/converters/data/freiburg.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/tests/converters/data/heidelberg.json` & `parkapi_sources-0.3.0/tests/converters/data/heidelberg.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/tests/converters/data/karlsruhe.json` & `parkapi_sources-0.3.0/tests/converters/data/karlsruhe.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/tests/converters/data/neckarsulm.csv` & `parkapi_sources-0.3.0/tests/converters/data/neckarsulm.csv`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/tests/converters/data/pbw/catalog-city.json` & `parkapi_sources-0.3.0/tests/converters/data/pbw/catalog-city.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/tests/converters/data/pbw/object-by-city-10.json` & `parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-10.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/tests/converters/data/pbw/object-by-city-11.json` & `parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-11.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/tests/converters/data/pbw/object-by-city-12.json` & `parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-12.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/tests/converters/data/pbw/object-by-city-15.json` & `parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-15.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/tests/converters/data/pbw/object-by-city-17.json` & `parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-17.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/tests/converters/data/pbw/object-by-city-18.json` & `parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-18.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/tests/converters/data/pbw/object-by-city-19.json` & `parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-19.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/tests/converters/data/pbw/object-by-city-31.json` & `parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-31.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/tests/converters/data/pbw/object-by-city-32.json` & `parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-32.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/tests/converters/data/pbw/object-by-city-33.json` & `parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-33.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/tests/converters/data/pbw/object-by-city-34.json` & `parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-34.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/tests/converters/data/pbw/object-by-city-4.json` & `parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-4.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/tests/converters/data/pbw/object-by-city-42.json` & `parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-42.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/tests/converters/data/pbw/object-by-city-48.json` & `parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-48.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/tests/converters/data/pbw/object-by-city-49.json` & `parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-49.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/tests/converters/data/pbw/object-by-city-51.json` & `parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-51.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/tests/converters/data/pbw/object-by-city-52.json` & `parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-52.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/tests/converters/data/pbw/object-by-city-60.json` & `parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-60.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/tests/converters/data/pbw/object-by-city-61.json` & `parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-61.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/tests/converters/data/pbw/object-by-city-7.json` & `parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-7.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/tests/converters/data/pbw/object-by-city-71.json` & `parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-71.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/tests/converters/data/pbw/object-by-city-9.json` & `parkapi_sources-0.3.0/tests/converters/data/pbw/object-by-city-9.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/tests/converters/data/pbw/object-dynamic-all.json` & `parkapi_sources-0.3.0/tests/converters/data/pbw/object-dynamic-all.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/tests/converters/data/pforzheim.json` & `parkapi_sources-0.3.0/tests/converters/data/pforzheim.json`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/tests/converters/data/reutlingen.csv` & `parkapi_sources-0.3.0/tests/converters/data/reutlingen.csv`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/tests/converters/data/stuttgart-realtime.xml` & `parkapi_sources-0.3.0/tests/converters/data/stuttgart-realtime.xml`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/tests/converters/data/stuttgart-static.xml` & `parkapi_sources-0.3.0/tests/converters/data/stuttgart-static.xml`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/tests/converters/data/ulm.html` & `parkapi_sources-0.3.0/tests/converters/data/ulm.html`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/tests/converters/data/vrs_p_r.xlsx` & `parkapi_sources-0.3.0/tests/converters/data/vrs_p_r.xlsx`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/tests/converters/freiburg_test.py` & `parkapi_sources-0.3.0/tests/converters/freiburg_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/tests/converters/heidelberg_test.py` & `parkapi_sources-0.3.0/tests/converters/heidelberg_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/tests/converters/helper.py` & `parkapi_sources-0.3.0/tests/converters/helper.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/tests/converters/karlsruhe_test.py` & `parkapi_sources-0.3.0/tests/converters/karlsruhe_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/tests/converters/neckarsulm_test.py` & `parkapi_sources-0.3.0/tests/converters/neckarsulm_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/tests/converters/pbw_test.py` & `parkapi_sources-0.3.0/tests/converters/pbw_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/tests/converters/pforzheim_test.py` & `parkapi_sources-0.3.0/tests/converters/pforzheim_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/tests/converters/reutlingen_test.py` & `parkapi_sources-0.3.0/tests/converters/reutlingen_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,12 +21,11 @@
     @staticmethod
     def test_get_static_parking_sites(reutlingen_push_converter: ReutlingenPushConverter):
         with get_data_path('reutlingen.csv').open() as reutlingen_file:
             reutlingen_data = StringIO(reutlingen_file.read())
 
         static_parking_site_inputs, import_parking_site_exceptions = reutlingen_push_converter.handle_csv_string(reutlingen_data)
 
-        assert len(static_parking_site_inputs) > len(
-            import_parking_site_exceptions
-        ), 'There should be more valid then invalid parking sites'
+        assert len(static_parking_site_inputs) == 12, 'There should be 12 parking sites'
+        assert len(import_parking_site_exceptions) == 102, 'There should be 102 exceptions'
 
         validate_static_parking_site_inputs(static_parking_site_inputs)
```

### Comparing `parkapi_sources-0.2.0/tests/converters/stuttgart_test.py` & `parkapi_sources-0.3.0/tests/converters/stuttgart_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/tests/converters/ulm_test.py` & `parkapi_sources-0.3.0/tests/converters/ulm_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/tests/converters/vrs_p_r_test.py` & `parkapi_sources-0.3.0/tests/converters/vrs_p_r_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/tests/models/xlsx_inputs_test.py` & `parkapi_sources-0.3.0/tests/models/xlsx_inputs_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/tests/util/data_xml_helper.py` & `parkapi_sources-0.3.0/tests/util/data_xml_helper.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/tests/util/encoding_test.py` & `parkapi_sources-0.3.0/tests/util/encoding_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/tests/util/xml_helper_test.py` & `parkapi_sources-0.3.0/tests/util/xml_helper_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/tests/validators/boolean_validators_test.py` & `parkapi_sources-0.3.0/tests/validators/boolean_validators_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/tests/validators/date_validators_test.py` & `parkapi_sources-0.3.0/tests/validators/date_validators_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/tests/validators/datetime_validators_test.py` & `parkapi_sources-0.3.0/tests/validators/datetime_validators_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/tests/validators/integer_validators_test.py` & `parkapi_sources-0.3.0/tests/validators/integer_validators_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/tests/validators/noneable_tests.py` & `parkapi_sources-0.3.0/tests/validators/noneable_tests.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/tests/validators/string_validators_test.py` & `parkapi_sources-0.3.0/tests/validators/string_validators_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/tests/validators/time_validators_test.py` & `parkapi_sources-0.3.0/tests/validators/time_validators_test.py`

 * *Files identical despite different names*

### Comparing `parkapi_sources-0.2.0/tox.ini` & `parkapi_sources-0.3.0/tox.ini`

 * *Files identical despite different names*

