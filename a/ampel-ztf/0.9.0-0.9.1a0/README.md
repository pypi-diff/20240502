# Comparing `tmp/ampel_ztf-0.9.0.tar.gz` & `tmp/ampel_ztf-0.9.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ampel_ztf-0.9.0.tar", max compression
+gzip compressed data, was "ampel_ztf-0.9.1a0.tar", max compression
```

## Comparing `ampel_ztf-0.9.0.tar` & `ampel_ztf-0.9.1a0.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0     1512 2023-04-07 13:56:59.167697 ampel_ztf-0.9.0/LICENSE
--rw-r--r--   0        0        0      391 2023-04-07 13:56:59.167697 ampel_ztf-0.9.0/README.md
--rw-r--r--   0        0        0        0 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/py.typed
--rwxr-xr-x   0        0        0     3644 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/template/ZTFLegacyChannelTemplate.py
--rwxr-xr-x   0        0        0      739 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/template/ZTFPeriodicSummaryT3.py
--rwxr-xr-x   0        0        0     2819 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/template/ZTFProcessLocalAlerts.py
--rwxr-xr-x   0        0        0    11970 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/util/Observatory.py
--rw-r--r--   0        0        0     3810 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/alert/HealpixPathSupplier.py
--rwxr-xr-x   0        0        0     9168 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/alert/PhotoAlertPlotter.py
--rw-r--r--   0        0        0    24540 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/alert/ZTFFPbotForcedPhotometryAlertSupplier.py
--rwxr-xr-x   0        0        0     3649 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/alert/ZTFForcedPhotometryAlertSupplier.py
--rwxr-xr-x   0        0        0     3582 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/alert/ZTFGeneralActiveAlertRegister.py
--rwxr-xr-x   0        0        0     2132 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/alert/ZTFGeneralAlertRegister.py
--rw-r--r--   0        0        0     5534 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/alert/ZTFIPACForcedPhotometryAlertSupplier.py
--rwxr-xr-x   0        0        0     2375 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/alert/ZiAlertSupplier.py
--rw-r--r--   0        0        0     2007 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/alert/ZiHealpixAlertSupplier.py
--rwxr-xr-x   0        0        0     2119 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/alert/ZiTaggedAlertSupplier.py
--rw-r--r--   0        0        0     5405 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/alert/load/ZTFHealpixAlertLoader.py
--rw-r--r--   0        0        0     1286 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/base/ArchiveUnit.py
--rwxr-xr-x   0        0        0     3612 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/base/CatalogMatchFilter.py
--rwxr-xr-x   0        0        0     5609 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/base/CatalogMatchUnit.py
--rwxr-xr-x   0        0        0     4803 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/dev/DevAlertConsumer.py
--rwxr-xr-x   0        0        0     6975 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/dev/DevSkyPortalClient.py
--rwxr-xr-x   0        0        0     3550 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/dev/ZTFAlert.py
--rw-r--r--   0        0        0     6187 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/ingest/ZiArchiveMuxer.py
--rw-r--r--   0        0        0      760 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/ingest/ZiCompilerOptions.py
--rwxr-xr-x   0        0        0     3580 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/ingest/ZiDataPointShaper.py
--rwxr-xr-x   0        0        0    10260 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/ingest/ZiMongoMuxer.py
--rwxr-xr-x   0        0        0     1062 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/ingest/tags.py
--rwxr-xr-x   0        0        0     2298 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/legacy_utils.py
--rwxr-xr-x   0        0        0    14327 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/t0/DecentFilter.py
--rw-r--r--   0        0        0    17003 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/t0/T0HealpixPathProcessor.py
--rw-r--r--   0        0        0    13501 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/t0/T0HealpixProcessor.py
--rwxr-xr-x   0        0        0     7702 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/t0/ZTFAlertStreamController.py
--rwxr-xr-x   0        0        0     7598 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/t0/load/AllConsumingConsumer.py
--rwxr-xr-x   0        0        0     2947 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/t0/load/UWAlertLoader.py
--rw-r--r--   0        0        0     2369 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/t0/load/ZTFAlertArchiver.py
--rw-r--r--   0        0        0     3265 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/t0/load/ZTFAlertArchiverV3.py
--rw-r--r--   0        0        0     3994 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/t0/load/ZTFArchiveAlertLoader.py
--rw-r--r--   0        0        0     1346 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/t0/load/avroutils.py
--rwxr-xr-x   0        0        0     2976 2023-04-07 13:56:59.191697 ampel_ztf-0.9.0/ampel/ztf/t0/load/fetcherutils.py
--rwxr-xr-x   0        0        0     1198 2023-04-07 13:56:59.195698 ampel_ztf-0.9.0/ampel/ztf/t1/ZiT1Combiner.py
--rwxr-xr-x   0        0        0     1048 2023-04-07 13:56:59.195698 ampel_ztf-0.9.0/ampel/ztf/t1/ZiT1RetroCombiner.py
--rwxr-xr-x   0        0        0     5674 2023-04-07 13:56:59.195698 ampel_ztf-0.9.0/ampel/ztf/t2/T2CatalogMatch.py
--rw-r--r--   0        0        0     2240 2023-04-07 13:56:59.195698 ampel_ztf-0.9.0/ampel/ztf/t2/T2LightCurveFeatures.py
--rwxr-xr-x   0        0        0     2757 2023-04-07 13:56:59.195698 ampel_ztf-0.9.0/ampel/ztf/t2/T2LightCurveSummary.py
--rwxr-xr-x   0        0        0     1339 2023-04-07 13:56:59.195698 ampel_ztf-0.9.0/ampel/ztf/t3/T3LegacyExtJournalAppender.py
--rwxr-xr-x   0        0        0     2891 2023-04-07 13:56:59.195698 ampel_ztf-0.9.0/ampel/ztf/t3/complement/FritzReport.py
--rwxr-xr-x   0        0        0     2481 2023-04-07 13:56:59.195698 ampel_ztf-0.9.0/ampel/ztf/t3/complement/GROWTHMarshalReport.py
--rwxr-xr-x   0        0        0     3890 2023-04-07 13:56:59.195698 ampel_ztf-0.9.0/ampel/ztf/t3/complement/TNSNames.py
--rwxr-xr-x   0        0        0      517 2023-04-07 13:56:59.195698 ampel_ztf-0.9.0/ampel/ztf/t3/complement/TNSReports.py
--rwxr-xr-x   0        0        0     3031 2023-04-07 13:56:59.195698 ampel_ztf-0.9.0/ampel/ztf/t3/complement/ZTFCutoutImages.py
--rwxr-xr-x   0        0        0     1248 2023-04-07 13:56:59.195698 ampel_ztf-0.9.0/ampel/ztf/t3/select/T3AdHocStockSelector.py
--rwxr-xr-x   0        0        0    30107 2023-04-07 13:56:59.195698 ampel_ztf-0.9.0/ampel/ztf/t3/skyportal/SkyPortalClient.py
--rwxr-xr-x   0        0        0     3876 2023-04-07 13:56:59.195698 ampel_ztf-0.9.0/ampel/ztf/t3/skyportal/SkyPortalPublisher.py
--rw-r--r--   0        0        0     2986 2023-04-07 13:56:59.195698 ampel_ztf-0.9.0/ampel/ztf/t4/T4ZTFArchiveTokenGenerator.py
--rwxr-xr-x   0        0        0     4337 2023-04-07 13:56:59.195698 ampel_ztf-0.9.0/ampel/ztf/util/ZTFIdMapper.py
--rw-r--r--   0        0        0     2781 2023-04-07 13:56:59.195698 ampel_ztf-0.9.0/ampel/ztf/util/ZTFNoisifiedIdMapper.py
--rw-r--r--   0        0        0     3832 2023-04-07 13:56:59.195698 ampel_ztf-0.9.0/ampel/ztf/view/ZTFT2Tabulator.py
--rw-r--r--   0        0        0     2293 2023-04-07 13:56:59.195698 ampel_ztf-0.9.0/conf/ampel-ztf/ampel.yml
--rw-r--r--   0        0        0     2689 2023-04-07 13:56:59.195698 ampel_ztf-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     2481 1970-01-01 00:00:00.000000 ampel_ztf-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1512 2023-12-20 10:21:24.488069 ampel_ztf-0.9.1a0/LICENSE
+-rw-r--r--   0        0        0      391 2023-12-20 10:21:24.488069 ampel_ztf-0.9.1a0/README.md
+-rw-r--r--   0        0        0        0 2023-12-20 10:21:24.508069 ampel_ztf-0.9.1a0/ampel/py.typed
+-rwxr-xr-x   0        0        0     3644 2023-12-20 10:21:24.508069 ampel_ztf-0.9.1a0/ampel/template/ZTFLegacyChannelTemplate.py
+-rwxr-xr-x   0        0        0      739 2023-12-20 10:21:24.508069 ampel_ztf-0.9.1a0/ampel/template/ZTFPeriodicSummaryT3.py
+-rwxr-xr-x   0        0        0     2819 2023-12-20 10:21:24.508069 ampel_ztf-0.9.1a0/ampel/template/ZTFProcessLocalAlerts.py
+-rwxr-xr-x   0        0        0    11970 2023-12-20 10:21:24.508069 ampel_ztf-0.9.1a0/ampel/util/Observatory.py
+-rw-r--r--   0        0        0     3810 2023-12-20 10:21:24.508069 ampel_ztf-0.9.1a0/ampel/ztf/alert/HealpixPathSupplier.py
+-rwxr-xr-x   0        0        0     9173 2023-12-20 10:21:24.508069 ampel_ztf-0.9.1a0/ampel/ztf/alert/PhotoAlertPlotter.py
+-rw-r--r--   0        0        0    24540 2023-12-20 10:21:24.508069 ampel_ztf-0.9.1a0/ampel/ztf/alert/ZTFFPbotForcedPhotometryAlertSupplier.py
+-rwxr-xr-x   0        0        0     3649 2023-12-20 10:21:24.508069 ampel_ztf-0.9.1a0/ampel/ztf/alert/ZTFForcedPhotometryAlertSupplier.py
+-rwxr-xr-x   0        0        0     3582 2023-12-20 10:21:24.508069 ampel_ztf-0.9.1a0/ampel/ztf/alert/ZTFGeneralActiveAlertRegister.py
+-rwxr-xr-x   0        0        0     2132 2023-12-20 10:21:24.508069 ampel_ztf-0.9.1a0/ampel/ztf/alert/ZTFGeneralAlertRegister.py
+-rw-r--r--   0        0        0     5534 2023-12-20 10:21:24.508069 ampel_ztf-0.9.1a0/ampel/ztf/alert/ZTFIPACForcedPhotometryAlertSupplier.py
+-rwxr-xr-x   0        0        0     2375 2023-12-20 10:21:24.508069 ampel_ztf-0.9.1a0/ampel/ztf/alert/ZiAlertSupplier.py
+-rw-r--r--   0        0        0     2007 2023-12-20 10:21:24.508069 ampel_ztf-0.9.1a0/ampel/ztf/alert/ZiHealpixAlertSupplier.py
+-rwxr-xr-x   0        0        0     2119 2023-12-20 10:21:24.508069 ampel_ztf-0.9.1a0/ampel/ztf/alert/ZiTaggedAlertSupplier.py
+-rw-r--r--   0        0        0     5443 2023-12-20 10:21:24.508069 ampel_ztf-0.9.1a0/ampel/ztf/alert/load/ZTFHealpixAlertLoader.py
+-rw-r--r--   0        0        0     1286 2023-12-20 10:21:24.508069 ampel_ztf-0.9.1a0/ampel/ztf/base/ArchiveUnit.py
+-rwxr-xr-x   0        0        0     3612 2023-12-20 10:21:24.508069 ampel_ztf-0.9.1a0/ampel/ztf/base/CatalogMatchFilter.py
+-rwxr-xr-x   0        0        0     5639 2023-12-20 10:21:24.508069 ampel_ztf-0.9.1a0/ampel/ztf/base/CatalogMatchUnit.py
+-rwxr-xr-x   0        0        0     4803 2023-12-20 10:21:24.508069 ampel_ztf-0.9.1a0/ampel/ztf/dev/DevAlertConsumer.py
+-rwxr-xr-x   0        0        0     6975 2023-12-20 10:21:24.508069 ampel_ztf-0.9.1a0/ampel/ztf/dev/DevSkyPortalClient.py
+-rwxr-xr-x   0        0        0     3648 2023-12-20 10:21:24.508069 ampel_ztf-0.9.1a0/ampel/ztf/dev/ZTFAlert.py
+-rw-r--r--   0        0        0     6225 2023-12-20 10:21:24.508069 ampel_ztf-0.9.1a0/ampel/ztf/ingest/ZiArchiveMuxer.py
+-rw-r--r--   0        0        0      760 2023-12-20 10:21:24.508069 ampel_ztf-0.9.1a0/ampel/ztf/ingest/ZiCompilerOptions.py
+-rwxr-xr-x   0        0        0     3580 2023-12-20 10:21:24.508069 ampel_ztf-0.9.1a0/ampel/ztf/ingest/ZiDataPointShaper.py
+-rwxr-xr-x   0        0        0    10260 2023-12-20 10:21:24.508069 ampel_ztf-0.9.1a0/ampel/ztf/ingest/ZiMongoMuxer.py
+-rwxr-xr-x   0        0        0     1062 2023-12-20 10:21:24.508069 ampel_ztf-0.9.1a0/ampel/ztf/ingest/tags.py
+-rwxr-xr-x   0        0        0     2298 2023-12-20 10:21:24.508069 ampel_ztf-0.9.1a0/ampel/ztf/legacy_utils.py
+-rwxr-xr-x   0        0        0    14357 2023-12-20 10:21:24.508069 ampel_ztf-0.9.1a0/ampel/ztf/t0/DecentFilter.py
+-rw-r--r--   0        0        0    17003 2023-12-20 10:21:24.508069 ampel_ztf-0.9.1a0/ampel/ztf/t0/T0HealpixPathProcessor.py
+-rw-r--r--   0        0        0    13501 2023-12-20 10:21:24.508069 ampel_ztf-0.9.1a0/ampel/ztf/t0/T0HealpixProcessor.py
+-rwxr-xr-x   0        0        0     7718 2023-12-20 10:21:24.508069 ampel_ztf-0.9.1a0/ampel/ztf/t0/ZTFAlertStreamController.py
+-rwxr-xr-x   0        0        0     8810 2023-12-20 10:21:24.508069 ampel_ztf-0.9.1a0/ampel/ztf/t0/load/AllConsumingConsumer.py
+-rwxr-xr-x   0        0        0     2990 2023-12-20 10:21:24.508069 ampel_ztf-0.9.1a0/ampel/ztf/t0/load/UWAlertLoader.py
+-rw-r--r--   0        0        0     2369 2023-12-20 10:21:24.508069 ampel_ztf-0.9.1a0/ampel/ztf/t0/load/ZTFAlertArchiver.py
+-rw-r--r--   0        0        0     3303 2023-12-20 10:21:24.508069 ampel_ztf-0.9.1a0/ampel/ztf/t0/load/ZTFAlertArchiverV3.py
+-rw-r--r--   0        0        0     4475 2023-12-20 10:21:24.508069 ampel_ztf-0.9.1a0/ampel/ztf/t0/load/ZTFArchiveAlertLoader.py
+-rw-r--r--   0        0        0     1346 2023-12-20 10:21:24.508069 ampel_ztf-0.9.1a0/ampel/ztf/t0/load/avroutils.py
+-rwxr-xr-x   0        0        0     2976 2023-12-20 10:21:24.508069 ampel_ztf-0.9.1a0/ampel/ztf/t0/load/fetcherutils.py
+-rwxr-xr-x   0        0        0     1198 2023-12-20 10:21:24.508069 ampel_ztf-0.9.1a0/ampel/ztf/t1/ZiT1Combiner.py
+-rwxr-xr-x   0        0        0     1048 2023-12-20 10:21:24.508069 ampel_ztf-0.9.1a0/ampel/ztf/t1/ZiT1RetroCombiner.py
+-rwxr-xr-x   0        0        0     5674 2023-12-20 10:21:24.508069 ampel_ztf-0.9.1a0/ampel/ztf/t2/T2CatalogMatch.py
+-rw-r--r--   0        0        0     2240 2023-12-20 10:21:24.508069 ampel_ztf-0.9.1a0/ampel/ztf/t2/T2LightCurveFeatures.py
+-rwxr-xr-x   0        0        0     2757 2023-12-20 10:21:24.512069 ampel_ztf-0.9.1a0/ampel/ztf/t2/T2LightCurveSummary.py
+-rwxr-xr-x   0        0        0     1339 2023-12-20 10:21:24.512069 ampel_ztf-0.9.1a0/ampel/ztf/t3/T3LegacyExtJournalAppender.py
+-rwxr-xr-x   0        0        0     2891 2023-12-20 10:21:24.512069 ampel_ztf-0.9.1a0/ampel/ztf/t3/complement/FritzReport.py
+-rwxr-xr-x   0        0        0     2511 2023-12-20 10:21:24.512069 ampel_ztf-0.9.1a0/ampel/ztf/t3/complement/GROWTHMarshalReport.py
+-rwxr-xr-x   0        0        0     3890 2023-12-20 10:21:24.512069 ampel_ztf-0.9.1a0/ampel/ztf/t3/complement/TNSNames.py
+-rwxr-xr-x   0        0        0      517 2023-12-20 10:21:24.512069 ampel_ztf-0.9.1a0/ampel/ztf/t3/complement/TNSReports.py
+-rwxr-xr-x   0        0        0     3061 2023-12-20 10:21:24.512069 ampel_ztf-0.9.1a0/ampel/ztf/t3/complement/ZTFCutoutImages.py
+-rwxr-xr-x   0        0        0     1248 2023-12-20 10:21:24.512069 ampel_ztf-0.9.1a0/ampel/ztf/t3/select/T3AdHocStockSelector.py
+-rwxr-xr-x   0        0        0    30107 2023-12-20 10:21:24.512069 ampel_ztf-0.9.1a0/ampel/ztf/t3/skyportal/SkyPortalClient.py
+-rwxr-xr-x   0        0        0     3876 2023-12-20 10:21:24.512069 ampel_ztf-0.9.1a0/ampel/ztf/t3/skyportal/SkyPortalPublisher.py
+-rw-r--r--   0        0        0     2986 2023-12-20 10:21:24.512069 ampel_ztf-0.9.1a0/ampel/ztf/t4/T4ZTFArchiveTokenGenerator.py
+-rwxr-xr-x   0        0        0     4337 2023-12-20 10:21:24.512069 ampel_ztf-0.9.1a0/ampel/ztf/util/ZTFIdMapper.py
+-rw-r--r--   0        0        0     2781 2023-12-20 10:21:24.512069 ampel_ztf-0.9.1a0/ampel/ztf/util/ZTFNoisifiedIdMapper.py
+-rw-r--r--   0        0        0     3832 2023-12-20 10:21:24.512069 ampel_ztf-0.9.1a0/ampel/ztf/view/ZTFT2Tabulator.py
+-rw-r--r--   0        0        0     2293 2023-12-20 10:21:24.512069 ampel_ztf-0.9.1a0/conf/ampel-ztf/ampel.yml
+-rw-r--r--   0        0        0     2680 2023-12-20 10:21:24.512069 ampel_ztf-0.9.1a0/pyproject.toml
+-rw-r--r--   0        0        0     2520 1970-01-01 00:00:00.000000 ampel_ztf-0.9.1a0/PKG-INFO
```

### Comparing `ampel_ztf-0.9.0/LICENSE` & `ampel_ztf-0.9.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.9.0/ampel/template/ZTFLegacyChannelTemplate.py` & `ampel_ztf-0.9.1a0/ampel/template/ZTFLegacyChannelTemplate.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.9.0/ampel/template/ZTFPeriodicSummaryT3.py` & `ampel_ztf-0.9.1a0/ampel/template/ZTFPeriodicSummaryT3.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.9.0/ampel/template/ZTFProcessLocalAlerts.py` & `ampel_ztf-0.9.1a0/ampel/template/ZTFProcessLocalAlerts.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.9.0/ampel/util/Observatory.py` & `ampel_ztf-0.9.1a0/ampel/util/Observatory.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.9.0/ampel/ztf/alert/HealpixPathSupplier.py` & `ampel_ztf-0.9.1a0/ampel/ztf/alert/HealpixPathSupplier.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.9.0/ampel/ztf/alert/PhotoAlertPlotter.py` & `ampel_ztf-0.9.1a0/ampel/ztf/alert/PhotoAlertPlotter.py`

 * *Files 2% similar despite different names*

```diff
@@ -270,26 +270,26 @@
 		create a summary plot for the given alert. This includes
 		the three cutouts (ref, sci, diff), the light curve, and
 		some printouts of several alert parameters.
 		"""
 
 		# set figure and axis
 		plt.close('all')
-		fig = plt.figure(figsize=[9, 5])
+		fig = plt.figure(figsize=(9, 5))
 		ref, width, heigh = 0.1, 0.15, 0.25
 		span = 0.05
 		ypos = 0.65
 		cutout_axes = {
-			'cutoutScience': fig.add_axes([ref, ypos, width, heigh]),
-			'cutoutTemplate': fig.add_axes([ref + (width + span), ypos, width, heigh]),
-			'cutoutDifference': fig.add_axes([ref + (width + span) * 2, ypos, width, heigh])
+			'cutoutScience': fig.add_axes((ref, ypos, width, heigh)),
+			'cutoutTemplate': fig.add_axes((ref + (width + span), ypos, width, heigh)),
+			'cutoutDifference': fig.add_axes((ref + (width + span) * 2, ypos, width, heigh))
 		}
-		axlc = fig.add_axes([ref, 0.1, (width + span) * 2 + width, 0.5])
+		axlc = fig.add_axes((ref, 0.1, (width + span) * 2 + width, 0.5))
 		if ps1_cutout:
-			fig.add_axes([ref + (width + span * 1.5) * 3, ypos, width, heigh])
+			fig.add_axes((ref + (width + span * 1.5) * 3, ypos, width, heigh))
 
 		# plot the cutouts
 		for which in ('cutoutScience', 'cutoutTemplate', 'cutoutDifference'):
 			self.plot_cutout(alert, which, ax=cutout_axes[which])
 
 		# plot the lightcurve
 		self.plot_lc(alert, ax=axlc)
@@ -302,14 +302,14 @@
 				info.append("%s : %.3f" % (k, candidate.get(k, np.nan)))
 			except Exception:
 				info.append("%s : %s" % (k, candidate.get(k)))
 		for kk in ["objectidps", "sgscore", "distpsnr", "srmag"]:
 			for k in [k for k in candidate.keys() if kk in k]:
 				info.append("%s : %.2f" % (k, float(candidate.get(k, np.nan))))
 		fig.text(0.68, 0.6, " \n".join(info), va="top", fontsize="medium", color="0.3")
-		fig.text(0.01, 0.99, alert.stock, fontsize="x-large", color="k", va="top", ha="left")
+		fig.text(0.01, 0.99, str(alert.stock), fontsize="x-large", color="k", va="top", ha="left")
 
 		# now go back to previous state
 		if self.interactive:
 			plt.show(fig)
 		else:
 			self.save_current_plot(alert, "summary_" + self.base_plot_name_tmpl, **kwargs)
```

### Comparing `ampel_ztf-0.9.0/ampel/ztf/alert/ZTFFPbotForcedPhotometryAlertSupplier.py` & `ampel_ztf-0.9.1a0/ampel/ztf/alert/ZTFFPbotForcedPhotometryAlertSupplier.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.9.0/ampel/ztf/alert/ZTFForcedPhotometryAlertSupplier.py` & `ampel_ztf-0.9.1a0/ampel/ztf/alert/ZTFForcedPhotometryAlertSupplier.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.9.0/ampel/ztf/alert/ZTFGeneralActiveAlertRegister.py` & `ampel_ztf-0.9.1a0/ampel/ztf/alert/ZTFGeneralActiveAlertRegister.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.9.0/ampel/ztf/alert/ZTFGeneralAlertRegister.py` & `ampel_ztf-0.9.1a0/ampel/ztf/alert/ZTFGeneralAlertRegister.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.9.0/ampel/ztf/alert/ZTFIPACForcedPhotometryAlertSupplier.py` & `ampel_ztf-0.9.1a0/ampel/ztf/alert/ZTFIPACForcedPhotometryAlertSupplier.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.9.0/ampel/ztf/alert/ZiAlertSupplier.py` & `ampel_ztf-0.9.1a0/ampel/ztf/alert/ZiAlertSupplier.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.9.0/ampel/ztf/alert/ZiHealpixAlertSupplier.py` & `ampel_ztf-0.9.1a0/ampel/ztf/alert/ZiHealpixAlertSupplier.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.9.0/ampel/ztf/alert/ZiTaggedAlertSupplier.py` & `ampel_ztf-0.9.1a0/ampel/ztf/alert/ZiTaggedAlertSupplier.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.9.0/ampel/ztf/alert/load/ZTFHealpixAlertLoader.py` & `ampel_ztf-0.9.1a0/ampel/ztf/alert/load/ZTFHealpixAlertLoader.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,15 +128,17 @@
             if chunk["remaining"]["chunks"] == 0:
                 self.query_start += self.query_size
                 self.stream = None
 
     @backoff.on_exception(
         backoff.expo,
         requests.exceptions.HTTPError,
-        giveup=lambda e: not isinstance(e, requests.HTTPError) or e.response.status_code not in {500, 502, 503, 504, 429, 408},
+        giveup=lambda e: not isinstance(e, requests.HTTPError)
+        or e.response is None
+        or e.response.status_code not in {500, 502, 503, 504, 429, 408},
         max_time=600,
     )
     def _get_chunk(self) -> dict[str, Any]:
         if self.stream is None:
             jd = Time(self.source.time, scale="utc").jd  # type: ignore[union-attr]
             response = self.session.post(
                 "alerts/healpix/skymap",
```

### Comparing `ampel_ztf-0.9.0/ampel/ztf/base/ArchiveUnit.py` & `ampel_ztf-0.9.1a0/ampel/ztf/base/ArchiveUnit.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.9.0/ampel/ztf/base/CatalogMatchFilter.py` & `ampel_ztf-0.9.1a0/ampel/ztf/base/CatalogMatchFilter.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.9.0/ampel/ztf/base/CatalogMatchUnit.py` & `ampel_ztf-0.9.1a0/ampel/ztf/base/CatalogMatchUnit.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,14 +127,15 @@
         max_tries=5,
         factor=10,
     )
     @backoff.on_exception(
         backoff.expo,
         requests.HTTPError,
         giveup=lambda e: not isinstance(e, requests.HTTPError)
+        or e.response is None
         or e.response.status_code not in {502, 503, 504, 429, 408},
         max_time=60,
     )
     def _cone_search(
         self,
         method: Literal["any", "nearest", "all"],
         ra: float,
```

### Comparing `ampel_ztf-0.9.0/ampel/ztf/dev/DevAlertConsumer.py` & `ampel_ztf-0.9.1a0/ampel/ztf/dev/DevAlertConsumer.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.9.0/ampel/ztf/dev/DevSkyPortalClient.py` & `ampel_ztf-0.9.1a0/ampel/ztf/dev/DevSkyPortalClient.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     with gzip.open(io.BytesIO(cutout_data), "rb") as f:
         with fits.open(f) as hdu:
             header = hdu[0].header
             img = np.flipud(hdu[0].data)
     mask = np.isfinite(img)
 
     fig = Figure(figsize=(1, 1))
-    ax = fig.add_axes([0.0, 0.0, 1.0, 1.0])
+    ax = fig.add_axes((0.0, 0.0, 1.0, 1.0))
     ax.set_axis_off()
     ax.imshow(
         img,
         # clip pixel values below the median
         norm=Normalize(*np.percentile(img[mask], [0.5, 99.5])),
         aspect="auto",
         origin="lower",
```

### Comparing `ampel_ztf-0.9.0/ampel/ztf/dev/ZTFAlert.py` & `ampel_ztf-0.9.1a0/ampel/ztf/dev/ZTFAlert.py`

 * *Files 7% similar despite different names*

```diff
@@ -119,8 +119,14 @@
 		return content
 
 
 	@staticmethod
 	def _deserialize(f) -> None | dict:
 		""" """
 		reader = fastavro.reader(f)
-		return next(reader, None)
+		alert = next(reader, None)
+		if alert is None:
+			return alert
+		else:
+			assert isinstance(alert, dict)
+			return alert
+
```

### Comparing `ampel_ztf-0.9.0/ampel/ztf/ingest/ZiArchiveMuxer.py` & `ampel_ztf-0.9.1a0/ampel/ztf/ingest/ZiArchiveMuxer.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,15 +108,17 @@
             )
         )
 
 
     @backoff.on_exception(
         backoff.expo,
         requests.HTTPError,
-        giveup=lambda e: not isinstance(e, requests.HTTPError) or e.response.status_code not in {503, 504, 429, 408},
+        giveup=lambda e: not isinstance(e, requests.HTTPError)
+        or e.response is None
+        or e.response.status_code not in {503, 504, 429, 408},
         max_time=600,
     )
     def get_photopoints(self, ztf_name: str, jd_center: float, time_pre: float, time_post: float) -> dict[str, Any]:
         response = self.session.get(
             f"object/{ztf_name}/photopoints",
             params={
                 "jd_end": jd_center+time_post,
```

### Comparing `ampel_ztf-0.9.0/ampel/ztf/ingest/ZiCompilerOptions.py` & `ampel_ztf-0.9.1a0/ampel/ztf/ingest/ZiCompilerOptions.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.9.0/ampel/ztf/ingest/ZiDataPointShaper.py` & `ampel_ztf-0.9.1a0/ampel/ztf/ingest/ZiDataPointShaper.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.9.0/ampel/ztf/ingest/ZiMongoMuxer.py` & `ampel_ztf-0.9.1a0/ampel/ztf/ingest/ZiMongoMuxer.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.9.0/ampel/ztf/ingest/tags.py` & `ampel_ztf-0.9.1a0/ampel/ztf/ingest/tags.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.9.0/ampel/ztf/legacy_utils.py` & `ampel_ztf-0.9.1a0/ampel/ztf/legacy_utils.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.9.0/ampel/ztf/t0/DecentFilter.py` & `ampel_ztf-0.9.1a0/ampel/ztf/t0/DecentFilter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # File:                Ampel-ZTF/ampel/ztf/t0/DecentFilter.py
 # License:             BSD-3-Clause
 # Author:              m. giomi <matteo.giomi@desy.de>
 # Date:                06.06.2018
-# Last Modified Date:  10.03.2021
-# Last Modified By:    Jakob van Santen <jakob.van.santen@desy.de>
+# Last Modified Date:  17.05.2023
+# Last Modified By:    Simeon Reusch <simeon.reusch@desy.de>
 
-import numpy as np
 from typing import Any
-from astropy.table import Table
-from astropy.coordinates import SkyCoord
 
+import numpy as np
 from ampel.abstract.AbsAlertFilter import AbsAlertFilter
-from ampel.ztf.base.CatalogMatchUnit import CatalogMatchUnit
 from ampel.protocol.AmpelAlertProtocol import AmpelAlertProtocol
+from ampel.ztf.base.CatalogMatchUnit import CatalogMatchUnit
+from astropy.coordinates import SkyCoord
+from astropy.table import Table
 
 
 class DecentFilter(CatalogMatchUnit, AbsAlertFilter):
     """
     General-purpose filter with ~ 0.6% acceptance. It selects alerts based on:
     * numper of previous detections
     * positive subtraction flag
