# Comparing `tmp/dkist-processing-common-6.2.1.tar.gz` & `tmp/dkist-processing-common-6.2.1rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist-processing-common-6.2.1.tar", last modified: Wed May  1 16:25:33 2024, max compression
+gzip compressed data, was "dkist-processing-common-6.2.1rc2.tar", last modified: Tue Apr 30 16:44:53 2024, max compression
```

## Comparing `dkist-processing-common-6.2.1.tar` & `dkist-processing-common-6.2.1rc2.tar`

### file list

```diff
@@ -1,134 +1,138 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-01 16:25:33.824902 dkist-processing-common-6.2.1/
--rw-rw-rw-   0 root         (0) root         (0)     2481 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      844 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      429 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/.readthedocs.yml
--rw-rw-rw-   0 root         (0) root         (0)    25154 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     4367 2024-05-01 16:25:33.824902 dkist-processing-common-6.2.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3730 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     3271 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-01 16:25:33.812902 dkist-processing-common-6.2.1/changelog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/changelog/.gitempty
--rwxrwxrwx   0 root         (0) root         (0)      642 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/check_changelog_updated.sh
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-01 16:25:33.812902 dkist-processing-common-6.2.1/dkist_processing_common/
--rw-rw-rw-   0 root         (0) root         (0)      317 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-01 16:25:33.812902 dkist-processing-common-6.2.1/dkist_processing_common/_util/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/_util/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2931 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/_util/config.py
--rw-rw-rw-   0 root         (0) root         (0)     3244 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/_util/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     1178 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/_util/dkist_location.py
--rw-rw-rw-   0 root         (0) root         (0)     3426 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/_util/graphql.py
--rw-rw-rw-   0 root         (0) root         (0)    10378 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/_util/scratch.py
--rw-rw-rw-   0 root         (0) root         (0)     6226 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/_util/tags.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-01 16:25:33.812902 dkist-processing-common-6.2.1/dkist_processing_common/codecs/
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/codecs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      823 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/codecs/asdf.py
--rw-rw-rw-   0 root         (0) root         (0)      495 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/codecs/bytes.py
--rw-rw-rw-   0 root         (0) root         (0)     2331 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/codecs/fits.py
--rw-rw-rw-   0 root         (0) root         (0)      977 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/codecs/iobase.py
--rw-rw-rw-   0 root         (0) root         (0)      939 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/codecs/json.py
--rw-rw-rw-   0 root         (0) root         (0)      197 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/codecs/path.py
--rw-rw-rw-   0 root         (0) root         (0)      679 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/codecs/str.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-01 16:25:33.816902 dkist-processing-common-6.2.1/dkist_processing_common/fonts/
--rw-rw-rw-   0 root         (0) root         (0)   656568 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/fonts/Lato-Regular.ttf
--rw-rw-rw-   0 root         (0) root         (0)      101 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/fonts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7037 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/manual.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-01 16:25:33.816902 dkist-processing-common-6.2.1/dkist_processing_common/models/
--rw-rw-rw-   0 root         (0) root         (0)       74 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5409 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/models/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     4113 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/models/fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)     5128 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/models/flower_pot.py
--rw-rw-rw-   0 root         (0) root         (0)     3681 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/models/graphql.py
--rw-rw-rw-   0 root         (0) root         (0)     1109 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/models/message.py
--rw-rw-rw-   0 root         (0) root         (0)     6532 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/models/parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     2225 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/models/quality.py
--rw-rw-rw-   0 root         (0) root         (0)     1096 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/models/quality_json_encoders.py
--rw-rw-rw-   0 root         (0) root         (0)    11331 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/models/tags.py
--rw-rw-rw-   0 root         (0) root         (0)      565 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/models/task_name.py
--rw-rw-rw-   0 root         (0) root         (0)      870 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/models/wavelength.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-01 16:25:33.816902 dkist-processing-common-6.2.1/dkist_processing_common/parsers/
--rw-rw-rw-   0 root         (0) root         (0)       67 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/parsers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6461 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/parsers/cs_step.py
--rw-rw-rw-   0 root         (0) root         (0)     1571 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/parsers/dsps_repeat.py
--rw-rw-rw-   0 root         (0) root         (0)      706 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/parsers/experiment_id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)     1536 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/parsers/id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)      921 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/parsers/l0_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)     2595 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/parsers/l1_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)      677 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/parsers/proposal_id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)     1058 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/parsers/quality.py
--rw-rw-rw-   0 root         (0) root         (0)     1230 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/parsers/single_value_single_key_flower.py
--rw-rw-rw-   0 root         (0) root         (0)     3938 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/parsers/task.py
--rw-rw-rw-   0 root         (0) root         (0)     7839 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/parsers/time.py
--rw-rw-rw-   0 root         (0) root         (0)     3041 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/parsers/unique_bud.py
--rw-rw-rw-   0 root         (0) root         (0)      545 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/parsers/wavelength.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-01 16:25:33.820902 dkist-processing-common-6.2.1/dkist_processing_common/tasks/
--rw-rw-rw-   0 root         (0) root         (0)      562 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12507 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/tasks/assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)    13069 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/tasks/base.py
--rw-rw-rw-   0 root         (0) root         (0)     8882 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/tasks/l1_output_data.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-01 16:25:33.820902 dkist-processing-common-6.2.1/dkist_processing_common/tasks/mixin/
--rw-rw-rw-   0 root         (0) root         (0)       68 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/tasks/mixin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6598 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/tasks/mixin/globus.py
--rw-rw-rw-   0 root         (0) root         (0)     6813 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/tasks/mixin/input_dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     2077 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/tasks/mixin/interservice_bus.py
--rw-rw-rw-   0 root         (0) root         (0)    14513 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/tasks/mixin/metadata_store.py
--rw-rw-rw-   0 root         (0) root         (0)     3242 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/tasks/mixin/object_store.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-01 16:25:33.820902 dkist-processing-common-6.2.1/dkist_processing_common/tasks/mixin/quality/
--rw-rw-rw-   0 root         (0) root         (0)      383 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/tasks/mixin/quality/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8115 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/tasks/mixin/quality/_base.py
--rw-rw-rw-   0 root         (0) root         (0)    47664 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/tasks/mixin/quality/_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     3699 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/tasks/output_data_base.py
--rw-rw-rw-   0 root         (0) root         (0)     7986 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/tasks/parse_l0_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     8852 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/tasks/quality_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     2270 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/tasks/teardown.py
--rw-rw-rw-   0 root         (0) root         (0)     5215 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/tasks/transfer_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     6120 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/tasks/trial_catalog.py
--rw-rw-rw-   0 root         (0) root         (0)     8200 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/tasks/trial_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)    19478 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/tasks/write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-01 16:25:33.824902 dkist-processing-common-6.2.1/dkist_processing_common/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    27198 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     4165 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/tests/test_assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)     7048 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/tests/test_base.py
--rw-rw-rw-   0 root         (0) root         (0)    11068 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/tests/test_codecs.py
--rw-rw-rw-   0 root         (0) root         (0)     5903 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/tests/test_constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2408 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/tests/test_cs_step.py
--rw-rw-rw-   0 root         (0) root         (0)      513 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/tests/test_dkist_location.py
--rw-rw-rw-   0 root         (0) root         (0)    10946 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/tests/test_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)     3151 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/tests/test_flower_pot.py
--rw-rw-rw-   0 root         (0) root         (0)    19450 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/tests/test_input_dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     3120 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/tests/test_output_data_base.py
--rw-rw-rw-   0 root         (0) root         (0)     8346 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/tests/test_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)    10629 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/tests/test_parse_l0_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     3198 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/tests/test_publish_catalog_messages.py
--rw-rw-rw-   0 root         (0) root         (0)     9356 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/tests/test_quality.py
--rw-rw-rw-   0 root         (0) root         (0)    36297 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/tests/test_quality_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    16481 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/tests/test_scratch.py
--rw-rw-rw-   0 root         (0) root         (0)    24306 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/tests/test_stems.py
--rw-rw-rw-   0 root         (0) root         (0)     5023 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/tests/test_tags.py
--rw-rw-rw-   0 root         (0) root         (0)     1234 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/tests/test_task_name.py
--rw-rw-rw-   0 root         (0) root         (0)     4027 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/tests/test_task_parsing.py
--rw-rw-rw-   0 root         (0) root         (0)     5494 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/tests/test_teardown.py
--rw-rw-rw-   0 root         (0) root         (0)     6658 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/tests/test_transfer_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     2109 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/tests/test_transfer_l1_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)     4614 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/tests/test_trial_catalog.py
--rw-rw-rw-   0 root         (0) root         (0)    15740 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/tests/test_trial_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)    10488 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/tests/test_workflow_task_base.py
--rw-rw-rw-   0 root         (0) root         (0)    17411 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/dkist_processing_common/tests/test_write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-01 16:25:33.812902 dkist-processing-common-6.2.1/dkist_processing_common.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     4367 2024-05-01 16:25:33.000000 dkist-processing-common-6.2.1/dkist_processing_common.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4991 2024-05-01 16:25:33.000000 dkist-processing-common-6.2.1/dkist_processing_common.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-01 16:25:33.000000 dkist-processing-common-6.2.1/dkist_processing_common.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      770 2024-05-01 16:25:33.000000 dkist-processing-common-6.2.1/dkist_processing_common.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       24 2024-05-01 16:25:33.000000 dkist-processing-common-6.2.1/dkist_processing_common.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-01 16:25:33.824902 dkist-processing-common-6.2.1/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4598 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      120 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     1890 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      113 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     4513 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)       29 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/docs/requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-01 16:25:33.824902 dkist-processing-common-6.2.1/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1462 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      780 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1839 2024-05-01 16:25:33.824902 dkist-processing-common-6.2.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      102 2024-05-01 16:25:27.000000 dkist-processing-common-6.2.1/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 16:44:53.947109 dkist-processing-common-6.2.1rc2/
+-rw-rw-rw-   0 root         (0) root         (0)     2481 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      844 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      429 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/.readthedocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)    24493 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4370 2024-04-30 16:44:53.947109 dkist-processing-common-6.2.1rc2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3730 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3271 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 16:44:53.935109 dkist-processing-common-6.2.1rc2/changelog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/changelog/.gitempty
+-rw-rw-rw-   0 root         (0) root         (0)       97 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/changelog/124.misc.rst
+-rw-rw-rw-   0 root         (0) root         (0)       68 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/changelog/186.misc.rst
+-rw-rw-rw-   0 root         (0) root         (0)       66 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/changelog/187.misc.rst
+-rw-rw-rw-   0 root         (0) root         (0)       28 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/changelog/188.misc.rst
+-rwxrwxrwx   0 root         (0) root         (0)      642 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/check_changelog_updated.sh
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 16:44:53.935109 dkist-processing-common-6.2.1rc2/dkist_processing_common/
+-rw-rw-rw-   0 root         (0) root         (0)      317 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 16:44:53.935109 dkist-processing-common-6.2.1rc2/dkist_processing_common/_util/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/_util/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2931 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/_util/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     3244 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/_util/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     1178 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/_util/dkist_location.py
+-rw-rw-rw-   0 root         (0) root         (0)     3426 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/_util/graphql.py
+-rw-rw-rw-   0 root         (0) root         (0)    10378 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/_util/scratch.py
+-rw-rw-rw-   0 root         (0) root         (0)     6226 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/_util/tags.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 16:44:53.935109 dkist-processing-common-6.2.1rc2/dkist_processing_common/codecs/
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/codecs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      823 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/codecs/asdf.py
+-rw-rw-rw-   0 root         (0) root         (0)      495 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/codecs/bytes.py
+-rw-rw-rw-   0 root         (0) root         (0)     2331 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/codecs/fits.py
+-rw-rw-rw-   0 root         (0) root         (0)      977 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/codecs/iobase.py
+-rw-rw-rw-   0 root         (0) root         (0)      939 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/codecs/json.py
+-rw-rw-rw-   0 root         (0) root         (0)      197 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/codecs/path.py
+-rw-rw-rw-   0 root         (0) root         (0)      679 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/codecs/str.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 16:44:53.939109 dkist-processing-common-6.2.1rc2/dkist_processing_common/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)   656568 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/fonts/Lato-Regular.ttf
+-rw-rw-rw-   0 root         (0) root         (0)      101 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/fonts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7037 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/manual.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 16:44:53.939109 dkist-processing-common-6.2.1rc2/dkist_processing_common/models/
+-rw-rw-rw-   0 root         (0) root         (0)       74 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5409 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/models/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     4113 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/models/fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)     5128 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/models/flower_pot.py
+-rw-rw-rw-   0 root         (0) root         (0)     3681 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/models/graphql.py
+-rw-rw-rw-   0 root         (0) root         (0)     1109 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/models/message.py
+-rw-rw-rw-   0 root         (0) root         (0)     6532 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/models/parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     2225 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/models/quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     1096 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/models/quality_json_encoders.py
+-rw-rw-rw-   0 root         (0) root         (0)    11331 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/models/tags.py
+-rw-rw-rw-   0 root         (0) root         (0)      565 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/models/task_name.py
+-rw-rw-rw-   0 root         (0) root         (0)      870 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/models/wavelength.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 16:44:53.939109 dkist-processing-common-6.2.1rc2/dkist_processing_common/parsers/
+-rw-rw-rw-   0 root         (0) root         (0)       67 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/parsers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6461 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/parsers/cs_step.py
+-rw-rw-rw-   0 root         (0) root         (0)     1571 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/parsers/dsps_repeat.py
+-rw-rw-rw-   0 root         (0) root         (0)      706 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/parsers/experiment_id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)     1536 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/parsers/id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)      921 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/parsers/l0_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)     2595 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/parsers/l1_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)      677 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/parsers/proposal_id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)     1058 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/parsers/quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     1230 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/parsers/single_value_single_key_flower.py
+-rw-rw-rw-   0 root         (0) root         (0)     3938 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/parsers/task.py
+-rw-rw-rw-   0 root         (0) root         (0)     7839 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/parsers/time.py
+-rw-rw-rw-   0 root         (0) root         (0)     3041 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/parsers/unique_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)      545 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/parsers/wavelength.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 16:44:53.943109 dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)      562 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12507 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)    13069 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     8882 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/l1_output_data.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 16:44:53.943109 dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/mixin/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/mixin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6598 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/mixin/globus.py
+-rw-rw-rw-   0 root         (0) root         (0)     6813 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/mixin/input_dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     2077 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/mixin/interservice_bus.py
+-rw-rw-rw-   0 root         (0) root         (0)    14513 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/mixin/metadata_store.py
+-rw-rw-rw-   0 root         (0) root         (0)     3242 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/mixin/object_store.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 16:44:53.943109 dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/mixin/quality/
+-rw-rw-rw-   0 root         (0) root         (0)      383 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/mixin/quality/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8115 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/mixin/quality/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    47664 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/mixin/quality/_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     3699 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/output_data_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     7986 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/parse_l0_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     8852 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/quality_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     2270 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/teardown.py
+-rw-rw-rw-   0 root         (0) root         (0)     5215 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/transfer_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     6120 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/trial_catalog.py
+-rw-rw-rw-   0 root         (0) root         (0)     8200 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/trial_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    19478 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 16:44:53.947109 dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    27198 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     4165 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)     7048 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    11068 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_codecs.py
+-rw-rw-rw-   0 root         (0) root         (0)     5903 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2408 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_cs_step.py
+-rw-rw-rw-   0 root         (0) root         (0)      513 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_dkist_location.py
+-rw-rw-rw-   0 root         (0) root         (0)    10946 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)     3151 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_flower_pot.py
+-rw-rw-rw-   0 root         (0) root         (0)    19450 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_input_dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     3120 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_output_data_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     8346 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)    10629 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_parse_l0_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     3198 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_publish_catalog_messages.py
+-rw-rw-rw-   0 root         (0) root         (0)     9356 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_quality.py
+-rw-rw-rw-   0 root         (0) root         (0)    36297 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_quality_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    16481 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_scratch.py
+-rw-rw-rw-   0 root         (0) root         (0)    24306 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_stems.py
+-rw-rw-rw-   0 root         (0) root         (0)     5023 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_tags.py
+-rw-rw-rw-   0 root         (0) root         (0)     1234 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_task_name.py
+-rw-rw-rw-   0 root         (0) root         (0)     4027 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_task_parsing.py
+-rw-rw-rw-   0 root         (0) root         (0)     5494 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_teardown.py
+-rw-rw-rw-   0 root         (0) root         (0)     6658 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_transfer_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     2109 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_transfer_l1_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     4614 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_trial_catalog.py
+-rw-rw-rw-   0 root         (0) root         (0)    15740 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_trial_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    10488 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_workflow_task_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    17411 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 16:44:53.935109 dkist-processing-common-6.2.1rc2/dkist_processing_common.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     4370 2024-04-30 16:44:53.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5083 2024-04-30 16:44:53.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-30 16:44:53.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      770 2024-04-30 16:44:53.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       24 2024-04-30 16:44:53.000000 dkist-processing-common-6.2.1rc2/dkist_processing_common.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 16:44:53.947109 dkist-processing-common-6.2.1rc2/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4598 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      120 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1890 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      113 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)       29 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/docs/requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 16:44:53.947109 dkist-processing-common-6.2.1rc2/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      780 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1839 2024-04-30 16:44:53.947109 dkist-processing-common-6.2.1rc2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      102 2024-04-30 16:44:48.000000 dkist-processing-common-6.2.1rc2/setup.py
```

### Comparing `dkist-processing-common-6.2.1/.gitignore` & `dkist-processing-common-6.2.1rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/.pre-commit-config.yaml` & `dkist-processing-common-6.2.1rc2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/CHANGELOG.rst` & `dkist-processing-common-6.2.1rc2/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-v6.2.1 (2024-05-01)
-===================
-
-Misc
-----
-
-- Change filenames of browse movie and quality report to free up namespace for other future files. (`#124 <https://bitbucket.org/dkistdc/dkist-processing-common/pull-requests/124>`__)
-- Trial framework asdf filenames match production run asdf filenames. (`#186 <https://bitbucket.org/dkistdc/dkist-processing-common/pull-requests/186>`__)
-- Capture tracing data for rollback calls to enhance observability. (`#187 <https://bitbucket.org/dkistdc/dkist-processing-common/pull-requests/187>`__)
-- Update legacy type hinting. (`#188 <https://bitbucket.org/dkistdc/dkist-processing-common/pull-requests/188>`__)
-
-
 v6.1.2 (2024-04-12)
 ===================
 
 Misc
 ----
 
 - Refactor retrieval of input dataset parts to only occur when directly requested. (`#180 <https://bitbucket.org/dkistdc/dkist-processing-common/pull-requests/180>`__)
