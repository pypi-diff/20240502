# Comparing `tmp/kpler.sdk-1.0.7.tar.gz` & `tmp/kpler.sdk-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kpler.sdk-1.0.7.tar", last modified: Tue Jun  1 16:53:50 2021, max compression
+gzip compressed data, was "dist/kpler.sdk-1.0.8.tar", last modified: Fri Jun 18 10:31:58 2021, max compression
```

## Comparing `kpler.sdk-1.0.7.tar` & `kpler.sdk-1.0.8.tar`

### file list

```diff
@@ -1,91 +1,92 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-06-01 16:53:50.000000 kpler.sdk-1.0.7/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2487 2021-06-01 16:53:50.000000 kpler.sdk-1.0.7/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1454 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-06-01 16:53:50.000000 kpler.sdk-1.0.7/doc/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      638 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/doc/Makefile
--rw-r--r--   0 circleci  (3434) circleci  (3434)      764 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/doc/make.bat
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-06-01 16:53:50.000000 kpler.sdk-1.0.7/doc/source/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/doc/source/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-06-01 16:53:50.000000 kpler.sdk-1.0.7/doc/source/_static/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-06-01 16:53:50.000000 kpler.sdk-1.0.7/doc/source/_static/css/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      121 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/doc/source/_static/css/custom.css
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4286 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/doc/source/_static/favicon.ico
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7954 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/doc/source/_static/logo-white.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1245 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/doc/source/change_log.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3109 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/doc/source/conf.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-06-01 16:53:50.000000 kpler.sdk-1.0.7/doc/source/examples/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      716 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/doc/source/examples/quick_one.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2370 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/doc/source/getting_started.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2420 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/doc/source/index.rst
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-06-01 16:53:50.000000 kpler.sdk-1.0.7/doc/source/resources/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      752 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/doc/source/resources/ballast_capacity_port_calls.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)      909 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/doc/source/resources/ballast_capacity_series.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)      924 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/doc/source/resources/congestion_series.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)      636 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/doc/source/resources/congestion_vessels.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)      197 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/doc/source/resources/contracts.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)      997 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/doc/source/resources/fleet_development_series.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)      747 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/doc/source/resources/fleet_development_vessels.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)      492 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/doc/source/resources/fleet_metrics_series.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)      360 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/doc/source/resources/fleet_metrics_vessels.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)      991 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/doc/source/resources/fleet_utilization_series.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)      733 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/doc/source/resources/fleet_utilization_vessels.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)      392 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/doc/source/resources/flows.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)      849 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/doc/source/resources/freight_metrics_series.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)      205 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/doc/source/resources/installations.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)      269 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/doc/source/resources/inventories.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)      200 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/doc/source/resources/inventories_tank_levels.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)      187 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/doc/source/resources/outages.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)      181 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/doc/source/resources/players.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)      192 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/doc/source/resources/port_calls.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)      184 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/doc/source/resources/prices.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)      185 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/doc/source/resources/products.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)      189 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/doc/source/resources/ship_to_ships.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)      230 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/doc/source/resources/trades.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)      181 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/doc/source/resources/vessels.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)      173 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/doc/source/resources/zones.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2021-06-01 16:53:50.000000 kpler.sdk-1.0.7/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1560 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-06-01 16:53:50.000000 kpler.sdk-1.0.7/src/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-06-01 16:53:50.000000 kpler.sdk-1.0.7/src/kpler/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-06-01 16:53:50.000000 kpler.sdk-1.0.7/src/kpler/sdk/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3171 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/src/kpler/sdk/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6552 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/src/kpler/sdk/client.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2929 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/src/kpler/sdk/configuration.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10439 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/src/kpler/sdk/enums.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1886 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/src/kpler/sdk/exceptions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6208 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/src/kpler/sdk/helpers.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-06-01 16:53:50.000000 kpler.sdk-1.0.7/src/kpler/sdk/resources/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/src/kpler/sdk/resources/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4547 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/src/kpler/sdk/resources/ballast_capacity_port_calls.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4864 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/src/kpler/sdk/resources/ballast_capacity_series.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5762 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/src/kpler/sdk/resources/congestion_series.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5532 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/src/kpler/sdk/resources/congestion_vessels.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4718 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/src/kpler/sdk/resources/contracts.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5923 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/src/kpler/sdk/resources/fleet_development_series.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6031 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/src/kpler/sdk/resources/fleet_development_vessels.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4728 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/src/kpler/sdk/resources/fleet_metrics.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5104 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/src/kpler/sdk/resources/fleet_metrics_vessels.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5375 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/src/kpler/sdk/resources/fleet_utilization_series.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4549 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/src/kpler/sdk/resources/fleet_utilization_vessels.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5774 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/src/kpler/sdk/resources/flows.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6672 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/src/kpler/sdk/resources/freight_metrics_series.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1262 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/src/kpler/sdk/resources/installations.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4661 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/src/kpler/sdk/resources/inventories.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2840 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/src/kpler/sdk/resources/inventories_tank_levels.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4981 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/src/kpler/sdk/resources/outages.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1172 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/src/kpler/sdk/resources/players.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5584 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/src/kpler/sdk/resources/port_calls.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4262 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/src/kpler/sdk/resources/prices.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1332 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/src/kpler/sdk/resources/products.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4887 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/src/kpler/sdk/resources/ship_to_ships.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7918 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/src/kpler/sdk/resources/trades.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4034 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/src/kpler/sdk/resources/vessels.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1178 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/src/kpler/sdk/resources/zones.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-06-01 16:53:50.000000 kpler.sdk-1.0.7/src/kpler.sdk.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2487 2021-06-01 16:53:50.000000 kpler.sdk-1.0.7/src/kpler.sdk.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2812 2021-06-01 16:53:50.000000 kpler.sdk-1.0.7/src/kpler.sdk.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2021-06-01 16:53:50.000000 kpler.sdk-1.0.7/src/kpler.sdk.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2021-06-01 16:53:50.000000 kpler.sdk-1.0.7/src/kpler.sdk.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)      286 2021-06-01 16:53:50.000000 kpler.sdk-1.0.7/src/kpler.sdk.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        6 2021-06-01 16:53:50.000000 kpler.sdk-1.0.7/src/kpler.sdk.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       78 2021-06-01 16:53:33.000000 kpler.sdk-1.0.7/tox.ini
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-06-18 10:31:58.000000 kpler.sdk-1.0.8/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11341 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2523 2021-06-18 10:31:58.000000 kpler.sdk-1.0.8/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1454 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-06-18 10:31:58.000000 kpler.sdk-1.0.8/doc/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      638 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/doc/Makefile
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      764 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/doc/make.bat
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-06-18 10:31:58.000000 kpler.sdk-1.0.8/doc/source/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/doc/source/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-06-18 10:31:58.000000 kpler.sdk-1.0.8/doc/source/_static/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-06-18 10:31:58.000000 kpler.sdk-1.0.8/doc/source/_static/css/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      121 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/doc/source/_static/css/custom.css
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4286 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/doc/source/_static/favicon.ico
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7954 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/doc/source/_static/logo-white.png
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1321 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/doc/source/change_log.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3109 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/doc/source/conf.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-06-18 10:31:58.000000 kpler.sdk-1.0.8/doc/source/examples/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      716 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/doc/source/examples/quick_one.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2370 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/doc/source/getting_started.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2420 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/doc/source/index.rst
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-06-18 10:31:58.000000 kpler.sdk-1.0.8/doc/source/resources/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      752 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/doc/source/resources/ballast_capacity_port_calls.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      909 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/doc/source/resources/ballast_capacity_series.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      924 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/doc/source/resources/congestion_series.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      636 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/doc/source/resources/congestion_vessels.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      197 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/doc/source/resources/contracts.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      997 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/doc/source/resources/fleet_development_series.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      747 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/doc/source/resources/fleet_development_vessels.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      492 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/doc/source/resources/fleet_metrics_series.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      360 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/doc/source/resources/fleet_metrics_vessels.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      991 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/doc/source/resources/fleet_utilization_series.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      733 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/doc/source/resources/fleet_utilization_vessels.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      392 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/doc/source/resources/flows.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      849 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/doc/source/resources/freight_metrics_series.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      205 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/doc/source/resources/installations.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      269 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/doc/source/resources/inventories.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      200 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/doc/source/resources/inventories_tank_levels.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      187 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/doc/source/resources/outages.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      181 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/doc/source/resources/players.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      192 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/doc/source/resources/port_calls.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      184 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/doc/source/resources/prices.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      185 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/doc/source/resources/products.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      189 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/doc/source/resources/ship_to_ships.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      230 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/doc/source/resources/trades.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      181 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/doc/source/resources/vessels.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      173 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/doc/source/resources/zones.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2021-06-18 10:31:58.000000 kpler.sdk-1.0.8/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1571 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-06-18 10:31:58.000000 kpler.sdk-1.0.8/src/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-06-18 10:31:58.000000 kpler.sdk-1.0.8/src/kpler/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-06-18 10:31:58.000000 kpler.sdk-1.0.8/src/kpler/sdk/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3171 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/src/kpler/sdk/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6552 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/src/kpler/sdk/client.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2929 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/src/kpler/sdk/configuration.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10439 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/src/kpler/sdk/enums.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1886 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/src/kpler/sdk/exceptions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6208 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/src/kpler/sdk/helpers.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-06-18 10:31:58.000000 kpler.sdk-1.0.8/src/kpler/sdk/resources/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/src/kpler/sdk/resources/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4547 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/src/kpler/sdk/resources/ballast_capacity_port_calls.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4864 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/src/kpler/sdk/resources/ballast_capacity_series.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5762 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/src/kpler/sdk/resources/congestion_series.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5532 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/src/kpler/sdk/resources/congestion_vessels.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4718 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/src/kpler/sdk/resources/contracts.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5923 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/src/kpler/sdk/resources/fleet_development_series.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6031 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/src/kpler/sdk/resources/fleet_development_vessels.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4728 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/src/kpler/sdk/resources/fleet_metrics.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5104 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/src/kpler/sdk/resources/fleet_metrics_vessels.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5375 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/src/kpler/sdk/resources/fleet_utilization_series.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4549 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/src/kpler/sdk/resources/fleet_utilization_vessels.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5774 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/src/kpler/sdk/resources/flows.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6672 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/src/kpler/sdk/resources/freight_metrics_series.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1262 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/src/kpler/sdk/resources/installations.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4661 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/src/kpler/sdk/resources/inventories.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2840 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/src/kpler/sdk/resources/inventories_tank_levels.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4981 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/src/kpler/sdk/resources/outages.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1172 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/src/kpler/sdk/resources/players.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5584 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/src/kpler/sdk/resources/port_calls.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4262 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/src/kpler/sdk/resources/prices.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1332 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/src/kpler/sdk/resources/products.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4887 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/src/kpler/sdk/resources/ship_to_ships.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7918 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/src/kpler/sdk/resources/trades.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4034 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/src/kpler/sdk/resources/vessels.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1178 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/src/kpler/sdk/resources/zones.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-06-18 10:31:58.000000 kpler.sdk-1.0.8/src/kpler.sdk.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2523 2021-06-18 10:31:58.000000 kpler.sdk-1.0.8/src/kpler.sdk.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2820 2021-06-18 10:31:58.000000 kpler.sdk-1.0.8/src/kpler.sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2021-06-18 10:31:58.000000 kpler.sdk-1.0.8/src/kpler.sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2021-06-18 10:31:58.000000 kpler.sdk-1.0.8/src/kpler.sdk.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      272 2021-06-18 10:31:58.000000 kpler.sdk-1.0.8/src/kpler.sdk.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        6 2021-06-18 10:31:58.000000 kpler.sdk-1.0.8/src/kpler.sdk.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       78 2021-06-18 10:31:43.000000 kpler.sdk-1.0.8/tox.ini
```

### Comparing `kpler.sdk-1.0.7/PKG-INFO` & `kpler.sdk-1.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: kpler.sdk
-Version: 1.0.7
+Version: 1.0.8
 Summary: A Python wrapper around the Kpler client API
 Home-page: http://github.com/kpler/python-sdk
 Author: Kpler
 Author-email: engineering@kpler.com
