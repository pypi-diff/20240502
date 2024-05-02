# Comparing `tmp/traveltimepy-3.9.6.tar.gz` & `tmp/traveltimepy-3.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "traveltimepy-3.9.6.tar", last modified: Thu Apr 25 08:18:59 2024, max compression
+gzip compressed data, was "traveltimepy-3.9.7.tar", last modified: Thu May  2 14:40:39 2024, max compression
```

## Comparing `traveltimepy-3.9.6.tar` & `traveltimepy-3.9.7.tar`

### file list

```diff
@@ -1,86 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:18:59.268463 traveltimepy-3.9.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    32697 2024-04-25 08:18:59.268463 traveltimepy-3.9.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    32426 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:18:59.256463 traveltimepy-3.9.6/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/benchmarks/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/benchmarks/time_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/benchmarks/time_filter_fast.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/benchmarks/time_map.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-25 08:18:59.268463 traveltimepy-3.9.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:18:59.260463 traveltimepy-3.9.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/tests/distance_map_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/tests/geocoding_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/tests/map_info_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/tests/postcodes_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/tests/routes_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/tests/supported_locations.py
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/tests/time_filter_fast_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/tests/time_filter_proto_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/tests/time_filter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/tests/time_map_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/tests/wkt_parsing_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/tests/wkt_pretty_print_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/tests/wkt_validate_objects_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:18:59.260463 traveltimepy-3.9.6/traveltimepy/
--rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-04-25 08:18:51.000000 traveltimepy-3.9.6/traveltimepy/TimeFilterFastRequest_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-25 08:18:51.000000 traveltimepy-3.9.6/traveltimepy/TimeFilterFastResponse_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/accept_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:18:59.264463 traveltimepy-3.9.6/traveltimepy/dto/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/dto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/dto/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:18:59.264463 traveltimepy-3.9.6/traveltimepy/dto/requests/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/dto/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/dto/requests/distance_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/dto/requests/postcodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/dto/requests/postcodes_zones.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/dto/requests/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/dto/requests/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/dto/requests/supported_locations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/dto/requests/time_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/dto/requests/time_filter_fast.py
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/dto/requests/time_filter_proto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/dto/requests/time_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/dto/requests/time_map_geojson.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/dto/requests/time_map_wkt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:18:59.264463 traveltimepy-3.9.6/traveltimepy/dto/responses/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/dto/responses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/dto/responses/error.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/dto/responses/map_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/dto/responses/postcodes.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/dto/responses/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/dto/responses/supported_locations.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/dto/responses/time_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/dto/responses/time_filter_fast.py
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/dto/responses/time_filter_proto.py
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/dto/responses/time_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/dto/responses/time_map_wkt.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/dto/responses/zones.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/dto/transportation.py
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/http.py
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/itertools.py
--rw-r--r--   0 runner    (1001) docker     (127)    27981 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/proto_http.py
--rw-r--r--   0 runner    (1001) docker     (127)    21930 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:18:59.268463 traveltimepy-3.9.6/traveltimepy/wkt/
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/wkt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/wkt/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/wkt/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/wkt/geometries.py
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/wkt/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-04-25 08:18:44.000000 traveltimepy-3.9.6/traveltimepy/wkt/parsing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 08:18:59.260463 traveltimepy-3.9.6/traveltimepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    32697 2024-04-25 08:18:59.000000 traveltimepy-3.9.6/traveltimepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-04-25 08:18:59.000000 traveltimepy-3.9.6/traveltimepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 08:18:59.000000 traveltimepy-3.9.6/traveltimepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 08:18:59.000000 traveltimepy-3.9.6/traveltimepy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-25 08:18:59.000000 traveltimepy-3.9.6/traveltimepy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-25 08:18:59.000000 traveltimepy-3.9.6/traveltimepy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:40:39.538840 traveltimepy-3.9.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    32697 2024-05-02 14:40:39.538840 traveltimepy-3.9.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    32426 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:40:39.526840 traveltimepy-3.9.7/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/benchmarks/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/benchmarks/time_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/benchmarks/time_filter_fast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/benchmarks/time_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-02 14:40:39.538840 traveltimepy-3.9.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:40:39.530840 traveltimepy-3.9.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/tests/distance_map_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/tests/geocoding_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/tests/map_info_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/tests/postcodes_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/tests/routes_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/tests/supported_locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/tests/time_filter_fast_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/tests/time_filter_proto_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/tests/time_filter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5436 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/tests/time_map_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/tests/wkt_parsing_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/tests/wkt_pretty_print_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/tests/wkt_validate_objects_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:40:39.530840 traveltimepy-3.9.7/traveltimepy/
+-rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-05-02 14:40:30.000000 traveltimepy-3.9.7/traveltimepy/TimeFilterFastRequest_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-05-02 14:40:30.000000 traveltimepy-3.9.7/traveltimepy/TimeFilterFastResponse_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/traveltimepy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/traveltimepy/accept_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:40:39.534840 traveltimepy-3.9.7/traveltimepy/dto/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/traveltimepy/dto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/traveltimepy/dto/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:40:39.534840 traveltimepy-3.9.7/traveltimepy/dto/requests/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/traveltimepy/dto/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/traveltimepy/dto/requests/distance_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/traveltimepy/dto/requests/postcodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/traveltimepy/dto/requests/postcodes_zones.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/traveltimepy/dto/requests/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/traveltimepy/dto/requests/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/traveltimepy/dto/requests/supported_locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/traveltimepy/dto/requests/time_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/traveltimepy/dto/requests/time_filter_fast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/traveltimepy/dto/requests/time_filter_proto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/traveltimepy/dto/requests/time_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/traveltimepy/dto/requests/time_map_geojson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/traveltimepy/dto/requests/time_map_wkt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:40:39.538840 traveltimepy-3.9.7/traveltimepy/dto/responses/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/traveltimepy/dto/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/traveltimepy/dto/responses/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/traveltimepy/dto/responses/map_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/traveltimepy/dto/responses/postcodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/traveltimepy/dto/responses/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/traveltimepy/dto/responses/supported_locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/traveltimepy/dto/responses/time_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/traveltimepy/dto/responses/time_filter_fast.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/traveltimepy/dto/responses/time_filter_proto.py
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/traveltimepy/dto/responses/time_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/traveltimepy/dto/responses/time_map_wkt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/traveltimepy/dto/responses/zones.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/traveltimepy/dto/transportation.py
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/traveltimepy/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/traveltimepy/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/traveltimepy/itertools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27950 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/traveltimepy/mapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:40:39.538840 traveltimepy-3.9.7/traveltimepy/proto/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/traveltimepy/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/traveltimepy/proto_http.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22164 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/traveltimepy/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/traveltimepy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:40:39.538840 traveltimepy-3.9.7/traveltimepy/wkt/
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/traveltimepy/wkt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/traveltimepy/wkt/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/traveltimepy/wkt/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/traveltimepy/wkt/geometries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/traveltimepy/wkt/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-05-02 14:40:25.000000 traveltimepy-3.9.7/traveltimepy/wkt/parsing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:40:39.534840 traveltimepy-3.9.7/traveltimepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    32697 2024-05-02 14:40:39.000000 traveltimepy-3.9.7/traveltimepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-05-02 14:40:39.000000 traveltimepy-3.9.7/traveltimepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 14:40:39.000000 traveltimepy-3.9.7/traveltimepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 14:40:39.000000 traveltimepy-3.9.7/traveltimepy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-02 14:40:39.000000 traveltimepy-3.9.7/traveltimepy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-02 14:40:39.000000 traveltimepy-3.9.7/traveltimepy.egg-info/top_level.txt
```

### Comparing `traveltimepy-3.9.6/LICENSE` & `traveltimepy-3.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.6/PKG-INFO` & `traveltimepy-3.9.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: traveltimepy
-Version: 3.9.6
+Version: 3.9.7
 Summary: "Python Interface to Travel Time."
 Author: TravelTime
 License: MIT
 Keywords: traveltimepy,api,maps
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # Travel Time Python SDK
 
 [![PyPI version](https://badge.fury.io/py/traveltimepy.svg)](https://badge.fury.io/py/traveltimepy) [![Unit Tests](https://github.com/traveltime-dev/traveltime-python-sdk/actions/workflows/ci.yml/badge.svg)](https://github.com/traveltime-dev/traveltime-python-sdk/actions/workflows/ci.yml) [![Python support](https://img.shields.io/badge/python-3.8+-blue.svg)](https://img.shields.io/badge/python-3.8+-blue)
```

### Comparing `traveltimepy-3.9.6/README.md` & `traveltimepy-3.9.7/README.md`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.6/benchmarks/common.py` & `traveltimepy-3.9.7/benchmarks/common.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.6/benchmarks/time_filter.py` & `traveltimepy-3.9.7/benchmarks/time_filter.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.6/benchmarks/time_filter_fast.py` & `traveltimepy-3.9.7/benchmarks/time_filter_fast.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     ]
     return await sdk.time_filter_fast_async(
         locations=locations,
         search_ids=dict(search_ids),
         transportation=Transportation(type="driving"),
     )
 
+
 if __name__ == "__main__":
     start = time.perf_counter()
     response = asyncio.run(generate_matrix(50))
     request_time = time.perf_counter() - start
     print("Request completed in {0:.0f}s for matrix 50 * 50".format(request_time))
 
     start = time.perf_counter()
```

### Comparing `traveltimepy-3.9.6/benchmarks/time_map.py` & `traveltimepy-3.9.7/benchmarks/time_map.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.6/setup.cfg` & `traveltimepy-3.9.7/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -7,42 +7,51 @@
 keywords = traveltimepy, api, maps
 license = MIT
 author = TravelTime
 
 [options]
 zip_safe = False
 include_package_data = True
-python_requires = >=3.7
+python_requires = >=3.8
 packages = find_namespace:
 install_requires = 
 	pydantic
 	typing-extensions
 	geojson-pydantic >= 1.0.1
 	shapely
 	dacite
 	certifi >= 2021.5.30
 	aiohttp
 	aiolimiter
 	aiohttp-retry
 	protobuf == 4.21.12
+	types-protobuf
 
 [options.extras_require]
 test = 
 	pytest
 	pytest-asyncio
 	flake8
+	mypy
+	black
 
 [flake8]
 per-file-ignores = __init__.py:F401
 max-line-length = 88
 extend-ignore = 
 	E203,
 exclude = 
 	build/
 	venv/
-	traveltimepy/TimeFilterFastRequest_pb2.py
-	traveltimepy/TimeFilterFastResponse_pb2.py
+	traveltimepy/proto/
+
+[mypy]
+ignore_missing_imports = True
+exclude = ^(traveltimepy/proto/.*|build/.*|venv/.*)$
+
+[mypy-traveltimepy/proto.*]
+follow_imports = skip
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `traveltimepy-3.9.6/tests/conftest.py` & `traveltimepy-3.9.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.6/tests/distance_map_test.py` & `traveltimepy-3.9.7/tests/distance_map_test.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.6/tests/postcodes_test.py` & `traveltimepy-3.9.7/tests/postcodes_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,64 +1,64 @@
 import pytest
 from datetime import datetime
 
-from traveltimepy import Coordinates, PublicTransport
+from traveltimepy import Coordinates, PublicTransport, TravelTimeSdk
 
 
 @pytest.mark.asyncio
-async def test_departures(sdk):
+async def test_departures(sdk: TravelTimeSdk):
     results = await sdk.postcodes_async(
         coordinates=[Coordinates(lat=51.507609, lng=-0.128315)],
         departure_time=datetime.now(),
         transportation=PublicTransport(),
     )
     assert len(results) > 0
 
 
 @pytest.mark.asyncio
-async def test_arrivals(sdk):
+async def test_arrivals(sdk: TravelTimeSdk):
     results = await sdk.postcodes_async(
         coordinates=[Coordinates(lat=51.507609, lng=-0.128315)],
         arrival_time=datetime.now(),
         transportation=PublicTransport(),
     )
     assert len(results) > 0
 
 
 @pytest.mark.asyncio
-async def test_districts_departure(sdk):
+async def test_districts_departure(sdk: TravelTimeSdk):
     results = await sdk.postcodes_districts_async(
         coordinates=[Coordinates(lat=51.507609, lng=-0.128315)],
         departure_time=datetime.now(),
         transportation=PublicTransport(),
     )
     assert len(results) > 0
 
 
 @pytest.mark.asyncio
-async def test_districts_arrival(sdk):
+async def test_districts_arrival(sdk: TravelTimeSdk):
     results = await sdk.postcodes_districts_async(
         coordinates=[Coordinates(lat=51.507609, lng=-0.128315)],
         arrival_time=datetime.now(),
         transportation=PublicTransport(),
     )
     assert len(results) > 0
 
 
 @pytest.mark.asyncio
-async def test_sectors_departure(sdk):
+async def test_sectors_departure(sdk: TravelTimeSdk):
     results = await sdk.postcodes_sectors_async(
         coordinates=[Coordinates(lat=51.507609, lng=-0.128315)],
         departure_time=datetime.now(),
         transportation=PublicTransport(),
     )
     assert len(results) > 0
 
 
 @pytest.mark.asyncio
-async def test_sectors_arrival(sdk):
+async def test_sectors_arrival(sdk: TravelTimeSdk):
     results = await sdk.postcodes_sectors_async(
         coordinates=[Coordinates(lat=51.507609, lng=-0.128315)],
         arrival_time=datetime.now(),
         transportation=PublicTransport(),
     )
     assert len(results) > 0
```

### Comparing `traveltimepy-3.9.6/tests/routes_test.py` & `traveltimepy-3.9.7/tests/routes_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,64 +1,70 @@
 from typing import List
 
 import pytest
 from datetime import datetime
 
 from traveltimepy import PublicTransport, Driving, Location, Coordinates
 from traveltimepy.dto.common import SnapPenalty
+from traveltimepy.sdk import TravelTimeSdk
 
 
 @pytest.mark.asyncio
-async def test_departures(sdk, locations):
+async def test_departures(sdk: TravelTimeSdk, locations):
     results = await sdk.routes_async(
         locations=locations,
         search_ids={
             "London center": ["Hyde Park", "ZSL London Zoo"],
             "ZSL London Zoo": ["Hyde Park", "London center"],
         },
         transportation=PublicTransport(),
         departure_time=datetime.now(),
     )
     assert len(results) == 2
 
 
 @pytest.mark.asyncio
-async def test_arrivals(sdk, locations):
+async def test_arrivals(sdk: TravelTimeSdk, locations):
     results = await sdk.routes_async(
         locations=locations,
         search_ids={
             "London center": ["Hyde Park", "ZSL London Zoo"],
             "ZSL London Zoo": ["Hyde Park", "London center"],
         },
         transportation=PublicTransport(),
         departure_time=datetime.now(),
     )
     assert len(results) == 2
 
 
 @pytest.mark.asyncio
-async def test_snap_penalty(sdk):
+async def test_snap_penalty(sdk: TravelTimeSdk):
     locations: List[Location] = [
-            Location(id="A", coords=Coordinates(lat=53.806479, lng=-2.615711)),
-            Location(id="B", coords=Coordinates(lat=53.810129, lng=-2.601099)),
-        ]
+        Location(id="A", coords=Coordinates(lat=53.806479, lng=-2.615711)),
+        Location(id="B", coords=Coordinates(lat=53.810129, lng=-2.601099)),
+    ]
     result_with_penalty = await sdk.routes_async(
         locations=locations,
         search_ids={
             "A": ["B"],
         },
         transportation=Driving(),
         departure_time=datetime.now(),
     )
-    traveltime_with_penalty = result_with_penalty[0].locations[0].properties[0].travel_time
+    traveltime_with_penalty = (
+        result_with_penalty[0].locations[0].properties[0].travel_time
+    )
     result_without_penalty = await sdk.routes_async(
         locations=locations,
         search_ids={
             "A": ["B"],
         },
         transportation=Driving(),
         departure_time=datetime.now(),
-        snap_penalty=SnapPenalty.DISABLED
+        snap_penalty=SnapPenalty.DISABLED,
     )
-    traveltime_without_penalty = result_without_penalty[0].locations[0].properties[0].travel_time
-
+    traveltime_without_penalty = (
+        result_without_penalty[0].locations[0].properties[0].travel_time
+    )
+    assert traveltime_with_penalty is not None
+    assert traveltime_without_penalty is not None
     assert traveltime_with_penalty > traveltime_without_penalty
```

### Comparing `traveltimepy-3.9.6/tests/supported_locations.py` & `traveltimepy-3.9.7/tests/supported_locations.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pytest
 
-from traveltimepy import Location, Coordinates
+from traveltimepy import Location, Coordinates, TravelTimeSdk
 
 
 @pytest.mark.asyncio
-async def test_supported_locations(sdk):
+async def test_supported_locations(sdk: TravelTimeSdk):
     locations = [
         Location(id="Kaunas", coords=Coordinates(lat=54.900008, lng=23.957734)),
         Location(id="London", coords=Coordinates(lat=51.506756, lng=-0.12805)),
         Location(id="Bangkok", coords=Coordinates(lat=13.761866, lng=100.544818)),
         Location(id="Lisbon", coords=Coordinates(lat=38.721869, lng=-9.138549)),
         Location(id="Unsupported", coords=Coordinates(lat=68.721869, lng=-9.138549)),
     ]
```

### Comparing `traveltimepy-3.9.6/tests/time_filter_fast_test.py` & `traveltimepy-3.9.7/tests/time_filter_test.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import pytest
+from datetime import datetime
 
-from traveltimepy.dto.requests.time_filter_fast import Transportation
+from traveltimepy import PublicTransport, TravelTimeSdk
 
 
 @pytest.mark.asyncio
-async def test_one_to_many(sdk, locations):
-    results = await sdk.time_filter_fast_async(
+async def test_departures(sdk: TravelTimeSdk, locations):
+    results = await sdk.time_filter_async(
         locations=locations,
         search_ids={
             "London center": ["Hyde Park", "ZSL London Zoo"],
             "ZSL London Zoo": ["Hyde Park", "London center"],
         },
-        transportation=Transportation(type="public_transport"),
+        transportation=PublicTransport(),
+        departure_time=datetime.now(),
     )
-
-    assert len(results) > 0
+    assert len(results) == 2
 
 
 @pytest.mark.asyncio
-async def test_many_to_one(sdk, locations):
-    results = await sdk.time_filter_fast_async(
+async def test_arrivals(sdk: TravelTimeSdk, locations):
+    results = await sdk.time_filter_async(
         locations=locations,
         search_ids={
             "London center": ["Hyde Park", "ZSL London Zoo"],
             "ZSL London Zoo": ["Hyde Park", "London center"],
         },
-        transportation=Transportation(type="public_transport"),
-        one_to_many=False,
+        transportation=PublicTransport(),
+        departure_time=datetime.now(),
     )
-
-    assert len(results) > 0
+    assert len(results) == 2
```

### Comparing `traveltimepy-3.9.6/tests/time_filter_proto_test.py` & `traveltimepy-3.9.7/tests/time_filter_proto_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,33 +2,34 @@
 
 from traveltimepy import Coordinates
 from traveltimepy.dto.common import PropertyProto
 from traveltimepy.dto.requests.time_filter_proto import (
     ProtoTransportation,
     ProtoCountry,
 )
+from traveltimepy.sdk import TravelTimeSdk
 
 
 @pytest.mark.asyncio
-async def test_one_to_many(proto_sdk):
+async def test_one_to_many(proto_sdk: TravelTimeSdk):
     results = await proto_sdk.time_filter_proto_async(
         origin=Coordinates(lat=51.425709, lng=-0.122061),
         destinations=[
             Coordinates(lat=51.348605, lng=-0.314783),
             Coordinates(lat=51.337205, lng=-0.315793),
         ],
         transportation=ProtoTransportation.DRIVING_FERRY,
         travel_time=7200,
         country=ProtoCountry.UNITED_KINGDOM,
     )
     assert len(results.travel_times) == 2 and len(results.distances) == 0
 
 
 @pytest.mark.asyncio
-async def test_many_to_one(proto_sdk):
+async def test_many_to_one(proto_sdk: TravelTimeSdk):
     results = await proto_sdk.time_filter_proto_async(
         origin=Coordinates(lat=51.425709, lng=-0.122061),
         destinations=[
             Coordinates(lat=51.348605, lng=-0.314783),
             Coordinates(lat=51.337205, lng=-0.315793),
         ],
         transportation=ProtoTransportation.DRIVING_FERRY,
@@ -36,15 +37,15 @@
         country=ProtoCountry.UNITED_KINGDOM,
         one_to_many=False,
     )
     assert len(results.travel_times) == 2 and len(results.distances) == 0
 
 
 @pytest.mark.asyncio
-async def test_one_to_many_with_distances(proto_sdk):
+async def test_one_to_many_with_distances(proto_sdk: TravelTimeSdk):
     results = await proto_sdk.time_filter_proto_async(
         origin=Coordinates(lat=51.425709, lng=-0.122061),
         destinations=[
             Coordinates(lat=51.348605, lng=-0.314783),
             Coordinates(lat=51.337205, lng=-0.315793),
         ],
         transportation=ProtoTransportation.DRIVING_FERRY,
@@ -52,15 +53,15 @@
         country=ProtoCountry.UNITED_KINGDOM,
         properties=[PropertyProto.DISTANCE],
     )
     assert len(results.travel_times) == 2 and len(results.distances) == 2
 
 
 @pytest.mark.asyncio
-async def test_many_to_one_with_distances(proto_sdk):
+async def test_many_to_one_with_distances(proto_sdk: TravelTimeSdk):
     results = await proto_sdk.time_filter_proto_async(
         origin=Coordinates(lat=51.425709, lng=-0.122061),
         destinations=[
             Coordinates(lat=51.348605, lng=-0.314783),
             Coordinates(lat=51.337205, lng=-0.315793),
         ],
         transportation=ProtoTransportation.DRIVING_FERRY,
```

### Comparing `traveltimepy-3.9.6/tests/time_filter_test.py` & `traveltimepy-3.9.7/tests/time_filter_fast_test.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import pytest
-from datetime import datetime
 
-from traveltimepy import PublicTransport
+from traveltimepy import Transportation, TravelTimeSdk
 
 
 @pytest.mark.asyncio
-async def test_departures(sdk, locations):
-    results = await sdk.time_filter_async(
+async def test_one_to_many(sdk: TravelTimeSdk, locations):
+    results = await sdk.time_filter_fast_async(
         locations=locations,
         search_ids={
             "London center": ["Hyde Park", "ZSL London Zoo"],
             "ZSL London Zoo": ["Hyde Park", "London center"],
         },
-        transportation=PublicTransport(),
-        departure_time=datetime.now(),
+        transportation=Transportation(type="public_transport"),
     )
-    assert len(results) == 2
+
+    assert len(results) > 0
 
 
 @pytest.mark.asyncio
-async def test_arrivals(sdk, locations):
-    results = await sdk.time_filter_async(
+async def test_many_to_one(sdk: TravelTimeSdk, locations):
+    results = await sdk.time_filter_fast_async(
         locations=locations,
         search_ids={
             "London center": ["Hyde Park", "ZSL London Zoo"],
             "ZSL London Zoo": ["Hyde Park", "London center"],
         },
-        transportation=PublicTransport(),
-        departure_time=datetime.now(),
+        transportation=Transportation(type="public_transport"),
+        one_to_many=False,
     )
-    assert len(results) == 2
+
+    assert len(results) > 0
```

### Comparing `traveltimepy-3.9.6/tests/time_map_test.py` & `traveltimepy-3.9.7/tests/time_map_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pytest
 from datetime import datetime
 
-from traveltimepy import Coordinates, Driving, LevelOfDetail, Range
+from traveltimepy import Coordinates, Driving, LevelOfDetail, Range, TravelTimeSdk
 
 
 @pytest.mark.asyncio
-async def test_departures(sdk):
+async def test_departures(sdk: TravelTimeSdk):
     results = await sdk.time_map_async(
         coordinates=[
             Coordinates(lat=51.507609, lng=-0.128315),
             Coordinates(lat=51.517609, lng=-0.138315),
         ],
         departure_time=datetime.now(),
         travel_time=900,
@@ -17,15 +17,15 @@
         search_range=Range(enabled=True, width=1800),
         level_of_detail=LevelOfDetail(scale_type="simple", level="lowest"),
     )
     assert len(results) == 2
 
 
 @pytest.mark.asyncio
-async def test_departures_geojson(sdk):
+async def test_departures_geojson(sdk: TravelTimeSdk):
     results = await sdk.time_map_geojson_async(
         coordinates=[
             Coordinates(lat=51.507609, lng=-0.128315),
             Coordinates(lat=51.517609, lng=-0.138315),
         ],
         departure_time=datetime.now(),
         travel_time=900,
@@ -33,15 +33,15 @@
         search_range=Range(enabled=True, width=1800),
         level_of_detail=LevelOfDetail(scale_type="simple", level="lowest"),
     )
     assert len(results) == 2
 
 
 @pytest.mark.asyncio
-async def test_departures_wkt(sdk):
+async def test_departures_wkt(sdk: TravelTimeSdk):
     response = await sdk.time_map_wkt_async(
         coordinates=[
             Coordinates(lat=51.507609, lng=-0.128315),
             Coordinates(lat=51.517609, lng=-0.138315),
         ],
         departure_time=datetime.now(),
         travel_time=900,
@@ -49,15 +49,15 @@
         search_range=Range(enabled=True, width=1800),
         level_of_detail=LevelOfDetail(scale_type="simple", level="lowest"),
     )
     assert len(response.results) == 2
 
 
 @pytest.mark.asyncio
-async def test_departures_wkt_no_holes(sdk):
+async def test_departures_wkt_no_holes(sdk: TravelTimeSdk):
     response = await sdk.time_map_wkt_no_holes_async(
         coordinates=[
             Coordinates(lat=51.507609, lng=-0.128315),
             Coordinates(lat=51.517609, lng=-0.138315),
         ],
         departure_time=datetime.now(),
         travel_time=900,
@@ -65,15 +65,15 @@
         search_range=Range(enabled=True, width=1800),
         level_of_detail=LevelOfDetail(scale_type="simple", level="lowest"),
     )
     assert len(response.results) == 2
 
 
 @pytest.mark.asyncio
-async def test_arrivals(sdk):
+async def test_arrivals(sdk: TravelTimeSdk):
     results = await sdk.time_map_async(
         coordinates=[
             Coordinates(lat=51.507609, lng=-0.128315),
             Coordinates(lat=51.517609, lng=-0.138315),
         ],
         arrival_time=datetime.now(),
         travel_time=900,
@@ -81,15 +81,15 @@
         search_range=Range(enabled=True, width=1800),
         level_of_detail=LevelOfDetail(scale_type="simple", level="lowest"),
     )
     assert len(results) == 2
 
 
 @pytest.mark.asyncio
-async def test_arrivals_geojson(sdk):
+async def test_arrivals_geojson(sdk: TravelTimeSdk):
     results = await sdk.time_map_geojson_async(
         coordinates=[
             Coordinates(lat=51.507609, lng=-0.128315),
             Coordinates(lat=51.517609, lng=-0.138315),
         ],
         arrival_time=datetime.now(),
         travel_time=900,
@@ -97,15 +97,15 @@
         search_range=Range(enabled=True, width=1800),
         level_of_detail=LevelOfDetail(scale_type="simple", level="lowest"),
     )
     assert len(results) == 2
 
 
 @pytest.mark.asyncio
-async def test_arrivals_wkt(sdk):
+async def test_arrivals_wkt(sdk: TravelTimeSdk):
     response = await sdk.time_map_wkt_async(
         coordinates=[
             Coordinates(lat=51.507609, lng=-0.128315),
             Coordinates(lat=51.517609, lng=-0.138315),
         ],
         arrival_time=datetime.now(),
         travel_time=900,
@@ -113,15 +113,15 @@
         search_range=Range(enabled=True, width=1800),
         level_of_detail=LevelOfDetail(scale_type="simple", level="lowest"),
     )
     assert len(response.results) == 2
 
 
 @pytest.mark.asyncio
-async def test_arrivals_wkt_no_holes(sdk):
+async def test_arrivals_wkt_no_holes(sdk: TravelTimeSdk):
     response = await sdk.time_map_wkt_no_holes_async(
         coordinates=[
             Coordinates(lat=51.507609, lng=-0.128315),
             Coordinates(lat=51.517609, lng=-0.138315),
         ],
         arrival_time=datetime.now(),
         travel_time=900,
@@ -129,15 +129,15 @@
         search_range=Range(enabled=True, width=1800),
         level_of_detail=LevelOfDetail(scale_type="simple", level="lowest"),
     )
     assert len(response.results) == 2
 
 
 @pytest.mark.asyncio
-async def test_union_departures(sdk):
+async def test_union_departures(sdk: TravelTimeSdk):
     result = await sdk.union_async(
         coordinates=[
             Coordinates(lat=51.507609, lng=-0.128315),
             Coordinates(lat=51.517609, lng=-0.138315),
         ],
         departure_time=datetime.now(),
         travel_time=900,
@@ -145,15 +145,15 @@
         search_range=Range(enabled=True, width=1800),
         level_of_detail=LevelOfDetail(scale_type="simple", level="lowest"),
     )
     assert len(result.shapes) > 0
 
 
 @pytest.mark.asyncio
-async def test_intersection_arrivals(sdk):
+async def test_intersection_arrivals(sdk: TravelTimeSdk):
     result = await sdk.intersection_async(
         coordinates=[
             Coordinates(lat=51.507609, lng=-0.128315),
             Coordinates(lat=51.517609, lng=-0.138315),
         ],
         arrival_time=datetime.now(),
         travel_time=900,
```

### Comparing `traveltimepy-3.9.6/tests/wkt_parsing_test.py` & `traveltimepy-3.9.7/tests/wkt_parsing_test.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.6/tests/wkt_pretty_print_test.py` & `traveltimepy-3.9.7/tests/wkt_pretty_print_test.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.6/tests/wkt_validate_objects_test.py` & `traveltimepy-3.9.7/tests/wkt_validate_objects_test.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.6/traveltimepy/TimeFilterFastRequest_pb2.py` & `traveltimepy-3.9.7/traveltimepy/TimeFilterFastRequest_pb2.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.6/traveltimepy/TimeFilterFastResponse_pb2.py` & `traveltimepy-3.9.7/traveltimepy/TimeFilterFastResponse_pb2.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.6/traveltimepy/__init__.py` & `traveltimepy-3.9.7/traveltimepy/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,14 @@
     PublicTransport,
     Driving,
     Ferry,
     Walking,
     Cycling,
     DrivingTrain,
     CyclingPublicTransport,
-    MaxChanges,
 )
 from traveltimepy.dto.requests.time_filter_proto import (
     ProtoTransportation,
     ProtoCountry,
 )
 from traveltimepy.dto.common import (
     Coordinates,
```

### Comparing `traveltimepy-3.9.6/traveltimepy/dto/common.py` & `traveltimepy-3.9.7/traveltimepy/dto/common.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.6/traveltimepy/dto/requests/distance_map.py` & `traveltimepy-3.9.7/traveltimepy/dto/requests/distance_map.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,16 +67,16 @@
     id: str
     search_ids: List[str]
 
 
 class DistanceMapRequest(TravelTimeRequest[TimeMapResponse]):
     departure_searches: List[DepartureSearch]
     arrival_searches: List[ArrivalSearch]
-    unions: List[Union] = None
-    intersections: List[Intersection] = None
+    unions: List[Union]
+    intersections: List[Intersection]
 
     def split_searches(self, window_size: int) -> List[TravelTimeRequest]:
         return [
             DistanceMapRequest(
                 departure_searches=departures,
                 arrival_searches=arrivals,
                 unions=self.unions,
```

### Comparing `traveltimepy-3.9.6/traveltimepy/dto/requests/postcodes.py` & `traveltimepy-3.9.7/traveltimepy/dto/requests/postcodes.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.6/traveltimepy/dto/requests/postcodes_zones.py` & `traveltimepy-3.9.7/traveltimepy/dto/requests/postcodes_zones.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.6/traveltimepy/dto/requests/routes.py` & `traveltimepy-3.9.7/traveltimepy/dto/requests/routes.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.6/traveltimepy/dto/requests/supported_locations.py` & `traveltimepy-3.9.7/traveltimepy/dto/requests/supported_locations.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.6/traveltimepy/dto/requests/time_filter.py` & `traveltimepy-3.9.7/traveltimepy/dto/requests/time_filter.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.6/traveltimepy/dto/requests/time_filter_fast.py` & `traveltimepy-3.9.7/traveltimepy/dto/requests/time_filter_fast.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     id: str
     departure_location_id: str
     arrival_location_ids: List[str]
     transportation: Transportation
     travel_time: int
     arrival_time_period: str
     properties: List[Property]
-    snap_penalty: Optional[SnapPenalty] = None,
+    snap_penalty: Optional[SnapPenalty] = None
 
 
 class ManyToOne(BaseModel):
     id: str
     arrival_location_id: str
     departure_location_ids: List[str]
     transportation: Transportation
```

### Comparing `traveltimepy-3.9.6/traveltimepy/dto/requests/time_filter_proto.py` & `traveltimepy-3.9.7/traveltimepy/dto/requests/time_filter_proto.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.6/traveltimepy/dto/requests/time_map.py` & `traveltimepy-3.9.7/traveltimepy/dto/requests/time_map.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,16 +70,16 @@
     id: str
     search_ids: List[str]
 
 
 class TimeMapRequest(TravelTimeRequest[TimeMapResponse]):
     departure_searches: List[DepartureSearch]
     arrival_searches: List[ArrivalSearch]
-    unions: List[Union] = None
-    intersections: List[Intersection] = None
+    unions: List[Union]
+    intersections: List[Intersection]
     snap_penalty: Optional[SnapPenalty] = None
 
     def split_searches(self, window_size: int) -> List[TravelTimeRequest]:
         return [
             TimeMapRequest(
                 departure_searches=departures,
                 arrival_searches=arrivals,
```

### Comparing `traveltimepy-3.9.6/traveltimepy/dto/requests/time_map_geojson.py` & `traveltimepy-3.9.7/traveltimepy/dto/requests/time_map_geojson.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 from typing import List
 
 from geojson_pydantic import FeatureCollection
 from traveltimepy.dto.requests.request import TravelTimeRequest
 from traveltimepy.dto.requests.time_map import (
-    TimeMapRequest,
     DepartureSearch,
     ArrivalSearch,
 )
 from traveltimepy.itertools import split, flatten
 
 
 class TimeMapRequestGeojson(TravelTimeRequest[FeatureCollection]):
     departure_searches: List[DepartureSearch]
     arrival_searches: List[ArrivalSearch]
 
     def split_searches(self, window_size: int) -> List[TravelTimeRequest]:
         return [
-            TimeMapRequest(
+            TimeMapRequestGeojson(
                 departure_searches=departures,
                 arrival_searches=arrivals,
             )
             for departures, arrivals in split(
                 self.departure_searches, self.arrival_searches, window_size
             )
         ]
```

### Comparing `traveltimepy-3.9.6/traveltimepy/dto/requests/time_map_wkt.py` & `traveltimepy-3.9.7/traveltimepy/dto/requests/time_map_wkt.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.6/traveltimepy/dto/responses/routes.py` & `traveltimepy-3.9.7/traveltimepy/dto/responses/routes.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.6/traveltimepy/dto/responses/time_filter.py` & `traveltimepy-3.9.7/traveltimepy/dto/responses/time_filter.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.6/traveltimepy/dto/responses/time_filter_fast.py` & `traveltimepy-3.9.7/traveltimepy/dto/responses/time_filter_fast.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.6/traveltimepy/dto/responses/time_map_wkt.py` & `traveltimepy-3.9.7/traveltimepy/dto/responses/time_map_wkt.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from typing import List, Union, Dict, Any, TypeVar, Optional
+from typing import Generic, List, Union, Dict, Any, TypeVar, Optional
 from pydantic import field_validator, BaseModel, Field
 
 from traveltimepy.wkt import WKTObject, parse_wkt
 from traveltimepy.wkt.helper import print_indented
 
 Props = TypeVar("Props", bound=Union[Dict[str, Any], BaseModel])
 
 
-class TimeMapWKTResult(BaseModel):
+class TimeMapWKTResult(BaseModel, Generic[Props]):
     search_id: str
     shape: WKTObject
     properties: Optional[Props] = Field(None)
 
     @field_validator("shape", mode="before")
     @classmethod
     def transform_shape(cls, shape: str) -> WKTObject:
```

### Comparing `traveltimepy-3.9.6/traveltimepy/dto/responses/zones.py` & `traveltimepy-3.9.7/traveltimepy/dto/responses/zones.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.6/traveltimepy/dto/transportation.py` & `traveltimepy-3.9.7/traveltimepy/dto/transportation.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.6/traveltimepy/http.py` & `traveltimepy-3.9.7/traveltimepy/http.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import asyncio
 import json
 from dataclasses import dataclass
-from typing import TypeVar, Type, Dict
+from typing import TypeVar, Type, Dict, Optional
 
 from aiohttp import ClientSession, ClientResponse, TCPConnector, ClientTimeout
+from pydantic import BaseModel
 from traveltimepy.dto.requests.request import TravelTimeRequest
 
 from traveltimepy.dto.responses.error import ResponseError
 from traveltimepy.errors import ApiError
 from aiohttp_retry import RetryClient, ExponentialRetry
 from aiolimiter import AsyncLimiter
 
-T = TypeVar("T")
+T = TypeVar("T", bound=BaseModel)
 DEFAULT_SPLIT_SIZE = 10
 
 
 @dataclass
 class SdkParams:
     host: str
     proto_host: str
@@ -31,15 +32,17 @@
     response_class: Type[T],
     url: str,
     headers: Dict[str, str],
     request: TravelTimeRequest,
     rate_limit: AsyncLimiter,
 ) -> T:
     async with rate_limit:
-        async with client.post(url=url, headers=headers, data=request.json()) as resp:
+        async with client.post(
+            url=url, headers=headers, data=request.model_dump_json()
+        ) as resp:
             return await _process_response(response_class, resp)
 
 
 async def send_post_async(
     response_class: Type[T],
     path: str,
     headers: Dict[str, str],
@@ -81,15 +84,15 @@
 
 
 async def send_get_async(
     response_class: Type[T],
     path: str,
     headers: Dict[str, str],
     sdk_params: SdkParams,
-    params: Dict[str, str] = None,
+    params: Optional[Dict[str, str]],
 ) -> T:
     async with ClientSession(
         timeout=ClientTimeout(total=sdk_params.timeout),
         connector=TCPConnector(ssl=False),
     ) as session:
         retry_options = ExponentialRetry(attempts=sdk_params.retry_attempts)
         async with RetryClient(
@@ -112,8 +115,8 @@
             f"Travel Time API request failed: {parsed.description}\n"
             f"Error code: {parsed.error_code}\n"
             f"Additional info: {parsed.additional_info}\n"
             f"<{parsed.documentation_link}>\n"
         )
         raise ApiError(msg)
     else:
-        return response_class.parse_obj(json_data)
+        return response_class.model_validate(json_data)
```

### Comparing `traveltimepy-3.9.6/traveltimepy/itertools.py` & `traveltimepy-3.9.7/traveltimepy/itertools.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 R = TypeVar("R")
 
 
 def sliding(values: List[T], window_size: int) -> List[List[T]]:
     return [values[i : i + window_size] for i in range(0, len(values), window_size)]
 
 
-def split(left: List[T], right: List[R], window_size: int) -> List[List[Tuple[T, R]]]:
+def split(
+    left: List[T], right: List[R], window_size: int
+) -> List[Tuple[List[T], List[R]]]:
     return list(
         itertools.zip_longest(
             sliding(left, window_size), sliding(right, window_size), fillvalue=[]
         )
     )
```

### Comparing `traveltimepy-3.9.6/traveltimepy/mapper.py` & `traveltimepy-3.9.7/traveltimepy/mapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import math
 from typing import Dict, Union, List, Optional
 
 from traveltimepy.dto.requests.distance_map import DistanceMapRequest
 from traveltimepy.dto.requests.time_map_geojson import TimeMapRequestGeojson
 from traveltimepy.dto.requests.time_map_wkt import TimeMapWKTRequest
 from traveltimepy.errors import ApiError
-from traveltimepy import TimeFilterFastRequest_pb2
+from traveltimepy.proto import TimeFilterFastRequest_pb2
 
 from traveltimepy.dto.common import (
     Location,
     Coordinates,
     FullRange,
     Property,
     Range,
@@ -480,39 +480,35 @@
                     id=f"Search {ind}",
                     coords=cur_coordinates,
                     travel_time=travel_time,
                     arrival_time=time_info.value,
                     transportation=transportation,
                     range=search_range,
                     level_of_detail=level_of_detail,
-                    snap_penalty=snap_penalty
+                    snap_penalty=snap_penalty,
                 )
                 for ind, cur_coordinates in enumerate(coordinates)
             ],
             departure_searches=[],
-            unions=[],
-            intersections=[],
         )
     elif isinstance(time_info, DepartureTime):
         return TimeMapWKTRequest(
             departure_searches=[
                 time_map.DepartureSearch(
                     id=f"Search {ind}",
                     coords=cur_coordinates,
                     travel_time=travel_time,
                     departure_time=time_info.value,
                     transportation=transportation,
                     range=search_range,
-                    snap_penalty=snap_penalty
+                    snap_penalty=snap_penalty,
                 )
                 for ind, cur_coordinates in enumerate(coordinates)
             ],
             arrival_searches=[],
-            unions=[],
-            intersections=[],
         )
     else:
         raise ApiError("arrival_time or departure_time should be specified")
 
 
 def create_distance_map(
     coordinates: List[Coordinates],
@@ -594,15 +590,15 @@
                     id=f"Search {ind}",
                     coords=cur_coordinates,
                     travel_time=travel_time,
                     arrival_time=time_info.value,
                     transportation=transportation,
                     range=search_range,
                     level_of_detail=level_of_detail,
-                    snap_penalty=snap_penalty
+                    snap_penalty=snap_penalty,
                 )
                 for ind, cur_coordinates in enumerate(coordinates)
             ],
             departure_searches=[],
             unions=[],
             intersections=[
                 time_map.Intersection(
@@ -618,15 +614,15 @@
                     id=f"Search {ind}",
                     coords=cur_coordinates,
                     travel_time=travel_time,
                     departure_time=time_info.value,
                     transportation=transportation,
                     range=search_range,
                     level_of_detail=level_of_detail,
-                    snap_penalty=snap_penalty
+                    snap_penalty=snap_penalty,
                 )
                 for ind, cur_coordinates in enumerate(coordinates)
             ],
             arrival_searches=[],
             unions=[],
             intersections=[
                 time_map.Intersection(
@@ -687,15 +683,15 @@
                     id=f"Search {ind}",
                     coords=cur_coordinates,
                     travel_time=travel_time,
                     departure_time=time_info.value,
                     transportation=transportation,
                     range=search_range,
                     level_of_detail=level_of_detail,
-                    snap_penalty=snap_penalty
+                    snap_penalty=snap_penalty,
                 )
                 for ind, cur_coordinates in enumerate(coordinates)
             ],
             arrival_searches=[],
             unions=[
                 time_map.Union(
                     id="Union search",
@@ -772,25 +768,25 @@
 def create_proto_request(
     origin: Coordinates,
     destinations: List[Coordinates],
     transportation: ProtoTransportation,
     properties: Optional[List[PropertyProto]],
     travel_time: int,
     one_to_many: bool = True,
-) -> TimeFilterFastRequest_pb2.TimeFilterFastRequest:
-    request = TimeFilterFastRequest_pb2.TimeFilterFastRequest()
+) -> TimeFilterFastRequest_pb2.TimeFilterFastRequest:  # type: ignore
+    request = TimeFilterFastRequest_pb2.TimeFilterFastRequest()  # type: ignore
 
     if one_to_many:
         request.oneToManyRequest.departureLocation.lat = origin.lat
         request.oneToManyRequest.departureLocation.lng = origin.lng
 
         request.oneToManyRequest.transportation.type = transportation.value.code
         request.oneToManyRequest.travelTime = travel_time
         request.oneToManyRequest.arrivalTimePeriod = (
-            TimeFilterFastRequest_pb2.TimePeriod.WEEKDAY_MORNING
+            TimeFilterFastRequest_pb2.TimePeriod.WEEKDAY_MORNING  # type: ignore
         )
         if properties is not None:
             request.oneToManyRequest.properties.extend(properties)
 
         mult = math.pow(10, 5)
         for destination in destinations:
             lat_delta = round((destination.lat - origin.lat) * mult)
@@ -799,15 +795,15 @@
     else:
         request.manyToOneRequest.arrivalLocation.lat = origin.lat
         request.manyToOneRequest.arrivalLocation.lng = origin.lng
 
         request.manyToOneRequest.transportation.type = transportation.value.code
         request.manyToOneRequest.travelTime = travel_time
         request.manyToOneRequest.arrivalTimePeriod = (
-            TimeFilterFastRequest_pb2.TimePeriod.WEEKDAY_MORNING
+            TimeFilterFastRequest_pb2.TimePeriod.WEEKDAY_MORNING  # type: ignore
         )
         if properties is not None:
             request.manyToOneRequest.properties.extend(properties)
 
         mult = math.pow(10, 5)
         for destination in destinations:
             lat_delta = round((destination.lat - origin.lat) * mult)
```

### Comparing `traveltimepy-3.9.6/traveltimepy/proto_http.py` & `traveltimepy-3.9.7/traveltimepy/proto_http.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,24 +4,23 @@
     ClientSession,
     ClientResponse,
     BasicAuth,
     TCPConnector,
     ClientTimeout,
 )
 
-from traveltimepy.TimeFilterFastResponse_pb2 import TimeFilterFastResponse
-from traveltimepy.TimeFilterFastRequest_pb2 import TimeFilterFastRequest
+from traveltimepy.proto import TimeFilterFastResponse_pb2, TimeFilterFastRequest_pb2
 from traveltimepy.dto.responses.time_filter_proto import TimeFilterProtoResponse
 from traveltimepy.errors import ApiError
 
 
 async def send_proto_async(
     url: str,
     headers: Dict[str, str],
-    data: TimeFilterFastRequest,
+    data: TimeFilterFastRequest_pb2.TimeFilterFastRequest,  # type: ignore
     app_id: str,
     api_key: str,
     timeout: int,
 ) -> TimeFilterProtoResponse:
     async with ClientSession(
         timeout=ClientTimeout(total=timeout), connector=TCPConnector(ssl=False)
     ) as session:
@@ -38,13 +37,13 @@
     content = await response.read()
     if response.status != 200:
         msg = (
             f"Travel Time API proto request failed with error code: {response.status}\n"
         )
         raise ApiError(msg)
     else:
-        response_body = TimeFilterFastResponse()
+        response_body = TimeFilterFastResponse_pb2.TimeFilterFastResponse()  # type: ignore
         response_body.ParseFromString(content)
         return TimeFilterProtoResponse(
             travel_times=response_body.properties.travelTimes[:],
             distances=response_body.properties.distances[:],
         )
```

### Comparing `traveltimepy-3.9.6/traveltimepy/sdk.py` & `traveltimepy-3.9.7/traveltimepy/sdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,14 +151,15 @@
 
     async def map_info_async(self) -> List[Map]:
         res = await send_get_async(
             MapInfoResponse,
             "map-info",
             self._headers(AcceptType.JSON),
             self._sdk_params,
+            None,
         )
         return res.maps
 
     async def geocoding_async(
         self,
         query: str,
         limit: Optional[int] = None,
@@ -224,15 +225,15 @@
             create_time_filter_fast(
                 locations,
                 search_ids,
                 transportation,
                 travel_time,
                 properties,
                 one_to_many,
-                snap_penalty
+                snap_penalty,
             ),
             self._sdk_params,
         )
         return resp.results
 
     async def postcodes_async(
         self,
@@ -374,15 +375,15 @@
             create_routes(
                 locations,
                 search_ids,
                 transportation,
                 time_info,
                 properties,
                 range,
-                snap_penalty
+                snap_penalty,
             ),
             self._sdk_params,
         )
         return resp.results
 
     async def time_filter_proto_async(
         self,
@@ -657,15 +658,20 @@
     ) -> List[TimeMapResult]:
         time_info = get_time_info(departure_time, arrival_time)
         resp = await send_post_async(
             TimeMapResponse,
             "distance-map",
             self._headers(AcceptType.JSON),
             create_distance_map(
-                coordinates, transportation, travel_distance, time_info, level_of_detail, snap_penalty
+                coordinates,
+                transportation,
+                travel_distance,
+                time_info,
+                level_of_detail,
+                snap_penalty,
             ),
             self._sdk_params,
         )
         return resp.results
 
     @staticmethod
     def _geocoding_reverse_params(lat: float, lng: float) -> Dict[str, str]:
@@ -709,14 +715,17 @@
             "User-Agent": f"Travel Time Python SDK {__version__}",
             "Content-Type": "application/json",
             "Accept": accept_type.value,
         }
 
 
 def get_time_info(departure_time: Optional[datetime], arrival_time: Optional[datetime]):
+    if not departure_time and not arrival_time:
+        raise ApiError("either arrival_time or departure_time has to be specified")
+
     if departure_time and arrival_time:
         raise ApiError("arrival_time and departure_time cannot be both specified")
 
     if departure_time:
         return DepartureTime(departure_time)
     elif arrival_time:
         return ArrivalTime(arrival_time)
```

### Comparing `traveltimepy-3.9.6/traveltimepy/wkt/error.py` & `traveltimepy-3.9.7/traveltimepy/wkt/error.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.6/traveltimepy/wkt/geometries.py` & `traveltimepy-3.9.7/traveltimepy/wkt/geometries.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.6/traveltimepy/wkt/parsing.py` & `traveltimepy-3.9.7/traveltimepy/wkt/parsing.py`

 * *Files identical despite different names*

### Comparing `traveltimepy-3.9.6/traveltimepy.egg-info/PKG-INFO` & `traveltimepy-3.9.7/traveltimepy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: traveltimepy
-Version: 3.9.6
+Version: 3.9.7
 Summary: "Python Interface to Travel Time."
 Author: TravelTime
 License: MIT
 Keywords: traveltimepy,api,maps
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # Travel Time Python SDK
 
 [![PyPI version](https://badge.fury.io/py/traveltimepy.svg)](https://badge.fury.io/py/traveltimepy) [![Unit Tests](https://github.com/traveltime-dev/traveltime-python-sdk/actions/workflows/ci.yml/badge.svg)](https://github.com/traveltime-dev/traveltime-python-sdk/actions/workflows/ci.yml) [![Python support](https://img.shields.io/badge/python-3.8+-blue.svg)](https://img.shields.io/badge/python-3.8+-blue)
```

### Comparing `traveltimepy-3.9.6/traveltimepy.egg-info/SOURCES.txt` & `traveltimepy-3.9.7/traveltimepy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -64,13 +64,14 @@
 traveltimepy/dto/responses/supported_locations.py
 traveltimepy/dto/responses/time_filter.py
 traveltimepy/dto/responses/time_filter_fast.py
 traveltimepy/dto/responses/time_filter_proto.py
 traveltimepy/dto/responses/time_map.py
 traveltimepy/dto/responses/time_map_wkt.py
 traveltimepy/dto/responses/zones.py
+traveltimepy/proto/__init__.py
 traveltimepy/wkt/__init__.py
 traveltimepy/wkt/constants.py
 traveltimepy/wkt/error.py
 traveltimepy/wkt/geometries.py
 traveltimepy/wkt/helper.py
 traveltimepy/wkt/parsing.py
```

