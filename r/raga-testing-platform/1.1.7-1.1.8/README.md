# Comparing `tmp/raga-testing-platform-1.1.7.tar.gz` & `tmp/raga-testing-platform-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raga-testing-platform-1.1.7.tar", last modified: Fri Nov 10 09:34:03 2023, max compression
+gzip compressed data, was "raga-testing-platform-1.1.8.tar", last modified: Fri Nov 10 11:35:30 2023, max compression
```

## Comparing `raga-testing-platform-1.1.7.tar` & `raga-testing-platform-1.1.8.tar`

### file list

```diff
@@ -1,106 +1,107 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-10 09:34:03.480201 raga-testing-platform-1.1.7/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6148 2023-11-06 08:07:34.000000 raga-testing-platform-1.1.7/.DS_Store
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-10 09:34:03.472201 raga-testing-platform-1.1.7/.github/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       78 2023-10-10 07:01:37.000000 raga-testing-platform-1.1.7/.github/CODEOWNERS
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-10 09:34:03.472201 raga-testing-platform-1.1.7/.github/workflows/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      813 2023-10-10 07:01:37.000000 raga-testing-platform-1.1.7/.github/workflows/build.yml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3164 2023-11-06 08:07:34.000000 raga-testing-platform-1.1.7/.gitignore
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-10 09:34:03.472201 raga-testing-platform-1.1.7/.idea/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       47 2023-10-10 07:01:37.000000 raga-testing-platform-1.1.7/.idea/.gitignore
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-10 09:34:03.472201 raga-testing-platform-1.1.7/.idea/inspectionProfiles/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      174 2023-10-10 07:01:37.000000 raga-testing-platform-1.1.7/.idea/inspectionProfiles/profiles_settings.xml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      312 2023-10-10 07:01:37.000000 raga-testing-platform-1.1.7/.idea/modules.xml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      167 2023-10-10 07:01:37.000000 raga-testing-platform-1.1.7/.idea/vcs.xml
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-10 09:34:03.472201 raga-testing-platform-1.1.7/.vscode/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      495 2023-10-10 07:01:37.000000 raga-testing-platform-1.1.7/.vscode/launch.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      148 2023-10-10 07:01:37.000000 raga-testing-platform-1.1.7/.vscode/settings.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1073 2023-10-10 07:01:37.000000 raga-testing-platform-1.1.7/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      273 2023-11-02 07:58:54.000000 raga-testing-platform-1.1.7/Makefile
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3259 2023-11-10 09:34:03.480201 raga-testing-platform-1.1.7/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2408 2023-10-10 07:01:37.000000 raga-testing-platform-1.1.7/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1025 2023-11-10 09:33:40.000000 raga-testing-platform-1.1.7/pyproject.toml
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-10 09:34:03.476201 raga-testing-platform-1.1.7/raga/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1180 2023-10-19 08:19:33.000000 raga-testing-platform-1.1.7/raga/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17487 2023-11-10 09:33:40.000000 raga-testing-platform-1.1.7/raga/_tests.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2287 2023-11-09 12:46:14.000000 raga-testing-platform-1.1.7/raga/constants.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16269 2023-11-09 12:47:47.000000 raga-testing-platform-1.1.7/raga/dataset.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      233 2023-11-01 10:18:58.000000 raga-testing-platform-1.1.7/raga/dataset_creds.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-10 09:34:03.476201 raga-testing-platform-1.1.7/raga/docs/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       82 2023-10-10 07:01:37.000000 raga-testing-platform-1.1.7/raga/docs/conf.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      160 2023-10-10 07:01:37.000000 raga-testing-platform-1.1.7/raga/docs/index.rst
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-10 09:34:03.476201 raga-testing-platform-1.1.7/raga/examples/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12292 2023-10-19 10:12:34.000000 raga-testing-platform-1.1.7/raga/examples/.DS_Store
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1871 2023-10-30 12:46:07.000000 raga-testing-platform-1.1.7/raga/examples/ab_event_unlabelled.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5838 2023-11-03 09:00:05.000000 raga-testing-platform-1.1.7/raga/examples/data_drift.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1453 2023-10-10 07:01:37.000000 raga-testing-platform-1.1.7/raga/examples/failure_mode_analysis_image_classification.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3135 2023-10-12 08:00:55.000000 raga-testing-platform-1.1.7/raga/examples/failure_mode_analysis_object_detection.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1819 2023-10-16 13:44:06.000000 raga-testing-platform-1.1.7/raga/examples/failure_mode_analysis_semantic_segmentation.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1304 2023-10-10 07:13:50.000000 raga-testing-platform-1.1.7/raga/examples/labelling_quality_image_classification.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1018 2023-10-10 07:13:50.000000 raga-testing-platform-1.1.7/raga/examples/labelling_quality_semantic_segment.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4282 2023-11-06 13:23:49.000000 raga-testing-platform-1.1.7/raga/examples/lm_dataloader.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17370 2023-11-04 09:31:35.000000 raga-testing-platform-1.1.7/raga/examples/lm_event_loader_failure_mode_analysis_object_detection-2.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17247 2023-11-06 11:46:47.000000 raga-testing-platform-1.1.7/raga/examples/lm_event_loader_failure_mode_analysis_object_detection.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3905 2023-10-10 07:13:50.000000 raga-testing-platform-1.1.7/raga/examples/lm_image_loader_failure_mode_analysis_object_detection-copy.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6809 2023-11-04 09:31:54.000000 raga-testing-platform-1.1.7/raga/examples/lm_image_loader_failure_mode_analysis_object_detection.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3979 2023-11-06 11:25:21.000000 raga-testing-platform-1.1.7/raga/examples/lm_inference_generator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2312 2023-11-06 07:49:51.000000 raga-testing-platform-1.1.7/raga/examples/lm_model_upload.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4804 2023-11-04 09:32:05.000000 raga-testing-platform-1.1.7/raga/examples/lm_video_loader_failure_mode_analysis_object_detection.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3222 2023-11-04 09:39:30.000000 raga-testing-platform-1.1.7/raga/examples/loader_ai_dash_object_detection.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4026 2023-11-04 09:32:14.000000 raga-testing-platform-1.1.7/raga/examples/loader_failure_mode_analysis_image_classification.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4616 2023-11-04 09:32:19.000000 raga-testing-platform-1.1.7/raga/examples/loader_failure_mode_analysis_object_detection.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3484 2023-11-08 04:25:01.000000 raga-testing-platform-1.1.7/raga/examples/loader_failure_mode_analysis_semantic_segmentation.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2682 2023-11-06 11:30:36.000000 raga-testing-platform-1.1.7/raga/examples/loader_failure_mode_analysis_super_resolution.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5382 2023-11-04 10:50:12.000000 raga-testing-platform-1.1.7/raga/examples/loader_honeywell_data.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3674 2023-11-04 09:28:00.000000 raga-testing-platform-1.1.7/raga/examples/loader_labeling_quality_image_classification.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-10-10 07:01:37.000000 raga-testing-platform-1.1.7/raga/examples/loader_labeling_quality_object_detection.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4005 2023-11-08 12:01:37.000000 raga-testing-platform-1.1.7/raga/examples/loader_labeling_quality_semantic_segmentation.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3960 2023-11-06 12:48:00.000000 raga-testing-platform-1.1.7/raga/examples/loader_labeling_quality_semantic_segmentation_data_drift.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3219 2023-11-04 10:07:44.000000 raga-testing-platform-1.1.7/raga/examples/loader_labeling_quality_semantic_segmentation_tree_health.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4460 2023-11-06 12:06:53.000000 raga-testing-platform-1.1.7/raga/examples/loader_labeling_quality_semantic_segmentation_v2.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4327 2023-11-04 09:32:44.000000 raga-testing-platform-1.1.7/raga/examples/loader_labeling_quality_semantic_segmentation_v3.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4311 2023-11-09 05:52:46.000000 raga-testing-platform-1.1.7/raga/examples/loader_labeling_quality_semantic_segmentation_v4.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4069 2023-11-09 10:36:24.000000 raga-testing-platform-1.1.7/raga/examples/loader_satsure_inference_oct_2023.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3323 2023-11-09 12:54:47.000000 raga-testing-platform-1.1.7/raga/examples/loader_satsure_new_dat_nov_2023.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3182 2023-11-08 10:41:47.000000 raga-testing-platform-1.1.7/raga/examples/loader_satsure_new_dat_nov_2023_100img.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1179 2023-11-09 13:57:13.000000 raga-testing-platform-1.1.7/raga/examples/loader_satsure_new_dat_nov_2023_using_ready_ds.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2134 2023-11-08 08:54:37.000000 raga-testing-platform-1.1.7/raga/examples/model_distribution-mistakescore.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1957 2023-11-08 07:25:59.000000 raga-testing-platform-1.1.7/raga/examples/model_distribution-v2.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1832 2023-11-06 06:28:12.000000 raga-testing-platform-1.1.7/raga/examples/model_distribution.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3383 2023-11-10 09:33:40.000000 raga-testing-platform-1.1.7/raga/examples/nano_dataset_upload_missing_values.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3775 2023-11-10 09:33:40.000000 raga-testing-platform-1.1.7/raga/examples/nano_dataset_upload_outlier.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      920 2023-11-10 09:33:40.000000 raga-testing-platform-1.1.7/raga/examples/ocr_missing_value_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      898 2023-11-10 09:33:40.000000 raga-testing-platform-1.1.7/raga/examples/ocr_outlier_detection_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      175 2023-11-02 06:18:57.000000 raga-testing-platform-1.1.7/raga/examples/poc.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1742 2023-10-10 07:01:37.000000 raga-testing-platform-1.1.7/raga/examples/sts_test.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      198 2023-10-10 07:01:37.000000 raga-testing-platform-1.1.7/raga/exception.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      565 2023-10-17 07:19:20.000000 raga-testing-platform-1.1.7/raga/filters.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5787 2023-11-09 10:09:37.000000 raga-testing-platform-1.1.7/raga/lightmetrics.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8687 2023-11-09 12:09:03.000000 raga-testing-platform-1.1.7/raga/model_executor_factory.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4559 2023-11-03 07:05:04.000000 raga-testing-platform-1.1.7/raga/post_deployment_checks.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    21149 2023-11-10 09:33:40.000000 raga-testing-platform-1.1.7/raga/raga_schema.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8340 2023-11-10 09:33:40.000000 raga-testing-platform-1.1.7/raga/test_session.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-10 09:34:03.480201 raga-testing-platform-1.1.7/raga/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       51 2023-10-10 07:01:37.000000 raga-testing-platform-1.1.7/raga/tests/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11040 2023-10-10 07:01:37.000000 raga-testing-platform-1.1.7/raga/tests/test_dataset.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2147 2023-10-10 07:01:37.000000 raga-testing-platform-1.1.7/raga/tests/test_dataset_util.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5143 2023-10-10 07:01:37.000000 raga-testing-platform-1.1.7/raga/tests/test_http_client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17083 2023-10-10 07:01:37.000000 raga-testing-platform-1.1.7/raga/tests/test_test_session.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7635 2023-10-10 07:01:37.000000 raga-testing-platform-1.1.7/raga/tests/test_tests.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-10 09:34:03.480201 raga-testing-platform-1.1.7/raga/utils/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      108 2023-10-10 07:01:37.000000 raga-testing-platform-1.1.7/raga/utils/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5501 2023-11-09 12:47:28.000000 raga-testing-platform-1.1.7/raga/utils/dataset_util.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      789 2023-10-10 07:01:37.000000 raga-testing-platform-1.1.7/raga/utils/file.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6994 2023-11-09 10:09:37.000000 raga-testing-platform-1.1.7/raga/utils/http_client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4499 2023-11-02 06:38:48.000000 raga-testing-platform-1.1.7/raga/utils/raga_config_reader.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-10 09:34:03.480201 raga-testing-platform-1.1.7/raga/validators/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      860 2023-10-10 07:01:37.000000 raga-testing-platform-1.1.7/raga/validators/dataset_creds_validations.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1744 2023-10-10 07:01:37.000000 raga-testing-platform-1.1.7/raga/validators/dataset_validations.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1684 2023-10-10 07:01:37.000000 raga-testing-platform-1.1.7/raga/validators/test_session_validation.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-10 09:34:03.480201 raga-testing-platform-1.1.7/raga_testing_platform.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3259 2023-11-10 09:34:03.000000 raga-testing-platform-1.1.7/raga_testing_platform.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3501 2023-11-10 09:34:03.000000 raga-testing-platform-1.1.7/raga_testing_platform.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-11-10 09:34:03.000000 raga-testing-platform-1.1.7/raga_testing_platform.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-11-10 09:34:03.000000 raga-testing-platform-1.1.7/raga_testing_platform.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        5 2023-11-10 09:34:03.000000 raga-testing-platform-1.1.7/raga_testing_platform.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-11-10 09:34:03.480201 raga-testing-platform-1.1.7/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       47 2023-10-10 07:01:37.000000 raga-testing-platform-1.1.7/sonar-project.properties
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-10 11:35:30.414739 raga-testing-platform-1.1.8/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6148 2023-11-06 08:07:34.000000 raga-testing-platform-1.1.8/.DS_Store
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-10 11:35:30.410739 raga-testing-platform-1.1.8/.github/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       78 2023-10-10 07:01:37.000000 raga-testing-platform-1.1.8/.github/CODEOWNERS
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-10 11:35:30.410739 raga-testing-platform-1.1.8/.github/workflows/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      813 2023-10-10 07:01:37.000000 raga-testing-platform-1.1.8/.github/workflows/build.yml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3164 2023-11-06 08:07:34.000000 raga-testing-platform-1.1.8/.gitignore
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-10 11:35:30.410739 raga-testing-platform-1.1.8/.idea/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       47 2023-10-10 07:01:37.000000 raga-testing-platform-1.1.8/.idea/.gitignore
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-10 11:35:30.410739 raga-testing-platform-1.1.8/.idea/inspectionProfiles/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      174 2023-10-10 07:01:37.000000 raga-testing-platform-1.1.8/.idea/inspectionProfiles/profiles_settings.xml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      312 2023-10-10 07:01:37.000000 raga-testing-platform-1.1.8/.idea/modules.xml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      167 2023-10-10 07:01:37.000000 raga-testing-platform-1.1.8/.idea/vcs.xml
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-10 11:35:30.410739 raga-testing-platform-1.1.8/.vscode/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      495 2023-10-10 07:01:37.000000 raga-testing-platform-1.1.8/.vscode/launch.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      148 2023-10-10 07:01:37.000000 raga-testing-platform-1.1.8/.vscode/settings.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1073 2023-10-10 07:01:37.000000 raga-testing-platform-1.1.8/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      273 2023-11-02 07:58:54.000000 raga-testing-platform-1.1.8/Makefile
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3259 2023-11-10 11:35:30.414739 raga-testing-platform-1.1.8/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2408 2023-10-10 07:01:37.000000 raga-testing-platform-1.1.8/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1025 2023-11-10 11:31:01.000000 raga-testing-platform-1.1.8/pyproject.toml
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-10 11:35:30.410739 raga-testing-platform-1.1.8/raga/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1180 2023-10-19 08:19:33.000000 raga-testing-platform-1.1.8/raga/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17487 2023-11-10 09:33:40.000000 raga-testing-platform-1.1.8/raga/_tests.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2287 2023-11-09 12:46:14.000000 raga-testing-platform-1.1.8/raga/constants.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16956 2023-11-10 10:58:47.000000 raga-testing-platform-1.1.8/raga/dataset.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      233 2023-11-01 10:18:58.000000 raga-testing-platform-1.1.8/raga/dataset_creds.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-10 11:35:30.410739 raga-testing-platform-1.1.8/raga/docs/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       82 2023-10-10 07:01:37.000000 raga-testing-platform-1.1.8/raga/docs/conf.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      160 2023-10-10 07:01:37.000000 raga-testing-platform-1.1.8/raga/docs/index.rst
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-10 11:35:30.414739 raga-testing-platform-1.1.8/raga/examples/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12292 2023-10-19 10:12:34.000000 raga-testing-platform-1.1.8/raga/examples/.DS_Store
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1871 2023-10-30 12:46:07.000000 raga-testing-platform-1.1.8/raga/examples/ab_event_unlabelled.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5838 2023-11-03 09:00:05.000000 raga-testing-platform-1.1.8/raga/examples/data_drift.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1453 2023-10-10 07:01:37.000000 raga-testing-platform-1.1.8/raga/examples/failure_mode_analysis_image_classification.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3135 2023-10-12 08:00:55.000000 raga-testing-platform-1.1.8/raga/examples/failure_mode_analysis_object_detection.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1819 2023-10-16 13:44:06.000000 raga-testing-platform-1.1.8/raga/examples/failure_mode_analysis_semantic_segmentation.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1304 2023-10-10 07:13:50.000000 raga-testing-platform-1.1.8/raga/examples/labelling_quality_image_classification.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1018 2023-10-10 07:13:50.000000 raga-testing-platform-1.1.8/raga/examples/labelling_quality_semantic_segment.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4283 2023-11-10 11:01:45.000000 raga-testing-platform-1.1.8/raga/examples/lm_dataloader.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17370 2023-11-04 09:31:35.000000 raga-testing-platform-1.1.8/raga/examples/lm_event_loader_failure_mode_analysis_object_detection-2.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17247 2023-11-06 11:46:47.000000 raga-testing-platform-1.1.8/raga/examples/lm_event_loader_failure_mode_analysis_object_detection.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3905 2023-10-10 07:13:50.000000 raga-testing-platform-1.1.8/raga/examples/lm_image_loader_failure_mode_analysis_object_detection-copy.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6809 2023-11-04 09:31:54.000000 raga-testing-platform-1.1.8/raga/examples/lm_image_loader_failure_mode_analysis_object_detection.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3979 2023-11-06 11:25:21.000000 raga-testing-platform-1.1.8/raga/examples/lm_inference_generator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2312 2023-11-06 07:49:51.000000 raga-testing-platform-1.1.8/raga/examples/lm_model_upload.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4804 2023-11-04 09:32:05.000000 raga-testing-platform-1.1.8/raga/examples/lm_video_loader_failure_mode_analysis_object_detection.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3222 2023-11-04 09:39:30.000000 raga-testing-platform-1.1.8/raga/examples/loader_ai_dash_object_detection.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4026 2023-11-04 09:32:14.000000 raga-testing-platform-1.1.8/raga/examples/loader_failure_mode_analysis_image_classification.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4616 2023-11-04 09:32:19.000000 raga-testing-platform-1.1.8/raga/examples/loader_failure_mode_analysis_object_detection.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3484 2023-11-08 04:25:01.000000 raga-testing-platform-1.1.8/raga/examples/loader_failure_mode_analysis_semantic_segmentation.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2682 2023-11-06 11:30:36.000000 raga-testing-platform-1.1.8/raga/examples/loader_failure_mode_analysis_super_resolution.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5382 2023-11-04 10:50:12.000000 raga-testing-platform-1.1.8/raga/examples/loader_honeywell_data.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3674 2023-11-04 09:28:00.000000 raga-testing-platform-1.1.8/raga/examples/loader_labeling_quality_image_classification.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-10-10 07:01:37.000000 raga-testing-platform-1.1.8/raga/examples/loader_labeling_quality_object_detection.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4005 2023-11-08 12:01:37.000000 raga-testing-platform-1.1.8/raga/examples/loader_labeling_quality_semantic_segmentation.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3960 2023-11-06 12:48:00.000000 raga-testing-platform-1.1.8/raga/examples/loader_labeling_quality_semantic_segmentation_data_drift.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3219 2023-11-04 10:07:44.000000 raga-testing-platform-1.1.8/raga/examples/loader_labeling_quality_semantic_segmentation_tree_health.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4460 2023-11-06 12:06:53.000000 raga-testing-platform-1.1.8/raga/examples/loader_labeling_quality_semantic_segmentation_v2.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4327 2023-11-04 09:32:44.000000 raga-testing-platform-1.1.8/raga/examples/loader_labeling_quality_semantic_segmentation_v3.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4311 2023-11-09 05:52:46.000000 raga-testing-platform-1.1.8/raga/examples/loader_labeling_quality_semantic_segmentation_v4.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4069 2023-11-09 10:36:24.000000 raga-testing-platform-1.1.8/raga/examples/loader_satsure_inference_oct_2023.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3323 2023-11-09 12:54:47.000000 raga-testing-platform-1.1.8/raga/examples/loader_satsure_new_dat_nov_2023.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3182 2023-11-08 10:41:47.000000 raga-testing-platform-1.1.8/raga/examples/loader_satsure_new_dat_nov_2023_100img.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1183 2023-11-10 10:27:05.000000 raga-testing-platform-1.1.8/raga/examples/loader_satsure_new_dat_nov_2023_using_ready_ds.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      388 2023-11-10 11:33:54.000000 raga-testing-platform-1.1.8/raga/examples/model-upload.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2134 2023-11-08 08:54:37.000000 raga-testing-platform-1.1.8/raga/examples/model_distribution-mistakescore.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1957 2023-11-08 07:25:59.000000 raga-testing-platform-1.1.8/raga/examples/model_distribution-v2.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1832 2023-11-06 06:28:12.000000 raga-testing-platform-1.1.8/raga/examples/model_distribution.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3383 2023-11-10 09:33:40.000000 raga-testing-platform-1.1.8/raga/examples/nano_dataset_upload_missing_values.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3775 2023-11-10 09:33:40.000000 raga-testing-platform-1.1.8/raga/examples/nano_dataset_upload_outlier.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      920 2023-11-10 09:33:40.000000 raga-testing-platform-1.1.8/raga/examples/ocr_missing_value_test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      898 2023-11-10 09:33:40.000000 raga-testing-platform-1.1.8/raga/examples/ocr_outlier_detection_test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      175 2023-11-02 06:18:57.000000 raga-testing-platform-1.1.8/raga/examples/poc.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1742 2023-10-10 07:01:37.000000 raga-testing-platform-1.1.8/raga/examples/sts_test.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      198 2023-10-10 07:01:37.000000 raga-testing-platform-1.1.8/raga/exception.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      565 2023-10-17 07:19:20.000000 raga-testing-platform-1.1.8/raga/filters.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7507 2023-11-10 11:33:54.000000 raga-testing-platform-1.1.8/raga/lightmetrics.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8687 2023-11-09 12:09:03.000000 raga-testing-platform-1.1.8/raga/model_executor_factory.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4559 2023-11-03 07:05:04.000000 raga-testing-platform-1.1.8/raga/post_deployment_checks.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    21149 2023-11-10 09:33:40.000000 raga-testing-platform-1.1.8/raga/raga_schema.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8340 2023-11-10 09:33:40.000000 raga-testing-platform-1.1.8/raga/test_session.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-10 11:35:30.414739 raga-testing-platform-1.1.8/raga/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       51 2023-10-10 07:01:37.000000 raga-testing-platform-1.1.8/raga/tests/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11040 2023-10-10 07:01:37.000000 raga-testing-platform-1.1.8/raga/tests/test_dataset.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2147 2023-10-10 07:01:37.000000 raga-testing-platform-1.1.8/raga/tests/test_dataset_util.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5143 2023-10-10 07:01:37.000000 raga-testing-platform-1.1.8/raga/tests/test_http_client.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17083 2023-10-10 07:01:37.000000 raga-testing-platform-1.1.8/raga/tests/test_test_session.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7635 2023-10-10 07:01:37.000000 raga-testing-platform-1.1.8/raga/tests/test_tests.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-10 11:35:30.414739 raga-testing-platform-1.1.8/raga/utils/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      108 2023-10-10 07:01:37.000000 raga-testing-platform-1.1.8/raga/utils/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5501 2023-11-09 12:47:28.000000 raga-testing-platform-1.1.8/raga/utils/dataset_util.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      789 2023-10-10 07:01:37.000000 raga-testing-platform-1.1.8/raga/utils/file.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6994 2023-11-09 10:09:37.000000 raga-testing-platform-1.1.8/raga/utils/http_client.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4499 2023-11-02 06:38:48.000000 raga-testing-platform-1.1.8/raga/utils/raga_config_reader.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-10 11:35:30.414739 raga-testing-platform-1.1.8/raga/validators/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      860 2023-10-10 07:01:37.000000 raga-testing-platform-1.1.8/raga/validators/dataset_creds_validations.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1744 2023-10-10 07:01:37.000000 raga-testing-platform-1.1.8/raga/validators/dataset_validations.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1684 2023-10-10 07:01:37.000000 raga-testing-platform-1.1.8/raga/validators/test_session_validation.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-10 11:35:30.414739 raga-testing-platform-1.1.8/raga_testing_platform.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3259 2023-11-10 11:35:30.000000 raga-testing-platform-1.1.8/raga_testing_platform.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3531 2023-11-10 11:35:30.000000 raga-testing-platform-1.1.8/raga_testing_platform.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-11-10 11:35:30.000000 raga-testing-platform-1.1.8/raga_testing_platform.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-11-10 11:35:30.000000 raga-testing-platform-1.1.8/raga_testing_platform.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        5 2023-11-10 11:35:30.000000 raga-testing-platform-1.1.8/raga_testing_platform.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-11-10 11:35:30.414739 raga-testing-platform-1.1.8/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       47 2023-10-10 07:01:37.000000 raga-testing-platform-1.1.8/sonar-project.properties
```

### Comparing `raga-testing-platform-1.1.7/.DS_Store` & `raga-testing-platform-1.1.8/.DS_Store`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.1.7/.github/workflows/build.yml` & `raga-testing-platform-1.1.8/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.1.7/.gitignore` & `raga-testing-platform-1.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.1.7/LICENSE` & `raga-testing-platform-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.1.7/PKG-INFO` & `raga-testing-platform-1.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raga-testing-platform
-Version: 1.1.7
+Version: 1.1.8
 Summary: Short description or overview of the raga package.
 Author-email: Raga AI <support@ragaai.com>
 Maintainer-email: Raga AI <support@ragaai.com>
 Project-URL: Homepage, https://github.com/whoosh-labs/testing-platform-python-client
 Project-URL: Bug Tracker, https://github.com/whoosh-labs/testing-platform-python-client/issues
 Keywords: testing-platform,raga-testing-platform,model-testing,AB_testing
 Classifier: Programming Language :: Python :: 3
```