```

### Comparing `dkist-processing-common-6.2.1/PKG-INFO` & `dkist-processing-common-6.2.1rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-common
-Version: 6.2.1
+Version: 6.2.1rc2
 Summary: Common task classes used by the DKIST Science Data Processing pipelines to process DKIST data.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-common/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/common
 Classifier: Programming Language :: Python
```

### Comparing `dkist-processing-common-6.2.1/README.rst` & `dkist-processing-common-6.2.1rc2/README.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/bitbucket-pipelines.yml` & `dkist-processing-common-6.2.1rc2/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/check_changelog_updated.sh` & `dkist-processing-common-6.2.1rc2/check_changelog_updated.sh`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/_util/config.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/_util/config.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/_util/constants.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/_util/constants.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/_util/dkist_location.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/_util/dkist_location.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/_util/graphql.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/_util/graphql.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/_util/scratch.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/_util/scratch.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/_util/tags.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/_util/tags.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/codecs/asdf.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/codecs/asdf.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/codecs/fits.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/codecs/fits.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/codecs/iobase.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/codecs/iobase.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/codecs/json.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/codecs/json.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/codecs/str.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/codecs/str.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/fonts/Lato-Regular.ttf` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/fonts/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/manual.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/manual.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/models/constants.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/models/constants.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/models/fits_access.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/models/fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/models/flower_pot.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/models/flower_pot.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/models/graphql.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/models/graphql.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/models/message.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/models/message.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/models/parameters.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/models/parameters.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/models/quality.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/models/quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/models/quality_json_encoders.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/models/quality_json_encoders.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/models/tags.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/models/tags.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/models/task_name.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/models/task_name.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/models/wavelength.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/models/wavelength.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/parsers/cs_step.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/parsers/cs_step.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/parsers/dsps_repeat.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/parsers/dsps_repeat.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/parsers/experiment_id_bud.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/parsers/experiment_id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/parsers/id_bud.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/parsers/id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/parsers/l0_fits_access.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/parsers/l0_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/parsers/l1_fits_access.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/parsers/l1_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/parsers/proposal_id_bud.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/parsers/proposal_id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/parsers/quality.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/parsers/quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/parsers/single_value_single_key_flower.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/parsers/single_value_single_key_flower.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/parsers/task.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/parsers/task.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/parsers/time.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/parsers/time.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/parsers/unique_bud.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/parsers/unique_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/parsers/wavelength.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/parsers/wavelength.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/tasks/__init__.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/tasks/assemble_movie.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/tasks/base.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/tasks/l1_output_data.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/l1_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/tasks/mixin/globus.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/mixin/globus.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/tasks/mixin/input_dataset.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/mixin/input_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/tasks/mixin/interservice_bus.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/mixin/interservice_bus.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/tasks/mixin/metadata_store.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/mixin/metadata_store.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/tasks/mixin/object_store.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/mixin/object_store.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/tasks/mixin/quality/_base.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/mixin/quality/_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/tasks/mixin/quality/_metrics.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/mixin/quality/_metrics.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/tasks/output_data_base.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/output_data_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/tasks/parse_l0_input_data.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/parse_l0_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/tasks/quality_metrics.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/quality_metrics.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/tasks/teardown.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/teardown.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/tasks/transfer_input_data.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/transfer_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/tasks/trial_catalog.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/trial_catalog.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/tasks/trial_output_data.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/trial_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/tasks/write_l1.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tasks/write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/tests/conftest.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/tests/test_assemble_movie.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/tests/test_base.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/tests/test_codecs.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_codecs.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/tests/test_constants.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/tests/test_cs_step.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_cs_step.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/tests/test_dkist_location.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_dkist_location.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/tests/test_fits_access.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/tests/test_flower_pot.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_flower_pot.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/tests/test_input_dataset.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_input_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/tests/test_output_data_base.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_output_data_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/tests/test_parameters.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/tests/test_parse_l0_input_data.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_parse_l0_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/tests/test_publish_catalog_messages.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_publish_catalog_messages.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/tests/test_quality.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/tests/test_quality_mixin.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_quality_mixin.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/tests/test_scratch.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_scratch.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/tests/test_stems.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_stems.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/tests/test_tags.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/tests/test_task_name.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_task_name.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/tests/test_task_parsing.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_task_parsing.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/tests/test_teardown.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_teardown.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/tests/test_transfer_input_data.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_transfer_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/tests/test_transfer_l1_output_data.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_transfer_l1_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/tests/test_trial_catalog.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_trial_catalog.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/tests/test_trial_output_data.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_trial_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/tests/test_workflow_task_base.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_workflow_task_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common/tests/test_write_l1.py` & `dkist-processing-common-6.2.1rc2/dkist_processing_common/tests/test_write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common.egg-info/PKG-INFO` & `dkist-processing-common-6.2.1rc2/dkist_processing_common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-common
-Version: 6.2.1
+Version: 6.2.1rc2
 Summary: Common task classes used by the DKIST Science Data Processing pipelines to process DKIST data.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-common/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/common
 Classifier: Programming Language :: Python