-License: MIT
+License: Apache License, Version 2.0
 Description: The Kpler Python SDK provides access to Kpler data.
         
         It can be easily integrated into notebooks, scripts, and applications.
         
         It is available to all Kpler API clients (credentials required)
         
         Documentation : https://python-sdk.dev.kpler.com
@@ -56,13 +56,13 @@
         ````
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: publish
-Provides-Extra: test
 Provides-Extra: doc
+Provides-Extra: test
```

### Comparing `kpler.sdk-1.0.7/README.md` & `kpler.sdk-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `kpler.sdk-1.0.7/doc/Makefile` & `kpler.sdk-1.0.8/doc/Makefile`

 * *Files identical despite different names*

### Comparing `kpler.sdk-1.0.7/doc/make.bat` & `kpler.sdk-1.0.8/doc/make.bat`

 * *Files identical despite different names*

### Comparing `kpler.sdk-1.0.7/doc/source/_static/favicon.ico` & `kpler.sdk-1.0.8/doc/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `kpler.sdk-1.0.7/doc/source/_static/logo-white.png` & `kpler.sdk-1.0.8/doc/source/_static/logo-white.png`

 * *Files identical despite different names*

### Comparing `kpler.sdk-1.0.7/doc/source/change_log.rst` & `kpler.sdk-1.0.8/doc/source/change_log.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Changelog
 *********
 
