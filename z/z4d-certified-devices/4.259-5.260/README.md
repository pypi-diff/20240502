# Comparing `tmp/z4d_certified_devices-4.259.tar.gz` & `tmp/z4d_certified_devices-5.260.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "z4d_certified_devices-4.259.tar", last modified: Sat Apr 27 16:48:30 2024, max compression
+gzip compressed data, was "z4d_certified_devices-5.260.tar", last modified: Thu May  2 12:11:51 2024, max compression
```

## Comparing `z4d_certified_devices-4.259.tar` & `z4d_certified_devices-5.260.tar`

### file list

```diff
@@ -1,641 +1,641 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:48:30.938391 z4d_certified_devices-4.259/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    36878 2024-04-27 16:48:30.938391 z4d_certified_devices-4.259/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-27 16:48:30.938391 z4d_certified_devices-4.259/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:48:30.846389 z4d_certified_devices-4.259/z4d_certified_devices/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:48:30.850390 z4d_certified_devices-4.259/z4d_certified_devices/Certified/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:48:30.850390 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Adeo/
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Adeo/LDSENK02F.json
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Adeo/LDSENK10.json
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Adeo/LXEK-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Adeo/LXEK-2.json
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Adeo/LXEK-7.json
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Adeo/SIN-4-1-20_LEX.json
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Adeo/SIN-4-FP-21_EQU.json
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Adeo/SIN-4-RS-20_LEX.json
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Adeo/ZBEK-13.json
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Adeo/ZBEK-14.json
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Adeo/ZBEK-3.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:48:30.850390 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Aeotec/
--rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Aeotec/aeotec-button.json
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Aeotec/aeotec-water.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:48:30.850390 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Aotec/
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Aotec/WG001-Z01.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:48:30.850390 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Bitron/
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Bitron/90201021A.json
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Bitron/90201021B.json
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Bitron/90201024.json
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Bitron/AV201021B.json
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Bitron/AV201024A.json
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Bitron/AV201029A.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:48:30.850390 z4d_certified_devices-4.259/z4d_certified_devices/Certified/CLEODE/
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/CLEODE/ZHUM.json
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/CLEODE/ZMOVE.json
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/CLEODE/ZPLUG.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:48:30.850390 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Candeo/
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Candeo/Candeo Zigbee Dimmer.json
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Candeo/HK-DIM-A.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:48:30.854390 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Casa.ia/
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Casa.ia/CAC221.json
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Casa.ia/CCB432.json
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Casa.ia/CDWS312.json
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Casa.ia/CKF204.json
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Casa.ia/CKF205.json
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Casa.ia/CMS323.json
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Casa.ia/CPB206.json
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Casa.ia/CPC321.json
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Casa.ia/CPR412-E.json
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Casa.ia/CPR412.json
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Casa.ia/CSAC451-E.json
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Casa.ia/CSAC451-WTC-E.json
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Casa.ia/CSLC601-D-E.json
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Casa.ia/CSLC601-E.json
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Casa.ia/CSLC631-3.json
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Casa.ia/CSP403.json
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Casa.ia/CTHS317ET.json
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Casa.ia/Dual_Relay_Module.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:48:30.854390 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Chameleon/
--rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Chameleon/MWA1-TIC-historique-mono-base.json
--rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Chameleon/MWA1-TIC-historique-mono-ejp.json
--rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Chameleon/MWA1-TIC-historique-mono-hchp.json
--rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Chameleon/MWA1-TIC-historique-mono-tempo.json
--rw-r--r--   0 runner    (1001) docker     (127)    11271 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Chameleon/MWA1-TIC-standard-mono-base.json
--rw-r--r--   0 runner    (1001) docker     (127)    11271 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Chameleon/MWA1-TIC.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:48:30.854390 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Custom/
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Custom/LYWSD03MMC.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:48:30.854390 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Danalock/
--rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Danalock/V3-BTZB.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:48:30.858390 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Danfoss/
--rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Danfoss/RV001.json
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Danfoss/eT093WRG.json
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Danfoss/eT093WRO.json
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Danfoss/eTRV0100.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:48:30.858390 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Develco/
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Develco/AQSZB-110.json
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Develco/EMIZB-141.json
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Develco/HESZB120.json
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Develco/HMSZB-110.json
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Develco/MOSZB-140.json
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Develco/SMSZB-120.json
--rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Develco/SPLZB-131.json
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Develco/SPLZB-132.json
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Develco/WISZB-120.json
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Develco/ZHEMI101.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:48:30.858390 z4d_certified_devices-4.259/z4d_certified_devices/Certified/ENKI-LEXMAN/
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/ENKI-LEXMAN/LXEK-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/ENKI-LEXMAN/LXEK-2.json
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/ENKI-LEXMAN/LXEK-7.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:48:30.858390 z4d_certified_devices-4.259/z4d_certified_devices/Certified/EcoDim/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/EcoDim/Dimmer-Switch-ZB3.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/EcoDim/Eco-Dim.07Eco-Dim.10.json
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/EcoDim/EcoDim-Zigbee 3.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:48:30.858390 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Eurotronics/
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Eurotronics/SPZB0001.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:48:30.862390 z4d_certified_devices-4.259/z4d_certified_devices/Certified/GLEDOPTO/
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/GLEDOPTO/GL-B-004P.json
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/GLEDOPTO/GL-B-007Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/GLEDOPTO/GL-B-008Z.json
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/GLEDOPTO/GL-B-008ZS.json
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/GLEDOPTO/GL-C-007-2ID.json
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/GLEDOPTO/GL-C-007.json
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/GLEDOPTO/GL-C-008.json
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/GLEDOPTO/GL-C-008S.json
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/GLEDOPTO/GL-C-008Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/GLEDOPTO/GL-C-009.json
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/GLEDOPTO/GL-D-003Z.json
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/GLEDOPTO/GL-FL-004TZS.json
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/GLEDOPTO/GL-MC-001.json
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/GLEDOPTO/GL-S-007ZS.json
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/GLEDOPTO/GLEDOPTO.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:48:30.866390 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Heiman/
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Heiman/COSensor-EF-3.0.json
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Heiman/COSensor-EM.json
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Heiman/COSensor-N.json
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Heiman/CO_V15.json
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Heiman/CO_YDLV10.json
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Heiman/DoorBell-EF-3.0.json
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Heiman/GASSensor-EF-3.0.json
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Heiman/GAS_V15.json
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Heiman/HS3AQ-EFA-3.0.json
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Heiman/RC-EF-3.0.json
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Heiman/RC-EM.json
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Heiman/SMOK_V16.json
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Heiman/SMOK_YDLV10.json
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Heiman/SRHMP-I1.json
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Heiman/SceneSwitch-EM-3.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Heiman/SmartPlug.json
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Heiman/SmokeSensor-EF-3.0.json
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Heiman/SmokeSensor-EM.json
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Heiman/SmokeSensor-N-3.0.json
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Heiman/SmokeSensor-N.json
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Heiman/TS0216.json
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Heiman/WarningDevice-EF-3.0.json
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Heiman/WarningDevice.json
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Heiman/WaterSensor-EF-3.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:48:30.874390 z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/FLOALT panel WS 30x90.json
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/FLOALT panel WS 60x60.json
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/FYRTUR block-out roller blind.json
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/KADRILJ roller blind.json
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/PARASOLL DoorWindow Sensor.json
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/Remote Control N2.json
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/STARKVIND Air purifier.json
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/STOFTMOLN ceilingwall lamp WW24.json
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI Driver 10W.json
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI Driver 30W.json
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI SHORTCUT Button.json
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI Signal Repeater.json
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E12 WS opal 400lm.json
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E14 W opch 400lm.json
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E14 WS 470lm.json
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E14 WS opal 400lm.json
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E14 WS opal 600lm.json
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E26 WS clear 950lm.json
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E26 WS opal 980lm.json
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 CWS 806lm.json
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 CWS opal 600lm.json
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 W opal 1000lm.json
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WS clear 806lm.json
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WS clear 950lm.json
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WS globe 1055lm.json
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WS opal 1000lm.json
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WS opal 950lm.json
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WS opal 980lm.json
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WW 806lm.json
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WW clear 250lm.json
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 opal 1000lm.json
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb GU10 W 400lm.json
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb GU10 WS 345lm.json
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb GU10 WS 400lm.json
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb GU10 WW 400lm.json
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI control outlet.json
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI motion sensor.json
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI onoff switch.json
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI openclose remote.json
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI remote control.json
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI transformer 10W.json
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI wireless dimmer.json
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRIbulbE14WScandleopal470lm.json
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRIbulbE14WSglobeopal470lm.json
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRIbulbE14WWclear250lm.json
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRIbulbE27WSglobeopal1055lm.json
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRIbulbE27WWclear250lm.json
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRIbulbGU10WS345lm.json
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/VINDSTYRKA.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:48:30.874390 z4d_certified_devices-4.259/z4d_certified_devices/Certified/INNR/
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/INNR/OSL 130 C.json
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/INNR/PL 110.json
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/INNR/PL 115.json
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/INNR/RB 248 T.json
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/INNR/RB 285 C.json
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/INNR/SP 120.json
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/INNR/SP 220.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:48:30.874390 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Idinio/
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Idinio/Dimmer-Switch-ZB3.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:48:30.874390 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Iluminize/
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Iluminize/511.201.json
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Iluminize/5120.1200.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:48:30.874390 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Konke/
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Konke/3AFE140103020000.json
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Konke/3AFE14010402000D.json
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Konke/3AFE170100510001.json
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Konke/3AFE220103020000.json
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Konke/3AFE28010402000D.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:48:30.874390 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LIVOLO/
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LIVOLO/TI0001.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:48:30.874390 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LS-Deutschland-GmbH/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LS-Deutschland-GmbH/Emotion.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:48:30.886390 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.airmonitor.acn01.json
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.ctrl_86plug.aq1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.ctrl_86plug.json
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.ctrl_ln2.aq1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.ctrl_ln2.json
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.ctrl_neutral1.json
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.ctrl_neutral2.json
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.curtain.acn002.json
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.light.aqcn02.json
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.lock.v1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.magnet.acn001.json
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.magnet.agl02.json
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.motion.ac01.json
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.motion.ac02.json
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.plug.json
--rw-r--r--   0 runner    (1001) docker     (127)     4643 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.plug.maeu01.json
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.plug.mmeu01.json
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.relay.c2acn01.json
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.remote.acn003.json
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.remote.b186acn01.json
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.remote.b186acn02.json
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.remote.b1acn01.json
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.remote.b286acn01.json
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.remote.b286acn02.json
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.remote.b286opcn01-bulb.json
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.remote.b286opcn01.json
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.remote.b28ac1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.remote.b486opcn01-bulb.json
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.remote.b486opcn01.json
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.remote.b686opcn01-bulb.json
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.remote.b686opcn01.json
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.router.json
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.sen_ill.mgl01.json
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.sens.json
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.sensor_86sw1.json
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.sensor_86sw2.json
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.sensor_cube.aqgl01.json
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.sensor_cube.json
--rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.sensor_ht.agl02.json
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.sensor_ht.json
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.sensor_magnet.acn001.json
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.sensor_magnet.aq2.json
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.sensor_magnet.json
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.sensor_motion.aq2.json
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.sensor_motion.json
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.sensor_natgas.json
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.sensor_smoke.acn03.json
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.sensor_smoke.json
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.sensor_swit.json
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.sensor_switch.aq2.json
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.sensor_switch.aq3.json
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.sensor_switch.aq3t.json
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.sensor_switch.json
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.sensor_wleak.aq1.json
--rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.switch.acn047.json
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.switch.b1lacn02.json
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.switch.b2lacn02.json
--rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.switch.b2lc04.json
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.switch.l0agl1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.switch.l1aeu1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.switch.l2aeu1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.switch.n0agl1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.switch.n1aeu1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.vibration.aq1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.weather.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:48:30.886390 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Legrand/
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Legrand/Cable outlet.json
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Legrand/Connected outlet.json
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Legrand/DIN power consumption module.json
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Legrand/Dimmer switch wo neutral.json
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Legrand/Double gangs remote switch.json
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Legrand/Micromodule switch.json
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Legrand/Mobile outlet.json
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Legrand/Remote motion sensor.json
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Legrand/Remote switch Wake up Sleep.json
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Legrand/Remote switch.json
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Legrand/Remote toggle switch.json
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Legrand/Shutter switch with neutral.json
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Legrand/Shutters central remote switch.json
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Legrand/Teleruptor.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:48:30.890390 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Lixee/
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Lixee/WS2812_light_controller.json
--rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-historique-mono.json
--rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-historique-tri.json
--rw-r--r--   0 runner    (1001) docker     (127)     5459 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-standard-mono-prod.json
--rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-standard-mono.json
--rw-r--r--   0 runner    (1001) docker     (127)     6879 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-standard-tri-prod.json
--rw-r--r--   0 runner    (1001) docker     (127)     5764 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-standard-tri.json
--rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Lixee/ZLinky_TIC.json
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Lixee/ZiPulses.json
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Lixee/Zigate-Router.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:48:30.890390 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Nexturn/
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Nexturn/VOC_Sensor.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:48:30.890390 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Nodon/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Nodon/SIN-4-1-20.json
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Nodon/SIN-4-FP-21.json
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Nodon/SIN-4-RS-20.json
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Nodon/SIN-4-RS-20_PRO.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:48:30.890390 z4d_certified_devices-4.259/z4d_certified_devices/Certified/OSRAM/
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/OSRAM/CLA60 TW OSRAM.json
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/OSRAM/Classic A60 W clear - LIGHTIFY.json
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/OSRAM/LEDVANCE DIM.json
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/OSRAM/LIGHTIFY Indoor Flex RGBW.json
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/OSRAM/LIGHTIFY Outdoor Flex RGBW.json
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/OSRAM/Lightify Switch Mini.json
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/OSRAM/PAR 16 50 RGBW - LIGHTIFY.json
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/OSRAM/PAR16 50 TW.json
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/OSRAM/Plug 01.json
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/OSRAM/Plug Z3.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:48:30.890390 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Orvibo/
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Orvibo/396483ce8b3f4e0d8e9d79079a35a420.json
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Orvibo/3c4e4fc81ed442efaf69353effcdfc5f.json
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Orvibo/50938c4c3c0b4049923cd5afbc151bde.json
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Orvibo/82c167c95ed746cdbd21d6817f72c593.json
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Orvibo/898ca74409a740b28d5841661e72268d.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:48:30.894390 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Others/
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Others/BDP3001.json
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Others/Dimmablelight.json
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Others/EcoDim-Zigbee 3.0.json
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Others/FB56-ZCW08KU1.1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Others/FNB56-ZCW25FB1.6.json
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Others/FNB56-ZCW25FB2.1.json
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Others/FNB56-ZSW01LX2.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Others/FNB56-ZSW02LX2.0.json
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Others/Lamp_01.json
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Others/NUET56-DL27LX1.1.json
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Others/SA-003-Zigbee.json
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Others/VMS_ADUROLIGHT.json
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Others/ZB-CL01.json
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Others/ZB-CT01.json
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Others/ZB-ONOFFPlug-D0005.json
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Others/ZB-SW01.json
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Others/ZB-SW02.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:48:30.898390 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Owon/
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Owon/AC201A.json
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Owon/AC211.json
--rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Owon/AC221.json
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Owon/CB432.json
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Owon/DWS312-E.json
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Owon/DWS312.json
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Owon/KF204.json
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Owon/KF205.json
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Owon/PB206.json
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Owon/PC321.json
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Owon/PIR323-A.json
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Owon/PIR323-PTH.json
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Owon/PIR323.json
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Owon/PR412.json
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Owon/THS317-ET.json
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Owon/THS317.json
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Owon/VBS308.json
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Owon/WSP402.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:48:30.906390 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/1744130P7.json
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/440400982841.json
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/440400982842.json
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/5041131P9.json
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/929002376101.json
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/929003052501_01.json
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/929003052501_02.json
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/929003053301_01.json
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/929003053301_02.json
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/929003054701.json
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/LCA001.json
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/LCT001.json
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/LCT003.json
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/LCT007.json
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/LCT010.json
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/LCT015.json
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/LCT024.json
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/LLC010.json
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/LOM001.json
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/LOM002.json
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/LOM008.json
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/LST002.json
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/LTA001.json
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/LTC001.json
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/LTG002.json
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/LTW001.json
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/LTW004.json
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/LTW010.json
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/LTW012.json
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/LTW013.json
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/LWA001.json
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/LWA004.json
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/LWA009.json
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/LWA018.json
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/LWB006.json
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/LWB010.json
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/LWE004.json
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/LWG004.json
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/LWO001.json
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/ROM001.json
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/RWL021.json
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/RWL022.json
--rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/SML001.json
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/SML002.json
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/SML003.json
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/SML004.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:48:30.906390 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Profalux/
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Profalux/BSO-Profalux.json
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Profalux/MAI-ZTS.json
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Profalux/MOT-C1Z06C.json
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Profalux/MOT-C1Z06F.json
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Profalux/Telecommande-Profalux.json
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Profalux/Volet-Profalux.json
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Profalux/VoletBSO-Profalux.json
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:48:30.906390 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Robb-Smarrt/
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Robb-Smarrt/ROB_200-004-0.json
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Robb-Smarrt/ROB_200-017-0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:48:30.906390 z4d_certified_devices-4.259/z4d_certified_devices/Certified/SALUS/
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/SALUS/SPE600.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:48:30.906390 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Samotech/
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Samotech/SM309.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:48:30.910390 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Schneider/
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Schneider/1GANGSHUTTER1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Schneider/CCT592011_AS.json
--rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Schneider/EH-ZB-BMS.json
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Schneider/EH-ZB-HACT.json
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Schneider/EH-ZB-LMACT.json
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Schneider/EH-ZB-RTS.json
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Schneider/EH-ZB-SPD-V2.json
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Schneider/EH-ZB-SPD.json
--rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Schneider/EH-ZB-VACT.json
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Schneider/NHPBSHUTTER1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Schneider/PUCKDIMMER1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Schneider/PUCKSHUTTER1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Schneider/PUCKSWITCH1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Schneider/SOCKETOUTLET1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Schneider/SOCKETOUTLET2.json
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Schneider/Wiser2-Thermostat.json
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Schneider/iTRV.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:48:30.910390 z4d_certified_devices-4.259/z4d_certified_devices/Certified/SmartThings/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/SmartThings/outletv4.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:48:30.914390 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Sonoff/
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Sonoff/01MINIZB.json
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Sonoff/66666-motion.json
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Sonoff/66666-temphumi.json
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Sonoff/66666.json
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Sonoff/BASICZBR3.json
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Sonoff/CK-BL702-SWP-01(7020).json
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Sonoff/DONGLE-E_R.json
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Sonoff/DS-01.json
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Sonoff/DS01.json
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Sonoff/MS01.json
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Sonoff/MSO1.json
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Sonoff/S26R2ZB.json
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Sonoff/SA-030-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Sonoff/SNZB-01P.json
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Sonoff/SNZB-02.json
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Sonoff/SNZB-02D.json
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Sonoff/SNZB-02P.json
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Sonoff/SNZB-03P.json
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Sonoff/SNZB-06P.json
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Sonoff/TH01.json
--rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Sonoff/TRVZB.json
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Sonoff/WB-01.json
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Sonoff/WB01.json
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Sonoff/ZBMINI-L.json
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Sonoff/ZBMINI-L2.json
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Sonoff/ZBMINIL2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:48:30.914390 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Sunricher/
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Sunricher/HK-SL-DIM-A.json
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Sunricher/ZG2858A.json
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Sunricher/ZG9101SAC-HP.json
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Sunricher/ZGRC-KEY-013.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:48:30.914390 z4d_certified_devices-4.259/z4d_certified_devices/Certified/TDURM0D01/
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/TDURM0D01/ZBT-Remote-ALL-RGBW.json
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/TDURM0D01/tint-ExtendedColor.json
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/TDURM0D01/tint-Remote-white.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:48:30.914390 z4d_certified_devices-4.259/z4d_certified_devices/Certified/TUYATEC/
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/TUYATEC/RH3001.json
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/TUYATEC/RH3040.json
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/TUYATEC/RH3052.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:48:30.934390 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0001.json
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0002.json
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0002_relay_switch.json
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0003-QS-Zigbee-S05-LN.json
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0003.json
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0003_relay_switch.json
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0004-_TZ3000_excgg5kb.json
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0004-_TZ3000_u3oupgdy.json
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0004-relay_switch.json
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0004.json
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0011.json
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0012.json
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0013.json
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0041.json
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0042.json
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0043.json
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0044.json
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0046.json
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS004F-_TZ3000_xabckq1v.json
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS004F.json
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0112.json
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0115.json
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS011F-2Gang-switches.json
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS011F-2gang-plug.json
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS011F-_TZ3000_zmy1waw6.json
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS011F-din.json
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS011F-multiprise.json
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS011F-plug-Elivco.json
--rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS011F-plug.json
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS011F-with_threshold.json
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS011F.json
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0121.json
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0201-Temp-Humi-10.json
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0201-Temp-Humi-IH-K009.json
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0201-_TZ3000_mxzo5rhf.json
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0201-_TZ3000_qaaysllp.json
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0201.json
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0202-WHD02.json
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0202-_TZ3210_jijr1sss.json
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0202.json
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0203.json
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0205.json
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0207-extender.json
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0207-waterleak.json
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0210.json
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0211.json
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0215A-secure-remote.json
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0215A-sos.json
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0219.json
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0222.json
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0224.json
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0225.json
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0302.json
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0502A.json
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0502B.json
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0503B.json
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0505A-HueSaturation.json
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0505A.json
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0505B.json
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-2Gangs-dimmer.json
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-2Gangs-switch.json
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-BLE-YL01.json
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-Clamp-Meter.json
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-Energy.json
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-Human-Presence.json
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-Irrigation-Valve.json
--rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-PC311-Z-TY.json
--rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-PC321-Z-TY.json
--rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-PJ-1203A.json
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-Parkside-Watering-Timer.json
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-Ronelabs-SEM101.json
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-Ronelabs-SEM301.json
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-SZ-T04.json
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-Smart-CO.json
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-Smart-Energy-1P+N.json
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-SmartAir.json
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-SmartAirHouseKeeper.json
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-Solar-Siren.json
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-WZ-M100-C.json
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-XOCA-DAC2161C.json
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-_TZE200_b6wax7g0.json
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-_TZE200_chyvmhay.json
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-_TZE200_dzuqwsyg.json
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-_TZE200_nklqjk62.json
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-_TZE200_t1blo2bj.json
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-curtain.json
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-dimmer.json
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-eTRV.json
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-eTRV1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-eTRV2.json
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-eTRV3.json
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-eTRV5.json
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-eTRV6.json
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-eTRV7.json
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-motion.json
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-photoelectric-smoke.json
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-radar.json
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-sirene.json
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-smoke.json
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-soil-sensor.json
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-switch.json
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-temphumi-2.json
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-temphumi.json
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-temphumix10.json
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-thermostat.json
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS1001.json
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS110E-SMD-02Z.json
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS110E-_QS-Zigbee-D02-TRIAC-LN.json
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS110E-_TZ3210_weaqkhab.json
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS110F-2gang-dimmer.json
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS110F-_TYZB01_qezuin6k.json
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS110F-_TZ3000_ktuoyvt5.json
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS110F-dimmer.json
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS130F-Blind.json
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_1dd0d5yi-Blind.json
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_1dd0d5yi-Vanne.json
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_1dd0d5yi.json
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_8kzqqzu4.json
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_dph3rpss.json
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_femsaaua.json
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_fvhunhxb.json
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_zirycpws.json
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TY0202.json
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/fvq6avy.json
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/ivfvd7h.json
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/kud7u2l.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:48:30.934390 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Woolley/
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Woolley/SA-029-1.json
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Woolley/Z111PL0H-1JX.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:48:30.934390 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Ynoa/
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Ynoa/ZBT-CCTLight-A0001.json
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Ynoa/ZBT-CCTLight-GU100001.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:48:30.934390 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Ysrai/
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Ysrai/ZB-CL01.json
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Ysrai/ZB-CT01.json
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Ysrai/ZB-DL01.json
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Ysrai/ZB-SW01.json
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Ysrai/ZB-SW02.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:48:30.934390 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Zehnder/
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Zehnder/TAFFETAS2 D1.00P1.01Z1.00.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:48:30.938391 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Zemismart/
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/Zemismart/LXN56-DC27LX1.1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:48:30.938391 z4d_certified_devices-4.259/z4d_certified_devices/Certified/eWeLink/
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/eWeLink/SA-003-Zigbee.json
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/eWeLink/SA-030-1.json
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/eWeLink/SWITCH-ZR02.json
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/Certified/eWeLink/SWITCH-ZR03-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-27 16:48:27.000000 z4d_certified_devices-4.259/z4d_certified_devices/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 16:48:30.938391 z4d_certified_devices-4.259/z4d_certified_devices.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    36878 2024-04-27 16:48:30.000000 z4d_certified_devices-4.259/z4d_certified_devices.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    34330 2024-04-27 16:48:30.000000 z4d_certified_devices-4.259/z4d_certified_devices.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 16:48:30.000000 z4d_certified_devices-4.259/z4d_certified_devices.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-27 16:48:30.000000 z4d_certified_devices-4.259/z4d_certified_devices.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 16:48:30.000000 z4d_certified_devices-4.259/z4d_certified_devices.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:11:51.941836 z4d_certified_devices-5.260/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    36878 2024-05-02 12:11:51.941836 z4d_certified_devices-5.260/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-02 12:11:51.941836 z4d_certified_devices-5.260/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:11:51.849836 z4d_certified_devices-5.260/z4d_certified_devices/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:11:51.849836 z4d_certified_devices-5.260/z4d_certified_devices/Certified/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:11:51.849836 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Adeo/
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Adeo/LDSENK02F.json
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Adeo/LDSENK10.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Adeo/LXEK-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Adeo/LXEK-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Adeo/LXEK-7.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Adeo/SIN-4-1-20_LEX.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Adeo/SIN-4-FP-21_EQU.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Adeo/SIN-4-RS-20_LEX.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Adeo/ZBEK-13.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Adeo/ZBEK-14.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Adeo/ZBEK-3.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:11:51.849836 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Aeotec/
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Aeotec/aeotec-button.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Aeotec/aeotec-water.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:11:51.849836 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Aotec/
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Aotec/WG001-Z01.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:11:51.853836 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Bitron/
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Bitron/90201021A.json
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Bitron/90201021B.json
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Bitron/90201024.json
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Bitron/AV201021B.json
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Bitron/AV201024A.json
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Bitron/AV201029A.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:11:51.853836 z4d_certified_devices-5.260/z4d_certified_devices/Certified/CLEODE/
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/CLEODE/ZHUM.json
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/CLEODE/ZMOVE.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/CLEODE/ZPLUG.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:11:51.853836 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Candeo/
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Candeo/Candeo Zigbee Dimmer.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Candeo/HK-DIM-A.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:11:51.853836 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Casa.ia/
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Casa.ia/CAC221.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Casa.ia/CCB432.json
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Casa.ia/CDWS312.json
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Casa.ia/CKF204.json
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Casa.ia/CKF205.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Casa.ia/CMS323.json
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Casa.ia/CPB206.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Casa.ia/CPC321.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Casa.ia/CPR412-E.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Casa.ia/CPR412.json
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Casa.ia/CSAC451-E.json
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Casa.ia/CSAC451-WTC-E.json
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Casa.ia/CSLC601-D-E.json
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Casa.ia/CSLC601-E.json
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Casa.ia/CSLC631-3.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Casa.ia/CSP403.json
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Casa.ia/CTHS317ET.json
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Casa.ia/Dual_Relay_Module.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:11:51.857836 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Chameleon/
+-rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Chameleon/MWA1-TIC-historique-mono-base.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Chameleon/MWA1-TIC-historique-mono-ejp.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Chameleon/MWA1-TIC-historique-mono-hchp.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Chameleon/MWA1-TIC-historique-mono-tempo.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11271 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Chameleon/MWA1-TIC-standard-mono-base.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11271 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Chameleon/MWA1-TIC.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:11:51.857836 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Custom/
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Custom/LYWSD03MMC.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:11:51.857836 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Danalock/
+-rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Danalock/V3-BTZB.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:11:51.857836 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Danfoss/
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Danfoss/RV001.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Danfoss/eT093WRG.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Danfoss/eT093WRO.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Danfoss/eTRV0100.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:11:51.857836 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Develco/
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Develco/AQSZB-110.json
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Develco/EMIZB-141.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Develco/HESZB120.json
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Develco/HMSZB-110.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Develco/MOSZB-140.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Develco/SMSZB-120.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Develco/SPLZB-131.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Develco/SPLZB-132.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Develco/WISZB-120.json
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Develco/ZHEMI101.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:11:51.857836 z4d_certified_devices-5.260/z4d_certified_devices/Certified/ENKI-LEXMAN/
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/ENKI-LEXMAN/LXEK-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/ENKI-LEXMAN/LXEK-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/ENKI-LEXMAN/LXEK-7.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:11:51.861836 z4d_certified_devices-5.260/z4d_certified_devices/Certified/EcoDim/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/EcoDim/Dimmer-Switch-ZB3.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/EcoDim/Eco-Dim.07Eco-Dim.10.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/EcoDim/EcoDim-Zigbee 3.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:11:51.861836 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Eurotronics/
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Eurotronics/SPZB0001.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:11:51.861836 z4d_certified_devices-5.260/z4d_certified_devices/Certified/GLEDOPTO/
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/GLEDOPTO/GL-B-004P.json
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/GLEDOPTO/GL-B-007Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/GLEDOPTO/GL-B-008Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/GLEDOPTO/GL-B-008ZS.json
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/GLEDOPTO/GL-C-007-2ID.json
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/GLEDOPTO/GL-C-007.json
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/GLEDOPTO/GL-C-008.json
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/GLEDOPTO/GL-C-008S.json
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/GLEDOPTO/GL-C-008Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/GLEDOPTO/GL-C-009.json
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/GLEDOPTO/GL-D-003Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/GLEDOPTO/GL-FL-004TZS.json
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/GLEDOPTO/GL-MC-001.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/GLEDOPTO/GL-S-007ZS.json
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/GLEDOPTO/GLEDOPTO.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:11:51.865836 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Heiman/
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Heiman/COSensor-EF-3.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Heiman/COSensor-EM.json
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Heiman/COSensor-N.json
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Heiman/CO_V15.json
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Heiman/CO_YDLV10.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Heiman/DoorBell-EF-3.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Heiman/GASSensor-EF-3.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Heiman/GAS_V15.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Heiman/HS3AQ-EFA-3.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Heiman/RC-EF-3.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Heiman/RC-EM.json
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Heiman/SMOK_V16.json
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Heiman/SMOK_YDLV10.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Heiman/SRHMP-I1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Heiman/SceneSwitch-EM-3.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Heiman/SmartPlug.json
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Heiman/SmokeSensor-EF-3.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Heiman/SmokeSensor-EM.json
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Heiman/SmokeSensor-N-3.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Heiman/SmokeSensor-N.json
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Heiman/TS0216.json
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Heiman/WarningDevice-EF-3.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Heiman/WarningDevice.json
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Heiman/WaterSensor-EF-3.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:11:51.873836 z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/FLOALT panel WS 30x90.json
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/FLOALT panel WS 60x60.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/FYRTUR block-out roller blind.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/KADRILJ roller blind.json
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/PARASOLL DoorWindow Sensor.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/Remote Control N2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/STARKVIND Air purifier.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/STOFTMOLN ceilingwall lamp WW24.json
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI Driver 10W.json
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI Driver 30W.json
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI SHORTCUT Button.json
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI Signal Repeater.json
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E12 WS opal 400lm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E14 W opch 400lm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E14 WS 470lm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E14 WS opal 400lm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E14 WS opal 600lm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E26 WS clear 950lm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E26 WS opal 980lm.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 CWS 806lm.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 CWS opal 600lm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 W opal 1000lm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WS clear 806lm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WS clear 950lm.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WS globe 1055lm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WS opal 1000lm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WS opal 950lm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WS opal 980lm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WW 806lm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WW clear 250lm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 opal 1000lm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb GU10 W 400lm.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb GU10 WS 345lm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb GU10 WS 400lm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb GU10 WW 400lm.json
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI control outlet.json
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI motion sensor.json
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI onoff switch.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI openclose remote.json
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI remote control.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI transformer 10W.json
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI wireless dimmer.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRIbulbE14WScandleopal470lm.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRIbulbE14WSglobeopal470lm.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRIbulbE14WWclear250lm.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRIbulbE27WSglobeopal1055lm.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRIbulbE27WWclear250lm.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRIbulbGU10WS345lm.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/VINDSTYRKA.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:11:51.873836 z4d_certified_devices-5.260/z4d_certified_devices/Certified/INNR/
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/INNR/OSL 130 C.json
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/INNR/PL 110.json
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/INNR/PL 115.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/INNR/RB 248 T.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/INNR/RB 285 C.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/INNR/SP 120.json
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/INNR/SP 220.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:11:51.873836 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Idinio/
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Idinio/Dimmer-Switch-ZB3.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:11:51.873836 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Iluminize/
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Iluminize/511.201.json
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Iluminize/5120.1200.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:11:51.877836 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Konke/
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Konke/3AFE140103020000.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Konke/3AFE14010402000D.json
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Konke/3AFE170100510001.json
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Konke/3AFE220103020000.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Konke/3AFE28010402000D.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:11:51.877836 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LIVOLO/
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LIVOLO/TI0001.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:11:51.877836 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LS-Deutschland-GmbH/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LS-Deutschland-GmbH/Emotion.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:11:51.885836 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.airmonitor.acn01.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.ctrl_86plug.aq1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.ctrl_86plug.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.ctrl_ln2.aq1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.ctrl_ln2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.ctrl_neutral1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.ctrl_neutral2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.curtain.acn002.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.light.aqcn02.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.lock.v1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.magnet.acn001.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.magnet.agl02.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.motion.ac01.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.motion.ac02.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.plug.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4643 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.plug.maeu01.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.plug.mmeu01.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.relay.c2acn01.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.remote.acn003.json
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.remote.b186acn01.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.remote.b186acn02.json
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.remote.b1acn01.json
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.remote.b286acn01.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.remote.b286acn02.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.remote.b286opcn01-bulb.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.remote.b286opcn01.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.remote.b28ac1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.remote.b486opcn01-bulb.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.remote.b486opcn01.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.remote.b686opcn01-bulb.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.remote.b686opcn01.json
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.router.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.sen_ill.mgl01.json
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.sens.json
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.sensor_86sw1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.sensor_86sw2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.sensor_cube.aqgl01.json
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.sensor_cube.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.sensor_ht.agl02.json
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.sensor_ht.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.sensor_magnet.acn001.json
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.sensor_magnet.aq2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.sensor_magnet.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.sensor_motion.aq2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.sensor_motion.json
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.sensor_natgas.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.sensor_smoke.acn03.json
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.sensor_smoke.json
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.sensor_swit.json
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.sensor_switch.aq2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.sensor_switch.aq3.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.sensor_switch.aq3t.json
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.sensor_switch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.sensor_wleak.aq1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.switch.acn047.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.switch.b1lacn02.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.switch.b2lacn02.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.switch.b2lc04.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.switch.l0agl1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.switch.l1aeu1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.switch.l2aeu1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.switch.n0agl1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.switch.n1aeu1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.vibration.aq1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.weather.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:11:51.889836 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Legrand/
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Legrand/Cable outlet.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Legrand/Connected outlet.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Legrand/DIN power consumption module.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Legrand/Dimmer switch wo neutral.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Legrand/Double gangs remote switch.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Legrand/Micromodule switch.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Legrand/Mobile outlet.json
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Legrand/Remote motion sensor.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Legrand/Remote switch Wake up Sleep.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Legrand/Remote switch.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Legrand/Remote toggle switch.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Legrand/Shutter switch with neutral.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Legrand/Shutters central remote switch.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Legrand/Teleruptor.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:11:51.889836 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Lixee/
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Lixee/WS2812_light_controller.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-historique-mono.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-historique-tri.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5459 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-standard-mono-prod.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-standard-mono.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6879 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-standard-tri-prod.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5764 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-standard-tri.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Lixee/ZLinky_TIC.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Lixee/ZiPulses.json
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Lixee/Zigate-Router.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:11:51.889836 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Nexturn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Nexturn/VOC_Sensor.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:11:51.893836 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Nodon/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Nodon/SIN-4-1-20.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Nodon/SIN-4-FP-21.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Nodon/SIN-4-RS-20.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Nodon/SIN-4-RS-20_PRO.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:11:51.893836 z4d_certified_devices-5.260/z4d_certified_devices/Certified/OSRAM/
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/OSRAM/CLA60 TW OSRAM.json
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/OSRAM/Classic A60 W clear - LIGHTIFY.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/OSRAM/LEDVANCE DIM.json
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/OSRAM/LIGHTIFY Indoor Flex RGBW.json
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/OSRAM/LIGHTIFY Outdoor Flex RGBW.json
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/OSRAM/Lightify Switch Mini.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/OSRAM/PAR 16 50 RGBW - LIGHTIFY.json
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/OSRAM/PAR16 50 TW.json
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/OSRAM/Plug 01.json
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/OSRAM/Plug Z3.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:11:51.893836 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Orvibo/
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Orvibo/396483ce8b3f4e0d8e9d79079a35a420.json
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Orvibo/3c4e4fc81ed442efaf69353effcdfc5f.json
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Orvibo/50938c4c3c0b4049923cd5afbc151bde.json
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Orvibo/82c167c95ed746cdbd21d6817f72c593.json
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Orvibo/898ca74409a740b28d5841661e72268d.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:11:51.897836 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Others/
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Others/BDP3001.json
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Others/Dimmablelight.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Others/EcoDim-Zigbee 3.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Others/FB56-ZCW08KU1.1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Others/FNB56-ZCW25FB1.6.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Others/FNB56-ZCW25FB2.1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Others/FNB56-ZSW01LX2.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Others/FNB56-ZSW02LX2.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Others/Lamp_01.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Others/NUET56-DL27LX1.1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Others/SA-003-Zigbee.json
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Others/VMS_ADUROLIGHT.json
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Others/ZB-CL01.json
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Others/ZB-CT01.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Others/ZB-ONOFFPlug-D0005.json
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Others/ZB-SW01.json
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Others/ZB-SW02.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:11:51.901836 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Owon/
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Owon/AC201A.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Owon/AC211.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Owon/AC221.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Owon/CB432.json
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Owon/DWS312-E.json
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Owon/DWS312.json
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Owon/KF204.json
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Owon/KF205.json
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Owon/PB206.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Owon/PC321.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Owon/PIR323-A.json
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Owon/PIR323-PTH.json
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Owon/PIR323.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Owon/PR412.json
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Owon/THS317-ET.json
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Owon/THS317.json
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Owon/VBS308.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Owon/WSP402.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:11:51.905836 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/1744130P7.json
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/440400982841.json
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/440400982842.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/5041131P9.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/929002376101.json
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/929003052501_01.json
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/929003052501_02.json
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/929003053301_01.json
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/929003053301_02.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/929003054701.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/LCA001.json
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/LCT001.json
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/LCT003.json
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/LCT007.json
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/LCT010.json
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/LCT015.json
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/LCT024.json
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/LLC010.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/LOM001.json
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/LOM002.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/LOM008.json
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/LST002.json
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/LTA001.json
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/LTC001.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/LTG002.json
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/LTW001.json
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/LTW004.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/LTW010.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/LTW012.json
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/LTW013.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/LWA001.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/LWA004.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/LWA009.json
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/LWA018.json
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/LWB006.json
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/LWB010.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/LWE004.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/LWG004.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/LWO001.json
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/ROM001.json
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/RWL021.json
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/RWL022.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/SML001.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/SML002.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/SML003.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/SML004.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:11:51.909836 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Profalux/
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Profalux/BSO-Profalux.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Profalux/MAI-ZTS.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Profalux/MOT-C1Z06C.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Profalux/MOT-C1Z06F.json
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Profalux/Telecommande-Profalux.json
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Profalux/Volet-Profalux.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Profalux/VoletBSO-Profalux.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:11:51.909836 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Robb-Smarrt/
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Robb-Smarrt/ROB_200-004-0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Robb-Smarrt/ROB_200-017-0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:11:51.909836 z4d_certified_devices-5.260/z4d_certified_devices/Certified/SALUS/
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/SALUS/SPE600.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:11:51.909836 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Samotech/
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Samotech/SM309.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:11:51.909836 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Schneider/
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Schneider/1GANGSHUTTER1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Schneider/CCT592011_AS.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Schneider/EH-ZB-BMS.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Schneider/EH-ZB-HACT.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Schneider/EH-ZB-LMACT.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Schneider/EH-ZB-RTS.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Schneider/EH-ZB-SPD-V2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Schneider/EH-ZB-SPD.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Schneider/EH-ZB-VACT.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Schneider/NHPBSHUTTER1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Schneider/PUCKDIMMER1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Schneider/PUCKSHUTTER1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Schneider/PUCKSWITCH1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Schneider/SOCKETOUTLET1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Schneider/SOCKETOUTLET2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Schneider/Wiser2-Thermostat.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Schneider/iTRV.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:11:51.913836 z4d_certified_devices-5.260/z4d_certified_devices/Certified/SmartThings/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/SmartThings/outletv4.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:11:51.917836 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Sonoff/
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Sonoff/01MINIZB.json
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Sonoff/66666-motion.json
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Sonoff/66666-temphumi.json
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Sonoff/66666.json
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Sonoff/BASICZBR3.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Sonoff/CK-BL702-SWP-01(7020).json
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Sonoff/DONGLE-E_R.json
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Sonoff/DS-01.json
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Sonoff/DS01.json
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Sonoff/MS01.json
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Sonoff/MSO1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Sonoff/S26R2ZB.json
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Sonoff/SA-030-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Sonoff/SNZB-01P.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Sonoff/SNZB-02.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Sonoff/SNZB-02D.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Sonoff/SNZB-02P.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Sonoff/SNZB-03P.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Sonoff/SNZB-06P.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Sonoff/TH01.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Sonoff/TRVZB.json
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Sonoff/WB-01.json
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Sonoff/WB01.json
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Sonoff/ZBMINI-L.json
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Sonoff/ZBMINI-L2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Sonoff/ZBMINIL2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:11:51.917836 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Sunricher/
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Sunricher/HK-SL-DIM-A.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Sunricher/ZG2858A.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Sunricher/ZG9101SAC-HP.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Sunricher/ZGRC-KEY-013.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:11:51.917836 z4d_certified_devices-5.260/z4d_certified_devices/Certified/TDURM0D01/
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/TDURM0D01/ZBT-Remote-ALL-RGBW.json
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/TDURM0D01/tint-ExtendedColor.json
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/TDURM0D01/tint-Remote-white.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:11:51.917836 z4d_certified_devices-5.260/z4d_certified_devices/Certified/TUYATEC/
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/TUYATEC/RH3001.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/TUYATEC/RH3040.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/TUYATEC/RH3052.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:11:51.937836 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0001.json
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0002.json
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0002_relay_switch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0003-QS-Zigbee-S05-LN.json
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0003.json
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0003_relay_switch.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0004-_TZ3000_excgg5kb.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0004-_TZ3000_u3oupgdy.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0004-relay_switch.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0004.json
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0011.json
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0012.json
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0013.json
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0041.json
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0042.json
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0043.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0044.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0046.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS004F-_TZ3000_xabckq1v.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS004F.json
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0112.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0115.json
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS011F-2Gang-switches.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS011F-2gang-plug.json
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS011F-_TZ3000_zmy1waw6.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS011F-din.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS011F-multiprise.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS011F-plug-Elivco.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS011F-plug.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS011F-with_threshold.json
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS011F.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0121.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0201-Temp-Humi-10.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0201-Temp-Humi-IH-K009.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0201-_TZ3000_mxzo5rhf.json
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0201-_TZ3000_qaaysllp.json
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0201.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0202-WHD02.json
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0202-_TZ3210_jijr1sss.json
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0202.json
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0203.json
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0205.json
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0207-extender.json
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0207-waterleak.json
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0210.json
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0211.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0215A-secure-remote.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0215A-sos.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0219.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0222.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0224.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0225.json
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0302.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0502A.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0502B.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0503B.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0505A-HueSaturation.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0505A.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0505B.json
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-2Gangs-dimmer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-2Gangs-switch.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-BLE-YL01.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-Clamp-Meter.json
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-Energy.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-Human-Presence.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-Irrigation-Valve.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-PC311-Z-TY.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-PC321-Z-TY.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-PJ-1203A.json
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-Parkside-Watering-Timer.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-Ronelabs-SEM101.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-Ronelabs-SEM301.json
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-SZ-T04.json
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-Smart-CO.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-Smart-Energy-1P+N.json
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-SmartAir.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-SmartAirHouseKeeper.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-Solar-Siren.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-WZ-M100-C.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-XOCA-DAC2161C.json
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-_TZE200_b6wax7g0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-_TZE200_chyvmhay.json
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-_TZE200_dzuqwsyg.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-_TZE200_nklqjk62.json
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-_TZE200_t1blo2bj.json
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-curtain.json
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-dimmer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-eTRV.json
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-eTRV1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-eTRV2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-eTRV3.json
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-eTRV5.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-eTRV6.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-eTRV7.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-motion.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-photoelectric-smoke.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-radar.json
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-sirene.json
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-smoke.json
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-soil-sensor.json
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-switch.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-temphumi-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-temphumi.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-temphumix10.json
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-thermostat.json
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS1001.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS110E-SMD-02Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS110E-_QS-Zigbee-D02-TRIAC-LN.json
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS110E-_TZ3210_weaqkhab.json
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS110F-2gang-dimmer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS110F-_TYZB01_qezuin6k.json
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS110F-_TZ3000_ktuoyvt5.json
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS110F-dimmer.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS130F-Blind.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_1dd0d5yi-Blind.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_1dd0d5yi-Vanne.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_1dd0d5yi.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_8kzqqzu4.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_dph3rpss.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_femsaaua.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_fvhunhxb.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_zirycpws.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TY0202.json
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/fvq6avy.json
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/ivfvd7h.json
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/kud7u2l.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:11:51.937836 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Woolley/
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Woolley/SA-029-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Woolley/Z111PL0H-1JX.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:11:51.937836 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Ynoa/
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Ynoa/ZBT-CCTLight-A0001.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Ynoa/ZBT-CCTLight-GU100001.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:11:51.941836 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Ysrai/
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Ysrai/ZB-CL01.json
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Ysrai/ZB-CT01.json
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Ysrai/ZB-DL01.json
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Ysrai/ZB-SW01.json
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Ysrai/ZB-SW02.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:11:51.941836 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Zehnder/
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Zehnder/TAFFETAS2 D1.00P1.01Z1.00.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:11:51.941836 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Zemismart/
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/Zemismart/LXN56-DC27LX1.1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:11:51.941836 z4d_certified_devices-5.260/z4d_certified_devices/Certified/eWeLink/
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/eWeLink/SA-003-Zigbee.json
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/eWeLink/SA-030-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/eWeLink/SWITCH-ZR02.json
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/Certified/eWeLink/SWITCH-ZR03-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-02 12:11:47.000000 z4d_certified_devices-5.260/z4d_certified_devices/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:11:51.941836 z4d_certified_devices-5.260/z4d_certified_devices.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    36878 2024-05-02 12:11:51.000000 z4d_certified_devices-5.260/z4d_certified_devices.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    34330 2024-05-02 12:11:51.000000 z4d_certified_devices-5.260/z4d_certified_devices.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 12:11:51.000000 z4d_certified_devices-5.260/z4d_certified_devices.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-02 12:11:51.000000 z4d_certified_devices-5.260/z4d_certified_devices.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 12:11:51.000000 z4d_certified_devices-5.260/z4d_certified_devices.egg-info/zip-safe
```

### Comparing `z4d_certified_devices-4.259/LICENSE.txt` & `z4d_certified_devices-5.260/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/PKG-INFO` & `z4d_certified_devices-5.260/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: z4d-certified-devices
-Version: 4.259
+Version: 5.260
 Summary: "Certified devices for Zigbee for Domoticz plugin"
 Home-page: https://github.com/zigbeefordomoticz/z4d-certified-devices
 Author: "Patrick Pichon"
 Author-email: "patrick@pichon.me"
 License: "GPL-3.0"
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: z4d-certified-devices Version: 4.259 Summary:
+Metadata-Version: 2.1 Name: z4d-certified-devices Version: 5.260 Summary:
 "Certified devices for Zigbee for Domoticz plugin" Home-page: https://
 github.com/zigbeefordomoticz/z4d-certified-devices Author: "Patrick Pichon"
 Author-email: "patrick@pichon.me" License: "GPL-3.0" Classifier: Programming
 Language :: Python :: 3 Description-Content-Type: text/markdown License-File:
 LICENSE.txt # z4d-certified-devices ## Overview This package is required for
 the [Zigbee for Domoticz](https://github.com/zigbeefordomoticz/Domoticz-Zigbee)
 plugin. It provides configuration files to optimized the pairing and behaviour
```

### Comparing `z4d_certified_devices-4.259/README.md` & `z4d_certified_devices-5.260/README.md`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/setup.cfg` & `z4d_certified_devices-5.260/setup.cfg`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Adeo/LDSENK02F.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Adeo/LDSENK02F.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Adeo/LDSENK10.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Adeo/LDSENK10.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Adeo/LXEK-1.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Adeo/LXEK-1.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Adeo/LXEK-2.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Adeo/LXEK-2.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Adeo/LXEK-7.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Adeo/LXEK-7.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Adeo/SIN-4-1-20_LEX.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Adeo/SIN-4-1-20_LEX.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Adeo/SIN-4-FP-21_EQU.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Adeo/SIN-4-FP-21_EQU.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Adeo/SIN-4-RS-20_LEX.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Adeo/SIN-4-RS-20_LEX.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Adeo/ZBEK-13.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Adeo/ZBEK-13.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Adeo/ZBEK-14.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Adeo/ZBEK-14.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Adeo/ZBEK-3.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Adeo/ZBEK-3.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Aeotec/aeotec-button.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Aeotec/aeotec-button.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Aeotec/aeotec-water.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Aeotec/aeotec-water.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Aotec/WG001-Z01.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Aotec/WG001-Z01.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Bitron/90201021A.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Bitron/90201021A.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Bitron/AV201024A.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Bitron/AV201024A.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Bitron/AV201029A.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Bitron/AV201029A.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/CLEODE/ZHUM.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/CLEODE/ZHUM.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/CLEODE/ZMOVE.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/CLEODE/ZMOVE.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/CLEODE/ZPLUG.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/CLEODE/ZPLUG.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Candeo/Candeo Zigbee Dimmer.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Candeo/Candeo Zigbee Dimmer.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Candeo/HK-DIM-A.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Candeo/HK-DIM-A.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Casa.ia/CAC221.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Casa.ia/CAC221.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Casa.ia/CCB432.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Casa.ia/CCB432.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Casa.ia/CDWS312.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Casa.ia/CDWS312.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Casa.ia/CKF205.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Casa.ia/CKF205.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Casa.ia/CMS323.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Casa.ia/CMS323.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Casa.ia/CPC321.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Casa.ia/CPC321.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Casa.ia/CPR412-E.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Casa.ia/CPR412-E.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Casa.ia/CPR412.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Casa.ia/CPR412.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Casa.ia/CSAC451-E.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Casa.ia/CSAC451-E.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Casa.ia/CSAC451-WTC-E.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Casa.ia/CSAC451-WTC-E.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Casa.ia/CSLC601-D-E.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Casa.ia/CSLC601-D-E.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Casa.ia/CSLC601-E.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Casa.ia/CSLC601-E.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Casa.ia/CSLC631-3.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Casa.ia/CSLC631-3.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Casa.ia/CSP403.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Casa.ia/CSP403.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Casa.ia/CTHS317ET.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Casa.ia/CTHS317ET.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Casa.ia/Dual_Relay_Module.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Casa.ia/Dual_Relay_Module.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Chameleon/MWA1-TIC-historique-mono-base.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Chameleon/MWA1-TIC-historique-mono-base.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Chameleon/MWA1-TIC-historique-mono-ejp.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Chameleon/MWA1-TIC-historique-mono-ejp.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Chameleon/MWA1-TIC-historique-mono-hchp.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Chameleon/MWA1-TIC-historique-mono-hchp.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Chameleon/MWA1-TIC-historique-mono-tempo.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Chameleon/MWA1-TIC-historique-mono-tempo.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Chameleon/MWA1-TIC-standard-mono-base.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Chameleon/MWA1-TIC-standard-mono-base.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Chameleon/MWA1-TIC.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Chameleon/MWA1-TIC.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Custom/LYWSD03MMC.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Custom/LYWSD03MMC.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Danalock/V3-BTZB.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Danalock/V3-BTZB.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Danfoss/RV001.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Danfoss/RV001.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Danfoss/eT093WRG.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Danfoss/eT093WRG.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Danfoss/eT093WRO.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Danfoss/eT093WRO.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Danfoss/eTRV0100.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Danfoss/eTRV0100.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Develco/AQSZB-110.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Develco/AQSZB-110.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Develco/EMIZB-141.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Develco/EMIZB-141.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Develco/HESZB120.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Develco/HESZB120.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Develco/HMSZB-110.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Develco/HMSZB-110.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Develco/MOSZB-140.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Develco/MOSZB-140.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Develco/SMSZB-120.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Develco/SMSZB-120.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Develco/SPLZB-131.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Develco/SPLZB-131.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Develco/SPLZB-132.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Develco/SPLZB-132.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Develco/WISZB-120.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Develco/WISZB-120.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Develco/ZHEMI101.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Develco/ZHEMI101.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/ENKI-LEXMAN/LXEK-1.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/ENKI-LEXMAN/LXEK-1.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/ENKI-LEXMAN/LXEK-2.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/ENKI-LEXMAN/LXEK-2.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/ENKI-LEXMAN/LXEK-7.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/ENKI-LEXMAN/LXEK-7.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/EcoDim/Dimmer-Switch-ZB3.0.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/EcoDim/Dimmer-Switch-ZB3.0.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/EcoDim/Eco-Dim.07Eco-Dim.10.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/EcoDim/Eco-Dim.07Eco-Dim.10.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/EcoDim/EcoDim-Zigbee 3.0.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/EcoDim/EcoDim-Zigbee 3.0.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Eurotronics/SPZB0001.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Eurotronics/SPZB0001.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/GLEDOPTO/GL-B-004P.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/GLEDOPTO/GL-B-004P.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/GLEDOPTO/GL-B-007Z.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/GLEDOPTO/GL-B-007Z.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/GLEDOPTO/GL-B-008Z.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/GLEDOPTO/GL-B-008Z.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/GLEDOPTO/GL-B-008ZS.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/GLEDOPTO/GL-B-008ZS.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/GLEDOPTO/GL-C-007-2ID.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/GLEDOPTO/GL-C-007-2ID.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/GLEDOPTO/GL-C-007.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/GLEDOPTO/GL-C-007.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/GLEDOPTO/GL-C-008.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/GLEDOPTO/GL-C-008.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/GLEDOPTO/GL-C-008S.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/GLEDOPTO/GL-C-008S.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/GLEDOPTO/GL-C-008Z.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/GLEDOPTO/GL-C-008Z.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/GLEDOPTO/GL-C-009.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/GLEDOPTO/GL-C-009.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/GLEDOPTO/GL-D-003Z.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/GLEDOPTO/GL-D-003Z.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/GLEDOPTO/GL-FL-004TZS.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/GLEDOPTO/GL-FL-004TZS.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/GLEDOPTO/GL-MC-001.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/GLEDOPTO/GL-MC-001.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/GLEDOPTO/GL-S-007ZS.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/GLEDOPTO/GL-S-007ZS.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/GLEDOPTO/GLEDOPTO.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/GLEDOPTO/GLEDOPTO.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Heiman/COSensor-EM.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Heiman/COSensor-EM.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Heiman/DoorBell-EF-3.0.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Heiman/DoorBell-EF-3.0.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Heiman/GASSensor-EF-3.0.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Heiman/GASSensor-EF-3.0.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Heiman/HS3AQ-EFA-3.0.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Heiman/HS3AQ-EFA-3.0.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Heiman/RC-EF-3.0.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Heiman/RC-EF-3.0.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Heiman/RC-EM.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Heiman/RC-EM.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Heiman/SRHMP-I1.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Heiman/SRHMP-I1.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Heiman/SceneSwitch-EM-3.0.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Heiman/SceneSwitch-EM-3.0.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Heiman/SmartPlug.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Heiman/SmartPlug.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Heiman/SmokeSensor-EM.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Heiman/SmokeSensor-EM.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Heiman/TS0216.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Heiman/TS0216.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Heiman/WarningDevice-EF-3.0.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Heiman/WarningDevice-EF-3.0.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Heiman/WarningDevice.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Heiman/WarningDevice.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Heiman/WaterSensor-EF-3.0.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Heiman/WaterSensor-EF-3.0.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/FLOALT panel WS 30x90.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/FLOALT panel WS 30x90.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/FLOALT panel WS 60x60.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/FLOALT panel WS 60x60.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/FYRTUR block-out roller blind.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/FYRTUR block-out roller blind.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/KADRILJ roller blind.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/KADRILJ roller blind.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/PARASOLL DoorWindow Sensor.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/PARASOLL DoorWindow Sensor.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/Remote Control N2.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/Remote Control N2.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/STARKVIND Air purifier.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/STARKVIND Air purifier.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/STOFTMOLN ceilingwall lamp WW24.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/STOFTMOLN ceilingwall lamp WW24.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI Driver 10W.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI Driver 10W.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI Driver 30W.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI Driver 30W.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI SHORTCUT Button.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI SHORTCUT Button.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI Signal Repeater.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI Signal Repeater.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E12 WS opal 400lm.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E12 WS opal 400lm.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E14 W opch 400lm.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E14 W opch 400lm.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E14 WS 470lm.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E14 WS 470lm.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E14 WS opal 400lm.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E14 WS opal 400lm.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E14 WS opal 600lm.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E14 WS opal 600lm.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E26 WS clear 950lm.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E26 WS clear 950lm.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E26 WS opal 980lm.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E26 WS opal 980lm.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 CWS 806lm.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 CWS 806lm.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 CWS opal 600lm.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 CWS opal 600lm.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 W opal 1000lm.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 W opal 1000lm.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WS clear 806lm.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WS clear 806lm.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WS clear 950lm.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WS clear 950lm.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WS globe 1055lm.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WS globe 1055lm.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WS opal 1000lm.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WS opal 1000lm.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WS opal 950lm.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WS opal 950lm.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WS opal 980lm.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WS opal 980lm.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WW 806lm.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WW 806lm.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WW clear 250lm.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 WW clear 250lm.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 opal 1000lm.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb E27 opal 1000lm.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb GU10 W 400lm.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb GU10 W 400lm.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb GU10 WS 345lm.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb GU10 WS 345lm.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb GU10 WS 400lm.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb GU10 WS 400lm.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb GU10 WW 400lm.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI bulb GU10 WW 400lm.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI control outlet.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI control outlet.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI motion sensor.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI motion sensor.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI onoff switch.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI onoff switch.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI openclose remote.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI openclose remote.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI remote control.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI remote control.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI transformer 10W.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRI transformer 10W.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRIbulbE14WScandleopal470lm.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRIbulbE14WScandleopal470lm.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRIbulbE14WSglobeopal470lm.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRIbulbE14WSglobeopal470lm.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRIbulbE14WWclear250lm.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRIbulbE14WWclear250lm.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRIbulbE27WSglobeopal1055lm.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRIbulbE27WSglobeopal1055lm.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRIbulbE27WWclear250lm.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRIbulbE27WWclear250lm.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRIbulbGU10WS345lm.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/TRADFRIbulbGU10WS345lm.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/IKEA_TRADFRI/VINDSTYRKA.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/IKEA_TRADFRI/VINDSTYRKA.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/INNR/OSL 130 C.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/INNR/OSL 130 C.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/INNR/PL 110.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/INNR/PL 110.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/INNR/PL 115.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/INNR/PL 115.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/INNR/RB 248 T.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/INNR/RB 248 T.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/INNR/RB 285 C.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/INNR/RB 285 C.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/INNR/SP 120.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/INNR/SP 120.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/INNR/SP 220.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/INNR/SP 220.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Idinio/Dimmer-Switch-ZB3.0.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Idinio/Dimmer-Switch-ZB3.0.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Iluminize/511.201.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Iluminize/511.201.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Iluminize/5120.1200.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Iluminize/5120.1200.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Konke/3AFE140103020000.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Konke/3AFE140103020000.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Konke/3AFE14010402000D.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Konke/3AFE14010402000D.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Konke/3AFE170100510001.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Konke/3AFE170100510001.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Konke/3AFE220103020000.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Konke/3AFE220103020000.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Konke/3AFE28010402000D.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Konke/3AFE28010402000D.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LIVOLO/TI0001.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LIVOLO/TI0001.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LS-Deutschland-GmbH/Emotion.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LS-Deutschland-GmbH/Emotion.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.airmonitor.acn01.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.airmonitor.acn01.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.ctrl_86plug.aq1.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.ctrl_86plug.aq1.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.ctrl_86plug.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.ctrl_86plug.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.ctrl_ln2.aq1.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.ctrl_ln2.aq1.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.ctrl_ln2.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.ctrl_ln2.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.ctrl_neutral1.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.ctrl_neutral1.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.ctrl_neutral2.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.ctrl_neutral2.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.curtain.acn002.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.curtain.acn002.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.light.aqcn02.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.light.aqcn02.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.lock.v1.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.lock.v1.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.magnet.acn001.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.magnet.acn001.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.magnet.agl02.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.magnet.agl02.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.motion.ac01.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.motion.ac01.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.motion.ac02.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.motion.ac02.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.plug.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.plug.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.plug.maeu01.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.plug.maeu01.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.plug.mmeu01.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.plug.mmeu01.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.relay.c2acn01.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.relay.c2acn01.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.remote.acn003.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.remote.acn003.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.remote.b186acn01.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.remote.b186acn01.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.remote.b186acn02.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.remote.b186acn02.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.remote.b1acn01.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.remote.b1acn01.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.remote.b286acn01.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.remote.b286acn01.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.remote.b286acn02.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.remote.b286acn02.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.remote.b286opcn01-bulb.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.remote.b286opcn01-bulb.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.remote.b286opcn01.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.remote.b286opcn01.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.remote.b28ac1.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.remote.b28ac1.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.remote.b486opcn01-bulb.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.remote.b486opcn01-bulb.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.remote.b486opcn01.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.remote.b486opcn01.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.remote.b686opcn01-bulb.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.remote.b686opcn01-bulb.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.remote.b686opcn01.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.remote.b686opcn01.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.router.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.router.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.sen_ill.mgl01.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.sen_ill.mgl01.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.sens.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.sens.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.sensor_86sw1.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.sensor_86sw1.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.sensor_86sw2.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.sensor_86sw2.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.sensor_cube.aqgl01.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.sensor_cube.aqgl01.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.sensor_cube.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.sensor_cube.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.sensor_ht.agl02.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.sensor_ht.agl02.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.sensor_ht.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.sensor_ht.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.sensor_magnet.acn001.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.sensor_magnet.acn001.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.sensor_magnet.aq2.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.sensor_magnet.aq2.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.sensor_magnet.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.sensor_magnet.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.sensor_motion.aq2.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.sensor_motion.aq2.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.sensor_motion.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.sensor_motion.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.sensor_natgas.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.sensor_natgas.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.sensor_smoke.acn03.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.sensor_smoke.acn03.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.sensor_smoke.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.sensor_smoke.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.sensor_swit.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.sensor_swit.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.sensor_switch.aq2.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.sensor_switch.aq2.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.sensor_switch.aq3.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.sensor_switch.aq3.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.sensor_switch.aq3t.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.sensor_switch.aq3t.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.sensor_switch.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.sensor_switch.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.sensor_wleak.aq1.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.sensor_wleak.aq1.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.switch.acn047.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.switch.acn047.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.switch.b1lacn02.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.switch.b1lacn02.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.switch.b2lacn02.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.switch.b2lacn02.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.switch.b2lc04.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.switch.b2lc04.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.switch.l0agl1.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.switch.l0agl1.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.switch.l1aeu1.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.switch.l1aeu1.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.switch.l2aeu1.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.switch.l2aeu1.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.switch.n0agl1.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.switch.n0agl1.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.switch.n1aeu1.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.switch.n1aeu1.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.vibration.aq1.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.vibration.aq1.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/LUMI/lumi.weather.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/LUMI/lumi.weather.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Legrand/Cable outlet.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Legrand/Cable outlet.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Legrand/Connected outlet.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Legrand/Connected outlet.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Legrand/DIN power consumption module.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Legrand/DIN power consumption module.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Legrand/Dimmer switch wo neutral.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Legrand/Dimmer switch wo neutral.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Legrand/Double gangs remote switch.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Legrand/Double gangs remote switch.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Legrand/Micromodule switch.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Legrand/Micromodule switch.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Legrand/Mobile outlet.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Legrand/Mobile outlet.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Legrand/Remote motion sensor.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Legrand/Remote motion sensor.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Legrand/Remote switch Wake up Sleep.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Legrand/Remote switch Wake up Sleep.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Legrand/Remote switch.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Legrand/Remote switch.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Legrand/Remote toggle switch.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Legrand/Remote toggle switch.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Legrand/Shutter switch with neutral.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Legrand/Shutter switch with neutral.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Legrand/Shutters central remote switch.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Legrand/Shutters central remote switch.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Legrand/Teleruptor.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Legrand/Teleruptor.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Lixee/WS2812_light_controller.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Lixee/WS2812_light_controller.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-historique-mono.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-historique-mono.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-historique-tri.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-historique-tri.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-standard-mono-prod.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-standard-mono-prod.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-standard-mono.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-standard-mono.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-standard-tri-prod.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-standard-tri-prod.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-standard-tri.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Lixee/ZLinky_TIC-standard-tri.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Lixee/ZLinky_TIC.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Lixee/ZLinky_TIC.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Lixee/ZiPulses.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Lixee/ZiPulses.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Lixee/Zigate-Router.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Lixee/Zigate-Router.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Nexturn/VOC_Sensor.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Nexturn/VOC_Sensor.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Nodon/SIN-4-1-20.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Nodon/SIN-4-1-20.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Nodon/SIN-4-FP-21.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Nodon/SIN-4-FP-21.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Nodon/SIN-4-RS-20.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Nodon/SIN-4-RS-20.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Nodon/SIN-4-RS-20_PRO.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Nodon/SIN-4-RS-20_PRO.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/OSRAM/CLA60 TW OSRAM.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/OSRAM/CLA60 TW OSRAM.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/OSRAM/Classic A60 W clear - LIGHTIFY.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/OSRAM/Classic A60 W clear - LIGHTIFY.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/OSRAM/LEDVANCE DIM.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/OSRAM/LEDVANCE DIM.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/OSRAM/LIGHTIFY Indoor Flex RGBW.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/OSRAM/LIGHTIFY Indoor Flex RGBW.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/OSRAM/LIGHTIFY Outdoor Flex RGBW.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/OSRAM/LIGHTIFY Outdoor Flex RGBW.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/OSRAM/Lightify Switch Mini.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/OSRAM/Lightify Switch Mini.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/OSRAM/PAR 16 50 RGBW - LIGHTIFY.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/OSRAM/PAR 16 50 RGBW - LIGHTIFY.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/OSRAM/PAR16 50 TW.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/OSRAM/PAR16 50 TW.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/OSRAM/Plug 01.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/OSRAM/Plug 01.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/OSRAM/Plug Z3.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/OSRAM/Plug Z3.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Orvibo/396483ce8b3f4e0d8e9d79079a35a420.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Orvibo/396483ce8b3f4e0d8e9d79079a35a420.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Orvibo/50938c4c3c0b4049923cd5afbc151bde.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Orvibo/50938c4c3c0b4049923cd5afbc151bde.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Orvibo/82c167c95ed746cdbd21d6817f72c593.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Orvibo/82c167c95ed746cdbd21d6817f72c593.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Orvibo/898ca74409a740b28d5841661e72268d.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Orvibo/898ca74409a740b28d5841661e72268d.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Others/BDP3001.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Others/BDP3001.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Others/Dimmablelight.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Others/Dimmablelight.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Others/EcoDim-Zigbee 3.0.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Others/EcoDim-Zigbee 3.0.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Others/FNB56-ZCW25FB1.6.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Others/FNB56-ZCW25FB1.6.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Others/FNB56-ZCW25FB2.1.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Others/FNB56-ZCW25FB2.1.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Others/FNB56-ZSW01LX2.0.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Others/FNB56-ZSW01LX2.0.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Others/FNB56-ZSW02LX2.0.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Others/FNB56-ZSW02LX2.0.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Others/Lamp_01.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Others/Lamp_01.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Others/NUET56-DL27LX1.1.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Others/NUET56-DL27LX1.1.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Others/VMS_ADUROLIGHT.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Others/VMS_ADUROLIGHT.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Others/ZB-CL01.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Others/ZB-CL01.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Others/ZB-CT01.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Others/ZB-CT01.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Others/ZB-ONOFFPlug-D0005.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Others/ZB-ONOFFPlug-D0005.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Others/ZB-SW02.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Others/ZB-SW02.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Owon/AC201A.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Owon/AC201A.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Owon/AC211.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Owon/AC211.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Owon/AC221.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Owon/AC221.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Owon/CB432.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Owon/CB432.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Owon/DWS312-E.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Owon/DWS312-E.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Owon/KF205.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Owon/KF205.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Owon/PC321.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Owon/PC321.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Owon/PIR323-A.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Owon/PIR323-A.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Owon/PIR323-PTH.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Owon/PIR323-PTH.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Owon/PIR323.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Owon/PIR323.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Owon/PR412.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Owon/PR412.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Owon/THS317-ET.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Owon/THS317-ET.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Owon/WSP402.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Owon/WSP402.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/1744130P7.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/1744130P7.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/440400982841.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/440400982841.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/440400982842.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/440400982842.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/5041131P9.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/5041131P9.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/929002376101.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/929002376101.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/929003052501_01.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/929003052501_01.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/929003052501_02.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/929003052501_02.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/929003053301_01.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/929003053301_01.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/929003053301_02.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/929003053301_02.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/929003054701.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/929003054701.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/LCA001.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/LCA001.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/LCT001.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/LCT001.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/LCT003.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/LCT003.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/LCT007.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/LCT007.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/LCT010.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/LCT010.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/LCT015.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/LCT015.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/LCT024.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/LCT024.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/LLC010.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/LLC010.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/LOM001.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/LOM001.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/LOM008.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/LOM008.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/LST002.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/LST002.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/LTA001.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/LTA001.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/LTC001.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/LTC001.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/LTG002.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/LTG002.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/LTW001.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/LTW001.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/LTW004.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/LTW004.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/LTW010.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/LTW010.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/LTW012.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/LTW012.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/LTW013.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/LTW013.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/LWA001.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/LWA001.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/LWA004.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/LWA004.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/LWA009.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/LWA009.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/LWA018.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/LWA018.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/LWB006.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/LWB006.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/LWB010.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/LWB010.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/LWE004.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/LWE004.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/LWG004.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/LWG004.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/LWO001.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/LWO001.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/ROM001.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/ROM001.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/RWL021.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/RWL021.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/RWL022.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/RWL022.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/SML001.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/SML001.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/SML002.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/SML002.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/SML003.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/SML003.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Philips/SML004.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Philips/SML004.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Profalux/BSO-Profalux.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Profalux/BSO-Profalux.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Profalux/MAI-ZTS.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Profalux/MAI-ZTS.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Profalux/MOT-C1Z06C.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Profalux/MOT-C1Z06C.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Profalux/MOT-C1Z06F.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Profalux/MOT-C1Z06F.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Profalux/Telecommande-Profalux.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Profalux/Telecommande-Profalux.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Profalux/Volet-Profalux.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Profalux/Volet-Profalux.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Profalux/VoletBSO-Profalux.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Profalux/VoletBSO-Profalux.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/README.md` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/README.md`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Robb-Smarrt/ROB_200-004-0.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Robb-Smarrt/ROB_200-004-0.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Robb-Smarrt/ROB_200-017-0.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Robb-Smarrt/ROB_200-017-0.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/SALUS/SPE600.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/SALUS/SPE600.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Samotech/SM309.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Samotech/SM309.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Schneider/1GANGSHUTTER1.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Schneider/1GANGSHUTTER1.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Schneider/CCT592011_AS.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Schneider/CCT592011_AS.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Schneider/EH-ZB-BMS.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Schneider/EH-ZB-BMS.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Schneider/EH-ZB-HACT.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Schneider/EH-ZB-HACT.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Schneider/EH-ZB-LMACT.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Schneider/EH-ZB-LMACT.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Schneider/EH-ZB-RTS.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Schneider/EH-ZB-RTS.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Schneider/EH-ZB-SPD-V2.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Schneider/EH-ZB-SPD-V2.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Schneider/EH-ZB-SPD.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Schneider/EH-ZB-SPD.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Schneider/EH-ZB-VACT.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Schneider/EH-ZB-VACT.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Schneider/NHPBSHUTTER1.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Schneider/NHPBSHUTTER1.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Schneider/PUCKDIMMER1.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Schneider/PUCKDIMMER1.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Schneider/PUCKSHUTTER1.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Schneider/PUCKSHUTTER1.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Schneider/PUCKSWITCH1.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Schneider/PUCKSWITCH1.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Schneider/SOCKETOUTLET1.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Schneider/SOCKETOUTLET1.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Schneider/SOCKETOUTLET2.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Schneider/SOCKETOUTLET2.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Schneider/Wiser2-Thermostat.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Schneider/Wiser2-Thermostat.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Schneider/iTRV.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Schneider/iTRV.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/SmartThings/outletv4.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/SmartThings/outletv4.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Sonoff/01MINIZB.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0012.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8092923280423282%*

 * *Differences: {"'ClusterToBind'": "{insert: [(1, '0019')]}",*

 * * "'ConfigureReporting'": "{'0006': {'Attributes': {'0000': {'TimeOut': '0258'}}}}",*

 * * "'Ep'": "{'01': {'0001': '', '0019': '', delete: ['0003', '1000']}, '02': OrderedDict([('0004', "*

 * *         "''), ('0005', ''), ('0006', ''), ('Type', 'Switch')]), delete: ['f2']}",*

 * * "'ReadAttributes'": "{'0000': {insert: [(1, '0001'), (2, '0002'), (3, '0003')], delete: [3]}, "*

 * *                     "'0001': []}",*

 * * "'_comment'": "'Tuya two gangs Line only'"}*

```diff
@@ -1,48 +1,54 @@
 {
     "ClusterToBind": [
-        "0006"
+        "0006",
+        "0019"
     ],
     "ConfigureReporting": {
         "0006": {
             "Attributes": {
                 "0000": {
                     "Change": "01",
                     "DataType": "10",
                     "MaxInterval": "012C",
                     "MinInterval": "0001",
-                    "TimeOut": "0000"
+                    "TimeOut": "0258"
                 }
             }
         }
     },
     "Ep": {
         "01": {
             "0000": "",
-            "0003": "",
+            "0001": "",
             "0004": "",
             "0005": "",
             "0006": "",
-            "1000": "",
+            "0019": "",
             "Type": "Switch"
         },
-        "f2": {
-            "0021": "",
-            "Type": ""
+        "02": {
+            "0004": "",
+            "0005": "",
+            "0006": "",
+            "Type": "Switch"
         }
     },
     "ReadAttributes": {
         "0000": [
             "0000",
+            "0001",
+            "0002",
+            "0003",
             "0004",
             "0005",
-            "0006",
             "0007"
         ],
+        "0001": [],
         "0006": [
             "0000"
         ]
     },
     "Type": "",
-    "_comment": "Sonoff Basic ZBR3",
+    "_comment": "Tuya two gangs Line only",
     "_version": "1.0"
 }
```

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Sonoff/66666-temphumi.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Sonoff/66666-temphumi.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Sonoff/66666.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Sonoff/66666.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Sonoff/CK-BL702-SWP-01(7020).json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Sonoff/CK-BL702-SWP-01(7020).json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Sonoff/S26R2ZB.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Sonoff/S26R2ZB.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Sonoff/SA-030-1.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Sonoff/SA-030-1.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Sonoff/SNZB-01P.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Sonoff/SNZB-01P.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Sonoff/SNZB-02.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Sonoff/SNZB-02.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Sonoff/SNZB-02D.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Sonoff/SNZB-02D.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Sonoff/SNZB-02P.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Sonoff/SNZB-02P.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Sonoff/SNZB-03P.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Sonoff/SNZB-03P.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Sonoff/SNZB-06P.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Sonoff/SNZB-06P.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Sonoff/TH01.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Sonoff/TH01.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Sonoff/TRVZB.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Sonoff/TRVZB.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Sonoff/ZBMINI-L2.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Sonoff/ZBMINI-L2.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Sonoff/ZBMINIL2.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Sonoff/ZBMINIL2.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Sunricher/HK-SL-DIM-A.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Sunricher/HK-SL-DIM-A.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Sunricher/ZG2858A.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Sunricher/ZG2858A.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Sunricher/ZG9101SAC-HP.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Sunricher/ZG9101SAC-HP.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Sunricher/ZGRC-KEY-013.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Sunricher/ZGRC-KEY-013.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/TDURM0D01/ZBT-Remote-ALL-RGBW.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/TDURM0D01/ZBT-Remote-ALL-RGBW.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/TDURM0D01/tint-ExtendedColor.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/TDURM0D01/tint-ExtendedColor.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/TDURM0D01/tint-Remote-white.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/TDURM0D01/tint-Remote-white.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/TUYATEC/RH3040.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/TUYATEC/RH3040.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/TUYATEC/RH3052.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/TUYATEC/RH3052.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0001.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0001.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0002.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0002.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0002_relay_switch.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0002_relay_switch.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0003.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0003.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0003_relay_switch.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0003_relay_switch.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0004-_TZ3000_excgg5kb.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0004-_TZ3000_excgg5kb.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0004-_TZ3000_u3oupgdy.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0004-_TZ3000_u3oupgdy.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0004-relay_switch.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0004-relay_switch.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0004.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0004.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0011.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0011.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0012.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0013.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9047619047619048%*

 * *Differences: {"'Ep'": "{'03': OrderedDict([('0004', ''), ('0005', ''), ('0006', ''), ('Type', 'Switch')])}",*

 * * "'_comment'": "'Tuya three gangs Line only'"}*

```diff
@@ -27,14 +27,20 @@
             "Type": "Switch"
         },
         "02": {
             "0004": "",
             "0005": "",
             "0006": "",
             "Type": "Switch"
+        },
+        "03": {
+            "0004": "",
+            "0005": "",
+            "0006": "",
+            "Type": "Switch"
         }
     },
     "ReadAttributes": {
         "0000": [
             "0000",
             "0001",
             "0002",
@@ -45,10 +51,10 @@
         ],
         "0001": [],
         "0006": [
             "0000"
         ]
     },
     "Type": "",
-    "_comment": "Tuya two gangs Line only",
+    "_comment": "Tuya three gangs Line only",
     "_version": "1.0"
 }
```

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0013.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-thermostat.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5306712962962963%*

 * *Differences: {"'ClusterToBind'": "['0000', 'ef00']",*

 * * "'ConfigureReporting'": '{replace: OrderedDict()}',*

 * * "'Ep'": "{'01': {'Type': 'Temp/ThermoSetpoint/ThermoOnOff/ThermoMode_2/HeatingStatus', 'ef00': "*

 * *         "'', '000a': '', delete: ['0001', '0006']}, delete: ['02', '03']}",*

 * * "'Param'": "OrderedDict([('ValveDetection', 1), ('SensorMode', 0), ('Calibration', 0)])",*

 * * "'ReadAttributes'": "{'0000': {insert: [(0, '0004'), (5, 'fffe')], delete: [4, 3, 2]}, delete: "*

 * *                     "['0001', '0006']}",*

 * * "'_comment'" […]*

```diff
@@ -1,60 +1,36 @@
 {
     "ClusterToBind": [
-        "0006",
-        "0019"
+        "0000",
+        "ef00"
     ],
-    "ConfigureReporting": {
-        "0006": {
-            "Attributes": {
-                "0000": {
-                    "Change": "01",
-                    "DataType": "10",
-                    "MaxInterval": "012C",
-                    "MinInterval": "0001",
-                    "TimeOut": "0258"
-                }
-            }
-        }
-    },
+    "ConfigureReporting": {},
     "Ep": {
         "01": {
             "0000": "",
-            "0001": "",
             "0004": "",
             "0005": "",
-            "0006": "",
+            "000a": "",
             "0019": "",
-            "Type": "Switch"
-        },
-        "02": {
-            "0004": "",
-            "0005": "",
-            "0006": "",
-            "Type": "Switch"
-        },
-        "03": {
-            "0004": "",
-            "0005": "",
-            "0006": "",
-            "Type": "Switch"
+            "Type": "Temp/ThermoSetpoint/ThermoOnOff/ThermoMode_2/HeatingStatus",
+            "ef00": ""
         }
     },
+    "Param": {
+        "Calibration": 0,
+        "SensorMode": 0,
+        "ValveDetection": 1
+    },
     "ReadAttributes": {
         "0000": [
+            "0004",
             "0000",
             "0001",
-            "0002",
-            "0003",
-            "0004",
             "0005",
-            "0007"
-        ],
-        "0001": [],
-        "0006": [
-            "0000"
+            "0007",
+            "fffe"
         ]
     },
     "Type": "",
-    "_comment": "Tuya three gangs Line only",
-    "_version": "1.0"
+    "_comment": "Tuya TRV: _TZE200_aoclfnxz /TS0601 /Moes /Thermostat BTH-002",
+    "_version": "0.10"
 }
```

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0041.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0041.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0042.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0042.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0043.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0043.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0044.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0044.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0046.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0046.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS004F-_TZ3000_xabckq1v.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS004F-_TZ3000_xabckq1v.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS004F.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS004F.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0112.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0112.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0115.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0115.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS011F-2Gang-switches.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS011F-2Gang-switches.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS011F-2gang-plug.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS011F-2gang-plug.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS011F-_TZ3000_zmy1waw6.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS011F-_TZ3000_zmy1waw6.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS011F-din.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS011F-din.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS011F-multiprise.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS011F-multiprise.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS011F-plug-Elivco.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS011F-plug-Elivco.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS011F-plug.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS011F-plug.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS011F-with_threshold.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS011F-with_threshold.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS011F.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS011F.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0121.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0121.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0201-Temp-Humi-10.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0201-Temp-Humi-10.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0201-Temp-Humi-IH-K009.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0201-Temp-Humi-IH-K009.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0201-_TZ3000_mxzo5rhf.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0201-_TZ3000_mxzo5rhf.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0201-_TZ3000_qaaysllp.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0201-_TZ3000_qaaysllp.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0201.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0201.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0202-WHD02.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0202-WHD02.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0202-_TZ3210_jijr1sss.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0202-_TZ3210_jijr1sss.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0202.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0202.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0207-extender.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0207-extender.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0207-waterleak.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0207-waterleak.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0210.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0210.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0215A-secure-remote.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0215A-secure-remote.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0215A-sos.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0215A-sos.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0219.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0219.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0222.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0222.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0224.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0224.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0225.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0225.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0302.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0302.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0502A.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0502A.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0502B.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0502B.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0503B.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0503B.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0505A-HueSaturation.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0505A-HueSaturation.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0505A.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0505A.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0505B.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0505B.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-2Gangs-dimmer.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-2Gangs-dimmer.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-BLE-YL01.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-BLE-YL01.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-Clamp-Meter.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-Clamp-Meter.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-Energy.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-Energy.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-Human-Presence.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-Human-Presence.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-Irrigation-Valve.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-Irrigation-Valve.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-PC311-Z-TY.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-PC311-Z-TY.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-PC321-Z-TY.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-PC321-Z-TY.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-PJ-1203A.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-PJ-1203A.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-Parkside-Watering-Timer.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-Parkside-Watering-Timer.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-Ronelabs-SEM101.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-Ronelabs-SEM101.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-Ronelabs-SEM301.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-Ronelabs-SEM301.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-SZ-T04.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-SZ-T04.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-Smart-CO.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-Smart-CO.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-Smart-Energy-1P+N.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-Smart-Energy-1P+N.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-SmartAirHouseKeeper.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-SmartAirHouseKeeper.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-Solar-Siren.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-Solar-Siren.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-WZ-M100-C.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-WZ-M100-C.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-XOCA-DAC2161C.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-XOCA-DAC2161C.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-_TZE200_b6wax7g0.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-_TZE200_b6wax7g0.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-_TZE200_dzuqwsyg.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-_TZE200_dzuqwsyg.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-_TZE200_nklqjk62.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-_TZE200_nklqjk62.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-_TZE200_t1blo2bj.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-_TZE200_t1blo2bj.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-curtain.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-curtain.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-dimmer.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-dimmer.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-eTRV1.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-eTRV1.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-eTRV2.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-eTRV2.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-eTRV3.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-eTRV3.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-eTRV5.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-eTRV5.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-eTRV6.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-eTRV6.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-eTRV7.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-eTRV7.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-motion.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-motion.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-photoelectric-smoke.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-photoelectric-smoke.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-radar.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-radar.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-sirene.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-sirene.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-soil-sensor.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-soil-sensor.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-temphumi-2.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-temphumi-2.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-temphumi.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-temphumi.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS0601-temphumix10.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS0601-temphumix10.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS1001.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS1001.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS110E-SMD-02Z.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS110E-SMD-02Z.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS110E-_QS-Zigbee-D02-TRIAC-LN.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS110E-_QS-Zigbee-D02-TRIAC-LN.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS110E-_TZ3210_weaqkhab.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS110E-_TZ3210_weaqkhab.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS110F-2gang-dimmer.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS110F-2gang-dimmer.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS110F-_TYZB01_qezuin6k.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS110F-_TYZB01_qezuin6k.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS110F-_TZ3000_ktuoyvt5.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS110F-_TZ3000_ktuoyvt5.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS110F-dimmer.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS110F-dimmer.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS130F-Blind.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS130F-Blind.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_1dd0d5yi-Blind.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_1dd0d5yi-Blind.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_1dd0d5yi-Vanne.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_1dd0d5yi-Vanne.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_1dd0d5yi.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_1dd0d5yi.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_8kzqqzu4.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_8kzqqzu4.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_dph3rpss.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_dph3rpss.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_femsaaua.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_femsaaua.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_fvhunhxb.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_fvhunhxb.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_zirycpws.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TS130F-_TZ3000_zirycpws.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Tuya/TY0202.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Tuya/TY0202.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Woolley/SA-029-1.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Woolley/SA-029-1.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Woolley/Z111PL0H-1JX.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Woolley/Z111PL0H-1JX.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Ynoa/ZBT-CCTLight-A0001.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Ynoa/ZBT-CCTLight-A0001.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Ynoa/ZBT-CCTLight-GU100001.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Ynoa/ZBT-CCTLight-GU100001.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Ysrai/ZB-CL01.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Ysrai/ZB-CL01.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Ysrai/ZB-CT01.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Ysrai/ZB-CT01.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Ysrai/ZB-DL01.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Ysrai/ZB-DL01.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Ysrai/ZB-SW02.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Ysrai/ZB-SW02.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Zehnder/TAFFETAS2 D1.00P1.01Z1.00.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Zehnder/TAFFETAS2 D1.00P1.01Z1.00.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/Zemismart/LXN56-DC27LX1.1.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/Zemismart/LXN56-DC27LX1.1.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/eWeLink/SA-003-Zigbee.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/eWeLink/SA-003-Zigbee.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/eWeLink/SA-030-1.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/eWeLink/SA-030-1.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/eWeLink/SWITCH-ZR02.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/eWeLink/SWITCH-ZR02.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/Certified/eWeLink/SWITCH-ZR03-1.json` & `z4d_certified_devices-5.260/z4d_certified_devices/Certified/eWeLink/SWITCH-ZR03-1.json`

 * *Files identical despite different names*

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices/__init__.py` & `z4d_certified_devices-5.260/z4d_certified_devices/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,81 +9,81 @@
 # Initial authors: zaraki673 & pipiche38
 #
 # SPDX-License-Identifier:    GPL-3.0 license
 
 import json
 import os.path
 from pathlib import Path
+import os
 
 from .version import __version__
 
 
 def z4d_import_device_configuration(self, path_name):
 
     model_certified = Path(path_name) / "Certified"
     plugin_version = self.pluginParameters.get("PluginVersion")
 
     if not os.path.isdir(model_certified):
-        self.log.logging("z4dCertifiedDevices", "Status", f"none existing Z4D Certified Db at {model_certified} !!!")
+        self.log.logging("z4dCertifiedDevices", "Status", f"Z4D found an empty Certified Db {model_certified}")
         return
     
     for device_brand in os.listdir(model_certified):
         if device_brand in ("README.md", ".PRECIOUS"):
             continue
-
-        model_directory = model_certified / device_brand
-
+    
+        model_directory = Path(model_certified) / device_brand
+    
         for model_device_file in os.listdir(model_directory):
             if model_device_file in ("README.md", ".PRECIOUS"):
                 continue
-
+    
             filename = model_directory / model_device_file
+    
             try:
                 with open(filename, "rt", encoding='utf-8') as file_handle:
                     model_definition = json.load(file_handle)
-
-            except ValueError as error:
-                self.log.logging("z4dCertifiedDevices", "Error", f"JSON ConfFile: {filename} load failed with error: {error}, skiping this config file.")
-                continue
-
-            except Exception as error:
-                self.log.logging("z4dCertifiedDevices", "Error", f"JSON ConfFile: {filename} load general error: {error}, skiping this config file.")
+    
+            except (ValueError, Exception) as error:
+                error_type = type(error).__name__
+                error_msg = f"JSON ConfFile: {filename} load failed with error: {error_type}, skipping this config file."
+                self.log.logging("z4dCertifiedDevices", "Error", error_msg)
                 continue
-
-            device_model_name = _get_model_name(model_device_file )
+    
+            device_model_name = _get_model_name(model_device_file)
+    
             if device_model_name in self.DeviceConf:
                 self.log.logging("z4dCertifiedDevices", "Debug", f"Config for {device_brand}/{device_model_name} not loaded as already defined")
                 continue
-
+    
             self.log.logging("z4dCertifiedDevices", "Debug", f"processing certified {device_brand}/{device_model_name}")
-
+    
             if not _is_model_requirement_match_plugin_version(self, model_definition, plugin_version):
-                self.log.logging( "z4dCertifiedDevices", "Error", f"Certified Devices load skip this Certified device %{device_brand}-{device_model_name} requires Plugin version {model_definition['MinPluginVersion']}")
+                min_plugin_version = model_definition.get("MinPluginVersion", "N/A")
+                error_msg = f"Certified Devices load skip this Certified device {device_brand}-{device_model_name} requires Plugin version {min_plugin_version}"
+                self.log.logging("z4dCertifiedDevices", "Error", error_msg)
                 continue
 
             _process_device_config_file(self, device_model_name, model_definition)
 
     self.log.logging("z4dCertifiedDevices", "Debug", f"Config loaded: {self.DeviceConf.keys()}")
     self.log.logging("z4dCertifiedDevices", "Debug", f"Certified Devices ModelManufMapping loaded - {self.ModelManufMapping.keys()}")
     
-    self.log.logging("z4dCertifiedDevices", "Status", f"{len(self.DeviceConf)} Certified devices loaded from z4d repository.")
+    self.log.logging("z4dCertifiedDevices", "Status", f"Z4D loads {len(self.DeviceConf)} Certified devices from repository.")
+
 
-def _get_model_name(model_device_file ):
-    """ Purpose is to remove .json from filename to get the Device Model"""
-    basename = os.path.basename(model_device_file)
-    device_model_name = os.path.splitext(basename)[0]
-    return device_model_name
+def _get_model_name(model_device_file):
+    """Remove .json from filename to get the Device Model."""
+    return os.path.splitext(os.path.basename(model_device_file))[0]
 
 
 def _is_model_requirement_match_plugin_version(self, model_definition, plugin_version):
     """ is the config file working with this version of the plugin """
     return not ("MinPluginVersion" in model_definition and plugin_version < model_definition["MinPluginVersion"])
 
     
 def _process_device_config_file(self, device_model_name, model_definition):
-    """ let's load the config into DeviceConf , and if needed (Tuya) lets also load into the model name mapping"""
-    self.DeviceConf[device_model_name] = dict(model_definition)
-    if "Identifier" not in model_definition:
-        return
-    for identifier_tuple in model_definition["Identifier"]:
-        self.ModelManufMapping[ tuple(identifier_tuple) ] = device_model_name
-
+    """Load the config into DeviceConf and, if needed (Tuya), load into the model name mapping."""
+    self.DeviceConf[device_model_name] = model_definition
+    identifier_list = model_definition.get("Identifier", [])
+    for identifier_tuple in identifier_list:
+        self.ModelManufMapping[tuple(identifier_tuple)] = device_model_name
```

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices.egg-info/PKG-INFO` & `z4d_certified_devices-5.260/z4d_certified_devices.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: z4d-certified-devices
-Version: 4.259
+Version: 5.260
 Summary: "Certified devices for Zigbee for Domoticz plugin"
 Home-page: https://github.com/zigbeefordomoticz/z4d-certified-devices
 Author: "Patrick Pichon"
 Author-email: "patrick@pichon.me"
 License: "GPL-3.0"
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: z4d-certified-devices Version: 4.259 Summary:
+Metadata-Version: 2.1 Name: z4d-certified-devices Version: 5.260 Summary:
 "Certified devices for Zigbee for Domoticz plugin" Home-page: https://
 github.com/zigbeefordomoticz/z4d-certified-devices Author: "Patrick Pichon"
 Author-email: "patrick@pichon.me" License: "GPL-3.0" Classifier: Programming
 Language :: Python :: 3 Description-Content-Type: text/markdown License-File:
 LICENSE.txt # z4d-certified-devices ## Overview This package is required for
 the [Zigbee for Domoticz](https://github.com/zigbeefordomoticz/Domoticz-Zigbee)
 plugin. It provides configuration files to optimized the pairing and behaviour
```

### Comparing `z4d_certified_devices-4.259/z4d_certified_devices.egg-info/SOURCES.txt` & `z4d_certified_devices-5.260/z4d_certified_devices.egg-info/SOURCES.txt`

 * *Files identical despite different names*

