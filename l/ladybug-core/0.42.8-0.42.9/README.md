# Comparing `tmp/ladybug-core-0.42.8.tar.gz` & `tmp/ladybug-core-0.42.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ladybug-core-0.42.8.tar", last modified: Fri Jan 12 20:23:55 2024, max compression
+gzip compressed data, was "dist/ladybug-core-0.42.9.tar", last modified: Thu Jan 18 00:56:03 2024, max compression
```

## Comparing `ladybug-core-0.42.8.tar` & `ladybug-core-0.42.9.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 20:23:55.000000 ladybug-core-0.42.8/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-01-12 20:23:55.000000 ladybug-core-0.42.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 20:23:55.000000 ladybug-core-0.42.8/ladybug/
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    52020 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/_datacollectionbase.py
--rw-r--r--   0 runner    (1001) docker     (127)    18442 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/analysisperiod.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 20:23:55.000000 ladybug-core-0.42.8/ladybug/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/cli/_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/cli/setconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     4989 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/cli/translate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/climatezone.py
--rw-r--r--   0 runner    (1001) docker     (127)    22056 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/color.py
--rw-r--r--   0 runner    (1001) docker     (127)    12022 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/compass.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/config.json
--rw-r--r--   0 runner    (1001) docker     (127)    11604 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    67221 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/datacollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4651 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/datacollectionimmutable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 20:23:55.000000 ladybug-core-0.42.8/ladybug/datatype/
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/datatype/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/datatype/angle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/datatype/area.py
--rw-r--r--   0 runner    (1001) docker     (127)    15374 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/datatype/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/datatype/current.py
--rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/datatype/distance.py
--rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/datatype/energy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/datatype/energyflux.py
--rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/datatype/energyintensity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/datatype/fraction.py
--rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/datatype/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/datatype/illuminance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/datatype/luminance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/datatype/mass.py
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/datatype/massflowrate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/datatype/power.py
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/datatype/pressure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/datatype/rvalue.py
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/datatype/specificenergy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/datatype/speed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/datatype/temperature.py
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/datatype/temperaturedelta.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/datatype/temperaturetime.py
--rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/datatype/thermalcondition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/datatype/time.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/datatype/uvalue.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/datatype/voltage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/datatype/volume.py
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/datatype/volumeflowrate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/datatype/volumeflowrateintensity.py
--rw-r--r--   0 runner    (1001) docker     (127)     9262 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/datautil.py
--rw-r--r--   0 runner    (1001) docker     (127)     8405 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/ddy.py
--rw-r--r--   0 runner    (1001) docker     (127)    58123 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/designday.py
--rw-r--r--   0 runner    (1001) docker     (127)    18177 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/dt.py
--rw-r--r--   0 runner    (1001) docker     (127)    88637 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/epw.py
--rw-r--r--   0 runner    (1001) docker     (127)    11805 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/futil.py
--rw-r--r--   0 runner    (1001) docker     (127)    11197 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/graphic.py
--rw-r--r--   0 runner    (1001) docker     (127)     6730 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/header.py
--rw-r--r--   0 runner    (1001) docker     (127)    25737 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/hourlyplot.py
--rw-r--r--   0 runner    (1001) docker     (127)    84135 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/legend.py
--rw-r--r--   0 runner    (1001) docker     (127)     8827 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/location.py
--rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/logutil.py
--rw-r--r--   0 runner    (1001) docker     (127)    50531 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/monthlychart.py
--rw-r--r--   0 runner    (1001) docker     (127)    42331 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/psychchart.py
--rw-r--r--   0 runner    (1001) docker     (127)    19292 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/psychrometrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5506 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/rootfinding.py
--rw-r--r--   0 runner    (1001) docker     (127)    55789 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/skymodel.py
--rw-r--r--   0 runner    (1001) docker     (127)    10504 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/solarenvelope.py
--rw-r--r--   0 runner    (1001) docker     (127)    48107 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)    36110 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/stat.py
--rw-r--r--   0 runner    (1001) docker     (127)    57112 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/sunpath.py
--rw-r--r--   0 runner    (1001) docker     (127)    30461 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/viewsphere.py
--rw-r--r--   0 runner    (1001) docker     (127)    53418 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/wea.py
--rw-r--r--   0 runner    (1001) docker     (127)    39127 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/windprofile.py
--rw-r--r--   0 runner    (1001) docker     (127)    37860 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/ladybug/windrose.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 20:23:55.000000 ladybug-core-0.42.8/ladybug_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-01-12 20:23:55.000000 ladybug-core-0.42.8/ladybug_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-01-12 20:23:55.000000 ladybug-core-0.42.8/ladybug_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-12 20:23:55.000000 ladybug-core-0.42.8/ladybug_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-01-12 20:23:55.000000 ladybug-core-0.42.8/ladybug_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-01-12 20:23:55.000000 ladybug-core-0.42.8/ladybug_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-12 20:23:55.000000 ladybug-core-0.42.8/ladybug_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-01-12 20:23:55.000000 ladybug-core-0.42.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-01-12 20:22:52.000000 ladybug-core-0.42.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 00:56:03.000000 ladybug-core-0.42.9/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-01-18 00:56:03.000000 ladybug-core-0.42.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 00:56:03.000000 ladybug-core-0.42.9/ladybug/
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52020 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/_datacollectionbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18442 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/analysisperiod.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 00:56:03.000000 ladybug-core-0.42.9/ladybug/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/cli/_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/cli/setconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4989 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/cli/translate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/climatezone.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22056 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/color.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12022 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/compass.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/config.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11604 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67221 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/datacollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4651 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/datacollectionimmutable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 00:56:03.000000 ladybug-core-0.42.9/ladybug/datatype/
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/datatype/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/datatype/angle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/datatype/area.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15374 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/datatype/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/datatype/current.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/datatype/distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/datatype/energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/datatype/energyflux.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/datatype/energyintensity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/datatype/fraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/datatype/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/datatype/illuminance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/datatype/luminance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/datatype/mass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/datatype/massflowrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/datatype/power.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/datatype/pressure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/datatype/rvalue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/datatype/specificenergy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/datatype/speed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/datatype/temperature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/datatype/temperaturedelta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/datatype/temperaturetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/datatype/thermalcondition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/datatype/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/datatype/uvalue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/datatype/voltage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/datatype/volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/datatype/volumeflowrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/datatype/volumeflowrateintensity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9262 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/datautil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8405 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/ddy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58123 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/designday.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18177 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/dt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    88637 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/epw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11805 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/futil.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11197 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/graphic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6730 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/header.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25737 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/hourlyplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84135 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/legend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8827 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/logutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50531 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/monthlychart.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42331 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/psychchart.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19292 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/psychrometrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5506 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/rootfinding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55789 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/skymodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10504 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/solarenvelope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48107 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36110 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/stat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57112 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/sunpath.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30461 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/viewsphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53418 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/wea.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39127 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/windprofile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37860 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/ladybug/windrose.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 00:56:03.000000 ladybug-core-0.42.9/ladybug_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-01-18 00:56:03.000000 ladybug-core-0.42.9/ladybug_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-01-18 00:56:03.000000 ladybug-core-0.42.9/ladybug_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 00:56:03.000000 ladybug-core-0.42.9/ladybug_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-01-18 00:56:03.000000 ladybug-core-0.42.9/ladybug_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-01-18 00:56:03.000000 ladybug-core-0.42.9/ladybug_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-18 00:56:03.000000 ladybug-core-0.42.9/ladybug_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-01-18 00:56:03.000000 ladybug-core-0.42.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-01-18 00:54:55.000000 ladybug-core-0.42.9/setup.py
```

### Comparing `ladybug-core-0.42.8/LICENSE` & `ladybug-core-0.42.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/PKG-INFO` & `ladybug-core-0.42.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ladybug-core
-Version: 0.42.8
+Version: 0.42.9
 Summary: Python library to load, analyze and modify EnergyPlus Weather files (epw).
 Home-page: https://github.com/ladybug-tools/ladybug
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `ladybug-core-0.42.8/README.md` & `ladybug-core-0.42.9/README.md`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/dev-requirements.txt` & `ladybug-core-0.42.9/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/__init__.py` & `ladybug-core-0.42.9/ladybug/__init__.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/_datacollectionbase.py` & `ladybug-core-0.42.9/ladybug/_datacollectionbase.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/analysisperiod.py` & `ladybug-core-0.42.9/ladybug/analysisperiod.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/cli/__init__.py` & `ladybug-core-0.42.9/ladybug/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/cli/_helper.py` & `ladybug-core-0.42.9/ladybug/cli/_helper.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/cli/setconfig.py` & `ladybug-core-0.42.9/ladybug/cli/setconfig.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/cli/translate.py` & `ladybug-core-0.42.9/ladybug/cli/translate.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/climatezone.py` & `ladybug-core-0.42.9/ladybug/climatezone.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/color.py` & `ladybug-core-0.42.9/ladybug/color.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/compass.py` & `ladybug-core-0.42.9/ladybug/compass.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/config.py` & `ladybug-core-0.42.9/ladybug/config.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/datacollection.py` & `ladybug-core-0.42.9/ladybug/datacollection.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/datacollectionimmutable.py` & `ladybug-core-0.42.9/ladybug/datacollectionimmutable.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/datatype/__init__.py` & `ladybug-core-0.42.9/ladybug/datatype/__init__.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/datatype/angle.py` & `ladybug-core-0.42.9/ladybug/datatype/angle.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/datatype/area.py` & `ladybug-core-0.42.9/ladybug/datatype/area.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/datatype/base.py` & `ladybug-core-0.42.9/ladybug/datatype/base.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/datatype/current.py` & `ladybug-core-0.42.9/ladybug/datatype/current.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/datatype/distance.py` & `ladybug-core-0.42.9/ladybug/datatype/distance.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/datatype/energy.py` & `ladybug-core-0.42.9/ladybug/datatype/energy.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/datatype/energyflux.py` & `ladybug-core-0.42.9/ladybug/datatype/energyflux.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/datatype/energyintensity.py` & `ladybug-core-0.42.9/ladybug/datatype/energyintensity.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/datatype/fraction.py` & `ladybug-core-0.42.9/ladybug/datatype/fraction.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/datatype/generic.py` & `ladybug-core-0.42.9/ladybug/datatype/generic.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/datatype/illuminance.py` & `ladybug-core-0.42.9/ladybug/datatype/illuminance.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/datatype/luminance.py` & `ladybug-core-0.42.9/ladybug/datatype/luminance.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/datatype/mass.py` & `ladybug-core-0.42.9/ladybug/datatype/mass.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/datatype/massflowrate.py` & `ladybug-core-0.42.9/ladybug/datatype/massflowrate.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/datatype/power.py` & `ladybug-core-0.42.9/ladybug/datatype/power.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/datatype/pressure.py` & `ladybug-core-0.42.9/ladybug/datatype/pressure.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/datatype/rvalue.py` & `ladybug-core-0.42.9/ladybug/datatype/rvalue.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/datatype/specificenergy.py` & `ladybug-core-0.42.9/ladybug/datatype/specificenergy.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/datatype/speed.py` & `ladybug-core-0.42.9/ladybug/datatype/speed.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/datatype/temperature.py` & `ladybug-core-0.42.9/ladybug/datatype/temperature.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/datatype/temperaturedelta.py` & `ladybug-core-0.42.9/ladybug/datatype/temperaturedelta.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/datatype/temperaturetime.py` & `ladybug-core-0.42.9/ladybug/datatype/temperaturetime.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/datatype/thermalcondition.py` & `ladybug-core-0.42.9/ladybug/datatype/thermalcondition.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/datatype/time.py` & `ladybug-core-0.42.9/ladybug/datatype/time.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/datatype/uvalue.py` & `ladybug-core-0.42.9/ladybug/datatype/uvalue.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/datatype/voltage.py` & `ladybug-core-0.42.9/ladybug/datatype/voltage.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/datatype/volume.py` & `ladybug-core-0.42.9/ladybug/datatype/volume.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/datatype/volumeflowrate.py` & `ladybug-core-0.42.9/ladybug/datatype/volumeflowrate.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/datatype/volumeflowrateintensity.py` & `ladybug-core-0.42.9/ladybug/datatype/volumeflowrateintensity.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/datautil.py` & `ladybug-core-0.42.9/ladybug/datautil.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/ddy.py` & `ladybug-core-0.42.9/ladybug/ddy.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/designday.py` & `ladybug-core-0.42.9/ladybug/designday.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/dt.py` & `ladybug-core-0.42.9/ladybug/dt.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/epw.py` & `ladybug-core-0.42.9/ladybug/epw.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/futil.py` & `ladybug-core-0.42.9/ladybug/futil.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/graphic.py` & `ladybug-core-0.42.9/ladybug/graphic.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/header.py` & `ladybug-core-0.42.9/ladybug/header.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/hourlyplot.py` & `ladybug-core-0.42.9/ladybug/hourlyplot.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/legend.py` & `ladybug-core-0.42.9/ladybug/legend.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/location.py` & `ladybug-core-0.42.9/ladybug/location.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/logutil.py` & `ladybug-core-0.42.9/ladybug/logutil.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/monthlychart.py` & `ladybug-core-0.42.9/ladybug/monthlychart.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/psychchart.py` & `ladybug-core-0.42.9/ladybug/psychchart.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/psychrometrics.py` & `ladybug-core-0.42.9/ladybug/psychrometrics.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/rootfinding.py` & `ladybug-core-0.42.9/ladybug/rootfinding.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/skymodel.py` & `ladybug-core-0.42.9/ladybug/skymodel.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/solarenvelope.py` & `ladybug-core-0.42.9/ladybug/solarenvelope.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/sql.py` & `ladybug-core-0.42.9/ladybug/sql.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/stat.py` & `ladybug-core-0.42.9/ladybug/stat.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/sunpath.py` & `ladybug-core-0.42.9/ladybug/sunpath.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/viewsphere.py` & `ladybug-core-0.42.9/ladybug/viewsphere.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/wea.py` & `ladybug-core-0.42.9/ladybug/wea.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/windprofile.py` & `ladybug-core-0.42.9/ladybug/windprofile.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug/windrose.py` & `ladybug-core-0.42.9/ladybug/windrose.py`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/ladybug_core.egg-info/PKG-INFO` & `ladybug-core-0.42.9/ladybug_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ladybug-core
-Version: 0.42.8
+Version: 0.42.9
 Summary: Python library to load, analyze and modify EnergyPlus Weather files (epw).
 Home-page: https://github.com/ladybug-tools/ladybug
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `ladybug-core-0.42.8/ladybug_core.egg-info/SOURCES.txt` & `ladybug-core-0.42.9/ladybug_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ladybug-core-0.42.8/setup.py` & `ladybug-core-0.42.9/setup.py`

 * *Files identical despite different names*