### Comparing `raga-testing-platform-1.1.7/README.md` & `raga-testing-platform-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.1.7/pyproject.toml` & `raga-testing-platform-1.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61", "setuptools_scm[toml]>=7"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "raga-testing-platform"
-version = "1.1.7"
+version = "1.1.8"
 authors = [
   { name="Raga AI", email="support@ragaai.com" },
 ]
 maintainers = [{ name = "Raga AI", email = "support@ragaai.com" }]
 dependencies = [
     "pandas==2.0.2",
     "urllib3==1.26.7",
```

### Comparing `raga-testing-platform-1.1.7/raga/__init__.py` & `raga-testing-platform-1.1.8/raga/__init__.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.1.7/raga/_tests.py` & `raga-testing-platform-1.1.8/raga/_tests.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.1.7/raga/constants.py` & `raga-testing-platform-1.1.8/raga/constants.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.1.7/raga/dataset.py` & `raga-testing-platform-1.1.8/raga/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,17 +167,26 @@
             failure_callback=on_upload_failed,
         )
         delete_files(self.csv_file, self.zip_file)
 
         self.dataset_file_id = self.create_dataset_load_definition(file_path, "csv", self.raga_schema.columns)
         res_data = self.notify_server(org=org)
         data = res_data.get('data')
+        print("JOOOOOB", org)
         if isinstance(data, dict) and data.get('jobId', None):
             spinner.start()