+- 1.0.8 - 2021-06-18
+    - review dependencies
+    - licensing source code
+
 - 1.0.7 - 2021-06-01
     - add `with_product_estimation` parameter for trades
     - documentation updates
     - availability to update the endpoints url for dev purpose
 
 - 1.0.5 - 2021-02-24
     - add `withFreightView` param according to the documentation
```

### Comparing `kpler.sdk-1.0.7/doc/source/conf.py` & `kpler.sdk-1.0.8/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `kpler.sdk-1.0.7/doc/source/examples/quick_one.py` & `kpler.sdk-1.0.8/doc/source/examples/quick_one.py`

 * *Files identical despite different names*

### Comparing `kpler.sdk-1.0.7/doc/source/getting_started.rst` & `kpler.sdk-1.0.8/doc/source/getting_started.rst`

 * *Files identical despite different names*

### Comparing `kpler.sdk-1.0.7/doc/source/index.rst` & `kpler.sdk-1.0.8/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `kpler.sdk-1.0.7/doc/source/resources/ballast_capacity_port_calls.rst` & `kpler.sdk-1.0.8/doc/source/resources/ballast_capacity_port_calls.rst`

 * *Files identical despite different names*

### Comparing `kpler.sdk-1.0.7/doc/source/resources/ballast_capacity_series.rst` & `kpler.sdk-1.0.8/doc/source/resources/ballast_capacity_series.rst`

 * *Files identical despite different names*