```

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common.egg-info/SOURCES.txt` & `dkist-processing-common-6.2.1rc2/dkist_processing_common.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 README.rst
 bitbucket-pipelines.yml
 check_changelog_updated.sh
 pyproject.toml
 setup.cfg
 setup.py
 changelog/.gitempty
+changelog/124.misc.rst
+changelog/186.misc.rst
+changelog/187.misc.rst
+changelog/188.misc.rst
 dkist_processing_common/__init__.py
 dkist_processing_common/manual.py
 dkist_processing_common.egg-info/PKG-INFO
 dkist_processing_common.egg-info/SOURCES.txt
 dkist_processing_common.egg-info/dependency_links.txt
 dkist_processing_common.egg-info/requires.txt
 dkist_processing_common.egg-info/top_level.txt
```

### Comparing `dkist-processing-common-6.2.1/dkist_processing_common.egg-info/requires.txt` & `dkist-processing-common-6.2.1rc2/dkist_processing_common.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/docs/Makefile` & `dkist-processing-common-6.2.1rc2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/docs/conf.py` & `dkist-processing-common-6.2.1rc2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/docs/make.bat` & `dkist-processing-common-6.2.1rc2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/licenses/LICENSE.rst` & `dkist-processing-common-6.2.1rc2/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/pyproject.toml` & `dkist-processing-common-6.2.1rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.1/setup.cfg` & `dkist-processing-common-6.2.1rc2/setup.cfg`

 * *Files identical despite different names*