+            print("JOOOOOB", org)
             self.wait_for_status(data.get('jobId', None))
+            print("JOOOOOB", org)
+            if org == "lm-v2":
+                print("PPPPPPLLLL")
+                res_data = self.notify_server(org="lm-img-v2")
+                data = res_data.get('data')
+                if isinstance(data, dict) and data.get('jobId', None):
+                    self.wait_for_status(data.get('jobId', None))
             spinner.stop()
 
     def load_dataset_from_file(self):
         from raga import REQUIRED_ARG
         if not self.format:
             raise DatasetException(f"{REQUIRED_ARG.format('format')}")
         if not self.model_name:
@@ -209,16 +218,19 @@
 
         arguments = make_arg(self.model_name, self.inference_col_name, self.embedding_col_name)
 
         self.dataset_file_id = self.create_dataset_load_definition(file_path, format, arguments)
         self.notify_server()
     
 
-    def lightmetrics_data_upload(self):
-        self.load(org="lm")
+    def lightmetrics_data_upload(self, api_version="v2"):
+        if api_version == "v1":
+            self.load(org="lm")
+        else:
+            self.load(org="lm-v2")
 
 
     def head(self):
         res_data = self.test_session.http_client.get(
             f"api/dataset/{self.dataset_id}/data",
             headers={"Authorization": f'Bearer {self.test_session.token}'},
         )