### Comparing `kpler.sdk-1.0.7/doc/source/resources/congestion_series.rst` & `kpler.sdk-1.0.8/doc/source/resources/congestion_series.rst`

 * *Files identical despite different names*

### Comparing `kpler.sdk-1.0.7/doc/source/resources/congestion_vessels.rst` & `kpler.sdk-1.0.8/doc/source/resources/congestion_vessels.rst`

 * *Files identical despite different names*

### Comparing `kpler.sdk-1.0.7/doc/source/resources/fleet_development_series.rst` & `kpler.sdk-1.0.8/doc/source/resources/fleet_development_series.rst`

 * *Files identical despite different names*

### Comparing `kpler.sdk-1.0.7/doc/source/resources/fleet_development_vessels.rst` & `kpler.sdk-1.0.8/doc/source/resources/fleet_development_vessels.rst`

 * *Files identical despite different names*

### Comparing `kpler.sdk-1.0.7/doc/source/resources/fleet_utilization_series.rst` & `kpler.sdk-1.0.8/doc/source/resources/fleet_utilization_series.rst`

 * *Files identical despite different names*

### Comparing `kpler.sdk-1.0.7/doc/source/resources/fleet_utilization_vessels.rst` & `kpler.sdk-1.0.8/doc/source/resources/fleet_utilization_vessels.rst`

 * *Files identical despite different names*

### Comparing `kpler.sdk-1.0.7/doc/source/resources/freight_metrics_series.rst` & `kpler.sdk-1.0.8/doc/source/resources/freight_metrics_series.rst`

 * *Files identical despite different names*

