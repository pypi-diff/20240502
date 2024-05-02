# Comparing `tmp/dcm-processor-1.1.2.tar.gz` & `tmp/dcm-processor-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcm-processor-1.1.2.tar", last modified: Tue Jun 20 09:46:41 2023, max compression
+gzip compressed data, was "dcm-processor-1.1.3.tar", last modified: Thu May  2 07:15:41 2024, max compression
```

## Comparing `dcm-processor-1.1.2.tar` & `dcm-processor-1.1.3.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-06-20 09:46:41.286114 dcm-processor-1.1.2/
--rwxr-xr-x   0 giles     (1000) giles     (1000)     1074 2021-05-11 10:55:48.000000 dcm-processor-1.1.2/LICENSE
--rwxr-xr-x   0 giles     (1000) giles     (1000)     6335 2023-06-20 09:46:41.286447 dcm-processor-1.1.2/PKG-INFO
--rwxr-xr-x   0 giles     (1000) giles     (1000)     5834 2023-04-17 10:06:58.000000 dcm-processor-1.1.2/README.md
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-06-20 09:46:41.094697 dcm-processor-1.1.2/dcm_processor/
--rwxr-xr-x   0 giles     (1000) giles     (1000)       61 2021-10-17 14:30:50.000000 dcm-processor-1.1.2/dcm_processor/__init__.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)    15407 2023-05-17 16:40:44.000000 dcm-processor-1.1.2/dcm_processor/argparser.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)    33214 2023-05-17 11:54:45.000000 dcm-processor-1.1.2/dcm_processor/files.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)    46033 2023-04-19 12:36:49.000000 dcm-processor-1.1.2/dcm_processor/script.py
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-06-20 09:46:41.055470 dcm-processor-1.1.2/dcm_processor/services/
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-06-20 09:46:41.054917 dcm-processor-1.1.2/dcm_processor/services/base/
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-06-20 09:46:41.117614 dcm-processor-1.1.2/dcm_processor/services/base/module/
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-06-20 09:46:41.202930 dcm-processor-1.1.2/dcm_processor/services/base/module/DicomAnonymizerService/
--rwxr-xr-x   0 giles     (1000) giles     (1000)   642195 2021-10-17 16:16:14.000000 dcm-processor-1.1.2/dcm_processor/services/base/module/DicomAnonymizerService/CTP.jar
--rwxr-xr-x   0 giles     (1000) giles     (1000)    17869 2021-10-17 16:16:15.000000 dcm-processor-1.1.2/dcm_processor/services/base/module/DicomAnonymizerService/DAT.jar
--rwxr-xr-x   0 giles     (1000) giles     (1000)      526 2023-04-06 14:13:53.000000 dcm-processor-1.1.2/dcm_processor/services/base/module/DicomAnonymizerService/__init__.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)     1590 2023-05-12 10:21:10.000000 dcm-processor-1.1.2/dcm_processor/services/base/module/DicomAnonymizerService/anonymize.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)    69564 2021-10-17 16:16:15.000000 dcm-processor-1.1.2/dcm_processor/services/base/module/DicomAnonymizerService/clibwrapper_jiio-1.2-pre-dr-b04.jar
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-06-20 09:46:41.212945 dcm-processor-1.1.2/dcm_processor/services/base/module/DicomAnonymizerService/config/
--rwxr-xr-x   0 giles     (1000) giles     (1000)    59932 2023-06-14 13:28:44.000000 dcm-processor-1.1.2/dcm_processor/services/base/module/DicomAnonymizerService/config/dicom-anonymizer.script
--rwxr-xr-x   0 giles     (1000) giles     (1000)      248 2021-10-17 16:16:15.000000 dcm-processor-1.1.2/dcm_processor/services/base/module/DicomAnonymizerService/config/hash_table.csv
--rwxr-xr-x   0 giles     (1000) giles     (1000)       86 2021-10-17 16:16:15.000000 dcm-processor-1.1.2/dcm_processor/services/base/module/DicomAnonymizerService/config/psudonyms.csv
--rwxr-xr-x   0 giles     (1000) giles     (1000)    10424 2021-10-17 16:16:15.000000 dcm-processor-1.1.2/dcm_processor/services/base/module/DicomAnonymizerService/dcm4che-imageio-rle-2.0.25.jar
--rwxr-xr-x   0 giles     (1000) giles     (1000)   863881 2021-10-17 16:16:16.000000 dcm-processor-1.1.2/dcm_processor/services/base/module/DicomAnonymizerService/dcm4che.jar
--rwxr-xr-x   0 giles     (1000) giles     (1000)     3479 2023-05-26 10:55:08.000000 dcm-processor-1.1.2/dcm_processor/services/base/module/DicomAnonymizerService/fhir_lib.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)  1172845 2021-10-17 16:16:18.000000 dcm-processor-1.1.2/dcm_processor/services/base/module/DicomAnonymizerService/jai_imageio-1.2-pre-dr-b04.jar
--rwxr-xr-x   0 giles     (1000) giles     (1000)   391834 2021-10-17 16:16:19.000000 dcm-processor-1.1.2/dcm_processor/services/base/module/DicomAnonymizerService/log4j.jar
--rwxr-xr-x   0 giles     (1000) giles     (1000)    28241 2021-10-17 16:16:19.000000 dcm-processor-1.1.2/dcm_processor/services/base/module/DicomAnonymizerService/pixelmed_codec.jar
--rwxr-xr-x   0 giles     (1000) giles     (1000)   338969 2021-10-17 16:16:20.000000 dcm-processor-1.1.2/dcm_processor/services/base/module/DicomAnonymizerService/util.jar
--rwxr-xr-x   0 giles     (1000) giles     (1000)     1777 2023-03-31 20:09:03.000000 dcm-processor-1.1.2/dcm_processor/services/base/module/DicomAnonymizerService/utils.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)       26 2021-10-17 16:16:20.000000 dcm-processor-1.1.2/dcm_processor/services/base/module/requirements.txt
--rwxr-xr-x   0 giles     (1000) giles     (1000)       72 2021-10-17 16:16:20.000000 dcm-processor-1.1.2/dcm_processor/services/base/module/script.sh
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-06-20 09:46:41.230374 dcm-processor-1.1.2/dcm_processor/services/base/module/storageManager/
--rwxr-xr-x   0 giles     (1000) giles     (1000)       24 2021-10-17 16:16:20.000000 dcm-processor-1.1.2/dcm_processor/services/base/module/storageManager/__init__.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)       95 2023-05-11 22:55:55.000000 dcm-processor-1.1.2/dcm_processor/services/base/module/storageManager/header_codes.json
--rwxr-xr-x   0 giles     (1000) giles     (1000)     6218 2023-01-31 18:15:24.000000 dcm-processor-1.1.2/dcm_processor/services/base/module/storageManager/lib.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)    10622 2023-05-11 22:55:44.000000 dcm-processor-1.1.2/dcm_processor/services/base/module/storageManager/main.py
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-06-20 09:46:41.235477 dcm-processor-1.1.2/dcm_processor/services/base/module/systemcleaner/
--rwxr-xr-x   0 giles     (1000) giles     (1000)       24 2021-10-17 16:16:20.000000 dcm-processor-1.1.2/dcm_processor/services/base/module/systemcleaner/__init__.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)     3908 2023-04-28 08:48:28.000000 dcm-processor-1.1.2/dcm_processor/services/base/module/systemcleaner/main.py
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-06-20 09:46:41.249408 dcm-processor-1.1.2/dcm_processor/services/base/registry/
--rwxr-xr-x   0 giles     (1000) giles     (1000)      491 2023-04-28 08:35:17.000000 dcm-processor-1.1.2/dcm_processor/services/base/registry/__init__.py
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-06-20 09:46:41.057350 dcm-processor-1.1.2/dcm_processor/services/dcm2nii/
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-06-20 09:46:41.276710 dcm-processor-1.1.2/dcm_processor/services/dcm2nii/module/
--rwxr-xr-x   0 giles     (1000) giles     (1000)     4030 2023-04-14 14:47:11.000000 dcm-processor-1.1.2/dcm_processor/services/dcm2nii/module/__init__.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)  1948128 2023-03-02 19:03:11.000000 dcm-processor-1.1.2/dcm_processor/services/dcm2nii/module/dcm2niix
--rwxr-xr-x   0 giles     (1000) giles     (1000)      406 2023-03-24 20:50:04.000000 dcm-processor-1.1.2/dcm_processor/services/dcm2nii/module/lib.py
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-06-20 09:46:41.285053 dcm-processor-1.1.2/dcm_processor/services/dcm2nii/registry/
--rwxr-xr-x   0 giles     (1000) giles     (1000)     1013 2023-04-14 12:17:35.000000 dcm-processor-1.1.2/dcm_processor/services/dcm2nii/registry/__init__.py
--rwxr-xr-x   0 giles     (1000) giles     (1000)      288 2023-04-18 12:25:35.000000 dcm-processor-1.1.2/dcm_processor/services/dcm2nii/registry/settings.json
--rwxr-xr-x   0 giles     (1000) giles     (1000)     6682 2023-04-21 16:23:38.000000 dcm-processor-1.1.2/dcm_processor/worker.py
-drwxr-xr-x   0 giles     (1000) giles     (1000)        0 2023-06-20 09:46:41.111460 dcm-processor-1.1.2/dcm_processor.egg-info/
--rwxr-xr-x   0 giles     (1000) giles     (1000)     6335 2023-06-20 09:46:39.000000 dcm-processor-1.1.2/dcm_processor.egg-info/PKG-INFO
--rwxr-xr-x   0 giles     (1000) giles     (1000)     2368 2023-06-20 09:46:40.000000 dcm-processor-1.1.2/dcm_processor.egg-info/SOURCES.txt
--rwxr-xr-x   0 giles     (1000) giles     (1000)        1 2023-06-20 09:46:39.000000 dcm-processor-1.1.2/dcm_processor.egg-info/dependency_links.txt
--rwxr-xr-x   0 giles     (1000) giles     (1000)       53 2023-06-20 09:46:39.000000 dcm-processor-1.1.2/dcm_processor.egg-info/entry_points.txt
--rwxr-xr-x   0 giles     (1000) giles     (1000)       76 2023-06-20 09:46:39.000000 dcm-processor-1.1.2/dcm_processor.egg-info/requires.txt
--rwxr-xr-x   0 giles     (1000) giles     (1000)       14 2023-06-20 09:46:39.000000 dcm-processor-1.1.2/dcm_processor.egg-info/top_level.txt
--rwxr-xr-x   0 giles     (1000) giles     (1000)       89 2021-10-17 14:23:09.000000 dcm-processor-1.1.2/pyproject.toml
--rwxr-xr-x   0 giles     (1000) giles     (1000)      980 2023-06-20 09:46:41.287873 dcm-processor-1.1.2/setup.cfg
--rwxr-xr-x   0 giles     (1000) giles     (1000)      109 2021-10-17 19:37:23.000000 dcm-processor-1.1.2/setup.py
+drwxrwxr-x   0 giles     (1000) giles     (1000)        0 2024-05-02 07:15:41.023697 dcm-processor-1.1.3/
+-rw-rw-r--   0 giles     (1000) giles     (1000)     1074 2024-05-02 06:52:40.000000 dcm-processor-1.1.3/LICENSE
+-rw-r--r--   0 giles     (1000) giles     (1000)     6486 2024-05-02 07:15:41.023697 dcm-processor-1.1.3/PKG-INFO
+-rw-rw-r--   0 giles     (1000) giles     (1000)     5834 2024-05-02 06:52:40.000000 dcm-processor-1.1.3/README.md
+drwxrwxr-x   0 giles     (1000) giles     (1000)        0 2024-05-02 07:15:41.019697 dcm-processor-1.1.3/dcm_processor/
+-rw-rw-r--   0 giles     (1000) giles     (1000)       61 2024-05-02 06:52:40.000000 dcm-processor-1.1.3/dcm_processor/__init__.py
+-rw-rw-r--   0 giles     (1000) giles     (1000)    15407 2024-05-02 06:52:40.000000 dcm-processor-1.1.3/dcm_processor/argparser.py
+-rw-rw-r--   0 giles     (1000) giles     (1000)    33214 2024-05-02 06:52:40.000000 dcm-processor-1.1.3/dcm_processor/files.py
+-rw-rw-r--   0 giles     (1000) giles     (1000)    46033 2024-05-02 06:52:40.000000 dcm-processor-1.1.3/dcm_processor/script.py
+drwxrwxr-x   0 giles     (1000) giles     (1000)        0 2024-05-02 07:15:41.019697 dcm-processor-1.1.3/dcm_processor/services/
+drwxrwxr-x   0 giles     (1000) giles     (1000)        0 2024-05-02 07:15:41.019697 dcm-processor-1.1.3/dcm_processor/services/base/
+drwxrwxr-x   0 giles     (1000) giles     (1000)        0 2024-05-02 07:15:41.019697 dcm-processor-1.1.3/dcm_processor/services/base/module/
+drwxrwxr-x   0 giles     (1000) giles     (1000)        0 2024-05-02 07:15:41.019697 dcm-processor-1.1.3/dcm_processor/services/base/module/DicomAnonymizerService/
+-rw-rw-r--   0 giles     (1000) giles     (1000)   642195 2024-05-02 06:52:40.000000 dcm-processor-1.1.3/dcm_processor/services/base/module/DicomAnonymizerService/CTP.jar
+-rw-rw-r--   0 giles     (1000) giles     (1000)    17869 2024-05-02 06:52:40.000000 dcm-processor-1.1.3/dcm_processor/services/base/module/DicomAnonymizerService/DAT.jar
+-rw-rw-r--   0 giles     (1000) giles     (1000)      526 2024-05-02 06:52:40.000000 dcm-processor-1.1.3/dcm_processor/services/base/module/DicomAnonymizerService/__init__.py
+-rw-rw-r--   0 giles     (1000) giles     (1000)     1590 2024-05-02 06:52:40.000000 dcm-processor-1.1.3/dcm_processor/services/base/module/DicomAnonymizerService/anonymize.py
+-rw-rw-r--   0 giles     (1000) giles     (1000)    69564 2024-05-02 06:52:40.000000 dcm-processor-1.1.3/dcm_processor/services/base/module/DicomAnonymizerService/clibwrapper_jiio-1.2-pre-dr-b04.jar
+drwxrwxr-x   0 giles     (1000) giles     (1000)        0 2024-05-02 07:15:41.019697 dcm-processor-1.1.3/dcm_processor/services/base/module/DicomAnonymizerService/config/
+-rw-rw-r--   0 giles     (1000) giles     (1000)    59932 2024-05-02 06:52:40.000000 dcm-processor-1.1.3/dcm_processor/services/base/module/DicomAnonymizerService/config/dicom-anonymizer.script
+-rw-rw-r--   0 giles     (1000) giles     (1000)      248 2024-05-02 06:52:40.000000 dcm-processor-1.1.3/dcm_processor/services/base/module/DicomAnonymizerService/config/hash_table.csv
+-rw-rw-r--   0 giles     (1000) giles     (1000)       86 2024-05-02 06:52:40.000000 dcm-processor-1.1.3/dcm_processor/services/base/module/DicomAnonymizerService/config/psudonyms.csv
+-rw-rw-r--   0 giles     (1000) giles     (1000)    10424 2024-05-02 06:52:40.000000 dcm-processor-1.1.3/dcm_processor/services/base/module/DicomAnonymizerService/dcm4che-imageio-rle-2.0.25.jar
+-rw-rw-r--   0 giles     (1000) giles     (1000)   863881 2024-05-02 06:52:40.000000 dcm-processor-1.1.3/dcm_processor/services/base/module/DicomAnonymizerService/dcm4che.jar
+-rw-rw-r--   0 giles     (1000) giles     (1000)     3479 2024-05-02 06:52:40.000000 dcm-processor-1.1.3/dcm_processor/services/base/module/DicomAnonymizerService/fhir_lib.py
+-rw-rw-r--   0 giles     (1000) giles     (1000)  1172845 2024-05-02 06:52:40.000000 dcm-processor-1.1.3/dcm_processor/services/base/module/DicomAnonymizerService/jai_imageio-1.2-pre-dr-b04.jar
+-rw-rw-r--   0 giles     (1000) giles     (1000)   391834 2024-05-02 06:52:40.000000 dcm-processor-1.1.3/dcm_processor/services/base/module/DicomAnonymizerService/log4j.jar
+-rw-rw-r--   0 giles     (1000) giles     (1000)    28241 2024-05-02 06:52:40.000000 dcm-processor-1.1.3/dcm_processor/services/base/module/DicomAnonymizerService/pixelmed_codec.jar
+-rw-rw-r--   0 giles     (1000) giles     (1000)   338969 2024-05-02 06:52:40.000000 dcm-processor-1.1.3/dcm_processor/services/base/module/DicomAnonymizerService/util.jar
+-rw-rw-r--   0 giles     (1000) giles     (1000)     1777 2024-05-02 06:52:40.000000 dcm-processor-1.1.3/dcm_processor/services/base/module/DicomAnonymizerService/utils.py
+-rw-rw-r--   0 giles     (1000) giles     (1000)       26 2024-05-02 06:52:40.000000 dcm-processor-1.1.3/dcm_processor/services/base/module/requirements.txt
+-rw-rw-r--   0 giles     (1000) giles     (1000)       72 2024-05-02 06:52:40.000000 dcm-processor-1.1.3/dcm_processor/services/base/module/script.sh
+drwxrwxr-x   0 giles     (1000) giles     (1000)        0 2024-05-02 07:15:41.019697 dcm-processor-1.1.3/dcm_processor/services/base/module/storageManager/
+-rw-rw-r--   0 giles     (1000) giles     (1000)       24 2024-05-02 06:52:40.000000 dcm-processor-1.1.3/dcm_processor/services/base/module/storageManager/__init__.py
+-rw-rw-r--   0 giles     (1000) giles     (1000)       95 2024-05-02 06:52:40.000000 dcm-processor-1.1.3/dcm_processor/services/base/module/storageManager/header_codes.json
+-rw-rw-r--   0 giles     (1000) giles     (1000)     6218 2024-05-02 06:52:40.000000 dcm-processor-1.1.3/dcm_processor/services/base/module/storageManager/lib.py
+-rw-rw-r--   0 giles     (1000) giles     (1000)    10622 2024-05-02 06:52:40.000000 dcm-processor-1.1.3/dcm_processor/services/base/module/storageManager/main.py
+drwxrwxr-x   0 giles     (1000) giles     (1000)        0 2024-05-02 07:15:41.019697 dcm-processor-1.1.3/dcm_processor/services/base/module/systemcleaner/
+-rw-rw-r--   0 giles     (1000) giles     (1000)       24 2024-05-02 06:52:40.000000 dcm-processor-1.1.3/dcm_processor/services/base/module/systemcleaner/__init__.py
+-rw-rw-r--   0 giles     (1000) giles     (1000)     3908 2024-05-02 06:52:40.000000 dcm-processor-1.1.3/dcm_processor/services/base/module/systemcleaner/main.py
+drwxrwxr-x   0 giles     (1000) giles     (1000)        0 2024-05-02 07:15:41.019697 dcm-processor-1.1.3/dcm_processor/services/base/registry/
+-rw-rw-r--   0 giles     (1000) giles     (1000)      491 2024-05-02 06:52:40.000000 dcm-processor-1.1.3/dcm_processor/services/base/registry/__init__.py
+drwxrwxr-x   0 giles     (1000) giles     (1000)        0 2024-05-02 07:15:41.019697 dcm-processor-1.1.3/dcm_processor/services/dcm2nii/
+drwxrwxr-x   0 giles     (1000) giles     (1000)        0 2024-05-02 07:15:41.023697 dcm-processor-1.1.3/dcm_processor/services/dcm2nii/module/
+-rw-rw-r--   0 giles     (1000) giles     (1000)     4030 2024-05-02 06:52:40.000000 dcm-processor-1.1.3/dcm_processor/services/dcm2nii/module/__init__.py
+-rw-rw-r--   0 giles     (1000) giles     (1000)  1948128 2024-05-02 06:52:40.000000 dcm-processor-1.1.3/dcm_processor/services/dcm2nii/module/dcm2niix
+-rw-rw-r--   0 giles     (1000) giles     (1000)      406 2024-05-02 06:52:40.000000 dcm-processor-1.1.3/dcm_processor/services/dcm2nii/module/lib.py
+drwxrwxr-x   0 giles     (1000) giles     (1000)        0 2024-05-02 07:15:41.023697 dcm-processor-1.1.3/dcm_processor/services/dcm2nii/registry/
+-rw-rw-r--   0 giles     (1000) giles     (1000)     1013 2024-05-02 06:52:40.000000 dcm-processor-1.1.3/dcm_processor/services/dcm2nii/registry/__init__.py
+-rw-rw-r--   0 giles     (1000) giles     (1000)      288 2024-05-02 06:52:40.000000 dcm-processor-1.1.3/dcm_processor/services/dcm2nii/registry/settings.json
+-rw-rw-r--   0 giles     (1000) giles     (1000)     6682 2024-05-02 06:52:40.000000 dcm-processor-1.1.3/dcm_processor/worker.py
+drwxrwxr-x   0 giles     (1000) giles     (1000)        0 2024-05-02 07:15:41.023697 dcm-processor-1.1.3/dcm_processor.egg-info/
+-rw-r--r--   0 giles     (1000) giles     (1000)     6486 2024-05-02 07:15:40.000000 dcm-processor-1.1.3/dcm_processor.egg-info/PKG-INFO
+-rw-rw-r--   0 giles     (1000) giles     (1000)     2368 2024-05-02 07:15:41.000000 dcm-processor-1.1.3/dcm_processor.egg-info/SOURCES.txt
+-rw-rw-r--   0 giles     (1000) giles     (1000)        1 2024-05-02 07:15:40.000000 dcm-processor-1.1.3/dcm_processor.egg-info/dependency_links.txt
+-rw-rw-r--   0 giles     (1000) giles     (1000)       53 2024-05-02 07:15:40.000000 dcm-processor-1.1.3/dcm_processor.egg-info/entry_points.txt
+-rw-rw-r--   0 giles     (1000) giles     (1000)       61 2024-05-02 07:15:40.000000 dcm-processor-1.1.3/dcm_processor.egg-info/requires.txt
+-rw-rw-r--   0 giles     (1000) giles     (1000)       14 2024-05-02 07:15:40.000000 dcm-processor-1.1.3/dcm_processor.egg-info/top_level.txt
+-rw-rw-r--   0 giles     (1000) giles     (1000)       89 2024-05-02 06:52:40.000000 dcm-processor-1.1.3/pyproject.toml
+-rw-rw-r--   0 giles     (1000) giles     (1000)      964 2024-05-02 07:15:41.023697 dcm-processor-1.1.3/setup.cfg
+-rw-rw-r--   0 giles     (1000) giles     (1000)      109 2024-05-02 06:52:40.000000 dcm-processor-1.1.3/setup.py
```

### Comparing `dcm-processor-1.1.2/LICENSE` & `dcm-processor-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.1.2/PKG-INFO` & `dcm-processor-1.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 Metadata-Version: 2.1
 Name: dcm-processor