@@ -247,15 +259,19 @@
         """
         Notifies the server to load the dataset with the provided experiment ID and data definition.
         """
         spinner.start()
         end_point = "api/experiment/load-data"
         if org=="lm":
             end_point = "api/experiment/load-data-lm"
-        
+        if org=="lm-v2":
+            end_point = "api/experiment/load-data-lm/v2"
+        if org=="lm-img-v2":
+            end_point = "api/experiment/load-image-data-lm"
+            
         res_data = self.test_session.http_client.post(
             end_point,
             {"experimentId": self.test_session.experiment_id, "datasetFileId": self.dataset_file_id},
             {"Authorization": f'Bearer {self.test_session.token}'},
         )
         logger.debug(res_data.get('data', ''))
         return res_data
```

### Comparing `raga-testing-platform-1.1.7/raga/examples/.DS_Store` & `raga-testing-platform-1.1.8/raga/examples/.DS_Store`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.1.7/raga/examples/ab_event_unlabelled.py` & `raga-testing-platform-1.1.8/raga/examples/ab_event_unlabelled.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.1.7/raga/examples/data_drift.py` & `raga-testing-platform-1.1.8/raga/examples/data_drift.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.1.7/raga/examples/failure_mode_analysis_image_classification.py` & `raga-testing-platform-1.1.8/raga/examples/failure_mode_analysis_image_classification.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.1.7/raga/examples/failure_mode_analysis_object_detection.py` & `raga-testing-platform-1.1.8/raga/examples/failure_mode_analysis_object_detection.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.1.7/raga/examples/failure_mode_analysis_semantic_segmentation.py` & `raga-testing-platform-1.1.8/raga/examples/failure_mode_analysis_semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.1.7/raga/examples/labelling_quality_image_classification.py` & `raga-testing-platform-1.1.8/raga/examples/labelling_quality_image_classification.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.1.7/raga/examples/labelling_quality_semantic_segment.py` & `raga-testing-platform-1.1.8/raga/examples/labelling_quality_semantic_segment.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.1.7/raga/examples/lm_dataloader.py` & `raga-testing-platform-1.1.8/raga/examples/lm_dataloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,14 +98,14 @@
 # # create test_session object of TestSession instance
 test_session = TestSession(project_name="testingProject", run_name= run_name, access_key="LGXJjQFD899MtVSrNHGH", secret_key="TC466Qu9PhpOjTuLu5aGkXyGbM7SSBeAzYH6HpcP", host="http://3.111.106.226:8080")
 
 creds = DatasetCreds(region="ap-south-1")
 
 # #create test_ds object of Dataset instance
 video_ds = Dataset(test_session=test_session,
-                  name="test-lm-loader-6-nov-v5",
+                  name="test-lm-loader-10-nov-v1",
                   type=DATASET_TYPE.VIDEO,
                   data=pd_video_data_frame,
                   schema=schema,
                   creds=creds)
 #load schema and pandas data frame
 video_ds.lightmetrics_data_upload()
```