@@ -32,16 +32,18 @@
     on the provided PS1 star-galaxy classification.
     """
 
     # History
     min_ndet: int  # number of previous detections
     min_tspan: float  # minimum duration of alert detection history [days]
     max_tspan: float  # maximum duration of alert detection history [days]
-    min_archive_tspan: float = 0. # minimum duration of alert detection history [days]
-    max_archive_tspan: float = 10**5. # maximum duration of alert detection history [days]
+    min_archive_tspan: float = 0.0  # minimum duration of alert detection history [days]
+    max_archive_tspan: float = (
+        10**5.0
+    )  # maximum duration of alert detection history [days]
 
     # Image quality
     min_drb: float = 0.0  # deep learning real bogus score
     min_rb: float  # real bogus score
     max_fwhm: float  # sexctrator FWHM (assume Gaussian) [pix]
     max_elong: float  # Axis ratio of image: aimage / bimage
     max_magdiff: float  # Difference: magap - magpsf [mag]
@@ -62,18 +64,17 @@
     gaia_pm_signif: float  # significance of proper motion detection of GAIA counterpart [sigma]
     gaia_plx_signif: float  # significance of parallax detection of GAIA counterpart [sigma]
     gaia_veto_gmag_min: float  # min gmag for normalized distance cut of GAIA counterparts [mag]
     gaia_veto_gmag_max: float  # max gmag for normalized distance cut of GAIA counterparts [mag]
     gaia_excessnoise_sig_max: float  # maximum allowed noise (expressed as significance) for Gaia match to be trusted.
 
     def post_init(self):
-
         # feedback
         for k in self.__annotations__:
-            self.logger.info(f"Using {k}={getattr(self, k)}")
+            self.logger.debug(f"Using {k}={getattr(self, k)}")
 
         # To make this tenable we should create this list dynamically depending on what entries are required
         # by the filter. Now deciding not to include drb in this list, eg.
         self.keys_to_check = (
             "fwhm",
             "elong",
             "magdiff",
@@ -93,18 +94,18 @@
 
     def _alert_has_keys(self, photop) -> bool:
         """
         check that given photopoint contains all the keys needed to filter
         """
         for el in self.keys_to_check:
             if el not in photop:
-                self.logger.info(None, extra={"missing": el})
+                self.logger.debug(None, extra={"missing": el})
                 return False
             if photop[el] is None:
-                self.logger.info(None, extra={"isNone": el})
+                self.logger.debug(None, extra={"isNone": el})
                 return False
         return True
 
     def get_galactic_latitude(self, transient):
         """
         compute galactic latitude of the transient
         """
@@ -180,15 +181,14 @@
                         "ExcessNoiseSig",
                     ],
                 }
             ],
         )[0]
 
         if srcs:
-
             gaia_tab = Table(
                 [
                     {k: np.nan if v is None else v for k, v in src["body"].items()}
                     for src in srcs
                 ]
             )
 
@@ -223,15 +223,15 @@
             # select just the sources that are close enough and that are not noisy
             gaia_tab = gaia_tab[gaia_tab["FLAG_PROX"]]
             gaia_tab = gaia_tab[gaia_tab["FLAG_Clean"]]
 
             # among the remaining sources there is anything with
             # significant proper motion or parallax measurement
             if (
-                any(gaia_tab["FLAG_PMRA"] == True) # noqa
+                any(gaia_tab["FLAG_PMRA"] == True)  # noqa
                 or any(gaia_tab["FLAG_PMDec"] == True)
                 or any(gaia_tab["FLAG_Plx"] == True)
             ):
                 return True
 
         return False
 
@@ -247,104 +247,103 @@
 
         # CUT ON THE HISTORY OF THE ALERT
         #################################
 
         pps = [el for el in alert.datapoints if el.get("candid") is not None]
         if len(pps) < self.min_ndet:
             # self.logger.debug("rejected: %d photopoints in alert (minimum required %d)"% (npp, self.min_ndet))
-            self.logger.info(None, extra={"nDet": len(pps)})
+            self.logger.debug(None, extra={"nDet": len(pps)})
             return None
 
         # cut on length of detection history
-        detections_jds = [el['jd'] for el in pps]
+        detections_jds = [el["jd"] for el in pps]
         det_tspan = max(detections_jds) - min(detections_jds)
         if not (self.min_tspan <= det_tspan <= self.max_tspan):
             # self.logger.debug("rejected: detection history is %.3f d long, \
             # requested between %.3f and %.3f d"% (det_tspan, self.min_tspan, self.max_tspan))
-            self.logger.info(None, extra={"tSpan": det_tspan})
+            self.logger.debug(None, extra={"tSpan": det_tspan})
             return None
 
         # IMAGE QUALITY CUTS
         ####################
 
         latest = alert.datapoints[0]
         if not self._alert_has_keys(latest):
             return None
 
         if latest["isdiffpos"] == "f" or latest["isdiffpos"] == "0":
             # self.logger.debug("rejected: 'isdiffpos' is %s", latest['isdiffpos'])
-            self.logger.info(None, extra={"isdiffpos": latest["isdiffpos"]})
+            self.logger.debug(None, extra={"isdiffpos": latest["isdiffpos"]})
             return None
 
         if latest["rb"] < self.min_rb:
             # self.logger.debug("rejected: RB score %.2f below threshod (%.2f)"% (latest['rb'], self.min_rb))
-            self.logger.info(None, extra={"rb": latest["rb"]})
+            self.logger.debug(None, extra={"rb": latest["rb"]})
             return None
 
         if self.min_drb > 0.0 and latest["drb"] < self.min_drb:
             # self.logger.debug("rejected: RB score %.2f below threshod (%.2f)"% (latest['rb'], self.min_rb))
-            self.logger.info(None, extra={"drb": latest["drb"]})
+            self.logger.debug(None, extra={"drb": latest["drb"]})
             return None
 
         if latest["fwhm"] > self.max_fwhm:
             # self.logger.debug("rejected: fwhm %.2f above threshod (%.2f)"% (latest['fwhm'], self.max_fwhm))
-            self.logger.info(None, extra={"fwhm": latest["fwhm"]})
+            self.logger.debug(None, extra={"fwhm": latest["fwhm"]})
             return None
 
         if latest["elong"] > self.max_elong:
             # self.logger.debug("rejected: elongation %.2f above threshod (%.2f)"% (latest['elong'], self.max_elong))
-            self.logger.info(None, extra={"elong": latest["elong"]})
+            self.logger.debug(None, extra={"elong": latest["elong"]})
             return None
 
         if abs(latest["magdiff"]) > self.max_magdiff:
             # self.logger.debug("rejected: magdiff (AP-PSF) %.2f above threshod (%.2f)"% (latest['magdiff'], self.max_magdiff))
-            self.logger.info(None, extra={"magdiff": latest["magdiff"]})
+            self.logger.debug(None, extra={"magdiff": latest["magdiff"]})
             return None
 
         # cut on archive length
-        if 'jdendhist' in latest.keys() and 'jdstarthist' in latest.keys():
-            archive_tspan = latest['jdendhist'] - latest['jdstarthist']
+        if "jdendhist" in latest.keys() and "jdstarthist" in latest.keys():
+            archive_tspan = latest["jdendhist"] - latest["jdstarthist"]
             if not (self.min_archive_tspan < archive_tspan < self.max_archive_tspan):
-                self.logger.info(None, extra={'archive_tspan': archive_tspan})
+                self.logger.debug(None, extra={"archive_tspan": archive_tspan})
                 return None
 
-
         # ASTRONOMY
         ###########
 
         # check for closeby ss objects
         if 0 <= latest["ssdistnr"] < self.min_sso_dist:
             # self.logger.debug("rejected: solar-system object close to transient (max allowed: %d)."% (self.min_sso_dist))
-            self.logger.info(None, extra={"ssdistnr": latest["ssdistnr"]})
+            self.logger.debug(None, extra={"ssdistnr": latest["ssdistnr"]})
             return None
 
         # cut on galactic latitude
         b = self.get_galactic_latitude(latest)
         if abs(b) < self.min_gal_lat:
             # self.logger.debug("rejected: b=%.4f, too close to Galactic plane (max allowed: %f)."% (b, self.min_gal_lat))
-            self.logger.info(None, extra={"galPlane": abs(b)})
+            self.logger.debug(None, extra={"galPlane": abs(b)})
             return None
 
         # check ps1 star-galaxy score
         if self.is_star_in_PS1(latest):
             # self.logger.debug("rejected: closest PS1 source %.2f arcsec away with sgscore of %.2f"% (latest['distpsnr1'], latest['sgscore1']))
-            self.logger.info(None, extra={"distpsnr1": latest["distpsnr1"]})
+            self.logger.debug(None, extra={"distpsnr1": latest["distpsnr1"]})
             return None
 
         if self.is_confused_in_PS1(latest):
             # self.logger.debug("rejected: three confused PS1 sources within %.2f arcsec from alert."% (self.ps1_confusion_rad))
-            self.logger.info(None, extra={"ps1Confusion": True})
+            self.logger.debug(None, extra={"ps1Confusion": True})
             return None
 
         # check with gaia
         if self.gaia_rs > 0 and self.is_star_in_gaia(latest):
             # self.logger.debug("rejected: within %.2f arcsec from a GAIA start (PM of PLX)" % (self.gaia_rs))
-            self.logger.info(None, extra={"gaiaIsStar": True})
+            self.logger.debug(None, extra={"gaiaIsStar": True})
             return None
 
         # self.logger.debug("Alert %s accepted. Latest pp ID: %d"%(alert.tran_id, latest['candid']))
         self.logger.debug("Alert accepted", extra={"latestPpId": latest["candid"]})
 
         # for key in self.keys_to_check:
-        # 	self.logger.debug("{}: {}".format(key, latest[key]))
+        #   self.logger.debug("{}: {}".format(key, latest[key]))
 
         return True
```

### Comparing `ampel_ztf-0.9.0/ampel/ztf/t0/T0HealpixPathProcessor.py` & `ampel_ztf-0.9.1a0/ampel/ztf/t0/T0HealpixPathProcessor.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.9.0/ampel/ztf/t0/T0HealpixProcessor.py` & `ampel_ztf-0.9.1a0/ampel/ztf/t0/T0HealpixProcessor.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.9.0/ampel/ztf/t0/ZTFAlertStreamController.py` & `ampel_ztf-0.9.1a0/ampel/ztf/t0/ZTFAlertStreamController.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
     def scale(self, name: None | str = None, multiplier: int = 1) -> None:
         if multiplier < 1:
             raise ValueError("multiplier must be nonnegative")
         assert self._scale_event
         self.multiplier = multiplier
         self._scale_event.set()
 
-    async def run(self) -> Sequence[bool]:
+    async def run(self) -> Sequence[bool | BaseException]:
         """
         Keep `self.multiplier` instances of this process alive until:
           
           * they all return 0/False, or
           * the task is cancelend,
         
         whichever comes first.