-Version: 1.1.2
+Version: 1.1.3
 Summary: A Command line tool for the dicom processor library
 Home-page: https://github.com/giesekow/dcm-processor-cli
 Author: Giles Tetteh
 Author-email: giles.tetteh@tum.de
 Keywords: orthanc,dicom,worker,processor,translation,medical
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: python-dotenv
+Requires-Dist: inquirer
+Requires-Dist: PyYAML
+Requires-Dist: GitPython
+Requires-Dist: ruamel_yaml
+Requires-Dist: requests
 
 # DCM PROCESSOR
 A dicom processing library setup with docker containers.
 
 ## DEPENDENCIES
 1. Python (version  >= 3.6)
 1. Docker
```

### Comparing `dcm-processor-1.1.2/README.md` & `dcm-processor-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.1.2/dcm_processor/argparser.py` & `dcm-processor-1.1.3/dcm_processor/argparser.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.1.2/dcm_processor/files.py` & `dcm-processor-1.1.3/dcm_processor/files.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.1.2/dcm_processor/script.py` & `dcm-processor-1.1.3/dcm_processor/script.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.1.2/dcm_processor/services/base/module/DicomAnonymizerService/CTP.jar` & `dcm-processor-1.1.3/dcm_processor/services/base/module/DicomAnonymizerService/CTP.jar`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.1.2/dcm_processor/services/base/module/DicomAnonymizerService/DAT.jar` & `dcm-processor-1.1.3/dcm_processor/services/base/module/DicomAnonymizerService/DAT.jar`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.1.2/dcm_processor/services/base/module/DicomAnonymizerService/__init__.py` & `dcm-processor-1.1.3/dcm_processor/services/base/module/DicomAnonymizerService/__init__.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.1.2/dcm_processor/services/base/module/DicomAnonymizerService/anonymize.py` & `dcm-processor-1.1.3/dcm_processor/services/base/module/DicomAnonymizerService/anonymize.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.1.2/dcm_processor/services/base/module/DicomAnonymizerService/clibwrapper_jiio-1.2-pre-dr-b04.jar` & `dcm-processor-1.1.3/dcm_processor/services/base/module/DicomAnonymizerService/clibwrapper_jiio-1.2-pre-dr-b04.jar`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.1.2/dcm_processor/services/base/module/DicomAnonymizerService/config/dicom-anonymizer.script` & `dcm-processor-1.1.3/dcm_processor/services/base/module/DicomAnonymizerService/config/dicom-anonymizer.script`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.1.2/dcm_processor/services/base/module/DicomAnonymizerService/dcm4che-imageio-rle-2.0.25.jar` & `dcm-processor-1.1.3/dcm_processor/services/base/module/DicomAnonymizerService/dcm4che-imageio-rle-2.0.25.jar`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.1.2/dcm_processor/services/base/module/DicomAnonymizerService/dcm4che.jar` & `dcm-processor-1.1.3/dcm_processor/services/base/module/DicomAnonymizerService/dcm4che.jar`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.1.2/dcm_processor/services/base/module/DicomAnonymizerService/fhir_lib.py` & `dcm-processor-1.1.3/dcm_processor/services/base/module/DicomAnonymizerService/fhir_lib.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.1.2/dcm_processor/services/base/module/DicomAnonymizerService/jai_imageio-1.2-pre-dr-b04.jar` & `dcm-processor-1.1.3/dcm_processor/services/base/module/DicomAnonymizerService/jai_imageio-1.2-pre-dr-b04.jar`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.1.2/dcm_processor/services/base/module/DicomAnonymizerService/log4j.jar` & `dcm-processor-1.1.3/dcm_processor/services/base/module/DicomAnonymizerService/log4j.jar`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.1.2/dcm_processor/services/base/module/DicomAnonymizerService/pixelmed_codec.jar` & `dcm-processor-1.1.3/dcm_processor/services/base/module/DicomAnonymizerService/pixelmed_codec.jar`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.1.2/dcm_processor/services/base/module/DicomAnonymizerService/util.jar` & `dcm-processor-1.1.3/dcm_processor/services/base/module/DicomAnonymizerService/util.jar`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.1.2/dcm_processor/services/base/module/DicomAnonymizerService/utils.py` & `dcm-processor-1.1.3/dcm_processor/services/base/module/DicomAnonymizerService/utils.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.1.2/dcm_processor/services/base/module/storageManager/lib.py` & `dcm-processor-1.1.3/dcm_processor/services/base/module/storageManager/lib.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.1.2/dcm_processor/services/base/module/storageManager/main.py` & `dcm-processor-1.1.3/dcm_processor/services/base/module/storageManager/main.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.1.2/dcm_processor/services/base/module/systemcleaner/main.py` & `dcm-processor-1.1.3/dcm_processor/services/base/module/systemcleaner/main.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.1.2/dcm_processor/services/dcm2nii/module/__init__.py` & `dcm-processor-1.1.3/dcm_processor/services/dcm2nii/module/__init__.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.1.2/dcm_processor/services/dcm2nii/module/dcm2niix` & `dcm-processor-1.1.3/dcm_processor/services/dcm2nii/module/dcm2niix`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.1.2/dcm_processor/services/dcm2nii/registry/__init__.py` & `dcm-processor-1.1.3/dcm_processor/services/dcm2nii/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.1.2/dcm_processor/worker.py` & `dcm-processor-1.1.3/dcm_processor/worker.py`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.1.2/dcm_processor.egg-info/PKG-INFO` & `dcm-processor-1.1.3/dcm_processor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 Metadata-Version: 2.1
 Name: dcm-processor
