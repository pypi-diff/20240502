# Comparing `tmp/opentrons_shared_data-7.2.2a3.tar.gz` & `tmp/opentrons_shared_data-7.3.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentrons_shared_data-7.2.2a3.tar", last modified: Mon Apr  8 17:00:35 2024, max compression
+gzip compressed data, was "opentrons_shared_data-7.3.0a0.tar", last modified: Thu May  2 12:07:30 2024, max compression
```

## Comparing `opentrons_shared_data-7.2.2a3.tar` & `opentrons_shared_data-7.3.0a0.tar`

### file list

```diff
@@ -1,674 +1,687 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.448622 opentrons_shared_data-7.2.2a3/
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-08 17:00:35.448622 opentrons_shared_data-7.2.2a3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.440622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-08 16:59:17.000000 opentrons_shared_data-7.2.2a3/opentrons_shared_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-08 16:59:17.000000 opentrons_shared_data-7.2.2a3/opentrons_shared_data/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.440622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/command/
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-04-08 16:59:17.000000 opentrons_shared_data-7.2.2a3/opentrons_shared_data/command/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.436622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.432622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/command/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.436622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/command/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    97753 2024-04-08 17:00:35.436622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/command/schemas/7.json
--rw-r--r--   0 runner    (1001) docker     (127)   121346 2024-04-08 17:00:35.436622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/command/schemas/8.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.436622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/commandAnnotation/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.436622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/commandAnnotation/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-08 17:00:35.436622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/commandAnnotation/schemas/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.252622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/deck/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.248623 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/deck/definitions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.252622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/deck/definitions/3/
--rw-r--r--   0 runner    (1001) docker     (127)    22836 2024-04-08 17:00:35.248623 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/deck/definitions/3/ot2_short_trash.json
--rw-r--r--   0 runner    (1001) docker     (127)    22828 2024-04-08 17:00:35.248623 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/deck/definitions/3/ot2_standard.json
--rw-r--r--   0 runner    (1001) docker     (127)    14062 2024-04-08 17:00:35.252622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/deck/definitions/3/ot3_standard.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.248623 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/deck/definitions/4/
--rw-r--r--   0 runner    (1001) docker     (127)     6517 2024-04-08 17:00:35.248623 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/deck/definitions/4/ot2_short_trash.json
--rw-r--r--   0 runner    (1001) docker     (127)     6493 2024-04-08 17:00:35.248623 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/deck/definitions/4/ot2_standard.json
--rw-r--r--   0 runner    (1001) docker     (127)    10643 2024-04-08 17:00:35.248623 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/deck/definitions/4/ot3_standard.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.252622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/deck/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-04-08 17:00:35.252622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/deck/schemas/1.json
--rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-04-08 17:00:35.252622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/deck/schemas/2.json
--rw-r--r--   0 runner    (1001) docker     (127)     5645 2024-04-08 17:00:35.252622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/deck/schemas/3.json
--rw-r--r--   0 runner    (1001) docker     (127)     7509 2024-04-08 17:00:35.252622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/deck/schemas/4.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.432622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/errors/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.432622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/errors/definitions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.432622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/errors/definitions/1/
--rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-04-08 17:00:35.432622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/errors/definitions/1/errors.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.432622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/errors/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-08 17:00:35.432622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/errors/schemas/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.432622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/gripper/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.428622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/gripper/definitions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.432622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/gripper/definitions/1/
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-08 17:00:35.432622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/gripper/definitions/1/gripperV1.1.json
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-08 17:00:35.432622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/gripper/definitions/1/gripperV1.2.json
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-08 17:00:35.432622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/gripper/definitions/1/gripperV1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.432622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/gripper/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-08 17:00:35.432622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/gripper/schemas/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.344622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.280622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.280622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-08 17:00:35.264622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/12-well-plate.json
--rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-04-08 17:00:35.272622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/24-vial-rack.json
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-04-08 17:00:35.264622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/24-well-plate.json
--rw-r--r--   0 runner    (1001) docker     (127)    49831 2024-04-08 17:00:35.260622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/384-plate.json
--rw-r--r--   0 runner    (1001) docker     (127)     6413 2024-04-08 17:00:35.252622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/48-vial-plate.json
--rw-r--r--   0 runner    (1001) docker     (127)     6798 2024-04-08 17:00:35.256622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/48-well-plate.json
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-04-08 17:00:35.264622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/5ml-3x4.json
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-08 17:00:35.260622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/6-well-plate.json
--rw-r--r--   0 runner    (1001) docker     (127)    12751 2024-04-08 17:00:35.268622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/96-PCR-flat.json
--rw-r--r--   0 runner    (1001) docker     (127)    12764 2024-04-08 17:00:35.272622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/96-PCR-tall.json
--rw-r--r--   0 runner    (1001) docker     (127)    12861 2024-04-08 17:00:35.256622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/96-deep-well.json
--rw-r--r--   0 runner    (1001) docker     (127)    12856 2024-04-08 17:00:35.256622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/96-flat.json
--rw-r--r--   0 runner    (1001) docker     (127)    13059 2024-04-08 17:00:35.272622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/96-well-plate-20mm.json
--rw-r--r--   0 runner    (1001) docker     (127)    44426 2024-04-08 17:00:35.272622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/MALDI-plate.json
--rw-r--r--   0 runner    (1001) docker     (127)    12767 2024-04-08 17:00:35.268622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/PCR-strip-tall.json
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-08 17:00:35.252622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/T25-flask.json
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-08 17:00:35.264622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/T75-flask.json
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-08 17:00:35.264622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/alum-block-pcr-strips.json
--rw-r--r--   0 runner    (1001) docker     (127)    13256 2024-04-08 17:00:35.280622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/biorad-hardshell-96-PCR.json
--rw-r--r--   0 runner    (1001) docker     (127)    11396 2024-04-08 17:00:35.256622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/e-gelgol.json
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-08 17:00:35.264622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/fixed-trash.json
--rw-r--r--   0 runner    (1001) docker     (127)    12454 2024-04-08 17:00:35.276622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/hampton-1ml-deep-block.json
--rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-04-08 17:00:35.260622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/opentrons-aluminum-block-2ml-eppendorf.json
--rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-04-08 17:00:35.268622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/opentrons-aluminum-block-2ml-screwcap.json
--rw-r--r--   0 runner    (1001) docker     (127)    13282 2024-04-08 17:00:35.268622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/opentrons-aluminum-block-96-PCR-plate.json
--rw-r--r--   0 runner    (1001) docker     (127)    13286 2024-04-08 17:00:35.280622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/opentrons-aluminum-block-PCR-strips-200ul.json
--rw-r--r--   0 runner    (1001) docker     (127)    10426 2024-04-08 17:00:35.268622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/opentrons-tiprack-10ul.json
--rw-r--r--   0 runner    (1001) docker     (127)     9948 2024-04-08 17:00:35.276622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/opentrons-tiprack-300ul.json
--rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-04-08 17:00:35.268622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/opentrons-tuberack-1.5ml-eppendorf.json
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-08 17:00:35.264622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/opentrons-tuberack-15_50ml.json
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-08 17:00:35.260622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/opentrons-tuberack-15ml.json
--rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-04-08 17:00:35.256622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/opentrons-tuberack-2ml-eppendorf.json
--rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-04-08 17:00:35.276622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/opentrons-tuberack-2ml-screwcap.json
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-08 17:00:35.272622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/opentrons-tuberack-50ml.json
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-08 17:00:35.276622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/point.json
--rw-r--r--   0 runner    (1001) docker     (127)    24220 2024-04-08 17:00:35.276622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/rigaku-compact-crystallization-plate.json
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-04-08 17:00:35.256622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/small_vial_rack_16x45.json
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-08 17:00:35.264622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/tall-fixed-trash.json
--rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-04-08 17:00:35.260622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/tiprack-1000ul-H.json
--rw-r--r--   0 runner    (1001) docker     (127)     9956 2024-04-08 17:00:35.256622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/tiprack-1000ul-chem.json
--rw-r--r--   0 runner    (1001) docker     (127)     9940 2024-04-08 17:00:35.264622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/tiprack-1000ul.json
--rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-04-08 17:00:35.252622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/tiprack-10ul-H.json
--rw-r--r--   0 runner    (1001) docker     (127)     9936 2024-04-08 17:00:35.276622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/tiprack-10ul.json
--rw-r--r--   0 runner    (1001) docker     (127)     9938 2024-04-08 17:00:35.268622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/tiprack-200ul.json
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-08 17:00:35.272622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/trash-box.json
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-08 17:00:35.264622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/trough-12row-short.json
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-08 17:00:35.268622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/trough-12row.json
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-08 17:00:35.264622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/trough-1row-25ml.json
--rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-04-08 17:00:35.276622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/tube-rack-.75ml.json
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-08 17:00:35.272622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/tube-rack-15_50ml.json
--rw-r--r--   0 runner    (1001) docker     (127)    10168 2024-04-08 17:00:35.260622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/tube-rack-2ml-9x9.json
--rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-04-08 17:00:35.264622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/tube-rack-2ml.json
--rw-r--r--   0 runner    (1001) docker     (127)    12066 2024-04-08 17:00:35.252622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/tube-rack-5ml-96.json
--rw-r--r--   0 runner    (1001) docker     (127)     9856 2024-04-08 17:00:35.264622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/tube-rack-80well.json
--rw-r--r--   0 runner    (1001) docker     (127)     6285 2024-04-08 17:00:35.256622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/wheaton_vial_rack.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.344622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.340622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/agilent_1_reservoir_290ml/
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-08 17:00:35.340622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/agilent_1_reservoir_290ml/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.340622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/appliedbiosystemsmicroamp_384_wellplate_40ul/
--rw-r--r--   0 runner    (1001) docker     (127)    45701 2024-04-08 17:00:35.340622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/appliedbiosystemsmicroamp_384_wellplate_40ul/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.304622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/armadillo_96_wellplate_200ul_pcr_full_skirt/
--rw-r--r--   0 runner    (1001) docker     (127)    12136 2024-04-08 17:00:35.304622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/armadillo_96_wellplate_200ul_pcr_full_skirt/1.json
--rw-r--r--   0 runner    (1001) docker     (127)    12440 2024-04-08 17:00:35.304622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/armadillo_96_wellplate_200ul_pcr_full_skirt/2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.304622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/axygen_1_reservoir_90ml/
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-08 17:00:35.304622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/axygen_1_reservoir_90ml/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.296622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/biorad_384_wellplate_50ul/
--rw-r--r--   0 runner    (1001) docker     (127)    46125 2024-04-08 17:00:35.296622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/biorad_384_wellplate_50ul/1.json
--rw-r--r--   0 runner    (1001) docker     (127)    46174 2024-04-08 17:00:35.296622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/biorad_384_wellplate_50ul/2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.308622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/biorad_96_wellplate_200ul_pcr/
--rw-r--r--   0 runner    (1001) docker     (127)    12276 2024-04-08 17:00:35.308622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/biorad_96_wellplate_200ul_pcr/1.json
--rw-r--r--   0 runner    (1001) docker     (127)    12584 2024-04-08 17:00:35.304622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/biorad_96_wellplate_200ul_pcr/2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.300622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/corning_12_wellplate_6.9ml_flat/
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-04-08 17:00:35.300622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/corning_12_wellplate_6.9ml_flat/1.json
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-08 17:00:35.300622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/corning_12_wellplate_6.9ml_flat/2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.288622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/corning_24_wellplate_3.4ml_flat/
--rw-r--r--   0 runner    (1001) docker     (127)     3672 2024-04-08 17:00:35.288622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/corning_24_wellplate_3.4ml_flat/1.json
--rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-04-08 17:00:35.288622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/corning_24_wellplate_3.4ml_flat/2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.312622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/corning_384_wellplate_112ul_flat/
--rw-r--r--   0 runner    (1001) docker     (127)    56163 2024-04-08 17:00:35.312622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/corning_384_wellplate_112ul_flat/1.json
--rw-r--r--   0 runner    (1001) docker     (127)    56362 2024-04-08 17:00:35.312622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/corning_384_wellplate_112ul_flat/2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.320622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/corning_48_wellplate_1.6ml_flat/
--rw-r--r--   0 runner    (1001) docker     (127)     6501 2024-04-08 17:00:35.320622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/corning_48_wellplate_1.6ml_flat/1.json
--rw-r--r--   0 runner    (1001) docker     (127)     6642 2024-04-08 17:00:35.320622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/corning_48_wellplate_1.6ml_flat/2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.320622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/corning_6_wellplate_16.8ml_flat/
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-08 17:00:35.320622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/corning_6_wellplate_16.8ml_flat/1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-08 17:00:35.320622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/corning_6_wellplate_16.8ml_flat/2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.300622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/corning_96_wellplate_360ul_flat/
--rw-r--r--   0 runner    (1001) docker     (127)    12547 2024-04-08 17:00:35.300622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/corning_96_wellplate_360ul_flat/1.json
--rw-r--r--   0 runner    (1001) docker     (127)    12748 2024-04-08 17:00:35.300622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/corning_96_wellplate_360ul_flat/2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.320622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/eppendorf_96_tiprack_1000ul_eptips/
--rw-r--r--   0 runner    (1001) docker     (127)    11971 2024-04-08 17:00:35.320622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/eppendorf_96_tiprack_1000ul_eptips/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.288622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/eppendorf_96_tiprack_10ul_eptips/
--rw-r--r--   0 runner    (1001) docker     (127)    11580 2024-04-08 17:00:35.288622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/eppendorf_96_tiprack_10ul_eptips/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.328622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/geb_96_tiprack_1000ul/
--rw-r--r--   0 runner    (1001) docker     (127)    11887 2024-04-08 17:00:35.328622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/geb_96_tiprack_1000ul/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.304622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/geb_96_tiprack_10ul/
--rw-r--r--   0 runner    (1001) docker     (127)    11881 2024-04-08 17:00:35.304622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/geb_96_tiprack_10ul/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.336622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/nest_12_reservoir_15ml/
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-08 17:00:35.336622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/nest_12_reservoir_15ml/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.340622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/nest_1_reservoir_195ml/
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-08 17:00:35.340622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/nest_1_reservoir_195ml/1.json
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-08 17:00:35.340622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/nest_1_reservoir_195ml/2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.284622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/nest_1_reservoir_290ml/
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-08 17:00:35.284622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/nest_1_reservoir_290ml/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.344622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/nest_96_wellplate_100ul_pcr_full_skirt/
--rw-r--r--   0 runner    (1001) docker     (127)    12218 2024-04-08 17:00:35.344622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/nest_96_wellplate_100ul_pcr_full_skirt/1.json
--rw-r--r--   0 runner    (1001) docker     (127)    12483 2024-04-08 17:00:35.344622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/nest_96_wellplate_100ul_pcr_full_skirt/2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.288622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/nest_96_wellplate_200ul_flat/
--rw-r--r--   0 runner    (1001) docker     (127)    11987 2024-04-08 17:00:35.288622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/nest_96_wellplate_200ul_flat/1.json
--rw-r--r--   0 runner    (1001) docker     (127)    12186 2024-04-08 17:00:35.288622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/nest_96_wellplate_200ul_flat/2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.328622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/nest_96_wellplate_2ml_deep/
--rw-r--r--   0 runner    (1001) docker     (127)    13764 2024-04-08 17:00:35.328622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/nest_96_wellplate_2ml_deep/1.json
--rw-r--r--   0 runner    (1001) docker     (127)    13970 2024-04-08 17:00:35.328622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/nest_96_wellplate_2ml_deep/2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.300622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_10_tuberack_falcon_4x50ml_6x15ml_conical/
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-04-08 17:00:35.300622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_10_tuberack_falcon_4x50ml_6x15ml_conical/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.308622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_10_tuberack_falcon_4x50ml_6x15ml_conical_acrylic/
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-08 17:00:35.308622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_10_tuberack_falcon_4x50ml_6x15ml_conical_acrylic/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.304622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_10_tuberack_nest_4x50ml_6x15ml_conical/
--rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-04-08 17:00:35.304622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_10_tuberack_nest_4x50ml_6x15ml_conical/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.340622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_15_tuberack_falcon_15ml_conical/
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-04-08 17:00:35.340622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_15_tuberack_falcon_15ml_conical/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.320622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_15_tuberack_nest_15ml_conical/
--rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-04-08 17:00:35.320622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_15_tuberack_nest_15ml_conical/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.292622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_1_trash_1100ml_fixed/
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-08 17:00:35.292622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_1_trash_1100ml_fixed/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.284622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_1_trash_3200ml_fixed/
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-08 17:00:35.284622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_1_trash_3200ml_fixed/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.340622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_1_trash_850ml_fixed/
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-08 17:00:35.340622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_1_trash_850ml_fixed/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.336622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_24_aluminumblock_generic_2ml_screwcap/
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-04-08 17:00:35.336622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_24_aluminumblock_generic_2ml_screwcap/1.json
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-04-08 17:00:35.336622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_24_aluminumblock_generic_2ml_screwcap/2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.308622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_24_aluminumblock_nest_0.5ml_screwcap/
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-08 17:00:35.308622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_24_aluminumblock_nest_0.5ml_screwcap/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.328622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_24_aluminumblock_nest_1.5ml_screwcap/
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-08 17:00:35.328622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_24_aluminumblock_nest_1.5ml_screwcap/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.288622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_24_aluminumblock_nest_1.5ml_snapcap/
--rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-04-08 17:00:35.288622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_24_aluminumblock_nest_1.5ml_snapcap/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.284622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_24_aluminumblock_nest_2ml_screwcap/
--rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-04-08 17:00:35.284622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_24_aluminumblock_nest_2ml_screwcap/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.292622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_24_aluminumblock_nest_2ml_snapcap/
--rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-04-08 17:00:35.292622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_24_aluminumblock_nest_2ml_snapcap/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.336622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_24_tuberack_eppendorf_1.5ml_safelock_snapcap/
--rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-04-08 17:00:35.336622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_24_tuberack_eppendorf_1.5ml_safelock_snapcap/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.324622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_24_tuberack_eppendorf_2ml_safelock_snapcap/
--rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-04-08 17:00:35.324622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_24_tuberack_eppendorf_2ml_safelock_snapcap/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.336622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_24_tuberack_eppendorf_2ml_safelock_snapcap_acrylic/
--rw-r--r--   0 runner    (1001) docker     (127)     3852 2024-04-08 17:00:35.336622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_24_tuberack_eppendorf_2ml_safelock_snapcap_acrylic/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.324622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_24_tuberack_generic_0.75ml_snapcap_acrylic/
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-08 17:00:35.324622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_24_tuberack_generic_0.75ml_snapcap_acrylic/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.280622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_24_tuberack_generic_2ml_screwcap/
--rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-04-08 17:00:35.280622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_24_tuberack_generic_2ml_screwcap/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.308622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_24_tuberack_nest_0.5ml_screwcap/
--rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-04-08 17:00:35.308622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_24_tuberack_nest_0.5ml_screwcap/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.284622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_24_tuberack_nest_1.5ml_screwcap/
--rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-04-08 17:00:35.284622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_24_tuberack_nest_1.5ml_screwcap/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.328622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_24_tuberack_nest_1.5ml_snapcap/
--rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-04-08 17:00:35.328622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_24_tuberack_nest_1.5ml_snapcap/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.280622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_24_tuberack_nest_2ml_screwcap/
--rw-r--r--   0 runner    (1001) docker     (127)     3741 2024-04-08 17:00:35.280622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_24_tuberack_nest_2ml_screwcap/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.304622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_24_tuberack_nest_2ml_snapcap/
--rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-04-08 17:00:35.304622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_24_tuberack_nest_2ml_snapcap/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.332622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_40_aluminumblock_eppendorf_24x2ml_safelock_snapcap_generic_16x0.2ml_pcr_strip/
--rw-r--r--   0 runner    (1001) docker     (127)     5902 2024-04-08 17:00:35.332622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_40_aluminumblock_eppendorf_24x2ml_safelock_snapcap_generic_16x0.2ml_pcr_strip/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.284622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_6_tuberack_falcon_50ml_conical/
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-04-08 17:00:35.284622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_6_tuberack_falcon_50ml_conical/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.308622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_6_tuberack_nest_50ml_conical/
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-08 17:00:35.308622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_6_tuberack_nest_50ml_conical/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.308622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_96_aluminumblock_biorad_wellplate_200ul/
--rw-r--r--   0 runner    (1001) docker     (127)    12264 2024-04-08 17:00:35.308622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_96_aluminumblock_biorad_wellplate_200ul/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.300622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_96_aluminumblock_generic_pcr_strip_200ul/
--rw-r--r--   0 runner    (1001) docker     (127)    12282 2024-04-08 17:00:35.300622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_96_aluminumblock_generic_pcr_strip_200ul/1.json
--rw-r--r--   0 runner    (1001) docker     (127)    12316 2024-04-08 17:00:35.296622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_96_aluminumblock_generic_pcr_strip_200ul/2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.316622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_96_aluminumblock_nest_wellplate_100ul/
--rw-r--r--   0 runner    (1001) docker     (127)    12373 2024-04-08 17:00:35.316622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_96_aluminumblock_nest_wellplate_100ul/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.316622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_96_deep_well_adapter/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-08 17:00:35.316622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_96_deep_well_adapter/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.308622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_96_deep_well_adapter_nest_wellplate_2ml_deep/
--rw-r--r--   0 runner    (1001) docker     (127)    14139 2024-04-08 17:00:35.308622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_96_deep_well_adapter_nest_wellplate_2ml_deep/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.320622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_96_filtertiprack_1000ul/
--rw-r--r--   0 runner    (1001) docker     (127)    11943 2024-04-08 17:00:35.320622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_96_filtertiprack_1000ul/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.300622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_96_filtertiprack_10ul/
--rw-r--r--   0 runner    (1001) docker     (127)    12037 2024-04-08 17:00:35.300622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_96_filtertiprack_10ul/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.292622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_96_filtertiprack_200ul/
--rw-r--r--   0 runner    (1001) docker     (127)    12039 2024-04-08 17:00:35.292622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_96_filtertiprack_200ul/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.316622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_96_filtertiprack_20ul/
--rw-r--r--   0 runner    (1001) docker     (127)    12037 2024-04-08 17:00:35.316622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_96_filtertiprack_20ul/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.292622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_96_flat_bottom_adapter/
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-08 17:00:35.292622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_96_flat_bottom_adapter/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.292622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_96_flat_bottom_adapter_nest_wellplate_200ul_flat/
--rw-r--r--   0 runner    (1001) docker     (127)    12347 2024-04-08 17:00:35.292622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_96_flat_bottom_adapter_nest_wellplate_200ul_flat/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.280622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_96_pcr_adapter/
--rw-r--r--   0 runner    (1001) docker     (127)    11150 2024-04-08 17:00:35.280622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_96_pcr_adapter/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.336622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_96_pcr_adapter_armadillo_wellplate_200ul/
--rw-r--r--   0 runner    (1001) docker     (127)    12358 2024-04-08 17:00:35.336622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_96_pcr_adapter_armadillo_wellplate_200ul/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.284622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_96_pcr_adapter_nest_wellplate_100ul_pcr_full_skirt/
--rw-r--r--   0 runner    (1001) docker     (127)    12419 2024-04-08 17:00:35.284622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_96_pcr_adapter_nest_wellplate_100ul_pcr_full_skirt/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.344622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_96_tiprack_1000ul/
--rw-r--r--   0 runner    (1001) docker     (127)    12016 2024-04-08 17:00:35.344622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_96_tiprack_1000ul/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.336622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_96_tiprack_10ul/
--rw-r--r--   0 runner    (1001) docker     (127)    12108 2024-04-08 17:00:35.336622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_96_tiprack_10ul/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.320622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_96_tiprack_20ul/
--rw-r--r--   0 runner    (1001) docker     (127)    12108 2024-04-08 17:00:35.320622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_96_tiprack_20ul/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.288622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_96_tiprack_300ul/
--rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-04-08 17:00:35.288622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_96_tiprack_300ul/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.332622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_96_well_aluminum_block/
--rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-04-08 17:00:35.332622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_96_well_aluminum_block/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.332622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_96_wellplate_200ul_pcr_full_skirt/
--rw-r--r--   0 runner    (1001) docker     (127)    12130 2024-04-08 17:00:35.332622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_96_wellplate_200ul_pcr_full_skirt/1.json
--rw-r--r--   0 runner    (1001) docker     (127)    12434 2024-04-08 17:00:35.332622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_96_wellplate_200ul_pcr_full_skirt/2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.280622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_aluminum_flat_bottom_plate/
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-08 17:00:35.280622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_aluminum_flat_bottom_plate/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.332622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_calibration_adapter_heatershaker_module/
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-08 17:00:35.332622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_calibration_adapter_heatershaker_module/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.332622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_calibration_adapter_temperature_module/
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-08 17:00:35.332622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_calibration_adapter_temperature_module/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.324622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_calibration_adapter_thermocycler_module/
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-08 17:00:35.324622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_calibration_adapter_thermocycler_module/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.316622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_calibrationblock_short_side_left/
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-08 17:00:35.316622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_calibrationblock_short_side_left/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.284622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_calibrationblock_short_side_right/
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-08 17:00:35.284622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_calibrationblock_short_side_right/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.288622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_flex_96_filtertiprack_1000ul/
--rw-r--r--   0 runner    (1001) docker     (127)    12182 2024-04-08 17:00:35.288622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_flex_96_filtertiprack_1000ul/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.328622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_flex_96_filtertiprack_200ul/
--rw-r--r--   0 runner    (1001) docker     (127)    12085 2024-04-08 17:00:35.328622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_flex_96_filtertiprack_200ul/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.292622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_flex_96_filtertiprack_50ul/
--rw-r--r--   0 runner    (1001) docker     (127)    11986 2024-04-08 17:00:35.292622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_flex_96_filtertiprack_50ul/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.316622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_flex_96_tiprack_1000ul/
--rw-r--r--   0 runner    (1001) docker     (127)    12169 2024-04-08 17:00:35.316622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_flex_96_tiprack_1000ul/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.324622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_flex_96_tiprack_200ul/
--rw-r--r--   0 runner    (1001) docker     (127)    12072 2024-04-08 17:00:35.324622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_flex_96_tiprack_200ul/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.340622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_flex_96_tiprack_50ul/
--rw-r--r--   0 runner    (1001) docker     (127)    11973 2024-04-08 17:00:35.340622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_flex_96_tiprack_50ul/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.292622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_flex_96_tiprack_adapter/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-08 17:00:35.292622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_flex_96_tiprack_adapter/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.316622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_universal_flat_adapter/
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-08 17:00:35.316622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_universal_flat_adapter/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.324622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_universal_flat_adapter_corning_384_wellplate_112ul_flat/
--rw-r--r--   0 runner    (1001) docker     (127)    56413 2024-04-08 17:00:35.324622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_universal_flat_adapter_corning_384_wellplate_112ul_flat/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.332622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/thermoscientificnunc_96_wellplate_1300ul/
--rw-r--r--   0 runner    (1001) docker     (127)    11975 2024-04-08 17:00:35.332622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/thermoscientificnunc_96_wellplate_1300ul/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.316622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/thermoscientificnunc_96_wellplate_2000ul/
--rw-r--r--   0 runner    (1001) docker     (127)    11875 2024-04-08 17:00:35.316622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/thermoscientificnunc_96_wellplate_2000ul/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.344622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/tipone_96_tiprack_200ul/
--rw-r--r--   0 runner    (1001) docker     (127)    12162 2024-04-08 17:00:35.344622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/tipone_96_tiprack_200ul/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.284622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/usascientific_12_reservoir_22ml/
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-08 17:00:35.284622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/usascientific_12_reservoir_22ml/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.280622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/usascientific_96_wellplate_2.4ml_deep/
--rw-r--r--   0 runner    (1001) docker     (127)    13960 2024-04-08 17:00:35.280622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/usascientific_96_wellplate_2.4ml_deep/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.344622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     8879 2024-04-08 17:00:35.344622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/schemas/2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.436622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/liquid/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.436622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/liquid/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-08 17:00:35.436622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/liquid/schemas/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.352622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/module/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.348622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/module/definitions/
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-08 17:00:35.344622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/module/definitions/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.348622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/module/definitions/2/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-08 17:00:35.344622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/module/definitions/2/magneticModuleV1.json
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-08 17:00:35.348622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/module/definitions/2/magneticModuleV2.json
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-08 17:00:35.348622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/module/definitions/2/temperatureModuleV1.json
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-08 17:00:35.348622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/module/definitions/2/temperatureModuleV2.json
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-08 17:00:35.348622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/module/definitions/2/thermocyclerModuleV1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.352622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/module/definitions/3/
--rw-r--r--   0 runner    (1001) docker     (127)    10821 2024-04-08 17:00:35.348622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/module/definitions/3/heaterShakerModuleV1.json
--rw-r--r--   0 runner    (1001) docker     (127)    78832 2024-04-08 17:00:35.348622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/module/definitions/3/magneticBlockV1.json
--rw-r--r--   0 runner    (1001) docker     (127)     8689 2024-04-08 17:00:35.348622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/module/definitions/3/magneticModuleV1.json
--rw-r--r--   0 runner    (1001) docker     (127)     9131 2024-04-08 17:00:35.348622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/module/definitions/3/magneticModuleV2.json
--rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-04-08 17:00:35.348622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/module/definitions/3/temperatureModuleV1.json
--rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-04-08 17:00:35.348622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/module/definitions/3/temperatureModuleV2.json
--rw-r--r--   0 runner    (1001) docker     (127)    38434 2024-04-08 17:00:35.348622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/module/definitions/3/thermocyclerModuleV1.json
--rw-r--r--   0 runner    (1001) docker     (127)    60037 2024-04-08 17:00:35.352622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/module/definitions/3/thermocyclerModuleV2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.352622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/module/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-08 17:00:35.352622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/module/schemas/1.json
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-08 17:00:35.352622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/module/schemas/2.json
--rw-r--r--   0 runner    (1001) docker     (127)     5427 2024-04-08 17:00:35.352622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/module/schemas/3.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.424622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.360622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.360622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/1/
--rw-r--r--   0 runner    (1001) docker     (127)   160656 2024-04-08 17:00:35.360622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/1/pipetteModelSpecs.json
--rw-r--r--   0 runner    (1001) docker     (127)    11476 2024-04-08 17:00:35.352622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/1/pipetteNameSpecs.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.408622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.404622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.404622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.400622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p10/
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-08 17:00:35.400622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p10/1_0.json
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-08 17:00:35.400622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p10/1_3.json
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-08 17:00:35.400622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p10/1_4.json
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-08 17:00:35.400622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p10/1_5.json
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-08 17:00:35.400622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p10/1_6.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.404622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p1000/
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-08 17:00:35.400622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p1000/1_0.json
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-08 17:00:35.400622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p1000/3_0.json
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-08 17:00:35.400622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p1000/3_3.json
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-08 17:00:35.404622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p1000/3_4.json
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-08 17:00:35.400622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p1000/3_5.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.400622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p20/
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-08 17:00:35.400622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p20/2_0.json
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-08 17:00:35.400622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p20/2_1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.400622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p300/
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-08 17:00:35.396622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p300/1_0.json
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-08 17:00:35.400622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p300/1_3.json
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-08 17:00:35.396622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p300/1_4.json
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-08 17:00:35.400622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p300/1_5.json
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-08 17:00:35.400622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p300/2_0.json
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-08 17:00:35.400622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p300/2_1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.404622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p50/
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-08 17:00:35.404622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p50/1_0.json
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-08 17:00:35.404622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p50/1_3.json
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-08 17:00:35.404622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p50/1_4.json
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-08 17:00:35.404622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p50/1_5.json
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-08 17:00:35.404622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p50/3_0.json
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-08 17:00:35.404622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p50/3_3.json
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-08 17:00:35.404622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p50/3_4.json
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-08 17:00:35.404622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p50/3_5.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.404622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/ninety_six_channel/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.408622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/ninety_six_channel/p1000/
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-08 17:00:35.404622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/ninety_six_channel/p1000/1_0.json
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-08 17:00:35.404622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/ninety_six_channel/p1000/3_0.json
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-08 17:00:35.408622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/ninety_six_channel/p1000/3_3.json
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-04-08 17:00:35.408622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/ninety_six_channel/p1000/3_4.json
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-08 17:00:35.404622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/ninety_six_channel/p1000/3_5.json
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-08 17:00:35.408622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/ninety_six_channel/p1000/3_6.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.396622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.392622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p10/
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-08 17:00:35.392622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p10/1_0.json
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-08 17:00:35.392622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p10/1_3.json
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-08 17:00:35.392622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p10/1_4.json
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-08 17:00:35.392622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p10/1_5.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.396622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p1000/
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-08 17:00:35.392622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p1000/1_0.json
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-08 17:00:35.392622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p1000/1_3.json
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-08 17:00:35.392622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p1000/1_4.json
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-08 17:00:35.396622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p1000/1_5.json
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-08 17:00:35.396622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p1000/2_0.json
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-08 17:00:35.396622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p1000/2_1.json
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-08 17:00:35.392622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p1000/2_2.json
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-08 17:00:35.392622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p1000/3_0.json
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-08 17:00:35.396622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p1000/3_3.json
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-08 17:00:35.396622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p1000/3_4.json
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-08 17:00:35.392622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p1000/3_5.json
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-08 17:00:35.396622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p1000/3_6.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.392622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p20/
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-08 17:00:35.392622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p20/2_0.json
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-08 17:00:35.392622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p20/2_1.json
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-08 17:00:35.392622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p20/2_2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.392622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p300/
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-08 17:00:35.388622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p300/1_0.json
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-08 17:00:35.388622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p300/1_3.json
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-08 17:00:35.388622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p300/1_4.json
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-08 17:00:35.392622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p300/1_5.json
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-08 17:00:35.392622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p300/2_0.json
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-08 17:00:35.392622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p300/2_1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.396622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p50/
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-08 17:00:35.396622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p50/1_0.json
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-08 17:00:35.396622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p50/1_3.json
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-08 17:00:35.396622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p50/1_4.json
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-08 17:00:35.396622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p50/1_5.json
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-08 17:00:35.396622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p50/3_0.json
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-08 17:00:35.396622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p50/3_3.json
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-08 17:00:35.396622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p50/3_4.json
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-08 17:00:35.396622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p50/3_5.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.420622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.420622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.416622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p10/
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-08 17:00:35.416622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p10/1_0.json
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-08 17:00:35.416622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p10/1_3.json
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-08 17:00:35.416622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p10/1_4.json
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-08 17:00:35.416622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p10/1_5.json
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-08 17:00:35.416622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p10/1_6.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.420622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p1000/
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-08 17:00:35.420622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p1000/1_0.json
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-08 17:00:35.420622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p1000/3_0.json
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-08 17:00:35.420622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p1000/3_3.json
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-08 17:00:35.420622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p1000/3_4.json
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-08 17:00:35.420622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p1000/3_5.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.420622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p20/
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-08 17:00:35.420622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p20/2_0.json
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-08 17:00:35.420622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p20/2_1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.416622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p300/
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-08 17:00:35.416622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p300/1_0.json
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-08 17:00:35.416622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p300/1_3.json
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-08 17:00:35.416622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p300/1_4.json
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-08 17:00:35.416622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p300/1_5.json
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-08 17:00:35.416622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p300/2_0.json
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-08 17:00:35.416622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p300/2_1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.420622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p50/
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-08 17:00:35.420622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p50/1_0.json
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-08 17:00:35.420622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p50/1_3.json
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-08 17:00:35.420622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p50/1_4.json
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-08 17:00:35.420622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p50/1_5.json
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-08 17:00:35.420622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p50/3_0.json
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-08 17:00:35.420622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p50/3_3.json
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-08 17:00:35.420622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p50/3_4.json
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-08 17:00:35.420622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p50/3_5.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.420622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/ninety_six_channel/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.424622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/ninety_six_channel/p1000/
--rw-r--r--   0 runner    (1001) docker     (127)     4508 2024-04-08 17:00:35.424622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/ninety_six_channel/p1000/1_0.json
--rw-r--r--   0 runner    (1001) docker     (127)     4508 2024-04-08 17:00:35.424622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/ninety_six_channel/p1000/3_0.json
--rw-r--r--   0 runner    (1001) docker     (127)     4508 2024-04-08 17:00:35.424622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/ninety_six_channel/p1000/3_3.json
--rw-r--r--   0 runner    (1001) docker     (127)     4508 2024-04-08 17:00:35.424622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/ninety_six_channel/p1000/3_4.json
--rw-r--r--   0 runner    (1001) docker     (127)     4508 2024-04-08 17:00:35.424622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/ninety_six_channel/p1000/3_5.json
--rw-r--r--   0 runner    (1001) docker     (127)     4508 2024-04-08 17:00:35.424622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/ninety_six_channel/p1000/3_6.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.412622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.408622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p10/
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-08 17:00:35.408622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p10/1_0.json
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-08 17:00:35.408622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p10/1_3.json
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-08 17:00:35.408622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p10/1_4.json
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-08 17:00:35.408622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p10/1_5.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.412622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p1000/
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-08 17:00:35.412622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p1000/1_0.json
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-08 17:00:35.412622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p1000/1_3.json
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-08 17:00:35.412622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p1000/1_4.json
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-08 17:00:35.412622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p1000/1_5.json
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-08 17:00:35.412622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p1000/2_0.json
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-08 17:00:35.412622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p1000/2_1.json
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-08 17:00:35.412622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p1000/2_2.json
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-08 17:00:35.412622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p1000/3_0.json
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-08 17:00:35.412622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p1000/3_3.json
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-08 17:00:35.412622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p1000/3_4.json
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-08 17:00:35.412622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p1000/3_5.json
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-08 17:00:35.412622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p1000/3_6.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.412622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p20/
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-08 17:00:35.412622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p20/2_0.json
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-08 17:00:35.412622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p20/2_1.json
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-08 17:00:35.408622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p20/2_2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.408622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p300/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-08 17:00:35.408622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p300/1_0.json
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-08 17:00:35.408622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p300/1_3.json
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-08 17:00:35.408622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p300/1_4.json
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-08 17:00:35.408622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p300/1_5.json
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-08 17:00:35.408622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p300/2_0.json
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-08 17:00:35.408622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p300/2_1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.416622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p50/
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-08 17:00:35.412622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p50/1_0.json
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-08 17:00:35.416622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p50/1_3.json
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-08 17:00:35.412622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p50/1_4.json
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-08 17:00:35.416622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p50/1_5.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-08 17:00:35.412622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p50/3_0.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-08 17:00:35.416622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p50/3_3.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-08 17:00:35.416622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p50/3_4.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-08 17:00:35.416622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p50/3_5.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.388622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.384622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.376622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p10/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.380622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p10/default/
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-08 17:00:35.376622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p10/default/1_0.json
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-08 17:00:35.376622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p10/default/1_3.json
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-08 17:00:35.376622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p10/default/1_4.json
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-08 17:00:35.376622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p10/default/1_5.json
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-08 17:00:35.380622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p10/default/1_6.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.380622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p1000/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.384622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p1000/default/
--rw-r--r--   0 runner    (1001) docker     (127)     7812 2024-04-08 17:00:35.380622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p1000/default/1_0.json
--rw-r--r--   0 runner    (1001) docker     (127)     7987 2024-04-08 17:00:35.380622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p1000/default/3_0.json
--rw-r--r--   0 runner    (1001) docker     (127)     7987 2024-04-08 17:00:35.380622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p1000/default/3_3.json
--rw-r--r--   0 runner    (1001) docker     (127)     8005 2024-04-08 17:00:35.384622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p1000/default/3_4.json
--rw-r--r--   0 runner    (1001) docker     (127)     5315 2024-04-08 17:00:35.380622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p1000/default/3_5.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.380622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p20/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.380622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p20/default/
--rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-04-08 17:00:35.380622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p20/default/2_0.json
--rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-04-08 17:00:35.380622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p20/default/2_1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.376622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p300/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.376622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p300/default/
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-08 17:00:35.376622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p300/default/1_0.json
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-08 17:00:35.376622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p300/default/1_3.json
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-08 17:00:35.376622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p300/default/1_4.json
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-08 17:00:35.376622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p300/default/1_5.json
--rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-04-08 17:00:35.376622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p300/default/2_0.json
--rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-04-08 17:00:35.376622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p300/default/2_1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.384622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p50/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.388622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p50/default/
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-04-08 17:00:35.384622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p50/default/1_0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-04-08 17:00:35.384622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p50/default/1_3.json
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-04-08 17:00:35.384622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p50/default/1_4.json
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-08 17:00:35.384622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p50/default/1_5.json
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-04-08 17:00:35.384622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p50/default/3_0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-04-08 17:00:35.384622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p50/default/3_3.json
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-04-08 17:00:35.388622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p50/default/3_4.json
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-08 17:00:35.384622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p50/default/3_5.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.384622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p50/lowVolumeDefault/
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-08 17:00:35.384622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p50/lowVolumeDefault/3_0.json
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-08 17:00:35.384622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p50/lowVolumeDefault/3_3.json
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-08 17:00:35.384622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p50/lowVolumeDefault/3_4.json
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-08 17:00:35.384622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p50/lowVolumeDefault/3_5.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.388622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/ninety_six_channel/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.388622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/ninety_six_channel/p1000/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.388622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/ninety_six_channel/p1000/default/
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-04-08 17:00:35.388622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/ninety_six_channel/p1000/default/1_0.json
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-04-08 17:00:35.388622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/ninety_six_channel/p1000/default/3_0.json
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-04-08 17:00:35.388622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/ninety_six_channel/p1000/default/3_3.json
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-04-08 17:00:35.388622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/ninety_six_channel/p1000/default/3_4.json
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-04-08 17:00:35.388622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/ninety_six_channel/p1000/default/3_5.json
--rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-04-08 17:00:35.388622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/ninety_six_channel/p1000/default/3_6.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.372622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.364622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p10/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.364622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p10/default/
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-08 17:00:35.364622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p10/default/1_0.json
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-08 17:00:35.364622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p10/default/1_3.json
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-08 17:00:35.364622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p10/default/1_4.json
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-08 17:00:35.364622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p10/default/1_5.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.368622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p1000/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.372622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p1000/default/
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-08 17:00:35.368622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p1000/default/1_0.json
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-08 17:00:35.368622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p1000/default/1_3.json
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-08 17:00:35.368622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p1000/default/1_4.json
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-08 17:00:35.368622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p1000/default/1_5.json
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-08 17:00:35.372622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p1000/default/2_0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-04-08 17:00:35.368622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p1000/default/2_1.json
--rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-04-08 17:00:35.368622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p1000/default/2_2.json
--rw-r--r--   0 runner    (1001) docker     (127)     7812 2024-04-08 17:00:35.368622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p1000/default/3_0.json
--rw-r--r--   0 runner    (1001) docker     (127)     7812 2024-04-08 17:00:35.368622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p1000/default/3_3.json
--rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-04-08 17:00:35.372622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p1000/default/3_4.json
--rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-04-08 17:00:35.368622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p1000/default/3_5.json
--rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-04-08 17:00:35.368622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p1000/default/3_6.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.364622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p20/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.368622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p20/default/
--rw-r--r--   0 runner    (1001) docker     (127)     9689 2024-04-08 17:00:35.368622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p20/default/2_0.json
--rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-04-08 17:00:35.364622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p20/default/2_1.json
--rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-04-08 17:00:35.364622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p20/default/2_2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.360622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p300/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.364622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p300/default/
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-08 17:00:35.360622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p300/default/1_0.json
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-08 17:00:35.360622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p300/default/1_3.json
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-08 17:00:35.360622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p300/default/1_4.json
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-08 17:00:35.364622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p300/default/1_5.json
--rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-04-08 17:00:35.364622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p300/default/2_0.json
--rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-04-08 17:00:35.364622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p300/default/2_1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.372622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p50/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.376622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p50/default/
--rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-04-08 17:00:35.372622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p50/default/1_0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-04-08 17:00:35.372622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p50/default/1_3.json
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-04-08 17:00:35.372622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p50/default/1_4.json
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-04-08 17:00:35.376622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p50/default/1_5.json
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-04-08 17:00:35.372622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p50/default/3_0.json
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-04-08 17:00:35.372622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p50/default/3_3.json
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-08 17:00:35.376622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p50/default/3_4.json
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-04-08 17:00:35.372622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p50/default/3_5.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.372622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p50/lowVolumeDefault/
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-08 17:00:35.372622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p50/lowVolumeDefault/3_0.json
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-08 17:00:35.372622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p50/lowVolumeDefault/3_3.json
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-08 17:00:35.372622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p50/lowVolumeDefault/3_4.json
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-08 17:00:35.372622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p50/lowVolumeDefault/3_5.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.424622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/schemas/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.424622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/schemas/1/
--rw-r--r--   0 runner    (1001) docker     (127)     3920 2024-04-08 17:00:35.424622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/schemas/1/pipetteModelSpecsSchema.json
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-08 17:00:35.424622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/schemas/1/pipetteNameSpecsSchema.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.424622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/schemas/2/
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-08 17:00:35.424622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/schemas/2/pipetteGeometrySchema.json
--rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-04-08 17:00:35.424622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/schemas/2/pipetteLiquidPropertiesSchema.json
--rw-r--r--   0 runner    (1001) docker     (127)     6316 2024-04-08 17:00:35.424622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/schemas/2/pipettePropertiesSchema.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.428622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/protocol/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.428622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/protocol/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     7657 2024-04-08 17:00:35.428622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/protocol/schemas/1.json
--rw-r--r--   0 runner    (1001) docker     (127)     9131 2024-04-08 17:00:35.428622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/protocol/schemas/2.json
--rw-r--r--   0 runner    (1001) docker     (127)     7691 2024-04-08 17:00:35.428622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/protocol/schemas/3.json
--rw-r--r--   0 runner    (1001) docker     (127)    15234 2024-04-08 17:00:35.428622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/protocol/schemas/4.json
--rw-r--r--   0 runner    (1001) docker     (127)    16750 2024-04-08 17:00:35.428622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/protocol/schemas/5.json
--rw-r--r--   0 runner    (1001) docker     (127)    29434 2024-04-08 17:00:35.428622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/protocol/schemas/6.json
--rw-r--r--   0 runner    (1001) docker     (127)     5959 2024-04-08 17:00:35.428622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/protocol/schemas/7.json
--rw-r--r--   0 runner    (1001) docker     (127)     3468 2024-04-08 17:00:35.428622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/protocol/schemas/8.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.432622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/robot/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.432622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/robot/definitions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.432622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/robot/definitions/1/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-08 17:00:35.432622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/robot/definitions/1/ot2.json
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-08 17:00:35.432622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/robot/definitions/1/ot3.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.432622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/robot/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-08 17:00:35.432622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/robot/schemas/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.440622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/deck/
--rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-04-08 16:59:17.000000 opentrons_shared_data-7.2.2a3/opentrons_shared_data/deck/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-04-08 16:59:17.000000 opentrons_shared_data-7.2.2a3/opentrons_shared_data/deck/dev_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.444622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-08 16:59:17.000000 opentrons_shared_data-7.2.2a3/opentrons_shared_data/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-08 16:59:17.000000 opentrons_shared_data-7.2.2a3/opentrons_shared_data/errors/categories.py
--rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-04-08 16:59:17.000000 opentrons_shared_data-7.2.2a3/opentrons_shared_data/errors/codes.py
--rw-r--r--   0 runner    (1001) docker     (127)    32183 2024-04-08 16:59:17.000000 opentrons_shared_data-7.2.2a3/opentrons_shared_data/errors/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.444622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/gripper/
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-04-08 16:59:17.000000 opentrons_shared_data-7.2.2a3/opentrons_shared_data/gripper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-08 16:59:17.000000 opentrons_shared_data-7.2.2a3/opentrons_shared_data/gripper/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-04-08 16:59:17.000000 opentrons_shared_data-7.2.2a3/opentrons_shared_data/gripper/gripper_definition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.444622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/labware/
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-08 16:59:17.000000 opentrons_shared_data-7.2.2a3/opentrons_shared_data/labware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-08 16:59:17.000000 opentrons_shared_data-7.2.2a3/opentrons_shared_data/labware/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-04-08 16:59:17.000000 opentrons_shared_data-7.2.2a3/opentrons_shared_data/labware/dev_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    10135 2024-04-08 16:59:17.000000 opentrons_shared_data-7.2.2a3/opentrons_shared_data/labware/labware_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-08 16:59:17.000000 opentrons_shared_data-7.2.2a3/opentrons_shared_data/load.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.444622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/module/
--rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-04-08 16:59:17.000000 opentrons_shared_data-7.2.2a3/opentrons_shared_data/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-04-08 16:59:17.000000 opentrons_shared_data-7.2.2a3/opentrons_shared_data/module/dev_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.444622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/pipette/
--rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-04-08 16:59:17.000000 opentrons_shared_data-7.2.2a3/opentrons_shared_data/pipette/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-04-08 16:59:17.000000 opentrons_shared_data-7.2.2a3/opentrons_shared_data/pipette/dev_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-08 16:59:17.000000 opentrons_shared_data-7.2.2a3/opentrons_shared_data/pipette/file_operation_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8723 2024-04-08 16:59:17.000000 opentrons_shared_data-7.2.2a3/opentrons_shared_data/pipette/load_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-04-08 16:59:17.000000 opentrons_shared_data-7.2.2a3/opentrons_shared_data/pipette/model_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    16027 2024-04-08 16:59:17.000000 opentrons_shared_data-7.2.2a3/opentrons_shared_data/pipette/mutable_configurations.py
--rw-r--r--   0 runner    (1001) docker     (127)    18513 2024-04-08 16:59:17.000000 opentrons_shared_data-7.2.2a3/opentrons_shared_data/pipette/pipette_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     7953 2024-04-08 16:59:17.000000 opentrons_shared_data-7.2.2a3/opentrons_shared_data/pipette/pipette_load_name_conversions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.444622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/pipette/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 16:59:17.000000 opentrons_shared_data-7.2.2a3/opentrons_shared_data/pipette/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18509 2024-04-08 16:59:17.000000 opentrons_shared_data-7.2.2a3/opentrons_shared_data/pipette/scripts/build_json_script.py
--rw-r--r--   0 runner    (1001) docker     (127)    16374 2024-04-08 16:59:17.000000 opentrons_shared_data-7.2.2a3/opentrons_shared_data/pipette/scripts/update_configuration_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     4767 2024-04-08 16:59:17.000000 opentrons_shared_data-7.2.2a3/opentrons_shared_data/pipette/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.448622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/protocol/
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-08 16:59:17.000000 opentrons_shared_data-7.2.2a3/opentrons_shared_data/protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-04-08 16:59:17.000000 opentrons_shared_data-7.2.2a3/opentrons_shared_data/protocol/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    11397 2024-04-08 16:59:17.000000 opentrons_shared_data-7.2.2a3/opentrons_shared_data/protocol/dev_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.448622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/protocol/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-08 16:59:17.000000 opentrons_shared_data-7.2.2a3/opentrons_shared_data/protocol/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4833 2024-04-08 16:59:17.000000 opentrons_shared_data-7.2.2a3/opentrons_shared_data/protocol/models/protocol_schema_v6.py
--rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-04-08 16:59:17.000000 opentrons_shared_data-7.2.2a3/opentrons_shared_data/protocol/models/protocol_schema_v7.py
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-08 16:59:17.000000 opentrons_shared_data-7.2.2a3/opentrons_shared_data/protocol/models/protocol_schema_v8.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-08 16:59:17.000000 opentrons_shared_data-7.2.2a3/opentrons_shared_data/protocol/models/shared_models.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 16:59:17.000000 opentrons_shared_data-7.2.2a3/opentrons_shared_data/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.448622 opentrons_shared_data-7.2.2a3/opentrons_shared_data/robot/
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-08 16:59:17.000000 opentrons_shared_data-7.2.2a3/opentrons_shared_data/robot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-08 16:59:17.000000 opentrons_shared_data-7.2.2a3/opentrons_shared_data/robot/dev_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:00:35.448622 opentrons_shared_data-7.2.2a3/opentrons_shared_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-08 17:00:35.000000 opentrons_shared_data-7.2.2a3/opentrons_shared_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-04-08 17:00:35.000000 opentrons_shared_data-7.2.2a3/opentrons_shared_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 17:00:35.000000 opentrons_shared_data-7.2.2a3/opentrons_shared_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 17:00:18.000000 opentrons_shared_data-7.2.2a3/opentrons_shared_data.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 17:00:35.000000 opentrons_shared_data-7.2.2a3/opentrons_shared_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-08 17:00:35.000000 opentrons_shared_data-7.2.2a3/opentrons_shared_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-08 17:00:35.448622 opentrons_shared_data-7.2.2a3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5694 2024-04-08 16:59:17.000000 opentrons_shared_data-7.2.2a3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.788448 opentrons_shared_data-7.3.0a0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-02 12:07:30.788448 opentrons_shared_data-7.3.0a0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.780448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-02 12:06:44.000000 opentrons_shared_data-7.3.0a0/opentrons_shared_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-02 12:06:44.000000 opentrons_shared_data-7.3.0a0/opentrons_shared_data/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.780448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/command/
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-02 12:06:44.000000 opentrons_shared_data-7.3.0a0/opentrons_shared_data/command/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.776448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.772448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/command/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.776448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/command/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)    97753 2024-05-02 12:07:30.776448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/command/schemas/7.json
+-rw-r--r--   0 runner    (1001) docker     (127)   123091 2024-05-02 12:07:30.776448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/command/schemas/8.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.776448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/commandAnnotation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.776448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/commandAnnotation/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-02 12:07:30.776448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/commandAnnotation/schemas/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.592448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/deck/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.588448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/deck/definitions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.588448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/deck/definitions/3/
+-rw-r--r--   0 runner    (1001) docker     (127)    22836 2024-05-02 12:07:30.588448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/deck/definitions/3/ot2_short_trash.json
+-rw-r--r--   0 runner    (1001) docker     (127)    22828 2024-05-02 12:07:30.588448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/deck/definitions/3/ot2_standard.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14062 2024-05-02 12:07:30.588448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/deck/definitions/3/ot3_standard.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.588448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/deck/definitions/4/
+-rw-r--r--   0 runner    (1001) docker     (127)     6517 2024-05-02 12:07:30.588448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/deck/definitions/4/ot2_short_trash.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6493 2024-05-02 12:07:30.588448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/deck/definitions/4/ot2_standard.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10643 2024-05-02 12:07:30.588448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/deck/definitions/4/ot3_standard.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.592448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/deck/definitions/5/
+-rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-05-02 12:07:30.592448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/deck/definitions/5/ot2_short_trash.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6613 2024-05-02 12:07:30.592448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/deck/definitions/5/ot2_standard.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19106 2024-05-02 12:07:30.592448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/deck/definitions/5/ot3_standard.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.592448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/deck/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-05-02 12:07:30.592448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/deck/schemas/1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-05-02 12:07:30.592448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/deck/schemas/2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5645 2024-05-02 12:07:30.592448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/deck/schemas/3.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7509 2024-05-02 12:07:30.592448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/deck/schemas/4.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8083 2024-05-02 12:07:30.592448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/deck/schemas/5.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.772448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/errors/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.772448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/errors/definitions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.772448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/errors/definitions/1/
+-rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-05-02 12:07:30.772448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/errors/definitions/1/errors.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.772448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/errors/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-02 12:07:30.772448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/errors/schemas/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.772448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/gripper/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.772448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/gripper/definitions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.772448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/gripper/definitions/1/
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-02 12:07:30.772448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/gripper/definitions/1/gripperV1.1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-02 12:07:30.772448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/gripper/definitions/1/gripperV1.2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-02 12:07:30.772448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/gripper/definitions/1/gripperV1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.772448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/gripper/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-05-02 12:07:30.772448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/gripper/schemas/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.684448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.660448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.684448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-02 12:07:30.684448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/12-well-plate.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-05-02 12:07:30.676448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/24-vial-rack.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-02 12:07:30.660448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/24-well-plate.json
+-rw-r--r--   0 runner    (1001) docker     (127)    49831 2024-05-02 12:07:30.672448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/384-plate.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6413 2024-05-02 12:07:30.680448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/48-vial-plate.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6798 2024-05-02 12:07:30.680448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/48-well-plate.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-05-02 12:07:30.676448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/5ml-3x4.json
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-02 12:07:30.680448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/6-well-plate.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12751 2024-05-02 12:07:30.680448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/96-PCR-flat.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12764 2024-05-02 12:07:30.676448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/96-PCR-tall.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12861 2024-05-02 12:07:30.668448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/96-deep-well.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12856 2024-05-02 12:07:30.684448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/96-flat.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13059 2024-05-02 12:07:30.664448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/96-well-plate-20mm.json
+-rw-r--r--   0 runner    (1001) docker     (127)    44426 2024-05-02 12:07:30.668448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/MALDI-plate.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12767 2024-05-02 12:07:30.660448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/PCR-strip-tall.json
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-02 12:07:30.676448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/T25-flask.json
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-02 12:07:30.660448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/T75-flask.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-02 12:07:30.676448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/alum-block-pcr-strips.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13256 2024-05-02 12:07:30.676448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/biorad-hardshell-96-PCR.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11396 2024-05-02 12:07:30.676448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/e-gelgol.json
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-02 12:07:30.672448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/fixed-trash.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12454 2024-05-02 12:07:30.668448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/hampton-1ml-deep-block.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-05-02 12:07:30.680448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/opentrons-aluminum-block-2ml-eppendorf.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-05-02 12:07:30.660448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/opentrons-aluminum-block-2ml-screwcap.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13282 2024-05-02 12:07:30.664448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/opentrons-aluminum-block-96-PCR-plate.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13286 2024-05-02 12:07:30.672448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/opentrons-aluminum-block-PCR-strips-200ul.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10426 2024-05-02 12:07:30.660448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/opentrons-tiprack-10ul.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9948 2024-05-02 12:07:30.668448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/opentrons-tiprack-300ul.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-05-02 12:07:30.672448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/opentrons-tuberack-1.5ml-eppendorf.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-02 12:07:30.680448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/opentrons-tuberack-15_50ml.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-02 12:07:30.672448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/opentrons-tuberack-15ml.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-05-02 12:07:30.668448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/opentrons-tuberack-2ml-eppendorf.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-05-02 12:07:30.660448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/opentrons-tuberack-2ml-screwcap.json
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-02 12:07:30.664448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/opentrons-tuberack-50ml.json
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-02 12:07:30.684448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/point.json
+-rw-r--r--   0 runner    (1001) docker     (127)    24220 2024-05-02 12:07:30.664448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/rigaku-compact-crystallization-plate.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-05-02 12:07:30.680448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/small_vial_rack_16x45.json
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-02 12:07:30.668448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/tall-fixed-trash.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-05-02 12:07:30.672448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/tiprack-1000ul-H.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9956 2024-05-02 12:07:30.676448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/tiprack-1000ul-chem.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9940 2024-05-02 12:07:30.664448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/tiprack-1000ul.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-05-02 12:07:30.684448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/tiprack-10ul-H.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9936 2024-05-02 12:07:30.680448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/tiprack-10ul.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9938 2024-05-02 12:07:30.684448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/tiprack-200ul.json
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-02 12:07:30.676448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/trash-box.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-02 12:07:30.684448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/trough-12row-short.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-02 12:07:30.684448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/trough-12row.json
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-02 12:07:30.684448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/trough-1row-25ml.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-05-02 12:07:30.664448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/tube-rack-.75ml.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-02 12:07:30.680448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/tube-rack-15_50ml.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10168 2024-05-02 12:07:30.684448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/tube-rack-2ml-9x9.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-05-02 12:07:30.676448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/tube-rack-2ml.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12066 2024-05-02 12:07:30.664448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/tube-rack-5ml-96.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9856 2024-05-02 12:07:30.680448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/tube-rack-80well.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6285 2024-05-02 12:07:30.660448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/wheaton_vial_rack.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.656448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.608448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/agilent_1_reservoir_290ml/
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-02 12:07:30.608448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/agilent_1_reservoir_290ml/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.660448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/appliedbiosystemsmicroamp_384_wellplate_40ul/
+-rw-r--r--   0 runner    (1001) docker     (127)    45701 2024-05-02 12:07:30.660448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/appliedbiosystemsmicroamp_384_wellplate_40ul/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.648448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/armadillo_96_wellplate_200ul_pcr_full_skirt/
+-rw-r--r--   0 runner    (1001) docker     (127)    12136 2024-05-02 12:07:30.648448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/armadillo_96_wellplate_200ul_pcr_full_skirt/1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12440 2024-05-02 12:07:30.648448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/armadillo_96_wellplate_200ul_pcr_full_skirt/2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.644448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/axygen_1_reservoir_90ml/
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-02 12:07:30.644448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/axygen_1_reservoir_90ml/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.604448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/biorad_384_wellplate_50ul/
+-rw-r--r--   0 runner    (1001) docker     (127)    46125 2024-05-02 12:07:30.600448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/biorad_384_wellplate_50ul/1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    46174 2024-05-02 12:07:30.604448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/biorad_384_wellplate_50ul/2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.640448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/biorad_96_wellplate_200ul_pcr/
+-rw-r--r--   0 runner    (1001) docker     (127)    12276 2024-05-02 12:07:30.640448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/biorad_96_wellplate_200ul_pcr/1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12584 2024-05-02 12:07:30.640448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/biorad_96_wellplate_200ul_pcr/2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.596448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/corning_12_wellplate_6.9ml_flat/
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-05-02 12:07:30.596448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/corning_12_wellplate_6.9ml_flat/1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-02 12:07:30.596448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/corning_12_wellplate_6.9ml_flat/2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.608448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/corning_24_wellplate_3.4ml_flat/
+-rw-r--r--   0 runner    (1001) docker     (127)     3672 2024-05-02 12:07:30.608448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/corning_24_wellplate_3.4ml_flat/1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-05-02 12:07:30.608448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/corning_24_wellplate_3.4ml_flat/2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.632448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/corning_384_wellplate_112ul_flat/
+-rw-r--r--   0 runner    (1001) docker     (127)    56163 2024-05-02 12:07:30.632448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/corning_384_wellplate_112ul_flat/1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    56362 2024-05-02 12:07:30.632448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/corning_384_wellplate_112ul_flat/2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.628448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/corning_48_wellplate_1.6ml_flat/
+-rw-r--r--   0 runner    (1001) docker     (127)     6501 2024-05-02 12:07:30.628448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/corning_48_wellplate_1.6ml_flat/1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6642 2024-05-02 12:07:30.628448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/corning_48_wellplate_1.6ml_flat/2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.644448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/corning_6_wellplate_16.8ml_flat/
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-02 12:07:30.644448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/corning_6_wellplate_16.8ml_flat/1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-02 12:07:30.644448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/corning_6_wellplate_16.8ml_flat/2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.616448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/corning_96_wellplate_360ul_flat/
+-rw-r--r--   0 runner    (1001) docker     (127)    12547 2024-05-02 12:07:30.616448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/corning_96_wellplate_360ul_flat/1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12748 2024-05-02 12:07:30.616448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/corning_96_wellplate_360ul_flat/2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.624448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/eppendorf_96_tiprack_1000ul_eptips/
+-rw-r--r--   0 runner    (1001) docker     (127)    11971 2024-05-02 12:07:30.624448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/eppendorf_96_tiprack_1000ul_eptips/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.596448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/eppendorf_96_tiprack_10ul_eptips/
+-rw-r--r--   0 runner    (1001) docker     (127)    11580 2024-05-02 12:07:30.596448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/eppendorf_96_tiprack_10ul_eptips/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.652448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/geb_96_tiprack_1000ul/
+-rw-r--r--   0 runner    (1001) docker     (127)    11887 2024-05-02 12:07:30.652448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/geb_96_tiprack_1000ul/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.640448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/geb_96_tiprack_10ul/
+-rw-r--r--   0 runner    (1001) docker     (127)    11881 2024-05-02 12:07:30.640448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/geb_96_tiprack_10ul/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.616448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/nest_12_reservoir_15ml/
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-05-02 12:07:30.616448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/nest_12_reservoir_15ml/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.656448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/nest_1_reservoir_195ml/
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-02 12:07:30.656448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/nest_1_reservoir_195ml/1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-02 12:07:30.656448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/nest_1_reservoir_195ml/2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.648448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/nest_1_reservoir_290ml/
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-02 12:07:30.648448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/nest_1_reservoir_290ml/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.608448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/nest_96_wellplate_100ul_pcr_full_skirt/
+-rw-r--r--   0 runner    (1001) docker     (127)    12218 2024-05-02 12:07:30.608448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/nest_96_wellplate_100ul_pcr_full_skirt/1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12483 2024-05-02 12:07:30.608448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/nest_96_wellplate_100ul_pcr_full_skirt/2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.636448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/nest_96_wellplate_200ul_flat/
+-rw-r--r--   0 runner    (1001) docker     (127)    11987 2024-05-02 12:07:30.632448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/nest_96_wellplate_200ul_flat/1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12186 2024-05-02 12:07:30.636448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/nest_96_wellplate_200ul_flat/2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.604448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/nest_96_wellplate_2ml_deep/
+-rw-r--r--   0 runner    (1001) docker     (127)    13764 2024-05-02 12:07:30.604448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/nest_96_wellplate_2ml_deep/1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13970 2024-05-02 12:07:30.604448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/nest_96_wellplate_2ml_deep/2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.628448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_10_tuberack_falcon_4x50ml_6x15ml_conical/
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-02 12:07:30.628448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_10_tuberack_falcon_4x50ml_6x15ml_conical/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.612448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_10_tuberack_falcon_4x50ml_6x15ml_conical_acrylic/
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-05-02 12:07:30.612448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_10_tuberack_falcon_4x50ml_6x15ml_conical_acrylic/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.644448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_10_tuberack_nest_4x50ml_6x15ml_conical/
+-rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-05-02 12:07:30.644448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_10_tuberack_nest_4x50ml_6x15ml_conical/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.616448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_15_tuberack_falcon_15ml_conical/
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-05-02 12:07:30.616448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_15_tuberack_falcon_15ml_conical/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.612448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_15_tuberack_nest_15ml_conical/
+-rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-05-02 12:07:30.612448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_15_tuberack_nest_15ml_conical/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.604448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_1_trash_1100ml_fixed/
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-02 12:07:30.604448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_1_trash_1100ml_fixed/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.612448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_1_trash_3200ml_fixed/
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-02 12:07:30.612448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_1_trash_3200ml_fixed/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.624448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_1_trash_850ml_fixed/
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-02 12:07:30.624448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_1_trash_850ml_fixed/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.656448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_24_aluminumblock_generic_2ml_screwcap/
+-rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-02 12:07:30.656448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_24_aluminumblock_generic_2ml_screwcap/1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-05-02 12:07:30.656448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_24_aluminumblock_generic_2ml_screwcap/2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.600448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_24_aluminumblock_nest_0.5ml_screwcap/
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-05-02 12:07:30.600448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_24_aluminumblock_nest_0.5ml_screwcap/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.596448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_24_aluminumblock_nest_1.5ml_screwcap/
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-05-02 12:07:30.596448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_24_aluminumblock_nest_1.5ml_screwcap/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.656448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_24_aluminumblock_nest_1.5ml_snapcap/
+-rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-05-02 12:07:30.656448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_24_aluminumblock_nest_1.5ml_snapcap/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.600448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_24_aluminumblock_nest_2ml_screwcap/
+-rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-05-02 12:07:30.600448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_24_aluminumblock_nest_2ml_screwcap/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.624448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_24_aluminumblock_nest_2ml_snapcap/
+-rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-05-02 12:07:30.624448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_24_aluminumblock_nest_2ml_snapcap/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.652448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_24_tuberack_eppendorf_1.5ml_safelock_snapcap/
+-rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-05-02 12:07:30.652448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_24_tuberack_eppendorf_1.5ml_safelock_snapcap/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.644448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_24_tuberack_eppendorf_2ml_safelock_snapcap/
+-rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-05-02 12:07:30.644448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_24_tuberack_eppendorf_2ml_safelock_snapcap/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.640448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_24_tuberack_eppendorf_2ml_safelock_snapcap_acrylic/
+-rw-r--r--   0 runner    (1001) docker     (127)     3852 2024-05-02 12:07:30.640448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_24_tuberack_eppendorf_2ml_safelock_snapcap_acrylic/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.596448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_24_tuberack_generic_0.75ml_snapcap_acrylic/
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-05-02 12:07:30.596448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_24_tuberack_generic_0.75ml_snapcap_acrylic/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.624448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_24_tuberack_generic_2ml_screwcap/
+-rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-05-02 12:07:30.624448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_24_tuberack_generic_2ml_screwcap/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.656448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_24_tuberack_nest_0.5ml_screwcap/
+-rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-05-02 12:07:30.656448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_24_tuberack_nest_0.5ml_screwcap/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.592448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_24_tuberack_nest_1.5ml_screwcap/
+-rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-05-02 12:07:30.592448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_24_tuberack_nest_1.5ml_screwcap/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.644448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_24_tuberack_nest_1.5ml_snapcap/
+-rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-05-02 12:07:30.644448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_24_tuberack_nest_1.5ml_snapcap/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.648448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_24_tuberack_nest_2ml_screwcap/
+-rw-r--r--   0 runner    (1001) docker     (127)     3741 2024-05-02 12:07:30.648448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_24_tuberack_nest_2ml_screwcap/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.644448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_24_tuberack_nest_2ml_snapcap/
+-rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-05-02 12:07:30.644448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_24_tuberack_nest_2ml_snapcap/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.616448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_40_aluminumblock_eppendorf_24x2ml_safelock_snapcap_generic_16x0.2ml_pcr_strip/
+-rw-r--r--   0 runner    (1001) docker     (127)     5902 2024-05-02 12:07:30.616448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_40_aluminumblock_eppendorf_24x2ml_safelock_snapcap_generic_16x0.2ml_pcr_strip/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.644448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_6_tuberack_falcon_50ml_conical/
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-05-02 12:07:30.644448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_6_tuberack_falcon_50ml_conical/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.596448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_6_tuberack_nest_50ml_conical/
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-02 12:07:30.596448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_6_tuberack_nest_50ml_conical/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.656448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_96_aluminumblock_biorad_wellplate_200ul/
+-rw-r--r--   0 runner    (1001) docker     (127)    12264 2024-05-02 12:07:30.656448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_96_aluminumblock_biorad_wellplate_200ul/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.652448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_96_aluminumblock_generic_pcr_strip_200ul/
+-rw-r--r--   0 runner    (1001) docker     (127)    12282 2024-05-02 12:07:30.652448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_96_aluminumblock_generic_pcr_strip_200ul/1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12316 2024-05-02 12:07:30.652448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_96_aluminumblock_generic_pcr_strip_200ul/2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.636448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_96_aluminumblock_nest_wellplate_100ul/
+-rw-r--r--   0 runner    (1001) docker     (127)    12373 2024-05-02 12:07:30.636448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_96_aluminumblock_nest_wellplate_100ul/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.612448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_96_deep_well_adapter/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-02 12:07:30.612448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_96_deep_well_adapter/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.608448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_96_deep_well_adapter_nest_wellplate_2ml_deep/
+-rw-r--r--   0 runner    (1001) docker     (127)    14139 2024-05-02 12:07:30.608448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_96_deep_well_adapter_nest_wellplate_2ml_deep/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.636448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_96_filtertiprack_1000ul/
+-rw-r--r--   0 runner    (1001) docker     (127)    11943 2024-05-02 12:07:30.636448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_96_filtertiprack_1000ul/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.636448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_96_filtertiprack_10ul/
+-rw-r--r--   0 runner    (1001) docker     (127)    12037 2024-05-02 12:07:30.636448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_96_filtertiprack_10ul/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.604448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_96_filtertiprack_200ul/
+-rw-r--r--   0 runner    (1001) docker     (127)    12039 2024-05-02 12:07:30.604448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_96_filtertiprack_200ul/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.644448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_96_filtertiprack_20ul/
+-rw-r--r--   0 runner    (1001) docker     (127)    12037 2024-05-02 12:07:30.644448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_96_filtertiprack_20ul/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.628448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_96_flat_bottom_adapter/
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-02 12:07:30.628448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_96_flat_bottom_adapter/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.612448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_96_flat_bottom_adapter_nest_wellplate_200ul_flat/
+-rw-r--r--   0 runner    (1001) docker     (127)    12347 2024-05-02 12:07:30.612448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_96_flat_bottom_adapter_nest_wellplate_200ul_flat/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.624448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_96_pcr_adapter/
+-rw-r--r--   0 runner    (1001) docker     (127)    11150 2024-05-02 12:07:30.624448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_96_pcr_adapter/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.616448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_96_pcr_adapter_armadillo_wellplate_200ul/
+-rw-r--r--   0 runner    (1001) docker     (127)    12358 2024-05-02 12:07:30.616448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_96_pcr_adapter_armadillo_wellplate_200ul/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.652448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_96_pcr_adapter_nest_wellplate_100ul_pcr_full_skirt/
+-rw-r--r--   0 runner    (1001) docker     (127)    12419 2024-05-02 12:07:30.652448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_96_pcr_adapter_nest_wellplate_100ul_pcr_full_skirt/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.596448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_96_tiprack_1000ul/
+-rw-r--r--   0 runner    (1001) docker     (127)    12016 2024-05-02 12:07:30.596448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_96_tiprack_1000ul/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.636448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_96_tiprack_10ul/
+-rw-r--r--   0 runner    (1001) docker     (127)    12108 2024-05-02 12:07:30.636448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_96_tiprack_10ul/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.612448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_96_tiprack_20ul/
+-rw-r--r--   0 runner    (1001) docker     (127)    12108 2024-05-02 12:07:30.612448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_96_tiprack_20ul/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.652448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_96_tiprack_300ul/
+-rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-02 12:07:30.652448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_96_tiprack_300ul/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.612448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_96_well_aluminum_block/
+-rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-05-02 12:07:30.612448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_96_well_aluminum_block/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.620448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_96_wellplate_200ul_pcr_full_skirt/
+-rw-r--r--   0 runner    (1001) docker     (127)    12130 2024-05-02 12:07:30.620448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_96_wellplate_200ul_pcr_full_skirt/1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12434 2024-05-02 12:07:30.620448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_96_wellplate_200ul_pcr_full_skirt/2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.648448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_aluminum_flat_bottom_plate/
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-02 12:07:30.648448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_aluminum_flat_bottom_plate/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.604448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_calibration_adapter_heatershaker_module/
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-02 12:07:30.604448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_calibration_adapter_heatershaker_module/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.624448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_calibration_adapter_temperature_module/
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-02 12:07:30.624448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_calibration_adapter_temperature_module/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.656448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_calibration_adapter_thermocycler_module/
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-02 12:07:30.656448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_calibration_adapter_thermocycler_module/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.644448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_calibrationblock_short_side_left/
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-02 12:07:30.644448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_calibrationblock_short_side_left/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.648448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_calibrationblock_short_side_right/
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-02 12:07:30.648448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_calibrationblock_short_side_right/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.640448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_flex_96_filtertiprack_1000ul/
+-rw-r--r--   0 runner    (1001) docker     (127)    12182 2024-05-02 12:07:30.640448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_flex_96_filtertiprack_1000ul/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.648448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_flex_96_filtertiprack_200ul/
+-rw-r--r--   0 runner    (1001) docker     (127)    12085 2024-05-02 12:07:30.648448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_flex_96_filtertiprack_200ul/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.640448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_flex_96_filtertiprack_50ul/
+-rw-r--r--   0 runner    (1001) docker     (127)    11986 2024-05-02 12:07:30.640448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_flex_96_filtertiprack_50ul/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.624448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_flex_96_tiprack_1000ul/
+-rw-r--r--   0 runner    (1001) docker     (127)    12169 2024-05-02 12:07:30.624448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_flex_96_tiprack_1000ul/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.624448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_flex_96_tiprack_200ul/
+-rw-r--r--   0 runner    (1001) docker     (127)    12072 2024-05-02 12:07:30.624448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_flex_96_tiprack_200ul/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.616448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_flex_96_tiprack_50ul/
+-rw-r--r--   0 runner    (1001) docker     (127)    11973 2024-05-02 12:07:30.616448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_flex_96_tiprack_50ul/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.648448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_flex_96_tiprack_adapter/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-02 12:07:30.648448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_flex_96_tiprack_adapter/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.636448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_universal_flat_adapter/
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-02 12:07:30.636448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_universal_flat_adapter/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.620448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_universal_flat_adapter_corning_384_wellplate_112ul_flat/
+-rw-r--r--   0 runner    (1001) docker     (127)    56413 2024-05-02 12:07:30.620448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_universal_flat_adapter_corning_384_wellplate_112ul_flat/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.632448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/thermoscientificnunc_96_wellplate_1300ul/
+-rw-r--r--   0 runner    (1001) docker     (127)    11975 2024-05-02 12:07:30.632448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/thermoscientificnunc_96_wellplate_1300ul/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.612448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/thermoscientificnunc_96_wellplate_2000ul/
+-rw-r--r--   0 runner    (1001) docker     (127)    11875 2024-05-02 12:07:30.612448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/thermoscientificnunc_96_wellplate_2000ul/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.628448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/tipone_96_tiprack_200ul/
+-rw-r--r--   0 runner    (1001) docker     (127)    12162 2024-05-02 12:07:30.628448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/tipone_96_tiprack_200ul/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.596448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/usascientific_12_reservoir_22ml/
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-05-02 12:07:30.596448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/usascientific_12_reservoir_22ml/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.608448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/usascientific_96_wellplate_2.4ml_deep/
+-rw-r--r--   0 runner    (1001) docker     (127)    13960 2024-05-02 12:07:30.608448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/usascientific_96_wellplate_2.4ml_deep/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.684448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     8879 2024-05-02 12:07:30.684448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/schemas/2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.776448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/liquid/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.776448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/liquid/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-02 12:07:30.776448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/liquid/schemas/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.692448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/module/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.688448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/module/definitions/
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-02 12:07:30.684448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/module/definitions/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.688448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/module/definitions/2/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-02 12:07:30.688448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/module/definitions/2/magneticModuleV1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-02 12:07:30.688448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/module/definitions/2/magneticModuleV2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-02 12:07:30.688448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/module/definitions/2/temperatureModuleV1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-02 12:07:30.688448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/module/definitions/2/temperatureModuleV2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-02 12:07:30.688448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/module/definitions/2/thermocyclerModuleV1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.692448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/module/definitions/3/
+-rw-r--r--   0 runner    (1001) docker     (127)    10821 2024-05-02 12:07:30.692448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/module/definitions/3/heaterShakerModuleV1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    78832 2024-05-02 12:07:30.692448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/module/definitions/3/magneticBlockV1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8689 2024-05-02 12:07:30.692448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/module/definitions/3/magneticModuleV1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9131 2024-05-02 12:07:30.688448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/module/definitions/3/magneticModuleV2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-05-02 12:07:30.692448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/module/definitions/3/temperatureModuleV1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-05-02 12:07:30.692448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/module/definitions/3/temperatureModuleV2.json
+-rw-r--r--   0 runner    (1001) docker     (127)    38434 2024-05-02 12:07:30.688448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/module/definitions/3/thermocyclerModuleV1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    60037 2024-05-02 12:07:30.688448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/module/definitions/3/thermocyclerModuleV2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.692448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/module/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-02 12:07:30.692448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/module/schemas/1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-05-02 12:07:30.692448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/module/schemas/2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5427 2024-05-02 12:07:30.692448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/module/schemas/3.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.764448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.756448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.764448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/1/
+-rw-r--r--   0 runner    (1001) docker     (127)   163243 2024-05-02 12:07:30.764448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/1/pipetteModelSpecs.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11476 2024-05-02 12:07:30.756448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/1/pipetteNameSpecs.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.728448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.720448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.728448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.724448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p10/
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-02 12:07:30.724448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p10/1_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-02 12:07:30.724448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p10/1_3.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-02 12:07:30.724448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p10/1_4.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-02 12:07:30.724448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p10/1_5.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-02 12:07:30.724448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p10/1_6.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.724448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p1000/
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-02 12:07:30.724448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p1000/1_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-02 12:07:30.720448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p1000/3_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-02 12:07:30.720448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p1000/3_3.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-02 12:07:30.720448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p1000/3_4.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-02 12:07:30.720448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p1000/3_5.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.728448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p20/
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-02 12:07:30.728448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p20/2_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-02 12:07:30.728448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p20/2_1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.724448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p300/
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-02 12:07:30.724448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p300/1_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-02 12:07:30.724448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p300/1_3.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-02 12:07:30.724448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p300/1_4.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-02 12:07:30.724448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p300/1_5.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-02 12:07:30.724448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p300/2_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-02 12:07:30.724448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p300/2_1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.728448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p50/
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-02 12:07:30.728448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p50/1_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-02 12:07:30.728448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p50/1_3.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-02 12:07:30.728448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p50/1_4.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-02 12:07:30.724448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p50/1_5.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-02 12:07:30.724448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p50/3_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-02 12:07:30.724448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p50/3_3.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-02 12:07:30.728448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p50/3_4.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-02 12:07:30.728448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p50/3_5.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.720448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/ninety_six_channel/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.720448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/ninety_six_channel/p1000/
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-02 12:07:30.720448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/ninety_six_channel/p1000/1_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-02 12:07:30.720448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/ninety_six_channel/p1000/3_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-02 12:07:30.720448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/ninety_six_channel/p1000/3_3.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-02 12:07:30.720448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/ninety_six_channel/p1000/3_4.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-02 12:07:30.720448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/ninety_six_channel/p1000/3_5.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-02 12:07:30.720448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/ninety_six_channel/p1000/3_6.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.720448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.716448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p10/
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-02 12:07:30.716448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p10/1_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-02 12:07:30.716448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p10/1_3.json
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-02 12:07:30.712448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p10/1_4.json
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-02 12:07:30.712448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p10/1_5.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.712448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p1000/
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-02 12:07:30.712448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p1000/1_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-02 12:07:30.712448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p1000/1_3.json
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-02 12:07:30.712448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p1000/1_4.json
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-02 12:07:30.712448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p1000/1_5.json
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-02 12:07:30.712448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p1000/2_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-02 12:07:30.712448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p1000/2_1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-02 12:07:30.712448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p1000/2_2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-02 12:07:30.712448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p1000/3_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-02 12:07:30.712448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p1000/3_3.json
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-02 12:07:30.712448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p1000/3_4.json
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-02 12:07:30.712448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p1000/3_5.json
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-02 12:07:30.712448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p1000/3_6.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.720448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p20/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-02 12:07:30.720448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p20/2_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-02 12:07:30.720448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p20/2_1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-02 12:07:30.720448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p20/2_2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.716448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p300/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-02 12:07:30.716448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p300/1_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-02 12:07:30.716448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p300/1_3.json
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-02 12:07:30.716448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p300/1_4.json
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-02 12:07:30.716448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p300/1_5.json
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-02 12:07:30.716448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p300/2_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-02 12:07:30.716448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p300/2_1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.720448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p50/
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-02 12:07:30.720448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p50/1_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-02 12:07:30.716448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p50/1_3.json
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-02 12:07:30.716448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p50/1_4.json
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-02 12:07:30.716448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p50/1_5.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-02 12:07:30.716448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p50/3_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-02 12:07:30.716448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p50/3_3.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-02 12:07:30.716448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p50/3_4.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-02 12:07:30.716448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p50/3_5.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-02 12:07:30.716448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p50/3_6.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.704448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.708448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.708448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p10/
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-02 12:07:30.708448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p10/1_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-02 12:07:30.704448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p10/1_3.json
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-02 12:07:30.704448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p10/1_4.json
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-02 12:07:30.704448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p10/1_5.json
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-02 12:07:30.704448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p10/1_6.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.704448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p1000/
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-02 12:07:30.704448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p1000/1_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-02 12:07:30.704448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p1000/3_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-02 12:07:30.704448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p1000/3_3.json
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-02 12:07:30.704448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p1000/3_4.json
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-02 12:07:30.704448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p1000/3_5.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.712448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p20/
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-02 12:07:30.712448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p20/2_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-02 12:07:30.712448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p20/2_1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.708448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p300/
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-02 12:07:30.708448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p300/1_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-02 12:07:30.708448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p300/1_3.json
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-02 12:07:30.708448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p300/1_4.json
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-02 12:07:30.708448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p300/1_5.json
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-02 12:07:30.708448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p300/2_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-02 12:07:30.708448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p300/2_1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.708448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p50/
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-02 12:07:30.708448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p50/1_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-02 12:07:30.708448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p50/1_3.json
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-02 12:07:30.708448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p50/1_4.json
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-02 12:07:30.708448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p50/1_5.json
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-02 12:07:30.708448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p50/3_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-02 12:07:30.708448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p50/3_3.json
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-02 12:07:30.708448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p50/3_4.json
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-02 12:07:30.708448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p50/3_5.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.700448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/ninety_six_channel/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.704448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/ninety_six_channel/p1000/
+-rw-r--r--   0 runner    (1001) docker     (127)     4508 2024-05-02 12:07:30.704448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/ninety_six_channel/p1000/1_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4508 2024-05-02 12:07:30.700448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/ninety_six_channel/p1000/3_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4508 2024-05-02 12:07:30.704448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/ninety_six_channel/p1000/3_3.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4508 2024-05-02 12:07:30.704448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/ninety_six_channel/p1000/3_4.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4508 2024-05-02 12:07:30.704448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/ninety_six_channel/p1000/3_5.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4508 2024-05-02 12:07:30.704448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/ninety_six_channel/p1000/3_6.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.700448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.696448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p10/
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-02 12:07:30.696448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p10/1_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-02 12:07:30.696448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p10/1_3.json
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-02 12:07:30.696448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p10/1_4.json
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-02 12:07:30.696448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p10/1_5.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.696448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p1000/
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-02 12:07:30.696448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p1000/1_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-02 12:07:30.696448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p1000/1_3.json
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-02 12:07:30.696448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p1000/1_4.json
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-02 12:07:30.696448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p1000/1_5.json
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-02 12:07:30.696448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p1000/2_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-02 12:07:30.696448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p1000/2_1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-02 12:07:30.692448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p1000/2_2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-02 12:07:30.692448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p1000/3_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-02 12:07:30.696448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p1000/3_3.json
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-02 12:07:30.696448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p1000/3_4.json
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-02 12:07:30.696448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p1000/3_5.json
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-02 12:07:30.696448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p1000/3_6.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.700448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p20/
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-02 12:07:30.700448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p20/2_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-02 12:07:30.700448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p20/2_1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-02 12:07:30.700448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p20/2_2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.700448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p300/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-02 12:07:30.700448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p300/1_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-02 12:07:30.700448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p300/1_3.json
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-02 12:07:30.696448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p300/1_4.json
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-02 12:07:30.696448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p300/1_5.json
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-02 12:07:30.696448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p300/2_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-02 12:07:30.696448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p300/2_1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.700448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p50/
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-02 12:07:30.700448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p50/1_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-02 12:07:30.700448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p50/1_3.json
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-02 12:07:30.700448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p50/1_4.json
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-02 12:07:30.700448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p50/1_5.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-02 12:07:30.700448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p50/3_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-02 12:07:30.700448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p50/3_3.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-02 12:07:30.700448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p50/3_4.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-02 12:07:30.700448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p50/3_5.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-02 12:07:30.700448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/single_channel/p50/3_6.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.744448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.756448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.748448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p10/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.748448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p10/default/
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-02 12:07:30.748448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p10/default/1_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-02 12:07:30.748448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p10/default/1_3.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-02 12:07:30.748448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p10/default/1_4.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-02 12:07:30.748448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p10/default/1_5.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-02 12:07:30.748448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p10/default/1_6.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.744448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p1000/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.748448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p1000/default/
+-rw-r--r--   0 runner    (1001) docker     (127)     7812 2024-05-02 12:07:30.748448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p1000/default/1_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8143 2024-05-02 12:07:30.744448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p1000/default/3_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8209 2024-05-02 12:07:30.744448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p1000/default/3_3.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8227 2024-05-02 12:07:30.748448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p1000/default/3_4.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-05-02 12:07:30.748448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p1000/default/3_5.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.756448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p20/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.756448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p20/default/
+-rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-05-02 12:07:30.756448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p20/default/2_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-05-02 12:07:30.756448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p20/default/2_1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.748448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p300/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.752448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p300/default/
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-02 12:07:30.752448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p300/default/1_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-02 12:07:30.752448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p300/default/1_3.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-02 12:07:30.752448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p300/default/1_4.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-02 12:07:30.748448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p300/default/1_5.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-05-02 12:07:30.752448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p300/default/2_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-05-02 12:07:30.748448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p300/default/2_1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.752448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p50/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.752448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p50/default/
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-02 12:07:30.752448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p50/default/1_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-02 12:07:30.752448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p50/default/1_3.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-05-02 12:07:30.752448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p50/default/1_4.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-02 12:07:30.752448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p50/default/1_5.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-02 12:07:30.752448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p50/default/3_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-02 12:07:30.752448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p50/default/3_3.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-05-02 12:07:30.752448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p50/default/3_4.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-02 12:07:30.752448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p50/default/3_5.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.756448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p50/lowVolumeDefault/
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-05-02 12:07:30.752448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p50/lowVolumeDefault/3_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-02 12:07:30.756448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p50/lowVolumeDefault/3_3.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-02 12:07:30.756448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p50/lowVolumeDefault/3_4.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-02 12:07:30.756448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p50/lowVolumeDefault/3_5.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.744448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/ninety_six_channel/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.744448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/ninety_six_channel/p1000/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.744448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/ninety_six_channel/p1000/default/
+-rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-05-02 12:07:30.744448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/ninety_six_channel/p1000/default/1_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-05-02 12:07:30.744448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/ninety_six_channel/p1000/default/3_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-05-02 12:07:30.744448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/ninety_six_channel/p1000/default/3_3.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-05-02 12:07:30.744448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/ninety_six_channel/p1000/default/3_4.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-05-02 12:07:30.744448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/ninety_six_channel/p1000/default/3_5.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3679 2024-05-02 12:07:30.744448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/ninety_six_channel/p1000/default/3_6.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.740448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.732448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p10/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.732448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p10/default/
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-02 12:07:30.732448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p10/default/1_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-02 12:07:30.732448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p10/default/1_3.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-02 12:07:30.732448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p10/default/1_4.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-02 12:07:30.732448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p10/default/1_5.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.728448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p1000/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.732448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p1000/default/
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-02 12:07:30.732448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p1000/default/1_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-02 12:07:30.732448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p1000/default/1_3.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-02 12:07:30.732448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p1000/default/1_4.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-02 12:07:30.732448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p1000/default/1_5.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-05-02 12:07:30.732448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p1000/default/2_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-05-02 12:07:30.728448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p1000/default/2_1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-02 12:07:30.728448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p1000/default/2_2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8139 2024-05-02 12:07:30.728448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p1000/default/3_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8205 2024-05-02 12:07:30.728448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p1000/default/3_3.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6263 2024-05-02 12:07:30.732448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p1000/default/3_4.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-05-02 12:07:30.732448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p1000/default/3_5.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-05-02 12:07:30.732448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p1000/default/3_6.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.740448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p20/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.740448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p20/default/
+-rw-r--r--   0 runner    (1001) docker     (127)     9689 2024-05-02 12:07:30.740448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p20/default/2_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5429 2024-05-02 12:07:30.740448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p20/default/2_1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6791 2024-05-02 12:07:30.740448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p20/default/2_2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.732448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p300/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.736448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p300/default/
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-05-02 12:07:30.736448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p300/default/1_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-05-02 12:07:30.736448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p300/default/1_3.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-05-02 12:07:30.736448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p300/default/1_4.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-02 12:07:30.736448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p300/default/1_5.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-05-02 12:07:30.736448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p300/default/2_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-02 12:07:30.736448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p300/default/2_1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.740448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p50/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.740448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p50/default/
+-rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-05-02 12:07:30.740448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p50/default/1_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-02 12:07:30.736448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p50/default/1_3.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-02 12:07:30.736448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p50/default/1_4.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-02 12:07:30.736448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p50/default/1_5.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-02 12:07:30.736448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p50/default/3_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-05-02 12:07:30.736448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p50/default/3_3.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-02 12:07:30.736448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p50/default/3_4.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-02 12:07:30.736448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p50/default/3_5.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-02 12:07:30.740448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p50/default/3_6.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.740448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p50/lowVolumeDefault/
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-02 12:07:30.740448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p50/lowVolumeDefault/3_0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-02 12:07:30.740448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p50/lowVolumeDefault/3_3.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-02 12:07:30.740448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p50/lowVolumeDefault/3_4.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-05-02 12:07:30.740448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p50/lowVolumeDefault/3_5.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-02 12:07:30.740448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p50/lowVolumeDefault/3_6.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.764448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/schemas/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.768448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/schemas/1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3920 2024-05-02 12:07:30.768448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/schemas/1/pipetteModelSpecsSchema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-02 12:07:30.768448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/schemas/1/pipetteNameSpecsSchema.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.764448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/schemas/2/
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-02 12:07:30.764448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/schemas/2/pipetteGeometrySchema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-05-02 12:07:30.764448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/schemas/2/pipetteLiquidPropertiesSchema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6690 2024-05-02 12:07:30.764448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/schemas/2/pipettePropertiesSchema.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.768448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/protocol/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.768448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/protocol/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     7657 2024-05-02 12:07:30.768448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/protocol/schemas/1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9131 2024-05-02 12:07:30.768448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/protocol/schemas/2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7691 2024-05-02 12:07:30.768448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/protocol/schemas/3.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15234 2024-05-02 12:07:30.768448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/protocol/schemas/4.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16750 2024-05-02 12:07:30.768448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/protocol/schemas/5.json
+-rw-r--r--   0 runner    (1001) docker     (127)    29434 2024-05-02 12:07:30.768448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/protocol/schemas/6.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5959 2024-05-02 12:07:30.768448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/protocol/schemas/7.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3468 2024-05-02 12:07:30.768448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/protocol/schemas/8.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.772448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/robot/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.772448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/robot/definitions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.772448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/robot/definitions/1/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-02 12:07:30.772448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/robot/definitions/1/ot2.json
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-02 12:07:30.772448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/robot/definitions/1/ot3.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.772448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/robot/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-02 12:07:30.772448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/robot/schemas/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.784448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/deck/
+-rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-05-02 12:06:44.000000 opentrons_shared_data-7.3.0a0/opentrons_shared_data/deck/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-05-02 12:06:44.000000 opentrons_shared_data-7.3.0a0/opentrons_shared_data/deck/dev_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.784448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-02 12:06:44.000000 opentrons_shared_data-7.3.0a0/opentrons_shared_data/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-05-02 12:06:44.000000 opentrons_shared_data-7.3.0a0/opentrons_shared_data/errors/categories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-05-02 12:06:44.000000 opentrons_shared_data-7.3.0a0/opentrons_shared_data/errors/codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33557 2024-05-02 12:06:44.000000 opentrons_shared_data-7.3.0a0/opentrons_shared_data/errors/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.784448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/gripper/
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-02 12:06:44.000000 opentrons_shared_data-7.3.0a0/opentrons_shared_data/gripper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-02 12:06:44.000000 opentrons_shared_data-7.3.0a0/opentrons_shared_data/gripper/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-05-02 12:06:44.000000 opentrons_shared_data-7.3.0a0/opentrons_shared_data/gripper/gripper_definition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.784448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/labware/
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-02 12:06:44.000000 opentrons_shared_data-7.3.0a0/opentrons_shared_data/labware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-02 12:06:44.000000 opentrons_shared_data-7.3.0a0/opentrons_shared_data/labware/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-05-02 12:06:44.000000 opentrons_shared_data-7.3.0a0/opentrons_shared_data/labware/dev_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10131 2024-05-02 12:06:44.000000 opentrons_shared_data-7.3.0a0/opentrons_shared_data/labware/labware_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-02 12:06:44.000000 opentrons_shared_data-7.3.0a0/opentrons_shared_data/load.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.784448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/module/
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-05-02 12:06:44.000000 opentrons_shared_data-7.3.0a0/opentrons_shared_data/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-05-02 12:06:44.000000 opentrons_shared_data-7.3.0a0/opentrons_shared_data/module/dev_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.784448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/performance/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-02 12:06:44.000000 opentrons_shared_data-7.3.0a0/opentrons_shared_data/performance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-02 12:06:44.000000 opentrons_shared_data-7.3.0a0/opentrons_shared_data/performance/dev_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.788448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/pipette/
+-rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-05-02 12:06:44.000000 opentrons_shared_data-7.3.0a0/opentrons_shared_data/pipette/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-05-02 12:06:44.000000 opentrons_shared_data-7.3.0a0/opentrons_shared_data/pipette/dev_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-02 12:06:44.000000 opentrons_shared_data-7.3.0a0/opentrons_shared_data/pipette/file_operation_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8723 2024-05-02 12:06:44.000000 opentrons_shared_data-7.3.0a0/opentrons_shared_data/pipette/load_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4043 2024-05-02 12:06:44.000000 opentrons_shared_data-7.3.0a0/opentrons_shared_data/pipette/model_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16332 2024-05-02 12:06:44.000000 opentrons_shared_data-7.3.0a0/opentrons_shared_data/pipette/mutable_configurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19399 2024-05-02 12:06:44.000000 opentrons_shared_data-7.3.0a0/opentrons_shared_data/pipette/pipette_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10077 2024-05-02 12:06:44.000000 opentrons_shared_data-7.3.0a0/opentrons_shared_data/pipette/pipette_load_name_conversions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.788448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/pipette/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:06:44.000000 opentrons_shared_data-7.3.0a0/opentrons_shared_data/pipette/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18573 2024-05-02 12:06:44.000000 opentrons_shared_data-7.3.0a0/opentrons_shared_data/pipette/scripts/build_json_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16374 2024-05-02 12:06:44.000000 opentrons_shared_data-7.3.0a0/opentrons_shared_data/pipette/scripts/update_configuration_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4767 2024-05-02 12:06:44.000000 opentrons_shared_data-7.3.0a0/opentrons_shared_data/pipette/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-02 12:06:44.000000 opentrons_shared_data-7.3.0a0/opentrons_shared_data/pipette/ul_per_mm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.788448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/protocol/
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-02 12:06:44.000000 opentrons_shared_data-7.3.0a0/opentrons_shared_data/protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-05-02 12:06:44.000000 opentrons_shared_data-7.3.0a0/opentrons_shared_data/protocol/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11397 2024-05-02 12:06:44.000000 opentrons_shared_data-7.3.0a0/opentrons_shared_data/protocol/dev_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.788448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/protocol/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-02 12:06:44.000000 opentrons_shared_data-7.3.0a0/opentrons_shared_data/protocol/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4833 2024-05-02 12:06:44.000000 opentrons_shared_data-7.3.0a0/opentrons_shared_data/protocol/models/protocol_schema_v6.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-05-02 12:06:44.000000 opentrons_shared_data-7.3.0a0/opentrons_shared_data/protocol/models/protocol_schema_v7.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-05-02 12:06:44.000000 opentrons_shared_data-7.3.0a0/opentrons_shared_data/protocol/models/protocol_schema_v8.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-02 12:06:44.000000 opentrons_shared_data-7.3.0a0/opentrons_shared_data/protocol/models/shared_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:06:44.000000 opentrons_shared_data-7.3.0a0/opentrons_shared_data/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.788448 opentrons_shared_data-7.3.0a0/opentrons_shared_data/robot/
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-02 12:06:44.000000 opentrons_shared_data-7.3.0a0/opentrons_shared_data/robot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-02 12:06:44.000000 opentrons_shared_data-7.3.0a0/opentrons_shared_data/robot/dev_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:07:30.788448 opentrons_shared_data-7.3.0a0/opentrons_shared_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-02 12:07:30.000000 opentrons_shared_data-7.3.0a0/opentrons_shared_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-05-02 12:07:30.000000 opentrons_shared_data-7.3.0a0/opentrons_shared_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 12:07:30.000000 opentrons_shared_data-7.3.0a0/opentrons_shared_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 12:07:14.000000 opentrons_shared_data-7.3.0a0/opentrons_shared_data.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-02 12:07:30.000000 opentrons_shared_data-7.3.0a0/opentrons_shared_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-02 12:07:30.000000 opentrons_shared_data-7.3.0a0/opentrons_shared_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-02 12:07:30.788448 opentrons_shared_data-7.3.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-05-02 12:06:44.000000 opentrons_shared_data-7.3.0a0/setup.py
```

### Comparing `opentrons_shared_data-7.2.2a3/PKG-INFO` & `opentrons_shared_data-7.3.0a0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentrons_shared_data
-Version: 7.2.2a3
+Version: 7.3.0a0
 Summary: A bundle of data and python binding that supports the Opentrons API. Does not need to be installed manually; only a dependency of the opentrons package
 Author: Opentrons
 Author-email: engineering@opentrons.com
 Maintainer: Opentrons
 Maintainer-email: engineering@opentrons.com
 License: Apache 2.0
 Project-URL: opentrons.com, https://www.opentrons.com
@@ -13,16 +13,14 @@
 Keywords: robots,protocols,synbio,pcr,automation,lab
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 License-File: ../../LICENSE
 Requires-Dist: jsonschema<4.18.0,>=3.0.1
 Requires-Dist: typing-extensions<5,>=4.0.0
 Requires-Dist: pydantic<2.0.0,>=1.10.9
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/command/__init__.py` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/command/__init__.py`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/command/schemas/7.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/command/schemas/7.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/command/schemas/8.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/command/schemas/8.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9970888976411316%*

 * *Differences: {"'definitions'": "{'CommandIntent': {'enum': {insert: [(2, 'fixit')]}}, "*

 * *                  "'QuadrantNozzleLayoutConfiguration': {'properties': {'frontRightNozzle': "*

 * *                  "{'pattern': '[A-Z]\\\\d{1,2}'}}}, 'VerifyTipPresenceParams': {'properties': "*

 * *                  "{'followSingularSensor': OrderedDict([('description', 'The sensor id to follow "*

 * *                  "if the other can be ignored.'), ('allOf', [OrderedDict([('$ref', "*

 * *                  "'#/definitions/InstrumentSensorId')])])]) […]*

```diff
@@ -648,15 +648,16 @@
             "title": "ColumnNozzleLayoutConfiguration",
             "type": "object"
         },
         "CommandIntent": {
             "description": "Run intent for a given command.\n\nProps:\n    PROTOCOL: the command is part of the protocol run itself.\n    SETUP: the command is part of the setup phase of a run.",
             "enum": [
                 "protocol",
-                "setup"
+                "setup",
+                "fixit"
             ],
             "title": "CommandIntent",
             "type": "string"
         },
         "CommentCreate": {
             "description": "Comment command request model.",
             "properties": {
@@ -1715,14 +1716,24 @@
                     ],
                     "description": "If this parameter is provided, the gantry will only be homed if the specified mount has an invalid position. If omitted, the homing action will be executed unconditionally."
                 }
             },
             "title": "HomeParams",
             "type": "object"
         },
+        "InstrumentSensorId": {
+            "description": "Primary and secondary sensor ids.",
+            "enum": [
+                "primary",
+                "secondary",
+                "both"
+            ],
+            "title": "InstrumentSensorId",
+            "type": "string"
+        },
         "LabwareMovementStrategy": {
             "description": "Strategy to use for labware movement.",
             "enum": [
                 "usingGripper",
                 "manualMoveWithPause",
                 "manualMoveWithoutPause"
             ],
@@ -2951,15 +2962,15 @@
             "type": "object"
         },
         "QuadrantNozzleLayoutConfiguration": {
             "description": "Information required for nozzle configurations of type QUADRANT.",
             "properties": {
                 "frontRightNozzle": {
                     "description": "The front right nozzle in your configuration.",
-                    "pattern": "[A-Z][0-100]",
+                    "pattern": "[A-Z]\\d{1,2}",
                     "title": "Frontrightnozzle",
                     "type": "string"
                 },
                 "primaryNozzle": {
                     "description": "The primary nozzle to use in the layout configuration. This nozzle will update the critical point of the current pipette. For now, this is also the back left corner of your rectangle.",
                     "enum": [
                         "A1",
@@ -2982,14 +2993,63 @@
             "required": [
                 "primaryNozzle",
                 "frontRightNozzle"
             ],
             "title": "QuadrantNozzleLayoutConfiguration",
             "type": "object"
         },
+        "ReloadLabwareCreate": {
+            "description": "Reload labware command creation request.",
+            "properties": {
+                "commandType": {
+                    "default": "reloadLabware",
+                    "enum": [
+                        "reloadLabware"
+                    ],
+                    "title": "Commandtype",
+                    "type": "string"
+                },
+                "intent": {
+                    "allOf": [
+                        {
+                            "$ref": "#/definitions/CommandIntent"
+                        }
+                    ],
+                    "description": "The reason the command was added. If not specified or `protocol`, the command will be treated as part of the protocol run itself, and added to the end of the existing command queue.\n\nIf `setup`, the command will be treated as part of run setup. A setup command may only be enqueued if the run has not started.\n\nUse setup commands for activities like pre-run calibration checks and module setup, like pre-heating."
+                },
+                "key": {
+                    "description": "A key value, unique in this run, that can be used to track the same logical command across multiple runs of the same protocol. If a value is not provided, one will be generated.",
+                    "title": "Key",
+                    "type": "string"
+                },
+                "params": {
+                    "$ref": "#/definitions/ReloadLabwareParams"
+                }
+            },
+            "required": [
+                "params"
+            ],
+            "title": "ReloadLabwareCreate",
+            "type": "object"
+        },
+        "ReloadLabwareParams": {
+            "description": "Payload required to load a labware into a slot.",
+            "properties": {
+                "labwareId": {
+                    "description": "The already-loaded labware instance to update.",
+                    "title": "Labwareid",
+                    "type": "string"
+                }
+            },
+            "required": [
+                "labwareId"
+            ],
+            "title": "ReloadLabwareParams",
+            "type": "object"
+        },
         "RetractAxisCreate": {
             "description": "Data to create a Retract Axis command.",
             "properties": {
                 "commandType": {
                     "default": "retractAxis",
                     "enum": [
                         "retractAxis"
@@ -3683,14 +3743,22 @@
                     "allOf": [
                         {
                             "$ref": "#/definitions/TipPresenceStatus"
                         }
                     ],
                     "description": "The expected tip presence status on the pipette."
                 },
+                "followSingularSensor": {
+                    "allOf": [
+                        {
+                            "$ref": "#/definitions/InstrumentSensorId"
+                        }
+                    ],
+                    "description": "The sensor id to follow if the other can be ignored."
+                },
                 "pipetteId": {
                     "description": "Identifier of pipette to use for liquid handling.",
                     "title": "Pipetteid",
                     "type": "string"
                 }
             },
             "required": [
@@ -4207,14 +4275,15 @@
             "moveToAddressableArea": "#/definitions/MoveToAddressableAreaCreate",
             "moveToAddressableAreaForDropTip": "#/definitions/MoveToAddressableAreaForDropTipCreate",
             "moveToCoordinates": "#/definitions/MoveToCoordinatesCreate",
             "moveToWell": "#/definitions/MoveToWellCreate",
             "pause": "#/definitions/WaitForResumeCreate",
             "pickUpTip": "#/definitions/PickUpTipCreate",
             "prepareToAspirate": "#/definitions/PrepareToAspirateCreate",
+            "reloadLabware": "#/definitions/ReloadLabwareCreate",
             "retractAxis": "#/definitions/RetractAxisCreate",
             "savePosition": "#/definitions/SavePositionCreate",
             "setRailLights": "#/definitions/SetRailLightsCreate",
             "setStatusBar": "#/definitions/SetStatusBarCreate",
             "temperatureModule/deactivate": "#/definitions/DeactivateTemperatureCreate",
             "temperatureModule/setTargetTemperature": "#/definitions/opentrons__protocol_engine__commands__temperature_module__set_target_temperature__SetTargetTemperatureCreate",
             "temperatureModule/waitForTemperature": "#/definitions/opentrons__protocol_engine__commands__temperature_module__wait_for_temperature__WaitForTemperatureCreate",
@@ -4277,14 +4346,17 @@
         {
             "$ref": "#/definitions/RetractAxisCreate"
         },
         {
             "$ref": "#/definitions/LoadLabwareCreate"
         },
         {
+            "$ref": "#/definitions/ReloadLabwareCreate"
+        },
+        {
             "$ref": "#/definitions/LoadLiquidCreate"
         },
         {
             "$ref": "#/definitions/LoadModuleCreate"
         },
         {
             "$ref": "#/definitions/LoadPipetteCreate"
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/commandAnnotation/schemas/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/commandAnnotation/schemas/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/deck/definitions/3/ot2_short_trash.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/deck/definitions/3/ot2_short_trash.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/deck/definitions/3/ot2_standard.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/deck/definitions/3/ot2_standard.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/deck/definitions/3/ot3_standard.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/deck/definitions/3/ot3_standard.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/deck/definitions/4/ot2_short_trash.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/deck/definitions/4/ot2_short_trash.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/deck/definitions/4/ot2_standard.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/deck/definitions/4/ot2_standard.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/deck/definitions/4/ot3_standard.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/deck/definitions/4/ot3_standard.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/deck/schemas/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/deck/schemas/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/deck/schemas/2.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/deck/schemas/2.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/deck/schemas/3.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/deck/schemas/3.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/deck/schemas/4.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/deck/schemas/4.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/errors/definitions/1/errors.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/errors/definitions/1/errors.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9861111111111112%*

 * *Differences: {"'codes'": "{'2016': OrderedDict([('detail', 'Motor Driver Error'), ('category', "*

 * *            "'roboticsControlError')]), '3019': OrderedDict([('detail', 'HEPA UV Failed'), "*

 * *            "('category', 'roboticsInteractionError')]), '4008': OrderedDict([('detail', 'Invalid "*

 * *            "stored data'), ('category', 'generalError')])}"}*

```diff
@@ -114,14 +114,18 @@
             "category": "roboticsControlError",
             "detail": "Execution Cancelled"
         },
         "2015": {
             "category": "roboticsControlError",
             "detail": "Gripper Pickup Failed"
         },
+        "2016": {
+            "category": "roboticsControlError",
+            "detail": "Motor Driver Error"
+        },
         "3000": {
             "category": "roboticsInteractionError",
             "detail": "A robotics interaction error occurred."
         },
         "3001": {
             "category": "roboticsInteractionError",
             "detail": "Labware Dropped"
@@ -186,14 +190,18 @@
             "category": "roboticsInteractionError",
             "detail": "Invalid Liquid Class Name"
         },
         "3018": {
             "category": "roboticsInteractionError",
             "detail": "Tip Detector Not Created"
         },
+        "3019": {
+            "category": "roboticsInteractionError",
+            "detail": "HEPA UV Failed"
+        },
         "4000": {
             "category": "generalError",
             "detail": "Unknown or Uncategorized Error"
         },
         "4001": {
             "category": "generalError",
             "detail": "Robot In Use"
@@ -217,10 +225,14 @@
         "4006": {
             "category": "generalError",
             "detail": "Invalid Protocol Data"
         },
         "4007": {
             "category": "generalError",
             "detail": "API Command is misconfigured"
+        },
+        "4008": {
+            "category": "generalError",
+            "detail": "Invalid stored data"
         }
     }
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/errors/schemas/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/errors/schemas/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/gripper/definitions/1/gripperV1.1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/gripper/definitions/1/gripperV1.1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/gripper/definitions/1/gripperV1.2.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/gripper/definitions/1/gripperV1.2.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/gripper/schemas/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/gripper/schemas/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/12-well-plate.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/12-well-plate.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/24-vial-rack.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/24-vial-rack.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/24-well-plate.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/24-well-plate.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/384-plate.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/384-plate.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/48-vial-plate.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/48-vial-plate.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/48-well-plate.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/48-well-plate.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/5ml-3x4.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/5ml-3x4.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/6-well-plate.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/6-well-plate.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/96-PCR-flat.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/96-PCR-flat.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/96-PCR-tall.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/96-PCR-tall.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/96-deep-well.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/96-deep-well.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/96-flat.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/96-flat.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/96-well-plate-20mm.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/96-well-plate-20mm.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/MALDI-plate.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/MALDI-plate.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/PCR-strip-tall.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/PCR-strip-tall.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/alum-block-pcr-strips.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/alum-block-pcr-strips.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/biorad-hardshell-96-PCR.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/biorad-hardshell-96-PCR.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/e-gelgol.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/e-gelgol.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/hampton-1ml-deep-block.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/hampton-1ml-deep-block.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/opentrons-aluminum-block-2ml-eppendorf.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/opentrons-aluminum-block-2ml-eppendorf.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/opentrons-aluminum-block-2ml-screwcap.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/opentrons-aluminum-block-2ml-screwcap.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/opentrons-aluminum-block-96-PCR-plate.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/opentrons-aluminum-block-96-PCR-plate.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/opentrons-aluminum-block-PCR-strips-200ul.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/opentrons-aluminum-block-PCR-strips-200ul.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/opentrons-tiprack-10ul.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/opentrons-tiprack-10ul.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/opentrons-tiprack-300ul.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/opentrons-tiprack-300ul.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/opentrons-tuberack-1.5ml-eppendorf.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/opentrons-tuberack-1.5ml-eppendorf.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/opentrons-tuberack-15_50ml.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/opentrons-tuberack-15_50ml.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/opentrons-tuberack-15ml.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/opentrons-tuberack-15ml.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/opentrons-tuberack-2ml-eppendorf.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/opentrons-tuberack-2ml-eppendorf.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/opentrons-tuberack-2ml-screwcap.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/opentrons-tuberack-2ml-screwcap.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/opentrons-tuberack-50ml.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/opentrons-tuberack-50ml.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/rigaku-compact-crystallization-plate.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/rigaku-compact-crystallization-plate.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/small_vial_rack_16x45.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/small_vial_rack_16x45.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/tiprack-1000ul-H.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/tiprack-1000ul-H.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/tiprack-1000ul-chem.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/tiprack-1000ul-chem.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/tiprack-1000ul.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/tiprack-1000ul.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/tiprack-10ul-H.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/tiprack-10ul-H.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/tiprack-10ul.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/tiprack-10ul.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/tiprack-200ul.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/tiprack-200ul.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/trough-12row-short.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/trough-12row-short.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/trough-12row.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/trough-12row.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/tube-rack-.75ml.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/tube-rack-.75ml.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/tube-rack-15_50ml.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/tube-rack-15_50ml.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/tube-rack-2ml-9x9.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/tube-rack-2ml-9x9.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/tube-rack-2ml.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/tube-rack-2ml.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/tube-rack-5ml-96.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/tube-rack-5ml-96.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/tube-rack-80well.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/tube-rack-80well.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/1/wheaton_vial_rack.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/1/wheaton_vial_rack.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/agilent_1_reservoir_290ml/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/agilent_1_reservoir_290ml/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/appliedbiosystemsmicroamp_384_wellplate_40ul/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/appliedbiosystemsmicroamp_384_wellplate_40ul/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/armadillo_96_wellplate_200ul_pcr_full_skirt/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/armadillo_96_wellplate_200ul_pcr_full_skirt/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/armadillo_96_wellplate_200ul_pcr_full_skirt/2.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/armadillo_96_wellplate_200ul_pcr_full_skirt/2.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/axygen_1_reservoir_90ml/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/axygen_1_reservoir_90ml/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/biorad_384_wellplate_50ul/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/biorad_384_wellplate_50ul/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/biorad_384_wellplate_50ul/2.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/biorad_384_wellplate_50ul/2.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/biorad_96_wellplate_200ul_pcr/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/biorad_96_wellplate_200ul_pcr/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/biorad_96_wellplate_200ul_pcr/2.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/biorad_96_wellplate_200ul_pcr/2.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/corning_12_wellplate_6.9ml_flat/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/corning_12_wellplate_6.9ml_flat/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/corning_12_wellplate_6.9ml_flat/2.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/corning_12_wellplate_6.9ml_flat/2.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/corning_24_wellplate_3.4ml_flat/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/corning_24_wellplate_3.4ml_flat/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/corning_24_wellplate_3.4ml_flat/2.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/corning_24_wellplate_3.4ml_flat/2.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/corning_384_wellplate_112ul_flat/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/corning_384_wellplate_112ul_flat/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/corning_384_wellplate_112ul_flat/2.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/corning_384_wellplate_112ul_flat/2.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/corning_48_wellplate_1.6ml_flat/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/corning_48_wellplate_1.6ml_flat/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/corning_48_wellplate_1.6ml_flat/2.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/corning_48_wellplate_1.6ml_flat/2.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/corning_6_wellplate_16.8ml_flat/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/corning_6_wellplate_16.8ml_flat/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/corning_6_wellplate_16.8ml_flat/2.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/corning_6_wellplate_16.8ml_flat/2.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/corning_96_wellplate_360ul_flat/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/corning_96_wellplate_360ul_flat/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/corning_96_wellplate_360ul_flat/2.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/corning_96_wellplate_360ul_flat/2.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/eppendorf_96_tiprack_1000ul_eptips/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/eppendorf_96_tiprack_1000ul_eptips/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/eppendorf_96_tiprack_10ul_eptips/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/eppendorf_96_tiprack_10ul_eptips/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/geb_96_tiprack_1000ul/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/geb_96_tiprack_1000ul/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/geb_96_tiprack_10ul/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/geb_96_tiprack_10ul/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/nest_12_reservoir_15ml/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/nest_12_reservoir_15ml/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/nest_1_reservoir_195ml/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/nest_1_reservoir_195ml/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/nest_1_reservoir_195ml/2.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/nest_1_reservoir_195ml/2.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/nest_1_reservoir_290ml/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/nest_1_reservoir_290ml/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/nest_96_wellplate_100ul_pcr_full_skirt/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/nest_96_wellplate_100ul_pcr_full_skirt/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/nest_96_wellplate_100ul_pcr_full_skirt/2.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/nest_96_wellplate_100ul_pcr_full_skirt/2.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/nest_96_wellplate_200ul_flat/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/nest_96_wellplate_200ul_flat/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/nest_96_wellplate_200ul_flat/2.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/nest_96_wellplate_200ul_flat/2.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/nest_96_wellplate_2ml_deep/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/nest_96_wellplate_2ml_deep/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/nest_96_wellplate_2ml_deep/2.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/nest_96_wellplate_2ml_deep/2.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_10_tuberack_falcon_4x50ml_6x15ml_conical/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_10_tuberack_falcon_4x50ml_6x15ml_conical/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_10_tuberack_falcon_4x50ml_6x15ml_conical_acrylic/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_10_tuberack_falcon_4x50ml_6x15ml_conical_acrylic/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_10_tuberack_nest_4x50ml_6x15ml_conical/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_10_tuberack_nest_4x50ml_6x15ml_conical/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_15_tuberack_falcon_15ml_conical/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_15_tuberack_falcon_15ml_conical/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_15_tuberack_nest_15ml_conical/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_15_tuberack_nest_15ml_conical/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_1_trash_1100ml_fixed/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_1_trash_1100ml_fixed/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_1_trash_3200ml_fixed/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_1_trash_3200ml_fixed/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_1_trash_850ml_fixed/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_1_trash_850ml_fixed/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_24_aluminumblock_generic_2ml_screwcap/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_24_aluminumblock_generic_2ml_screwcap/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_24_aluminumblock_generic_2ml_screwcap/2.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_24_aluminumblock_generic_2ml_screwcap/2.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_24_aluminumblock_nest_0.5ml_screwcap/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_24_aluminumblock_nest_0.5ml_screwcap/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_24_aluminumblock_nest_1.5ml_screwcap/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_24_aluminumblock_nest_1.5ml_screwcap/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_24_aluminumblock_nest_1.5ml_snapcap/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_24_aluminumblock_nest_1.5ml_snapcap/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_24_aluminumblock_nest_2ml_screwcap/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_24_aluminumblock_nest_2ml_screwcap/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_24_aluminumblock_nest_2ml_snapcap/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_24_aluminumblock_nest_2ml_snapcap/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_24_tuberack_eppendorf_1.5ml_safelock_snapcap/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_24_tuberack_eppendorf_1.5ml_safelock_snapcap/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_24_tuberack_eppendorf_2ml_safelock_snapcap/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_24_tuberack_eppendorf_2ml_safelock_snapcap/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_24_tuberack_eppendorf_2ml_safelock_snapcap_acrylic/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_24_tuberack_eppendorf_2ml_safelock_snapcap_acrylic/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_24_tuberack_generic_0.75ml_snapcap_acrylic/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_24_tuberack_generic_0.75ml_snapcap_acrylic/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_24_tuberack_generic_2ml_screwcap/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_24_tuberack_generic_2ml_screwcap/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_24_tuberack_nest_0.5ml_screwcap/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_24_tuberack_nest_0.5ml_screwcap/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_24_tuberack_nest_1.5ml_screwcap/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_24_tuberack_nest_1.5ml_screwcap/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_24_tuberack_nest_1.5ml_snapcap/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_24_tuberack_nest_1.5ml_snapcap/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_24_tuberack_nest_2ml_screwcap/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_24_tuberack_nest_2ml_screwcap/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_24_tuberack_nest_2ml_snapcap/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_24_tuberack_nest_2ml_snapcap/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_40_aluminumblock_eppendorf_24x2ml_safelock_snapcap_generic_16x0.2ml_pcr_strip/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_40_aluminumblock_eppendorf_24x2ml_safelock_snapcap_generic_16x0.2ml_pcr_strip/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_6_tuberack_falcon_50ml_conical/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_6_tuberack_falcon_50ml_conical/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_6_tuberack_nest_50ml_conical/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_6_tuberack_nest_50ml_conical/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_96_aluminumblock_biorad_wellplate_200ul/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_96_aluminumblock_biorad_wellplate_200ul/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_96_aluminumblock_generic_pcr_strip_200ul/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_96_aluminumblock_generic_pcr_strip_200ul/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_96_aluminumblock_generic_pcr_strip_200ul/2.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_96_aluminumblock_generic_pcr_strip_200ul/2.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_96_aluminumblock_nest_wellplate_100ul/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_96_aluminumblock_nest_wellplate_100ul/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_96_deep_well_adapter/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_96_deep_well_adapter/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_96_deep_well_adapter_nest_wellplate_2ml_deep/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_96_deep_well_adapter_nest_wellplate_2ml_deep/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_96_filtertiprack_1000ul/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_96_filtertiprack_1000ul/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_96_filtertiprack_10ul/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_96_filtertiprack_10ul/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_96_filtertiprack_200ul/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_96_filtertiprack_200ul/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_96_filtertiprack_20ul/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_96_filtertiprack_20ul/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_96_flat_bottom_adapter/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_96_flat_bottom_adapter/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_96_flat_bottom_adapter_nest_wellplate_200ul_flat/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_96_flat_bottom_adapter_nest_wellplate_200ul_flat/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_96_pcr_adapter/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_96_pcr_adapter/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_96_pcr_adapter_armadillo_wellplate_200ul/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_96_pcr_adapter_armadillo_wellplate_200ul/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_96_pcr_adapter_nest_wellplate_100ul_pcr_full_skirt/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_96_pcr_adapter_nest_wellplate_100ul_pcr_full_skirt/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_96_tiprack_1000ul/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_96_tiprack_1000ul/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_96_tiprack_10ul/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_96_tiprack_10ul/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_96_tiprack_20ul/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_96_tiprack_20ul/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_96_tiprack_300ul/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_96_tiprack_300ul/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_96_well_aluminum_block/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_96_well_aluminum_block/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_96_wellplate_200ul_pcr_full_skirt/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_96_wellplate_200ul_pcr_full_skirt/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_96_wellplate_200ul_pcr_full_skirt/2.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_96_wellplate_200ul_pcr_full_skirt/2.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_aluminum_flat_bottom_plate/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_aluminum_flat_bottom_plate/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_calibration_adapter_heatershaker_module/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_calibration_adapter_heatershaker_module/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_calibration_adapter_temperature_module/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_calibration_adapter_temperature_module/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_calibration_adapter_thermocycler_module/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_calibration_adapter_thermocycler_module/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_calibrationblock_short_side_left/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_calibrationblock_short_side_left/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_calibrationblock_short_side_right/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_calibrationblock_short_side_right/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_flex_96_filtertiprack_1000ul/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_flex_96_filtertiprack_1000ul/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_flex_96_filtertiprack_200ul/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_flex_96_filtertiprack_200ul/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_flex_96_filtertiprack_50ul/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_flex_96_filtertiprack_50ul/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_flex_96_tiprack_1000ul/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_flex_96_tiprack_1000ul/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_flex_96_tiprack_200ul/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_flex_96_tiprack_200ul/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_flex_96_tiprack_50ul/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_flex_96_tiprack_50ul/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_flex_96_tiprack_adapter/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_flex_96_tiprack_adapter/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_universal_flat_adapter/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_universal_flat_adapter/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/opentrons_universal_flat_adapter_corning_384_wellplate_112ul_flat/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/opentrons_universal_flat_adapter_corning_384_wellplate_112ul_flat/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/thermoscientificnunc_96_wellplate_1300ul/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/thermoscientificnunc_96_wellplate_1300ul/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/thermoscientificnunc_96_wellplate_2000ul/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/thermoscientificnunc_96_wellplate_2000ul/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/tipone_96_tiprack_200ul/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/tipone_96_tiprack_200ul/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/usascientific_12_reservoir_22ml/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/usascientific_12_reservoir_22ml/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/definitions/2/usascientific_96_wellplate_2.4ml_deep/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/definitions/2/usascientific_96_wellplate_2.4ml_deep/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/labware/schemas/2.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/labware/schemas/2.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/liquid/schemas/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/liquid/schemas/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/module/definitions/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/module/definitions/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/module/definitions/2/magneticModuleV2.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/module/definitions/2/magneticModuleV2.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/module/definitions/2/temperatureModuleV2.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/module/definitions/2/temperatureModuleV2.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/module/definitions/3/heaterShakerModuleV1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/module/definitions/3/heaterShakerModuleV1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/module/definitions/3/magneticBlockV1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/module/definitions/3/magneticBlockV1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/module/definitions/3/magneticModuleV1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/module/definitions/3/magneticModuleV1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/module/definitions/3/magneticModuleV2.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/module/definitions/3/magneticModuleV2.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/module/definitions/3/temperatureModuleV1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/module/definitions/3/temperatureModuleV1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/module/definitions/3/temperatureModuleV2.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/module/definitions/3/temperatureModuleV2.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/module/definitions/3/thermocyclerModuleV1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/module/definitions/3/thermocyclerModuleV1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/module/definitions/3/thermocyclerModuleV2.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/module/definitions/3/thermocyclerModuleV2.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/module/schemas/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/module/schemas/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/module/schemas/2.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/module/schemas/2.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/module/schemas/3.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/module/schemas/3.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/1/pipetteModelSpecs.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/1/pipetteModelSpecs.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9976190476190476%*

 * *Differences: {"'config'": "{'p50_single_v3.6': OrderedDict([('name', 'p50_single_flex'), ('backCompatNames', "*

 * *             "[]), ('top', OrderedDict([('value', 0.5), ('min', 0), ('max', 45), ('units', 'mm'), "*

 * *             "('type', 'float')])), ('bottom', OrderedDict([('value', 71.5), ('min', 55), ('max', "*

 * *             "80), ('type', 'float'), ('units', 'mm')])), ('blowout', OrderedDict([('value', "*

 * *             "76.5), ('min', 60), ('max', 85), ('units', 'mm'), ('type', 'float')])), ('dropTip', "*

 * *             "Order […]*

```diff
@@ -21626,14 +21626,414 @@
                             0.0001,
                             0.7382
                         ]
                     ]
                 }
             ]
         },
+        "p50_single_v3.6": {
+            "backCompatNames": [],
+            "blowout": {
+                "max": 85,
+                "min": 60,
+                "type": "float",
+                "units": "mm",
+                "value": 76.5
+            },
+            "bottom": {
+                "max": 80,
+                "min": 55,
+                "type": "float",
+                "units": "mm",
+                "value": 71.5
+            },
+            "dropTip": {
+                "max": 119,
+                "min": 78,
+                "type": "float",
+                "units": "mm",
+                "value": 90.5
+            },
+            "dropTipCurrent": {
+                "max": 1.25,
+                "min": 0.1,
+                "type": "float",
+                "units": "amps",
+                "value": 1.0
+            },
+            "dropTipSpeed": {
+                "max": 30,
+                "min": 0.001,
+                "type": "float",
+                "units": "mm/sec",
+                "value": 7
+            },
+            "idleCurrent": 0.3,
+            "modelOffset": [
+                0.0,
+                0.0,
+                25.14
+            ],
+            "name": "p50_single_flex",
+            "nozzleOffset": [
+                -8.0,
+                -22.0,
+                -259.15
+            ],
+            "pickUpCurrent": {
+                "max": 2.0,
+                "min": 0.05,
+                "type": "float",
+                "units": "amps",
+                "value": 0.15
+            },
+            "pickUpDistance": {
+                "max": 30,
+                "min": 1,
+                "type": "float",
+                "units": "mm",
+                "value": 15
+            },
+            "pickUpIncrement": {
+                "max": 10.0,
+                "min": 0.0,
+                "type": "float",
+                "units": "mm",
+                "value": 0.0
+            },
+            "pickUpPresses": {
+                "max": 10,
+                "min": 0,
+                "type": "int",
+                "units": "presses",
+                "value": 1
+            },
+            "pickUpSpeed": {
+                "max": 30,
+                "min": 1,
+                "type": "float",
+                "units": "mm/s",
+                "value": 5
+            },
+            "plungerCurrent": {
+                "max": 1.5,
+                "min": 0.1,
+                "type": "float",
+                "units": "amps",
+                "value": 1.0
+            },
+            "quirks": [],
+            "returnTipHeight": 0.78,
+            "tipLength": {
+                "max": 100,
+                "min": 0,
+                "type": "float",
+                "units": "mm",
+                "value": 78.3
+            },
+            "tipOverlap": {
+                "default": 10.5,
+                "opentrons/opentrons_96_tiprack_50ul/1": 10.5
+            },
+            "top": {
+                "max": 45,
+                "min": 0,
+                "type": "float",
+                "units": "mm",
+                "value": 0.5
+            },
+            "ulPerMm": [
+                {
+                    "aspirate": [
+                        [
+                            0.6464,
+                            0.4817,
+                            0.0427
+                        ],
+                        [
+                            1.0889,
+                            0.2539,
+                            0.1591
+                        ],
+                        [
+                            1.5136,
+                            0.1624,
+                            0.2587
+                        ],
+                        [
+                            1.9108,
+                            0.1042,
+                            0.3467
+                        ],
+                        [
+                            2.2941,
+                            0.0719,
+                            0.4085
+                        ],
+                        [
+                            2.9978,
+                            0.037,
+                            0.4886
+                        ],
+                        [
+                            3.7731,
+                            0.0378,
+                            0.4863
+                        ],
+                        [
+                            4.7575,
+                            0.0516,
+                            0.4342
+                        ],
+                        [
+                            5.5024,
+                            0.011,
+                            0.6275
+                        ],
+                        [
+                            6.2686,
+                            0.0114,
+                            0.6253
+                        ],
+                        [
+                            7.005,
+                            0.0054,
+                            0.6625
+                        ],
+                        [
+                            8.5207,
+                            0.0063,
+                            0.6563
+                        ],
+                        [
+                            10.0034,
+                            0.003,
+                            0.6844
+                        ],
+                        [
+                            11.5075,
+                            0.0031,
+                            0.6833
+                        ],
+                        [
+                            13.0327,
+                            0.0032,
+                            0.6829
+                        ],
+                        [
+                            14.5356,
+                            0.0018,
+                            0.7003
+                        ],
+                        [
+                            17.5447,
+                            0.0014,
+                            0.7063
+                        ],
+                        [
+                            20.5576,
+                            0.0011,
+                            0.7126
+                        ],
+                        [
+                            23.5624,
+                            0.0007,
+                            0.7197
+                        ],
+                        [
+                            26.5785,
+                            0.0007,
+                            0.721
+                        ],
+                        [
+                            29.593,
+                            0.0005,
+                            0.7248
+                        ],
+                        [
+                            32.6109,
+                            0.0004,
+                            0.7268
+                        ],
+                        [
+                            35.6384,
+                            0.0004,
+                            0.727
+                        ],
+                        [
+                            38.6439,
+                            0.0002,
+                            0.7343
+                        ],
+                        [
+                            41.6815,
+                            0.0004,
+                            0.7284
+                        ],
+                        [
+                            44.6895,
+                            0.0002,
+                            0.7372
+                        ],
+                        [
+                            47.6926,
+                            0.0001,
+                            0.7393
+                        ],
+                        [
+                            51.4567,
+                            0.0001,
+                            0.7382
+                        ]
+                    ],
+                    "dispense": [
+                        [
+                            0.6464,
+                            0.4817,
+                            0.0427
+                        ],
+                        [
+                            1.0889,
+                            0.2539,
+                            0.1591
+                        ],
+                        [
+                            1.5136,
+                            0.1624,
+                            0.2587
+                        ],
+                        [
+                            1.9108,
+                            0.1042,
+                            0.3467
+                        ],
+                        [
+                            2.2941,
+                            0.0719,
+                            0.4085
+                        ],
+                        [
+                            2.9978,
+                            0.037,
+                            0.4886
+                        ],
+                        [
+                            3.7731,
+                            0.0378,
+                            0.4863
+                        ],
+                        [
+                            4.7575,
+                            0.0516,
+                            0.4342
+                        ],
+                        [
+                            5.5024,
+                            0.011,
+                            0.6275
+                        ],
+                        [
+                            6.2686,
+                            0.0114,
+                            0.6253
+                        ],
+                        [
+                            7.005,
+                            0.0054,
+                            0.6625
+                        ],
+                        [
+                            8.5207,
+                            0.0063,
+                            0.6563
+                        ],
+                        [
+                            10.0034,
+                            0.003,
+                            0.6844
+                        ],
+                        [
+                            11.5075,
+                            0.0031,
+                            0.6833
+                        ],
+                        [
+                            13.0327,
+                            0.0032,
+                            0.6829
+                        ],
+                        [
+                            14.5356,
+                            0.0018,
+                            0.7003
+                        ],
+                        [
+                            17.5447,
+                            0.0014,
+                            0.7063
+                        ],
+                        [
+                            20.5576,
+                            0.0011,
+                            0.7126
+                        ],
+                        [
+                            23.5624,
+                            0.0007,
+                            0.7197
+                        ],
+                        [
+                            26.5785,
+                            0.0007,
+                            0.721
+                        ],
+                        [
+                            29.593,
+                            0.0005,
+                            0.7248
+                        ],
+                        [
+                            32.6109,
+                            0.0004,
+                            0.7268
+                        ],
+                        [
+                            35.6384,
+                            0.0004,
+                            0.727
+                        ],
+                        [
+                            38.6439,
+                            0.0002,
+                            0.7343
+                        ],
+                        [
+                            41.6815,
+                            0.0004,
+                            0.7284
+                        ],
+                        [
+                            44.6895,
+                            0.0002,
+                            0.7372
+                        ],
+                        [
+                            47.6926,
+                            0.0001,
+                            0.7393
+                        ],
+                        [
+                            51.4567,
+                            0.0001,
+                            0.7382
+                        ]
+                    ]
+                }
+            ]
+        },
         "p50_single_v4.3": {
             "backCompatNames": [],
             "blowout": {
                 "max": 85,
                 "min": 60,
                 "type": "float",
                 "units": "mm",
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/1/pipetteNameSpecs.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/1/pipetteNameSpecs.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p10/1_0.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p10/1_3.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8969275210084033%*

 * *Differences: {"'channels'": '1',*

 * * "'displayName'": "'P10 Single-Channel GEN1'",*

 * * "'partialTipConfigurations'": "{'partialTipSupported': False, 'availableConfigurations': None}",*

 * * "'pickUpTipConfigurations'": "{'pressFit': {'currentByTipCount': {delete: ['2', '3', '4', '5', "*

 * *                              "'6', '7', '8']}, 'speedByTipCount': OrderedDict([('1', 30.0)]), "*

 * *                              "'distanceByTipCount': OrderedDict([('1', 10.0)]), delete: ['speed', "*

 * *                              "'distance']}}",*

 * * "'p […]*

```diff
@@ -1,68 +1,56 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipettePropertiesSchema.json",
     "availableSensors": {
         "sensors": []
     },
     "backCompatNames": [],
     "backlashDistance": 0.0,
-    "channels": 8,
+    "channels": 1,
     "displayCategory": "GEN1",
-    "displayName": "P10 8-Channel GEN1",
+    "displayName": "P10 Single-Channel GEN1",
     "dropTipConfigurations": {
         "plungerEject": {
             "current": 0.5,
             "speed": 5.0
         }
     },
     "model": "p10",
     "partialTipConfigurations": {
-        "availableConfigurations": [
-            1,
-            2,
-            3,
-            4,
-            5,
-            6,
-            7,
-            8
-        ],
-        "partialTipSupported": true
+        "availableConfigurations": null,
+        "partialTipSupported": false
     },
     "pickUpTipConfigurations": {
         "pressFit": {
             "currentByTipCount": {
-                "1": 0.1,
-                "2": 0.1,
-                "3": 0.15,
-                "4": 0.2,
-                "5": 0.25,
-                "6": 0.3,
-                "7": 0.35,
-                "8": 0.4
+                "1": 0.1
+            },
+            "distanceByTipCount": {
+                "1": 10.0
             },
-            "distance": 10.0,
             "increment": 1.0,
             "presses": 3,
-            "speed": 30.0
+            "speedByTipCount": {
+                "1": 30.0
+            }
         }
     },
     "plungerHomingConfigurations": {
-        "current": 0.5,
+        "current": 0.3,
         "speed": 30
     },
     "plungerMotorConfigurations": {
         "idle": 0.05,
-        "run": 0.5
+        "run": 0.3
     },
     "plungerPositionsConfigurations": {
         "default": {
-            "blowout": -1.0,
-            "bottom": 2.0,
-            "drop": -4.0,
+            "blowout": -2.5,
+            "bottom": 0.5,
+            "drop": -6.0,
             "top": 19.5
         }
     },
     "quirks": [
         "dropTipShake"
     ],
     "shaftDiameter": 1.0,
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p10/1_3.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p10/1_4.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8969275210084033%*

 * *Differences: {"'channels'": '1',*

 * * "'displayName'": "'P10 Single-Channel GEN1'",*

 * * "'partialTipConfigurations'": "{'partialTipSupported': False, 'availableConfigurations': None}",*

 * * "'pickUpTipConfigurations'": "{'pressFit': {'currentByTipCount': {delete: ['2', '3', '4', '5', "*

 * *                              "'6', '7', '8']}, 'speedByTipCount': OrderedDict([('1', 30.0)]), "*

 * *                              "'distanceByTipCount': OrderedDict([('1', 10.0)]), delete: ['speed', "*

 * *                              "'distance']}}",*

 * * "'p […]*

```diff
@@ -1,68 +1,56 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipettePropertiesSchema.json",
     "availableSensors": {
         "sensors": []
     },
     "backCompatNames": [],
     "backlashDistance": 0.0,
-    "channels": 8,
+    "channels": 1,
     "displayCategory": "GEN1",
-    "displayName": "P10 8-Channel GEN1",
+    "displayName": "P10 Single-Channel GEN1",
     "dropTipConfigurations": {
         "plungerEject": {
             "current": 0.5,
             "speed": 5.0
         }
     },
     "model": "p10",
     "partialTipConfigurations": {
-        "availableConfigurations": [
-            1,
-            2,
-            3,
-            4,
-            5,
-            6,
-            7,
-            8
-        ],
-        "partialTipSupported": true
+        "availableConfigurations": null,
+        "partialTipSupported": false
     },
     "pickUpTipConfigurations": {
         "pressFit": {
             "currentByTipCount": {
-                "1": 0.1,
-                "2": 0.1,
-                "3": 0.15,
-                "4": 0.2,
-                "5": 0.25,
-                "6": 0.3,
-                "7": 0.35,
-                "8": 0.4
+                "1": 0.1
+            },
+            "distanceByTipCount": {
+                "1": 10.0
             },
-            "distance": 10.0,
             "increment": 1.0,
             "presses": 3,
-            "speed": 30.0
+            "speedByTipCount": {
+                "1": 30.0
+            }
         }
     },
     "plungerHomingConfigurations": {
-        "current": 0.5,
+        "current": 0.3,
         "speed": 30
     },
     "plungerMotorConfigurations": {
         "idle": 0.05,
-        "run": 0.5
+        "run": 0.3
     },
     "plungerPositionsConfigurations": {
         "default": {
-            "blowout": -2.5,
-            "bottom": 0.5,
-            "drop": -5.5,
+            "blowout": -0.5,
+            "bottom": 2.5,
+            "drop": -5.2,
             "top": 19.5
         }
     },
     "quirks": [
         "dropTipShake"
     ],
     "shaftDiameter": 1.0,
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p10/1_4.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p10/1_5.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8969275210084033%*

 * *Differences: {"'channels'": '1',*

 * * "'displayName'": "'P10 Single-Channel GEN1'",*

 * * "'partialTipConfigurations'": "{'partialTipSupported': False, 'availableConfigurations': None}",*

 * * "'pickUpTipConfigurations'": "{'pressFit': {'currentByTipCount': {delete: ['2', '3', '4', '5', "*

 * *                              "'6', '7', '8']}, 'speedByTipCount': OrderedDict([('1', 30.0)]), "*

 * *                              "'distanceByTipCount': OrderedDict([('1', 10.0)]), delete: ['speed', "*

 * *                              "'distance']}}",*

 * * "'p […]*

```diff
@@ -1,68 +1,56 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipettePropertiesSchema.json",
     "availableSensors": {
         "sensors": []
     },
     "backCompatNames": [],
     "backlashDistance": 0.0,
-    "channels": 8,
+    "channels": 1,
     "displayCategory": "GEN1",
-    "displayName": "P10 8-Channel GEN1",
+    "displayName": "P10 Single-Channel GEN1",
     "dropTipConfigurations": {
         "plungerEject": {
             "current": 0.5,
             "speed": 5.0
         }
     },
     "model": "p10",
     "partialTipConfigurations": {
-        "availableConfigurations": [
-            1,
-            2,
-            3,
-            4,
-            5,
-            6,
-            7,
-            8
-        ],
-        "partialTipSupported": true
+        "availableConfigurations": null,
+        "partialTipSupported": false
     },
     "pickUpTipConfigurations": {
         "pressFit": {
             "currentByTipCount": {
-                "1": 0.1,
-                "2": 0.1,
-                "3": 0.15,
-                "4": 0.2,
-                "5": 0.25,
-                "6": 0.3,
-                "7": 0.35,
-                "8": 0.4
+                "1": 0.1
+            },
+            "distanceByTipCount": {
+                "1": 10.0
             },
-            "distance": 10.0,
             "increment": 1.0,
             "presses": 3,
-            "speed": 30.0
+            "speedByTipCount": {
+                "1": 30.0
+            }
         }
     },
     "plungerHomingConfigurations": {
-        "current": 0.5,
+        "current": 0.3,
         "speed": 30
     },
     "plungerMotorConfigurations": {
         "idle": 0.05,
-        "run": 0.5
+        "run": 0.3
     },
     "plungerPositionsConfigurations": {
         "default": {
-            "blowout": -1.0,
-            "bottom": 2.0,
-            "drop": -4.5,
+            "blowout": -0.5,
+            "bottom": 2.5,
+            "drop": -5.2,
             "top": 19.5
         }
     },
     "quirks": [
         "dropTipShake"
     ],
     "shaftDiameter": 1.0,
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p10/1_5.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p10/1_3.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9698660714285715%*

 * *Differences: {"'pickUpTipConfigurations'": "{'pressFit': {'increment': 1.0, 'currentByTipCount': {'2': 0.1, "*

 * *                              "'3': 0.15, '4': 0.2, '5': 0.25, '6': 0.3, '7': 0.35, '8': 0.4}, "*

 * *                              "'speedByTipCount': OrderedDict([('1', 30.0), ('2', 30.0), ('3', "*

 * *                              "30.0), ('4', 30.0), ('5', 30.0), ('6', 30.0), ('7', 30.0), ('8', "*

 * *                              "30.0)]), 'distanceByTipCount': OrderedDict([('1', 10.0), ('2', "*

 * *                            […]*

```diff
@@ -28,44 +28,61 @@
         ],
         "partialTipSupported": true
     },
     "pickUpTipConfigurations": {
         "pressFit": {
             "currentByTipCount": {
                 "1": 0.1,
-                "2": 0.14,
-                "3": 0.21,
-                "4": 0.28,
-                "5": 0.34,
-                "6": 0.41,
-                "7": 0.48,
-                "8": 0.55
+                "2": 0.1,
+                "3": 0.15,
+                "4": 0.2,
+                "5": 0.25,
+                "6": 0.3,
+                "7": 0.35,
+                "8": 0.4
             },
-            "distance": 10.0,
-            "increment": 3.0,
+            "distanceByTipCount": {
+                "1": 10.0,
+                "2": 10.0,
+                "3": 10.0,
+                "4": 10.0,
+                "5": 10.0,
+                "6": 10.0,
+                "7": 10.0,
+                "8": 10.0
+            },
+            "increment": 1.0,
             "presses": 3,
-            "speed": 30.0
+            "speedByTipCount": {
+                "1": 30.0,
+                "2": 30.0,
+                "3": 30.0,
+                "4": 30.0,
+                "5": 30.0,
+                "6": 30.0,
+                "7": 30.0,
+                "8": 30.0
+            }
         }
     },
     "plungerHomingConfigurations": {
         "current": 0.5,
         "speed": 30
     },
     "plungerMotorConfigurations": {
         "idle": 0.05,
         "run": 0.5
     },
     "plungerPositionsConfigurations": {
         "default": {
-            "blowout": -1.0,
-            "bottom": 2.0,
-            "drop": -4.5,
+            "blowout": -2.5,
+            "bottom": 0.5,
+            "drop": -5.5,
             "top": 19.5
         }
     },
     "quirks": [
-        "dropTipShake",
-        "doubleDropTip"
+        "dropTipShake"
     ],
     "shaftDiameter": 1.0,
     "shaftULperMM": 0.785
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p10/1_6.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p1000/3_0.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6760110294117647%*

 * *Differences: {"'availableSensors'": "{'sensors': ['pressure', 'capacitive', 'environment'], 'pressure': "*

 * *                       "OrderedDict([('count', 1)]), 'capacitive': OrderedDict([('count', 1)]), "*

 * *                       "'environment': OrderedDict([('count', 1)])}",*

 * * "'backlashDistance'": '0.1',*

 * * "'channels'": '1',*

 * * "'displayCategory'": "'FLEX'",*

 * * "'displayName'": "'Flex 1-Channel 1000 μL'",*

 * * "'dropTipConfigurations'": "{'plungerEject': {'current': 1.0, 'speed': 10}}",*

 * * "'model'": "'p1000'",*

 * * "'partialTipConfigur […]*

```diff
@@ -1,71 +1,69 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipettePropertiesSchema.json",
     "availableSensors": {
-        "sensors": []
+        "capacitive": {
+            "count": 1
+        },
+        "environment": {
+            "count": 1
+        },
+        "pressure": {
+            "count": 1
+        },
+        "sensors": [
+            "pressure",
+            "capacitive",
+            "environment"
+        ]
     },
     "backCompatNames": [],
-    "backlashDistance": 0.0,
-    "channels": 8,
-    "displayCategory": "GEN1",
-    "displayName": "P10 8-Channel GEN1",
+    "backlashDistance": 0.1,
+    "channels": 1,
+    "displayCategory": "FLEX",
+    "displayName": "Flex 1-Channel 1000 \u03bcL",
     "dropTipConfigurations": {
         "plungerEject": {
-            "current": 0.5,
-            "speed": 5.0
+            "current": 1.0,
+            "speed": 10
         }
     },
-    "model": "p10",
+    "model": "p1000",
     "partialTipConfigurations": {
-        "availableConfigurations": [
-            1,
-            2,
-            3,
-            4,
-            5,
-            6,
-            7,
-            8
-        ],
-        "partialTipSupported": true
+        "availableConfigurations": null,
+        "partialTipSupported": false
     },
     "pickUpTipConfigurations": {
         "pressFit": {
             "currentByTipCount": {
-                "1": 0.1,
-                "2": 0.14,
-                "3": 0.21,
-                "4": 0.28,
-                "5": 0.34,
-                "6": 0.41,
-                "7": 0.48,
-                "8": 0.55
+                "1": 0.15
             },
-            "distance": 10.0,
-            "increment": 3.0,
-            "presses": 3,
-            "speed": 30.0
+            "distanceByTipCount": {
+                "1": 13.0
+            },
+            "increment": 0.0,
+            "presses": 1,
+            "speedByTipCount": {
+                "1": 5.0
+            }
         }
     },
     "plungerHomingConfigurations": {
-        "current": 0.5,
+        "current": 1.0,
         "speed": 30
     },
     "plungerMotorConfigurations": {
-        "idle": 0.05,
-        "run": 0.5
+        "idle": 0.3,
+        "run": 1.0
     },
     "plungerPositionsConfigurations": {
         "default": {
-            "blowout": -1.0,
-            "bottom": 2.0,
-            "drop": -4.5,
-            "top": 19.5
+            "blowout": 76.5,
+            "bottom": 71.5,
+            "drop": 90.5,
+            "top": 0.5
         }
     },
-    "quirks": [
-        "dropTipShake",
-        "doubleDropTip"
-    ],
-    "shaftDiameter": 1.0,
-    "shaftULperMM": 0.785
+    "quirks": [],
+    "shaftDiameter": 4.5,
+    "shaftULperMM": 15.904
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p1000/1_0.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p50/3_4.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7755383403361344%*

 * *Differences: {"'availableSensors'": "{'pressure': {'count': 1}, 'capacitive': {'count': 1}}",*

 * * "'backlashDistance'": '0.1',*

 * * "'channels'": '1',*

 * * "'displayName'": "'Flex 1-Channel 50 μL'",*

 * * "'dropTipConfigurations'": "{'plungerEject': {'speed': 15}}",*

 * * "'model'": "'p50'",*

 * * "'partialTipConfigurations'": "{'partialTipSupported': False, 'availableConfigurations': None}",*

 * * "'pickUpTipConfigurations'": "{'pressFit': {'currentByTipCount': {'1': 0.2, delete: ['2', '3', "*

 * *                              "'4', '5', '6', '7', '8']}, […]*

```diff
@@ -1,81 +1,75 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipettePropertiesSchema.json",
     "availableSensors": {
         "capacitive": {
-            "count": 2
+            "count": 1
         },
         "environment": {
             "count": 1
         },
         "pressure": {
-            "count": 2
+            "count": 1
         },
         "sensors": [
             "pressure",
             "capacitive",
             "environment"
         ]
     },
     "backCompatNames": [],
-    "backlashDistance": 0.0,
-    "channels": 8,
+    "backlashDistance": 0.1,
+    "channels": 1,
     "displayCategory": "FLEX",
-    "displayName": "Flex 8-Channel 1000 uL",
+    "displayName": "Flex 1-Channel 50 \u03bcL",
     "dropTipConfigurations": {
         "plungerEject": {
             "current": 1.0,
-            "speed": 10
+            "speed": 15
         }
     },
-    "model": "p1000",
+    "model": "p50",
     "partialTipConfigurations": {
-        "availableConfigurations": [
-            1,
-            2,
-            3,
-            4,
-            5,
-            6,
-            7,
-            8
-        ],
-        "partialTipSupported": true
+        "availableConfigurations": null,
+        "partialTipSupported": false
     },
     "pickUpTipConfigurations": {
         "pressFit": {
             "currentByTipCount": {
-                "1": 0.15,
-                "2": 0.13,
-                "3": 0.19,
-                "4": 0.25,
-                "5": 0.31,
-                "6": 0.38,
-                "7": 0.44,
-                "8": 0.5
+                "1": 0.2
+            },
+            "distanceByTipCount": {
+                "1": 13.0
             },
-            "distance": 13.0,
             "increment": 0.0,
             "presses": 1,
-            "speed": 10
+            "speedByTipCount": {
+                "1": 10.0
+            }
         }
     },
     "plungerHomingConfigurations": {
         "current": 1.0,
         "speed": 30
     },
     "plungerMotorConfigurations": {
         "idle": 0.3,
         "run": 1.0
     },
     "plungerPositionsConfigurations": {
         "default": {
             "blowout": 76.5,
             "bottom": 71.5,
-            "drop": 92.5,
-            "top": 0.5
+            "drop": 90.5,
+            "top": 0.0
+        },
+        "lowVolumeDefault": {
+            "blowout": 76.5,
+            "bottom": 61.5,
+            "drop": 90.5,
+            "top": 0.0
         }
     },
     "quirks": [],
-    "shaftDiameter": 9.0,
-    "shaftULperMM": 63.617
+    "shaftDiameter": 1.0,
+    "shaftULperMM": 0.785
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p1000/3_0.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p50/3_5.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8049501050420167%*

 * *Differences: {"'availableSensors'": "{'pressure': {'count': 1}, 'capacitive': {'count': 1}}",*

 * * "'channels'": '1',*

 * * "'displayName'": "'Flex 1-Channel 50 μL'",*

 * * "'dropTipConfigurations'": "{'plungerEject': {'speed': 15}}",*

 * * "'model'": "'p50'",*

 * * "'partialTipConfigurations'": "{'partialTipSupported': False, 'availableConfigurations': None}",*

 * * "'pickUpTipConfigurations'": "{'pressFit': {'currentByTipCount': {'1': 0.2, delete: ['2', '3', "*

 * *                              "'4', '5', '6', '7', '8']}, 'speedByTipCount': OrderedDic […]*

```diff
@@ -1,81 +1,75 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipettePropertiesSchema.json",
     "availableSensors": {
         "capacitive": {
-            "count": 2
+            "count": 1
         },
         "environment": {
             "count": 1
         },
         "pressure": {
-            "count": 2
+            "count": 1
         },
         "sensors": [
             "pressure",
             "capacitive",
             "environment"
         ]
     },
     "backCompatNames": [],
     "backlashDistance": 0.1,
-    "channels": 8,
+    "channels": 1,
     "displayCategory": "FLEX",
-    "displayName": "Flex 8-Channel 1000 \u03bcL",
+    "displayName": "Flex 1-Channel 50 \u03bcL",
     "dropTipConfigurations": {
         "plungerEject": {
             "current": 1.0,
-            "speed": 10
+            "speed": 15
         }
     },
-    "model": "p1000",
+    "model": "p50",
     "partialTipConfigurations": {
-        "availableConfigurations": [
-            1,
-            2,
-            3,
-            4,
-            5,
-            6,
-            7,
-            8
-        ],
-        "partialTipSupported": true
+        "availableConfigurations": null,
+        "partialTipSupported": false
     },
     "pickUpTipConfigurations": {
         "pressFit": {
             "currentByTipCount": {
-                "1": 0.15,
-                "2": 0.13,
-                "3": 0.19,
-                "4": 0.25,
-                "5": 0.31,
-                "6": 0.38,
-                "7": 0.44,
-                "8": 0.5
+                "1": 0.2
+            },
+            "distanceByTipCount": {
+                "1": 13.0
             },
-            "distance": 13.0,
             "increment": 0.0,
             "presses": 1,
-            "speed": 10
+            "speedByTipCount": {
+                "1": 10.0
+            }
         }
     },
     "plungerHomingConfigurations": {
         "current": 1.0,
         "speed": 30
     },
     "plungerMotorConfigurations": {
         "idle": 0.3,
         "run": 1.0
     },
     "plungerPositionsConfigurations": {
         "default": {
             "blowout": 76.5,
             "bottom": 71.5,
-            "drop": 92.5,
-            "top": 0.5
+            "drop": 90.5,
+            "top": 0.0
+        },
+        "lowVolumeDefault": {
+            "blowout": 76.5,
+            "bottom": 61.5,
+            "drop": 90.5,
+            "top": 0.0
         }
     },
     "quirks": [],
-    "shaftDiameter": 4.5,
-    "shaftULperMM": 15.904
+    "shaftDiameter": 1.0,
+    "shaftULperMM": 0.785
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p1000/3_3.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p50/3_6.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8049501050420167%*

 * *Differences: {"'availableSensors'": "{'pressure': {'count': 1}, 'capacitive': {'count': 1}}",*

 * * "'channels'": '1',*

 * * "'displayName'": "'Flex 1-Channel 50 μL'",*

 * * "'dropTipConfigurations'": "{'plungerEject': {'speed': 15}}",*

 * * "'model'": "'p50'",*

 * * "'partialTipConfigurations'": "{'partialTipSupported': False, 'availableConfigurations': None}",*

 * * "'pickUpTipConfigurations'": "{'pressFit': {'currentByTipCount': {'1': 0.2, delete: ['2', '3', "*

 * *                              "'4', '5', '6', '7', '8']}, 'speedByTipCount': OrderedDic […]*

```diff
@@ -1,81 +1,75 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipettePropertiesSchema.json",
     "availableSensors": {
         "capacitive": {
-            "count": 2
+            "count": 1
         },
         "environment": {
             "count": 1
         },
         "pressure": {
-            "count": 2
+            "count": 1
         },
         "sensors": [
             "pressure",
             "capacitive",
             "environment"
         ]
     },
     "backCompatNames": [],
     "backlashDistance": 0.1,
-    "channels": 8,
+    "channels": 1,
     "displayCategory": "FLEX",
-    "displayName": "Flex 8-Channel 1000 \u03bcL",
+    "displayName": "Flex 1-Channel 50 \u03bcL",
     "dropTipConfigurations": {
         "plungerEject": {
             "current": 1.0,
-            "speed": 10
+            "speed": 15
         }
     },
-    "model": "p1000",
+    "model": "p50",
     "partialTipConfigurations": {
-        "availableConfigurations": [
-            1,
-            2,
-            3,
-            4,
-            5,
-            6,
-            7,
-            8
-        ],
-        "partialTipSupported": true
+        "availableConfigurations": null,
+        "partialTipSupported": false
     },
     "pickUpTipConfigurations": {
         "pressFit": {
             "currentByTipCount": {
-                "1": 0.15,
-                "2": 0.13,
-                "3": 0.19,
-                "4": 0.25,
-                "5": 0.31,
-                "6": 0.38,
-                "7": 0.44,
-                "8": 0.5
+                "1": 0.2
+            },
+            "distanceByTipCount": {
+                "1": 13.0
             },
-            "distance": 13.0,
             "increment": 0.0,
             "presses": 1,
-            "speed": 10
+            "speedByTipCount": {
+                "1": 10.0
+            }
         }
     },
     "plungerHomingConfigurations": {
         "current": 1.0,
         "speed": 30
     },
     "plungerMotorConfigurations": {
         "idle": 0.3,
         "run": 1.0
     },
     "plungerPositionsConfigurations": {
         "default": {
             "blowout": 76.5,
             "bottom": 71.5,
-            "drop": 92.5,
-            "top": 0.5
+            "drop": 90.5,
+            "top": 0.0
+        },
+        "lowVolumeDefault": {
+            "blowout": 76.5,
+            "bottom": 61.5,
+            "drop": 90.5,
+            "top": 0.0
         }
     },
     "quirks": [],
-    "shaftDiameter": 4.5,
-    "shaftULperMM": 15.904
+    "shaftDiameter": 1.0,
+    "shaftULperMM": 0.785
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p1000/3_4.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p1000/3_3.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9097295168067226%*

 * *Differences: {"'availableSensors'": "{'pressure': {'count': 1}, 'capacitive': {'count': 1}}",*

 * * "'channels'": '1',*

 * * "'displayName'": "'Flex 1-Channel 1000 μL'",*

 * * "'partialTipConfigurations'": "{'partialTipSupported': False, 'availableConfigurations': None}",*

 * * "'pickUpTipConfigurations'": "{'pressFit': {'currentByTipCount': {'1': 0.15, delete: ['2', '3', "*

 * *                              "'4', '5', '6', '7', '8']}, 'speedByTipCount': OrderedDict([('1', "*

 * *                              "5.0)]), 'distanceByTipCount': OrderedDi […]*

```diff
@@ -1,81 +1,69 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipettePropertiesSchema.json",
     "availableSensors": {
         "capacitive": {
-            "count": 2
+            "count": 1
         },
         "environment": {
             "count": 1
         },
         "pressure": {
-            "count": 2
+            "count": 1
         },
         "sensors": [
             "pressure",
             "capacitive",
             "environment"
         ]
     },
     "backCompatNames": [],
     "backlashDistance": 0.1,
-    "channels": 8,
+    "channels": 1,
     "displayCategory": "FLEX",
-    "displayName": "Flex 8-Channel 1000 \u03bcL",
+    "displayName": "Flex 1-Channel 1000 \u03bcL",
     "dropTipConfigurations": {
         "plungerEject": {
             "current": 1.0,
             "speed": 10
         }
     },
     "model": "p1000",
     "partialTipConfigurations": {
-        "availableConfigurations": [
-            1,
-            2,
-            3,
-            4,
-            5,
-            6,
-            7,
-            8
-        ],
-        "partialTipSupported": true
+        "availableConfigurations": null,
+        "partialTipSupported": false
     },
     "pickUpTipConfigurations": {
         "pressFit": {
             "currentByTipCount": {
-                "1": 0.2,
-                "2": 0.14,
-                "3": 0.21,
-                "4": 0.28,
-                "5": 0.34,
-                "6": 0.41,
-                "7": 0.48,
-                "8": 0.55
+                "1": 0.15
+            },
+            "distanceByTipCount": {
+                "1": 13.0
             },
-            "distance": 13.0,
             "increment": 0.0,
             "presses": 1,
-            "speed": 10
+            "speedByTipCount": {
+                "1": 5.0
+            }
         }
     },
     "plungerHomingConfigurations": {
         "current": 1.0,
         "speed": 30
     },
     "plungerMotorConfigurations": {
         "idle": 0.3,
         "run": 1.0
     },
     "plungerPositionsConfigurations": {
         "default": {
             "blowout": 76.5,
             "bottom": 71.5,
-            "drop": 91.5,
-            "top": 0.0
+            "drop": 90.5,
+            "top": 0.5
         }
     },
     "quirks": [],
     "shaftDiameter": 4.5,
     "shaftULperMM": 15.904
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p1000/3_5.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p1000/3_4.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9079569327731093%*

 * *Differences: {"'availableSensors'": "{'pressure': {'count': 1}, 'capacitive': {'count': 1}}",*

 * * "'channels'": '1',*

 * * "'displayName'": "'Flex 1-Channel 1000 μL'",*

 * * "'dropTipConfigurations'": "{'plungerEject': {'speed': 15}}",*

 * * "'partialTipConfigurations'": "{'partialTipSupported': False, 'availableConfigurations': None}",*

 * * "'pickUpTipConfigurations'": "{'pressFit': {'currentByTipCount': {delete: ['2', '3', '4', '5', "*

 * *                              "'6', '7', '8']}, 'speedByTipCount': OrderedDict([('1', 10.0)]), "*

 * *          […]*

```diff
@@ -1,81 +1,69 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipettePropertiesSchema.json",
     "availableSensors": {
         "capacitive": {
-            "count": 2
+            "count": 1
         },
         "environment": {
             "count": 1
         },
         "pressure": {
-            "count": 2
+            "count": 1
         },
         "sensors": [
             "pressure",
             "capacitive",
             "environment"
         ]
     },
     "backCompatNames": [],
     "backlashDistance": 0.1,
-    "channels": 8,
+    "channels": 1,
     "displayCategory": "FLEX",
-    "displayName": "Flex 8-Channel 1000 \u03bcL",
+    "displayName": "Flex 1-Channel 1000 \u03bcL",
     "dropTipConfigurations": {
         "plungerEject": {
             "current": 1.0,
-            "speed": 10
+            "speed": 15
         }
     },
     "model": "p1000",
     "partialTipConfigurations": {
-        "availableConfigurations": [
-            1,
-            2,
-            3,
-            4,
-            5,
-            6,
-            7,
-            8
-        ],
-        "partialTipSupported": true
+        "availableConfigurations": null,
+        "partialTipSupported": false
     },
     "pickUpTipConfigurations": {
         "pressFit": {
             "currentByTipCount": {
-                "1": 0.2,
-                "2": 0.14,
-                "3": 0.21,
-                "4": 0.28,
-                "5": 0.34,
-                "6": 0.41,
-                "7": 0.48,
-                "8": 0.55
+                "1": 0.2
+            },
+            "distanceByTipCount": {
+                "1": 13.0
             },
-            "distance": 13.0,
             "increment": 0.0,
             "presses": 1,
-            "speed": 10
+            "speedByTipCount": {
+                "1": 10.0
+            }
         }
     },
     "plungerHomingConfigurations": {
         "current": 1.0,
         "speed": 30
     },
     "plungerMotorConfigurations": {
         "idle": 0.3,
         "run": 1.0
     },
     "plungerPositionsConfigurations": {
         "default": {
             "blowout": 76.5,
             "bottom": 71.5,
-            "drop": 91.5,
+            "drop": 90.5,
             "top": 0.0
         }
     },
     "quirks": [],
     "shaftDiameter": 4.5,
     "shaftULperMM": 15.904
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p20/2_0.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p300/1_4.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7036502100840336%*

 * *Differences: {"'backCompatNames'": '[]',*

 * * "'channels'": '1',*

 * * "'displayCategory'": "'GEN1'",*

 * * "'displayName'": "'P300 Single-Channel GEN1'",*

 * * "'dropTipConfigurations'": "{'plungerEject': {'current': 0.5, 'speed': 5.0}}",*

 * * "'model'": "'p300'",*

 * * "'partialTipConfigurations'": "{'partialTipSupported': False, 'availableConfigurations': None}",*

 * * "'pickUpTipConfigurations'": "{'pressFit': {'presses': 3, 'increment': 1.0, 'currentByTipCount': "*

 * *                              "{delete: ['2', '3', '4', '5', '6', '7', '8']}, 'speed […]*

```diff
@@ -1,70 +1,58 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipettePropertiesSchema.json",
     "availableSensors": {
         "sensors": []
     },
-    "backCompatNames": [
-        "p10_multi"
-    ],
+    "backCompatNames": [],
     "backlashDistance": 0.0,
-    "channels": 8,
-    "displayCategory": "GEN2",
-    "displayName": "P20 8-Channel GEN2",
+    "channels": 1,
+    "displayCategory": "GEN1",
+    "displayName": "P300 Single-Channel GEN1",
     "dropTipConfigurations": {
         "plungerEject": {
-            "current": 1.25,
-            "speed": 15.0
+            "current": 0.5,
+            "speed": 5.0
         }
     },
-    "model": "p20",
+    "model": "p300",
     "partialTipConfigurations": {
-        "availableConfigurations": [
-            1,
-            2,
-            3,
-            4,
-            5,
-            6,
-            7,
-            8
-        ],
-        "partialTipSupported": true
+        "availableConfigurations": null,
+        "partialTipSupported": false
     },
     "pickUpTipConfigurations": {
         "pressFit": {
             "currentByTipCount": {
-                "1": 0.1,
-                "2": 0.15,
-                "3": 0.23,
-                "4": 0.28,
-                "5": 0.38,
-                "6": 0.45,
-                "7": 0.53,
-                "8": 0.6
+                "1": 0.1
+            },
+            "distanceByTipCount": {
+                "1": 10.0
             },
-            "distance": 11.0,
-            "increment": 0.0,
-            "presses": 1,
-            "speed": 10.0
+            "increment": 1.0,
+            "presses": 3,
+            "speedByTipCount": {
+                "1": 30.0
+            }
         }
     },
     "plungerHomingConfigurations": {
-        "current": 1.0,
+        "current": 0.3,
         "speed": 30
     },
     "plungerMotorConfigurations": {
-        "idle": 0.3,
-        "run": 1.0
+        "idle": 0.05,
+        "run": 0.3
     },
     "plungerPositionsConfigurations": {
         "default": {
-            "blowout": -13.0,
-            "bottom": -8.5,
-            "drop": -31.6,
+            "blowout": 0.0,
+            "bottom": 3.0,
+            "drop": -4.5,
             "top": 19.5
         }
     },
-    "quirks": [],
-    "shaftDiameter": 1.0,
-    "shaftULperMM": 0.785
+    "quirks": [
+        "dropTipShake"
+    ],
+    "shaftDiameter": 5.0,
+    "shaftULperMM": 19.635
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p20/2_1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p300/1_5.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7036502100840336%*

 * *Differences: {"'backCompatNames'": '[]',*

 * * "'channels'": '1',*

 * * "'displayCategory'": "'GEN1'",*

 * * "'displayName'": "'P300 Single-Channel GEN1'",*

 * * "'dropTipConfigurations'": "{'plungerEject': {'current': 0.5, 'speed': 5.0}}",*

 * * "'model'": "'p300'",*

 * * "'partialTipConfigurations'": "{'partialTipSupported': False, 'availableConfigurations': None}",*

 * * "'pickUpTipConfigurations'": "{'pressFit': {'presses': 3, 'increment': 1.0, 'currentByTipCount': "*

 * *                              "{delete: ['2', '3', '4', '5', '6', '7', '8']}, 'speed […]*

```diff
@@ -1,70 +1,58 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipettePropertiesSchema.json",
     "availableSensors": {
         "sensors": []
     },
-    "backCompatNames": [
-        "p10_multi"
-    ],
+    "backCompatNames": [],
     "backlashDistance": 0.0,
-    "channels": 8,
-    "displayCategory": "GEN2",
-    "displayName": "P20 8-Channel GEN2",
+    "channels": 1,
+    "displayCategory": "GEN1",
+    "displayName": "P300 Single-Channel GEN1",
     "dropTipConfigurations": {
         "plungerEject": {
-            "current": 1.25,
-            "speed": 15.0
+            "current": 0.5,
+            "speed": 5.0
         }
     },
-    "model": "p20",
+    "model": "p300",
     "partialTipConfigurations": {
-        "availableConfigurations": [
-            1,
-            2,
-            3,
-            4,
-            5,
-            6,
-            7,
-            8
-        ],
-        "partialTipSupported": true
+        "availableConfigurations": null,
+        "partialTipSupported": false
     },
     "pickUpTipConfigurations": {
         "pressFit": {
             "currentByTipCount": {
-                "1": 0.1,
-                "2": 0.15,
-                "3": 0.23,
-                "4": 0.28,
-                "5": 0.38,
-                "6": 0.45,
-                "7": 0.53,
-                "8": 0.6
+                "1": 0.1
+            },
+            "distanceByTipCount": {
+                "1": 10.0
             },
-            "distance": 11.0,
-            "increment": 0.0,
-            "presses": 1,
-            "speed": 10.0
+            "increment": 1.0,
+            "presses": 3,
+            "speedByTipCount": {
+                "1": 30.0
+            }
         }
     },
     "plungerHomingConfigurations": {
-        "current": 1.0,
+        "current": 0.3,
         "speed": 30
     },
     "plungerMotorConfigurations": {
-        "idle": 0.3,
-        "run": 1.0
+        "idle": 0.05,
+        "run": 0.3
     },
     "plungerPositionsConfigurations": {
         "default": {
-            "blowout": -13.0,
-            "bottom": -8.5,
-            "drop": -31.6,
+            "blowout": 0.0,
+            "bottom": 3.0,
+            "drop": -4.5,
             "top": 19.5
         }
     },
-    "quirks": [],
-    "shaftDiameter": 1.0,
-    "shaftULperMM": 0.785
+    "quirks": [
+        "dropTipShake"
+    ],
+    "shaftDiameter": 5.0,
+    "shaftULperMM": 19.635
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p300/1_0.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p50/1_4.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8086922268907564%*

 * *Differences: {"'channels'": '1',*

 * * "'displayName'": "'P50 Single-Channel GEN1'",*

 * * "'model'": "'p50'",*

 * * "'partialTipConfigurations'": "{'partialTipSupported': False, 'availableConfigurations': None}",*

 * * "'pickUpTipConfigurations'": "{'pressFit': {'currentByTipCount': {delete: ['2', '3', '4', '5', "*

 * *                              "'6', '7', '8']}, 'speedByTipCount': OrderedDict([('1', 30.0)]), "*

 * *                              "'distanceByTipCount': OrderedDict([('1', 10.0)]), delete: ['speed', "*

 * *                               […]*

```diff
@@ -1,70 +1,58 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipettePropertiesSchema.json",
     "availableSensors": {
         "sensors": []
     },
     "backCompatNames": [],
     "backlashDistance": 0.0,
-    "channels": 8,
+    "channels": 1,
     "displayCategory": "GEN1",
-    "displayName": "P300 8-Channel GEN1",
+    "displayName": "P50 Single-Channel GEN1",
     "dropTipConfigurations": {
         "plungerEject": {
             "current": 0.5,
             "speed": 5.0
         }
     },
-    "model": "p300",
+    "model": "p50",
     "partialTipConfigurations": {
-        "availableConfigurations": [
-            1,
-            2,
-            3,
-            4,
-            5,
-            6,
-            7,
-            8
-        ],
-        "partialTipSupported": true
+        "availableConfigurations": null,
+        "partialTipSupported": false
     },
     "pickUpTipConfigurations": {
         "pressFit": {
             "currentByTipCount": {
-                "1": 0.1,
-                "2": 0.15,
-                "3": 0.23,
-                "4": 0.3,
-                "5": 0.38,
-                "6": 0.45,
-                "7": 0.53,
-                "8": 0.6
+                "1": 0.1
+            },
+            "distanceByTipCount": {
+                "1": 10.0
             },
-            "distance": 10.0,
             "increment": 1.0,
             "presses": 3,
-            "speed": 30.0
+            "speedByTipCount": {
+                "1": 30.0
+            }
         }
     },
     "plungerHomingConfigurations": {
-        "current": 0.5,
+        "current": 0.3,
         "speed": 30
     },
     "plungerMotorConfigurations": {
         "idle": 0.05,
-        "run": 0.5
+        "run": 0.3
     },
     "plungerPositionsConfigurations": {
         "default": {
-            "blowout": 3.0,
-            "bottom": 3.5,
-            "drop": -2.0,
+            "blowout": 0.5,
+            "bottom": 2.0,
+            "drop": -5.0,
             "top": 19.5
         }
     },
     "quirks": [
         "dropTipShake"
     ],
-    "shaftDiameter": 5.0,
-    "shaftULperMM": 19.635
+    "shaftDiameter": 2.0,
+    "shaftULperMM": 3.142
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p300/1_3.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p50/1_5.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8086922268907564%*

 * *Differences: {"'channels'": '1',*

 * * "'displayName'": "'P50 Single-Channel GEN1'",*

 * * "'model'": "'p50'",*

 * * "'partialTipConfigurations'": "{'partialTipSupported': False, 'availableConfigurations': None}",*

 * * "'pickUpTipConfigurations'": "{'pressFit': {'currentByTipCount': {delete: ['2', '3', '4', '5', "*

 * *                              "'6', '7', '8']}, 'speedByTipCount': OrderedDict([('1', 30.0)]), "*

 * *                              "'distanceByTipCount': OrderedDict([('1', 10.0)]), delete: ['speed', "*

 * *                               […]*

```diff
@@ -1,70 +1,58 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipettePropertiesSchema.json",
     "availableSensors": {
         "sensors": []
     },
     "backCompatNames": [],
     "backlashDistance": 0.0,
-    "channels": 8,
+    "channels": 1,
     "displayCategory": "GEN1",
-    "displayName": "P300 8-Channel GEN1",
+    "displayName": "P50 Single-Channel GEN1",
     "dropTipConfigurations": {
         "plungerEject": {
             "current": 0.5,
             "speed": 5.0
         }
     },
-    "model": "p300",
+    "model": "p50",
     "partialTipConfigurations": {
-        "availableConfigurations": [
-            1,
-            2,
-            3,
-            4,
-            5,
-            6,
-            7,
-            8
-        ],
-        "partialTipSupported": true
+        "availableConfigurations": null,
+        "partialTipSupported": false
     },
     "pickUpTipConfigurations": {
         "pressFit": {
             "currentByTipCount": {
-                "1": 0.1,
-                "2": 0.15,
-                "3": 0.23,
-                "4": 0.3,
-                "5": 0.38,
-                "6": 0.45,
-                "7": 0.53,
-                "8": 0.6
+                "1": 0.1
+            },
+            "distanceByTipCount": {
+                "1": 10.0
             },
-            "distance": 10.0,
             "increment": 1.0,
             "presses": 3,
-            "speed": 30.0
+            "speedByTipCount": {
+                "1": 30.0
+            }
         }
     },
     "plungerHomingConfigurations": {
-        "current": 0.5,
+        "current": 0.3,
         "speed": 30
     },
     "plungerMotorConfigurations": {
         "idle": 0.05,
-        "run": 0.5
+        "run": 0.3
     },
     "plungerPositionsConfigurations": {
         "default": {
-            "blowout": 1.5,
-            "bottom": 3.5,
-            "drop": -3.5,
+            "blowout": 0.5,
+            "bottom": 2.0,
+            "drop": -5.0,
             "top": 19.5
         }
     },
     "quirks": [
         "dropTipShake"
     ],
-    "shaftDiameter": 5.0,
-    "shaftULperMM": 19.635
+    "shaftDiameter": 2.0,
+    "shaftULperMM": 3.142
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p300/1_4.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p50/1_0.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8086922268907564%*

 * *Differences: {"'channels'": '1',*

 * * "'displayName'": "'P50 Single-Channel GEN1'",*

 * * "'model'": "'p50'",*

 * * "'partialTipConfigurations'": "{'partialTipSupported': False, 'availableConfigurations': None}",*

 * * "'pickUpTipConfigurations'": "{'pressFit': {'currentByTipCount': {delete: ['2', '3', '4', '5', "*

 * *                              "'6', '7', '8']}, 'speedByTipCount': OrderedDict([('1', 30.0)]), "*

 * *                              "'distanceByTipCount': OrderedDict([('1', 10.0)]), delete: ['speed', "*

 * *                               […]*

```diff
@@ -1,70 +1,58 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipettePropertiesSchema.json",
     "availableSensors": {
         "sensors": []
     },
     "backCompatNames": [],
     "backlashDistance": 0.0,
-    "channels": 8,
+    "channels": 1,
     "displayCategory": "GEN1",
-    "displayName": "P300 8-Channel GEN1",
+    "displayName": "P50 Single-Channel GEN1",
     "dropTipConfigurations": {
         "plungerEject": {
             "current": 0.5,
             "speed": 5.0
         }
     },
-    "model": "p300",
+    "model": "p50",
     "partialTipConfigurations": {
-        "availableConfigurations": [
-            1,
-            2,
-            3,
-            4,
-            5,
-            6,
-            7,
-            8
-        ],
-        "partialTipSupported": true
+        "availableConfigurations": null,
+        "partialTipSupported": false
     },
     "pickUpTipConfigurations": {
         "pressFit": {
             "currentByTipCount": {
-                "1": 0.1,
-                "2": 0.15,
-                "3": 0.23,
-                "4": 0.3,
-                "5": 0.38,
-                "6": 0.45,
-                "7": 0.53,
-                "8": 0.6
+                "1": 0.1
+            },
+            "distanceByTipCount": {
+                "1": 10.0
             },
-            "distance": 10.0,
             "increment": 1.0,
             "presses": 3,
-            "speed": 30.0
+            "speedByTipCount": {
+                "1": 30.0
+            }
         }
     },
     "plungerHomingConfigurations": {
-        "current": 0.5,
+        "current": 0.3,
         "speed": 30
     },
     "plungerMotorConfigurations": {
         "idle": 0.05,
-        "run": 0.5
+        "run": 0.3
     },
     "plungerPositionsConfigurations": {
         "default": {
-            "blowout": 1.5,
-            "bottom": 3.5,
-            "drop": -3.5,
+            "blowout": 2.0,
+            "bottom": 2.01,
+            "drop": -4.5,
             "top": 19.5
         }
     },
     "quirks": [
         "dropTipShake"
     ],
-    "shaftDiameter": 5.0,
-    "shaftULperMM": 19.635
+    "shaftDiameter": 2.0,
+    "shaftULperMM": 3.142
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p300/1_5.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p300/2_0.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7403492647058824%*

 * *Differences: {"'backCompatNames'": "['p300_single']",*

 * * "'channels'": '1',*

 * * "'displayCategory'": "'GEN2'",*

 * * "'displayName'": "'P300 Single-Channel GEN2'",*

 * * "'dropTipConfigurations'": "{'plungerEject': {'current': 1.25, 'speed': 7.0}}",*

 * * "'partialTipConfigurations'": "{'partialTipSupported': False, 'availableConfigurations': None}",*

 * * "'pickUpTipConfigurations'": "{'pressFit': {'presses': 1, 'increment': 0.0, 'currentByTipCount': "*

 * *                              "{'1': 0.125, delete: ['2', '3', '4', '5', '6', '7', '8']}, "*

 * * […]*

```diff
@@ -1,71 +1,58 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipettePropertiesSchema.json",
     "availableSensors": {
         "sensors": []
     },
-    "backCompatNames": [],
+    "backCompatNames": [
+        "p300_single"
+    ],
     "backlashDistance": 0.0,
-    "channels": 8,
-    "displayCategory": "GEN1",
-    "displayName": "P300 8-Channel GEN1",
+    "channels": 1,
+    "displayCategory": "GEN2",
+    "displayName": "P300 Single-Channel GEN2",
     "dropTipConfigurations": {
         "plungerEject": {
-            "current": 0.5,
-            "speed": 5.0
+            "current": 1.25,
+            "speed": 7.0
         }
     },
     "model": "p300",
     "partialTipConfigurations": {
-        "availableConfigurations": [
-            1,
-            2,
-            3,
-            4,
-            5,
-            6,
-            7,
-            8
-        ],
-        "partialTipSupported": true
+        "availableConfigurations": null,
+        "partialTipSupported": false
     },
     "pickUpTipConfigurations": {
         "pressFit": {
             "currentByTipCount": {
-                "1": 0.1,
-                "2": 0.23,
-                "3": 0.34,
-                "4": 0.45,
-                "5": 0.56,
-                "6": 0.68,
-                "7": 0.79,
-                "8": 0.9
+                "1": 0.125
+            },
+            "distanceByTipCount": {
+                "1": 17.0
             },
-            "distance": 10.0,
-            "increment": 3.0,
-            "presses": 3,
-            "speed": 30.0
+            "increment": 0.0,
+            "presses": 1,
+            "speedByTipCount": {
+                "1": 10.0
+            }
         }
     },
     "plungerHomingConfigurations": {
-        "current": 0.5,
+        "current": 1.0,
         "speed": 30
     },
     "plungerMotorConfigurations": {
         "idle": 0.05,
-        "run": 0.5
+        "run": 1.0
     },
     "plungerPositionsConfigurations": {
         "default": {
-            "blowout": 1.5,
-            "bottom": 3.5,
-            "drop": -3.5,
+            "blowout": -19.0,
+            "bottom": -14.5,
+            "drop": -37.0,
             "top": 19.5
         }
     },
-    "quirks": [
-        "dropTipShake",
-        "doubleDropTip"
-    ],
-    "shaftDiameter": 5.0,
-    "shaftULperMM": 19.635
+    "quirks": [],
+    "shaftDiameter": 3.5,
+    "shaftULperMM": 9.621
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p300/2_0.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p300/1_0.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7329963235294118%*

 * *Differences: {"'backCompatNames'": '[]',*

 * * "'channels'": '1',*

 * * "'displayCategory'": "'GEN1'",*

 * * "'displayName'": "'P300 Single-Channel GEN1'",*

 * * "'dropTipConfigurations'": "{'plungerEject': {'current': 0.5, 'speed': 5.0}}",*

 * * "'partialTipConfigurations'": "{'partialTipSupported': False, 'availableConfigurations': None}",*

 * * "'pickUpTipConfigurations'": "{'pressFit': {'presses': 3, 'increment': 1.0, 'currentByTipCount': "*

 * *                              "{'1': 0.1, delete: ['2', '3', '4', '5', '6', '7', '8']}, "*

 * *                 […]*

```diff
@@ -1,72 +1,58 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipettePropertiesSchema.json",
     "availableSensors": {
         "sensors": []
     },
-    "backCompatNames": [
-        "p300_multi"
-    ],
+    "backCompatNames": [],
     "backlashDistance": 0.0,
-    "channels": 8,
-    "displayCategory": "GEN2",
-    "displayName": "P300 8-Channel GEN2",
+    "channels": 1,
+    "displayCategory": "GEN1",
+    "displayName": "P300 Single-Channel GEN1",
     "dropTipConfigurations": {
         "plungerEject": {
-            "current": 1.25,
-            "speed": 7.5
+            "current": 0.5,
+            "speed": 5.0
         }
     },
     "model": "p300",
     "partialTipConfigurations": {
-        "availableConfigurations": [
-            1,
-            2,
-            3,
-            4,
-            5,
-            6,
-            7,
-            8
-        ],
-        "partialTipSupported": true
+        "availableConfigurations": null,
+        "partialTipSupported": false
     },
     "pickUpTipConfigurations": {
         "pressFit": {
             "currentByTipCount": {
-                "1": 0.13,
-                "2": 0.2,
-                "3": 0.3,
-                "4": 0.4,
-                "5": 0.5,
-                "6": 0.6,
-                "7": 0.7,
-                "8": 0.8
+                "1": 0.1
+            },
+            "distanceByTipCount": {
+                "1": 10.0
             },
-            "distance": 11.0,
-            "increment": 0.0,
-            "presses": 1,
-            "speed": 10.0
+            "increment": 1.0,
+            "presses": 3,
+            "speedByTipCount": {
+                "1": 30.0
+            }
         }
     },
     "plungerHomingConfigurations": {
-        "current": 1.0,
+        "current": 0.3,
         "speed": 30
     },
     "plungerMotorConfigurations": {
-        "idle": 0.3,
-        "run": 1.0
+        "idle": 0.05,
+        "run": 0.3
     },
     "plungerPositionsConfigurations": {
         "default": {
-            "blowout": -19.0,
-            "bottom": -14.5,
-            "drop": -33.4,
+            "blowout": 0.0,
+            "bottom": 1.5,
+            "drop": -4.0,
             "top": 19.5
         }
     },
     "quirks": [
-        "needsUnstick"
+        "dropTipShake"
     ],
-    "shaftDiameter": 3.5,
-    "shaftULperMM": 9.621
+    "shaftDiameter": 5.0,
+    "shaftULperMM": 19.635
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p300/2_1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p300/1_3.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7329963235294118%*

 * *Differences: {"'backCompatNames'": '[]',*

 * * "'channels'": '1',*

 * * "'displayCategory'": "'GEN1'",*

 * * "'displayName'": "'P300 Single-Channel GEN1'",*

 * * "'dropTipConfigurations'": "{'plungerEject': {'current': 0.5, 'speed': 5.0}}",*

 * * "'partialTipConfigurations'": "{'partialTipSupported': False, 'availableConfigurations': None}",*

 * * "'pickUpTipConfigurations'": "{'pressFit': {'presses': 3, 'increment': 1.0, 'currentByTipCount': "*

 * *                              "{'1': 0.1, delete: ['2', '3', '4', '5', '6', '7', '8']}, "*

 * *                 […]*

```diff
@@ -1,72 +1,58 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipettePropertiesSchema.json",
     "availableSensors": {
         "sensors": []
     },
-    "backCompatNames": [
-        "p300_multi"
-    ],
+    "backCompatNames": [],
     "backlashDistance": 0.0,
-    "channels": 8,
-    "displayCategory": "GEN2",
-    "displayName": "P300 8-Channel GEN2",
+    "channels": 1,
+    "displayCategory": "GEN1",
+    "displayName": "P300 Single-Channel GEN1",
     "dropTipConfigurations": {
         "plungerEject": {
-            "current": 1.25,
-            "speed": 7.5
+            "current": 0.5,
+            "speed": 5.0
         }
     },
     "model": "p300",
     "partialTipConfigurations": {
-        "availableConfigurations": [
-            1,
-            2,
-            3,
-            4,
-            5,
-            6,
-            7,
-            8
-        ],
-        "partialTipSupported": true
+        "availableConfigurations": null,
+        "partialTipSupported": false
     },
     "pickUpTipConfigurations": {
         "pressFit": {
             "currentByTipCount": {
-                "1": 0.13,
-                "2": 0.2,
-                "3": 0.3,
-                "4": 0.4,
-                "5": 0.5,
-                "6": 0.6,
-                "7": 0.7,
-                "8": 0.8
+                "1": 0.1
+            },
+            "distanceByTipCount": {
+                "1": 10.0
             },
-            "distance": 11.0,
-            "increment": 0.0,
-            "presses": 1,
-            "speed": 10.0
+            "increment": 1.0,
+            "presses": 3,
+            "speedByTipCount": {
+                "1": 30.0
+            }
         }
     },
     "plungerHomingConfigurations": {
-        "current": 1.0,
+        "current": 0.3,
         "speed": 30
     },
     "plungerMotorConfigurations": {
-        "idle": 0.3,
-        "run": 1.0
+        "idle": 0.05,
+        "run": 0.3
     },
     "plungerPositionsConfigurations": {
         "default": {
-            "blowout": -19.0,
-            "bottom": -14.5,
-            "drop": -33.4,
+            "blowout": -1.5,
+            "bottom": 1.5,
+            "drop": -5.5,
             "top": 19.5
         }
     },
     "quirks": [
-        "needsUnstick"
+        "dropTipShake"
     ],
-    "shaftDiameter": 3.5,
-    "shaftULperMM": 9.621
+    "shaftDiameter": 5.0,
+    "shaftULperMM": 19.635
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p50/1_0.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p1000/1_3.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8068539915966387%*

 * *Differences: {"'channels'": '1',*

 * * "'displayName'": "'P1000 Single-Channel GEN1'",*

 * * "'dropTipConfigurations'": "{'plungerEject': {'current': 0.7}}",*

 * * "'model'": "'p1000'",*

 * * "'partialTipConfigurations'": "{'partialTipSupported': False, 'availableConfigurations': None}",*

 * * "'pickUpTipConfigurations'": "{'pressFit': {'currentByTipCount': {delete: ['2', '3', '4', '5', "*

 * *                              "'6', '7', '8']}, 'speedByTipCount': OrderedDict([('1', 30.0)]), "*

 * *                              "'distanceByTipCount': OrderedD […]*

```diff
@@ -1,70 +1,59 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipettePropertiesSchema.json",
     "availableSensors": {
         "sensors": []
     },
     "backCompatNames": [],
     "backlashDistance": 0.0,
-    "channels": 8,
+    "channels": 1,
     "displayCategory": "GEN1",
-    "displayName": "P50 8-Channel GEN1",
+    "displayName": "P1000 Single-Channel GEN1",
     "dropTipConfigurations": {
         "plungerEject": {
-            "current": 0.5,
+            "current": 0.7,
             "speed": 5.0
         }
     },
-    "model": "p50",
+    "model": "p1000",
     "partialTipConfigurations": {
-        "availableConfigurations": [
-            1,
-            2,
-            3,
-            4,
-            5,
-            6,
-            7,
-            8
-        ],
-        "partialTipSupported": true
+        "availableConfigurations": null,
+        "partialTipSupported": false
     },
     "pickUpTipConfigurations": {
         "pressFit": {
             "currentByTipCount": {
-                "1": 0.1,
-                "2": 0.15,
-                "3": 0.23,
-                "4": 0.3,
-                "5": 0.38,
-                "6": 0.45,
-                "7": 0.53,
-                "8": 0.6
+                "1": 0.1
+            },
+            "distanceByTipCount": {
+                "1": 15.0
             },
-            "distance": 10.0,
             "increment": 1.0,
             "presses": 3,
-            "speed": 30.0
+            "speedByTipCount": {
+                "1": 30.0
+            }
         }
     },
     "plungerHomingConfigurations": {
         "current": 0.5,
         "speed": 30
     },
     "plungerMotorConfigurations": {
         "idle": 0.05,
         "run": 0.5
     },
     "plungerPositionsConfigurations": {
         "default": {
-            "blowout": 2.0,
+            "blowout": 0.5,
             "bottom": 2.5,
-            "drop": -3.5,
+            "drop": -4.0,
             "top": 19.5
         }
     },
     "quirks": [
+        "pickupTipShake",
         "dropTipShake"
     ],
-    "shaftDiameter": 2.0,
-    "shaftULperMM": 3.142
+    "shaftDiameter": 9.0,
+    "shaftULperMM": 63.617
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p50/1_3.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p1000/1_4.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8068539915966387%*

 * *Differences: {"'channels'": '1',*

 * * "'displayName'": "'P1000 Single-Channel GEN1'",*

 * * "'dropTipConfigurations'": "{'plungerEject': {'current': 0.7}}",*

 * * "'model'": "'p1000'",*

 * * "'partialTipConfigurations'": "{'partialTipSupported': False, 'availableConfigurations': None}",*

 * * "'pickUpTipConfigurations'": "{'pressFit': {'currentByTipCount': {delete: ['2', '3', '4', '5', "*

 * *                              "'6', '7', '8']}, 'speedByTipCount': OrderedDict([('1', 30.0)]), "*

 * *                              "'distanceByTipCount': OrderedD […]*

```diff
@@ -1,70 +1,59 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipettePropertiesSchema.json",
     "availableSensors": {
         "sensors": []
     },
     "backCompatNames": [],
     "backlashDistance": 0.0,
-    "channels": 8,
+    "channels": 1,
     "displayCategory": "GEN1",
-    "displayName": "P50 8-Channel GEN1",
+    "displayName": "P1000 Single-Channel GEN1",
     "dropTipConfigurations": {
         "plungerEject": {
-            "current": 0.5,
+            "current": 0.7,
             "speed": 5.0
         }
     },
-    "model": "p50",
+    "model": "p1000",
     "partialTipConfigurations": {
-        "availableConfigurations": [
-            1,
-            2,
-            3,
-            4,
-            5,
-            6,
-            7,
-            8
-        ],
-        "partialTipSupported": true
+        "availableConfigurations": null,
+        "partialTipSupported": false
     },
     "pickUpTipConfigurations": {
         "pressFit": {
             "currentByTipCount": {
-                "1": 0.1,
-                "2": 0.15,
-                "3": 0.23,
-                "4": 0.3,
-                "5": 0.38,
-                "6": 0.45,
-                "7": 0.53,
-                "8": 0.6
+                "1": 0.1
+            },
+            "distanceByTipCount": {
+                "1": 15.0
             },
-            "distance": 10.0,
             "increment": 1.0,
             "presses": 3,
-            "speed": 30.0
+            "speedByTipCount": {
+                "1": 30.0
+            }
         }
     },
     "plungerHomingConfigurations": {
         "current": 0.5,
         "speed": 30
     },
     "plungerMotorConfigurations": {
         "idle": 0.05,
         "run": 0.5
     },
     "plungerPositionsConfigurations": {
         "default": {
             "blowout": 0.5,
-            "bottom": 2.0,
-            "drop": -5.0,
+            "bottom": 2.5,
+            "drop": -4.0,
             "top": 19.5
         }
     },
     "quirks": [
+        "pickupTipShake",
         "dropTipShake"
     ],
-    "shaftDiameter": 2.0,
-    "shaftULperMM": 3.142
+    "shaftDiameter": 9.0,
+    "shaftULperMM": 63.617
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p50/1_4.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p50/1_3.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9006039915966387%*

 * *Differences: {"'channels'": '1',*

 * * "'displayName'": "'P50 Single-Channel GEN1'",*

 * * "'partialTipConfigurations'": "{'partialTipSupported': False, 'availableConfigurations': None}",*

 * * "'pickUpTipConfigurations'": "{'pressFit': {'currentByTipCount': {delete: ['2', '3', '4', '5', "*

 * *                              "'6', '7', '8']}, 'speedByTipCount': OrderedDict([('1', 30.0)]), "*

 * *                              "'distanceByTipCount': OrderedDict([('1', 10.0)]), delete: ['speed', "*

 * *                              "'distance']}}",*

 * * "'p […]*

```diff
@@ -1,68 +1,56 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipettePropertiesSchema.json",
     "availableSensors": {
         "sensors": []
     },
     "backCompatNames": [],
     "backlashDistance": 0.0,
-    "channels": 8,
+    "channels": 1,
     "displayCategory": "GEN1",
-    "displayName": "P50 8-Channel GEN1",
+    "displayName": "P50 Single-Channel GEN1",
     "dropTipConfigurations": {
         "plungerEject": {
             "current": 0.5,
             "speed": 5.0
         }
     },
     "model": "p50",
     "partialTipConfigurations": {
-        "availableConfigurations": [
-            1,
-            2,
-            3,
-            4,
-            5,
-            6,
-            7,
-            8
-        ],
-        "partialTipSupported": true
+        "availableConfigurations": null,
+        "partialTipSupported": false
     },
     "pickUpTipConfigurations": {
         "pressFit": {
             "currentByTipCount": {
-                "1": 0.1,
-                "2": 0.15,
-                "3": 0.23,
-                "4": 0.3,
-                "5": 0.38,
-                "6": 0.45,
-                "7": 0.53,
-                "8": 0.6
+                "1": 0.1
+            },
+            "distanceByTipCount": {
+                "1": 10.0
             },
-            "distance": 10.0,
             "increment": 1.0,
             "presses": 3,
-            "speed": 30.0
+            "speedByTipCount": {
+                "1": 30.0
+            }
         }
     },
     "plungerHomingConfigurations": {
-        "current": 0.5,
+        "current": 0.3,
         "speed": 30
     },
     "plungerMotorConfigurations": {
         "idle": 0.05,
-        "run": 0.5
+        "run": 0.3
     },
     "plungerPositionsConfigurations": {
         "default": {
             "blowout": 0.5,
             "bottom": 2.0,
-            "drop": -4.0,
+            "drop": -6.0,
             "top": 19.5
         }
     },
     "quirks": [
         "dropTipShake"
     ],
     "shaftDiameter": 2.0,
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p50/1_5.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p20/2_1.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7036502100840336%*

 * *Differences: {"'backCompatNames'": "['p10_single']",*

 * * "'channels'": '1',*

 * * "'displayCategory'": "'GEN2'",*

 * * "'displayName'": "'P20 Single-Channel GEN2'",*

 * * "'dropTipConfigurations'": "{'plungerEject': {'current': 1.0, 'speed': 15.0}}",*

 * * "'model'": "'p20'",*

 * * "'partialTipConfigurations'": "{'partialTipSupported': False, 'availableConfigurations': None}",*

 * * "'pickUpTipConfigurations'": "{'pressFit': {'presses': 1, 'increment': 0.0, 'currentByTipCount': "*

 * *                              "{delete: ['2', '3', '4', '5', '6', '7', '8 […]*

```diff
@@ -1,71 +1,58 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipettePropertiesSchema.json",
     "availableSensors": {
         "sensors": []
     },
-    "backCompatNames": [],
+    "backCompatNames": [
+        "p10_single"
+    ],
     "backlashDistance": 0.0,
-    "channels": 8,
-    "displayCategory": "GEN1",
-    "displayName": "P50 8-Channel GEN1",
+    "channels": 1,
+    "displayCategory": "GEN2",
+    "displayName": "P20 Single-Channel GEN2",
     "dropTipConfigurations": {
         "plungerEject": {
-            "current": 0.5,
-            "speed": 5.0
+            "current": 1.0,
+            "speed": 15.0
         }
     },
-    "model": "p50",
+    "model": "p20",
     "partialTipConfigurations": {
-        "availableConfigurations": [
-            1,
-            2,
-            3,
-            4,
-            5,
-            6,
-            7,
-            8
-        ],
-        "partialTipSupported": true
+        "availableConfigurations": null,
+        "partialTipSupported": false
     },
     "pickUpTipConfigurations": {
         "pressFit": {
             "currentByTipCount": {
-                "1": 0.1,
-                "2": 0.2,
-                "3": 0.3,
-                "4": 0.4,
-                "5": 0.5,
-                "6": 0.6,
-                "7": 0.7,
-                "8": 0.8
+                "1": 0.1
+            },
+            "distanceByTipCount": {
+                "1": 14.0
             },
-            "distance": 10.0,
-            "increment": 3.0,
-            "presses": 3,
-            "speed": 30.0
+            "increment": 0.0,
+            "presses": 1,
+            "speedByTipCount": {
+                "1": 10.0
+            }
         }
     },
     "plungerHomingConfigurations": {
-        "current": 0.5,
+        "current": 1.0,
         "speed": 30
     },
     "plungerMotorConfigurations": {
-        "idle": 0.05,
-        "run": 0.5
+        "idle": 0.3,
+        "run": 1.0
     },
     "plungerPositionsConfigurations": {
         "default": {
-            "blowout": 0.5,
-            "bottom": 2.0,
-            "drop": -4.0,
+            "blowout": -13.0,
+            "bottom": -8.5,
+            "drop": -27.0,
             "top": 19.5
         }
     },
-    "quirks": [
-        "doubleDropTip",
-        "dropTipShake"
-    ],
-    "shaftDiameter": 2.0,
-    "shaftULperMM": 3.142
+    "quirks": [],
+    "shaftDiameter": 1.0,
+    "shaftULperMM": 0.785
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p50/3_0.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p50/3_0.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9116334033613446%*

 * *Differences: {"'availableSensors'": "{'pressure': {'count': 1}, 'capacitive': {'count': 1}}",*

 * * "'channels'": '1',*

 * * "'displayName'": "'Flex 1-Channel 50 μL'",*

 * * "'partialTipConfigurations'": "{'partialTipSupported': False, 'availableConfigurations': None}",*

 * * "'pickUpTipConfigurations'": "{'pressFit': {'currentByTipCount': {delete: ['2', '3', '4', '5', "*

 * *                              "'6', '7', '8']}, 'speedByTipCount': OrderedDict([('1', 5.0)]), "*

 * *                              "'distanceByTipCount': OrderedDict([('1', 13. […]*

```diff
@@ -1,87 +1,75 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipettePropertiesSchema.json",
     "availableSensors": {
         "capacitive": {
-            "count": 2
+            "count": 1
         },
         "environment": {
             "count": 1
         },
         "pressure": {
-            "count": 2
+            "count": 1
         },
         "sensors": [
             "pressure",
             "capacitive",
             "environment"
         ]
     },
     "backCompatNames": [],
     "backlashDistance": 0.1,
-    "channels": 8,
+    "channels": 1,
     "displayCategory": "FLEX",
-    "displayName": "Flex 8-Channel 50 \u03bcL",
+    "displayName": "Flex 1-Channel 50 \u03bcL",
     "dropTipConfigurations": {
         "plungerEject": {
             "current": 1.0,
             "speed": 10
         }
     },
     "model": "p50",
     "partialTipConfigurations": {
-        "availableConfigurations": [
-            1,
-            2,
-            3,
-            4,
-            5,
-            6,
-            7,
-            8
-        ],
-        "partialTipSupported": true
+        "availableConfigurations": null,
+        "partialTipSupported": false
     },
     "pickUpTipConfigurations": {
         "pressFit": {
             "currentByTipCount": {
-                "1": 0.15,
-                "2": 0.13,
-                "3": 0.19,
-                "4": 0.25,
-                "5": 0.31,
-                "6": 0.38,
-                "7": 0.44,
-                "8": 0.5
+                "1": 0.15
+            },
+            "distanceByTipCount": {
+                "1": 13.0
             },
-            "distance": 13.0,
             "increment": 0.0,
             "presses": 1,
-            "speed": 10
+            "speedByTipCount": {
+                "1": 5.0
+            }
         }
     },
     "plungerHomingConfigurations": {
         "current": 1.0,
         "speed": 30
     },
     "plungerMotorConfigurations": {
         "idle": 0.3,
         "run": 1.0
     },
     "plungerPositionsConfigurations": {
         "default": {
             "blowout": 76.5,
             "bottom": 71.5,
-            "drop": 92.5,
+            "drop": 90.5,
             "top": 0.5
         },
         "lowVolumeDefault": {
             "blowout": 76.5,
             "bottom": 61.5,
-            "drop": 92.5,
+            "drop": 90.5,
             "top": 0.5
         }
     },
     "quirks": [],
     "shaftDiameter": 1.0,
     "shaftULperMM": 0.785
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p50/3_3.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p50/3_3.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9116334033613446%*

 * *Differences: {"'availableSensors'": "{'pressure': {'count': 1}, 'capacitive': {'count': 1}}",*

 * * "'channels'": '1',*

 * * "'displayName'": "'Flex 1-Channel 50 μL'",*

 * * "'partialTipConfigurations'": "{'partialTipSupported': False, 'availableConfigurations': None}",*

 * * "'pickUpTipConfigurations'": "{'pressFit': {'currentByTipCount': {delete: ['2', '3', '4', '5', "*

 * *                              "'6', '7', '8']}, 'speedByTipCount': OrderedDict([('1', 5)]), "*

 * *                              "'distanceByTipCount': OrderedDict([('1', 13.0) […]*

```diff
@@ -1,87 +1,75 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipettePropertiesSchema.json",
     "availableSensors": {
         "capacitive": {
-            "count": 2
+            "count": 1
         },
         "environment": {
             "count": 1
         },
         "pressure": {
-            "count": 2
+            "count": 1
         },
         "sensors": [
             "pressure",
             "capacitive",
             "environment"
         ]
     },
     "backCompatNames": [],
     "backlashDistance": 0.1,
-    "channels": 8,
+    "channels": 1,
     "displayCategory": "FLEX",
-    "displayName": "Flex 8-Channel 50 \u03bcL",
+    "displayName": "Flex 1-Channel 50 \u03bcL",
     "dropTipConfigurations": {
         "plungerEject": {
             "current": 1.0,
             "speed": 10
         }
     },
     "model": "p50",
     "partialTipConfigurations": {
-        "availableConfigurations": [
-            1,
-            2,
-            3,
-            4,
-            5,
-            6,
-            7,
-            8
-        ],
-        "partialTipSupported": true
+        "availableConfigurations": null,
+        "partialTipSupported": false
     },
     "pickUpTipConfigurations": {
         "pressFit": {
             "currentByTipCount": {
-                "1": 0.15,
-                "2": 0.13,
-                "3": 0.19,
-                "4": 0.25,
-                "5": 0.31,
-                "6": 0.38,
-                "7": 0.44,
-                "8": 0.5
+                "1": 0.15
+            },
+            "distanceByTipCount": {
+                "1": 13.0
             },
-            "distance": 13.0,
             "increment": 0.0,
             "presses": 1,
-            "speed": 10
+            "speedByTipCount": {
+                "1": 5
+            }
         }
     },
     "plungerHomingConfigurations": {
         "current": 1.0,
         "speed": 30
     },
     "plungerMotorConfigurations": {
         "idle": 0.3,
         "run": 1.0
     },
     "plungerPositionsConfigurations": {
         "default": {
             "blowout": 76.5,
             "bottom": 71.5,
-            "drop": 92.5,
+            "drop": 90.5,
             "top": 0.5
         },
         "lowVolumeDefault": {
             "blowout": 76.5,
             "bottom": 61.5,
-            "drop": 92.5,
+            "drop": 90.5,
             "top": 0.5
         }
     },
     "quirks": [],
     "shaftDiameter": 1.0,
     "shaftULperMM": 0.785
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p50/3_4.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p1000/3_5.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8059348739495799%*

 * *Differences: {"'availableSensors'": "{'pressure': {'count': 1}, 'capacitive': {'count': 1}}",*

 * * "'channels'": '1',*

 * * "'displayName'": "'Flex 1-Channel 1000 μL'",*

 * * "'dropTipConfigurations'": "{'plungerEject': {'speed': 15}}",*

 * * "'model'": "'p1000'",*

 * * "'partialTipConfigurations'": "{'partialTipSupported': False, 'availableConfigurations': None}",*

 * * "'pickUpTipConfigurations'": "{'pressFit': {'currentByTipCount': {delete: ['2', '3', '4', '5', "*

 * *                              "'6', '7', '8']}, 'speedByTipCount': OrderedDict([('1 […]*

```diff
@@ -1,87 +1,69 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipettePropertiesSchema.json",
     "availableSensors": {
         "capacitive": {
-            "count": 2
+            "count": 1
         },
         "environment": {
             "count": 1
         },
         "pressure": {
-            "count": 2
+            "count": 1
         },
         "sensors": [
             "pressure",
             "capacitive",
             "environment"
         ]
     },
     "backCompatNames": [],
     "backlashDistance": 0.1,
-    "channels": 8,
+    "channels": 1,
     "displayCategory": "FLEX",
-    "displayName": "Flex 8-Channel 50 \u03bcL",
+    "displayName": "Flex 1-Channel 1000 \u03bcL",
     "dropTipConfigurations": {
         "plungerEject": {
             "current": 1.0,
-            "speed": 10
+            "speed": 15
         }
     },
-    "model": "p50",
+    "model": "p1000",
     "partialTipConfigurations": {
-        "availableConfigurations": [
-            1,
-            2,
-            3,
-            4,
-            5,
-            6,
-            7,
-            8
-        ],
-        "partialTipSupported": true
+        "availableConfigurations": null,
+        "partialTipSupported": false
     },
     "pickUpTipConfigurations": {
         "pressFit": {
             "currentByTipCount": {
-                "1": 0.2,
-                "2": 0.14,
-                "3": 0.2,
-                "4": 0.28,
-                "5": 0.34,
-                "6": 0.41,
-                "7": 0.48,
-                "8": 0.55
+                "1": 0.2
+            },
+            "distanceByTipCount": {
+                "1": 13.0
             },
-            "distance": 13.0,
             "increment": 0.0,
             "presses": 1,
-            "speed": 10
+            "speedByTipCount": {
+                "1": 10.0
+            }
         }
     },
     "plungerHomingConfigurations": {
         "current": 1.0,
         "speed": 30
     },
     "plungerMotorConfigurations": {
         "idle": 0.3,
         "run": 1.0
     },
     "plungerPositionsConfigurations": {
         "default": {
             "blowout": 76.5,
             "bottom": 71.5,
-            "drop": 91.5,
-            "top": 0.0
-        },
-        "lowVolumeDefault": {
-            "blowout": 76.5,
-            "bottom": 61.5,
-            "drop": 91.5,
+            "drop": 90.5,
             "top": 0.0
         }
     },
     "quirks": [],
-    "shaftDiameter": 1.0,
-    "shaftULperMM": 0.785
+    "shaftDiameter": 4.5,
+    "shaftULperMM": 15.904
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p50/3_5.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p1000/3_6.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8059348739495799%*

 * *Differences: {"'availableSensors'": "{'pressure': {'count': 1}, 'capacitive': {'count': 1}}",*

 * * "'channels'": '1',*

 * * "'displayName'": "'Flex 1-Channel 1000 μL'",*

 * * "'dropTipConfigurations'": "{'plungerEject': {'speed': 15}}",*

 * * "'model'": "'p1000'",*

 * * "'partialTipConfigurations'": "{'partialTipSupported': False, 'availableConfigurations': None}",*

 * * "'pickUpTipConfigurations'": "{'pressFit': {'currentByTipCount': {delete: ['2', '3', '4', '5', "*

 * *                              "'6', '7', '8']}, 'speedByTipCount': OrderedDict([('1 […]*

```diff
@@ -1,87 +1,69 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipettePropertiesSchema.json",
     "availableSensors": {
         "capacitive": {
-            "count": 2
+            "count": 1
         },
         "environment": {
             "count": 1
         },
         "pressure": {
-            "count": 2
+            "count": 1
         },
         "sensors": [
             "pressure",
             "capacitive",
             "environment"
         ]
     },
     "backCompatNames": [],
     "backlashDistance": 0.1,
-    "channels": 8,
+    "channels": 1,
     "displayCategory": "FLEX",
-    "displayName": "Flex 8-Channel 50 \u03bcL",
+    "displayName": "Flex 1-Channel 1000 \u03bcL",
     "dropTipConfigurations": {
         "plungerEject": {
             "current": 1.0,
-            "speed": 10
+            "speed": 15
         }
     },
-    "model": "p50",
+    "model": "p1000",
     "partialTipConfigurations": {
-        "availableConfigurations": [
-            1,
-            2,
-            3,
-            4,
-            5,
-            6,
-            7,
-            8
-        ],
-        "partialTipSupported": true
+        "availableConfigurations": null,
+        "partialTipSupported": false
     },
     "pickUpTipConfigurations": {
         "pressFit": {
             "currentByTipCount": {
-                "1": 0.2,
-                "2": 0.14,
-                "3": 0.2,
-                "4": 0.28,
-                "5": 0.34,
-                "6": 0.41,
-                "7": 0.48,
-                "8": 0.55
+                "1": 0.2
+            },
+            "distanceByTipCount": {
+                "1": 13.0
             },
-            "distance": 13.0,
             "increment": 0.0,
             "presses": 1,
-            "speed": 10
+            "speedByTipCount": {
+                "1": 10.0
+            }
         }
     },
     "plungerHomingConfigurations": {
         "current": 1.0,
         "speed": 30
     },
     "plungerMotorConfigurations": {
         "idle": 0.3,
         "run": 1.0
     },
     "plungerPositionsConfigurations": {
         "default": {
             "blowout": 76.5,
             "bottom": 71.5,
-            "drop": 91.5,
-            "top": 0.0
-        },
-        "lowVolumeDefault": {
-            "blowout": 76.5,
-            "bottom": 61.5,
-            "drop": 91.5,
+            "drop": 90.5,
             "top": 0.0
         }
     },
     "quirks": [],
-    "shaftDiameter": 1.0,
-    "shaftULperMM": 0.785
+    "shaftDiameter": 4.5,
+    "shaftULperMM": 15.904
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/ninety_six_channel/p1000/1_0.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/ninety_six_channel/p1000/1_0.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9962406015037595%*

 * *Differences: {"'pickUpTipConfigurations'": "{'pressFit': {'speedByTipCount': OrderedDict([('1', 10.0), ('2', "*

 * *                              "10.0), ('3', 10.0), ('4', 10.0), ('5', 10.0), ('6', 10.0), ('7', "*

 * *                              "10.0), ('8', 10.0), ('12', 10.0), ('16', 10.0), ('24', 10.0), "*

 * *                              "('48', 10.0)]), 'distanceByTipCount': OrderedDict([('1', 13.0), "*

 * *                              "('2', 13.0), ('3', 13.0), ('4', 13.0), ('5', 13.0), ('6', 13.0), "*

 * *                           […]*

```diff
@@ -63,18 +63,44 @@
                 "4": 0.35,
                 "48": 0.75,
                 "5": 0.4,
                 "6": 0.45,
                 "7": 0.5,
                 "8": 0.55
             },
-            "distance": 13.0,
+            "distanceByTipCount": {
+                "1": 13.0,
+                "12": 13.0,
+                "16": 13.0,
+                "2": 13.0,
+                "24": 13.0,
+                "3": 13.0,
+                "4": 13.0,
+                "48": 13.0,
+                "5": 13.0,
+                "6": 13.0,
+                "7": 13.0,
+                "8": 13.0
+            },
             "increment": 0.0,
             "presses": 1,
-            "speed": 10.0
+            "speedByTipCount": {
+                "1": 10.0,
+                "12": 10.0,
+                "16": 10.0,
+                "2": 10.0,
+                "24": 10.0,
+                "3": 10.0,
+                "4": 10.0,
+                "48": 10.0,
+                "5": 10.0,
+                "6": 10.0,
+                "7": 10.0,
+                "8": 10.0
+            }
         }
     },
     "plungerHomingConfigurations": {
         "current": 2.0,
         "speed": 5
     },
     "plungerMotorConfigurations": {
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/ninety_six_channel/p1000/3_0.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/ninety_six_channel/p1000/3_6.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9368107769423558%*

 * *Differences: {"'backlashDistance'": '3.0',*

 * * "'dropTipConfigurations'": "{'camAction': {'distance': 10.8, 'prep_move_distance': 19.0}, delete: "*

 * *                            "['plungerEject']}",*

 * * "'pickUpTipConfigurations'": "{'pressFit': {'speedByTipCount': OrderedDict([('1', 10.0), ('2', "*

 * *                              "10.0), ('3', 10.0), ('4', 10.0), ('5', 10.0), ('6', 10.0), ('7', "*

 * *                              "10.0), ('8', 10.0), ('12', 10.0), ('16', 10.0), ('24', 10.0), "*

 * *                              "('48', 10. […]*

```diff
@@ -13,30 +13,25 @@
         "sensors": [
             "pressure",
             "capacitive",
             "environment"
         ]
     },
     "backCompatNames": [],
-    "backlashDistance": 0.3,
+    "backlashDistance": 3.0,
     "channels": 96,
     "displayCategory": "FLEX",
     "displayName": "Flex 96-Channel 1000 \u03bcL",
     "dropTipConfigurations": {
         "camAction": {
             "current": 1.5,
-            "distance": 10.5,
-            "prep_move_distance": 16.0,
+            "distance": 10.8,
+            "prep_move_distance": 19.0,
             "prep_move_speed": 10.0,
             "speed": 5.5
-        },
-        "plungerEject": {
-            "current": 1.5,
-            "distance": 10.5,
-            "speed": 5.5
         }
     },
     "endTipActionRetractDistanceMM": 2.0,
     "model": "p1000",
     "partialTipConfigurations": {
         "availableConfigurations": [
             1,
@@ -52,15 +47,15 @@
     "pickUpTipConfigurations": {
         "camAction": {
             "connectTiprackDistanceMM": 7.0,
             "currentByTipCount": {
                 "96": 1.5
             },
             "distance": 10.0,
-            "prep_move_distance": 9.0,
+            "prep_move_distance": 8.25,
             "prep_move_speed": 10.0,
             "speed": 5.5
         },
         "pressFit": {
             "currentByTipCount": {
                 "1": 0.2,
                 "12": 0.19,
@@ -71,34 +66,60 @@
                 "4": 0.35,
                 "48": 0.75,
                 "5": 0.4,
                 "6": 0.45,
                 "7": 0.5,
                 "8": 0.55
             },
-            "distance": 13.0,
+            "distanceByTipCount": {
+                "1": 13.0,
+                "12": 13.0,
+                "16": 13.0,
+                "2": 13.0,
+                "24": 13.0,
+                "3": 13.0,
+                "4": 13.0,
+                "48": 13.0,
+                "5": 13.0,
+                "6": 13.0,
+                "7": 13.0,
+                "8": 13.0
+            },
             "increment": 0.0,
             "presses": 1,
-            "speed": 10.0
+            "speedByTipCount": {
+                "1": 10.0,
+                "12": 10.0,
+                "16": 10.0,
+                "2": 10.0,
+                "24": 10.0,
+                "3": 10.0,
+                "4": 10.0,
+                "48": 10.0,
+                "5": 10.0,
+                "6": 10.0,
+                "7": 10.0,
+                "8": 10.0
+            }
         }
     },
     "plungerHomingConfigurations": {
-        "current": 2.0,
+        "current": 0.8,
         "speed": 5
     },
     "plungerMotorConfigurations": {
         "idle": 0.3,
-        "run": 2.0
+        "run": 0.8
     },
     "plungerPositionsConfigurations": {
         "default": {
-            "blowout": 71,
-            "bottom": 66,
+            "blowout": 73.5,
+            "bottom": 68.5,
             "drop": 80,
-            "top": 0
+            "top": 0.5
         }
     },
     "quirks": [],
     "shaftDiameter": 4.5,
     "shaftULperMM": 15.904,
     "tipPresenceCheckDistanceMM": 8.0
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/ninety_six_channel/p1000/3_3.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p1000/1_0.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6877289377289377%*

 * *Differences: {"'backlashDistance'": '0.0',*

 * * "'channels'": '8',*

 * * "'displayName'": "'Flex 8-Channel 1000 uL'",*

 * * "'dropTipConfigurations'": "{replace: OrderedDict([('plungerEject', OrderedDict([('current', "*

 * *                            "1.0), ('speed', 10)]))])}",*

 * * "'partialTipConfigurations'": "{'availableConfigurations': {insert: [(1, 2), (2, 3), (3, 4), (4, "*

 * *                               '5), (5, 6), (6, 7)], delete: [6, 5, 4, 3, 2]}}',*

 * * "'pickUpTipConfigurations'": "{'pressFit': {'currentByTipCount': {'1': 0.15, '2': […]*

```diff
@@ -13,87 +13,87 @@
         "sensors": [
             "pressure",
             "capacitive",
             "environment"
         ]
     },
     "backCompatNames": [],
-    "backlashDistance": 0.3,
-    "channels": 96,
+    "backlashDistance": 0.0,
+    "channels": 8,
     "displayCategory": "FLEX",
-    "displayName": "Flex 96-Channel 1000 \u03bcL",
+    "displayName": "Flex 8-Channel 1000 uL",
     "dropTipConfigurations": {
-        "camAction": {
-            "current": 1.5,
-            "distance": 10.5,
-            "prep_move_distance": 16.0,
-            "prep_move_speed": 10.0,
-            "speed": 5.5
+        "plungerEject": {
+            "current": 1.0,
+            "speed": 10
         }
     },
-    "endTipActionRetractDistanceMM": 2.0,
     "model": "p1000",
     "partialTipConfigurations": {
         "availableConfigurations": [
             1,
-            8,
-            12,
-            16,
-            24,
-            48,
-            96
+            2,
+            3,
+            4,
+            5,
+            6,
+            7,
+            8
         ],
         "partialTipSupported": true
     },
     "pickUpTipConfigurations": {
-        "camAction": {
-            "connectTiprackDistanceMM": 7.0,
-            "currentByTipCount": {
-                "96": 1.5
-            },
-            "distance": 10.0,
-            "prep_move_distance": 9.0,
-            "prep_move_speed": 10.0,
-            "speed": 5.5
-        },
         "pressFit": {
             "currentByTipCount": {
-                "1": 0.2,
-                "12": 0.19,
-                "16": 0.25,
-                "2": 0.25,
-                "24": 0.38,
-                "3": 0.3,
-                "4": 0.35,
-                "48": 0.75,
-                "5": 0.4,
-                "6": 0.45,
-                "7": 0.5,
-                "8": 0.55
+                "1": 0.15,
+                "2": 0.13,
+                "3": 0.19,
+                "4": 0.25,
+                "5": 0.31,
+                "6": 0.38,
+                "7": 0.44,
+                "8": 0.5
+            },
+            "distanceByTipCount": {
+                "1": 13.0,
+                "2": 13.0,
+                "3": 13.0,
+                "4": 13.0,
+                "5": 13.0,
+                "6": 13.0,
+                "7": 13.0,
+                "8": 13.0
             },
-            "distance": 13.0,
             "increment": 0.0,
             "presses": 1,
-            "speed": 10.0
+            "speedByTipCount": {
+                "1": 10.0,
+                "2": 10.0,
+                "3": 10.0,
+                "4": 10.0,
+                "5": 10.0,
+                "6": 10.0,
+                "7": 10.0,
+                "8": 10.0
+            }
         }
     },
     "plungerHomingConfigurations": {
-        "current": 2.0,
-        "speed": 5
+        "current": 1.0,
+        "speed": 30
     },
     "plungerMotorConfigurations": {
         "idle": 0.3,
-        "run": 2.0
+        "run": 1.0
     },
     "plungerPositionsConfigurations": {
         "default": {
-            "blowout": 71,
-            "bottom": 66,
-            "drop": 80,
-            "top": 0
+            "blowout": 76.5,
+            "bottom": 71.5,
+            "drop": 92.5,
+            "top": 0.5
         }
     },
     "quirks": [],
-    "shaftDiameter": 4.5,
-    "shaftULperMM": 15.904,
-    "tipPresenceCheckDistanceMM": 8.0
+    "shaftDiameter": 9.0,
+    "shaftULperMM": 63.617
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/ninety_six_channel/p1000/3_4.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/ninety_six_channel/p1000/3_5.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9956923558897244%*

 * *Differences: {"'pickUpTipConfigurations'": "{'pressFit': {'speedByTipCount': OrderedDict([('1', 10.0), ('2', "*

 * *                              "10.0), ('3', 10.0), ('4', 10.0), ('5', 10.0), ('6', 10.0), ('7', "*

 * *                              "10.0), ('8', 10.0), ('12', 10.0), ('16', 10.0), ('24', 10.0), "*

 * *                              "('48', 10.0)]), 'distanceByTipCount': OrderedDict([('1', 13.0), "*

 * *                              "('2', 13.0), ('3', 13.0), ('4', 13.0), ('5', 13.0), ('6', 13.0), "*

 * *                           […]*

```diff
@@ -47,15 +47,15 @@
     "pickUpTipConfigurations": {
         "camAction": {
             "connectTiprackDistanceMM": 7.0,
             "currentByTipCount": {
                 "96": 1.5
             },
             "distance": 10.0,
-            "prep_move_distance": 9.0,
+            "prep_move_distance": 8.25,
             "prep_move_speed": 10.0,
             "speed": 5.5
         },
         "pressFit": {
             "currentByTipCount": {
                 "1": 0.2,
                 "12": 0.19,
@@ -66,18 +66,44 @@
                 "4": 0.35,
                 "48": 0.75,
                 "5": 0.4,
                 "6": 0.45,
                 "7": 0.5,
                 "8": 0.55
             },
-            "distance": 13.0,
+            "distanceByTipCount": {
+                "1": 13.0,
+                "12": 13.0,
+                "16": 13.0,
+                "2": 13.0,
+                "24": 13.0,
+                "3": 13.0,
+                "4": 13.0,
+                "48": 13.0,
+                "5": 13.0,
+                "6": 13.0,
+                "7": 13.0,
+                "8": 13.0
+            },
             "increment": 0.0,
             "presses": 1,
-            "speed": 10.0
+            "speedByTipCount": {
+                "1": 10.0,
+                "12": 10.0,
+                "16": 10.0,
+                "2": 10.0,
+                "24": 10.0,
+                "3": 10.0,
+                "4": 10.0,
+                "48": 10.0,
+                "5": 10.0,
+                "6": 10.0,
+                "7": 10.0,
+                "8": 10.0
+            }
         }
     },
     "plungerHomingConfigurations": {
         "current": 0.8,
         "speed": 5
     },
     "plungerMotorConfigurations": {
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/ninety_six_channel/p1000/3_5.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/ninety_six_channel/p1000/3_4.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9956923558897244%*

 * *Differences: {"'pickUpTipConfigurations'": "{'pressFit': {'speedByTipCount': OrderedDict([('1', 10.0), ('2', "*

 * *                              "10.0), ('3', 10.0), ('4', 10.0), ('5', 10.0), ('6', 10.0), ('7', "*

 * *                              "10.0), ('8', 10.0), ('12', 10.0), ('16', 10.0), ('24', 10.0), "*

 * *                              "('48', 10.0)]), 'distanceByTipCount': OrderedDict([('1', 13.0), "*

 * *                              "('2', 13.0), ('3', 13.0), ('4', 13.0), ('5', 13.0), ('6', 13.0), "*

 * *                           […]*

```diff
@@ -47,15 +47,15 @@
     "pickUpTipConfigurations": {
         "camAction": {
             "connectTiprackDistanceMM": 7.0,
             "currentByTipCount": {
                 "96": 1.5
             },
             "distance": 10.0,
-            "prep_move_distance": 8.25,
+            "prep_move_distance": 9.0,
             "prep_move_speed": 10.0,
             "speed": 5.5
         },
         "pressFit": {
             "currentByTipCount": {
                 "1": 0.2,
                 "12": 0.19,
@@ -66,18 +66,44 @@
                 "4": 0.35,
                 "48": 0.75,
                 "5": 0.4,
                 "6": 0.45,
                 "7": 0.5,
                 "8": 0.55
             },
-            "distance": 13.0,
+            "distanceByTipCount": {
+                "1": 13.0,
+                "12": 13.0,
+                "16": 13.0,
+                "2": 13.0,
+                "24": 13.0,
+                "3": 13.0,
+                "4": 13.0,
+                "48": 13.0,
+                "5": 13.0,
+                "6": 13.0,
+                "7": 13.0,
+                "8": 13.0
+            },
             "increment": 0.0,
             "presses": 1,
-            "speed": 10.0
+            "speedByTipCount": {
+                "1": 10.0,
+                "12": 10.0,
+                "16": 10.0,
+                "2": 10.0,
+                "24": 10.0,
+                "3": 10.0,
+                "4": 10.0,
+                "48": 10.0,
+                "5": 10.0,
+                "6": 10.0,
+                "7": 10.0,
+                "8": 10.0
+            }
         }
     },
     "plungerHomingConfigurations": {
         "current": 0.8,
         "speed": 5
     },
     "plungerMotorConfigurations": {
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/ninety_six_channel/p1000/3_6.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/ninety_six_channel/p1000/3_3.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9486528822055138%*

 * *Differences: {"'backlashDistance'": '0.3',*

 * * "'dropTipConfigurations'": "{'camAction': {'distance': 10.5, 'prep_move_distance': 16.0}}",*

 * * "'pickUpTipConfigurations'": "{'pressFit': {'speedByTipCount': OrderedDict([('1', 10.0), ('2', "*

 * *                              "10.0), ('3', 10.0), ('4', 10.0), ('5', 10.0), ('6', 10.0), ('7', "*

 * *                              "10.0), ('8', 10.0), ('12', 10.0), ('16', 10.0), ('24', 10.0), "*

 * *                              "('48', 10.0)]), 'distanceByTipCount': OrderedDict([('1', 13.0), "*

 * *  […]*

```diff
@@ -13,23 +13,23 @@
         "sensors": [
             "pressure",
             "capacitive",
             "environment"
         ]
     },
     "backCompatNames": [],
-    "backlashDistance": 3.0,
+    "backlashDistance": 0.3,
     "channels": 96,
     "displayCategory": "FLEX",
     "displayName": "Flex 96-Channel 1000 \u03bcL",
     "dropTipConfigurations": {
         "camAction": {
             "current": 1.5,
-            "distance": 10.8,
-            "prep_move_distance": 19.0,
+            "distance": 10.5,
+            "prep_move_distance": 16.0,
             "prep_move_speed": 10.0,
             "speed": 5.5
         }
     },
     "endTipActionRetractDistanceMM": 2.0,
     "model": "p1000",
     "partialTipConfigurations": {
@@ -47,15 +47,15 @@
     "pickUpTipConfigurations": {
         "camAction": {
             "connectTiprackDistanceMM": 7.0,
             "currentByTipCount": {
                 "96": 1.5
             },
             "distance": 10.0,
-            "prep_move_distance": 8.25,
+            "prep_move_distance": 9.0,
             "prep_move_speed": 10.0,
             "speed": 5.5
         },
         "pressFit": {
             "currentByTipCount": {
                 "1": 0.2,
                 "12": 0.19,
@@ -66,34 +66,60 @@
                 "4": 0.35,
                 "48": 0.75,
                 "5": 0.4,
                 "6": 0.45,
                 "7": 0.5,
                 "8": 0.55
             },
-            "distance": 13.0,
+            "distanceByTipCount": {
+                "1": 13.0,
+                "12": 13.0,
+                "16": 13.0,
+                "2": 13.0,
+                "24": 13.0,
+                "3": 13.0,
+                "4": 13.0,
+                "48": 13.0,
+                "5": 13.0,
+                "6": 13.0,
+                "7": 13.0,
+                "8": 13.0
+            },
             "increment": 0.0,
             "presses": 1,
-            "speed": 10.0
+            "speedByTipCount": {
+                "1": 10.0,
+                "12": 10.0,
+                "16": 10.0,
+                "2": 10.0,
+                "24": 10.0,
+                "3": 10.0,
+                "4": 10.0,
+                "48": 10.0,
+                "5": 10.0,
+                "6": 10.0,
+                "7": 10.0,
+                "8": 10.0
+            }
         }
     },
     "plungerHomingConfigurations": {
-        "current": 0.8,
+        "current": 2.0,
         "speed": 5
     },
     "plungerMotorConfigurations": {
         "idle": 0.3,
-        "run": 0.8
+        "run": 2.0
     },
     "plungerPositionsConfigurations": {
         "default": {
-            "blowout": 73.5,
-            "bottom": 68.5,
+            "blowout": 71,
+            "bottom": 66,
             "drop": 80,
-            "top": 0.5
+            "top": 0
         }
     },
     "quirks": [],
     "shaftDiameter": 4.5,
     "shaftULperMM": 15.904,
     "tipPresenceCheckDistanceMM": 8.0
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p10/1_0.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p10/1_5.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8866859243697479%*

 * *Differences: {"'channels'": '8',*

 * * "'displayName'": "'P10 8-Channel GEN1'",*

 * * "'partialTipConfigurations'": "{'partialTipSupported': True, 'availableConfigurations': [1, 2, 3, "*

 * *                               '4, 5, 6, 7, 8]}',*

 * * "'pickUpTipConfigurations'": "{'pressFit': {'increment': 3.0, 'currentByTipCount': {'2': 0.14, "*

 * *                              "'3': 0.21, '4': 0.28, '5': 0.34, '6': 0.41, '7': 0.48, '8': 0.55}, "*

 * *                              "'speedByTipCount': OrderedDict([('1', 30.0), ('2', 30.0), ('3', "*

 * *     […]*

```diff
@@ -1,54 +1,89 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipettePropertiesSchema.json",
     "availableSensors": {
         "sensors": []
     },
     "backCompatNames": [],
     "backlashDistance": 0.0,
-    "channels": 1,
+    "channels": 8,
     "displayCategory": "GEN1",
-    "displayName": "P10 Single-Channel GEN1",
+    "displayName": "P10 8-Channel GEN1",
     "dropTipConfigurations": {
         "plungerEject": {
             "current": 0.5,
             "speed": 5.0
         }
     },
     "model": "p10",
     "partialTipConfigurations": {
-        "availableConfigurations": null,
-        "partialTipSupported": false
+        "availableConfigurations": [
+            1,
+            2,
+            3,
+            4,
+            5,
+            6,
+            7,
+            8
+        ],
+        "partialTipSupported": true
     },
     "pickUpTipConfigurations": {
         "pressFit": {
             "currentByTipCount": {
-                "1": 0.1
+                "1": 0.1,
+                "2": 0.14,
+                "3": 0.21,
+                "4": 0.28,
+                "5": 0.34,
+                "6": 0.41,
+                "7": 0.48,
+                "8": 0.55
             },
-            "distance": 10.0,
-            "increment": 1.0,
+            "distanceByTipCount": {
+                "1": 10.0,
+                "2": 10.0,
+                "3": 10.0,
+                "4": 10.0,
+                "5": 10.0,
+                "6": 10.0,
+                "7": 10.0,
+                "8": 10.0
+            },
+            "increment": 3.0,
             "presses": 3,
-            "speed": 30.0
+            "speedByTipCount": {
+                "1": 30.0,
+                "2": 30.0,
+                "3": 30.0,
+                "4": 30.0,
+                "5": 30.0,
+                "6": 30.0,
+                "7": 30.0,
+                "8": 30.0
+            }
         }
     },
     "plungerHomingConfigurations": {
-        "current": 0.3,
+        "current": 0.5,
         "speed": 30
     },
     "plungerMotorConfigurations": {
         "idle": 0.05,
-        "run": 0.3
+        "run": 0.5
     },
     "plungerPositionsConfigurations": {
         "default": {
             "blowout": -1.0,
             "bottom": 2.0,
             "drop": -4.5,
             "top": 19.5
         }
     },
     "quirks": [
-        "dropTipShake"
+        "dropTipShake",
+        "doubleDropTip"
     ],
     "shaftDiameter": 1.0,
     "shaftULperMM": 0.785
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p10/1_3.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p1000/1_5.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8348214285714285%*

 * *Differences: {"'displayName'": "'P1000 Single-Channel GEN1'",*

 * * "'dropTipConfigurations'": "{'plungerEject': {'current': 0.7}}",*

 * * "'model'": "'p1000'",*

 * * "'pickUpTipConfigurations'": "{'pressFit': {'currentByTipCount': {'1': 0.15}, 'speedByTipCount': "*

 * *                              "OrderedDict([('1', 30.0)]), 'distanceByTipCount': "*

 * *                              "OrderedDict([('1', 15.0)]), delete: ['speed', 'distance']}}",*

 * * "'plungerHomingConfigurations'": "{'current': 0.5}",*

 * * "'plungerMotorConfigurations'": "{'run': 0. […]*

```diff
@@ -3,52 +3,57 @@
     "availableSensors": {
         "sensors": []
     },
     "backCompatNames": [],
     "backlashDistance": 0.0,
     "channels": 1,
     "displayCategory": "GEN1",
-    "displayName": "P10 Single-Channel GEN1",
+    "displayName": "P1000 Single-Channel GEN1",
     "dropTipConfigurations": {
         "plungerEject": {
-            "current": 0.5,
+            "current": 0.7,
             "speed": 5.0
         }
     },
-    "model": "p10",
+    "model": "p1000",
     "partialTipConfigurations": {
         "availableConfigurations": null,
         "partialTipSupported": false
     },
     "pickUpTipConfigurations": {
         "pressFit": {
             "currentByTipCount": {
-                "1": 0.1
+                "1": 0.15
+            },
+            "distanceByTipCount": {
+                "1": 15.0
             },
-            "distance": 10.0,
             "increment": 1.0,
             "presses": 3,
-            "speed": 30.0
+            "speedByTipCount": {
+                "1": 30.0
+            }
         }
     },
     "plungerHomingConfigurations": {
-        "current": 0.3,
+        "current": 0.5,
         "speed": 30
     },
     "plungerMotorConfigurations": {
         "idle": 0.05,
-        "run": 0.3
+        "run": 0.5
     },
     "plungerPositionsConfigurations": {
         "default": {
-            "blowout": -2.5,
-            "bottom": 0.5,
-            "drop": -6.0,
+            "blowout": 0.5,
+            "bottom": 2.5,
+            "drop": -4.0,
             "top": 19.5
         }
     },
     "quirks": [
+        "pickupTipShake",
         "dropTipShake"
     ],
-    "shaftDiameter": 1.0,
-    "shaftULperMM": 0.785
+    "shaftDiameter": 9.0,
+    "shaftULperMM": 63.617
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p10/1_4.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p1000/1_0.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8390231092436975%*

 * *Differences: {"'displayName'": "'P1000 Single-Channel GEN1'",*

 * * "'model'": "'p1000'",*

 * * "'pickUpTipConfigurations'": "{'pressFit': {'speedByTipCount': OrderedDict([('1', 30.0)]), "*

 * *                              "'distanceByTipCount': OrderedDict([('1', 15.0)]), delete: ['speed', "*

 * *                              "'distance']}}",*

 * * "'plungerHomingConfigurations'": "{'current': 0.5}",*

 * * "'plungerMotorConfigurations'": "{'run': 0.5}",*

 * * "'plungerPositionsConfigurations'": "{'default': {'bottom': 3.0, 'blowout': 1.0, 'drop': -2.2} […]*

```diff
@@ -3,52 +3,57 @@
     "availableSensors": {
         "sensors": []
     },
     "backCompatNames": [],
     "backlashDistance": 0.0,
     "channels": 1,
     "displayCategory": "GEN1",
-    "displayName": "P10 Single-Channel GEN1",
+    "displayName": "P1000 Single-Channel GEN1",
     "dropTipConfigurations": {
         "plungerEject": {
             "current": 0.5,
             "speed": 5.0
         }
     },
-    "model": "p10",
+    "model": "p1000",
     "partialTipConfigurations": {
         "availableConfigurations": null,
         "partialTipSupported": false
     },
     "pickUpTipConfigurations": {
         "pressFit": {
             "currentByTipCount": {
                 "1": 0.1
             },
-            "distance": 10.0,
+            "distanceByTipCount": {
+                "1": 15.0
+            },
             "increment": 1.0,
             "presses": 3,
-            "speed": 30.0
+            "speedByTipCount": {
+                "1": 30.0
+            }
         }
     },
     "plungerHomingConfigurations": {
-        "current": 0.3,
+        "current": 0.5,
         "speed": 30
     },
     "plungerMotorConfigurations": {
         "idle": 0.05,
-        "run": 0.3
+        "run": 0.5
     },
     "plungerPositionsConfigurations": {
         "default": {
-            "blowout": -0.5,
-            "bottom": 2.5,
-            "drop": -5.2,
+            "blowout": 1.0,
+            "bottom": 3.0,
+            "drop": -2.2,
             "top": 19.5
         }
     },
     "quirks": [
+        "pickupTipShake",
         "dropTipShake"
     ],
-    "shaftDiameter": 1.0,
-    "shaftULperMM": 0.785
+    "shaftDiameter": 9.0,
+    "shaftULperMM": 63.617
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p10/1_5.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p1000/2_1.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7481617647058824%*

 * *Differences: {"'backCompatNames'": "['p1000_single']",*

 * * "'displayCategory'": "'GEN2'",*

 * * "'displayName'": "'P1000 Single-Channel GEN2'",*

 * * "'dropTipConfigurations'": "{'plungerEject': {'current': 1.25, 'speed': 7.0}}",*

 * * "'model'": "'p1000'",*

 * * "'pickUpTipConfigurations'": "{'pressFit': {'presses': 1, 'increment': 0.0, 'currentByTipCount': "*

 * *                              "{'1': 0.17}, 'speedByTipCount': OrderedDict([('1', 10.0)]), "*

 * *                              "'distanceByTipCount': OrderedDict([('1', 17.0)]), delete: ['s […]*

```diff
@@ -1,54 +1,60 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipettePropertiesSchema.json",
     "availableSensors": {
         "sensors": []
     },
-    "backCompatNames": [],
+    "backCompatNames": [
+        "p1000_single"
+    ],
     "backlashDistance": 0.0,
     "channels": 1,
-    "displayCategory": "GEN1",
-    "displayName": "P10 Single-Channel GEN1",
+    "displayCategory": "GEN2",
+    "displayName": "P1000 Single-Channel GEN2",
     "dropTipConfigurations": {
         "plungerEject": {
-            "current": 0.5,
-            "speed": 5.0
+            "current": 1.25,
+            "speed": 7.0
         }
     },
-    "model": "p10",
+    "model": "p1000",
     "partialTipConfigurations": {
         "availableConfigurations": null,
         "partialTipSupported": false
     },
     "pickUpTipConfigurations": {
         "pressFit": {
             "currentByTipCount": {
-                "1": 0.1
+                "1": 0.17
+            },
+            "distanceByTipCount": {
+                "1": 17.0
             },
-            "distance": 10.0,
-            "increment": 1.0,
-            "presses": 3,
-            "speed": 30.0
+            "increment": 0.0,
+            "presses": 1,
+            "speedByTipCount": {
+                "1": 10.0
+            }
         }
     },
     "plungerHomingConfigurations": {
-        "current": 0.3,
+        "current": 1.0,
         "speed": 30
     },
     "plungerMotorConfigurations": {
-        "idle": 0.05,
-        "run": 0.3
+        "idle": 0.3,
+        "run": 1.0
     },
     "plungerPositionsConfigurations": {
         "default": {
-            "blowout": -0.5,
-            "bottom": 2.5,
-            "drop": -5.2,
+            "blowout": -23.0,
+            "bottom": -18.5,
+            "drop": -37.0,
             "top": 19.5
         }
     },
     "quirks": [
-        "dropTipShake"
+        "pickupTipShake"
     ],
-    "shaftDiameter": 1.0,
-    "shaftULperMM": 0.785
+    "shaftDiameter": 6.0,
+    "shaftULperMM": 28.274
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p1000/1_0.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p300/1_5.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8027398459383753%*

 * *Differences: {"'channels'": '8',*

 * * "'displayName'": "'P300 8-Channel GEN1'",*

 * * "'model'": "'p300'",*

 * * "'partialTipConfigurations'": "{'partialTipSupported': True, 'availableConfigurations': [1, 2, 3, "*

 * *                               '4, 5, 6, 7, 8]}',*

 * * "'pickUpTipConfigurations'": "{'pressFit': {'increment': 3.0, 'currentByTipCount': {'2': 0.23, "*

 * *                              "'3': 0.34, '4': 0.45, '5': 0.56, '6': 0.68, '7': 0.79, '8': 0.9}, "*

 * *                              "'speedByTipCount': OrderedDict([('1', 30.0), ('2 […]*

```diff
@@ -1,55 +1,89 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipettePropertiesSchema.json",
     "availableSensors": {
         "sensors": []
     },
     "backCompatNames": [],
     "backlashDistance": 0.0,
-    "channels": 1,
+    "channels": 8,
     "displayCategory": "GEN1",
-    "displayName": "P1000 Single-Channel GEN1",
+    "displayName": "P300 8-Channel GEN1",
     "dropTipConfigurations": {
         "plungerEject": {
             "current": 0.5,
             "speed": 5.0
         }
     },
-    "model": "p1000",
+    "model": "p300",
     "partialTipConfigurations": {
-        "availableConfigurations": null,
-        "partialTipSupported": false
+        "availableConfigurations": [
+            1,
+            2,
+            3,
+            4,
+            5,
+            6,
+            7,
+            8
+        ],
+        "partialTipSupported": true
     },
     "pickUpTipConfigurations": {
         "pressFit": {
             "currentByTipCount": {
-                "1": 0.1
+                "1": 0.1,
+                "2": 0.23,
+                "3": 0.34,
+                "4": 0.45,
+                "5": 0.56,
+                "6": 0.68,
+                "7": 0.79,
+                "8": 0.9
             },
-            "distance": 15.0,
-            "increment": 1.0,
+            "distanceByTipCount": {
+                "1": 10.0,
+                "2": 10.0,
+                "3": 10.0,
+                "4": 10.0,
+                "5": 10.0,
+                "6": 10.0,
+                "7": 10.0,
+                "8": 10.0
+            },
+            "increment": 3.0,
             "presses": 3,
-            "speed": 30.0
+            "speedByTipCount": {
+                "1": 30.0,
+                "2": 30.0,
+                "3": 30.0,
+                "4": 30.0,
+                "5": 30.0,
+                "6": 30.0,
+                "7": 30.0,
+                "8": 30.0
+            }
         }
     },
     "plungerHomingConfigurations": {
         "current": 0.5,
         "speed": 30
     },
     "plungerMotorConfigurations": {
         "idle": 0.05,
         "run": 0.5
     },
     "plungerPositionsConfigurations": {
         "default": {
-            "blowout": 1.0,
-            "bottom": 3.0,
-            "drop": -2.2,
+            "blowout": 1.5,
+            "bottom": 3.5,
+            "drop": -3.5,
             "top": 19.5
         }
     },
     "quirks": [
-        "pickupTipShake",
-        "dropTipShake"
+        "dropTipShake",
+        "doubleDropTip"
     ],
-    "shaftDiameter": 9.0,
-    "shaftULperMM": 63.617
+    "shaftDiameter": 5.0,
+    "shaftULperMM": 19.635
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p1000/1_3.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p1000/2_2.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7922794117647058%*

 * *Differences: {"'backCompatNames'": "['p1000_single']",*

 * * "'displayCategory'": "'GEN2'",*

 * * "'displayName'": "'P1000 Single-Channel GEN2'",*

 * * "'dropTipConfigurations'": "{'plungerEject': {'current': 1.25, 'speed': 7.0}}",*

 * * "'pickUpTipConfigurations'": "{'pressFit': {'presses': 1, 'increment': 0.0, 'currentByTipCount': "*

 * *                              "{'1': 0.17}, 'speedByTipCount': OrderedDict([('1', 10.0)]), "*

 * *                              "'distanceByTipCount': OrderedDict([('1', 17.0)]), delete: ['speed', "*

 * *               […]*

```diff
@@ -1,55 +1,60 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipettePropertiesSchema.json",
     "availableSensors": {
         "sensors": []
     },
-    "backCompatNames": [],
+    "backCompatNames": [
+        "p1000_single"
+    ],
     "backlashDistance": 0.0,
     "channels": 1,
-    "displayCategory": "GEN1",
-    "displayName": "P1000 Single-Channel GEN1",
+    "displayCategory": "GEN2",
+    "displayName": "P1000 Single-Channel GEN2",
     "dropTipConfigurations": {
         "plungerEject": {
-            "current": 0.7,
-            "speed": 5.0
+            "current": 1.25,
+            "speed": 7.0
         }
     },
     "model": "p1000",
     "partialTipConfigurations": {
         "availableConfigurations": null,
         "partialTipSupported": false
     },
     "pickUpTipConfigurations": {
         "pressFit": {
             "currentByTipCount": {
-                "1": 0.1
+                "1": 0.17
+            },
+            "distanceByTipCount": {
+                "1": 17.0
             },
-            "distance": 15.0,
-            "increment": 1.0,
-            "presses": 3,
-            "speed": 30.0
+            "increment": 0.0,
+            "presses": 1,
+            "speedByTipCount": {
+                "1": 10.0
+            }
         }
     },
     "plungerHomingConfigurations": {
-        "current": 0.5,
+        "current": 1.0,
         "speed": 30
     },
     "plungerMotorConfigurations": {
-        "idle": 0.05,
-        "run": 0.5
+        "idle": 0.3,
+        "run": 1.0
     },
     "plungerPositionsConfigurations": {
         "default": {
-            "blowout": 0.5,
-            "bottom": 2.5,
-            "drop": -4.0,
+            "blowout": -23.0,
+            "bottom": -18.5,
+            "drop": -37.0,
             "top": 19.5
         }
     },
     "quirks": [
-        "pickupTipShake",
-        "dropTipShake"
+        "pickupTipShake"
     ],
-    "shaftDiameter": 9.0,
-    "shaftULperMM": 63.617
+    "shaftDiameter": 6.0,
+    "shaftULperMM": 28.274
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p1000/1_4.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p1000/2_0.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7996323529411765%*

 * *Differences: {"'backCompatNames'": "['p1000_single']",*

 * * "'displayCategory'": "'GEN2'",*

 * * "'displayName'": "'P1000 Single-Channel GEN2'",*

 * * "'dropTipConfigurations'": "{'plungerEject': {'current': 1.25, 'speed': 7.0}}",*

 * * "'pickUpTipConfigurations'": "{'pressFit': {'presses': 1, 'increment': 0.0, 'currentByTipCount': "*

 * *                              "{'1': 0.17}, 'speedByTipCount': OrderedDict([('1', 10.0)]), "*

 * *                              "'distanceByTipCount': OrderedDict([('1', 17.0)]), delete: ['speed', "*

 * *               […]*

```diff
@@ -1,55 +1,60 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipettePropertiesSchema.json",
     "availableSensors": {
         "sensors": []
     },
-    "backCompatNames": [],
+    "backCompatNames": [
+        "p1000_single"
+    ],
     "backlashDistance": 0.0,
     "channels": 1,
-    "displayCategory": "GEN1",
-    "displayName": "P1000 Single-Channel GEN1",
+    "displayCategory": "GEN2",
+    "displayName": "P1000 Single-Channel GEN2",
     "dropTipConfigurations": {
         "plungerEject": {
-            "current": 0.7,
-            "speed": 5.0
+            "current": 1.25,
+            "speed": 7.0
         }
     },
     "model": "p1000",
     "partialTipConfigurations": {
         "availableConfigurations": null,
         "partialTipSupported": false
     },
     "pickUpTipConfigurations": {
         "pressFit": {
             "currentByTipCount": {
-                "1": 0.1
+                "1": 0.17
+            },
+            "distanceByTipCount": {
+                "1": 17.0
             },
-            "distance": 15.0,
-            "increment": 1.0,
-            "presses": 3,
-            "speed": 30.0
+            "increment": 0.0,
+            "presses": 1,
+            "speedByTipCount": {
+                "1": 10.0
+            }
         }
     },
     "plungerHomingConfigurations": {
-        "current": 0.5,
+        "current": 1.0,
         "speed": 30
     },
     "plungerMotorConfigurations": {
         "idle": 0.05,
-        "run": 0.5
+        "run": 1.0
     },
     "plungerPositionsConfigurations": {
         "default": {
-            "blowout": 0.5,
-            "bottom": 2.5,
-            "drop": -4.0,
+            "blowout": -23.0,
+            "bottom": -18.5,
+            "drop": -37.0,
             "top": 19.5
         }
     },
     "quirks": [
-        "pickupTipShake",
-        "dropTipShake"
+        "pickupTipShake"
     ],
-    "shaftDiameter": 9.0,
-    "shaftULperMM": 63.617
+    "shaftDiameter": 6.0,
+    "shaftULperMM": 28.274
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p1000/1_5.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p10/1_0.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8348214285714285%*

 * *Differences: {"'displayName'": "'P10 Single-Channel GEN1'",*

 * * "'dropTipConfigurations'": "{'plungerEject': {'current': 0.5}}",*

 * * "'model'": "'p10'",*

 * * "'pickUpTipConfigurations'": "{'pressFit': {'currentByTipCount': {'1': 0.1}, 'speedByTipCount': "*

 * *                              "OrderedDict([('1', 30.0)]), 'distanceByTipCount': "*

 * *                              "OrderedDict([('1', 10.0)]), delete: ['speed', 'distance']}}",*

 * * "'plungerHomingConfigurations'": "{'current': 0.3}",*

 * * "'plungerMotorConfigurations'": "{'run': 0.3}",*

 * * […]*

```diff
@@ -3,53 +3,56 @@
     "availableSensors": {
         "sensors": []
     },
     "backCompatNames": [],
     "backlashDistance": 0.0,
     "channels": 1,
     "displayCategory": "GEN1",
-    "displayName": "P1000 Single-Channel GEN1",
+    "displayName": "P10 Single-Channel GEN1",
     "dropTipConfigurations": {
         "plungerEject": {
-            "current": 0.7,
+            "current": 0.5,
             "speed": 5.0
         }
     },
-    "model": "p1000",
+    "model": "p10",
     "partialTipConfigurations": {
         "availableConfigurations": null,
         "partialTipSupported": false
     },
     "pickUpTipConfigurations": {
         "pressFit": {
             "currentByTipCount": {
-                "1": 0.15
+                "1": 0.1
+            },
+            "distanceByTipCount": {
+                "1": 10.0
             },
-            "distance": 15.0,
             "increment": 1.0,
             "presses": 3,
-            "speed": 30.0
+            "speedByTipCount": {
+                "1": 30.0
+            }
         }
     },
     "plungerHomingConfigurations": {
-        "current": 0.5,
+        "current": 0.3,
         "speed": 30
     },
     "plungerMotorConfigurations": {
         "idle": 0.05,
-        "run": 0.5
+        "run": 0.3
     },
     "plungerPositionsConfigurations": {
         "default": {
-            "blowout": 0.5,
-            "bottom": 2.5,
-            "drop": -4.0,
+            "blowout": -1.0,
+            "bottom": 2.0,
+            "drop": -4.5,
             "top": 19.5
         }
     },
     "quirks": [
-        "pickupTipShake",
         "dropTipShake"
     ],
-    "shaftDiameter": 9.0,
-    "shaftULperMM": 63.617
+    "shaftDiameter": 1.0,
+    "shaftULperMM": 0.785
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p1000/3_0.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p50/3_4.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8086265756302521%*

 * *Differences: {"'availableSensors'": "{'pressure': {'count': 2}, 'capacitive': {'count': 2}}",*

 * * "'channels'": '8',*

 * * "'displayName'": "'Flex 8-Channel 50 μL'",*

 * * "'model'": "'p50'",*

 * * "'partialTipConfigurations'": "{'partialTipSupported': True, 'availableConfigurations': [1, 2, 3, "*

 * *                               '4, 5, 6, 7, 8]}',*

 * * "'pickUpTipConfigurations'": "{'pressFit': {'currentByTipCount': {'1': 0.2, '2': 0.14, '3': 0.2, "*

 * *                              "'4': 0.28, '5': 0.34, '6': 0.41, '7': 0.48, '8': 0.55}, "*

 * *       […]*

```diff
@@ -1,65 +1,105 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipettePropertiesSchema.json",
     "availableSensors": {
         "capacitive": {
-            "count": 1
+            "count": 2
         },
         "environment": {
             "count": 1
         },
         "pressure": {
-            "count": 1
+            "count": 2
         },
         "sensors": [
             "pressure",
             "capacitive",
             "environment"
         ]
     },
     "backCompatNames": [],
     "backlashDistance": 0.1,
-    "channels": 1,
+    "channels": 8,
     "displayCategory": "FLEX",
-    "displayName": "Flex 1-Channel 1000 \u03bcL",
+    "displayName": "Flex 8-Channel 50 \u03bcL",
     "dropTipConfigurations": {
         "plungerEject": {
             "current": 1.0,
             "speed": 10
         }
     },
-    "model": "p1000",
+    "model": "p50",
     "partialTipConfigurations": {
-        "availableConfigurations": null,
-        "partialTipSupported": false
+        "availableConfigurations": [
+            1,
+            2,
+            3,
+            4,
+            5,
+            6,
+            7,
+            8
+        ],
+        "partialTipSupported": true
     },
     "pickUpTipConfigurations": {
         "pressFit": {
             "currentByTipCount": {
-                "1": 0.15
+                "1": 0.2,
+                "2": 0.14,
+                "3": 0.2,
+                "4": 0.28,
+                "5": 0.34,
+                "6": 0.41,
+                "7": 0.48,
+                "8": 0.55
+            },
+            "distanceByTipCount": {
+                "1": 13.0,
+                "2": 13.0,
+                "3": 13.0,
+                "4": 13.0,
+                "5": 13.0,
+                "6": 13.0,
+                "7": 13.0,
+                "8": 13.0
             },
-            "distance": 13.0,
             "increment": 0.0,
             "presses": 1,
-            "speed": 5
+            "speedByTipCount": {
+                "1": 10.0,
+                "2": 10.0,
+                "3": 10.0,
+                "4": 10.0,
+                "5": 10.0,
+                "6": 10.0,
+                "7": 10.0,
+                "8": 10.0
+            }
         }
     },
     "plungerHomingConfigurations": {
         "current": 1.0,
         "speed": 30
     },
     "plungerMotorConfigurations": {
         "idle": 0.3,
         "run": 1.0
     },
     "plungerPositionsConfigurations": {
         "default": {
             "blowout": 76.5,
             "bottom": 71.5,
-            "drop": 90.5,
-            "top": 0.5
+            "drop": 91.5,
+            "top": 0.0
+        },
+        "lowVolumeDefault": {
+            "blowout": 76.5,
+            "bottom": 61.5,
+            "drop": 91.5,
+            "top": 0.0
         }
     },
     "quirks": [],
-    "shaftDiameter": 4.5,
-    "shaftULperMM": 15.904
+    "shaftDiameter": 1.0,
+    "shaftULperMM": 0.785
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p1000/3_3.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p50/3_5.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8086265756302521%*

 * *Differences: {"'availableSensors'": "{'pressure': {'count': 2}, 'capacitive': {'count': 2}}",*

 * * "'channels'": '8',*

 * * "'displayName'": "'Flex 8-Channel 50 μL'",*

 * * "'model'": "'p50'",*

 * * "'partialTipConfigurations'": "{'partialTipSupported': True, 'availableConfigurations': [1, 2, 3, "*

 * *                               '4, 5, 6, 7, 8]}',*

 * * "'pickUpTipConfigurations'": "{'pressFit': {'currentByTipCount': {'1': 0.2, '2': 0.14, '3': 0.2, "*

 * *                              "'4': 0.28, '5': 0.34, '6': 0.41, '7': 0.48, '8': 0.55}, "*

 * *       […]*

```diff
@@ -1,65 +1,105 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipettePropertiesSchema.json",
     "availableSensors": {
         "capacitive": {
-            "count": 1
+            "count": 2
         },
         "environment": {
             "count": 1
         },
         "pressure": {
-            "count": 1
+            "count": 2
         },
         "sensors": [
             "pressure",
             "capacitive",
             "environment"
         ]
     },
     "backCompatNames": [],
     "backlashDistance": 0.1,
-    "channels": 1,
+    "channels": 8,
     "displayCategory": "FLEX",
-    "displayName": "Flex 1-Channel 1000 \u03bcL",
+    "displayName": "Flex 8-Channel 50 \u03bcL",
     "dropTipConfigurations": {
         "plungerEject": {
             "current": 1.0,
             "speed": 10
         }
     },
-    "model": "p1000",
+    "model": "p50",
     "partialTipConfigurations": {
-        "availableConfigurations": null,
-        "partialTipSupported": false
+        "availableConfigurations": [
+            1,
+            2,
+            3,
+            4,
+            5,
+            6,
+            7,
+            8
+        ],
+        "partialTipSupported": true
     },
     "pickUpTipConfigurations": {
         "pressFit": {
             "currentByTipCount": {
-                "1": 0.15
+                "1": 0.2,
+                "2": 0.14,
+                "3": 0.2,
+                "4": 0.28,
+                "5": 0.34,
+                "6": 0.41,
+                "7": 0.48,
+                "8": 0.55
+            },
+            "distanceByTipCount": {
+                "1": 13.0,
+                "2": 13.0,
+                "3": 13.0,
+                "4": 13.0,
+                "5": 13.0,
+                "6": 13.0,
+                "7": 13.0,
+                "8": 13.0
             },
-            "distance": 13.0,
             "increment": 0.0,
             "presses": 1,
-            "speed": 5
+            "speedByTipCount": {
+                "1": 10.0,
+                "2": 10.0,
+                "3": 10.0,
+                "4": 10.0,
+                "5": 10.0,
+                "6": 10.0,
+                "7": 10.0,
+                "8": 10.0
+            }
         }
     },
     "plungerHomingConfigurations": {
         "current": 1.0,
         "speed": 30
     },
     "plungerMotorConfigurations": {
         "idle": 0.3,
         "run": 1.0
     },
     "plungerPositionsConfigurations": {
         "default": {
             "blowout": 76.5,
             "bottom": 71.5,
-            "drop": 90.5,
-            "top": 0.5
+            "drop": 91.5,
+            "top": 0.0
+        },
+        "lowVolumeDefault": {
+            "blowout": 76.5,
+            "bottom": 61.5,
+            "drop": 91.5,
+            "top": 0.0
         }
     },
     "quirks": [],
-    "shaftDiameter": 4.5,
-    "shaftULperMM": 15.904
+    "shaftDiameter": 1.0,
+    "shaftULperMM": 0.785
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p1000/3_4.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p20/2_2.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7521008403361344%*

 * *Differences: {"'availableSensors'": "{'sensors': [], delete: ['pressure', 'capacitive', 'environment']}",*

 * * "'backCompatNames'": "['p10_single']",*

 * * "'backlashDistance'": '0.0',*

 * * "'displayCategory'": "'GEN2'",*

 * * "'displayName'": "'P20 Single-Channel GEN2'",*

 * * "'model'": "'p20'",*

 * * "'pickUpTipConfigurations'": "{'pressFit': {'currentByTipCount': {'1': 0.1}, 'speedByTipCount': "*

 * *                              "OrderedDict([('1', 10.0)]), 'distanceByTipCount': "*

 * *                              "OrderedDict([('1', 14.0)]), delete:  […]*

```diff
@@ -1,65 +1,58 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipettePropertiesSchema.json",
     "availableSensors": {
-        "capacitive": {
-            "count": 1
-        },
-        "environment": {
-            "count": 1
-        },
-        "pressure": {
-            "count": 1
-        },
-        "sensors": [
-            "pressure",
-            "capacitive",
-            "environment"
-        ]
+        "sensors": []
     },
-    "backCompatNames": [],
-    "backlashDistance": 0.1,
+    "backCompatNames": [
+        "p10_single"
+    ],
+    "backlashDistance": 0.0,
     "channels": 1,
-    "displayCategory": "FLEX",
-    "displayName": "Flex 1-Channel 1000 \u03bcL",
+    "displayCategory": "GEN2",
+    "displayName": "P20 Single-Channel GEN2",
     "dropTipConfigurations": {
         "plungerEject": {
             "current": 1.0,
-            "speed": 15
+            "speed": 15.0
         }
     },
-    "model": "p1000",
+    "model": "p20",
     "partialTipConfigurations": {
         "availableConfigurations": null,
         "partialTipSupported": false
     },
     "pickUpTipConfigurations": {
         "pressFit": {
             "currentByTipCount": {
-                "1": 0.2
+                "1": 0.1
+            },
+            "distanceByTipCount": {
+                "1": 14.0
             },
-            "distance": 13.0,
             "increment": 0.0,
             "presses": 1,
-            "speed": 10
+            "speedByTipCount": {
+                "1": 10.0
+            }
         }
     },
     "plungerHomingConfigurations": {
         "current": 1.0,
         "speed": 30
     },
     "plungerMotorConfigurations": {
         "idle": 0.3,
         "run": 1.0
     },
     "plungerPositionsConfigurations": {
         "default": {
-            "blowout": 76.5,
-            "bottom": 71.5,
-            "drop": 90.5,
-            "top": 0.0
+            "blowout": -13.0,
+            "bottom": -8.5,
+            "drop": -27.0,
+            "top": 19.5
         }
     },
     "quirks": [],
-    "shaftDiameter": 4.5,
-    "shaftULperMM": 15.904
+    "shaftDiameter": 1.0,
+    "shaftULperMM": 0.785
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p1000/3_5.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p20/2_0.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7447478991596638%*

 * *Differences: {"'availableSensors'": "{'sensors': [], delete: ['pressure', 'capacitive', 'environment']}",*

 * * "'backCompatNames'": "['p10_single']",*

 * * "'backlashDistance'": '0.0',*

 * * "'displayCategory'": "'GEN2'",*

 * * "'displayName'": "'P20 Single-Channel GEN2'",*

 * * "'model'": "'p20'",*

 * * "'pickUpTipConfigurations'": "{'pressFit': {'currentByTipCount': {'1': 0.1}, 'speedByTipCount': "*

 * *                              "OrderedDict([('1', 10.0)]), 'distanceByTipCount': "*

 * *                              "OrderedDict([('1', 14.0)]), delete:  […]*

```diff
@@ -1,65 +1,58 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipettePropertiesSchema.json",
     "availableSensors": {
-        "capacitive": {
-            "count": 1
-        },
-        "environment": {
-            "count": 1
-        },
-        "pressure": {
-            "count": 1
-        },
-        "sensors": [
-            "pressure",
-            "capacitive",
-            "environment"
-        ]
+        "sensors": []
     },
-    "backCompatNames": [],
-    "backlashDistance": 0.1,
+    "backCompatNames": [
+        "p10_single"
+    ],
+    "backlashDistance": 0.0,
     "channels": 1,
-    "displayCategory": "FLEX",
-    "displayName": "Flex 1-Channel 1000 \u03bcL",
+    "displayCategory": "GEN2",
+    "displayName": "P20 Single-Channel GEN2",
     "dropTipConfigurations": {
         "plungerEject": {
             "current": 1.0,
-            "speed": 15
+            "speed": 15.0
         }
     },
-    "model": "p1000",
+    "model": "p20",
     "partialTipConfigurations": {
         "availableConfigurations": null,
         "partialTipSupported": false
     },
     "pickUpTipConfigurations": {
         "pressFit": {
             "currentByTipCount": {
-                "1": 0.2
+                "1": 0.1
+            },
+            "distanceByTipCount": {
+                "1": 14.0
             },
-            "distance": 13.0,
             "increment": 0.0,
             "presses": 1,
-            "speed": 10
+            "speedByTipCount": {
+                "1": 10.0
+            }
         }
     },
     "plungerHomingConfigurations": {
         "current": 1.0,
         "speed": 30
     },
     "plungerMotorConfigurations": {
-        "idle": 0.3,
+        "idle": 0.05,
         "run": 1.0
     },
     "plungerPositionsConfigurations": {
         "default": {
-            "blowout": 76.5,
-            "bottom": 71.5,
-            "drop": 90.5,
-            "top": 0.0
+            "blowout": -13.0,
+            "bottom": -8.5,
+            "drop": -27.0,
+            "top": 19.5
         }
     },
     "quirks": [],
-    "shaftDiameter": 4.5,
-    "shaftULperMM": 15.904
+    "shaftDiameter": 1.0,
+    "shaftULperMM": 0.785
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p1000/3_6.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p300/2_1.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7447478991596638%*

 * *Differences: {"'availableSensors'": "{'sensors': [], delete: ['pressure', 'capacitive', 'environment']}",*

 * * "'backCompatNames'": "['p300_single']",*

 * * "'backlashDistance'": '0.0',*

 * * "'displayCategory'": "'GEN2'",*

 * * "'displayName'": "'P300 Single-Channel GEN2'",*

 * * "'dropTipConfigurations'": "{'plungerEject': {'current': 1.25, 'speed': 7.0}}",*

 * * "'model'": "'p300'",*

 * * "'pickUpTipConfigurations'": "{'pressFit': {'currentByTipCount': {'1': 0.125}, 'speedByTipCount': "*

 * *                              "OrderedDict([('1', 10.0)]), 'dist […]*

```diff
@@ -1,65 +1,58 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipettePropertiesSchema.json",
     "availableSensors": {
-        "capacitive": {
-            "count": 1
-        },
-        "environment": {
-            "count": 1
-        },
-        "pressure": {
-            "count": 1
-        },
-        "sensors": [
-            "pressure",
-            "capacitive",
-            "environment"
-        ]
+        "sensors": []
     },
-    "backCompatNames": [],
-    "backlashDistance": 0.1,
+    "backCompatNames": [
+        "p300_single"
+    ],
+    "backlashDistance": 0.0,
     "channels": 1,
-    "displayCategory": "FLEX",
-    "displayName": "Flex 1-Channel 1000 \u03bcL",
+    "displayCategory": "GEN2",
+    "displayName": "P300 Single-Channel GEN2",
     "dropTipConfigurations": {
         "plungerEject": {
-            "current": 1.0,
-            "speed": 15
+            "current": 1.25,
+            "speed": 7.0
         }
     },
-    "model": "p1000",
+    "model": "p300",
     "partialTipConfigurations": {
         "availableConfigurations": null,
         "partialTipSupported": false
     },
     "pickUpTipConfigurations": {
         "pressFit": {
             "currentByTipCount": {
-                "1": 0.2
+                "1": 0.125
+            },
+            "distanceByTipCount": {
+                "1": 17.0
             },
-            "distance": 13.0,
             "increment": 0.0,
             "presses": 1,
-            "speed": 10
+            "speedByTipCount": {
+                "1": 10.0
+            }
         }
     },
     "plungerHomingConfigurations": {
         "current": 1.0,
         "speed": 30
     },
     "plungerMotorConfigurations": {
         "idle": 0.3,
         "run": 1.0
     },
     "plungerPositionsConfigurations": {
         "default": {
-            "blowout": 76.5,
-            "bottom": 71.5,
-            "drop": 90.5,
-            "top": 0.0
+            "blowout": -19.0,
+            "bottom": -14.5,
+            "drop": -37.0,
+            "top": 19.5
         }
     },
     "quirks": [],
-    "shaftDiameter": 4.5,
-    "shaftULperMM": 15.904
+    "shaftDiameter": 3.5,
+    "shaftULperMM": 9.621
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p20/2_0.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p10/1_6.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7698266806722689%*

 * *Differences: {"'backCompatNames'": '[]',*

 * * "'channels'": '8',*

 * * "'displayCategory'": "'GEN1'",*

 * * "'displayName'": "'P10 8-Channel GEN1'",*

 * * "'dropTipConfigurations'": "{'plungerEject': {'current': 0.5, 'speed': 5.0}}",*

 * * "'model'": "'p10'",*

 * * "'partialTipConfigurations'": "{'partialTipSupported': True, 'availableConfigurations': [1, 2, 3, "*

 * *                               '4, 5, 6, 7, 8]}',*

 * * "'pickUpTipConfigurations'": "{'pressFit': {'presses': 3, 'increment': 3.0, 'currentByTipCount': "*

 * *                              "{'2': 0 […]*

```diff
@@ -1,54 +1,89 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipettePropertiesSchema.json",
     "availableSensors": {
         "sensors": []
     },
-    "backCompatNames": [
-        "p10_single"
-    ],
+    "backCompatNames": [],
     "backlashDistance": 0.0,
-    "channels": 1,
-    "displayCategory": "GEN2",
-    "displayName": "P20 Single-Channel GEN2",
+    "channels": 8,
+    "displayCategory": "GEN1",
+    "displayName": "P10 8-Channel GEN1",
     "dropTipConfigurations": {
         "plungerEject": {
-            "current": 1.0,
-            "speed": 15.0
+            "current": 0.5,
+            "speed": 5.0
         }
     },
-    "model": "p20",
+    "model": "p10",
     "partialTipConfigurations": {
-        "availableConfigurations": null,
-        "partialTipSupported": false
+        "availableConfigurations": [
+            1,
+            2,
+            3,
+            4,
+            5,
+            6,
+            7,
+            8
+        ],
+        "partialTipSupported": true
     },
     "pickUpTipConfigurations": {
         "pressFit": {
             "currentByTipCount": {
-                "1": 0.1
+                "1": 0.1,
+                "2": 0.14,
+                "3": 0.21,
+                "4": 0.28,
+                "5": 0.34,
+                "6": 0.41,
+                "7": 0.48,
+                "8": 0.55
+            },
+            "distanceByTipCount": {
+                "1": 10.0,
+                "2": 10.0,
+                "3": 10.0,
+                "4": 10.0,
+                "5": 10.0,
+                "6": 10.0,
+                "7": 10.0,
+                "8": 10.0
             },
-            "distance": 14.0,
-            "increment": 0.0,
-            "presses": 1,
-            "speed": 10.0
+            "increment": 3.0,
+            "presses": 3,
+            "speedByTipCount": {
+                "1": 30.0,
+                "2": 30.0,
+                "3": 30.0,
+                "4": 30.0,
+                "5": 30.0,
+                "6": 30.0,
+                "7": 30.0,
+                "8": 30.0
+            }
         }
     },
     "plungerHomingConfigurations": {
-        "current": 1.0,
+        "current": 0.5,
         "speed": 30
     },
     "plungerMotorConfigurations": {
         "idle": 0.05,
-        "run": 1.0
+        "run": 0.5
     },
     "plungerPositionsConfigurations": {
         "default": {
-            "blowout": -13.0,
-            "bottom": -8.5,
-            "drop": -27.0,
+            "blowout": -1.0,
+            "bottom": 2.0,
+            "drop": -4.5,
             "top": 19.5
         }
     },
-    "quirks": [],
+    "quirks": [
+        "dropTipShake",
+        "doubleDropTip"
+    ],
     "shaftDiameter": 1.0,
     "shaftULperMM": 0.785
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p20/2_1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p50/1_4.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7036502100840336%*

 * *Differences: {"'backCompatNames'": '[]',*

 * * "'channels'": '8',*

 * * "'displayCategory'": "'GEN1'",*

 * * "'displayName'": "'P50 8-Channel GEN1'",*

 * * "'dropTipConfigurations'": "{'plungerEject': {'current': 0.5, 'speed': 5.0}}",*

 * * "'model'": "'p50'",*

 * * "'partialTipConfigurations'": "{'partialTipSupported': True, 'availableConfigurations': [1, 2, 3, "*

 * *                               '4, 5, 6, 7, 8]}',*

 * * "'pickUpTipConfigurations'": "{'pressFit': {'presses': 3, 'increment': 1.0, 'currentByTipCount': "*

 * *                              "{'2': 0 […]*

```diff
@@ -1,54 +1,88 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipettePropertiesSchema.json",
     "availableSensors": {
         "sensors": []
     },
-    "backCompatNames": [
-        "p10_single"
-    ],
+    "backCompatNames": [],
     "backlashDistance": 0.0,
-    "channels": 1,
-    "displayCategory": "GEN2",
-    "displayName": "P20 Single-Channel GEN2",
+    "channels": 8,
+    "displayCategory": "GEN1",
+    "displayName": "P50 8-Channel GEN1",
     "dropTipConfigurations": {
         "plungerEject": {
-            "current": 1.0,
-            "speed": 15.0
+            "current": 0.5,
+            "speed": 5.0
         }
     },
-    "model": "p20",
+    "model": "p50",
     "partialTipConfigurations": {
-        "availableConfigurations": null,
-        "partialTipSupported": false
+        "availableConfigurations": [
+            1,
+            2,
+            3,
+            4,
+            5,
+            6,
+            7,
+            8
+        ],
+        "partialTipSupported": true
     },
     "pickUpTipConfigurations": {
         "pressFit": {
             "currentByTipCount": {
-                "1": 0.1
+                "1": 0.1,
+                "2": 0.15,
+                "3": 0.23,
+                "4": 0.3,
+                "5": 0.38,
+                "6": 0.45,
+                "7": 0.53,
+                "8": 0.6
+            },
+            "distanceByTipCount": {
+                "1": 10.0,
+                "2": 10.0,
+                "3": 10.0,
+                "4": 10.0,
+                "5": 10.0,
+                "6": 10.0,
+                "7": 10.0,
+                "8": 10.0
             },
-            "distance": 14.0,
-            "increment": 0.0,
-            "presses": 1,
-            "speed": 10.0
+            "increment": 1.0,
+            "presses": 3,
+            "speedByTipCount": {
+                "1": 30.0,
+                "2": 30.0,
+                "3": 30.0,
+                "4": 30.0,
+                "5": 30.0,
+                "6": 30.0,
+                "7": 30.0,
+                "8": 30.0
+            }
         }
     },
     "plungerHomingConfigurations": {
-        "current": 1.0,
+        "current": 0.5,
         "speed": 30
     },
     "plungerMotorConfigurations": {
-        "idle": 0.3,
-        "run": 1.0
+        "idle": 0.05,
+        "run": 0.5
     },
     "plungerPositionsConfigurations": {
         "default": {
-            "blowout": -13.0,
-            "bottom": -8.5,
-            "drop": -27.0,
+            "blowout": 0.5,
+            "bottom": 2.0,
+            "drop": -4.0,
             "top": 19.5
         }
     },
-    "quirks": [],
-    "shaftDiameter": 1.0,
-    "shaftULperMM": 0.785
+    "quirks": [
+        "dropTipShake"
+    ],
+    "shaftDiameter": 2.0,
+    "shaftULperMM": 3.142
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p20/2_2.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p50/1_3.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7036502100840336%*

 * *Differences: {"'backCompatNames'": '[]',*

 * * "'channels'": '8',*

 * * "'displayCategory'": "'GEN1'",*

 * * "'displayName'": "'P50 8-Channel GEN1'",*

 * * "'dropTipConfigurations'": "{'plungerEject': {'current': 0.5, 'speed': 5.0}}",*

 * * "'model'": "'p50'",*

 * * "'partialTipConfigurations'": "{'partialTipSupported': True, 'availableConfigurations': [1, 2, 3, "*

 * *                               '4, 5, 6, 7, 8]}',*

 * * "'pickUpTipConfigurations'": "{'pressFit': {'presses': 3, 'increment': 1.0, 'currentByTipCount': "*

 * *                              "{'2': 0 […]*

```diff
@@ -1,54 +1,88 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipettePropertiesSchema.json",
     "availableSensors": {
         "sensors": []
     },
-    "backCompatNames": [
-        "p10_single"
-    ],
+    "backCompatNames": [],
     "backlashDistance": 0.0,
-    "channels": 1,
-    "displayCategory": "GEN2",
-    "displayName": "P20 Single-Channel GEN2",
+    "channels": 8,
+    "displayCategory": "GEN1",
+    "displayName": "P50 8-Channel GEN1",
     "dropTipConfigurations": {
         "plungerEject": {
-            "current": 1.0,
-            "speed": 15.0
+            "current": 0.5,
+            "speed": 5.0
         }
     },
-    "model": "p20",
+    "model": "p50",
     "partialTipConfigurations": {
-        "availableConfigurations": null,
-        "partialTipSupported": false
+        "availableConfigurations": [
+            1,
+            2,
+            3,
+            4,
+            5,
+            6,
+            7,
+            8
+        ],
+        "partialTipSupported": true
     },
     "pickUpTipConfigurations": {
         "pressFit": {
             "currentByTipCount": {
-                "1": 0.1
+                "1": 0.1,
+                "2": 0.15,
+                "3": 0.23,
+                "4": 0.3,
+                "5": 0.38,
+                "6": 0.45,
+                "7": 0.53,
+                "8": 0.6
+            },
+            "distanceByTipCount": {
+                "1": 10.0,
+                "2": 10.0,
+                "3": 10.0,
+                "4": 10.0,
+                "5": 10.0,
+                "6": 10.0,
+                "7": 10.0,
+                "8": 10.0
             },
-            "distance": 14.0,
-            "increment": 0.0,
-            "presses": 1,
-            "speed": 10.0
+            "increment": 1.0,
+            "presses": 3,
+            "speedByTipCount": {
+                "1": 30.0,
+                "2": 30.0,
+                "3": 30.0,
+                "4": 30.0,
+                "5": 30.0,
+                "6": 30.0,
+                "7": 30.0,
+                "8": 30.0
+            }
         }
     },
     "plungerHomingConfigurations": {
-        "current": 1.0,
+        "current": 0.5,
         "speed": 30
     },
     "plungerMotorConfigurations": {
-        "idle": 0.3,
-        "run": 1.0
+        "idle": 0.05,
+        "run": 0.5
     },
     "plungerPositionsConfigurations": {
         "default": {
-            "blowout": -13.0,
-            "bottom": -8.5,
-            "drop": -27.0,
+            "blowout": 0.5,
+            "bottom": 2.0,
+            "drop": -5.0,
             "top": 19.5
         }
     },
-    "quirks": [],
-    "shaftDiameter": 1.0,
-    "shaftULperMM": 0.785
+    "quirks": [
+        "dropTipShake"
+    ],
+    "shaftDiameter": 2.0,
+    "shaftULperMM": 3.142
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p300/1_0.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p50/1_5.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7947741596638656%*

 * *Differences: {"'channels'": '8',*

 * * "'displayName'": "'P50 8-Channel GEN1'",*

 * * "'model'": "'p50'",*

 * * "'partialTipConfigurations'": "{'partialTipSupported': True, 'availableConfigurations': [1, 2, 3, "*

 * *                               '4, 5, 6, 7, 8]}',*

 * * "'pickUpTipConfigurations'": "{'pressFit': {'increment': 3.0, 'currentByTipCount': {'2': 0.2, "*

 * *                              "'3': 0.3, '4': 0.4, '5': 0.5, '6': 0.6, '7': 0.7, '8': 0.8}, "*

 * *                              "'speedByTipCount': OrderedDict([('1', 30.0), ('2', 30.0) […]*

```diff
@@ -1,54 +1,89 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipettePropertiesSchema.json",
     "availableSensors": {
         "sensors": []
     },
     "backCompatNames": [],
     "backlashDistance": 0.0,
-    "channels": 1,
+    "channels": 8,
     "displayCategory": "GEN1",
-    "displayName": "P300 Single-Channel GEN1",
+    "displayName": "P50 8-Channel GEN1",
     "dropTipConfigurations": {
         "plungerEject": {
             "current": 0.5,
             "speed": 5.0
         }
     },
-    "model": "p300",
+    "model": "p50",
     "partialTipConfigurations": {
-        "availableConfigurations": null,
-        "partialTipSupported": false
+        "availableConfigurations": [
+            1,
+            2,
+            3,
+            4,
+            5,
+            6,
+            7,
+            8
+        ],
+        "partialTipSupported": true
     },
     "pickUpTipConfigurations": {
         "pressFit": {
             "currentByTipCount": {
-                "1": 0.1
+                "1": 0.1,
+                "2": 0.2,
+                "3": 0.3,
+                "4": 0.4,
+                "5": 0.5,
+                "6": 0.6,
+                "7": 0.7,
+                "8": 0.8
             },
-            "distance": 10.0,
-            "increment": 1.0,
+            "distanceByTipCount": {
+                "1": 10.0,
+                "2": 10.0,
+                "3": 10.0,
+                "4": 10.0,
+                "5": 10.0,
+                "6": 10.0,
+                "7": 10.0,
+                "8": 10.0
+            },
+            "increment": 3.0,
             "presses": 3,
-            "speed": 30.0
+            "speedByTipCount": {
+                "1": 30.0,
+                "2": 30.0,
+                "3": 30.0,
+                "4": 30.0,
+                "5": 30.0,
+                "6": 30.0,
+                "7": 30.0,
+                "8": 30.0
+            }
         }
     },
     "plungerHomingConfigurations": {
-        "current": 0.3,
+        "current": 0.5,
         "speed": 30
     },
     "plungerMotorConfigurations": {
         "idle": 0.05,
-        "run": 0.3
+        "run": 0.5
     },
     "plungerPositionsConfigurations": {
         "default": {
-            "blowout": 0.0,
-            "bottom": 1.5,
+            "blowout": 0.5,
+            "bottom": 2.0,
             "drop": -4.0,
             "top": 19.5
         }
     },
     "quirks": [
+        "doubleDropTip",
         "dropTipShake"
     ],
-    "shaftDiameter": 5.0,
-    "shaftULperMM": 19.635
+    "shaftDiameter": 2.0,
+    "shaftULperMM": 3.142
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p300/1_3.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p20/2_0.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7036502100840336%*

 * *Differences: {"'backCompatNames'": "['p10_multi']",*

 * * "'channels'": '8',*

 * * "'displayCategory'": "'GEN2'",*

 * * "'displayName'": "'P20 8-Channel GEN2'",*

 * * "'dropTipConfigurations'": "{'plungerEject': {'current': 1.25, 'speed': 15.0}}",*

 * * "'model'": "'p20'",*

 * * "'partialTipConfigurations'": "{'partialTipSupported': True, 'availableConfigurations': [1, 2, 3, "*

 * *                               '4, 5, 6, 7, 8]}',*

 * * "'pickUpTipConfigurations'": "{'pressFit': {'presses': 1, 'increment': 0.0, 'currentByTipCount': "*

 * *                          […]*

```diff
@@ -1,54 +1,88 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipettePropertiesSchema.json",
     "availableSensors": {
         "sensors": []
     },
-    "backCompatNames": [],
+    "backCompatNames": [
+        "p10_multi"
+    ],
     "backlashDistance": 0.0,
-    "channels": 1,
-    "displayCategory": "GEN1",
-    "displayName": "P300 Single-Channel GEN1",
+    "channels": 8,
+    "displayCategory": "GEN2",
+    "displayName": "P20 8-Channel GEN2",
     "dropTipConfigurations": {
         "plungerEject": {
-            "current": 0.5,
-            "speed": 5.0
+            "current": 1.25,
+            "speed": 15.0
         }
     },
-    "model": "p300",
+    "model": "p20",
     "partialTipConfigurations": {
-        "availableConfigurations": null,
-        "partialTipSupported": false
+        "availableConfigurations": [
+            1,
+            2,
+            3,
+            4,
+            5,
+            6,
+            7,
+            8
+        ],
+        "partialTipSupported": true
     },
     "pickUpTipConfigurations": {
         "pressFit": {
             "currentByTipCount": {
-                "1": 0.1
+                "1": 0.1,
+                "2": 0.15,
+                "3": 0.23,
+                "4": 0.28,
+                "5": 0.38,
+                "6": 0.45,
+                "7": 0.53,
+                "8": 0.6
+            },
+            "distanceByTipCount": {
+                "1": 11.0,
+                "2": 11.0,
+                "3": 11.0,
+                "4": 11.0,
+                "5": 11.0,
+                "6": 11.0,
+                "7": 11.0,
+                "8": 11.0
             },
-            "distance": 10.0,
-            "increment": 1.0,
-            "presses": 3,
-            "speed": 30.0
+            "increment": 0.0,
+            "presses": 1,
+            "speedByTipCount": {
+                "1": 10.0,
+                "2": 10.0,
+                "3": 10.0,
+                "4": 10.0,
+                "5": 10.0,
+                "6": 10.0,
+                "7": 10.0,
+                "8": 10.0
+            }
         }
     },
     "plungerHomingConfigurations": {
-        "current": 0.3,
+        "current": 1.0,
         "speed": 30
     },
     "plungerMotorConfigurations": {
-        "idle": 0.05,
-        "run": 0.3
+        "idle": 0.3,
+        "run": 1.0
     },
     "plungerPositionsConfigurations": {
         "default": {
-            "blowout": -1.5,
-            "bottom": 1.5,
-            "drop": -5.5,
+            "blowout": -13.0,
+            "bottom": -8.5,
+            "drop": -31.6,
             "top": 19.5
         }
     },
-    "quirks": [
-        "dropTipShake"
-    ],
-    "shaftDiameter": 5.0,
-    "shaftULperMM": 19.635
+    "quirks": [],
+    "shaftDiameter": 1.0,
+    "shaftULperMM": 0.785
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p300/1_4.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p20/2_1.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7036502100840336%*

 * *Differences: {"'backCompatNames'": "['p10_multi']",*

 * * "'channels'": '8',*

 * * "'displayCategory'": "'GEN2'",*

 * * "'displayName'": "'P20 8-Channel GEN2'",*

 * * "'dropTipConfigurations'": "{'plungerEject': {'current': 1.25, 'speed': 15.0}}",*

 * * "'model'": "'p20'",*

 * * "'partialTipConfigurations'": "{'partialTipSupported': True, 'availableConfigurations': [1, 2, 3, "*

 * *                               '4, 5, 6, 7, 8]}',*

 * * "'pickUpTipConfigurations'": "{'pressFit': {'presses': 1, 'increment': 0.0, 'currentByTipCount': "*

 * *                          […]*

```diff
@@ -1,54 +1,88 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipettePropertiesSchema.json",
     "availableSensors": {
         "sensors": []
     },
-    "backCompatNames": [],
+    "backCompatNames": [
+        "p10_multi"
+    ],
     "backlashDistance": 0.0,
-    "channels": 1,
-    "displayCategory": "GEN1",
-    "displayName": "P300 Single-Channel GEN1",
+    "channels": 8,
+    "displayCategory": "GEN2",
+    "displayName": "P20 8-Channel GEN2",
     "dropTipConfigurations": {
         "plungerEject": {
-            "current": 0.5,
-            "speed": 5.0
+            "current": 1.25,
+            "speed": 15.0
         }
     },
-    "model": "p300",
+    "model": "p20",
     "partialTipConfigurations": {
-        "availableConfigurations": null,
-        "partialTipSupported": false
+        "availableConfigurations": [
+            1,
+            2,
+            3,
+            4,
+            5,
+            6,
+            7,
+            8
+        ],
+        "partialTipSupported": true
     },
     "pickUpTipConfigurations": {
         "pressFit": {
             "currentByTipCount": {
-                "1": 0.1
+                "1": 0.1,
+                "2": 0.15,
+                "3": 0.23,
+                "4": 0.28,
+                "5": 0.38,
+                "6": 0.45,
+                "7": 0.53,
+                "8": 0.6
+            },
+            "distanceByTipCount": {
+                "1": 11.0,
+                "2": 11.0,
+                "3": 11.0,
+                "4": 11.0,
+                "5": 11.0,
+                "6": 11.0,
+                "7": 11.0,
+                "8": 11.0
             },
-            "distance": 10.0,
-            "increment": 1.0,
-            "presses": 3,
-            "speed": 30.0
+            "increment": 0.0,
+            "presses": 1,
+            "speedByTipCount": {
+                "1": 10.0,
+                "2": 10.0,
+                "3": 10.0,
+                "4": 10.0,
+                "5": 10.0,
+                "6": 10.0,
+                "7": 10.0,
+                "8": 10.0
+            }
         }
     },
     "plungerHomingConfigurations": {
-        "current": 0.3,
+        "current": 1.0,
         "speed": 30
     },
     "plungerMotorConfigurations": {
-        "idle": 0.05,
-        "run": 0.3
+        "idle": 0.3,
+        "run": 1.0
     },
     "plungerPositionsConfigurations": {
         "default": {
-            "blowout": 0.0,
-            "bottom": 3.0,
-            "drop": -4.5,
+            "blowout": -13.0,
+            "bottom": -8.5,
+            "drop": -31.6,
             "top": 19.5
         }
     },
-    "quirks": [
-        "dropTipShake"
-    ],
-    "shaftDiameter": 5.0,
-    "shaftULperMM": 19.635
+    "quirks": [],
+    "shaftDiameter": 1.0,
+    "shaftULperMM": 0.785
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p300/1_5.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p300/1_0.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8969275210084033%*

 * *Differences: {"'channels'": '8',*

 * * "'displayName'": "'P300 8-Channel GEN1'",*

 * * "'partialTipConfigurations'": "{'partialTipSupported': True, 'availableConfigurations': [1, 2, 3, "*

 * *                               '4, 5, 6, 7, 8]}',*

 * * "'pickUpTipConfigurations'": "{'pressFit': {'currentByTipCount': {'2': 0.15, '3': 0.23, '4': 0.3, "*

 * *                              "'5': 0.38, '6': 0.45, '7': 0.53, '8': 0.6}, 'speedByTipCount': "*

 * *                              "OrderedDict([('1', 30.0), ('2', 30.0), ('3', 30.0), ('4', 30.0), "*

 * *    […]*

```diff
@@ -1,52 +1,86 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipettePropertiesSchema.json",
     "availableSensors": {
         "sensors": []
     },
     "backCompatNames": [],
     "backlashDistance": 0.0,
-    "channels": 1,
+    "channels": 8,
     "displayCategory": "GEN1",
-    "displayName": "P300 Single-Channel GEN1",
+    "displayName": "P300 8-Channel GEN1",
     "dropTipConfigurations": {
         "plungerEject": {
             "current": 0.5,
             "speed": 5.0
         }
     },
     "model": "p300",
     "partialTipConfigurations": {
-        "availableConfigurations": null,
-        "partialTipSupported": false
+        "availableConfigurations": [
+            1,
+            2,
+            3,
+            4,
+            5,
+            6,
+            7,
+            8
+        ],
+        "partialTipSupported": true
     },
     "pickUpTipConfigurations": {
         "pressFit": {
             "currentByTipCount": {
-                "1": 0.1
+                "1": 0.1,
+                "2": 0.15,
+                "3": 0.23,
+                "4": 0.3,
+                "5": 0.38,
+                "6": 0.45,
+                "7": 0.53,
+                "8": 0.6
+            },
+            "distanceByTipCount": {
+                "1": 10.0,
+                "2": 10.0,
+                "3": 10.0,
+                "4": 10.0,
+                "5": 10.0,
+                "6": 10.0,
+                "7": 10.0,
+                "8": 10.0
             },
-            "distance": 10.0,
             "increment": 1.0,
             "presses": 3,
-            "speed": 30.0
+            "speedByTipCount": {
+                "1": 30.0,
+                "2": 30.0,
+                "3": 30.0,
+                "4": 30.0,
+                "5": 30.0,
+                "6": 30.0,
+                "7": 30.0,
+                "8": 30.0
+            }
         }
     },
     "plungerHomingConfigurations": {
-        "current": 0.3,
+        "current": 0.5,
         "speed": 30
     },
     "plungerMotorConfigurations": {
         "idle": 0.05,
-        "run": 0.3
+        "run": 0.5
     },
     "plungerPositionsConfigurations": {
         "default": {
-            "blowout": 0.0,
-            "bottom": 3.0,
-            "drop": -4.5,
+            "blowout": 3.0,
+            "bottom": 3.5,
+            "drop": -2.0,
             "top": 19.5
         }
     },
     "quirks": [
         "dropTipShake"
     ],
     "shaftDiameter": 5.0,
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p300/2_0.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p300/1_3.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7403492647058824%*

 * *Differences: {"'backCompatNames'": '[]',*

 * * "'channels'": '8',*

 * * "'displayCategory'": "'GEN1'",*

 * * "'displayName'": "'P300 8-Channel GEN1'",*

 * * "'dropTipConfigurations'": "{'plungerEject': {'current': 0.5, 'speed': 5.0}}",*

 * * "'partialTipConfigurations'": "{'partialTipSupported': True, 'availableConfigurations': [1, 2, 3, "*

 * *                               '4, 5, 6, 7, 8]}',*

 * * "'pickUpTipConfigurations'": "{'pressFit': {'presses': 3, 'increment': 1.0, 'currentByTipCount': "*

 * *                              "{'1': 0.1, '2': 0.15, '3':  […]*

```diff
@@ -1,54 +1,88 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipettePropertiesSchema.json",
     "availableSensors": {
         "sensors": []
     },
-    "backCompatNames": [
-        "p300_single"
-    ],
+    "backCompatNames": [],
     "backlashDistance": 0.0,
-    "channels": 1,
-    "displayCategory": "GEN2",
-    "displayName": "P300 Single-Channel GEN2",
+    "channels": 8,
+    "displayCategory": "GEN1",
+    "displayName": "P300 8-Channel GEN1",
     "dropTipConfigurations": {
         "plungerEject": {
-            "current": 1.25,
-            "speed": 7.0
+            "current": 0.5,
+            "speed": 5.0
         }
     },
     "model": "p300",
     "partialTipConfigurations": {
-        "availableConfigurations": null,
-        "partialTipSupported": false
+        "availableConfigurations": [
+            1,
+            2,
+            3,
+            4,
+            5,
+            6,
+            7,
+            8
+        ],
+        "partialTipSupported": true
     },
     "pickUpTipConfigurations": {
         "pressFit": {
             "currentByTipCount": {
-                "1": 0.125
+                "1": 0.1,
+                "2": 0.15,
+                "3": 0.23,
+                "4": 0.3,
+                "5": 0.38,
+                "6": 0.45,
+                "7": 0.53,
+                "8": 0.6
+            },
+            "distanceByTipCount": {
+                "1": 10.0,
+                "2": 10.0,
+                "3": 10.0,
+                "4": 10.0,
+                "5": 10.0,
+                "6": 10.0,
+                "7": 10.0,
+                "8": 10.0
             },
-            "distance": 17.0,
-            "increment": 0.0,
-            "presses": 1,
-            "speed": 10.0
+            "increment": 1.0,
+            "presses": 3,
+            "speedByTipCount": {
+                "1": 30.0,
+                "2": 30.0,
+                "3": 30.0,
+                "4": 30.0,
+                "5": 30.0,
+                "6": 30.0,
+                "7": 30.0,
+                "8": 30.0
+            }
         }
     },
     "plungerHomingConfigurations": {
-        "current": 1.0,
+        "current": 0.5,
         "speed": 30
     },
     "plungerMotorConfigurations": {
         "idle": 0.05,
-        "run": 1.0
+        "run": 0.5
     },
     "plungerPositionsConfigurations": {
         "default": {
-            "blowout": -19.0,
-            "bottom": -14.5,
-            "drop": -37.0,
+            "blowout": 1.5,
+            "bottom": 3.5,
+            "drop": -3.5,
             "top": 19.5
         }
     },
-    "quirks": [],
-    "shaftDiameter": 3.5,
-    "shaftULperMM": 9.621
+    "quirks": [
+        "dropTipShake"
+    ],
+    "shaftDiameter": 5.0,
+    "shaftULperMM": 19.635
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p300/2_1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p300/1_4.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7329963235294118%*

 * *Differences: {"'backCompatNames'": '[]',*

 * * "'channels'": '8',*

 * * "'displayCategory'": "'GEN1'",*

 * * "'displayName'": "'P300 8-Channel GEN1'",*

 * * "'dropTipConfigurations'": "{'plungerEject': {'current': 0.5, 'speed': 5.0}}",*

 * * "'partialTipConfigurations'": "{'partialTipSupported': True, 'availableConfigurations': [1, 2, 3, "*

 * *                               '4, 5, 6, 7, 8]}',*

 * * "'pickUpTipConfigurations'": "{'pressFit': {'presses': 3, 'increment': 1.0, 'currentByTipCount': "*

 * *                              "{'1': 0.1, '2': 0.15, '3':  […]*

```diff
@@ -1,54 +1,88 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipettePropertiesSchema.json",
     "availableSensors": {
         "sensors": []
     },
-    "backCompatNames": [
-        "p300_single"
-    ],
+    "backCompatNames": [],
     "backlashDistance": 0.0,
-    "channels": 1,
-    "displayCategory": "GEN2",
-    "displayName": "P300 Single-Channel GEN2",
+    "channels": 8,
+    "displayCategory": "GEN1",
+    "displayName": "P300 8-Channel GEN1",
     "dropTipConfigurations": {
         "plungerEject": {
-            "current": 1.25,
-            "speed": 7.0
+            "current": 0.5,
+            "speed": 5.0
         }
     },
     "model": "p300",
     "partialTipConfigurations": {
-        "availableConfigurations": null,
-        "partialTipSupported": false
+        "availableConfigurations": [
+            1,
+            2,
+            3,
+            4,
+            5,
+            6,
+            7,
+            8
+        ],
+        "partialTipSupported": true
     },
     "pickUpTipConfigurations": {
         "pressFit": {
             "currentByTipCount": {
-                "1": 0.125
+                "1": 0.1,
+                "2": 0.15,
+                "3": 0.23,
+                "4": 0.3,
+                "5": 0.38,
+                "6": 0.45,
+                "7": 0.53,
+                "8": 0.6
+            },
+            "distanceByTipCount": {
+                "1": 10.0,
+                "2": 10.0,
+                "3": 10.0,
+                "4": 10.0,
+                "5": 10.0,
+                "6": 10.0,
+                "7": 10.0,
+                "8": 10.0
             },
-            "distance": 17.0,
-            "increment": 0.0,
-            "presses": 1,
-            "speed": 10.0
+            "increment": 1.0,
+            "presses": 3,
+            "speedByTipCount": {
+                "1": 30.0,
+                "2": 30.0,
+                "3": 30.0,
+                "4": 30.0,
+                "5": 30.0,
+                "6": 30.0,
+                "7": 30.0,
+                "8": 30.0
+            }
         }
     },
     "plungerHomingConfigurations": {
-        "current": 1.0,
+        "current": 0.5,
         "speed": 30
     },
     "plungerMotorConfigurations": {
-        "idle": 0.3,
-        "run": 1.0
+        "idle": 0.05,
+        "run": 0.5
     },
     "plungerPositionsConfigurations": {
         "default": {
-            "blowout": -19.0,
-            "bottom": -14.5,
-            "drop": -37.0,
+            "blowout": 1.5,
+            "bottom": 3.5,
+            "drop": -3.5,
             "top": 19.5
         }
     },
-    "quirks": [],
-    "shaftDiameter": 3.5,
-    "shaftULperMM": 9.621
+    "quirks": [
+        "dropTipShake"
+    ],
+    "shaftDiameter": 5.0,
+    "shaftULperMM": 19.635
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p50/1_0.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p50/1_0.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8987657563025211%*

 * *Differences: {"'channels'": '8',*

 * * "'displayName'": "'P50 8-Channel GEN1'",*

 * * "'partialTipConfigurations'": "{'partialTipSupported': True, 'availableConfigurations': [1, 2, 3, "*

 * *                               '4, 5, 6, 7, 8]}',*

 * * "'pickUpTipConfigurations'": "{'pressFit': {'currentByTipCount': {'2': 0.15, '3': 0.23, '4': 0.3, "*

 * *                              "'5': 0.38, '6': 0.45, '7': 0.53, '8': 0.6}, 'speedByTipCount': "*

 * *                              "OrderedDict([('1', 30.0), ('2', 30.0), ('3', 30.0), ('4', 30.0), "*

 * *     […]*

```diff
@@ -1,52 +1,86 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipettePropertiesSchema.json",
     "availableSensors": {
         "sensors": []
     },
     "backCompatNames": [],
     "backlashDistance": 0.0,
-    "channels": 1,
+    "channels": 8,
     "displayCategory": "GEN1",
-    "displayName": "P50 Single-Channel GEN1",
+    "displayName": "P50 8-Channel GEN1",
     "dropTipConfigurations": {
         "plungerEject": {
             "current": 0.5,
             "speed": 5.0
         }
     },
     "model": "p50",
     "partialTipConfigurations": {
-        "availableConfigurations": null,
-        "partialTipSupported": false
+        "availableConfigurations": [
+            1,
+            2,
+            3,
+            4,
+            5,
+            6,
+            7,
+            8
+        ],
+        "partialTipSupported": true
     },
     "pickUpTipConfigurations": {
         "pressFit": {
             "currentByTipCount": {
-                "1": 0.1
+                "1": 0.1,
+                "2": 0.15,
+                "3": 0.23,
+                "4": 0.3,
+                "5": 0.38,
+                "6": 0.45,
+                "7": 0.53,
+                "8": 0.6
+            },
+            "distanceByTipCount": {
+                "1": 10.0,
+                "2": 10.0,
+                "3": 10.0,
+                "4": 10.0,
+                "5": 10.0,
+                "6": 10.0,
+                "7": 10.0,
+                "8": 10.0
             },
-            "distance": 10.0,
             "increment": 1.0,
             "presses": 3,
-            "speed": 30.0
+            "speedByTipCount": {
+                "1": 30.0,
+                "2": 30.0,
+                "3": 30.0,
+                "4": 30.0,
+                "5": 30.0,
+                "6": 30.0,
+                "7": 30.0,
+                "8": 30.0
+            }
         }
     },
     "plungerHomingConfigurations": {
-        "current": 0.3,
+        "current": 0.5,
         "speed": 30
     },
     "plungerMotorConfigurations": {
         "idle": 0.05,
-        "run": 0.3
+        "run": 0.5
     },
     "plungerPositionsConfigurations": {
         "default": {
             "blowout": 2.0,
-            "bottom": 2.01,
-            "drop": -4.5,
+            "bottom": 2.5,
+            "drop": -3.5,
             "top": 19.5
         }
     },
     "quirks": [
         "dropTipShake"
     ],
     "shaftDiameter": 2.0,
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p50/1_3.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p10/1_0.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.810530462184874%*

 * *Differences: {"'channels'": '8',*

 * * "'displayName'": "'P10 8-Channel GEN1'",*

 * * "'model'": "'p10'",*

 * * "'partialTipConfigurations'": "{'partialTipSupported': True, 'availableConfigurations': [1, 2, 3, "*

 * *                               '4, 5, 6, 7, 8]}',*

 * * "'pickUpTipConfigurations'": "{'pressFit': {'currentByTipCount': {'2': 0.1, '3': 0.15, '4': 0.2, "*

 * *                              "'5': 0.25, '6': 0.3, '7': 0.35, '8': 0.4}, 'speedByTipCount': "*

 * *                              "OrderedDict([('1', 30.0), ('2', 30.0), ('3', 30.0),  […]*

```diff
@@ -1,54 +1,88 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipettePropertiesSchema.json",
     "availableSensors": {
         "sensors": []
     },
     "backCompatNames": [],
     "backlashDistance": 0.0,
-    "channels": 1,
+    "channels": 8,
     "displayCategory": "GEN1",
-    "displayName": "P50 Single-Channel GEN1",
+    "displayName": "P10 8-Channel GEN1",
     "dropTipConfigurations": {
         "plungerEject": {
             "current": 0.5,
             "speed": 5.0
         }
     },
-    "model": "p50",
+    "model": "p10",
     "partialTipConfigurations": {
-        "availableConfigurations": null,
-        "partialTipSupported": false
+        "availableConfigurations": [
+            1,
+            2,
+            3,
+            4,
+            5,
+            6,
+            7,
+            8
+        ],
+        "partialTipSupported": true
     },
     "pickUpTipConfigurations": {
         "pressFit": {
             "currentByTipCount": {
-                "1": 0.1
+                "1": 0.1,
+                "2": 0.1,
+                "3": 0.15,
+                "4": 0.2,
+                "5": 0.25,
+                "6": 0.3,
+                "7": 0.35,
+                "8": 0.4
+            },
+            "distanceByTipCount": {
+                "1": 10.0,
+                "2": 10.0,
+                "3": 10.0,
+                "4": 10.0,
+                "5": 10.0,
+                "6": 10.0,
+                "7": 10.0,
+                "8": 10.0
             },
-            "distance": 10.0,
             "increment": 1.0,
             "presses": 3,
-            "speed": 30.0
+            "speedByTipCount": {
+                "1": 30.0,
+                "2": 30.0,
+                "3": 30.0,
+                "4": 30.0,
+                "5": 30.0,
+                "6": 30.0,
+                "7": 30.0,
+                "8": 30.0
+            }
         }
     },
     "plungerHomingConfigurations": {
-        "current": 0.3,
+        "current": 0.5,
         "speed": 30
     },
     "plungerMotorConfigurations": {
         "idle": 0.05,
-        "run": 0.3
+        "run": 0.5
     },
     "plungerPositionsConfigurations": {
         "default": {
-            "blowout": 0.5,
+            "blowout": -1.0,
             "bottom": 2.0,
-            "drop": -6.0,
+            "drop": -4.0,
             "top": 19.5
         }
     },
     "quirks": [
         "dropTipShake"
     ],
-    "shaftDiameter": 2.0,
-    "shaftULperMM": 3.142
+    "shaftDiameter": 1.0,
+    "shaftULperMM": 0.785
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p50/1_4.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p10/1_4.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.810530462184874%*

 * *Differences: {"'channels'": '8',*

 * * "'displayName'": "'P10 8-Channel GEN1'",*

 * * "'model'": "'p10'",*

 * * "'partialTipConfigurations'": "{'partialTipSupported': True, 'availableConfigurations': [1, 2, 3, "*

 * *                               '4, 5, 6, 7, 8]}',*

 * * "'pickUpTipConfigurations'": "{'pressFit': {'currentByTipCount': {'2': 0.1, '3': 0.15, '4': 0.2, "*

 * *                              "'5': 0.25, '6': 0.3, '7': 0.35, '8': 0.4}, 'speedByTipCount': "*

 * *                              "OrderedDict([('1', 30.0), ('2', 30.0), ('3', 30.0),  […]*

```diff
@@ -1,54 +1,88 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipettePropertiesSchema.json",
     "availableSensors": {
         "sensors": []
     },
     "backCompatNames": [],
     "backlashDistance": 0.0,
-    "channels": 1,
+    "channels": 8,
     "displayCategory": "GEN1",
-    "displayName": "P50 Single-Channel GEN1",
+    "displayName": "P10 8-Channel GEN1",
     "dropTipConfigurations": {
         "plungerEject": {
             "current": 0.5,
             "speed": 5.0
         }
     },
-    "model": "p50",
+    "model": "p10",
     "partialTipConfigurations": {
-        "availableConfigurations": null,
-        "partialTipSupported": false
+        "availableConfigurations": [
+            1,
+            2,
+            3,
+            4,
+            5,
+            6,
+            7,
+            8
+        ],
+        "partialTipSupported": true
     },
     "pickUpTipConfigurations": {
         "pressFit": {
             "currentByTipCount": {
-                "1": 0.1
+                "1": 0.1,
+                "2": 0.1,
+                "3": 0.15,
+                "4": 0.2,
+                "5": 0.25,
+                "6": 0.3,
+                "7": 0.35,
+                "8": 0.4
+            },
+            "distanceByTipCount": {
+                "1": 10.0,
+                "2": 10.0,
+                "3": 10.0,
+                "4": 10.0,
+                "5": 10.0,
+                "6": 10.0,
+                "7": 10.0,
+                "8": 10.0
             },
-            "distance": 10.0,
             "increment": 1.0,
             "presses": 3,
-            "speed": 30.0
+            "speedByTipCount": {
+                "1": 30.0,
+                "2": 30.0,
+                "3": 30.0,
+                "4": 30.0,
+                "5": 30.0,
+                "6": 30.0,
+                "7": 30.0,
+                "8": 30.0
+            }
         }
     },
     "plungerHomingConfigurations": {
-        "current": 0.3,
+        "current": 0.5,
         "speed": 30
     },
     "plungerMotorConfigurations": {
         "idle": 0.05,
-        "run": 0.3
+        "run": 0.5
     },
     "plungerPositionsConfigurations": {
         "default": {
-            "blowout": 0.5,
+            "blowout": -1.0,
             "bottom": 2.0,
-            "drop": -5.0,
+            "drop": -4.5,
             "top": 19.5
         }
     },
     "quirks": [
         "dropTipShake"
     ],
-    "shaftDiameter": 2.0,
-    "shaftULperMM": 3.142
+    "shaftDiameter": 1.0,
+    "shaftULperMM": 0.785
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p50/1_5.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p1000/3_0.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6760110294117647%*

 * *Differences: {"'availableSensors'": "{'sensors': ['pressure', 'capacitive', 'environment'], 'pressure': "*

 * *                       "OrderedDict([('count', 2)]), 'capacitive': OrderedDict([('count', 2)]), "*

 * *                       "'environment': OrderedDict([('count', 1)])}",*

 * * "'backlashDistance'": '0.1',*

 * * "'channels'": '8',*

 * * "'displayCategory'": "'FLEX'",*

 * * "'displayName'": "'Flex 8-Channel 1000 μL'",*

 * * "'dropTipConfigurations'": "{'plungerEject': {'current': 1.0, 'speed': 10}}",*

 * * "'model'": "'p1000'",*

 * * "'partialTipConfigur […]*

```diff
@@ -1,54 +1,99 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipettePropertiesSchema.json",
     "availableSensors": {
-        "sensors": []
+        "capacitive": {
+            "count": 2
+        },
+        "environment": {
+            "count": 1
+        },
+        "pressure": {
+            "count": 2
+        },
+        "sensors": [
+            "pressure",
+            "capacitive",
+            "environment"
+        ]
     },
     "backCompatNames": [],
-    "backlashDistance": 0.0,
-    "channels": 1,
-    "displayCategory": "GEN1",
-    "displayName": "P50 Single-Channel GEN1",
+    "backlashDistance": 0.1,
+    "channels": 8,
+    "displayCategory": "FLEX",
+    "displayName": "Flex 8-Channel 1000 \u03bcL",
     "dropTipConfigurations": {
         "plungerEject": {
-            "current": 0.5,
-            "speed": 5.0
+            "current": 1.0,
+            "speed": 10
         }
     },
-    "model": "p50",
+    "model": "p1000",
     "partialTipConfigurations": {
-        "availableConfigurations": null,
-        "partialTipSupported": false
+        "availableConfigurations": [
+            1,
+            2,
+            3,
+            4,
+            5,
+            6,
+            7,
+            8
+        ],
+        "partialTipSupported": true
     },
     "pickUpTipConfigurations": {
         "pressFit": {
             "currentByTipCount": {
-                "1": 0.1
+                "1": 0.15,
+                "2": 0.13,
+                "3": 0.19,
+                "4": 0.25,
+                "5": 0.31,
+                "6": 0.38,
+                "7": 0.44,
+                "8": 0.5
             },
-            "distance": 10.0,
-            "increment": 1.0,
-            "presses": 3,
-            "speed": 30.0
+            "distanceByTipCount": {
+                "1": 13.0,
+                "2": 13.0,
+                "3": 13.0,
+                "4": 13.0,
+                "5": 13.0,
+                "6": 13.0,
+                "7": 13.0,
+                "8": 13.0
+            },
+            "increment": 0.0,
+            "presses": 1,
+            "speedByTipCount": {
+                "1": 10.0,
+                "2": 10.0,
+                "3": 10.0,
+                "4": 10.0,
+                "5": 10.0,
+                "6": 10.0,
+                "7": 10.0,
+                "8": 10.0
+            }
         }
     },
     "plungerHomingConfigurations": {
-        "current": 0.3,
+        "current": 1.0,
         "speed": 30
     },
     "plungerMotorConfigurations": {
-        "idle": 0.05,
-        "run": 0.3
+        "idle": 0.3,
+        "run": 1.0
     },
     "plungerPositionsConfigurations": {
         "default": {
-            "blowout": 0.5,
-            "bottom": 2.0,
-            "drop": -5.0,
-            "top": 19.5
+            "blowout": 76.5,
+            "bottom": 71.5,
+            "drop": 92.5,
+            "top": 0.5
         }
     },
-    "quirks": [
-        "dropTipShake"
-    ],
-    "shaftDiameter": 2.0,
-    "shaftULperMM": 3.142
+    "quirks": [],
+    "shaftDiameter": 4.5,
+    "shaftULperMM": 15.904
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p50/3_0.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p1000/3_4.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8086265756302521%*

 * *Differences: {"'availableSensors'": "{'pressure': {'count': 2}, 'capacitive': {'count': 2}}",*

 * * "'channels'": '8',*

 * * "'displayName'": "'Flex 8-Channel 1000 μL'",*

 * * "'model'": "'p1000'",*

 * * "'partialTipConfigurations'": "{'partialTipSupported': True, 'availableConfigurations': [1, 2, 3, "*

 * *                               '4, 5, 6, 7, 8]}',*

 * * "'pickUpTipConfigurations'": "{'pressFit': {'currentByTipCount': {'1': 0.2, '2': 0.14, '3': 0.21, "*

 * *                              "'4': 0.28, '5': 0.34, '6': 0.41, '7': 0.48, '8': 0.55}, "*

 * *  […]*

```diff
@@ -1,71 +1,99 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipettePropertiesSchema.json",
     "availableSensors": {
         "capacitive": {
-            "count": 1
+            "count": 2
         },
         "environment": {
             "count": 1
         },
         "pressure": {
-            "count": 1
+            "count": 2
         },
         "sensors": [
             "pressure",
             "capacitive",
             "environment"
         ]
     },
     "backCompatNames": [],
     "backlashDistance": 0.1,
-    "channels": 1,
+    "channels": 8,
     "displayCategory": "FLEX",
-    "displayName": "Flex 1-Channel 50 \u03bcL",
+    "displayName": "Flex 8-Channel 1000 \u03bcL",
     "dropTipConfigurations": {
         "plungerEject": {
             "current": 1.0,
             "speed": 10
         }
     },
-    "model": "p50",
+    "model": "p1000",
     "partialTipConfigurations": {
-        "availableConfigurations": null,
-        "partialTipSupported": false
+        "availableConfigurations": [
+            1,
+            2,
+            3,
+            4,
+            5,
+            6,
+            7,
+            8
+        ],
+        "partialTipSupported": true
     },
     "pickUpTipConfigurations": {
         "pressFit": {
             "currentByTipCount": {
-                "1": 0.15
+                "1": 0.2,
+                "2": 0.14,
+                "3": 0.21,
+                "4": 0.28,
+                "5": 0.34,
+                "6": 0.41,
+                "7": 0.48,
+                "8": 0.55
+            },
+            "distanceByTipCount": {
+                "1": 13.0,
+                "2": 13.0,
+                "3": 13.0,
+                "4": 13.0,
+                "5": 13.0,
+                "6": 13.0,
+                "7": 13.0,
+                "8": 13.0
             },
-            "distance": 13.0,
             "increment": 0.0,
             "presses": 1,
-            "speed": 5
+            "speedByTipCount": {
+                "1": 10.0,
+                "2": 10.0,
+                "3": 10.0,
+                "4": 10.0,
+                "5": 10.0,
+                "6": 10.0,
+                "7": 10.0,
+                "8": 10.0
+            }
         }
     },
     "plungerHomingConfigurations": {
         "current": 1.0,
         "speed": 30
     },
     "plungerMotorConfigurations": {
         "idle": 0.3,
         "run": 1.0
     },
     "plungerPositionsConfigurations": {
         "default": {
             "blowout": 76.5,
             "bottom": 71.5,
-            "drop": 90.5,
-            "top": 0.5
-        },
-        "lowVolumeDefault": {
-            "blowout": 76.5,
-            "bottom": 61.5,
-            "drop": 90.5,
-            "top": 0.5
+            "drop": 91.5,
+            "top": 0.0
         }
     },
     "quirks": [],
-    "shaftDiameter": 1.0,
-    "shaftULperMM": 0.785
+    "shaftDiameter": 4.5,
+    "shaftULperMM": 15.904
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p50/3_3.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p1000/3_5.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8086265756302521%*

 * *Differences: {"'availableSensors'": "{'pressure': {'count': 2}, 'capacitive': {'count': 2}}",*

 * * "'channels'": '8',*

 * * "'displayName'": "'Flex 8-Channel 1000 μL'",*

 * * "'model'": "'p1000'",*

 * * "'partialTipConfigurations'": "{'partialTipSupported': True, 'availableConfigurations': [1, 2, 3, "*

 * *                               '4, 5, 6, 7, 8]}',*

 * * "'pickUpTipConfigurations'": "{'pressFit': {'currentByTipCount': {'1': 0.2, '2': 0.14, '3': 0.21, "*

 * *                              "'4': 0.28, '5': 0.34, '6': 0.41, '7': 0.48, '8': 0.55}, "*

 * *  […]*

```diff
@@ -1,71 +1,99 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipettePropertiesSchema.json",
     "availableSensors": {
         "capacitive": {
-            "count": 1
+            "count": 2
         },
         "environment": {
             "count": 1
         },
         "pressure": {
-            "count": 1
+            "count": 2
         },
         "sensors": [
             "pressure",
             "capacitive",
             "environment"
         ]
     },
     "backCompatNames": [],
     "backlashDistance": 0.1,
-    "channels": 1,
+    "channels": 8,
     "displayCategory": "FLEX",
-    "displayName": "Flex 1-Channel 50 \u03bcL",
+    "displayName": "Flex 8-Channel 1000 \u03bcL",
     "dropTipConfigurations": {
         "plungerEject": {
             "current": 1.0,
             "speed": 10
         }
     },
-    "model": "p50",
+    "model": "p1000",
     "partialTipConfigurations": {
-        "availableConfigurations": null,
-        "partialTipSupported": false
+        "availableConfigurations": [
+            1,
+            2,
+            3,
+            4,
+            5,
+            6,
+            7,
+            8
+        ],
+        "partialTipSupported": true
     },
     "pickUpTipConfigurations": {
         "pressFit": {
             "currentByTipCount": {
-                "1": 0.15
+                "1": 0.2,
+                "2": 0.14,
+                "3": 0.21,
+                "4": 0.28,
+                "5": 0.34,
+                "6": 0.41,
+                "7": 0.48,
+                "8": 0.55
+            },
+            "distanceByTipCount": {
+                "1": 13.0,
+                "2": 13.0,
+                "3": 13.0,
+                "4": 13.0,
+                "5": 13.0,
+                "6": 13.0,
+                "7": 13.0,
+                "8": 13.0
             },
-            "distance": 13.0,
             "increment": 0.0,
             "presses": 1,
-            "speed": 5
+            "speedByTipCount": {
+                "1": 10.0,
+                "2": 10.0,
+                "3": 10.0,
+                "4": 10.0,
+                "5": 10.0,
+                "6": 10.0,
+                "7": 10.0,
+                "8": 10.0
+            }
         }
     },
     "plungerHomingConfigurations": {
         "current": 1.0,
         "speed": 30
     },
     "plungerMotorConfigurations": {
         "idle": 0.3,
         "run": 1.0
     },
     "plungerPositionsConfigurations": {
         "default": {
             "blowout": 76.5,
             "bottom": 71.5,
-            "drop": 90.5,
-            "top": 0.5
-        },
-        "lowVolumeDefault": {
-            "blowout": 76.5,
-            "bottom": 61.5,
-            "drop": 90.5,
-            "top": 0.5
+            "drop": 91.5,
+            "top": 0.0
         }
     },
     "quirks": [],
-    "shaftDiameter": 1.0,
-    "shaftULperMM": 0.785
+    "shaftDiameter": 4.5,
+    "shaftULperMM": 15.904
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p50/3_4.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p50/3_0.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9060530462184874%*

 * *Differences: {"'availableSensors'": "{'pressure': {'count': 2}, 'capacitive': {'count': 2}}",*

 * * "'channels'": '8',*

 * * "'displayName'": "'Flex 8-Channel 50 μL'",*

 * * "'dropTipConfigurations'": "{'plungerEject': {'speed': 10}}",*

 * * "'partialTipConfigurations'": "{'partialTipSupported': True, 'availableConfigurations': [1, 2, 3, "*

 * *                               '4, 5, 6, 7, 8]}',*

 * * "'pickUpTipConfigurations'": "{'pressFit': {'currentByTipCount': {'1': 0.15, '2': 0.13, '3': "*

 * *                              "0.19, '4': 0.25, '5': 0.31 […]*

```diff
@@ -1,71 +1,105 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipettePropertiesSchema.json",
     "availableSensors": {
         "capacitive": {
-            "count": 1
+            "count": 2
         },
         "environment": {
             "count": 1
         },
         "pressure": {
-            "count": 1
+            "count": 2
         },
         "sensors": [
             "pressure",
             "capacitive",
             "environment"
         ]
     },
     "backCompatNames": [],
     "backlashDistance": 0.1,
-    "channels": 1,
+    "channels": 8,
     "displayCategory": "FLEX",
-    "displayName": "Flex 1-Channel 50 \u03bcL",
+    "displayName": "Flex 8-Channel 50 \u03bcL",
     "dropTipConfigurations": {
         "plungerEject": {
             "current": 1.0,
-            "speed": 15
+            "speed": 10
         }
     },
     "model": "p50",
     "partialTipConfigurations": {
-        "availableConfigurations": null,
-        "partialTipSupported": false
+        "availableConfigurations": [
+            1,
+            2,
+            3,
+            4,
+            5,
+            6,
+            7,
+            8
+        ],
+        "partialTipSupported": true
     },
     "pickUpTipConfigurations": {
         "pressFit": {
             "currentByTipCount": {
-                "1": 0.2
+                "1": 0.15,
+                "2": 0.13,
+                "3": 0.19,
+                "4": 0.25,
+                "5": 0.31,
+                "6": 0.38,
+                "7": 0.44,
+                "8": 0.5
+            },
+            "distanceByTipCount": {
+                "1": 13.0,
+                "2": 13.0,
+                "3": 13.0,
+                "4": 13.0,
+                "5": 13.0,
+                "6": 13.0,
+                "7": 13.0,
+                "8": 13.0
             },
-            "distance": 13.0,
             "increment": 0.0,
             "presses": 1,
-            "speed": 10
+            "speedByTipCount": {
+                "1": 10.0,
+                "2": 10.0,
+                "3": 10.0,
+                "4": 10.0,
+                "5": 10.0,
+                "6": 10.0,
+                "7": 10.0,
+                "8": 10.0
+            }
         }
     },
     "plungerHomingConfigurations": {
         "current": 1.0,
         "speed": 30
     },
     "plungerMotorConfigurations": {
         "idle": 0.3,
         "run": 1.0
     },
     "plungerPositionsConfigurations": {
         "default": {
             "blowout": 76.5,
             "bottom": 71.5,
-            "drop": 90.5,
-            "top": 0.0
+            "drop": 92.5,
+            "top": 0.5
         },
         "lowVolumeDefault": {
             "blowout": 76.5,
             "bottom": 61.5,
-            "drop": 90.5,
-            "top": 0.0
+            "drop": 92.5,
+            "top": 0.5
         }
     },
     "quirks": [],
     "shaftDiameter": 1.0,
     "shaftULperMM": 0.785
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/general/single_channel/p50/3_5.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/general/eight_channel/p50/3_3.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9060530462184874%*

 * *Differences: {"'availableSensors'": "{'pressure': {'count': 2}, 'capacitive': {'count': 2}}",*

 * * "'channels'": '8',*

 * * "'displayName'": "'Flex 8-Channel 50 μL'",*

 * * "'dropTipConfigurations'": "{'plungerEject': {'speed': 10}}",*

 * * "'partialTipConfigurations'": "{'partialTipSupported': True, 'availableConfigurations': [1, 2, 3, "*

 * *                               '4, 5, 6, 7, 8]}',*

 * * "'pickUpTipConfigurations'": "{'pressFit': {'currentByTipCount': {'1': 0.15, '2': 0.13, '3': "*

 * *                              "0.19, '4': 0.25, '5': 0.31 […]*

```diff
@@ -1,71 +1,105 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipettePropertiesSchema.json",
     "availableSensors": {
         "capacitive": {
-            "count": 1
+            "count": 2
         },
         "environment": {
             "count": 1
         },
         "pressure": {
-            "count": 1
+            "count": 2
         },
         "sensors": [
             "pressure",
             "capacitive",
             "environment"
         ]
     },
     "backCompatNames": [],
     "backlashDistance": 0.1,
-    "channels": 1,
+    "channels": 8,
     "displayCategory": "FLEX",
-    "displayName": "Flex 1-Channel 50 \u03bcL",
+    "displayName": "Flex 8-Channel 50 \u03bcL",
     "dropTipConfigurations": {
         "plungerEject": {
             "current": 1.0,
-            "speed": 15
+            "speed": 10
         }
     },
     "model": "p50",
     "partialTipConfigurations": {
-        "availableConfigurations": null,
-        "partialTipSupported": false
+        "availableConfigurations": [
+            1,
+            2,
+            3,
+            4,
+            5,
+            6,
+            7,
+            8
+        ],
+        "partialTipSupported": true
     },
     "pickUpTipConfigurations": {
         "pressFit": {
             "currentByTipCount": {
-                "1": 0.2
+                "1": 0.15,
+                "2": 0.13,
+                "3": 0.19,
+                "4": 0.25,
+                "5": 0.31,
+                "6": 0.38,
+                "7": 0.44,
+                "8": 0.5
+            },
+            "distanceByTipCount": {
+                "1": 13.0,
+                "2": 13.0,
+                "3": 13.0,
+                "4": 13.0,
+                "5": 13.0,
+                "6": 13.0,
+                "7": 13.0,
+                "8": 13.0
             },
-            "distance": 13.0,
             "increment": 0.0,
             "presses": 1,
-            "speed": 10
+            "speedByTipCount": {
+                "1": 10.0,
+                "2": 10.0,
+                "3": 10.0,
+                "4": 10.0,
+                "5": 10.0,
+                "6": 10.0,
+                "7": 10.0,
+                "8": 10.0
+            }
         }
     },
     "plungerHomingConfigurations": {
         "current": 1.0,
         "speed": 30
     },
     "plungerMotorConfigurations": {
         "idle": 0.3,
         "run": 1.0
     },
     "plungerPositionsConfigurations": {
         "default": {
             "blowout": 76.5,
             "bottom": 71.5,
-            "drop": 90.5,
-            "top": 0.0
+            "drop": 92.5,
+            "top": 0.5
         },
         "lowVolumeDefault": {
             "blowout": 76.5,
             "bottom": 61.5,
-            "drop": 90.5,
-            "top": 0.0
+            "drop": 92.5,
+            "top": 0.5
         }
     },
     "quirks": [],
     "shaftDiameter": 1.0,
     "shaftULperMM": 0.785
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p10/1_0.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p10/1_0.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p10/1_3.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p10/1_3.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p10/1_4.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p10/1_4.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p10/1_5.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p10/1_5.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p10/1_6.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p10/1_6.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p1000/1_0.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p1000/1_0.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p1000/3_0.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p1000/3_0.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p1000/3_3.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p1000/3_3.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p1000/3_4.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p1000/3_4.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p1000/3_5.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p1000/3_5.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p20/2_0.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p20/2_0.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p20/2_1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p20/2_1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p300/1_0.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p300/1_0.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p300/1_3.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p300/1_3.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p300/1_4.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p300/1_4.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p300/1_5.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p300/1_5.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p300/2_0.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p300/2_0.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p300/2_1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p300/2_1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p50/1_0.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p50/1_0.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p50/1_3.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p50/1_3.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p50/1_4.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p50/1_4.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p50/1_5.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p50/1_5.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p50/3_0.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p50/3_0.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p50/3_3.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p50/3_3.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p50/3_4.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p50/3_4.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p50/3_5.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/eight_channel/p50/3_5.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/ninety_six_channel/p1000/1_0.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/ninety_six_channel/p1000/1_0.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/ninety_six_channel/p1000/3_0.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/ninety_six_channel/p1000/3_0.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/ninety_six_channel/p1000/3_3.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/ninety_six_channel/p1000/3_3.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/ninety_six_channel/p1000/3_4.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/ninety_six_channel/p1000/3_4.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/ninety_six_channel/p1000/3_5.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/ninety_six_channel/p1000/3_5.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/geometry/ninety_six_channel/p1000/3_6.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/geometry/ninety_six_channel/p1000/3_6.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p10/default/1_0.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p10/default/1_0.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p10/default/1_3.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p10/default/1_3.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p10/default/1_4.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p10/default/1_4.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p10/default/1_5.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p10/default/1_5.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p10/default/1_6.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p10/default/1_6.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p1000/default/1_0.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p1000/default/1_0.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p1000/default/3_0.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p1000/default/3_3.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9541666666666666%*

 * *Differences: {"'defaultTipracks'": "{insert: [(3, 'opentrons/opentrons_flex_96_filtertiprack_1000ul/1'), (4, "*

 * *                      "'opentrons/opentrons_flex_96_filtertiprack_200ul/1'), (5, "*

 * *                      "'opentrons/opentrons_flex_96_filtertiprack_50ul/1')]}",*

 * * "'supportedTips'": "{'t50': {'uiMaxFlowRate': 808.3}, 't200': {'uiMaxFlowRate': 905.7}, 't1000': "*

 * *                    "{'uiMaxFlowRate': 787.7}}"}*

```diff
@@ -8,15 +8,18 @@
         "opentrons/opentrons_flex_96_tiprack_1000ul/1": 10.17,
         "opentrons/opentrons_flex_96_tiprack_200ul/1": 10.1,
         "opentrons/opentrons_flex_96_tiprack_50ul/1": 10.05
     },
     "defaultTipracks": [
         "opentrons/opentrons_flex_96_tiprack_1000ul/1",
         "opentrons/opentrons_flex_96_tiprack_200ul/1",
-        "opentrons/opentrons_flex_96_tiprack_50ul/1"
+        "opentrons/opentrons_flex_96_tiprack_50ul/1",
+        "opentrons/opentrons_flex_96_filtertiprack_1000ul/1",
+        "opentrons/opentrons_flex_96_filtertiprack_200ul/1",
+        "opentrons/opentrons_flex_96_filtertiprack_50ul/1"
     ],
     "maxVolume": 1000,
     "minVolume": 5,
     "supportedTips": {
         "t1000": {
             "aspirate": {
                 "default": {
@@ -457,15 +460,16 @@
                         [
                             1051.4648,
                             0.0001,
                             15.391
                         ]
                     ]
                 }
-            }
+            },
+            "uiMaxFlowRate": 787.7
         },
         "t200": {
             "aspirate": {
                 "default": {
                     "1": [
                         [
                             0.8314,
@@ -903,15 +907,16 @@
                         [
                             214.0264,
                             0.0008,
                             15.123
                         ]
                     ]
                 }
-            }
+            },
+            "uiMaxFlowRate": 905.7
         },
         "t50": {
             "aspirate": {
                 "default": {
                     "1": [
                         [
                             0.4148,
@@ -1359,11 +1364,12 @@
                         [
                             51.4512,
                             0.0064,
                             13.9651
                         ]
                     ]
                 }
-            }
+            },
+            "uiMaxFlowRate": 808.3
         }
     }
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p1000/default/3_3.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p1000/default/3_0.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9226190476190476%*

 * *Differences: {"'defaultTipOverlapDictionary'": "{'opentrons/opentrons_flex_96_tiprack_200ul/1': 10.5, "*

 * *                                  "'opentrons/opentrons_flex_96_tiprack_50ul/1': 10.5, "*

 * *                                  "'opentrons/opentrons_flex_96_tiprack_1000ul/1': 10.5, "*

 * *                                  "'opentrons/opentrons_flex_96_filtertiprack_200ul/1': 10.5, "*

 * *                                  "'opentrons/opentrons_flex_96_filtertiprack_50ul/1': 10.5, "*

 * *                                  "'opentrons/open […]*

```diff
@@ -1,22 +1,25 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipetteLiquidPropertiesSchema.json",
     "defaultTipOverlapDictionary": {
         "default": 10.5,
-        "opentrons/opentrons_flex_96_filtertiprack_1000ul/1": 10.17,
-        "opentrons/opentrons_flex_96_filtertiprack_200ul/1": 10.1,
-        "opentrons/opentrons_flex_96_filtertiprack_50ul/1": 10.05,
-        "opentrons/opentrons_flex_96_tiprack_1000ul/1": 10.17,
-        "opentrons/opentrons_flex_96_tiprack_200ul/1": 10.1,
-        "opentrons/opentrons_flex_96_tiprack_50ul/1": 10.05
+        "opentrons/opentrons_flex_96_filtertiprack_1000ul/1": 10.5,
+        "opentrons/opentrons_flex_96_filtertiprack_200ul/1": 10.5,
+        "opentrons/opentrons_flex_96_filtertiprack_50ul/1": 10.5,
+        "opentrons/opentrons_flex_96_tiprack_1000ul/1": 10.5,
+        "opentrons/opentrons_flex_96_tiprack_200ul/1": 10.5,
+        "opentrons/opentrons_flex_96_tiprack_50ul/1": 10.5
     },
     "defaultTipracks": [
         "opentrons/opentrons_flex_96_tiprack_1000ul/1",
         "opentrons/opentrons_flex_96_tiprack_200ul/1",
-        "opentrons/opentrons_flex_96_tiprack_50ul/1"
+        "opentrons/opentrons_flex_96_tiprack_50ul/1",
+        "opentrons/opentrons_flex_96_filtertiprack_1000ul/1",
+        "opentrons/opentrons_flex_96_filtertiprack_200ul/1",
+        "opentrons/opentrons_flex_96_filtertiprack_50ul/1"
     ],
     "maxVolume": 1000,
     "minVolume": 5,
     "supportedTips": {
         "t1000": {
             "aspirate": {
                 "default": {
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p1000/default/3_4.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p1000/default/3_4.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9541666666666666%*

 * *Differences: {"'defaultTipracks'": "{insert: [(3, 'opentrons/opentrons_flex_96_filtertiprack_1000ul/1'), (4, "*

 * *                      "'opentrons/opentrons_flex_96_filtertiprack_200ul/1'), (5, "*

 * *                      "'opentrons/opentrons_flex_96_filtertiprack_50ul/1')]}",*

 * * "'supportedTips'": "{'t50': {'uiMaxFlowRate': 808.3}, 't200': {'uiMaxFlowRate': 905.7}, 't1000': "*

 * *                    "{'uiMaxFlowRate': 787.7}}"}*

```diff
@@ -8,15 +8,18 @@
         "opentrons/opentrons_flex_96_tiprack_1000ul/1": 10.17,
         "opentrons/opentrons_flex_96_tiprack_200ul/1": 10.1,
         "opentrons/opentrons_flex_96_tiprack_50ul/1": 10.05
     },
     "defaultTipracks": [
         "opentrons/opentrons_flex_96_tiprack_1000ul/1",
         "opentrons/opentrons_flex_96_tiprack_200ul/1",
-        "opentrons/opentrons_flex_96_tiprack_50ul/1"
+        "opentrons/opentrons_flex_96_tiprack_50ul/1",
+        "opentrons/opentrons_flex_96_filtertiprack_1000ul/1",
+        "opentrons/opentrons_flex_96_filtertiprack_200ul/1",
+        "opentrons/opentrons_flex_96_filtertiprack_50ul/1"
     ],
     "maxVolume": 1000,
     "minVolume": 5,
     "supportedTips": {
         "t1000": {
             "aspirate": {
                 "default": {
@@ -457,15 +460,16 @@
                         [
                             1051.4648,
                             0.0001,
                             15.391
                         ]
                     ]
                 }
-            }
+            },
+            "uiMaxFlowRate": 787.7
         },
         "t200": {
             "aspirate": {
                 "default": {
                     "1": [
                         [
                             0.8314,
@@ -903,15 +907,16 @@
                         [
                             214.0264,
                             0.0008,
                             15.123
                         ]
                     ]
                 }
-            }
+            },
+            "uiMaxFlowRate": 905.7
         },
         "t50": {
             "aspirate": {
                 "default": {
                     "1": [
                         [
                             0.4148,
@@ -1359,11 +1364,12 @@
                         [
                             51.4512,
                             0.0064,
                             13.9651
                         ]
                     ]
                 }
-            }
+            },
+            "uiMaxFlowRate": 808.3
         }
     }
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p1000/default/3_5.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p1000/default/3_5.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9541666666666666%*

 * *Differences: {"'defaultTipracks'": "{insert: [(3, 'opentrons/opentrons_flex_96_filtertiprack_1000ul/1'), (4, "*

 * *                      "'opentrons/opentrons_flex_96_filtertiprack_200ul/1'), (5, "*

 * *                      "'opentrons/opentrons_flex_96_filtertiprack_50ul/1')]}",*

 * * "'supportedTips'": "{'t50': {'uiMaxFlowRate': 802.9}, 't200': {'uiMaxFlowRate': 847.9}, 't1000': "*

 * *                    "{'uiMaxFlowRate': 744.6}}"}*

```diff
@@ -8,15 +8,18 @@
         "opentrons/opentrons_flex_96_tiprack_1000ul/1": 10.17,
         "opentrons/opentrons_flex_96_tiprack_200ul/1": 10.1,
         "opentrons/opentrons_flex_96_tiprack_50ul/1": 10.05
     },
     "defaultTipracks": [
         "opentrons/opentrons_flex_96_tiprack_1000ul/1",
         "opentrons/opentrons_flex_96_tiprack_200ul/1",
-        "opentrons/opentrons_flex_96_tiprack_50ul/1"
+        "opentrons/opentrons_flex_96_tiprack_50ul/1",
+        "opentrons/opentrons_flex_96_filtertiprack_1000ul/1",
+        "opentrons/opentrons_flex_96_filtertiprack_200ul/1",
+        "opentrons/opentrons_flex_96_filtertiprack_50ul/1"
     ],
     "maxVolume": 1000,
     "minVolume": 5,
     "supportedTips": {
         "t1000": {
             "aspirate": {
                 "default": {
@@ -197,15 +200,16 @@
                         [
                             1106.0857,
                             0.0001,
                             15.3551
                         ]
                     ]
                 }
-            }
+            },
+            "uiMaxFlowRate": 744.6
         },
         "t200": {
             "aspirate": {
                 "default": {
                     "1": [
                         [
                             0.28375,
@@ -473,15 +477,16 @@
                         [
                             211.27375,
                             0.000719,
                             15.121662
                         ]
                     ]
                 }
-            }
+            },
+            "uiMaxFlowRate": 847.9
         },
         "t50": {
             "aspirate": {
                 "default": {
                     "1": [
                         [
                             0.12,
@@ -759,11 +764,12 @@
                         [
                             54.08,
                             0.001949,
                             14.229706
                         ]
                     ]
                 }
-            }
+            },
+            "uiMaxFlowRate": 802.9
         }
     }
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p20/default/2_0.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p20/default/2_0.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p20/default/2_1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p20/default/2_1.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9947916666666666%*

 * *Differences: {"'supportedTips'": "{'t20': {'uiMaxFlowRate': 25}, 't10': {'uiMaxFlowRate': 23}}"}*

```diff
@@ -327,15 +327,16 @@
                         [
                             21.0316,
                             0.0003,
                             0.7447
                         ]
                     ]
                 }
-            }
+            },
+            "uiMaxFlowRate": 23
         },
         "t20": {
             "aspirate": {
                 "default": {
                     "1": [
                         [
                             0.873,
@@ -641,11 +642,12 @@
                         [
                             21.0316,
                             0.0003,
                             0.7447
                         ]
                     ]
                 }
-            }
+            },
+            "uiMaxFlowRate": 25
         }
     }
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p300/default/1_0.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p300/default/1_0.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p300/default/1_3.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p300/default/1_3.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p300/default/1_4.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p300/default/1_4.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p300/default/1_5.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p300/default/1_5.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p300/default/2_0.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p300/default/2_0.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p300/default/2_1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p300/default/2_1.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9953703703703703%*

 * *Differences: {"'supportedTips'": "{'t200': {'uiMaxFlowRate': 335.3}, 't300': {'uiMaxFlowRate': 335.3}}"}*

```diff
@@ -331,15 +331,16 @@
                         [
                             301.4592,
                             0.0004,
                             9.1587
                         ]
                     ]
                 }
-            }
+            },
+            "uiMaxFlowRate": 335.3
         },
         "t300": {
             "aspirate": {
                 "default": {
                     "1": [
                         [
                             15.1131,
@@ -656,11 +657,12 @@
                         [
                             301.4592,
                             0.0004,
                             9.1587
                         ]
                     ]
                 }
-            }
+            },
+            "uiMaxFlowRate": 335.3
         }
     }
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p50/default/1_0.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p50/default/1_0.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p50/default/1_3.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p50/default/1_3.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p50/default/1_4.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p50/default/1_4.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p50/default/1_5.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p50/default/1_5.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p50/default/3_0.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p50/default/3_0.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9583333333333334%*

 * *Differences: {"'defaultTipracks'": "{insert: [(1, 'opentrons/opentrons_flex_96_filtertiprack_50ul/1')]}"}*

```diff
@@ -2,15 +2,16 @@
     "$otSharedSchema": "#/pipette/schemas/2/pipetteLiquidPropertiesSchema.json",
     "defaultTipOverlapDictionary": {
         "default": 10.5,
         "opentrons/opentrons_flex_96_filtertiprack_50ul/1": 10.05,
         "opentrons/opentrons_flex_96_tiprack_50ul/1": 10.05
     },
     "defaultTipracks": [
-        "opentrons/opentrons_flex_96_tiprack_50ul/1"
+        "opentrons/opentrons_flex_96_tiprack_50ul/1",
+        "opentrons/opentrons_flex_96_filtertiprack_50ul/1"
     ],
     "maxVolume": 50,
     "minVolume": 5,
     "supportedTips": {
         "t50": {
             "aspirate": {
                 "default": {
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p50/default/3_3.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p50/default/3_3.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9541666666666666%*

 * *Differences: {"'defaultTipracks'": "{insert: [(1, 'opentrons/opentrons_flex_96_filtertiprack_50ul/1')]}",*

 * * "'supportedTips'": "{'t50': {'uiMaxFlowRate': 46.8}}"}*

```diff
@@ -2,15 +2,16 @@
     "$otSharedSchema": "#/pipette/schemas/2/pipetteLiquidPropertiesSchema.json",
     "defaultTipOverlapDictionary": {
         "default": 10.5,
         "opentrons/opentrons_flex_96_filtertiprack_50ul/1": 10.05,
         "opentrons/opentrons_flex_96_tiprack_50ul/1": 10.05
     },
     "defaultTipracks": [
-        "opentrons/opentrons_flex_96_tiprack_50ul/1"
+        "opentrons/opentrons_flex_96_tiprack_50ul/1",
+        "opentrons/opentrons_flex_96_filtertiprack_50ul/1"
     ],
     "maxVolume": 50,
     "minVolume": 5,
     "supportedTips": {
         "t50": {
             "aspirate": {
                 "default": {
@@ -321,11 +322,12 @@
                         [
                             51.4567,
                             0.0001,
                             0.7382
                         ]
                     ]
                 }
-            }
+            },
+            "uiMaxFlowRate": 46.8
         }
     }
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p50/default/3_4.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p50/default/3_0.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9279513888888888%*

 * *Differences: {"'defaultTipOverlapDictionary'": "{'opentrons/opentrons_flex_96_tiprack_50ul/1': 10.5, "*

 * *                                  "'opentrons/opentrons_flex_96_filtertiprack_50ul/1': 10.5}",*

 * * "'defaultTipracks'": "{insert: [(1, 'opentrons/opentrons_flex_96_filtertiprack_50ul/1')]}",*

 * * "'supportedTips'": "{'t50': {'defaultAspirateFlowRate': {'default': 8, 'valuesByApiLevel': "*

 * *                    "{'2.14': 8}}, 'defaultDispenseFlowRate': {'default': 8, 'valuesByApiLevel': "*

 * *                    "{'2.14': 8}}, 'defau […]*

```diff
@@ -1,16 +1,17 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipetteLiquidPropertiesSchema.json",
     "defaultTipOverlapDictionary": {
         "default": 10.5,
-        "opentrons/opentrons_flex_96_filtertiprack_50ul/1": 10.05,
-        "opentrons/opentrons_flex_96_tiprack_50ul/1": 10.05
+        "opentrons/opentrons_flex_96_filtertiprack_50ul/1": 10.5,
+        "opentrons/opentrons_flex_96_tiprack_50ul/1": 10.5
     },
     "defaultTipracks": [
-        "opentrons/opentrons_flex_96_tiprack_50ul/1"
+        "opentrons/opentrons_flex_96_tiprack_50ul/1",
+        "opentrons/opentrons_flex_96_filtertiprack_50ul/1"
     ],
     "maxVolume": 50,
     "minVolume": 5,
     "supportedTips": {
         "t50": {
             "aspirate": {
                 "default": {
@@ -155,29 +156,29 @@
                             0.0001,
                             0.7382
                         ]
                     ]
                 }
             },
             "defaultAspirateFlowRate": {
-                "default": 35,
+                "default": 8,
                 "valuesByApiLevel": {
-                    "2.14": 35
+                    "2.14": 8
                 }
             },
             "defaultBlowOutFlowRate": {
-                "default": 57,
+                "default": 4,
                 "valuesByApiLevel": {
-                    "2.14": 57
+                    "2.14": 4
                 }
             },
             "defaultDispenseFlowRate": {
-                "default": 57,
+                "default": 8,
                 "valuesByApiLevel": {
-                    "2.14": 57
+                    "2.14": 8
                 }
             },
             "defaultFlowAcceleration": 1200.0,
             "defaultPushOutVolume": 2,
             "defaultReturnTipHeight": 0.71,
             "defaultTipLength": 57.9,
             "dispense": {
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p50/default/3_5.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p50/default/3_5.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9541666666666666%*

 * *Differences: {"'defaultTipracks'": "{insert: [(1, 'opentrons/opentrons_flex_96_filtertiprack_50ul/1')]}",*

 * * "'supportedTips'": "{'t50': {'uiMaxFlowRate': 46.7}}"}*

```diff
@@ -2,15 +2,16 @@
     "$otSharedSchema": "#/pipette/schemas/2/pipetteLiquidPropertiesSchema.json",
     "defaultTipOverlapDictionary": {
         "default": 10.5,
         "opentrons/opentrons_flex_96_filtertiprack_50ul/1": 10.05,
         "opentrons/opentrons_flex_96_tiprack_50ul/1": 10.05
     },
     "defaultTipracks": [
-        "opentrons/opentrons_flex_96_tiprack_50ul/1"
+        "opentrons/opentrons_flex_96_tiprack_50ul/1",
+        "opentrons/opentrons_flex_96_filtertiprack_50ul/1"
     ],
     "maxVolume": 50,
     "minVolume": 5,
     "supportedTips": {
         "t50": {
             "aspirate": {
                 "default": {
@@ -281,11 +282,12 @@
                         [
                             53.2317,
                             0.0001,
                             0.7403
                         ]
                     ]
                 }
-            }
+            },
+            "uiMaxFlowRate": 46.7
         }
     }
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p50/lowVolumeDefault/3_0.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p50/lowVolumeDefault/3_0.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9583333333333334%*

 * *Differences: {"'defaultTipracks'": "{insert: [(1, 'opentrons/opentrons_flex_96_filtertiprack_50ul/1')]}"}*

```diff
@@ -2,15 +2,16 @@
     "$otSharedSchema": "#/pipette/schemas/2/pipetteLiquidPropertiesSchema.json",
     "defaultTipOverlapDictionary": {
         "default": 10.5,
         "opentrons/opentrons_flex_96_filtertiprack_50ul/1": 10.05,
         "opentrons/opentrons_flex_96_tiprack_50ul/1": 10.05
     },
     "defaultTipracks": [
-        "opentrons/opentrons_flex_96_tiprack_50ul/1"
+        "opentrons/opentrons_flex_96_tiprack_50ul/1",
+        "opentrons/opentrons_flex_96_filtertiprack_50ul/1"
     ],
     "maxVolume": 30,
     "minVolume": 1,
     "supportedTips": {
         "t50": {
             "aspirate": {
                 "default": {
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p50/lowVolumeDefault/3_3.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p50/lowVolumeDefault/3_3.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9541666666666666%*

 * *Differences: {"'defaultTipracks'": "{insert: [(1, 'opentrons/opentrons_flex_96_filtertiprack_50ul/1')]}",*

 * * "'supportedTips'": "{'t50': {'uiMaxFlowRate': 32.6}}"}*

```diff
@@ -2,15 +2,16 @@
     "$otSharedSchema": "#/pipette/schemas/2/pipetteLiquidPropertiesSchema.json",
     "defaultTipOverlapDictionary": {
         "default": 10.5,
         "opentrons/opentrons_flex_96_filtertiprack_50ul/1": 10.05,
         "opentrons/opentrons_flex_96_tiprack_50ul/1": 10.05
     },
     "defaultTipracks": [
-        "opentrons/opentrons_flex_96_tiprack_50ul/1"
+        "opentrons/opentrons_flex_96_tiprack_50ul/1",
+        "opentrons/opentrons_flex_96_filtertiprack_50ul/1"
     ],
     "maxVolume": 30,
     "minVolume": 1,
     "supportedTips": {
         "t50": {
             "aspirate": {
                 "default": {
@@ -271,11 +272,12 @@
                         [
                             45.795,
                             0.0003,
                             0.7308
                         ]
                     ]
                 }
-            }
+            },
+            "uiMaxFlowRate": 32.6
         }
     }
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p50/lowVolumeDefault/3_4.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p50/lowVolumeDefault/3_4.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9518229166666666%*

 * *Differences: {"'defaultTipracks'": "{insert: [(1, 'opentrons/opentrons_flex_96_filtertiprack_50ul/1')]}",*

 * * "'supportedTips'": "{'t50': {'defaultAspirateFlowRate': {'default': 32.6, 'valuesByApiLevel': "*

 * *                    "{'2.14': 32.6}}, 'defaultDispenseFlowRate': {'default': 32.6, "*

 * *                    "'valuesByApiLevel': {'2.14': 32.6}}, 'defaultBlowOutFlowRate': {'default': "*

 * *                    "32.6, 'valuesByApiLevel': {'2.14': 32.6}}, 'uiMaxFlowRate': 32.6}}"}*

```diff
@@ -2,15 +2,16 @@
     "$otSharedSchema": "#/pipette/schemas/2/pipetteLiquidPropertiesSchema.json",
     "defaultTipOverlapDictionary": {
         "default": 10.5,
         "opentrons/opentrons_flex_96_filtertiprack_50ul/1": 10.05,
         "opentrons/opentrons_flex_96_tiprack_50ul/1": 10.05
     },
     "defaultTipracks": [
-        "opentrons/opentrons_flex_96_tiprack_50ul/1"
+        "opentrons/opentrons_flex_96_tiprack_50ul/1",
+        "opentrons/opentrons_flex_96_filtertiprack_50ul/1"
     ],
     "maxVolume": 30,
     "minVolume": 1,
     "supportedTips": {
         "t50": {
             "aspirate": {
                 "default": {
@@ -130,29 +131,29 @@
                             0.0003,
                             0.7308
                         ]
                     ]
                 }
             },
             "defaultAspirateFlowRate": {
-                "default": 35,
+                "default": 32.6,
                 "valuesByApiLevel": {
-                    "2.14": 35
+                    "2.14": 32.6
                 }
             },
             "defaultBlowOutFlowRate": {
-                "default": 57,
+                "default": 32.6,
                 "valuesByApiLevel": {
-                    "2.14": 57
+                    "2.14": 32.6
                 }
             },
             "defaultDispenseFlowRate": {
-                "default": 57,
+                "default": 32.6,
                 "valuesByApiLevel": {
-                    "2.14": 57
+                    "2.14": 32.6
                 }
             },
             "defaultFlowAcceleration": 1200.0,
             "defaultPushOutVolume": 7,
             "defaultReturnTipHeight": 0.71,
             "defaultTipLength": 57.9,
             "dispense": {
@@ -271,11 +272,12 @@
                         [
                             45.795,
                             0.0003,
                             0.7308
                         ]
                     ]
                 }
-            }
+            },
+            "uiMaxFlowRate": 32.6
         }
     }
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p50/lowVolumeDefault/3_5.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p50/lowVolumeDefault/3_5.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9518229166666666%*

 * *Differences: {"'defaultTipracks'": "{insert: [(1, 'opentrons/opentrons_flex_96_filtertiprack_50ul/1')]}",*

 * * "'supportedTips'": "{'t50': {'defaultAspirateFlowRate': {'default': 32.6, 'valuesByApiLevel': "*

 * *                    "{'2.14': 32.6}}, 'defaultDispenseFlowRate': {'default': 32.6, "*

 * *                    "'valuesByApiLevel': {'2.14': 32.6}}, 'defaultBlowOutFlowRate': {'default': "*

 * *                    "32.6, 'valuesByApiLevel': {'2.14': 32.6}}, 'uiMaxFlowRate': 32.6}}"}*

```diff
@@ -2,15 +2,16 @@
     "$otSharedSchema": "#/pipette/schemas/2/pipetteLiquidPropertiesSchema.json",
     "defaultTipOverlapDictionary": {
         "default": 10.5,
         "opentrons/opentrons_flex_96_filtertiprack_50ul/1": 10.05,
         "opentrons/opentrons_flex_96_tiprack_50ul/1": 10.05
     },
     "defaultTipracks": [
-        "opentrons/opentrons_flex_96_tiprack_50ul/1"
+        "opentrons/opentrons_flex_96_tiprack_50ul/1",
+        "opentrons/opentrons_flex_96_filtertiprack_50ul/1"
     ],
     "maxVolume": 30,
     "minVolume": 1,
     "supportedTips": {
         "t50": {
             "aspirate": {
                 "default": {
@@ -130,29 +131,29 @@
                             0.0003,
                             0.7308
                         ]
                     ]
                 }
             },
             "defaultAspirateFlowRate": {
-                "default": 35,
+                "default": 32.6,
                 "valuesByApiLevel": {
-                    "2.14": 35
+                    "2.14": 32.6
                 }
             },
             "defaultBlowOutFlowRate": {
-                "default": 57,
+                "default": 32.6,
                 "valuesByApiLevel": {
-                    "2.14": 57
+                    "2.14": 32.6
                 }
             },
             "defaultDispenseFlowRate": {
-                "default": 57,
+                "default": 32.6,
                 "valuesByApiLevel": {
-                    "2.14": 57
+                    "2.14": 32.6
                 }
             },
             "defaultFlowAcceleration": 1200.0,
             "defaultPushOutVolume": 7,
             "defaultReturnTipHeight": 0.71,
             "defaultTipLength": 57.9,
             "dispense": {
@@ -271,11 +272,12 @@
                         [
                             45.795,
                             0.0003,
                             0.7308
                         ]
                     ]
                 }
-            }
+            },
+            "uiMaxFlowRate": 32.6
         }
     }
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/ninety_six_channel/p1000/default/1_0.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/ninety_six_channel/p1000/default/1_0.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9226190476190476%*

 * *Differences: {"'defaultTipOverlapDictionary'": "{'opentrons/opentrons_flex_96_filtertiprack_1000ul/1': 10.5, "*

 * *                                  "'opentrons/opentrons_flex_96_filtertiprack_200ul/1': 10.5, "*

 * *                                  "'opentrons/opentrons_flex_96_filtertiprack_50ul/1': 10.5}",*

 * * "'defaultTipracks'": "{insert: [(3, 'opentrons/opentrons_flex_96_filtertiprack_1000ul/1'), (4, "*

 * *                      "'opentrons/opentrons_flex_96_filtertiprack_200ul/1'), (5, "*

 * *                      "'opentrons/opentron […]*

```diff
@@ -1,19 +1,25 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipetteLiquidPropertiesSchema.json",
     "defaultTipOverlapDictionary": {
         "default": 10.5,
+        "opentrons/opentrons_flex_96_filtertiprack_1000ul/1": 10.5,
+        "opentrons/opentrons_flex_96_filtertiprack_200ul/1": 10.5,
+        "opentrons/opentrons_flex_96_filtertiprack_50ul/1": 10.5,
         "opentrons/opentrons_flex_96_tiprack_1000ul/1": 10.5,
         "opentrons/opentrons_flex_96_tiprack_200ul/1": 10.5,
         "opentrons/opentrons_flex_96_tiprack_50ul/1": 10.5
     },
     "defaultTipracks": [
         "opentrons/opentrons_flex_96_tiprack_1000ul/1",
         "opentrons/opentrons_flex_96_tiprack_200ul/1",
-        "opentrons/opentrons_flex_96_tiprack_50ul/1"
+        "opentrons/opentrons_flex_96_tiprack_50ul/1",
+        "opentrons/opentrons_flex_96_filtertiprack_1000ul/1",
+        "opentrons/opentrons_flex_96_filtertiprack_200ul/1",
+        "opentrons/opentrons_flex_96_filtertiprack_50ul/1"
     ],
     "maxVolume": 1000,
     "minVolume": 5,
     "supportedTips": {
         "t1000": {
             "aspirate": {
                 "default": {
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/ninety_six_channel/p1000/default/3_0.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/ninety_six_channel/p1000/default/3_0.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9226190476190476%*

 * *Differences: {"'defaultTipOverlapDictionary'": "{'opentrons/opentrons_flex_96_filtertiprack_1000ul/1': 10.5, "*

 * *                                  "'opentrons/opentrons_flex_96_filtertiprack_200ul/1': 10.5, "*

 * *                                  "'opentrons/opentrons_flex_96_filtertiprack_50ul/1': 10.5}",*

 * * "'defaultTipracks'": "{insert: [(3, 'opentrons/opentrons_flex_96_filtertiprack_1000ul/1'), (4, "*

 * *                      "'opentrons/opentrons_flex_96_filtertiprack_200ul/1'), (5, "*

 * *                      "'opentrons/opentron […]*

```diff
@@ -1,19 +1,25 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipetteLiquidPropertiesSchema.json",
     "defaultTipOverlapDictionary": {
         "default": 10.5,
+        "opentrons/opentrons_flex_96_filtertiprack_1000ul/1": 10.5,
+        "opentrons/opentrons_flex_96_filtertiprack_200ul/1": 10.5,
+        "opentrons/opentrons_flex_96_filtertiprack_50ul/1": 10.5,
         "opentrons/opentrons_flex_96_tiprack_1000ul/1": 10.5,
         "opentrons/opentrons_flex_96_tiprack_200ul/1": 10.5,
         "opentrons/opentrons_flex_96_tiprack_50ul/1": 10.5
     },
     "defaultTipracks": [
         "opentrons/opentrons_flex_96_tiprack_1000ul/1",
         "opentrons/opentrons_flex_96_tiprack_200ul/1",
-        "opentrons/opentrons_flex_96_tiprack_50ul/1"
+        "opentrons/opentrons_flex_96_tiprack_50ul/1",
+        "opentrons/opentrons_flex_96_filtertiprack_1000ul/1",
+        "opentrons/opentrons_flex_96_filtertiprack_200ul/1",
+        "opentrons/opentrons_flex_96_filtertiprack_50ul/1"
     ],
     "maxVolume": 1000,
     "minVolume": 5,
     "supportedTips": {
         "t1000": {
             "aspirate": {
                 "default": {
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/ninety_six_channel/p1000/default/3_3.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/ninety_six_channel/p1000/default/3_5.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.918452380952381%*

 * *Differences: {"'defaultTipOverlapDictionary'": "{'opentrons/opentrons_flex_96_filtertiprack_1000ul/1': 10.5, "*

 * *                                  "'opentrons/opentrons_flex_96_filtertiprack_200ul/1': 10.5, "*

 * *                                  "'opentrons/opentrons_flex_96_filtertiprack_50ul/1': 10.5}",*

 * * "'defaultTipracks'": "{insert: [(3, 'opentrons/opentrons_flex_96_filtertiprack_1000ul/1'), (4, "*

 * *                      "'opentrons/opentrons_flex_96_filtertiprack_200ul/1'), (5, "*

 * *                      "'opentrons/opentron […]*

```diff
@@ -1,19 +1,25 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipetteLiquidPropertiesSchema.json",
     "defaultTipOverlapDictionary": {
         "default": 10.5,
+        "opentrons/opentrons_flex_96_filtertiprack_1000ul/1": 10.5,
+        "opentrons/opentrons_flex_96_filtertiprack_200ul/1": 10.5,
+        "opentrons/opentrons_flex_96_filtertiprack_50ul/1": 10.5,
         "opentrons/opentrons_flex_96_tiprack_1000ul/1": 10.5,
         "opentrons/opentrons_flex_96_tiprack_200ul/1": 10.5,
         "opentrons/opentrons_flex_96_tiprack_50ul/1": 10.5
     },
     "defaultTipracks": [
         "opentrons/opentrons_flex_96_tiprack_1000ul/1",
         "opentrons/opentrons_flex_96_tiprack_200ul/1",
-        "opentrons/opentrons_flex_96_tiprack_50ul/1"
+        "opentrons/opentrons_flex_96_tiprack_50ul/1",
+        "opentrons/opentrons_flex_96_filtertiprack_1000ul/1",
+        "opentrons/opentrons_flex_96_filtertiprack_200ul/1",
+        "opentrons/opentrons_flex_96_filtertiprack_50ul/1"
     ],
     "maxVolume": 1000,
     "minVolume": 5,
     "supportedTips": {
         "t1000": {
             "aspirate": {
                 "default": {
@@ -214,15 +220,16 @@
                         [
                             1049.145714,
                             -1.3e-05,
                             15.535884
                         ]
                     ]
                 }
-            }
+            },
+            "uiMaxFlowRate": 185.1
         },
         "t200": {
             "aspirate": {
                 "default": {
                     "1": [
                         [
                             1.39875,
@@ -360,15 +367,16 @@
                         [
                             211.0225,
                             0.000928,
                             15.059476
                         ]
                     ]
                 }
-            }
+            },
+            "uiMaxFlowRate": 185.1
         },
         "t50": {
             "aspirate": {
                 "default": {
                     "1": [
                         [
                             1.933333,
@@ -516,11 +524,12 @@
                         [
                             54.82,
                             0.001805,
                             14.43229
                         ]
                     ]
                 }
-            }
+            },
+            "uiMaxFlowRate": 189.1
         }
     }
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/ninety_six_channel/p1000/default/3_4.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/ninety_six_channel/p1000/default/3_3.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.918452380952381%*

 * *Differences: {"'defaultTipOverlapDictionary'": "{'opentrons/opentrons_flex_96_filtertiprack_1000ul/1': 10.5, "*

 * *                                  "'opentrons/opentrons_flex_96_filtertiprack_200ul/1': 10.5, "*

 * *                                  "'opentrons/opentrons_flex_96_filtertiprack_50ul/1': 10.5}",*

 * * "'defaultTipracks'": "{insert: [(3, 'opentrons/opentrons_flex_96_filtertiprack_1000ul/1'), (4, "*

 * *                      "'opentrons/opentrons_flex_96_filtertiprack_200ul/1'), (5, "*

 * *                      "'opentrons/opentron […]*

```diff
@@ -1,19 +1,25 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipetteLiquidPropertiesSchema.json",
     "defaultTipOverlapDictionary": {
         "default": 10.5,
+        "opentrons/opentrons_flex_96_filtertiprack_1000ul/1": 10.5,
+        "opentrons/opentrons_flex_96_filtertiprack_200ul/1": 10.5,
+        "opentrons/opentrons_flex_96_filtertiprack_50ul/1": 10.5,
         "opentrons/opentrons_flex_96_tiprack_1000ul/1": 10.5,
         "opentrons/opentrons_flex_96_tiprack_200ul/1": 10.5,
         "opentrons/opentrons_flex_96_tiprack_50ul/1": 10.5
     },
     "defaultTipracks": [
         "opentrons/opentrons_flex_96_tiprack_1000ul/1",
         "opentrons/opentrons_flex_96_tiprack_200ul/1",
-        "opentrons/opentrons_flex_96_tiprack_50ul/1"
+        "opentrons/opentrons_flex_96_tiprack_50ul/1",
+        "opentrons/opentrons_flex_96_filtertiprack_1000ul/1",
+        "opentrons/opentrons_flex_96_filtertiprack_200ul/1",
+        "opentrons/opentrons_flex_96_filtertiprack_50ul/1"
     ],
     "maxVolume": 1000,
     "minVolume": 5,
     "supportedTips": {
         "t1000": {
             "aspirate": {
                 "default": {
@@ -214,15 +220,16 @@
                         [
                             1049.145714,
                             -1.3e-05,
                             15.535884
                         ]
                     ]
                 }
-            }
+            },
+            "uiMaxFlowRate": 184.8
         },
         "t200": {
             "aspirate": {
                 "default": {
                     "1": [
                         [
                             1.39875,
@@ -360,15 +367,16 @@
                         [
                             211.0225,
                             0.000928,
                             15.059476
                         ]
                     ]
                 }
-            }
+            },
+            "uiMaxFlowRate": 185.1
         },
         "t50": {
             "aspirate": {
                 "default": {
                     "1": [
                         [
                             1.933333,
@@ -516,11 +524,12 @@
                         [
                             54.82,
                             0.001805,
                             14.43229
                         ]
                     ]
                 }
-            }
+            },
+            "uiMaxFlowRate": 189.1
         }
     }
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/ninety_six_channel/p1000/default/3_5.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/ninety_six_channel/p1000/default/3_4.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.918452380952381%*

 * *Differences: {"'defaultTipOverlapDictionary'": "{'opentrons/opentrons_flex_96_filtertiprack_1000ul/1': 10.5, "*

 * *                                  "'opentrons/opentrons_flex_96_filtertiprack_200ul/1': 10.5, "*

 * *                                  "'opentrons/opentrons_flex_96_filtertiprack_50ul/1': 10.5}",*

 * * "'defaultTipracks'": "{insert: [(3, 'opentrons/opentrons_flex_96_filtertiprack_1000ul/1'), (4, "*

 * *                      "'opentrons/opentrons_flex_96_filtertiprack_200ul/1'), (5, "*

 * *                      "'opentrons/opentron […]*

```diff
@@ -1,19 +1,25 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipetteLiquidPropertiesSchema.json",
     "defaultTipOverlapDictionary": {
         "default": 10.5,
+        "opentrons/opentrons_flex_96_filtertiprack_1000ul/1": 10.5,
+        "opentrons/opentrons_flex_96_filtertiprack_200ul/1": 10.5,
+        "opentrons/opentrons_flex_96_filtertiprack_50ul/1": 10.5,
         "opentrons/opentrons_flex_96_tiprack_1000ul/1": 10.5,
         "opentrons/opentrons_flex_96_tiprack_200ul/1": 10.5,
         "opentrons/opentrons_flex_96_tiprack_50ul/1": 10.5
     },
     "defaultTipracks": [
         "opentrons/opentrons_flex_96_tiprack_1000ul/1",
         "opentrons/opentrons_flex_96_tiprack_200ul/1",
-        "opentrons/opentrons_flex_96_tiprack_50ul/1"
+        "opentrons/opentrons_flex_96_tiprack_50ul/1",
+        "opentrons/opentrons_flex_96_filtertiprack_1000ul/1",
+        "opentrons/opentrons_flex_96_filtertiprack_200ul/1",
+        "opentrons/opentrons_flex_96_filtertiprack_50ul/1"
     ],
     "maxVolume": 1000,
     "minVolume": 5,
     "supportedTips": {
         "t1000": {
             "aspirate": {
                 "default": {
@@ -214,15 +220,16 @@
                         [
                             1049.145714,
                             -1.3e-05,
                             15.535884
                         ]
                     ]
                 }
-            }
+            },
+            "uiMaxFlowRate": 184.8
         },
         "t200": {
             "aspirate": {
                 "default": {
                     "1": [
                         [
                             1.39875,
@@ -360,15 +367,16 @@
                         [
                             211.0225,
                             0.000928,
                             15.059476
                         ]
                     ]
                 }
-            }
+            },
+            "uiMaxFlowRate": 185.1
         },
         "t50": {
             "aspirate": {
                 "default": {
                     "1": [
                         [
                             1.933333,
@@ -516,11 +524,12 @@
                         [
                             54.82,
                             0.001805,
                             14.43229
                         ]
                     ]
                 }
-            }
+            },
+            "uiMaxFlowRate": 189.1
         }
     }
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/ninety_six_channel/p1000/default/3_6.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/ninety_six_channel/p1000/default/3_6.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9958333333333332%*

 * *Differences: {"'supportedTips'": "{'t50': {'uiMaxFlowRate': 194}, 't200': {'uiMaxFlowRate': 194}, 't1000': "*

 * *                    "{'uiMaxFlowRate': 187.2}}"}*

```diff
@@ -214,15 +214,16 @@
                         [
                             1037.1873,
                             0.0005,
                             14.8072
                         ]
                     ]
                 }
-            }
+            },
+            "uiMaxFlowRate": 187.2
         },
         "t200": {
             "aspirate": {
                 "default": {
                     "1": [
                         [
                             1.9331,
@@ -360,15 +361,16 @@
                         [
                             211.1169,
                             0.0005,
                             15.1655
                         ]
                     ]
                 }
-            }
+            },
+            "uiMaxFlowRate": 194
         },
         "t50": {
             "aspirate": {
                 "default": {
                     "1": [
                         [
                             1.9733,
@@ -516,11 +518,12 @@
                         [
                             55.4792,
                             -0.0013,
                             14.7754
                         ]
                     ]
                 }
-            }
+            },
+            "uiMaxFlowRate": 194
         }
     }
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p10/default/1_0.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p10/default/1_0.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p10/default/1_3.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p10/default/1_3.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p10/default/1_4.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p10/default/1_4.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p10/default/1_5.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p10/default/1_5.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p1000/default/1_0.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p1000/default/1_0.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p1000/default/1_3.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p1000/default/1_3.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p1000/default/1_4.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p1000/default/1_4.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p1000/default/1_5.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p1000/default/1_5.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p1000/default/2_0.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p1000/default/2_0.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p1000/default/2_1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p1000/default/2_1.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9953703703703703%*

 * *Differences: {"'supportedTips'": "{'t1000': {'uiMaxFlowRate': 1018.6}}"}*

```diff
@@ -346,11 +346,12 @@
                         [
                             1012.2269,
                             0.0,
                             27.3121
                         ]
                     ]
                 }
-            }
+            },
+            "uiMaxFlowRate": 1018.6
         }
     }
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p1000/default/2_2.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p1000/default/2_2.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9953703703703703%*

 * *Differences: {"'supportedTips'": "{'t1000': {'uiMaxFlowRate': 1020.7}}"}*

```diff
@@ -346,11 +346,12 @@
                         [
                             1013.9597,
                             0.0001,
                             27.2644
                         ]
                     ]
                 }
-            }
+            },
+            "uiMaxFlowRate": 1020.7
         }
     }
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p1000/default/3_0.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p1000/default/3_3.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.918452380952381%*

 * *Differences: {"'defaultTipOverlapDictionary'": "{'opentrons/opentrons_flex_96_filtertiprack_1000ul/1': 10.5, "*

 * *                                  "'opentrons/opentrons_flex_96_filtertiprack_200ul/1': 10.5, "*

 * *                                  "'opentrons/opentrons_flex_96_filtertiprack_50ul/1': 10.5}",*

 * * "'defaultTipracks'": "{insert: [(3, 'opentrons/opentrons_flex_96_filtertiprack_1000ul/1'), (4, "*

 * *                      "'opentrons/opentrons_flex_96_filtertiprack_200ul/1'), (5, "*

 * *                      "'opentrons/opentron […]*

```diff
@@ -1,19 +1,25 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipetteLiquidPropertiesSchema.json",
     "defaultTipOverlapDictionary": {
         "default": 10.5,
+        "opentrons/opentrons_flex_96_filtertiprack_1000ul/1": 10.5,
+        "opentrons/opentrons_flex_96_filtertiprack_200ul/1": 10.5,
+        "opentrons/opentrons_flex_96_filtertiprack_50ul/1": 10.5,
         "opentrons/opentrons_flex_96_tiprack_1000ul/1": 10.5,
         "opentrons/opentrons_flex_96_tiprack_200ul/1": 10.5,
         "opentrons/opentrons_flex_96_tiprack_50ul/1": 10.5
     },
     "defaultTipracks": [
         "opentrons/opentrons_flex_96_tiprack_1000ul/1",
         "opentrons/opentrons_flex_96_tiprack_200ul/1",
-        "opentrons/opentrons_flex_96_tiprack_50ul/1"
+        "opentrons/opentrons_flex_96_tiprack_50ul/1",
+        "opentrons/opentrons_flex_96_filtertiprack_1000ul/1",
+        "opentrons/opentrons_flex_96_filtertiprack_200ul/1",
+        "opentrons/opentrons_flex_96_filtertiprack_50ul/1"
     ],
     "maxVolume": 1000,
     "minVolume": 5,
     "supportedTips": {
         "t1000": {
             "aspirate": {
                 "default": {
@@ -454,15 +460,16 @@
                         [
                             1051.4648,
                             0.0001,
                             15.391
                         ]
                     ]
                 }
-            }
+            },
+            "uiMaxFlowRate": 787.7
         },
         "t200": {
             "aspirate": {
                 "default": {
                     "1": [
                         [
                             0.8314,
@@ -900,15 +907,16 @@
                         [
                             214.0264,
                             0.0008,
                             15.123
                         ]
                     ]
                 }
-            }
+            },
+            "uiMaxFlowRate": 905.7
         },
         "t50": {
             "aspirate": {
                 "default": {
                     "1": [
                         [
                             0.4148,
@@ -1356,11 +1364,12 @@
                         [
                             51.4512,
                             0.0064,
                             13.9651
                         ]
                     ]
                 }
-            }
+            },
+            "uiMaxFlowRate": 808.3
         }
     }
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p1000/default/3_3.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p1000/default/3_0.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9047619047619048%*

 * *Differences: {"'defaultTipOverlapDictionary'": "{'opentrons/opentrons_flex_96_tiprack_1000ul/1': 10.17, "*

 * *                                  "'opentrons/opentrons_flex_96_tiprack_200ul/1': 10.1, "*

 * *                                  "'opentrons/opentrons_flex_96_tiprack_50ul/1': 10.05, "*

 * *                                  "'opentrons/opentrons_flex_96_filtertiprack_200ul/1': 10.1, "*

 * *                                  "'opentrons/opentrons_flex_96_filtertiprack_50ul/1': 10.05, "*

 * *                                  "'opentrons/o […]*

```diff
@@ -1,19 +1,25 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipetteLiquidPropertiesSchema.json",
     "defaultTipOverlapDictionary": {
         "default": 10.5,
-        "opentrons/opentrons_flex_96_tiprack_1000ul/1": 10.5,
-        "opentrons/opentrons_flex_96_tiprack_200ul/1": 10.5,
-        "opentrons/opentrons_flex_96_tiprack_50ul/1": 10.5
+        "opentrons/opentrons_flex_96_filtertiprack_1000ul/1": 10.17,
+        "opentrons/opentrons_flex_96_filtertiprack_200ul/1": 10.1,
+        "opentrons/opentrons_flex_96_filtertiprack_50ul/1": 10.05,
+        "opentrons/opentrons_flex_96_tiprack_1000ul/1": 10.17,
+        "opentrons/opentrons_flex_96_tiprack_200ul/1": 10.1,
+        "opentrons/opentrons_flex_96_tiprack_50ul/1": 10.05
     },
     "defaultTipracks": [
         "opentrons/opentrons_flex_96_tiprack_1000ul/1",
         "opentrons/opentrons_flex_96_tiprack_200ul/1",
-        "opentrons/opentrons_flex_96_tiprack_50ul/1"
+        "opentrons/opentrons_flex_96_tiprack_50ul/1",
+        "opentrons/opentrons_flex_96_filtertiprack_1000ul/1",
+        "opentrons/opentrons_flex_96_filtertiprack_200ul/1",
+        "opentrons/opentrons_flex_96_filtertiprack_50ul/1"
     ],
     "maxVolume": 1000,
     "minVolume": 5,
     "supportedTips": {
         "t1000": {
             "aspirate": {
                 "default": {
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p1000/default/3_4.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p1000/default/3_4.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.918452380952381%*

 * *Differences: {"'defaultTipOverlapDictionary'": "{'opentrons/opentrons_flex_96_filtertiprack_1000ul/1': 10.5, "*

 * *                                  "'opentrons/opentrons_flex_96_filtertiprack_200ul/1': 10.5, "*

 * *                                  "'opentrons/opentrons_flex_96_filtertiprack_50ul/1': 10.5}",*

 * * "'defaultTipracks'": "{insert: [(3, 'opentrons/opentrons_flex_96_filtertiprack_1000ul/1'), (4, "*

 * *                      "'opentrons/opentrons_flex_96_filtertiprack_200ul/1'), (5, "*

 * *                      "'opentrons/opentron […]*

```diff
@@ -1,19 +1,25 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipetteLiquidPropertiesSchema.json",
     "defaultTipOverlapDictionary": {
         "default": 10.5,
+        "opentrons/opentrons_flex_96_filtertiprack_1000ul/1": 10.5,
+        "opentrons/opentrons_flex_96_filtertiprack_200ul/1": 10.5,
+        "opentrons/opentrons_flex_96_filtertiprack_50ul/1": 10.5,
         "opentrons/opentrons_flex_96_tiprack_1000ul/1": 10.5,
         "opentrons/opentrons_flex_96_tiprack_200ul/1": 10.5,
         "opentrons/opentrons_flex_96_tiprack_50ul/1": 10.5
     },
     "defaultTipracks": [
         "opentrons/opentrons_flex_96_tiprack_1000ul/1",
         "opentrons/opentrons_flex_96_tiprack_200ul/1",
-        "opentrons/opentrons_flex_96_tiprack_50ul/1"
+        "opentrons/opentrons_flex_96_tiprack_50ul/1",
+        "opentrons/opentrons_flex_96_filtertiprack_1000ul/1",
+        "opentrons/opentrons_flex_96_filtertiprack_200ul/1",
+        "opentrons/opentrons_flex_96_filtertiprack_50ul/1"
     ],
     "maxVolume": 1000,
     "minVolume": 5,
     "supportedTips": {
         "t1000": {
             "aspirate": {
                 "default": {
@@ -334,15 +340,16 @@
                         [
                             1101.4771,
                             0.0001,
                             15.2962
                         ]
                     ]
                 }
-            }
+            },
+            "uiMaxFlowRate": 763.3
         },
         "t200": {
             "aspirate": {
                 "default": {
                     "1": [
                         [
                             0.1983,
@@ -660,15 +667,16 @@
                         [
                             210.66,
                             0.0012,
                             14.9867
                         ]
                     ]
                 }
-            }
+            },
+            "uiMaxFlowRate": 745
         },
         "t50": {
             "aspirate": {
                 "default": {
                     "1": [
                         [
                             0.0671,
@@ -986,11 +994,12 @@
                         [
                             53.6686,
                             0.0113,
                             13.6208
                         ]
                     ]
                 }
-            }
+            },
+            "uiMaxFlowRate": 762.1
         }
     }
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p1000/default/3_5.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p1000/default/3_5.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.918452380952381%*

 * *Differences: {"'defaultTipOverlapDictionary'": "{'opentrons/opentrons_flex_96_filtertiprack_1000ul/1': 10.5, "*

 * *                                  "'opentrons/opentrons_flex_96_filtertiprack_200ul/1': 10.5, "*

 * *                                  "'opentrons/opentrons_flex_96_filtertiprack_50ul/1': 10.5}",*

 * * "'defaultTipracks'": "{insert: [(3, 'opentrons/opentrons_flex_96_filtertiprack_1000ul/1'), (4, "*

 * *                      "'opentrons/opentrons_flex_96_filtertiprack_200ul/1'), (5, "*

 * *                      "'opentrons/opentron […]*

```diff
@@ -1,19 +1,25 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipetteLiquidPropertiesSchema.json",
     "defaultTipOverlapDictionary": {
         "default": 10.5,
+        "opentrons/opentrons_flex_96_filtertiprack_1000ul/1": 10.5,
+        "opentrons/opentrons_flex_96_filtertiprack_200ul/1": 10.5,
+        "opentrons/opentrons_flex_96_filtertiprack_50ul/1": 10.5,
         "opentrons/opentrons_flex_96_tiprack_1000ul/1": 10.5,
         "opentrons/opentrons_flex_96_tiprack_200ul/1": 10.5,
         "opentrons/opentrons_flex_96_tiprack_50ul/1": 10.5
     },
     "defaultTipracks": [
         "opentrons/opentrons_flex_96_tiprack_1000ul/1",
         "opentrons/opentrons_flex_96_tiprack_200ul/1",
-        "opentrons/opentrons_flex_96_tiprack_50ul/1"
+        "opentrons/opentrons_flex_96_tiprack_50ul/1",
+        "opentrons/opentrons_flex_96_filtertiprack_1000ul/1",
+        "opentrons/opentrons_flex_96_filtertiprack_200ul/1",
+        "opentrons/opentrons_flex_96_filtertiprack_50ul/1"
     ],
     "maxVolume": 1000,
     "minVolume": 5,
     "supportedTips": {
         "t1000": {
             "aspirate": {
                 "default": {
@@ -194,15 +200,16 @@
                         [
                             1102.5675,
                             0.0,
                             15.3839
                         ]
                     ]
                 }
-            }
+            },
+            "uiMaxFlowRate": 753.5
         },
         "t200": {
             "aspirate": {
                 "default": {
                     "1": [
                         [
                             1.5742,
@@ -370,15 +377,16 @@
                         [
                             211.5867,
                             0.0009,
                             15.1088
                         ]
                     ]
                 }
-            }
+            },
+            "uiMaxFlowRate": 802.5
         },
         "t50": {
             "aspirate": {
                 "default": {
                     "1": [
                         [
                             0.7033,
@@ -596,11 +604,12 @@
                         [
                             54.06,
                             0.0016,
                             14.2446
                         ]
                     ]
                 }
-            }
+            },
+            "uiMaxFlowRate": 785.2
         }
     }
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p1000/default/3_6.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p1000/default/3_6.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.918452380952381%*

 * *Differences: {"'defaultTipOverlapDictionary'": "{'opentrons/opentrons_flex_96_filtertiprack_1000ul/1': 10.5, "*

 * *                                  "'opentrons/opentrons_flex_96_filtertiprack_200ul/1': 10.5, "*

 * *                                  "'opentrons/opentrons_flex_96_filtertiprack_50ul/1': 10.5}",*

 * * "'defaultTipracks'": "{insert: [(3, 'opentrons/opentrons_flex_96_filtertiprack_1000ul/1'), (4, "*

 * *                      "'opentrons/opentrons_flex_96_filtertiprack_200ul/1'), (5, "*

 * *                      "'opentrons/opentron […]*

```diff
@@ -1,19 +1,25 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipetteLiquidPropertiesSchema.json",
     "defaultTipOverlapDictionary": {
         "default": 10.5,
+        "opentrons/opentrons_flex_96_filtertiprack_1000ul/1": 10.5,
+        "opentrons/opentrons_flex_96_filtertiprack_200ul/1": 10.5,
+        "opentrons/opentrons_flex_96_filtertiprack_50ul/1": 10.5,
         "opentrons/opentrons_flex_96_tiprack_1000ul/1": 10.5,
         "opentrons/opentrons_flex_96_tiprack_200ul/1": 10.5,
         "opentrons/opentrons_flex_96_tiprack_50ul/1": 10.5
     },
     "defaultTipracks": [
         "opentrons/opentrons_flex_96_tiprack_1000ul/1",
         "opentrons/opentrons_flex_96_tiprack_200ul/1",
-        "opentrons/opentrons_flex_96_tiprack_50ul/1"
+        "opentrons/opentrons_flex_96_tiprack_50ul/1",
+        "opentrons/opentrons_flex_96_filtertiprack_1000ul/1",
+        "opentrons/opentrons_flex_96_filtertiprack_200ul/1",
+        "opentrons/opentrons_flex_96_filtertiprack_50ul/1"
     ],
     "maxVolume": 1000,
     "minVolume": 5,
     "supportedTips": {
         "t1000": {
             "aspirate": {
                 "default": {
@@ -194,15 +200,16 @@
                         [
                             1105.26,
                             0.000122,
                             15.323864
                         ]
                     ]
                 }
-            }
+            },
+            "uiMaxFlowRate": 727.3
         },
         "t200": {
             "aspirate": {
                 "default": {
                     "1": [
                         [
                             1.5742,
@@ -370,15 +377,16 @@
                         [
                             211.5867,
                             0.0009,
                             15.1088
                         ]
                     ]
                 }
-            }
+            },
+            "uiMaxFlowRate": 802.5
         },
         "t50": {
             "aspirate": {
                 "default": {
                     "1": [
                         [
                             0.7033,
@@ -596,11 +604,12 @@
                         [
                             54.06,
                             0.0016,
                             14.2446
                         ]
                     ]
                 }
-            }
+            },
+            "uiMaxFlowRate": 785.2
         }
     }
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p20/default/2_0.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p20/default/2_0.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p20/default/2_1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p20/default/2_1.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9947916666666666%*

 * *Differences: {"'supportedTips'": "{'t20': {'uiMaxFlowRate': 25.3}, 't10': {'uiMaxFlowRate': 25.3}}"}*

```diff
@@ -330,15 +330,16 @@
                         [
                             21.3395,
                             0.0008,
                             0.746
                         ]
                     ]
                 }
-            }
+            },
+            "uiMaxFlowRate": 25.3
         },
         "t20": {
             "aspirate": {
                 "default": {
                     "1": [
                         [
                             0.9034,
@@ -931,11 +932,12 @@
                     ],
                     [
                         21.3395,
                         0.0008,
                         0.746
                     ]
                 ]
-            }
+            },
+            "uiMaxFlowRate": 25.3
         }
     }
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p20/default/2_2.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p20/default/2_2.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9947916666666666%*

 * *Differences: {"'supportedTips'": "{'t20': {'uiMaxFlowRate': 25}, 't10': {'uiMaxFlowRate': 25}}"}*

```diff
@@ -614,15 +614,16 @@
                     ],
                     [
                         21.3288,
                         0.0008,
                         0.7455
                     ]
                 ]
-            }
+            },
+            "uiMaxFlowRate": 25
         },
         "t20": {
             "aspirate": {
                 "default": {
                     "1": [
                         [
                             0.8679,
@@ -1215,11 +1216,12 @@
                     ],
                     [
                         21.3288,
                         0.0008,
                         0.7455
                     ]
                 ]
-            }
+            },
+            "uiMaxFlowRate": 25
         }
     }
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p300/default/1_0.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p300/default/1_0.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p300/default/1_3.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p300/default/1_3.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p300/default/1_4.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p300/default/1_4.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p300/default/1_5.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p300/default/1_5.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p300/default/2_0.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p300/default/2_0.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p300/default/2_1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p300/default/2_1.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9947916666666666%*

 * *Differences: {"'supportedTips'": "{'t200': {'uiMaxFlowRate': 329.3}, 't300': {'uiMaxFlowRate': 329.3}}"}*

```diff
@@ -333,15 +333,16 @@
                         [
                             306.8498,
                             0.0005,
                             9.1596
                         ]
                     ]
                 }
-            }
+            },
+            "uiMaxFlowRate": 329.3
         },
         "t300": {
             "aspirate": {
                 "default": {
                     "1": [
                         [
                             14.7756,
@@ -660,11 +661,12 @@
                         [
                             306.8498,
                             0.0005,
                             9.1596
                         ]
                     ]
                 }
-            }
+            },
+            "uiMaxFlowRate": 329.3
         }
     }
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p50/default/1_0.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p50/default/1_0.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p50/default/1_3.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p50/default/1_3.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p50/default/1_4.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p50/default/1_4.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p50/default/1_5.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p50/default/1_5.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p50/default/3_0.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p50/default/3_3.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9263888888888889%*

 * *Differences: {"'defaultTipOverlapDictionary'": "{'opentrons/opentrons_flex_96_filtertiprack_50ul/1': 10.5}",*

 * * "'defaultTipracks'": "{insert: [(1, 'opentrons/opentrons_flex_96_filtertiprack_50ul/1')]}",*

 * * "'supportedTips'": "{'t50': {'uiMaxFlowRate': 46.8}}"}*

```diff
@@ -1,15 +1,17 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipetteLiquidPropertiesSchema.json",
     "defaultTipOverlapDictionary": {
         "default": 10.5,
+        "opentrons/opentrons_flex_96_filtertiprack_50ul/1": 10.5,
         "opentrons/opentrons_flex_96_tiprack_50ul/1": 10.5
     },
     "defaultTipracks": [
-        "opentrons/opentrons_flex_96_tiprack_50ul/1"
+        "opentrons/opentrons_flex_96_tiprack_50ul/1",
+        "opentrons/opentrons_flex_96_filtertiprack_50ul/1"
     ],
     "maxVolume": 50,
     "minVolume": 5,
     "supportedTips": {
         "t50": {
             "aspirate": {
                 "default": {
@@ -320,11 +322,12 @@
                         [
                             51.4567,
                             0.0001,
                             0.7382
                         ]
                     ]
                 }
-            }
+            },
+            "uiMaxFlowRate": 46.8
         }
     }
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p50/default/3_3.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/eight_channel/p50/default/3_4.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.91015625%*

 * *Differences: {"'defaultTipOverlapDictionary'": "{'opentrons/opentrons_flex_96_tiprack_50ul/1': 10.05, "*

 * *                                  "'opentrons/opentrons_flex_96_filtertiprack_50ul/1': 10.05}",*

 * * "'defaultTipracks'": "{insert: [(1, 'opentrons/opentrons_flex_96_filtertiprack_50ul/1')]}",*

 * * "'supportedTips'": "{'t50': {'defaultAspirateFlowRate': {'default': 35, 'valuesByApiLevel': "*

 * *                    "{'2.14': 35}}, 'defaultDispenseFlowRate': {'default': 57, 'valuesByApiLevel': "*

 * *                    "{'2.14': 57}},  […]*

```diff
@@ -1,15 +1,17 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipetteLiquidPropertiesSchema.json",
     "defaultTipOverlapDictionary": {
         "default": 10.5,
-        "opentrons/opentrons_flex_96_tiprack_50ul/1": 10.5
+        "opentrons/opentrons_flex_96_filtertiprack_50ul/1": 10.05,
+        "opentrons/opentrons_flex_96_tiprack_50ul/1": 10.05
     },
     "defaultTipracks": [
-        "opentrons/opentrons_flex_96_tiprack_50ul/1"
+        "opentrons/opentrons_flex_96_tiprack_50ul/1",
+        "opentrons/opentrons_flex_96_filtertiprack_50ul/1"
     ],
     "maxVolume": 50,
     "minVolume": 5,
     "supportedTips": {
         "t50": {
             "aspirate": {
                 "default": {
@@ -154,29 +156,29 @@
                             0.0001,
                             0.7382
                         ]
                     ]
                 }
             },
             "defaultAspirateFlowRate": {
-                "default": 8,
+                "default": 35,
                 "valuesByApiLevel": {
-                    "2.14": 8
+                    "2.14": 35
                 }
             },
             "defaultBlowOutFlowRate": {
-                "default": 4,
+                "default": 57,
                 "valuesByApiLevel": {
-                    "2.14": 4
+                    "2.14": 57
                 }
             },
             "defaultDispenseFlowRate": {
-                "default": 8,
+                "default": 57,
                 "valuesByApiLevel": {
-                    "2.14": 8
+                    "2.14": 57
                 }
             },
             "defaultFlowAcceleration": 1200.0,
             "defaultPushOutVolume": 2,
             "defaultReturnTipHeight": 0.71,
             "defaultTipLength": 57.9,
             "dispense": {
@@ -320,11 +322,12 @@
                         [
                             51.4567,
                             0.0001,
                             0.7382
                         ]
                     ]
                 }
-            }
+            },
+            "uiMaxFlowRate": 46.8
         }
     }
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p50/default/3_4.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p50/default/3_4.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9263888888888889%*

 * *Differences: {"'defaultTipOverlapDictionary'": "{'opentrons/opentrons_flex_96_filtertiprack_50ul/1': 10.5}",*

 * * "'defaultTipracks'": "{insert: [(1, 'opentrons/opentrons_flex_96_filtertiprack_50ul/1')]}",*

 * * "'supportedTips'": "{'t50': {'uiMaxFlowRate': 46.3}}"}*

```diff
@@ -1,15 +1,17 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipetteLiquidPropertiesSchema.json",
     "defaultTipOverlapDictionary": {
         "default": 10.5,
+        "opentrons/opentrons_flex_96_filtertiprack_50ul/1": 10.5,
         "opentrons/opentrons_flex_96_tiprack_50ul/1": 10.5
     },
     "defaultTipracks": [
-        "opentrons/opentrons_flex_96_tiprack_50ul/1"
+        "opentrons/opentrons_flex_96_tiprack_50ul/1",
+        "opentrons/opentrons_flex_96_filtertiprack_50ul/1"
     ],
     "maxVolume": 50,
     "minVolume": 5,
     "supportedTips": {
         "t50": {
             "aspirate": {
                 "default": {
@@ -330,11 +332,12 @@
                         [
                             52.8383,
                             0.0,
                             0.7369
                         ]
                     ]
                 }
-            }
+            },
+            "uiMaxFlowRate": 46.3
         }
     }
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p50/default/3_5.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p50/default/3_5.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9263888888888889%*

 * *Differences: {"'defaultTipOverlapDictionary'": "{'opentrons/opentrons_flex_96_filtertiprack_50ul/1': 10.5}",*

 * * "'defaultTipracks'": "{insert: [(1, 'opentrons/opentrons_flex_96_filtertiprack_50ul/1')]}",*

 * * "'supportedTips'": "{'t50': {'uiMaxFlowRate': 47}}"}*

```diff
@@ -1,15 +1,17 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipetteLiquidPropertiesSchema.json",
     "defaultTipOverlapDictionary": {
         "default": 10.5,
+        "opentrons/opentrons_flex_96_filtertiprack_50ul/1": 10.5,
         "opentrons/opentrons_flex_96_tiprack_50ul/1": 10.5
     },
     "defaultTipracks": [
-        "opentrons/opentrons_flex_96_tiprack_50ul/1"
+        "opentrons/opentrons_flex_96_tiprack_50ul/1",
+        "opentrons/opentrons_flex_96_filtertiprack_50ul/1"
     ],
     "maxVolume": 50,
     "minVolume": 5,
     "supportedTips": {
         "t50": {
             "aspirate": {
                 "default": {
@@ -230,11 +232,12 @@
                         [
                             53.046,
                             -0.0005,
                             0.7676
                         ]
                     ]
                 }
-            }
+            },
+            "uiMaxFlowRate": 47
         }
     }
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p50/lowVolumeDefault/3_0.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p50/lowVolumeDefault/3_0.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9305555555555555%*

 * *Differences: {"'defaultTipOverlapDictionary'": "{'opentrons/opentrons_flex_96_filtertiprack_50ul/1': 10.5}",*

 * * "'defaultTipracks'": "{insert: [(1, 'opentrons/opentrons_flex_96_filtertiprack_50ul/1')]}"}*

```diff
@@ -1,15 +1,17 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipetteLiquidPropertiesSchema.json",
     "defaultTipOverlapDictionary": {
         "default": 10.5,
+        "opentrons/opentrons_flex_96_filtertiprack_50ul/1": 10.5,
         "opentrons/opentrons_flex_96_tiprack_50ul/1": 10.5
     },
     "defaultTipracks": [
-        "opentrons/opentrons_flex_96_tiprack_50ul/1"
+        "opentrons/opentrons_flex_96_tiprack_50ul/1",
+        "opentrons/opentrons_flex_96_filtertiprack_50ul/1"
     ],
     "maxVolume": 30,
     "minVolume": 1,
     "supportedTips": {
         "t50": {
             "aspirate": {
                 "default": {
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p50/lowVolumeDefault/3_3.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p50/lowVolumeDefault/3_3.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9263888888888889%*

 * *Differences: {"'defaultTipOverlapDictionary'": "{'opentrons/opentrons_flex_96_filtertiprack_50ul/1': 10.5}",*

 * * "'defaultTipracks'": "{insert: [(1, 'opentrons/opentrons_flex_96_filtertiprack_50ul/1')]}",*

 * * "'supportedTips'": "{'t50': {'uiMaxFlowRate': 31.8}}"}*

```diff
@@ -1,15 +1,17 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipetteLiquidPropertiesSchema.json",
     "defaultTipOverlapDictionary": {
         "default": 10.5,
+        "opentrons/opentrons_flex_96_filtertiprack_50ul/1": 10.5,
         "opentrons/opentrons_flex_96_tiprack_50ul/1": 10.5
     },
     "defaultTipracks": [
-        "opentrons/opentrons_flex_96_tiprack_50ul/1"
+        "opentrons/opentrons_flex_96_tiprack_50ul/1",
+        "opentrons/opentrons_flex_96_filtertiprack_50ul/1"
     ],
     "maxVolume": 30,
     "minVolume": 1,
     "supportedTips": {
         "t50": {
             "aspirate": {
                 "default": {
@@ -220,11 +222,12 @@
                         [
                             45.73,
                             0.000284,
                             0.731072
                         ]
                     ]
                 }
-            }
+            },
+            "uiMaxFlowRate": 31.8
         }
     }
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p50/lowVolumeDefault/3_4.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p50/lowVolumeDefault/3_4.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9240451388888888%*

 * *Differences: {"'defaultTipOverlapDictionary'": "{'opentrons/opentrons_flex_96_filtertiprack_50ul/1': 10.5}",*

 * * "'defaultTipracks'": "{insert: [(1, 'opentrons/opentrons_flex_96_filtertiprack_50ul/1')]}",*

 * * "'supportedTips'": "{'t50': {'defaultAspirateFlowRate': {'default': 31.8, 'valuesByApiLevel': "*

 * *                    "{'2.14': 31.8}}, 'defaultDispenseFlowRate': {'default': 31.8, "*

 * *                    "'valuesByApiLevel': {'2.14': 31.8}}, 'defaultBlowOutFlowRate': {'default': "*

 * *                    "31.8, 'valuesByApiLeve […]*

```diff
@@ -1,15 +1,17 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipetteLiquidPropertiesSchema.json",
     "defaultTipOverlapDictionary": {
         "default": 10.5,
+        "opentrons/opentrons_flex_96_filtertiprack_50ul/1": 10.5,
         "opentrons/opentrons_flex_96_tiprack_50ul/1": 10.5
     },
     "defaultTipracks": [
-        "opentrons/opentrons_flex_96_tiprack_50ul/1"
+        "opentrons/opentrons_flex_96_tiprack_50ul/1",
+        "opentrons/opentrons_flex_96_filtertiprack_50ul/1"
     ],
     "maxVolume": 30,
     "minVolume": 1,
     "supportedTips": {
         "t50": {
             "aspirate": {
                 "default": {
@@ -104,29 +106,29 @@
                             0.000284,
                             0.731072
                         ]
                     ]
                 }
             },
             "defaultAspirateFlowRate": {
-                "default": 35,
+                "default": 31.8,
                 "valuesByApiLevel": {
-                    "2.14": 35
+                    "2.14": 31.8
                 }
             },
             "defaultBlowOutFlowRate": {
-                "default": 57,
+                "default": 31.8,
                 "valuesByApiLevel": {
-                    "2.14": 57
+                    "2.14": 31.8
                 }
             },
             "defaultDispenseFlowRate": {
-                "default": 57,
+                "default": 31.8,
                 "valuesByApiLevel": {
-                    "2.14": 57
+                    "2.14": 31.8
                 }
             },
             "defaultFlowAcceleration": 1200.0,
             "defaultPushOutVolume": 7,
             "defaultReturnTipHeight": 0.71,
             "defaultTipLength": 57.9,
             "dispense": {
@@ -220,11 +222,12 @@
                         [
                             45.73,
                             0.000284,
                             0.731072
                         ]
                     ]
                 }
-            }
+            },
+            "uiMaxFlowRate": 31.8
         }
     }
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p50/lowVolumeDefault/3_5.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/definitions/2/liquid/single_channel/p50/lowVolumeDefault/3_5.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9240451388888888%*

 * *Differences: {"'defaultTipOverlapDictionary'": "{'opentrons/opentrons_flex_96_filtertiprack_50ul/1': 10.5}",*

 * * "'defaultTipracks'": "{insert: [(1, 'opentrons/opentrons_flex_96_filtertiprack_50ul/1')]}",*

 * * "'supportedTips'": "{'t50': {'defaultAspirateFlowRate': {'default': 26.7, 'valuesByApiLevel': "*

 * *                    "{'2.14': 26.7}}, 'defaultDispenseFlowRate': {'default': 26.7, "*

 * *                    "'valuesByApiLevel': {'2.14': 26.7}}, 'defaultBlowOutFlowRate': {'default': "*

 * *                    "26.7, 'valuesByApiLeve […]*

```diff
@@ -1,15 +1,17 @@
 {
     "$otSharedSchema": "#/pipette/schemas/2/pipetteLiquidPropertiesSchema.json",
     "defaultTipOverlapDictionary": {
         "default": 10.5,
+        "opentrons/opentrons_flex_96_filtertiprack_50ul/1": 10.5,
         "opentrons/opentrons_flex_96_tiprack_50ul/1": 10.5
     },
     "defaultTipracks": [
-        "opentrons/opentrons_flex_96_tiprack_50ul/1"
+        "opentrons/opentrons_flex_96_tiprack_50ul/1",
+        "opentrons/opentrons_flex_96_filtertiprack_50ul/1"
     ],
     "maxVolume": 30,
     "minVolume": 1,
     "supportedTips": {
         "t50": {
             "aspirate": {
                 "default": {
@@ -99,29 +101,29 @@
                             0.000207,
                             0.726887
                         ]
                     ]
                 }
             },
             "defaultAspirateFlowRate": {
-                "default": 35,
+                "default": 26.7,
                 "valuesByApiLevel": {
-                    "2.14": 35
+                    "2.14": 26.7
                 }
             },
             "defaultBlowOutFlowRate": {
-                "default": 57,
+                "default": 26.7,
                 "valuesByApiLevel": {
-                    "2.14": 57
+                    "2.14": 26.7
                 }
             },
             "defaultDispenseFlowRate": {
-                "default": 57,
+                "default": 26.7,
                 "valuesByApiLevel": {
-                    "2.14": 57
+                    "2.14": 26.7
                 }
             },
             "defaultFlowAcceleration": 1200.0,
             "defaultPushOutVolume": 7,
             "defaultReturnTipHeight": 0.71,
             "defaultTipLength": 57.9,
             "dispense": {
@@ -210,11 +212,12 @@
                         [
                             45.25,
                             0.000207,
                             0.726887
                         ]
                     ]
                 }
-            }
+            },
+            "uiMaxFlowRate": 26.7
         }
     }
 }
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/schemas/1/pipetteModelSpecsSchema.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/schemas/1/pipetteModelSpecsSchema.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/schemas/1/pipetteNameSpecsSchema.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/schemas/1/pipetteNameSpecsSchema.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/schemas/2/pipetteGeometrySchema.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/schemas/2/pipetteGeometrySchema.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/pipette/schemas/2/pipettePropertiesSchema.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/pipette/schemas/2/pipettePropertiesSchema.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9740228477754739%*

 * *Differences: {"'definitions'": "{'distanceRange': OrderedDict([('type', 'number'), ('minimum', 0.0), "*

 * *                  "('maximum', 100)]), 'speedRange': OrderedDict([('type', 'number'), ('minimum', "*

 * *                  "0.0), ('maximum', 100)]), 'distanceByTipCount': OrderedDict([('type', "*

 * *                  "'object'), ('patternProperties', OrderedDict([('\\\\d+', OrderedDict([('$ref', "*

 * *                  "'#/definitions/distanceRange')]))]))]), 'speedByTipCount': "*

 * *                  "OrderedDict([('type', 'object'), […]*

```diff
@@ -27,14 +27,27 @@
             "enum": [
                 "GEN1",
                 "GEN2",
                 "FLEX"
             ],
             "type": "string"
         },
+        "distanceByTipCount": {
+            "patternProperties": {
+                "\\d+": {
+                    "$ref": "#/definitions/distanceRange"
+                }
+            },
+            "type": "object"
+        },
+        "distanceRange": {
+            "maximum": 100,
+            "minimum": 0.0,
+            "type": "number"
+        },
         "editConfigurations": {
             "description": "Object allowing you to modify a config",
             "properties": {
                 "displayName": {
                     "type": "string"
                 },
                 "max": {
@@ -76,14 +89,27 @@
                 384
             ],
             "type": "number"
         },
         "positiveNumber": {
             "minimum": 0,
             "type": "number"
+        },
+        "speedByTipCount": {
+            "patternProperties": {
+                "\\d+": {
+                    "$ref": "#/definitions/speedRange"
+                }
+            },
+            "type": "object"
+        },
+        "speedRange": {
+            "maximum": 100,
+            "minimum": 0.0,
+            "type": "number"
         }
     },
     "description": "Version-level pipette specifications, which may vary across different versions of the same pipette",
     "properties": {
         "$otSharedSchema": {
             "description": "The path to a valid Opentrons shared schema relative to the shared-data directory, without its extension. For instance, #/pipette/schemas/2/pipettePropertiesSchema.json is a reference to this schema.",
             "type": "string"
@@ -266,32 +292,32 @@
                     "properties": {
                         "pressFit": {
                             "additionalProperties": false,
                             "properties": {
                                 "currentByTipCount": {
                                     "$ref": "#/definitions/currentByTipCount"
                                 },
-                                "distance": {
-                                    "$ref": "#/definitions/positiveNumber"
+                                "distanceByTipCount": {
+                                    "$ref": "#/definitions/distanceByTipCount"
                                 },
                                 "increment": {
                                     "$ref": "#/definitions/positiveNumber"
                                 },
                                 "presses": {
                                     "$ref": "#/definitions/positiveNumber"
                                 },
-                                "speed": {
-                                    "$ref": "#/definitions/positiveNumber"
+                                "speedByTipCount": {
+                                    "$ref": "#/definitions/speedByTipCount"
                                 }
                             },
                             "required": [
                                 "presses",
-                                "speed",
+                                "speedByTipCount",
                                 "increment",
-                                "distance",
+                                "distanceByTipCount",
                                 "currentByTipCount"
                             ],
                             "type": "object"
                         }
                     },
                     "required": [
                         "pressFit"
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/protocol/schemas/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/protocol/schemas/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/protocol/schemas/2.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/protocol/schemas/2.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/protocol/schemas/3.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/protocol/schemas/3.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/protocol/schemas/4.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/protocol/schemas/4.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/protocol/schemas/5.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/protocol/schemas/5.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/protocol/schemas/6.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/protocol/schemas/6.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/protocol/schemas/7.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/protocol/schemas/7.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/protocol/schemas/8.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/protocol/schemas/8.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/data/robot/schemas/1.json` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/data/robot/schemas/1.json`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/deck/__init__.py` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/deck/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,17 +11,19 @@
     from .dev_types import (
         DeckSchema,
         DeckDefinition,
         DeckDefinitionV3,
         DeckSchemaVersion3,
         DeckDefinitionV4,
         DeckSchemaVersion4,
+        DeckDefinitionV5,
+        DeckSchemaVersion5,
     )
 
-DEFAULT_DECK_DEFINITION_VERSION: Final = 4
+DEFAULT_DECK_DEFINITION_VERSION: Final = 5
 
 
 class Offset(NamedTuple):
     x: float = 0.0
     y: float = 0.0
     z: float = 0.0
 
@@ -35,14 +37,19 @@
     "right": Offset(x=CALIBRATION_SQUARE_SIZE * 0.5),
     "top": Offset(y=CALIBRATION_SQUARE_SIZE * 0.5),
     "bottom": Offset(y=-CALIBRATION_SQUARE_SIZE * 0.5),
 }
 
 
 @overload
+def load(name: str, version: "DeckSchemaVersion5") -> "DeckDefinitionV5":
+    ...
+
+
+@overload
 def load(name: str, version: "DeckSchemaVersion4") -> "DeckDefinitionV4":
     ...
 
 
 @overload
 def load(name: str, version: "DeckSchemaVersion3") -> "DeckDefinitionV3":
     ...
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/deck/dev_types.py` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/deck/dev_types.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from typing import Any, Dict, List, NewType, Union
 from typing_extensions import Literal, TypedDict
 
 from ..module.dev_types import ModuleType
 
 
+DeckSchemaVersion5 = Literal[5]
 DeckSchemaVersion4 = Literal[4]
 DeckSchemaVersion3 = Literal[3]
 DeckSchemaVersion2 = Literal[2]
 DeckSchemaVersion1 = Literal[1]
 
 DeckSchema = NewType("DeckSchema", Dict[str, Any])
 
@@ -107,17 +108,19 @@
     id: str
     position: List[float]
     displayName: str
 
 
 class CutoutFixture(TypedDict):
     id: str
+    expectOpentronsModuleSerialNumber: bool
     mayMountTo: List[str]
     displayName: str
     providesAddressableAreas: Dict[str, List[str]]
+    fixtureGroup: Dict[str, List[Dict[str, str]]]
     height: float
 
 
 Fixture = Union[
     FixedLabwareBySlot, FixedLabwareByPosition, FixedVolumeBySlot, FixedVolumeByPosition
 ]
 
@@ -172,8 +175,23 @@
     cutoutFixtures: List[CutoutFixture]
 
 
 class DeckDefinitionV4(_RequiredDeckDefinitionV4, total=False):
     gripperOffsets: Dict[str, GripperOffsets]
 
 
-DeckDefinition = Union[DeckDefinitionV3, DeckDefinitionV4]
+class _RequiredDeckDefinitionV5(TypedDict):
+    otId: str
+    schemaVersion: Literal[5]
+    cornerOffsetFromOrigin: List[float]
+    dimensions: List[float]
+    metadata: Metadata
+    robot: Robot
+    locations: LocationsV4
+    cutoutFixtures: List[CutoutFixture]
+
+
+class DeckDefinitionV5(_RequiredDeckDefinitionV5, total=False):
+    gripperOffsets: Dict[str, GripperOffsets]
+
+
+DeckDefinition = Union[DeckDefinitionV3, DeckDefinitionV4, DeckDefinitionV5]
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/errors/__init__.py` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/errors/categories.py` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/errors/categories.py`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/errors/codes.py` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/errors/codes.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,15 @@
     EARLY_CAPACITIVE_SENSE_TRIGGER = _code_from_dict_entry("2009")
     INACCURATE_NON_CONTACT_SWEEP = _code_from_dict_entry("2010")
     MISALIGNED_GANTRY = _code_from_dict_entry("2011")
     UNMATCHED_TIP_PRESENCE_STATES = _code_from_dict_entry("2012")
     POSITION_UNKNOWN = _code_from_dict_entry("2013")
     EXECUTION_CANCELLED = _code_from_dict_entry("2014")
     FAILED_GRIPPER_PICKUP_ERROR = _code_from_dict_entry("2015")
+    MOTOR_DRIVER_ERROR = _code_from_dict_entry("2016")
     ROBOTICS_INTERACTION_ERROR = _code_from_dict_entry("3000")
     LABWARE_DROPPED = _code_from_dict_entry("3001")
     LABWARE_NOT_PICKED_UP = _code_from_dict_entry("3002")
     TIP_PICKUP_FAILED = _code_from_dict_entry("3003")
     TIP_DROP_FAILED = _code_from_dict_entry("3004")
     UNEXPECTED_TIP_REMOVAL = _code_from_dict_entry("3005")
     PIPETTE_OVERPRESSURE = _code_from_dict_entry("3006")
@@ -73,22 +74,24 @@
     UNEXPECTED_TIP_ATTACH = _code_from_dict_entry("3012")
     FIRMWARE_UPDATE_REQUIRED = _code_from_dict_entry("3013")
     INVALID_ACTUATOR = _code_from_dict_entry("3014")
     MODULE_NOT_PRESENT = _code_from_dict_entry("3015")
     INVALID_INSTRUMENT_DATA = _code_from_dict_entry("3016")
     INVALID_LIQUID_CLASS_NAME = _code_from_dict_entry("3017")
     TIP_DETECTOR_NOT_FOUND = _code_from_dict_entry("3018")
+    HEPA_UV_FAILED = _code_from_dict_entry("3019")
     GENERAL_ERROR = _code_from_dict_entry("4000")
     ROBOT_IN_USE = _code_from_dict_entry("4001")
     API_REMOVED = _code_from_dict_entry("4002")
     NOT_SUPPORTED_ON_ROBOT_TYPE = _code_from_dict_entry("4003")
     COMMAND_PRECONDITION_VIOLATED = _code_from_dict_entry("4004")
     COMMAND_PARAMETER_LIMIT_VIOLATED = _code_from_dict_entry("4005")
     INVALID_PROTOCOL_DATA = _code_from_dict_entry("4006")
     API_MISCONFIGURATION = _code_from_dict_entry("4007")
+    INVALID_STORED_DATA = _code_from_dict_entry("4008")
 
     @classmethod
     @lru_cache(25)
     def by_error_code(cls, error_code: str) -> "ErrorCodes":
         """Get an error by its code.
 
         Note: this is a linear search because it makes life easier and also this is rare in python.
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/errors/exceptions.py` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/errors/exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -554,19 +554,17 @@
         states: Dict[int, int],
         detail: Optional[Dict[str, str]] = None,
         wrapping: Optional[Sequence[EnumeratedError]] = None,
     ) -> None:
         """Build an UnmatchedTipPresenceStatesError."""
         format_tip_state = {0: "not detected", 1: "detected"}
         msg = (
-            "Received two differing tip presence statuses:"
-            "\nRear Sensor tips"
-            + format_tip_state[states[0]]
-            + "\nFront Sensor tips"
-            + format_tip_state[states[1]]
+            f"Received two differing tip presence statuses."
+            f" Rear Sensor tips: {format_tip_state[states[0]]}."
+            f" Front Sensor tips: {format_tip_state[states[1]]}."
         )
         if detail:
             msg += str(detail)
         super().__init__(
             ErrorCodes.UNMATCHED_TIP_PRESENCE_STATES,
             msg,
             detail,
@@ -596,14 +594,27 @@
         detail: Optional[Dict[str, str]] = None,
         wrapping: Optional[Sequence[EnumeratedError]] = None,
     ) -> None:
         """Build a ExecutionCancelledError."""
         super().__init__(ErrorCodes.EXECUTION_CANCELLED, message, detail, wrapping)
 
 
+class MotorDriverError(RoboticsControlError):
+    """An error indicating that a motor driver is in error state."""
+
+    def __init__(
+        self,
+        message: Optional[str] = None,
+        detail: Optional[Dict[str, str]] = None,
+        wrapping: Optional[Sequence[EnumeratedError]] = None,
+    ) -> None:
+        """Build a MotorDriverError."""
+        super().__init__(ErrorCodes.MOTOR_DRIVER_ERROR, message, detail, wrapping)
+
+
 class LabwareDroppedError(RoboticsInteractionError):
     """An error indicating that the gripper dropped labware it was holding."""
 
     def __init__(
         self,
         message: Optional[str] = None,
         detail: Optional[Dict[str, str]] = None,
@@ -676,14 +687,27 @@
         checked_detail: Dict[str, Any] = detail or {}
         checked_detail["pipette_name"] = pipette_name
         checked_detail["mount"] = mount
         message = f"Cannot perform {action} with a tip already attached."
         super().__init__(ErrorCodes.UNEXPECTED_TIP_ATTACH, message, detail, wrapping)
 
 
+class HepaUVFailedError(RoboticsInteractionError):
+    """An error indicating that the HEPA UV module has errored."""
+
+    def __init__(
+        self,
+        message: Optional[str] = None,
+        detail: Optional[Dict[str, str]] = None,
+        wrapping: Optional[Sequence[EnumeratedError]] = None,
+    ) -> None:
+        """Build an HepaUVFailedError."""
+        super().__init__(ErrorCodes.HEPA_UV_FAILED, message, detail, wrapping)
+
+
 class FirmwareUpdateRequiredError(RoboticsInteractionError):
     """An error indicating that a firmware update is required."""
 
     def __init__(
         self,
         action: str,
         subsystems_to_update: List[Any],
@@ -927,7 +951,23 @@
         self,
         message: Optional[str] = None,
         detail: Optional[Dict[str, str]] = None,
         wrapping: Optional[Sequence[EnumeratedError]] = None,
     ) -> None:
         """Build an InvalidProtocolData."""
         super().__init__(ErrorCodes.INVALID_PROTOCOL_DATA, message, detail, wrapping)
+
+
+class InvalidStoredData(GeneralError):
+    """An error indicating that some stored data is invalid.
+
+    This will usually be because it was saved by a future version of the software.
+    """
+
+    def __init__(
+        self,
+        message: Optional[str] = None,
+        detail: Optional[Dict[str, str]] = None,
+        wrapping: Optional[Sequence[EnumeratedError]] = None,
+    ) -> None:
+        """Build an InvalidStoredData."""
+        super().__init__(ErrorCodes.INVALID_STORED_DATA, message, detail, wrapping)
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/gripper/__init__.py` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/gripper/__init__.py`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/gripper/gripper_definition.py` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/gripper/gripper_definition.py`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/labware/__init__.py` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/labware/__init__.py`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/labware/dev_types.py` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/labware/dev_types.py`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/labware/labware_definition.py` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/labware/labware_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,15 +156,15 @@
         None,
         description="Required if labware is tiprack, specifies the length of "
         "the area of the tip that overlaps the nozzle of the pipette",
     )
     loadName: str = Field(
         ...,
         description="Name used to reference a labware definition",
-        pattern=SAFE_STRING_REGEX,
+        regex=SAFE_STRING_REGEX,
     )
     isMagneticModuleCompatible: bool = Field(
         ...,
         description="Flag marking whether a labware is compatible by default "
         "with the Magnetic Module",
     )
     magneticModuleEngageHeight: Optional[_NonNegativeNumber] = Field(
@@ -258,15 +258,15 @@
     )
     version: int = Field(
         ...,
         description="Version of the labware definition itself "
         "(eg myPlate v1/v2/v3). An incrementing integer",
         ge=1.0,
     )
-    namespace: str = Field(..., pattern=SAFE_STRING_REGEX)
+    namespace: str = Field(..., regex=SAFE_STRING_REGEX)
     metadata: Metadata = Field(
         ..., description="Properties used for search and display"
     )
     brand: BrandData = Field(
         ...,
         description="Real-world labware that the definition is modeled "
         "from and/or compatible with",
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/load.py` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/load.py`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/module/__init__.py` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/module/__init__.py`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/module/dev_types.py` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/module/dev_types.py`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/pipette/__init__.py` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/pipette/__init__.py`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/pipette/dev_types.py` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/pipette/dev_types.py`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/pipette/file_operation_helpers.py` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/pipette/file_operation_helpers.py`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/pipette/load_data.py` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/pipette/load_data.py`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/pipette/model_constants.py` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/pipette/model_constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,18 +62,28 @@
     "dropTip": ["plungerPositionsConfigurations", "default", "drop"],
     "pickUpCurrent": [
         "pickUpTipConfigurations",
         "pressFit",
         "currentByTipCount",
         "##EACHTIP##",
     ],
-    "pickUpDistance": ["pickUpTipConfigurations", "pressFit", "distance"],
+    "pickUpDistance": [
+        "pickUpTipConfigurations",
+        "pressFit",
+        "distanceByTipCount",
+        "##EACHTIP##",
+    ],
     "pickUpIncrement": ["pickUpTipConfigurations", "pressFit", "increment"],
     "pickUpPresses": ["pickUpTipConfigurations", "pressFit", "presses"],
-    "pickUpSpeed": ["pickUpTipConfigurations", "pressFit", "speed"],
+    "pickUpSpeed": [
+        "pickUpTipConfigurations",
+        "pressFit",
+        "speedByTipCount",
+        "##EACHTIP##",
+    ],
     "plungerCurrent": ["plungerMotorConfigurations", "run"],
     "dropTipCurrent": ["dropTipConfigurations", "plungerEject", "current"],
     "dropTipSpeed": ["dropTipConfigurations", "plungerEject", "speed"],
     "maxVolume": ["liquid_properties", "default", "maxVolume"],
     "minVolume": ["liquid_properties", "default", "minVolume"],
     "tipLength": [
         "liquid_properties",
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/pipette/mutable_configurations.py` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/pipette/mutable_configurations.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,18 +186,24 @@
 
 
 def _find_default(name: str, configs: Dict[str, Any]) -> MutableConfig:
     """Find the default value from the configs and return it as a mutable config."""
     keypath = _MAP_KEY_TO_V2[name]
     nested_name = keypath[-1]
 
-    if name == "pickUpCurrent":
-        min_max_dict = _MIN_MAX_LOOKUP["current"]
-        type_lookup = _TYPE_LOOKUP["current"]
-        units_lookup = _UNITS_LOOKUP["current"]
+    name_to_lookup_key_map = {
+        "pickUpCurrent": "current",
+        "pickUpDistance": "distance",
+        "pickUpSpeed": "speed",
+    }
+    if name in name_to_lookup_key_map.keys():
+        lookup_key = name_to_lookup_key_map[name]
+        min_max_dict = _MIN_MAX_LOOKUP[lookup_key]
+        type_lookup = _TYPE_LOOKUP[lookup_key]
+        units_lookup = _UNITS_LOOKUP[lookup_key]
     else:
         min_max_dict = _MIN_MAX_LOOKUP[nested_name]
         type_lookup = _TYPE_LOOKUP[nested_name]
         units_lookup = _UNITS_LOOKUP[nested_name]
     default_value = _get_default_value_for(configs, keypath)
     return MutableConfig(
         value=default_value,
@@ -300,14 +306,15 @@
     Load pipette config data with any overrides available.
 
     This function reads from disk each time, so changes to the overrides
     will be picked up in subsequent calls.
 
     :param str pipette_model: The pipette model name (i.e. "p10_single_v1.3")
                               for which to load configuration
+    :param pipette_override_path: The path to the on-disk file which has the config overrides.
     :param pipette_serial_number: An (optional) unique ID for the pipette to locate
                        config overrides. If the ID is not specified, the system
                        assumes this is a simulated pipette and does not
                        save settings. If the ID is specified but no overrides
                        corresponding to the ID are found, the system creates a
                        new overrides file for it.
     :type pipette_serial_number: str or None
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/pipette/pipette_definition.py` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/pipette/pipette_definition.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,25 +68,25 @@
 
 
 class SupportedTipsDefinition(BaseModel):
     """Tip parameters available for every tip size."""
 
     default_aspirate_flowrate: FlowRateDefinition = Field(
         ...,
-        description="The flowrate used in aspirations by default.",
+        description="The flowrate used in aspirations by default. For lowVolumeDefault only, the flowrate matches uiMaxFlowRate for ui purposes, it does not change physical behavior.",
         alias="defaultAspirateFlowRate",
     )
     default_dispense_flowrate: FlowRateDefinition = Field(
         ...,
-        description="The flowrate used in dispenses by default.",
+        description="The flowrate used in dispenses by default. For lowVolumeDefault only, the flowrate matches uiMaxFlowRate for ui purposes, it does not change physical behavior.",
         alias="defaultDispenseFlowRate",
     )
     default_blowout_flowrate: FlowRateDefinition = Field(
         ...,
-        description="The flowrate used in blowouts by default.",
+        description="The flowrate used in blowouts by default. For lowVolumeDefault only, the flowrate matches uiMaxFlowRate for ui purposes, it does not change physical behavior.",
         alias="defaultBlowOutFlowRate",
     )
     default_flow_acceleration: float = Field(
         float("inf"),  # no default works for all pipettes
         description="The acceleration used during aspirate/dispense/blowout in ul/s^2.",
         alias="defaultFlowAcceleration",
     )
@@ -107,14 +107,21 @@
         ..., description="The default pipetting functions list for dispensing."
     )
     default_push_out_volume: float = Field(
         ...,
         description="The default volume for a push-out during dispense.",
         alias="defaultPushOutVolume",
     )
+    ui_max_flow_rate: float = Field(
+        float(
+            "inf"
+        ),  # some pipettes (GEN1, unreleased prototype models) don't have a max flow rate
+        description="The lowest volume max flow rate for a pipette's given supported tip, minus 2 percent for safety.",
+        alias="uiMaxFlowRate",
+    )
 
 
 class MotorConfigurations(BaseModel):
     idle: float = Field(
         ..., description="The plunger motor current to use during idle states."
     )
     run: float = Field(
@@ -157,19 +164,23 @@
         ...,
         description="The number of times to force pickup (incrementally more each time by increment)",
     )
     increment: float = Field(
         ...,
         description="The increment to move the pipette down on each force tip pickup press",
     )
-    distance: float = Field(
-        ..., description="The starting distance to begin a pick up tip from"
+    distance_by_tip_count: Dict[int, float] = Field(
+        ...,
+        description="The starting distance to begin a pick up tip from, based on number of tips being picked up",
+        alias="distanceByTipCount",
     )
-    speed: float = Field(
-        ..., description="The speed to move the Z axis for each force pickup"
+    speed_by_tip_count: Dict[int, float] = Field(
+        ...,
+        description="The speed to move the Z axis for each force pickup, based on number of tips being picked up",
+        alias="speedByTipCount",
     )
     current_by_tip_count: Dict[int, float] = Field(
         ...,
         description="A current dictionary look-up by partial tip configuration.",
         alias="currentByTipCount",
     )
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/pipette/pipette_load_name_conversions.py` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/pipette/pipette_load_name_conversions.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 import re
-from typing import List, Optional, Union, cast
+from functools import lru_cache
+from typing import List, Optional, Union, cast, Literal, Tuple
+from opentrons_shared_data import get_shared_data_root
 from .dev_types import PipetteModel, PipetteName
+
 from .types import (
     PipetteChannelType,
     PipetteModelType,
     PipetteVersionType,
     PipetteGenerationType,
     PipetteModelMajorVersionType,
     PipetteModelMinorVersionType,
@@ -102,34 +105,86 @@
     if len(version_list) > 1:
         minor = cast(PipetteModelMinorVersionType, int(version_list[1]))
     else:
         minor = 0
     return PipetteVersionType(major, minor)
 
 
-def version_from_generation(pipette_name_list: List[str]) -> PipetteVersionType:
-    """Convert a string generation name to a py:obj:PipetteVersionType.
+def get_channel_from_pipette_name(pipette_name_tuple: Tuple[str, ...]) -> str:
+    if "single" in pipette_name_tuple:
+        return "single_channel"
+    elif "96" in pipette_name_tuple:
+        return "ninety_six_channel"
+    else:
+        return "eight_channel"
+
+
+def get_major_version_from_pipette_name(
+    pipette_name_tuple: Tuple[str, ...],
+) -> Literal[1, 2, 3]:
+    #   special-casing for 96-channel to return version 3
+    if (
+        "flex" in pipette_name_tuple
+        or "gen3" in pipette_name_tuple
+        or "96" in pipette_name_tuple
+    ):
+        return 3
+    elif "gen2" in pipette_name_tuple:
+        return 2
+    else:
+        return 1
 
-    Pipette generations are strings in the format of "gen1" or "gen2", and
-    usually associated withe :py:data:PipetteName.
+
+@lru_cache(4)
+def version_from_generation(pipette_name_tuple: Tuple[str, ...]) -> PipetteVersionType:
+    """Convert pipetteName to a py:obj:PipetteVersionType
+
+    Given the pipette_name_tuple, cycle through each definition file path
+    and find the latest version (major and minor version combined) that
+    exists and return that version.
 
     Args:
-        pipette_name_list (List[str]): A list of strings from the separated by `_`
-        py:data:PipetteName.
+        pipette_name_tuple (Tuple[str, ...]): A tuple of strings from the separated
+        by `_` py:data:PipetteName.
 
     Returns:
         PipetteVersionType: A pipette version object.
-
     """
-    if "flex" in pipette_name_list or "gen3" in pipette_name_list:
-        return PipetteVersionType(3, 0)
-    elif "gen2" in pipette_name_list:
-        return PipetteVersionType(2, 0)
-    else:
-        return PipetteVersionType(1, 0)
+    major_version_from_pipette_name = get_major_version_from_pipette_name(
+        pipette_name_tuple
+    )
+    model_from_pipette_name = pipette_name_tuple[0]
+    channel_from_pipette_name = get_channel_from_pipette_name(pipette_name_tuple)
+
+    paths_to_validate = (
+        get_shared_data_root() / "pipette" / "definitions" / "2" / "general"
+    )
+    version_paths = (
+        paths_to_validate / channel_from_pipette_name / model_from_pipette_name
+    )
+
+    highest_minor_version: PipetteModelMinorVersionType = 0
+
+    for version_file in version_paths.iterdir():
+        version_list = version_file.stem.split("_")
+        major_version = version_list[0]
+        minor_version = version_list[1]
+
+        # Check if the major version matches the expected major version
+        if major_version == str(major_version_from_pipette_name):
+            minor_version_int = int(minor_version)
+            minor_version_lit: PipetteModelMinorVersionType = cast(
+                PipetteModelMinorVersionType, minor_version_int
+            )
+
+            # Update the highest minor version if this version is higher
+            if highest_minor_version < minor_version_lit:
+                highest_minor_version = minor_version_lit
+
+    return PipetteVersionType(major_version_from_pipette_name, highest_minor_version)
 
 
 def generation_from_string(pipette_name_list: List[str]) -> PipetteGenerationType:
     """Convert a string generation name to a py:obj:PipetteGenerationType.
 
     Args:
         pipette_name_list (List[str]): A list of strings from the separated by `_`
@@ -190,15 +245,20 @@
 
     """
     split_pipette_name = name.split("_")
     channels = channels_from_string(split_pipette_name[1])
     if provided_version:
         version = version_from_string(provided_version)
     else:
-        version = version_from_generation(split_pipette_name)
+        pipette_name_tuple: Tuple[str, str, str] = (
+            split_pipette_name[0],
+            split_pipette_name[1],
+            split_pipette_name[2] if len(split_pipette_name) > 2 else "",
+        )
+        version = version_from_generation(pipette_name_tuple)
 
     pipette_type = PipetteModelType[split_pipette_name[0]]
 
     return PipetteModelVersionType(pipette_type, channels, version)
 
 
 def convert_pipette_model(
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/pipette/scripts/build_json_script.py` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/pipette/scripts/build_json_script.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,21 +56,23 @@
             input(
                 "please provide the increment to move the pipette down for force pickup\n"
             )
         )
         distance = float(
             input("please provide the starting distance for pick up tip\n")
         )
-    print(f"TODO: Current {current} is not used yet")
+    print(
+        f"TODO: Current {current}, speed {speed} and distance {distance} is not used yet"
+    )
     return PickUpTipConfigurations(
         pressFit=PressFitPickUpTipConfiguration(
-            speed=speed,
+            speedByTipCount={},
             presses=presses,
             increment=increment,
-            distance=distance,
+            distanceByTipCount={},
             currentByTipCount={},
         )
     )
 
 
 def _build_drop_tip_data(
     model_configurations: Optional[PipetteModelSpec] = None,
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/pipette/scripts/update_configuration_files.py` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/pipette/scripts/update_configuration_files.py`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/pipette/types.py` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/pipette/types.py`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/protocol/constants.py` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/protocol/constants.py`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/protocol/dev_types.py` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/protocol/dev_types.py`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/protocol/models/__init__.py` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/protocol/models/__init__.py`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/protocol/models/protocol_schema_v6.py` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/protocol/models/protocol_schema_v6.py`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/protocol/models/protocol_schema_v7.py` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/protocol/models/protocol_schema_v7.py`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/protocol/models/protocol_schema_v8.py` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/protocol/models/protocol_schema_v8.py`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/protocol/models/shared_models.py` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/protocol/models/shared_models.py`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/robot/__init__.py` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/robot/__init__.py`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data/robot/dev_types.py` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data/robot/dev_types.py`

 * *Files identical despite different names*

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data.egg-info/PKG-INFO` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentrons_shared_data
-Version: 7.2.2a3
+Version: 7.3.0a0
 Summary: A bundle of data and python binding that supports the Opentrons API. Does not need to be installed manually; only a dependency of the opentrons package
 Author: Opentrons
 Author-email: engineering@opentrons.com
 Maintainer: Opentrons
 Maintainer-email: engineering@opentrons.com
 License: Apache 2.0
 Project-URL: opentrons.com, https://www.opentrons.com
@@ -13,16 +13,14 @@
 Keywords: robots,protocols,synbio,pcr,automation,lab
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 License-File: ../../LICENSE
 Requires-Dist: jsonschema<4.18.0,>=3.0.1
 Requires-Dist: typing-extensions<5,>=4.0.0
 Requires-Dist: pydantic<2.0.0,>=1.10.9
```

### Comparing `opentrons_shared_data-7.2.2a3/opentrons_shared_data.egg-info/SOURCES.txt` & `opentrons_shared_data-7.3.0a0/opentrons_shared_data.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -23,23 +23,26 @@
 opentrons_shared_data/gripper/gripper_definition.py
 opentrons_shared_data/labware/__init__.py
 opentrons_shared_data/labware/constants.py
 opentrons_shared_data/labware/dev_types.py
 opentrons_shared_data/labware/labware_definition.py
 opentrons_shared_data/module/__init__.py
 opentrons_shared_data/module/dev_types.py
+opentrons_shared_data/performance/__init__.py
+opentrons_shared_data/performance/dev_types.py
 opentrons_shared_data/pipette/__init__.py
 opentrons_shared_data/pipette/dev_types.py
 opentrons_shared_data/pipette/file_operation_helpers.py
 opentrons_shared_data/pipette/load_data.py
 opentrons_shared_data/pipette/model_constants.py
 opentrons_shared_data/pipette/mutable_configurations.py
 opentrons_shared_data/pipette/pipette_definition.py
 opentrons_shared_data/pipette/pipette_load_name_conversions.py
 opentrons_shared_data/pipette/types.py
+opentrons_shared_data/pipette/ul_per_mm.py
 opentrons_shared_data/pipette/scripts/__init__.py
 opentrons_shared_data/pipette/scripts/build_json_script.py
 opentrons_shared_data/pipette/scripts/update_configuration_files.py
 opentrons_shared_data/protocol/__init__.py
 opentrons_shared_data/protocol/constants.py
 opentrons_shared_data/protocol/dev_types.py
 opentrons_shared_data/protocol/models/__init__.py
```

### Comparing `opentrons_shared_data-7.2.2a3/setup.py` & `opentrons_shared_data-7.3.0a0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,16 +126,14 @@
 CLASSIFIERS = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Operating System :: OS Independent",
     "Intended Audience :: Science/Research",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Topic :: Scientific/Engineering",
 ]
 KEYWORDS = ["robots", "protocols", "synbio", "pcr", "automation", "lab"]
 DESCRIPTION = (
     "A bundle of data and python binding that supports the Opentrons API. "
     "Does not need to be installed manually; only a dependency of the "
@@ -147,15 +145,15 @@
     "typing-extensions>=4.0.0,<5",
     "pydantic>=1.10.9,<2.0.0",
 ]
 
 
 if __name__ == "__main__":
     setup(
-        python_requires=">=3.8",
+        python_requires=">=3.10",
         name=DISTNAME,
         description=DESCRIPTION,
         license=LICENSE,
         version=VERSION,
         author=AUTHOR,
         author_email=EMAIL,
         maintainer=AUTHOR,
```