### Comparing `kpler.sdk-1.0.7/setup.py` & `kpler.sdk-1.0.8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,32 +10,31 @@
     use_scm_version=True,
     setup_requires=["setuptools_scm"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="http://github.com/kpler/python-sdk",
     author="Kpler",
     author_email="engineering@kpler.com",
-    license="MIT",
+    license="Apache License, Version 2.0",
     packages=find_namespace_packages(
         where="src",
         include=["kpler*"],
     ),
     package_dir={"": "src"},
     install_requires=[
-        "pandas>=1.1.4",
-        "numpy>=1.19.0",
-        "requests>=2.24.0",
+        "pandas>=1.0.0",
+        "requests>=2.20.0",
     ],
     zip_safe=False,
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
-        "License :: OSI Approved :: MIT License",
+        "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     extras_require={
         "doc": [
             "Sphinx==3.2.1",
             "sphinx_rtd_theme==0.5.0",
             "sphinx-autodoc-typehints==1.6.0",
```

### Comparing `kpler.sdk-1.0.7/src/kpler/sdk/__init__.py` & `kpler.sdk-1.0.8/src/kpler/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `kpler.sdk-1.0.7/src/kpler/sdk/client.py` & `kpler.sdk-1.0.8/src/kpler/sdk/client.py`

 * *Files identical despite different names*

### Comparing `kpler.sdk-1.0.7/src/kpler/sdk/configuration.py` & `kpler.sdk-1.0.8/src/kpler/sdk/configuration.py`

 * *Files identical despite different names*

### Comparing `kpler.sdk-1.0.7/src/kpler/sdk/enums.py` & `kpler.sdk-1.0.8/src/kpler/sdk/enums.py`

 * *Files identical despite different names*

### Comparing `kpler.sdk-1.0.7/src/kpler/sdk/exceptions.py` & `kpler.sdk-1.0.8/src/kpler/sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `kpler.sdk-1.0.7/src/kpler/sdk/helpers.py` & `kpler.sdk-1.0.8/src/kpler/sdk/helpers.py`

 * *Files identical despite different names*

### Comparing `kpler.sdk-1.0.7/src/kpler/sdk/resources/ballast_capacity_port_calls.py` & `kpler.sdk-1.0.8/src/kpler/sdk/resources/ballast_capacity_port_calls.py`

 * *Files identical despite different names*

### Comparing `kpler.sdk-1.0.7/src/kpler/sdk/resources/ballast_capacity_series.py` & `kpler.sdk-1.0.8/src/kpler/sdk/resources/ballast_capacity_series.py`

 * *Files identical despite different names*

### Comparing `kpler.sdk-1.0.7/src/kpler/sdk/resources/congestion_series.py` & `kpler.sdk-1.0.8/src/kpler/sdk/resources/congestion_series.py`

 * *Files identical despite different names*

### Comparing `kpler.sdk-1.0.7/src/kpler/sdk/resources/congestion_vessels.py` & `kpler.sdk-1.0.8/src/kpler/sdk/resources/congestion_vessels.py`

 * *Files identical despite different names*

### Comparing `kpler.sdk-1.0.7/src/kpler/sdk/resources/contracts.py` & `kpler.sdk-1.0.8/src/kpler/sdk/resources/contracts.py`

 * *Files identical despite different names*

### Comparing `kpler.sdk-1.0.7/src/kpler/sdk/resources/fleet_development_series.py` & `kpler.sdk-1.0.8/src/kpler/sdk/resources/fleet_development_series.py`

 * *Files identical despite different names*

### Comparing `kpler.sdk-1.0.7/src/kpler/sdk/resources/fleet_development_vessels.py` & `kpler.sdk-1.0.8/src/kpler/sdk/resources/fleet_development_vessels.py`

 * *Files identical despite different names*

### Comparing `kpler.sdk-1.0.7/src/kpler/sdk/resources/fleet_metrics.py` & `kpler.sdk-1.0.8/src/kpler/sdk/resources/fleet_metrics.py`

 * *Files identical despite different names*

### Comparing `kpler.sdk-1.0.7/src/kpler/sdk/resources/fleet_metrics_vessels.py` & `kpler.sdk-1.0.8/src/kpler/sdk/resources/fleet_metrics_vessels.py`

 * *Files identical despite different names*

### Comparing `kpler.sdk-1.0.7/src/kpler/sdk/resources/fleet_utilization_series.py` & `kpler.sdk-1.0.8/src/kpler/sdk/resources/fleet_utilization_series.py`

 * *Files identical despite different names*

### Comparing `kpler.sdk-1.0.7/src/kpler/sdk/resources/fleet_utilization_vessels.py` & `kpler.sdk-1.0.8/src/kpler/sdk/resources/fleet_utilization_vessels.py`

 * *Files identical despite different names*

### Comparing `kpler.sdk-1.0.7/src/kpler/sdk/resources/flows.py` & `kpler.sdk-1.0.8/src/kpler/sdk/resources/flows.py`

 * *Files identical despite different names*

### Comparing `kpler.sdk-1.0.7/src/kpler/sdk/resources/freight_metrics_series.py` & `kpler.sdk-1.0.8/src/kpler/sdk/resources/freight_metrics_series.py`

 * *Files identical despite different names*

### Comparing `kpler.sdk-1.0.7/src/kpler/sdk/resources/installations.py` & `kpler.sdk-1.0.8/src/kpler/sdk/resources/installations.py`

 * *Files identical despite different names*

### Comparing `kpler.sdk-1.0.7/src/kpler/sdk/resources/inventories.py` & `kpler.sdk-1.0.8/src/kpler/sdk/resources/inventories.py`

 * *Files identical despite different names*

### Comparing `kpler.sdk-1.0.7/src/kpler/sdk/resources/inventories_tank_levels.py` & `kpler.sdk-1.0.8/src/kpler/sdk/resources/inventories_tank_levels.py`

 * *Files identical despite different names*

### Comparing `kpler.sdk-1.0.7/src/kpler/sdk/resources/outages.py` & `kpler.sdk-1.0.8/src/kpler/sdk/resources/outages.py`

 * *Files identical despite different names*

### Comparing `kpler.sdk-1.0.7/src/kpler/sdk/resources/players.py` & `kpler.sdk-1.0.8/src/kpler/sdk/resources/players.py`

 * *Files identical despite different names*

### Comparing `kpler.sdk-1.0.7/src/kpler/sdk/resources/port_calls.py` & `kpler.sdk-1.0.8/src/kpler/sdk/resources/port_calls.py`

 * *Files identical despite different names*

### Comparing `kpler.sdk-1.0.7/src/kpler/sdk/resources/prices.py` & `kpler.sdk-1.0.8/src/kpler/sdk/resources/prices.py`

 * *Files identical despite different names*

### Comparing `kpler.sdk-1.0.7/src/kpler/sdk/resources/products.py` & `kpler.sdk-1.0.8/src/kpler/sdk/resources/products.py`

 * *Files identical despite different names*

### Comparing `kpler.sdk-1.0.7/src/kpler/sdk/resources/ship_to_ships.py` & `kpler.sdk-1.0.8/src/kpler/sdk/resources/ship_to_ships.py`

 * *Files identical despite different names*

### Comparing `kpler.sdk-1.0.7/src/kpler/sdk/resources/trades.py` & `kpler.sdk-1.0.8/src/kpler/sdk/resources/trades.py`

 * *Files identical despite different names*

### Comparing `kpler.sdk-1.0.7/src/kpler/sdk/resources/vessels.py` & `kpler.sdk-1.0.8/src/kpler/sdk/resources/vessels.py`

 * *Files identical despite different names*

### Comparing `kpler.sdk-1.0.7/src/kpler/sdk/resources/zones.py` & `kpler.sdk-1.0.8/src/kpler/sdk/resources/zones.py`

 * *Files identical despite different names*

### Comparing `kpler.sdk-1.0.7/src/kpler.sdk.egg-info/PKG-INFO` & `kpler.sdk-1.0.8/src/kpler.sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: kpler.sdk
-Version: 1.0.7
+Version: 1.0.8
 Summary: A Python wrapper around the Kpler client API
 Home-page: http://github.com/kpler/python-sdk
 Author: Kpler
 Author-email: engineering@kpler.com
-License: MIT
+License: Apache License, Version 2.0
 Description: The Kpler Python SDK provides access to Kpler data.
         
         It can be easily integrated into notebooks, scripts, and applications.
         
         It is available to all Kpler API clients (credentials required)
         
         Documentation : https://python-sdk.dev.kpler.com
@@ -56,13 +56,13 @@
         ````
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: publish
-Provides-Extra: test
 Provides-Extra: doc
+Provides-Extra: test
```

### Comparing `kpler.sdk-1.0.7/src/kpler.sdk.egg-info/SOURCES.txt` & `kpler.sdk-1.0.8/src/kpler.sdk.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 tox.ini
 doc/Makefile
 doc/make.bat
 doc/source/__init__.py
 doc/source/change_log.rst
```