```

### Comparing `ampel_ztf-0.9.0/ampel/ztf/t0/load/AllConsumingConsumer.py` & `ampel_ztf-0.9.1a0/ampel/ztf/t0/load/AllConsumingConsumer.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 # Last Modified By:    valery brinnel <firstname.lastname@gmail.com>
 
 import enum
 import json
 import sys
 import time
 import uuid
+from collections.abc import Collection
 
 import confluent_kafka
 
 from ampel.metrics.AmpelMetricsRegistry import AmpelMetricsRegistry
 from ampel.protocol.LoggerProtocol import LoggerProtocol
 
 
@@ -108,15 +109,18 @@
         broker,
         timeout=None,
         topics=["^ztf_.*"],
         auto_commit=True,
         logger: None | LoggerProtocol=None,
         **consumer_config,
     ):
-        """ """
+        """
+        :param auto_commit: implicitly store the offset of the last emitted
+            message on the next call to consume()
+        """
 
         self._metrics = KafkaMetrics.instance()
         config = {
             "bootstrap.servers": broker,
             "default.topic.config": {"auto.offset.reset": "smallest"},
             "enable.auto.commit": True,
             "receive.message.max.bytes": 2**29,
@@ -151,14 +155,34 @@
             raise StopIteration
         else:
             return message
 
     def __iter__(self):
         return self
 
+    def store_offsets(
+        self,
+        offsets: Collection[confluent_kafka.TopicPartition],
+    ):
+        if self._logger:
+            self._logger.debug(f"Storing offsets: {offsets}")
+        try:
+            self._consumer.store_offsets(offsets=offsets)
+        except confluent_kafka.KafkaException as exc:
+            # librdkafka will refuse to store offsets on a partition that is not
+            # currently assigned. this can happen if the group is rebalanced
+            # while a batch of messages is in flight. see also:
+            # https://github.com/confluentinc/confluent-kafka-dotnet/issues/1861
+            err = exc.args[0]
+            if err.code() == confluent_kafka.KafkaError._STATE:
+                ...
+            else:
+                raise KafkaError(err)
+
+
     def commit(self):
         if self._offsets:
             offsets = [
                 confluent_kafka.TopicPartition(topic, partition, offset + 1)
                 for (topic, partition), offset in self._offsets.items()
             ]
             if self._logger:
@@ -178,15 +202,21 @@
         Block until one message has arrived, and return it.
 
         Messages returned to the caller marked for committal
         upon the _next_ call to consume().
         """
         # mark the last emitted message for committal
         if self._auto_commit:
-            self.commit()
+            self.store_offsets(
+                [
+                    confluent_kafka.TopicPartition(topic, partition, offset + 1)
+                    for (topic, partition), offset in self._offsets.items()
+                ]
+            )
+            self._offsets.clear()
 
         message = None
         for _ in range(self._poll_attempts):
             # wake up occasionally to catch SIGINT
             message = self._consumer.poll(self._poll_interval)
             if message is not None:
                 if err := message.error():
```

### Comparing `ampel_ztf-0.9.0/ampel/ztf/t0/load/UWAlertLoader.py` & `ampel_ztf-0.9.1a0/ampel/ztf/t0/load/UWAlertLoader.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,14 +61,15 @@
         :returns: dict instance of the alert content
         :raises StopIteration: when next(fastavro.reader) has dried out
         """
         topic_stats: defaultdict[str, list[float]] = defaultdict(lambda: [float("inf"), -float("inf"), 0])
         for message in itertools.islice(self._consumer, limit):
             reader = fastavro.reader(io.BytesIO(message.value()))
             alert = next(reader)  # raise StopIteration
+            assert isinstance(alert, dict)
             stats = topic_stats[message.topic()]
             if alert["candidate"]["jd"] < stats[0]:
                 stats[0] = alert["candidate"]["jd"]
             if alert["candidate"]["jd"] > stats[1]:
                 stats[1] = alert["candidate"]["jd"]
             stats[2] += 1
             yield io.BytesIO(message.value())
```

### Comparing `ampel_ztf-0.9.0/ampel/ztf/t0/load/ZTFAlertArchiver.py` & `ampel_ztf-0.9.1a0/ampel/ztf/t0/load/ZTFAlertArchiver.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.9.0/ampel/ztf/t0/load/ZTFAlertArchiverV3.py` & `ampel_ztf-0.9.1a0/ampel/ztf/t0/load/ZTFAlertArchiverV3.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,15 @@
         # the _next_ iteration of the loop. this ensures that the offsets
         # are only committed once the chunk is actually archived.
         def emit() -> Iterator[bytes]:
             nonlocal schema
             if not alerts:
                 return
             chunk = io.BytesIO()
+            assert schema is not None
             fastavro.writer(chunk, schema, alerts)
             yield chunk.getvalue()
             alerts.clear()
             schema = None
             self.consumer.commit()
 
         for message in self.consumer:
```

### Comparing `ampel_ztf-0.9.0/ampel/ztf/t0/load/ZTFArchiveAlertLoader.py` & `ampel_ztf-0.9.1a0/ampel/ztf/t0/load/ZTFArchiveAlertLoader.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # File:                Ampel-ZTF/ampel/ztf/t0/load/ZTFArchiveAlertLoader.py
 # License:             BSD-3-Clause
 # Author:              jvs
 # Date:                20.10.2021
-# Last Modified Date:  22.12.2022
-# Last Modified By:    valery brinnel <firstname.lastname@gmail.com>
+# Last Modified Date:  17.05.2023
+# Last Modified By:    Simeon Reusch <simeon.reusch@desy.de>
 
-import logging, backoff, requests
+import logging
 from typing import Any
+
+import backoff
+import requests
 from ampel.abstract.AbsAlertLoader import AbsAlertLoader
 from ampel.base.AmpelBaseModel import AmpelBaseModel
 
 log = logging.getLogger(__name__)
 
 
 class ZTFSource(AmpelBaseModel):
@@ -36,14 +39,16 @@
 
     #: Base URL of archive service
     archive: str = "https://ampel.zeuthen.desy.de/api/ztf/archive/v3"
 
     #: A stream identifier, created via POST /api/ztf/archive/streams/, or a query
     stream: None | str | ZTFSource = '%%ztf_stream_token'
 
+    with_history: bool = True
+
     def __init__(self, **kwargs) -> None:
         super().__init__(**kwargs)
         self._it = None
 
     def __iter__(self):
         return self.get_alerts()
 
@@ -59,52 +64,65 @@
             while True:
                 chunk = self._get_chunk(session)
                 yield from chunk["alerts"] if isinstance(chunk, dict) else chunk
                 # NB: if generator exits before we get here, chunk is never acknowledged
                 if "chunk" in chunk:
                     self._acknowledge_chunk(session, chunk["chunk"])
                     log.info(
-                        None, extra={"streamToken": self.stream, "chunk": chunk["chunk"]}
+                        None,
+                        extra={"streamToken": self.stream, "chunk": chunk["chunk"]},
                     )
                 if isinstance(self.stream, ZTFSource) or (
                     len(chunk["alerts"]) == 0 and chunk["remaining"]["chunks"] == 0
                 ):
                     break
 
     @backoff.on_exception(
         backoff.expo,
         requests.HTTPError,
-        giveup = lambda e: (
-            not isinstance(e, requests.HTTPError) or
-            e.response.status_code not in {502, 503, 504, 429, 408}
+        giveup=lambda e: (
+            not isinstance(e, requests.HTTPError)
+            or e.response is None
+            or e.response.status_code not in {502, 503, 504, 429, 408, 423}
         ),
-        max_time = 600,
+        max_time=600,
     )
     def _get_chunk(self, session: requests.Session) -> dict[str, Any]:
-
         if isinstance(self.stream, ZTFSource):
             params = {"with_history": self.stream.with_history}
             for k in ("jd_start", "jd_end", "programid"):
                 if (x := getattr(self.stream, k)) is not None:
                     params[k] = x
             response = session.get(
                 f"{self.archive}/object/{self.stream.ztf_name}/alerts",
-                headers = {"Authorization": f"bearer {self.stream.archive_token}"},
-                params = params
+                headers={"Authorization": f"bearer {self.stream.archive_token}"},
+                params=params,
             )
         else:
-            response = session.get(f"{self.archive}/stream/{self.stream}/chunk")
+            response = session.get(
+                f"{self.archive}/stream/{self.stream}/chunk",
+                params={"with_history": self.with_history},
+            )
+            remaining_chunks: int | None = (
+                response.json().get("remaining", {}).get("chunks")
+            )
+            if remaining_chunks is not None:
+                self.logger.info(f"Remaining chunks: {remaining_chunks}")
+
         response.raise_for_status()
         return response.json()
 
     @backoff.on_exception(
         backoff.expo,
         requests.HTTPError,
-        giveup = (
-            lambda e: not isinstance(e, requests.HTTPError) or
-            e.response.status_code not in {502, 503, 504, 429, 408}
+        giveup=(
+            lambda e: not isinstance(e, requests.HTTPError)
+            or e.response is None
+            or e.response.status_code not in {502, 503, 504, 429, 408}
         ),
-        max_time = 600,
+        max_time=600,
     )
     def _acknowledge_chunk(self, session: requests.Session, chunk_id: int) -> None:
-        response = session.post(f"{self.archive}/stream/{self.stream}/chunk/{chunk_id}/acknowledge")
+        response = session.post(
+            f"{self.archive}/stream/{self.stream}/chunk/{chunk_id}/acknowledge"
+        )
         response.raise_for_status()
```

### Comparing `ampel_ztf-0.9.0/ampel/ztf/t0/load/avroutils.py` & `ampel_ztf-0.9.1a0/ampel/ztf/t0/load/avroutils.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.9.0/ampel/ztf/t0/load/fetcherutils.py` & `ampel_ztf-0.9.1a0/ampel/ztf/t0/load/fetcherutils.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.9.0/ampel/ztf/t1/ZiT1Combiner.py` & `ampel_ztf-0.9.1a0/ampel/ztf/t1/ZiT1Combiner.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.9.0/ampel/ztf/t1/ZiT1RetroCombiner.py` & `ampel_ztf-0.9.1a0/ampel/ztf/t1/ZiT1RetroCombiner.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.9.0/ampel/ztf/t2/T2CatalogMatch.py` & `ampel_ztf-0.9.1a0/ampel/ztf/t2/T2CatalogMatch.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.9.0/ampel/ztf/t2/T2LightCurveFeatures.py` & `ampel_ztf-0.9.1a0/ampel/ztf/t2/T2LightCurveFeatures.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.9.0/ampel/ztf/t2/T2LightCurveSummary.py` & `ampel_ztf-0.9.1a0/ampel/ztf/t2/T2LightCurveSummary.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.9.0/ampel/ztf/t3/T3LegacyExtJournalAppender.py` & `ampel_ztf-0.9.1a0/ampel/ztf/t3/T3LegacyExtJournalAppender.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.9.0/ampel/ztf/t3/complement/FritzReport.py` & `ampel_ztf-0.9.1a0/ampel/ztf/t3/complement/FritzReport.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.9.0/ampel/ztf/t3/complement/GROWTHMarshalReport.py` & `ampel_ztf-0.9.1a0/ampel/ztf/t3/complement/GROWTHMarshalReport.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,14 +37,15 @@
             else:
                 record["extra"][self.__class__.__name__] = report
 
     @backoff.on_exception(
         backoff.expo,
         requests.HTTPError,
         giveup=lambda e: not isinstance(e, requests.HTTPError)
+        or e.response is None
         or e.response.status_code not in {502, 503, 429},
         max_time=60,
     )
     def _lookup(self, name) -> None | dict[str, Any]:
         response = self.session.get(f"catalogs/GROWTHMarshal/{name}")
         if response.status_code == 404:
             return None
```

### Comparing `ampel_ztf-0.9.0/ampel/ztf/t3/complement/TNSNames.py` & `ampel_ztf-0.9.1a0/ampel/ztf/t3/complement/TNSNames.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.9.0/ampel/ztf/t3/complement/TNSReports.py` & `ampel_ztf-0.9.1a0/ampel/ztf/t3/complement/TNSReports.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.9.0/ampel/ztf/t3/complement/ZTFCutoutImages.py` & `ampel_ztf-0.9.1a0/ampel/ztf/t3/complement/ZTFCutoutImages.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,15 @@
         max_tries=5,
         factor=10,
     )
     @backoff.on_exception(
         backoff.expo,
         requests.HTTPError,
         giveup=lambda e: not isinstance(e, requests.HTTPError)
+        or e.response is None
         or e.response.status_code not in {502, 503, 504, 429, 408},
         max_time=60,
     )
     def get_cutout(self, candid: int) -> None | dict[str, bytes]:
         response = self.session.get(f"cutouts/{candid}")
         if response.status_code == 404:
             return None
```

### Comparing `ampel_ztf-0.9.0/ampel/ztf/t3/select/T3AdHocStockSelector.py` & `ampel_ztf-0.9.1a0/ampel/ztf/t3/select/T3AdHocStockSelector.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.9.0/ampel/ztf/t3/skyportal/SkyPortalClient.py` & `ampel_ztf-0.9.1a0/ampel/ztf/t3/skyportal/SkyPortalClient.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,15 @@
     with gzip.open(io.BytesIO(cutout_data), "rb") as f:
         with fits.open(f) as hdu:
             # header = hdu[0].header
             img = np.flipud(hdu[0].data)
     mask = np.isfinite(img)
 
     fig = Figure(figsize=(1, 1))
-    ax = fig.add_axes([0.0, 0.0, 1.0, 1.0])
+    ax = fig.add_axes((0.0, 0.0, 1.0, 1.0))
     ax.set_axis_off()
     ax.imshow(
         img,
         # clip pixel values below the median
         norm=Normalize(*np.percentile(img[mask], [0.5, 99.5])),
         aspect="auto",
         origin="lower",
```

### Comparing `ampel_ztf-0.9.0/ampel/ztf/t3/skyportal/SkyPortalPublisher.py` & `ampel_ztf-0.9.1a0/ampel/ztf/t3/skyportal/SkyPortalPublisher.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.9.0/ampel/ztf/t4/T4ZTFArchiveTokenGenerator.py` & `ampel_ztf-0.9.1a0/ampel/ztf/t4/T4ZTFArchiveTokenGenerator.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.9.0/ampel/ztf/util/ZTFIdMapper.py` & `ampel_ztf-0.9.1a0/ampel/ztf/util/ZTFIdMapper.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.9.0/ampel/ztf/util/ZTFNoisifiedIdMapper.py` & `ampel_ztf-0.9.1a0/ampel/ztf/util/ZTFNoisifiedIdMapper.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.9.0/ampel/ztf/view/ZTFT2Tabulator.py` & `ampel_ztf-0.9.1a0/ampel/ztf/view/ZTFT2Tabulator.py`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.9.0/conf/ampel-ztf/ampel.yml` & `ampel_ztf-0.9.1a0/conf/ampel-ztf/ampel.yml`

 * *Files identical despite different names*

### Comparing `ampel_ztf-0.9.0/pyproject.toml` & `ampel_ztf-0.9.1a0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ampel-ztf"
-version = "0.9.0"
+version = "0.9.1a0"
 description = "Zwicky Transient Facility support for the Ampel system"
 authors = [
     "Valery Brinnel",
     "Jakob van Santen <jakob.van.santen@desy.de>",
     "Sjoert van Velzen",
     "Jakob Nordin",
 ]
@@ -32,44 +32,43 @@
     'conf/*/*/*.yaml',
     'conf/*/*.yml',
     'conf/*/*/*.yml',
 ]
 
 
 [tool.poetry.dependencies]
-python = ">=3.10,<3.12"
+python = "^3.10"
 astropy = "^5.0"
 matplotlib = "^3.3.4"
 aiohttp = "^3.7.3"
 nest-asyncio = "^1.4.3"
 backoff = "^2.0.0"
 fastavro = "~1.6.0"
 requests = "^2.25.1"
-requests-toolbelt = "^0.10.0"
+requests-toolbelt = "^1.0.0"
 confluent-kafka = {version = "^2.0.0", optional = true}
 healpy = {version = "^1.15", optional = true}
 light-curve = {version = ">=0.7,<0.8", optional = true}
 ampel-ztf-archive = {version = "^0.8.0-alpha.0", optional = true}
-ampel-interface = "^0.9.0"
-ampel-core = "^0.9.0"
-ampel-photometry = "^0.9.0"
-ampel-alerts = "^0.9.0"
-ampel-plot = {version = "^0.8.3-3", optional = true}
+ampel-core = "^0.9.1a0"
+ampel-photometry = "^0.9.1a0"
+ampel-alerts = "^0.9.1a0"
+ampel-plot = {version = "^0.8.3-3", optional = true, python = "<3.12"}
 pandas = {version = "^1.5.2", optional = true}
 scipy = "^1.9.3"
-planobs = {version = "^0.6.1", optional = true}
+planobs = {version = "^0.7.0", optional = true}
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.2.2"
-pytest-cov = "^4.0.0"
-pytest-mock = "^3.10.0"
+pytest = "^7.4.2"
+pytest-cov = "^4.1.0"
+pytest-mock = "^3.11.1"
 mongomock = "^4.1.2"
-mypy = "^1.1.1"
-pytest-timeout = "^2.1.0"
-pytest-asyncio = "^0.21.0"
+mypy = "^1.6.0"
+pytest-timeout = "^2.2.0"
+pytest-asyncio = "^0.21.1"
 types-requests = "^2.25.9"
 before_after = "^1.0.1"
 
 [tool.poetry.extras]
 archive = ["ampel-ztf-archive"]
 healpix = ["healpy"]
 light-curve = ["light-curve"]
```

### Comparing `ampel_ztf-0.9.0/PKG-INFO` & `ampel_ztf-0.9.1a0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 Metadata-Version: 2.1
 Name: ampel-ztf
-Version: 0.9.0
+Version: 0.9.1a0
 Summary: Zwicky Transient Facility support for the Ampel system
 Home-page: https://ampelproject.github.io
 License: BSD-3-Clause
 Author: Valery Brinnel
 Maintainer: Jakob van Santen
 Maintainer-email: jakob.van.santen@desy.de
-Requires-Python: >=3.10,<3.12
+Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Typing :: Typed
 Provides-Extra: archive
 Provides-Extra: bayes
 Provides-Extra: fp
 Provides-Extra: healpix
 Provides-Extra: kafka
 Provides-Extra: light-curve
 Provides-Extra: plot
 Requires-Dist: aiohttp (>=3.7.3,<4.0.0)
-Requires-Dist: ampel-alerts (>=0.9.0,<0.10.0)
-Requires-Dist: ampel-core (>=0.9.0,<0.10.0)
-Requires-Dist: ampel-interface (>=0.9.0,<0.10.0)
-Requires-Dist: ampel-photometry (>=0.9.0,<0.10.0)
-Requires-Dist: ampel-plot (>=0.8.3-3,<0.9.0) ; extra == "plot" or extra == "bayes"
+Requires-Dist: ampel-alerts (>=0.9.1a0,<0.10.0)
+Requires-Dist: ampel-core (>=0.9.1a0,<0.10.0)
+Requires-Dist: ampel-photometry (>=0.9.1a0,<0.10.0)
+Requires-Dist: ampel-plot (>=0.8.3-3,<0.9.0) ; (python_version < "3.12") and (extra == "plot" or extra == "bayes")
 Requires-Dist: ampel-ztf-archive (>=0.8.0-alpha.0,<0.9.0) ; extra == "archive"
 Requires-Dist: astropy (>=5.0,<6.0)
 Requires-Dist: backoff (>=2.0.0,<3.0.0)
 Requires-Dist: confluent-kafka (>=2.0.0,<3.0.0) ; extra == "kafka"
 Requires-Dist: fastavro (>=1.6.0,<1.7.0)
 Requires-Dist: healpy (>=1.15,<2.0) ; extra == "healpix"
 Requires-Dist: light-curve (>=0.7,<0.8) ; extra == "light-curve"
 Requires-Dist: matplotlib (>=3.3.4,<4.0.0)
 Requires-Dist: nest-asyncio (>=1.4.3,<2.0.0)
 Requires-Dist: pandas (>=1.5.2,<2.0.0) ; extra == "fp" or extra == "bayes"
-Requires-Dist: planobs (>=0.6.1,<0.7.0) ; extra == "fp" or extra == "bayes"
+Requires-Dist: planobs (>=0.7.0,<0.8.0) ; extra == "fp" or extra == "bayes"
 Requires-Dist: requests (>=2.25.1,<3.0.0)
-Requires-Dist: requests-toolbelt (>=0.10.0,<0.11.0)
+Requires-Dist: requests-toolbelt (>=1.0.0,<2.0.0)
 Requires-Dist: scipy (>=1.9.3,<2.0.0)
 Project-URL: Repository, https://github.com/AmpelProject/Ampel-ZTF
 Description-Content-Type: text/markdown
 
 
 
 <img align="left" src="https://desycloud.desy.de/index.php/s/6gJs9bYBG3tWFDz/preview" width="150" height="150"/>
```