### Comparing `raga-testing-platform-1.1.7/raga/examples/lm_event_loader_failure_mode_analysis_object_detection-2.py` & `raga-testing-platform-1.1.8/raga/examples/lm_event_loader_failure_mode_analysis_object_detection-2.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.1.7/raga/examples/lm_event_loader_failure_mode_analysis_object_detection.py` & `raga-testing-platform-1.1.8/raga/examples/lm_event_loader_failure_mode_analysis_object_detection.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.1.7/raga/examples/lm_image_loader_failure_mode_analysis_object_detection-copy.py` & `raga-testing-platform-1.1.8/raga/examples/lm_image_loader_failure_mode_analysis_object_detection-copy.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.1.7/raga/examples/lm_image_loader_failure_mode_analysis_object_detection.py` & `raga-testing-platform-1.1.8/raga/examples/lm_image_loader_failure_mode_analysis_object_detection.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.1.7/raga/examples/lm_inference_generator.py` & `raga-testing-platform-1.1.8/raga/examples/lm_inference_generator.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.1.7/raga/examples/lm_model_upload.py` & `raga-testing-platform-1.1.8/raga/examples/lm_model_upload.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.1.7/raga/examples/lm_video_loader_failure_mode_analysis_object_detection.py` & `raga-testing-platform-1.1.8/raga/examples/lm_video_loader_failure_mode_analysis_object_detection.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.1.7/raga/examples/loader_ai_dash_object_detection.py` & `raga-testing-platform-1.1.8/raga/examples/loader_ai_dash_object_detection.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.1.7/raga/examples/loader_failure_mode_analysis_image_classification.py` & `raga-testing-platform-1.1.8/raga/examples/loader_failure_mode_analysis_image_classification.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.1.7/raga/examples/loader_failure_mode_analysis_object_detection.py` & `raga-testing-platform-1.1.8/raga/examples/loader_failure_mode_analysis_object_detection.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.1.7/raga/examples/loader_failure_mode_analysis_semantic_segmentation.py` & `raga-testing-platform-1.1.8/raga/examples/loader_failure_mode_analysis_semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.1.7/raga/examples/loader_failure_mode_analysis_super_resolution.py` & `raga-testing-platform-1.1.8/raga/examples/loader_failure_mode_analysis_super_resolution.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.1.7/raga/examples/loader_honeywell_data.py` & `raga-testing-platform-1.1.8/raga/examples/loader_honeywell_data.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.1.7/raga/examples/loader_labeling_quality_image_classification.py` & `raga-testing-platform-1.1.8/raga/examples/loader_labeling_quality_image_classification.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.1.7/raga/examples/loader_labeling_quality_semantic_segmentation.py` & `raga-testing-platform-1.1.8/raga/examples/loader_labeling_quality_semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.1.7/raga/examples/loader_labeling_quality_semantic_segmentation_data_drift.py` & `raga-testing-platform-1.1.8/raga/examples/loader_labeling_quality_semantic_segmentation_data_drift.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.1.7/raga/examples/loader_labeling_quality_semantic_segmentation_tree_health.py` & `raga-testing-platform-1.1.8/raga/examples/loader_labeling_quality_semantic_segmentation_tree_health.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.1.7/raga/examples/loader_labeling_quality_semantic_segmentation_v2.py` & `raga-testing-platform-1.1.8/raga/examples/loader_labeling_quality_semantic_segmentation_v2.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.1.7/raga/examples/loader_labeling_quality_semantic_segmentation_v3.py` & `raga-testing-platform-1.1.8/raga/examples/loader_labeling_quality_semantic_segmentation_v3.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.1.7/raga/examples/loader_labeling_quality_semantic_segmentation_v4.py` & `raga-testing-platform-1.1.8/raga/examples/loader_labeling_quality_semantic_segmentation_v4.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.1.7/raga/examples/loader_satsure_inference_oct_2023.py` & `raga-testing-platform-1.1.8/raga/examples/loader_satsure_inference_oct_2023.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.1.7/raga/examples/loader_satsure_new_dat_nov_2023.py` & `raga-testing-platform-1.1.8/raga/examples/loader_satsure_new_dat_nov_2023.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.1.7/raga/examples/loader_satsure_new_dat_nov_2023_100img.py` & `raga-testing-platform-1.1.8/raga/examples/loader_satsure_new_dat_nov_2023_100img.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.1.7/raga/examples/loader_satsure_new_dat_nov_2023_using_ready_ds.py` & `raga-testing-platform-1.1.8/raga/examples/loader_satsure_new_dat_nov_2023_using_ready_ds.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     8: "built_area",
     9: "bare_ground",
     10: "snow_or_ice",
     11: "clouds",
 }
 
 def csv_parser(csv_path):