-Version: 1.1.2
+Version: 1.1.3
 Summary: A Command line tool for the dicom processor library
 Home-page: https://github.com/giesekow/dcm-processor-cli
 Author: Giles Tetteh
 Author-email: giles.tetteh@tum.de
 Keywords: orthanc,dicom,worker,processor,translation,medical
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: python-dotenv
+Requires-Dist: inquirer
+Requires-Dist: PyYAML
+Requires-Dist: GitPython
+Requires-Dist: ruamel_yaml
+Requires-Dist: requests
 
 # DCM PROCESSOR
 A dicom processing library setup with docker containers.
 
 ## DEPENDENCIES
 1. Python (version  >= 3.6)
 1. Docker
```

### Comparing `dcm-processor-1.1.2/dcm_processor.egg-info/SOURCES.txt` & `dcm-processor-1.1.3/dcm_processor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dcm-processor-1.1.2/setup.cfg` & `dcm-processor-1.1.3/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dcm-processor
-version = 1.1.2
+version = 1.1.3
 author = Giles Tetteh
 author_email = giles.tetteh@tum.de
 description = A Command line tool for the dicom processor library
 url = https://github.com/giesekow/dcm-processor-cli
 long_description = file: README.md
 long_description_content_type = text/markdown
 license_files = LICENSE
@@ -22,15 +22,14 @@
 
 [options]
 packages = dcm_processor
 include_package_data = True
 install_requires = 
 	python-dotenv
 	inquirer
-	docker-compose
 	PyYAML
 	GitPython
 	ruamel_yaml
 	requests
 
 [options.entry_points]
 console_scripts =
```