-    data_frame = pd.read_csv(csv_path)
+    data_frame = pd.read_csv(csv_path).head(10)
     return data_frame
 
 
 pd_data_frame = csv_parser("./assets/test.csv")
 
 
 schema = RagaSchema()
@@ -34,15 +34,15 @@
 # satsure-prod
 test_session = TestSession(project_name="testingProject", run_name = run_name, profile="dev")
 
 cred = DatasetCreds(region="us-east-2")
 
 #create test_ds object of Dataset instance
 test_ds = Dataset(test_session=test_session,
-                  name="satsure_new_data_nov_9_v1",
+                  name="satsure_new_data_nov",
                   type=DATASET_TYPE.IMAGE,
                   data=pd_data_frame,
                   schema=schema,
                   creds=cred,
                   temp=True)
 
 #load to server
```

### Comparing `raga-testing-platform-1.1.7/raga/examples/model_distribution-mistakescore.py` & `raga-testing-platform-1.1.8/raga/examples/model_distribution-mistakescore.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.1.7/raga/examples/model_distribution-v2.py` & `raga-testing-platform-1.1.8/raga/examples/model_distribution-v2.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.1.7/raga/examples/model_distribution.py` & `raga-testing-platform-1.1.8/raga/examples/model_distribution.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.1.7/raga/examples/nano_dataset_upload_missing_values.py` & `raga-testing-platform-1.1.8/raga/examples/nano_dataset_upload_missing_values.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.1.7/raga/examples/nano_dataset_upload_outlier.py` & `raga-testing-platform-1.1.8/raga/examples/nano_dataset_upload_outlier.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.1.7/raga/examples/ocr_missing_value_test.py` & `raga-testing-platform-1.1.8/raga/examples/ocr_missing_value_test.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.1.7/raga/examples/ocr_outlier_detection_test.py` & `raga-testing-platform-1.1.8/raga/examples/ocr_outlier_detection_test.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.1.7/raga/examples/sts_test.py` & `raga-testing-platform-1.1.8/raga/examples/sts_test.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.1.7/raga/filters.py` & `raga-testing-platform-1.1.8/raga/filters.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.1.7/raga/lightmetrics.py` & `raga-testing-platform-1.1.8/raga/lightmetrics.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 import json
+import logging
 import os
+import pathlib
 import zipfile
-from raga import TestSession, Filter
-from raga import spinner
+
+from raga import Filter, TestSession, spinner
 from raga.utils.dataset_util import upload_file
 
+logger = logging.getLogger(__name__)
+
 def lightmetrics_inference_generator(test_session:TestSession, dataset_name: str, model_name:str, model_inference_col_name:str, event_inference_col_name:str, filter:Filter):
-    from raga.constants import INVALID_RESPONSE, INVALID_RESPONSE_DATA, REQUIRED_ARG_V2
+    from raga.constants import (INVALID_RESPONSE, INVALID_RESPONSE_DATA,
+                                REQUIRED_ARG_V2)
     dataset_id = lightmetrics_inference_generator_validation(test_session, dataset_name, model_name, model_inference_col_name, event_inference_col_name, filter)
     payload = {
             "datasetId": dataset_id,
             "experimentId": test_session.experiment_id,
             "model": model_name,
             "modelInferenceColName": model_inference_col_name,
             "eventInferenceColName": event_inference_col_name,
@@ -20,15 +25,16 @@
 
     if not isinstance(res_data, dict):
         spinner.stop()
         raise ValueError(INVALID_RESPONSE)
     spinner.stop()
 
 def lightmetrics_inference_generator_validation(test_session:TestSession, dataset_name:str, model_name:str, model_inference_col_name:str, event_inference_col_name:str, filter:Filter):
-    from raga.constants import INVALID_RESPONSE, INVALID_RESPONSE_DATA, REQUIRED_ARG_V2
+    from raga.constants import (INVALID_RESPONSE, INVALID_RESPONSE_DATA,
+                                REQUIRED_ARG_V2)
 
     assert isinstance(test_session, TestSession), f"{REQUIRED_ARG_V2.format('test_session', 'instance of the TestSession')}"
     assert isinstance(dataset_name, str) and dataset_name, f"{REQUIRED_ARG_V2.format('dataset_name', 'str')}"
     res_data = test_session.http_client.get(f"api/dataset?projectId={test_session.project_id}&name={dataset_name}", headers={"Authorization": f'Bearer {test_session.token}'})
 
     if not isinstance(res_data, dict):
             raise ValueError(INVALID_RESPONSE)
@@ -39,45 +45,84 @@
         raise KeyError(INVALID_RESPONSE_DATA)
     assert isinstance(model_name, str) and model_name, f"{REQUIRED_ARG_V2.format('model_name', 'str')}"
     assert isinstance(model_inference_col_name, str) and model_inference_col_name, f"{REQUIRED_ARG_V2.format('model_inference_col_name', 'str')}"
     assert isinstance(event_inference_col_name, str) and event_inference_col_name, f"{REQUIRED_ARG_V2.format('event_inference_col_name', 'str')}"
     assert isinstance(filter, Filter) and filter, f"{REQUIRED_ARG_V2.format('filter', 'instance of the Filter')}"
     return dataset_id
 
-def lightmetrics_model_upload(test_session:TestSession, file_path:str, name:str, version:str, override:bool=True):
+def lightmetrics_model_upload(test_session:TestSession, file_path:str, name:str, version:str, api_version="v1"):
+    if api_version == "v2":
+        lightmetrics_model_upload_v2(test_session, file_path, name, version)
+    else:
+        lightmetrics_model_upload_v1(test_session, file_path, name, version)
+
+def lightmetrics_model_upload_v1(test_session: TestSession, file_path: str, name: str, version: str,
+                              override: bool = True):
     from raga.constants import INVALID_RESPONSE, INVALID_RESPONSE_DATA, REQUIRED_ARG_V2
     assert isinstance(file_path, str) and file_path, f"{REQUIRED_ARG_V2.format('file_path', 'str')}"
     assert isinstance(name, str) and name, f"{REQUIRED_ARG_V2.format('name', 'str')}"
     assert isinstance(version, str) and version, f"{REQUIRED_ARG_V2.format('version', 'str')}"
+
+    if not os.path.exists(file_path):
+        raise FileNotFoundError(f"{file_path} does not exist.")
+    if not file_path.lower().endswith(".zip"):
+        raise TypeError("File mush be zip")
+    model_zip_validation(file_path, name)
+
+    payload = {
+        "projectId": test_session.project_id,
+        "modelName": name,
+        "modelVersion": version
+    }
+
+    res_data = test_session.http_client.post(f"api/model-upload", data=payload,
+                                             headers={"Authorization": f'Bearer {test_session.token}'}, file=file_path)
+
+    if not isinstance(res_data, dict):
+        spinner.stop()
+        raise ValueError(INVALID_RESPONSE)
+    spinner.stop()
+
+
+def lightmetrics_model_upload_v2(test_session:TestSession, file_path:str, name:str, version:str, override:bool=True):
+    from raga.constants import (INVALID_RESPONSE, INVALID_RESPONSE_DATA,
+                                REQUIRED_ARG_V2)
+    assert isinstance(file_path, str) and file_path, f"{REQUIRED_ARG_V2.format('file_path', 'str')}"
+    assert isinstance(name, str) and name, f"{REQUIRED_ARG_V2.format('name', 'str')}"
+    assert isinstance(version, str) and version, f"{REQUIRED_ARG_V2.format('version', 'str')}"
     
     if not os.path.exists(file_path):
         raise FileNotFoundError(f"{file_path} does not exist.")
     if not file_path.lower().endswith(".zip"):
         raise TypeError("File mush be zip")
     model_zip_validation(file_path, name)
     
 
     payload = {
+            "file": pathlib.Path(file_path).name,
             "projectId": test_session.project_id,
             "modelName": name,
             "modelVersion": version
         }
     
-    res_data = test_session.http_client.post(f"api/model-upload", data=payload, headers={"Authorization": f'Bearer {test_session.token}'}, file=file_path)
-
+    res_data = test_session.http_client.post(f"api/model-upload/v2", data=payload, headers={"Authorization": f'Bearer {test_session.token}'})
     if not isinstance(res_data, dict):
         spinner.stop()
         raise ValueError(INVALID_RESPONSE)
     else:
-        model_upload_to_url(res_data.get("uploadPreSignedUrl"), file_path)
-        res_data = test_session.http_client.put(f"api/models-version/{res_data.get('modelVersionEntity').get('id')}", headers={"Authorization": f'Bearer {test_session.token}'})
+        if res_data.get('success') == True:
+            data = res_data.get('data')
+            model_upload_to_url(data.get("uploadPreSignedUrl"), file_path)
+        else:
+            raise ValueError('Failed to upload model')
     spinner.stop()
 
 def model_upload_to_url(url: str, file: str):
-    upload_file(url, file=file)
+    # TODO: add retry mechanism
+    upload_file(url, file)
 
 def model_zip_validation(path, model_name):
     with zipfile.ZipFile(path, "r") as zip_file:
         all_names = zip_file.namelist()
         directories = [name for name in all_names if name.endswith("/") and '/' in name]
         if directories:
             directories.sort(key=lambda x: x.count('/'))
```

### Comparing `raga-testing-platform-1.1.7/raga/model_executor_factory.py` & `raga-testing-platform-1.1.8/raga/model_executor_factory.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.1.7/raga/post_deployment_checks.py` & `raga-testing-platform-1.1.8/raga/post_deployment_checks.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.1.7/raga/raga_schema.py` & `raga-testing-platform-1.1.8/raga/raga_schema.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.1.7/raga/test_session.py` & `raga-testing-platform-1.1.8/raga/test_session.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.1.7/raga/tests/test_dataset.py` & `raga-testing-platform-1.1.8/raga/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.1.7/raga/tests/test_dataset_util.py` & `raga-testing-platform-1.1.8/raga/tests/test_dataset_util.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.1.7/raga/tests/test_http_client.py` & `raga-testing-platform-1.1.8/raga/tests/test_http_client.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.1.7/raga/tests/test_test_session.py` & `raga-testing-platform-1.1.8/raga/tests/test_test_session.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.1.7/raga/tests/test_tests.py` & `raga-testing-platform-1.1.8/raga/tests/test_tests.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.1.7/raga/utils/dataset_util.py` & `raga-testing-platform-1.1.8/raga/utils/dataset_util.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.1.7/raga/utils/file.py` & `raga-testing-platform-1.1.8/raga/utils/file.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.1.7/raga/utils/http_client.py` & `raga-testing-platform-1.1.8/raga/utils/http_client.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.1.7/raga/utils/raga_config_reader.py` & `raga-testing-platform-1.1.8/raga/utils/raga_config_reader.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.1.7/raga/validators/dataset_creds_validations.py` & `raga-testing-platform-1.1.8/raga/validators/dataset_creds_validations.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.1.7/raga/validators/dataset_validations.py` & `raga-testing-platform-1.1.8/raga/validators/dataset_validations.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.1.7/raga/validators/test_session_validation.py` & `raga-testing-platform-1.1.8/raga/validators/test_session_validation.py`

 * *Files identical despite different names*

### Comparing `raga-testing-platform-1.1.7/raga_testing_platform.egg-info/PKG-INFO` & `raga-testing-platform-1.1.8/raga_testing_platform.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raga-testing-platform
-Version: 1.1.7
+Version: 1.1.8
 Summary: Short description or overview of the raga package.
 Author-email: Raga AI <support@ragaai.com>
 Maintainer-email: Raga AI <support@ragaai.com>
 Project-URL: Homepage, https://github.com/whoosh-labs/testing-platform-python-client
 Project-URL: Bug Tracker, https://github.com/whoosh-labs/testing-platform-python-client/issues
 Keywords: testing-platform,raga-testing-platform,model-testing,AB_testing
 Classifier: Programming Language :: Python :: 3
```

### Comparing `raga-testing-platform-1.1.7/raga_testing_platform.egg-info/SOURCES.txt` & `raga-testing-platform-1.1.8/raga_testing_platform.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 raga/examples/loader_labeling_quality_semantic_segmentation_v2.py
 raga/examples/loader_labeling_quality_semantic_segmentation_v3.py
 raga/examples/loader_labeling_quality_semantic_segmentation_v4.py
 raga/examples/loader_satsure_inference_oct_2023.py
 raga/examples/loader_satsure_new_dat_nov_2023.py
 raga/examples/loader_satsure_new_dat_nov_2023_100img.py
 raga/examples/loader_satsure_new_dat_nov_2023_using_ready_ds.py
+raga/examples/model-upload.py
 raga/examples/model_distribution-mistakescore.py
 raga/examples/model_distribution-v2.py
 raga/examples/model_distribution.py
 raga/examples/nano_dataset_upload_missing_values.py
 raga/examples/nano_dataset_upload_outlier.py
 raga/examples/ocr_missing_value_test.py
 raga/examples/ocr_outlier_detection_test.py
```

