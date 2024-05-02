# Comparing `tmp/dkist_processing_visp-2.8.2.tar.gz` & `tmp/dkist_processing_visp-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist_processing_visp-2.8.2.tar", last modified: Fri Nov 24 18:11:31 2023, max compression
+gzip compressed data, was "dkist_processing_visp-2.9.0.tar", last modified: Wed Nov 29 15:25:42 2023, max compression
```

## Comparing `dkist_processing_visp-2.8.2.tar` & `dkist_processing_visp-2.9.0.tar`

### file list

```diff
@@ -1,116 +1,117 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-11-24 18:11:31.032228 dkist_processing_visp-2.8.2/
--rw-rw-rw-   0 root         (0) root         (0)     2461 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      841 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      306 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/.readthedocs.yml
--rw-rw-rw-   0 root         (0) root         (0)    24594 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     6213 2023-11-24 18:11:31.032228 dkist_processing_visp-2.8.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5645 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     3652 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/SCIENCE_CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     3428 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-11-24 18:11:31.024228 dkist_processing_visp-2.8.2/changelog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/changelog/.gitempty
--rwxrwxrwx   0 root         (0) root         (0)      642 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/check_changelog_updated.sh
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-11-24 18:11:31.024228 dkist_processing_visp-2.8.2/dkist_processing_visp/
--rw-rw-rw-   0 root         (0) root         (0)      339 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-11-24 18:11:31.024228 dkist_processing_visp-2.8.2/dkist_processing_visp/fonts/
--rw-rw-rw-   0 root         (0) root         (0)   656568 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/fonts/Lato-Regular.ttf
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-11-24 18:11:31.024228 dkist_processing_visp-2.8.2/dkist_processing_visp/models/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4534 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/models/constants.py
--rw-rw-rw-   0 root         (0) root         (0)    11324 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/models/parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     1271 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/models/tags.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-11-24 18:11:31.028228 dkist_processing_visp-2.8.2/dkist_processing_visp/parsers/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/parsers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5370 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/parsers/map_repeats.py
--rw-rw-rw-   0 root         (0) root         (0)     3005 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/parsers/modulator_states.py
--rw-rw-rw-   0 root         (0) root         (0)      876 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/parsers/polarimeter_mode.py
--rw-rw-rw-   0 root         (0) root         (0)     2913 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/parsers/raster_step.py
--rw-rw-rw-   0 root         (0) root         (0)     1268 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/parsers/task.py
--rw-rw-rw-   0 root         (0) root         (0)      901 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/parsers/time.py
--rw-rw-rw-   0 root         (0) root         (0)     1335 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/parsers/visp_l0_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)      859 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/parsers/visp_l1_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)      843 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/parsers/wavelength.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-11-24 18:11:31.028228 dkist_processing_visp-2.8.2/dkist_processing_visp/tasks/
--rw-rw-rw-   0 root         (0) root         (0)      772 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3329 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/tasks/assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)    16004 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/tasks/background_light.py
--rw-rw-rw-   0 root         (0) root         (0)     4674 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/tasks/dark.py
--rw-rw-rw-   0 root         (0) root         (0)    42011 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/tasks/geometric.py
--rw-rw-rw-   0 root         (0) root         (0)    20533 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/tasks/instrument_polarization.py
--rw-rw-rw-   0 root         (0) root         (0)      428 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/tasks/l1_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)     5943 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/tasks/lamp.py
--rw-rw-rw-   0 root         (0) root         (0)     7121 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/tasks/make_movie_frames.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-11-24 18:11:31.028228 dkist_processing_visp-2.8.2/dkist_processing_visp/tasks/mixin/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/tasks/mixin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5642 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/tasks/mixin/corrections.py
--rw-rw-rw-   0 root         (0) root         (0)     1343 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/tasks/mixin/downsample.py
--rw-rw-rw-   0 root         (0) root         (0)     7412 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/tasks/mixin/input_frame_loaders.py
--rw-rw-rw-   0 root         (0) root         (0)    11004 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/tasks/mixin/intermediate_frame_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     4056 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/tasks/mixin/line_zones.py
--rw-rw-rw-   0 root         (0) root         (0)     5810 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/tasks/parse.py
--rw-rw-rw-   0 root         (0) root         (0)     8004 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/tasks/quality_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)    28529 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/tasks/science.py
--rw-rw-rw-   0 root         (0) root         (0)    25541 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/tasks/solar.py
--rw-rw-rw-   0 root         (0) root         (0)     1648 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/tasks/trial_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)     1559 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/tasks/visp_base.py
--rw-rw-rw-   0 root         (0) root         (0)     6896 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/tasks/write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-11-24 18:11:31.032228 dkist_processing_visp-2.8.2/dkist_processing_visp/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17036 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/tests/conftest.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-11-24 18:11:31.032228 dkist_processing_visp-2.8.2/dkist_processing_visp/tests/local_trial_workflows/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/tests/local_trial_workflows/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    19357 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/tests/local_trial_workflows/l0_to_l1.py
--rw-rw-rw-   0 root         (0) root         (0)     8265 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/tests/local_trial_workflows/local_trial_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     2471 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/tests/test_assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)    18423 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/tests/test_background_light.py
--rw-rw-rw-   0 root         (0) root         (0)     1132 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/tests/test_build_quality_report.py
--rw-rw-rw-   0 root         (0) root         (0)     5558 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/tests/test_dark.py
--rw-rw-rw-   0 root         (0) root         (0)     2173 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/tests/test_downsample.py
--rw-rw-rw-   0 root         (0) root         (0)    14296 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/tests/test_geometric.py
--rw-rw-rw-   0 root         (0) root         (0)    12554 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/tests/test_instrument_polarization.py
--rw-rw-rw-   0 root         (0) root         (0)     5755 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/tests/test_lamp.py
--rw-rw-rw-   0 root         (0) root         (0)     3978 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/tests/test_make_movie_frames.py
--rw-rw-rw-   0 root         (0) root         (0)    11689 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/tests/test_map_repeats.py
--rw-rw-rw-   0 root         (0) root         (0)     2578 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/tests/test_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)    20404 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/tests/test_parse.py
--rw-rw-rw-   0 root         (0) root         (0)     4344 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/tests/test_quality.py
--rw-rw-rw-   0 root         (0) root         (0)    22657 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/tests/test_science.py
--rw-rw-rw-   0 root         (0) root         (0)     9915 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/tests/test_solar.py
--rw-rw-rw-   0 root         (0) root         (0)     1082 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/tests/test_submit_quality.py
--rw-rw-rw-   0 root         (0) root         (0)     5297 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/tests/test_trial_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)     5049 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/tests/test_visp_base.py
--rw-rw-rw-   0 root         (0) root         (0)     1878 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/tests/test_visp_constants.py
--rw-rw-rw-   0 root         (0) root         (0)      286 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/tests/test_workflows.py
--rw-rw-rw-   0 root         (0) root         (0)     5709 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/tests/test_write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-11-24 18:11:31.032228 dkist_processing_visp-2.8.2/dkist_processing_visp/workflows/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/workflows/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3110 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/workflows/l0_processing.py
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/workflows/single_task_workflows.py
--rw-rw-rw-   0 root         (0) root         (0)     3206 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/dkist_processing_visp/workflows/trial_workflows.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-11-24 18:11:31.024228 dkist_processing_visp-2.8.2/dkist_processing_visp.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     6213 2023-11-24 18:11:30.000000 dkist_processing_visp-2.8.2/dkist_processing_visp.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3971 2023-11-24 18:11:31.000000 dkist_processing_visp-2.8.2/dkist_processing_visp.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-11-24 18:11:30.000000 dkist_processing_visp-2.8.2/dkist_processing_visp.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      636 2023-11-24 18:11:30.000000 dkist_processing_visp-2.8.2/dkist_processing_visp.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-11-24 18:11:30.000000 dkist_processing_visp-2.8.2/dkist_processing_visp.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-11-24 18:11:31.032228 dkist_processing_visp-2.8.2/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4598 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)     4844 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/docs/background_light.rst
--rw-rw-rw-   0 root         (0) root         (0)      346 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     2028 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     6427 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/docs/gain_correction.rst
--rw-rw-rw-   0 root         (0) root         (0)      273 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      623 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/docs/l0_to_l1_visp.rst
--rw-rw-rw-   0 root         (0) root         (0)     4513 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)     4995 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/docs/polarization_calibration.rst
--rw-rw-rw-   0 root         (0) root         (0)       29 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/docs/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      292 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/docs/requirements_table.rst
--rw-rw-rw-   0 root         (0) root         (0)     2429 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/docs/science_calibration.rst
--rw-rw-rw-   0 root         (0) root         (0)      300 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/docs/scientific_changelog.rst
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-11-24 18:11:31.032228 dkist_processing_visp-2.8.2/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1462 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      776 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/pyproject.toml
--rwxrwxrwx   0 root         (0) root         (0)       60 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/science_towncrier.sh
--rw-rw-rw-   0 root         (0) root         (0)     1702 2023-11-24 18:11:31.036228 dkist_processing_visp-2.8.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      102 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      422 2023-11-24 18:11:25.000000 dkist_processing_visp-2.8.2/towncrier_science.toml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-11-29 15:25:42.799698 dkist_processing_visp-2.9.0/
+-rw-rw-rw-   0 root         (0) root         (0)     2461 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      841 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      306 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/.readthedocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)    26949 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6213 2023-11-29 15:25:42.799698 dkist_processing_visp-2.9.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5645 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3652 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/SCIENCE_CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3428 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-11-29 15:25:42.791698 dkist_processing_visp-2.9.0/changelog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/changelog/.gitempty
+-rwxrwxrwx   0 root         (0) root         (0)      642 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/check_changelog_updated.sh
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-11-29 15:25:42.791698 dkist_processing_visp-2.9.0/dkist_processing_visp/
+-rw-rw-rw-   0 root         (0) root         (0)      339 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-11-29 15:25:42.791698 dkist_processing_visp-2.9.0/dkist_processing_visp/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)   656568 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/fonts/Lato-Regular.ttf
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-11-29 15:25:42.795698 dkist_processing_visp-2.9.0/dkist_processing_visp/models/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5127 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/models/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)    10005 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/models/parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     1497 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/models/tags.py
+-rw-rw-rw-   0 root         (0) root         (0)      186 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/models/task_name.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-11-29 15:25:42.795698 dkist_processing_visp-2.9.0/dkist_processing_visp/parsers/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/parsers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5467 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/parsers/map_repeats.py
+-rw-rw-rw-   0 root         (0) root         (0)     3005 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/parsers/modulator_states.py
+-rw-rw-rw-   0 root         (0) root         (0)      540 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/parsers/polarimeter_mode.py
+-rw-rw-rw-   0 root         (0) root         (0)     3045 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/parsers/raster_step.py
+-rw-rw-rw-   0 root         (0) root         (0)     4350 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/parsers/time.py
+-rw-rw-rw-   0 root         (0) root         (0)     1335 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/parsers/visp_l0_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)      859 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/parsers/visp_l1_fits_access.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-11-29 15:25:42.795698 dkist_processing_visp-2.9.0/dkist_processing_visp/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)      772 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3329 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/tasks/assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)    16047 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/tasks/background_light.py
+-rw-rw-rw-   0 root         (0) root         (0)     4367 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/tasks/dark.py
+-rw-rw-rw-   0 root         (0) root         (0)    41841 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/tasks/geometric.py
+-rw-rw-rw-   0 root         (0) root         (0)    20461 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/tasks/instrument_polarization.py
+-rw-rw-rw-   0 root         (0) root         (0)      428 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/tasks/l1_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     5824 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/tasks/lamp.py
+-rw-rw-rw-   0 root         (0) root         (0)     7283 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/tasks/make_movie_frames.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-11-29 15:25:42.795698 dkist_processing_visp-2.9.0/dkist_processing_visp/tasks/mixin/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/tasks/mixin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      869 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/tasks/mixin/beam_access.py
+-rw-rw-rw-   0 root         (0) root         (0)     5642 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/tasks/mixin/corrections.py
+-rw-rw-rw-   0 root         (0) root         (0)     1343 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/tasks/mixin/downsample.py
+-rw-rw-rw-   0 root         (0) root         (0)     9090 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/tasks/mixin/intermediate_frame_helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     4056 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/tasks/mixin/line_zones.py
+-rw-rw-rw-   0 root         (0) root         (0)     6383 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/tasks/parse.py
+-rw-rw-rw-   0 root         (0) root         (0)     8223 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/tasks/quality_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)    27623 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/tasks/science.py
+-rw-rw-rw-   0 root         (0) root         (0)    25643 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/tasks/solar.py
+-rw-rw-rw-   0 root         (0) root         (0)     1895 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/tasks/trial_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     1477 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/tasks/visp_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     6896 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/tasks/write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-11-29 15:25:42.799698 dkist_processing_visp-2.9.0/dkist_processing_visp/tests/
+-rw-rw-rw-   0 root         (0) root         (0)    12502 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/tests/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15609 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)    15515 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/tests/header_models.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-11-29 15:25:42.799698 dkist_processing_visp-2.9.0/dkist_processing_visp/tests/local_trial_workflows/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/tests/local_trial_workflows/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    19490 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/tests/local_trial_workflows/l0_to_l1.py
+-rw-rw-rw-   0 root         (0) root         (0)     8447 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/tests/local_trial_workflows/local_trial_helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2293 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/tests/test_assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)    17401 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/tests/test_background_light.py
+-rw-rw-rw-   0 root         (0) root         (0)     1132 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/tests/test_build_quality_report.py
+-rw-rw-rw-   0 root         (0) root         (0)     5592 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/tests/test_dark.py
+-rw-rw-rw-   0 root         (0) root         (0)     2193 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/tests/test_downsample.py
+-rw-rw-rw-   0 root         (0) root         (0)    11872 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/tests/test_geometric.py
+-rw-rw-rw-   0 root         (0) root         (0)     9892 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/tests/test_instrument_polarization.py
+-rw-rw-rw-   0 root         (0) root         (0)     5252 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/tests/test_lamp.py
+-rw-rw-rw-   0 root         (0) root         (0)     2566 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/tests/test_make_movie_frames.py
+-rw-rw-rw-   0 root         (0) root         (0)     7511 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/tests/test_map_repeats.py
+-rw-rw-rw-   0 root         (0) root         (0)     4132 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/tests/test_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)    18227 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/tests/test_parse.py
+-rw-rw-rw-   0 root         (0) root         (0)     3385 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/tests/test_quality.py
+-rw-rw-rw-   0 root         (0) root         (0)    19953 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/tests/test_science.py
+-rw-rw-rw-   0 root         (0) root         (0)     9261 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/tests/test_solar.py
+-rw-rw-rw-   0 root         (0) root         (0)     1082 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/tests/test_submit_quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     5542 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/tests/test_trial_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     4521 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/tests/test_visp_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1878 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/tests/test_visp_constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      286 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/tests/test_workflows.py
+-rw-rw-rw-   0 root         (0) root         (0)     5494 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/tests/test_write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-11-29 15:25:42.799698 dkist_processing_visp-2.9.0/dkist_processing_visp/workflows/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/workflows/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3110 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/workflows/l0_processing.py
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/workflows/single_task_workflows.py
+-rw-rw-rw-   0 root         (0) root         (0)     3206 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/dkist_processing_visp/workflows/trial_workflows.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-11-29 15:25:42.791698 dkist_processing_visp-2.9.0/dkist_processing_visp.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     6213 2023-11-29 15:25:42.000000 dkist_processing_visp-2.9.0/dkist_processing_visp.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4007 2023-11-29 15:25:42.000000 dkist_processing_visp-2.9.0/dkist_processing_visp.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-11-29 15:25:42.000000 dkist_processing_visp-2.9.0/dkist_processing_visp.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      614 2023-11-29 15:25:42.000000 dkist_processing_visp-2.9.0/dkist_processing_visp.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-11-29 15:25:42.000000 dkist_processing_visp-2.9.0/dkist_processing_visp.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-11-29 15:25:42.799698 dkist_processing_visp-2.9.0/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4598 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)     5147 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/docs/background_light.rst
+-rw-rw-rw-   0 root         (0) root         (0)      346 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2028 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     6427 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/docs/gain_correction.rst
+-rw-rw-rw-   0 root         (0) root         (0)      273 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      623 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/docs/l0_to_l1_visp.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)     4995 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/docs/polarization_calibration.rst
+-rw-rw-rw-   0 root         (0) root         (0)       29 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/docs/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      292 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/docs/requirements_table.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2429 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/docs/science_calibration.rst
+-rw-rw-rw-   0 root         (0) root         (0)      300 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/docs/scientific_changelog.rst
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-11-29 15:25:42.799698 dkist_processing_visp-2.9.0/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      776 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/pyproject.toml
+-rwxrwxrwx   0 root         (0) root         (0)       60 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/science_towncrier.sh
+-rw-rw-rw-   0 root         (0) root         (0)     1675 2023-11-29 15:25:42.799698 dkist_processing_visp-2.9.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      102 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      422 2023-11-29 15:25:34.000000 dkist_processing_visp-2.9.0/towncrier_science.toml
```

### Comparing `dkist_processing_visp-2.8.2/.gitignore` & `dkist_processing_visp-2.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.8.2/.pre-commit-config.yaml` & `dkist_processing_visp-2.9.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.8.2/CHANGELOG.rst` & `dkist_processing_visp-2.9.0/CHANGELOG.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,36 @@
+v2.9.0 (2023-11-29)
+===================
+
+Features
+--------
+
+- Use `DarkReadoutExpTimePickyBud` to fail fast (during `Parse`)if the required set of dark frames are not present in the input data. (`#133 <https://bitbucket.org/dkistdc/dkist-processing-visp/pull-requests/133>`__)
+
+
+Misc
+----
+
+- Create new `VispParsingParameters` class that contains only those parameters that are needed for parsing. (`#127 <https://bitbucket.org/dkistdc/dkist-processing-visp/pull-requests/127>`__)
+- Simplify `VispParameter` class by using new defaults and mixins from `dkist-processing-common`. (`#127 <https://bitbucket.org/dkistdc/dkist-processing-visp/pull-requests/127>`__)
+- Use new `TaskName` paradigm from `dkist-processing-common` to minimize replication of constant strings corresponding to IP task types. (`#128 <https://bitbucket.org/dkistdc/dkist-processing-visp/pull-requests/128>`__)
+- Use new `TaskUniqueBud` to simplify and normalize parsing Buds with the framework in `dkist-processing-common`. (`#128 <https://bitbucket.org/dkistdc/dkist-processing-visp/pull-requests/128>`__)
+- Refactor `IntermediateFrameHelpersMixin` to have clearer arguments and method flow. `intermediate_frame_helpers_load_intermediate_arrays` now just takes in raw tags. (`#130 <https://bitbucket.org/dkistdc/dkist-processing-visp/pull-requests/130>`__)
+- Remove all usage of `FitsDataMixin`. The codec aware `write` and `read` are how we do this now. (`#131 <https://bitbucket.org/dkistdc/dkist-processing-visp/pull-requests/131>`__)
+- Refactor stale and mostly-unused `InputFrameLoadersMixin` to `BeamAccessMixin` that contains method for extracting a single beam from raw input data. (`#132 <https://bitbucket.org/dkistdc/dkist-processing-visp/pull-requests/132>`__)
+- Big refactor of unit tests for improved maintainability. (`#135 <https://bitbucket.org/dkistdc/dkist-processing-visp/pull-requests/135>`__)
+- Remove `nd_left_matrix_multiply` and instead import it from updated `dkist-processing-math`. It's the same function, just in a more obvious place. (`#136 <https://bitbucket.org/dkistdc/dkist-processing-visp/pull-requests/136>`__)
+
+
+Documentation
+-------------
+
+- Update online doc for background light algorithm to indicate that it isn't applied since a hardware fix in Nov 2022. (`#138 <https://bitbucket.org/dkistdc/dkist-processing-visp/pull-requests/138>`__)
+
+
 v2.8.2 (2023-11-24)
 ===================
 
 Misc
 ----
 
 - Updates to core and common to patch security vulnerabilities and deprecations. (`#135 <https://bitbucket.org/dkistdc/dkist-processing-visp/pull-requests/135>`__)
```

### Comparing `dkist_processing_visp-2.8.2/PKG-INFO` & `dkist_processing_visp-2.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist_processing_visp
-Version: 2.8.2
+Version: 2.9.0
 Summary: Science processing code for the ViSP instrument on DKIST
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-visp/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/visp
 Classifier: Programming Language :: Python
```

### Comparing `dkist_processing_visp-2.8.2/README.rst` & `dkist_processing_visp-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.8.2/SCIENCE_CHANGELOG.rst` & `dkist_processing_visp-2.9.0/SCIENCE_CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.8.2/bitbucket-pipelines.yml` & `dkist_processing_visp-2.9.0/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.8.2/check_changelog_updated.sh` & `dkist_processing_visp-2.9.0/check_changelog_updated.sh`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.8.2/dkist_processing_visp/fonts/Lato-Regular.ttf` & `dkist_processing_visp-2.9.0/dkist_processing_visp/fonts/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.8.2/dkist_processing_visp/models/constants.py` & `dkist_processing_visp-2.9.0/dkist_processing_visp/models/constants.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,18 +16,20 @@
     lamp_readout_exp_times = "LAMP_READOUT_EXP_TIMES"
     solar_exposure_times = "SOLAR_EXPOSURE_TIMES"
     solar_readout_exp_times = "SOLAR_READOUT_EXP_TIMES"
     observe_exposure_times = "OBSERVE_EXPOSURE_TIMES"
     observe_readout_exp_times = "OBSERVE_READOUT_EXP_TIMES"
     polcal_exposure_times = "POLCAL_EXPOSURE_TIMES"
     polcal_readout_exp_times = "POLCAL_READOUT_EXP_TIMES"
+    non_dark_task_readout_exp_times = "NON_DARK_TASK_READOUT_EXP_TIMES"
     num_map_scans = "NUM_MAP_SCANS"
     axis_1_type = "AXIS_1_TYPE"
     axis_2_type = "AXIS_2_TYPE"
     axis_3_type = "AXIS_3_TYPE"
+    dark_readout_exp_time_picky_bud = "DARK_READOUT_EXP_TIME_PICKY_BUD"
 
 
 class VispConstants(ConstantsBase):
     """Visp specific constants to add to the common constants."""
 
     @property
     def wavelength(self) -> float:
@@ -111,14 +113,24 @@
         """Find the polarization calibration readout exposure time."""
         if self.correct_for_polarization:
             return self._db_dict[VispBudName.polcal_readout_exp_times.value]
         else:
             return []
 
     @property
+    def non_dark_task_readout_exp_times(self) -> [float]:
+        """
+        Find all readout exposure times that *need* to exist in a dark IP.
+
+        Every non-dark task needs to be corrected with an average dark frame of the same readout exp time, which means
+        we need DARK IP task frames for all of these readout exposure times.
+        """
+        return self._db_dict[VispBudName.non_dark_task_readout_exp_times.value]
+
+    @property
     def observe_readout_exp_times(self) -> [float]:
         """Find the observation readout exposure time."""
         return self._db_dict[VispBudName.observe_readout_exp_times.value]
 
     @property
     def axis_1_type(self) -> str:
         """Find the type of the first array axis."""
```

### Comparing `dkist_processing_visp-2.8.2/dkist_processing_visp/models/parameters.py` & `dkist_processing_visp-2.9.0/dkist_processing_visp/models/parameters.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,28 @@
 """Visp calibration pipeline parameters."""
-from datetime import datetime
-from typing import Any
-
-import numpy as np
 from dkist_processing_common.models.parameters import ParameterBase
-from dkist_processing_common.tasks.mixin.input_dataset import InputDatasetParameterValue
-from dkist_service_configuration import logger
+from dkist_processing_common.models.parameters import ParameterWavelengthMixin
 
 
-class VispParameters(ParameterBase):
-    """Put all Visp parameters parsed from the input dataset document in a single property."""
+class VispParsingParameters(ParameterBase):
+    """
+    Parameters specifically (and only) for the Parse task.
+
+    Needed because the Parse task doesn't know what the wavelength is yet and therefore can't use the
+    `ParameterWaveLengthMixin`.
+    """
+
+    @property
+    def max_cs_step_time_sec(self):
+        """Time window within which CS steps with identical GOS configurations are considered to be the same."""
+        return self._find_most_recent_past_value("visp_max_cs_step_time_sec")
 
-    def __init__(
-        self,
-        input_dataset_parameters: dict[str, list[InputDatasetParameterValue]],
-        wavelength: float | None = None,
-        obs_ip_start_time: str | None = None,
-    ):
-        super().__init__(input_dataset_parameters)
-        self._wavelength = wavelength
-        try:
-            self._obs_ip_start_datetime = datetime.fromisoformat(obs_ip_start_time)
-        except TypeError:
-            logger.info(
-                "WARNING: "
-                "The task containing this parameters object did not provide an obs ip start time. "
-                "This only makes sense for the Parse task."
-            )
+
+class VispParameters(ParameterBase, ParameterWavelengthMixin):
+    """Put all Visp parameters parsed from the input dataset document in a single property."""
 
     @property
     def beam_border(self):
         """Pixel location of the border between ViSP beams."""
         return self._find_most_recent_past_value("visp_beam_border")
 
     @property
@@ -172,19 +164,14 @@
 
     @property
     def solar_zone_rel_height(self):
         """Relative height at which to compute the width of strong spectral features."""
         return self._find_most_recent_past_value("visp_solar_zone_rel_height")
 
     @property
-    def max_cs_step_time_sec(self):
-        """Time window within which CS steps with identical GOS configurations are considered to be the same."""
-        return self._find_most_recent_past_value("visp_max_cs_step_time_sec")
-
-    @property
     def polcal_spatial_median_filter_width_px(self) -> int:
         """Return the size of the median filter to apply in the spatial dimension to polcal data."""
         return self._find_most_recent_past_value("visp_polcal_spatial_median_filter_width_px")
 
     @property
     def polcal_num_spatial_bins(self) -> int:
         """
@@ -225,26 +212,7 @@
         """Name of set of fitting flags to use during PAC Calibration Unit parameter fits."""
         return self._find_most_recent_past_value("visp_pac_fit_mode")
 
     @property
     def pac_init_set(self):
         """Name of set of initial values for Calibration Unit parameter fit."""
         return self._find_most_recent_past_value("visp_pac_init_set")
-
-    def _find_parameter_closest_wavelength(self, parameter_name: str) -> Any:
-        """
-        Find the database value for a parameter that is closest to the requested wavelength.
-
-        NOTE: If the requested wavelength is exactly between two database values, the value from the smaller wavelength
-        will be returned
-        """
-        if self._wavelength is None:
-            raise ValueError(
-                f"Cannot get wavelength dependent parameter {parameter_name} without wavelength"
-            )
-
-        parameter_dict = self._find_most_recent_past_value(parameter_name)
-        wavelengths = np.array(parameter_dict["wavelength"])
-        values = parameter_dict["values"]
-        idx = np.argmin(np.abs(wavelengths - self._wavelength))
-        chosen_value = values[idx]
-        return chosen_value
```

### Comparing `dkist_processing_visp-2.8.2/dkist_processing_visp/models/tags.py` & `dkist_processing_visp-2.9.0/dkist_processing_visp/models/tags.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """ViSP tags."""
 from enum import Enum
 
 from dkist_processing_common.models.tags import Tag
 
+from dkist_processing_visp.models.task_name import VispTaskName
+
 
 class VispStemName(str, Enum):
     """ViSP specific tag stems."""
 
     beam = "BEAM"
     raster_step = "RASTER_STEP"  # The number of the current step within a raster scan
     modstate = "MODSTATE"
@@ -14,14 +16,19 @@
     map_scan = "MAP_SCAN"
 
 
 class VispTag(Tag):
     """ViSP specific tag formatting."""
 
     @classmethod
+    def task_background(cls) -> str:
+        """Tags intermediate background frames."""
+        return cls.task(VispTaskName.background.value)
+
+    @classmethod
     def beam(cls, beam_num: int) -> str:
         """
         Tags by beam number.
 
         Parameters
         ----------
         beam_num: int
```

### Comparing `dkist_processing_visp-2.8.2/dkist_processing_visp/parsers/map_repeats.py` & `dkist_processing_visp-2.9.0/dkist_processing_visp/parsers/map_repeats.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from collections import defaultdict
 from functools import cached_property
 from typing import Type
 
 from astropy.time import Time
 from dkist_processing_common.models.flower_pot import SpilledDirt
 from dkist_processing_common.models.flower_pot import Stem
+from dkist_processing_common.models.task_name import TaskName
 
 from dkist_processing_visp.models.constants import VispBudName
 from dkist_processing_visp.models.tags import VispStemName
 from dkist_processing_visp.parsers.visp_l0_fits_access import VispL0FitsAccess
 
 
 class SingleScanStep:
@@ -74,15 +75,15 @@
                 scan_step_obj
             )
 
         return scan_step_dict
 
     def setter(self, fits_obj: VispL0FitsAccess) -> SingleScanStep | Type[SpilledDirt]:
         """Ingest observe frames as SingleScanStep objects."""
-        if fits_obj.ip_task_type != "observe":
+        if fits_obj.ip_task_type.casefold() != TaskName.observe.value.casefold():
             return SpilledDirt
         return SingleScanStep(fits_obj=fits_obj)
 
 
 class MapScanFlower(MapScanStemBase):
     """Flower for computing and assigning map scan numbers."""
```

### Comparing `dkist_processing_visp-2.8.2/dkist_processing_visp/parsers/modulator_states.py` & `dkist_processing_visp-2.9.0/dkist_processing_visp/parsers/modulator_states.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.8.2/dkist_processing_visp/parsers/raster_step.py` & `dkist_processing_visp-2.9.0/dkist_processing_visp/parsers/raster_step.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Copies of UniqueBud and SingleValueSingleKeyFlower from common that only activate if the frames are "observe" task."""
 from typing import Type
 
 from dkist_processing_common.models.flower_pot import SpilledDirt
 from dkist_processing_common.models.flower_pot import Stem
+from dkist_processing_common.models.task_name import TaskName
 from dkist_processing_common.parsers.single_value_single_key_flower import (
     SingleValueSingleKeyFlower,
 )
 
 from dkist_processing_visp.models.constants import VispBudName
 from dkist_processing_visp.models.tags import VispStemName
 from dkist_processing_visp.parsers.visp_l0_fits_access import VispL0FitsAccess
@@ -26,15 +27,15 @@
         Setter for the bud.
 
         Parameters
         ----------
         fits_obj:
             A single FitsAccess object
         """
-        if fits_obj.ip_task_type != "observe":
+        if fits_obj.ip_task_type.casefold() != TaskName.observe.value.casefold():
             return SpilledDirt
 
         num_raster = getattr(fits_obj, self.total_num_key)
         single_step = getattr(fits_obj, self.single_step_key)
 
         return num_raster, single_step
 
@@ -75,10 +76,10 @@
         Setter for a flower.
 
         Parameters
         ----------
         fits_obj:
             A single FitsAccess object
         """
-        if fits_obj.ip_task_type != "observe":
+        if fits_obj.ip_task_type.casefold() != TaskName.observe.value.casefold():
             return SpilledDirt
         return super().setter(fits_obj)
```

### Comparing `dkist_processing_visp-2.8.2/dkist_processing_visp/parsers/visp_l0_fits_access.py` & `dkist_processing_visp-2.9.0/dkist_processing_visp/parsers/visp_l0_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.8.2/dkist_processing_visp/parsers/visp_l1_fits_access.py` & `dkist_processing_visp-2.9.0/dkist_processing_visp/parsers/visp_l1_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.8.2/dkist_processing_visp/tasks/__init__.py` & `dkist_processing_visp-2.9.0/dkist_processing_visp/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.8.2/dkist_processing_visp/tasks/assemble_movie.py` & `dkist_processing_visp-2.9.0/dkist_processing_visp/tasks/assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.8.2/dkist_processing_visp/tasks/background_light.py` & `dkist_processing_visp-2.9.0/dkist_processing_visp/tasks/background_light.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,30 +10,31 @@
 from dkist_processing_common.tasks.mixin.quality import QualityMixin
 from dkist_processing_math.arithmetic import subtract_array_from_arrays
 from dkist_processing_math.statistics import average_numpy_arrays
 from dkist_processing_math.transform.binning import resize_arrays
 from dkist_service_configuration import logger
 
 from dkist_processing_visp.models.tags import VispTag
+from dkist_processing_visp.models.task_name import VispTaskName
 from dkist_processing_visp.parsers.visp_l0_fits_access import VispL0FitsAccess
+from dkist_processing_visp.tasks.mixin.beam_access import BeamAccessMixin
 from dkist_processing_visp.tasks.mixin.corrections import CorrectionsMixin
 from dkist_processing_visp.tasks.mixin.downsample import DownsampleMixin
-from dkist_processing_visp.tasks.mixin.input_frame_loaders import InputFrameLoadersMixin
 from dkist_processing_visp.tasks.mixin.intermediate_frame_helpers import (
     IntermediateFrameHelpersMixin,
 )
 from dkist_processing_visp.tasks.visp_base import VispTaskBase
 
 __all__ = ["BackgroundLightCalibration"]
 
 
 class BackgroundLightCalibration(
     VispTaskBase,
     IntermediateFrameHelpersMixin,
-    InputFrameLoadersMixin,
+    BeamAccessMixin,
     DownsampleMixin,
     CorrectionsMixin,
     QualityMixin,
 ):
     """
     Task class for measuring additive background light that is not captured in the dark frames.
 
@@ -100,27 +101,27 @@
 
             logger.info(f"Resampling background light to full-frame for {beam = }")
             full_background_light = self.upsample_background_light(
                 small_background_light, full_shape=(full_num_wave, full_name_slit_pos)
             )
 
             self.intermediate_frame_helpers_write_arrays(
-                arrays=full_background_light, beam=beam, task="BACKGROUND"
+                arrays=full_background_light, beam=beam, task=VispTaskName.background.value
             )
             num_used_polcal_files = resampled_data.shape[0]
 
             # Note: This probably does nothing, but it *might* :shrug:
             del resampled_data
             del small_background_light
             del full_background_light
             gc.collect()
 
         with self.apm_processing_step("Computing and logging quality metrics"):
             self.quality_store_task_type_counts(
-                task_type="BACKGROUND",
+                task_type=VispTaskName.background.value,
                 total_frames=num_used_polcal_files,
             )
 
     def check_exposure_times_match(self) -> None:
         """
         Make sure that the polcal exposure times are the same as solar gain and science exposure times.
 
@@ -182,15 +183,15 @@
         logger.info(f"Using median filtering to resample spatial dimension to {num_bins} bins")
 
         for modstate in range(1, self.constants.num_modstates + 1):
             for cs_step in range(self.constants.num_cs_steps):
                 cs_step_tags = [
                     VispTag.input(),
                     VispTag.frame(),
-                    VispTag.task("POLCAL"),
+                    VispTag.task_polcal(),
                     VispTag.modstate(modstate),
                     VispTag.cs_step(cs_step),
                 ]
                 pol_cal_objs = list(
                     self.read(
                         tags=cs_step_tags,
                         decoder=fits_access_decoder,
@@ -215,16 +216,15 @@
                             tags=tags,
                             decoder=fits_access_decoder,
                             fits_access_class=VispL0FitsAccess,
                         )
                     )
 
                     readout_normalized_arrays = [
-                        self.input_frame_loaders_get_beam(obj.data, beam=beam)
-                        / obj.num_raw_frames_per_fpa
+                        self.beam_access_get_beam(obj.data, beam=beam) / obj.num_raw_frames_per_fpa
                         for obj in pol_cal_objs
                     ]
                     input_data = average_numpy_arrays(readout_normalized_arrays)
                     dark_subtracted_array = next(subtract_array_from_arrays(input_data, dark_array))
                     all_readout_frames.append(dark_subtracted_array)
 
                 avg_readout_frames = average_numpy_arrays(all_readout_frames)
```

### Comparing `dkist_processing_visp-2.8.2/dkist_processing_visp/tasks/dark.py` & `dkist_processing_visp-2.9.0/dkist_processing_visp/tasks/dark.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 """Visp dark task."""
 from dkist_processing_common.codecs.fits import fits_access_decoder
+from dkist_processing_common.models.task_name import TaskName
 from dkist_processing_common.tasks.mixin.quality import QualityMixin
 from dkist_processing_math.statistics import average_numpy_arrays
 from dkist_service_configuration import logger
 
 from dkist_processing_visp.models.tags import VispTag
 from dkist_processing_visp.parsers.visp_l0_fits_access import VispL0FitsAccess
-from dkist_processing_visp.tasks.mixin.input_frame_loaders import InputFrameLoadersMixin
+from dkist_processing_visp.tasks.mixin.beam_access import BeamAccessMixin
 from dkist_processing_visp.tasks.mixin.intermediate_frame_helpers import (
     IntermediateFrameHelpersMixin,
 )
 from dkist_processing_visp.tasks.visp_base import VispTaskBase
 
 __all__ = ["DarkCalibration"]
 
 
-class DarkCalibration(
-    VispTaskBase, InputFrameLoadersMixin, IntermediateFrameHelpersMixin, QualityMixin
-):
+class DarkCalibration(VispTaskBase, BeamAccessMixin, IntermediateFrameHelpersMixin, QualityMixin):
     """
     Task class for calculation of the averaged dark frame for a VISP calibration run.
 
     Parameters
     ----------
     recipe_run_id : int
         id of the recipe run used to identify the workflow run this task is part of
+
     workflow_name : str
         name of the workflow to which this instance of the task belongs
+
     workflow_version : str
         version of the workflow to which this instance of the task belongs
-
-
-
     """
 
     record_provenance = True
 
     def run(self):
         """
         For each beam.
@@ -46,73 +44,66 @@
             - Record quality metrics
 
         Returns
         -------
         None
 
         """
-        target_readout_exp_times = list(
-            set(
-                self.constants.solar_readout_exp_times
-                + self.constants.observe_readout_exp_times
-                + self.constants.polcal_readout_exp_times
-                + self.constants.lamp_readout_exp_times
-            )
-        )
-        logger.info(f"{target_readout_exp_times = }")
+        required_readout_exp_times = list(self.constants.non_dark_task_readout_exp_times)
+        logger.info(f"{required_readout_exp_times = }")
+
         with self.apm_task_step(
             f"Calculating dark frames for {self.constants.num_beams} beams and "
-            f"{len(target_readout_exp_times)} readout exp times"
+            f"{len(required_readout_exp_times)} readout exp times"
         ):
             total_dark_frames_used = 0
-            for readout_exp_time in target_readout_exp_times:
+            for readout_exp_time in required_readout_exp_times:
                 for beam in range(1, self.constants.num_beams + 1):
                     logger.info(
                         f"Gathering input dark frames for {readout_exp_time = } and {beam = }"
                     )
                     dark_tags = [
                         VispTag.input(),
                         VispTag.frame(),
-                        VispTag.task("DARK"),
+                        VispTag.task_dark(),
                         VispTag.readout_exp_time(readout_exp_time),
                     ]
                     current_exp_dark_count = self.scratch.count_all(tags=dark_tags)
-                    if current_exp_dark_count == 0:
-                        raise ValueError(f"Could not find any darks for {readout_exp_time = }")
                     total_dark_frames_used += current_exp_dark_count
 
                     input_dark_objs = self.read(
                         tags=dark_tags,
                         decoder=fits_access_decoder,
                         fits_access_class=VispL0FitsAccess,
                     )
 
                     with self.apm_processing_step(
                         f"Calculating dark for {readout_exp_time = } and {beam = }"
                     ):
                         readout_normalized_arrays = (
-                            self.input_frame_loaders_get_beam(o.data, beam=beam)
-                            / o.num_raw_frames_per_fpa
+                            self.beam_access_get_beam(o.data, beam=beam) / o.num_raw_frames_per_fpa
                             for o in input_dark_objs
                         )
                         averaged_dark_array = average_numpy_arrays(readout_normalized_arrays)
 
                     with self.apm_writing_step(f"Writing dark for {readout_exp_time = } {beam = }"):
                         self.intermediate_frame_helpers_write_arrays(
                             averaged_dark_array,
                             beam=beam,
-                            task="DARK",
+                            task=TaskName.dark.value,
                             readout_exp_time=readout_exp_time,
                         )
 
         with self.apm_processing_step("Computing and logging quality metrics"):
             no_of_raw_dark_frames: int = self.scratch.count_all(
                 tags=[
                     VispTag.input(),
                     VispTag.frame(),
-                    VispTag.task("DARK"),
+                    VispTag.task_dark(),
                 ],
             )
             unused_count = int(no_of_raw_dark_frames - (total_dark_frames_used / 2))
             self.quality_store_task_type_counts(
-                task_type="dark", total_frames=no_of_raw_dark_frames, frames_not_used=unused_count
+                task_type=TaskName.dark.value,
+                total_frames=no_of_raw_dark_frames,
+                frames_not_used=unused_count,
             )
```

### Comparing `dkist_processing_visp-2.8.2/dkist_processing_visp/tasks/geometric.py` & `dkist_processing_visp-2.9.0/dkist_processing_visp/tasks/geometric.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,39 +10,40 @@
 import skimage.morphology as skimo
 import skimage.registration as skir
 from astropy.modeling import fitting
 from astropy.modeling import models
 from astropy.stats import sigma_clip
 from dkist_processing_common.codecs.fits import fits_access_decoder
 from dkist_processing_common.codecs.fits import fits_array_encoder
+from dkist_processing_common.models.task_name import TaskName
 from dkist_processing_common.tasks.mixin.quality import QualityMixin
 from dkist_processing_math.arithmetic import subtract_array_from_arrays
 from dkist_processing_math.statistics import average_numpy_arrays
 from dkist_service_configuration import logger
 from scipy.fft import fftn
 from scipy.optimize import minimize
 from skimage.registration._phase_cross_correlation import _upsampled_dft
 
 from dkist_processing_visp.models.tags import VispTag
 from dkist_processing_visp.parsers.visp_l0_fits_access import VispL0FitsAccess
+from dkist_processing_visp.tasks.mixin.beam_access import BeamAccessMixin
 from dkist_processing_visp.tasks.mixin.corrections import CorrectionsMixin
-from dkist_processing_visp.tasks.mixin.input_frame_loaders import InputFrameLoadersMixin
 from dkist_processing_visp.tasks.mixin.intermediate_frame_helpers import (
     IntermediateFrameHelpersMixin,
 )
 from dkist_processing_visp.tasks.mixin.line_zones import LineZonesMixin
 from dkist_processing_visp.tasks.visp_base import VispTaskBase
 
 __all__ = ["GeometricCalibration"]
 
 
 class GeometricCalibration(
     VispTaskBase,
     IntermediateFrameHelpersMixin,
-    InputFrameLoadersMixin,
+    BeamAccessMixin,
     CorrectionsMixin,
     QualityMixin,
     LineZonesMixin,
 ):
     """
     Task class for computing the spectral geometry. Geometry is represented by three quantities.
 
@@ -131,20 +132,20 @@
                     self.write_spectral_shifts(shifts=spec_shifts, beam=beam)
 
         with self.apm_processing_step("Computing and logging quality metrics"):
             no_of_raw_geo_frames: int = self.scratch.count_all(
                 tags=[
                     VispTag.input(),
                     VispTag.frame(),
-                    VispTag.task("SOLAR_GAIN"),
+                    VispTag.task_solar_gain(),
                 ],
             )
 
             self.quality_store_task_type_counts(
-                task_type="GEOMETRIC", total_frames=no_of_raw_geo_frames
+                task_type=TaskName.geometric.value, total_frames=no_of_raw_geo_frames
             )
 
     def pre_run(self) -> None:
         """Run before run() with Elastic APM span capturing."""
         super().pre_run()
         self._fiducial_array = None
         self._fiducial_mask = None
@@ -161,17 +162,16 @@
             The current modulator state
 
         Returns
         -------
         np.ndarray
             Dark corrected data array
         """
-        array_generator = self.intermediate_frame_helpers_load_intermediate_arrays(
-            beam=beam, task="GC_SOLAR_BASIC", modstate=modstate
-        )
+        tags = [VispTag.task("GC_SOLAR_BASIC"), VispTag.beam(beam), VispTag.modstate(modstate)]
+        array_generator = self.intermediate_frame_helpers_load_intermediate_arrays(tags=tags)
         return next(array_generator)
 
     def basic_corrected_lamp_data(self, beam: int, modstate: int) -> np.ndarray:
         """
         Dark corrected lamp gain array for a single beam and modstate.
 
         Parameters
@@ -182,17 +182,16 @@
             The current modulator state
 
         Returns
         -------
         np.ndarray
             Dark corrected data array
         """
-        array_generator = self.intermediate_frame_helpers_load_intermediate_arrays(
-            beam=beam, task="GC_LAMP_BASIC", modstate=modstate
-        )
+        tags = [VispTag.task("GC_LAMP_BASIC"), VispTag.beam(beam), VispTag.modstate(modstate)]
+        array_generator = self.intermediate_frame_helpers_load_intermediate_arrays(tags=tags)
         return next(array_generator)
 
     @property
     def fiducial_array(self) -> np.ndarray:
         """Target array used for determining state offsets."""
         if self._fiducial_array is None:
             raise ValueError("Fiducial array has not been set. This should never happen.")
@@ -253,53 +252,48 @@
 
         Returns
         -------
         Generator[np.ndarray, None, None]
             Generator of state offset corrected arrays
 
         """
-        array_generator = self.intermediate_frame_helpers_load_intermediate_arrays(
-            beam=beam, task="GC_OFFSET"
-        )
+        tags = [VispTag.task("GC_OFFSET"), VispTag.beam(beam)]
+        array_generator = self.intermediate_frame_helpers_load_intermediate_arrays(tags=tags)
         return array_generator
 
     def do_basic_corrections(self):
         """Apply dark correction to all data that will be used for Geometric Calibration."""
         self._prep_lamp_gain()
         self._prep_input_solar_gain()
 
     def _prep_lamp_gain(self):
         """Apply dark corrections fo INPUT lamp frames."""
         for readout_exp_time in self.constants.lamp_readout_exp_times:
             for beam in range(1, self.constants.num_beams + 1):
                 logger.info(
                     f"Starting basic lamp reductions for {readout_exp_time = } and {beam = }"
                 )
-                try:
-                    dark_array = self.intermediate_frame_helpers_load_dark_array(
-                        beam=beam, readout_exp_time=readout_exp_time
-                    )
-                except StopIteration:
-                    raise ValueError(f"No matching dark found for {readout_exp_time = } s")
+                dark_array = self.intermediate_frame_helpers_load_dark_array(
+                    beam=beam, readout_exp_time=readout_exp_time
+                )
 
                 for modstate in range(1, self.constants.num_modstates + 1):
                     tags = [
                         VispTag.input(),
                         VispTag.frame(),
-                        VispTag.task("LAMP_GAIN"),
+                        VispTag.task_lamp_gain(),
                         VispTag.modstate(modstate),
                         VispTag.readout_exp_time(readout_exp_time),
                     ]
                     input_lamp_gain_objs = self.read(
                         tags=tags, decoder=fits_access_decoder, fits_access_class=VispL0FitsAccess
                     )
 
                     readout_normalized_arrays = (
-                        self.input_frame_loaders_get_beam(o.data, beam=beam)
-                        / o.num_raw_frames_per_fpa
+                        self.beam_access_get_beam(o.data, beam=beam) / o.num_raw_frames_per_fpa
                         for o in input_lamp_gain_objs
                     )
 
                     avg_lamp_array = average_numpy_arrays(readout_normalized_arrays)
 
                     dark_corrected_lamp_array = next(
                         subtract_array_from_arrays(
@@ -320,37 +314,33 @@
         Apply dark correction to INPUT solar gain images.
 
         Lamp correction is not applied because it was found to reduce contrast between the spectra and the hairlines.
         """
         for readout_exp_time in self.constants.solar_readout_exp_times:
             for beam in range(1, self.constants.num_beams + 1):
                 logger.info(f"Starting basic reductions for {readout_exp_time = } and {beam = }")
-                try:
-                    dark_array = self.intermediate_frame_helpers_load_dark_array(
-                        beam=beam, readout_exp_time=readout_exp_time
-                    )
-                except StopIteration:
-                    raise ValueError(f"No matching dark found for {readout_exp_time = } s")
+                dark_array = self.intermediate_frame_helpers_load_dark_array(
+                    beam=beam, readout_exp_time=readout_exp_time
+                )
 
                 for modstate in range(1, self.constants.num_modstates + 1):
 
                     tags = [
                         VispTag.input(),
                         VispTag.frame(),
-                        VispTag.task("SOLAR_GAIN"),
+                        VispTag.task_solar_gain(),
                         VispTag.modstate(modstate),
                         VispTag.readout_exp_time(readout_exp_time),
                     ]
                     input_solar_gain_objs = self.read(
                         tags=tags, decoder=fits_access_decoder, fits_access_class=VispL0FitsAccess
                     )
 
                     readout_normalized_arrays = (
-                        self.input_frame_loaders_get_beam(o.data, beam=beam)
-                        / o.num_raw_frames_per_fpa
+                        self.beam_access_get_beam(o.data, beam=beam) / o.num_raw_frames_per_fpa
                         for o in input_solar_gain_objs
                     )
 
                     avg_solar_array = average_numpy_arrays(readout_normalized_arrays)
 
                     dark_corrected_solar_array = next(
                         subtract_array_from_arrays(
@@ -654,18 +644,17 @@
 
     def prep_refine_ang_input(self, beam: int, angle: float) -> tuple[np.ndarray, np.ndarray]:
         """Prepare an averaged, high-pass-filtered array for a single beam.
 
         Average is over all modulation states.
         """
         logger.info(f"Prepping beam {beam} data for angle refinement")
+        solar_basic_tags = [VispTag.task("GC_SOLAR_BASIC"), VispTag.beam(beam)]
         arrays = list(
-            self.intermediate_frame_helpers_load_intermediate_arrays(
-                beam=beam, task="GC_SOLAR_BASIC"
-            )
+            self.intermediate_frame_helpers_load_intermediate_arrays(tags=solar_basic_tags)
         )
         # list needed here because np.stack is depreciating working with a generator
         angle_corr_arrays = list(self.corrections_correct_geometry(arrays, angle=angle))
         modstate_avg = np.mean(np.stack(angle_corr_arrays), axis=0)
 
         mask = self.compute_offset_mask(modstate_avg)
         high_pass_filtered_array = self.high_pass_filter_array(modstate_avg)
@@ -1023,15 +1012,15 @@
 
         Returns
         -------
         None
         """
         array = np.array([angle])
         self.intermediate_frame_helpers_write_arrays(
-            arrays=array, beam=beam, task="GEOMETRIC_ANGLE"
+            arrays=array, beam=beam, task=TaskName.geometric_angle.value
         )
 
     def write_state_offset(self, offset: np.ndarray, beam: int, modstate: int) -> None:
         """
         Write the state offset component of the geometric calibration for a single modstate and beam.
 
         Parameters
@@ -1047,15 +1036,15 @@
 
         Returns
         -------
         None
 
         """
         self.intermediate_frame_helpers_write_arrays(
-            arrays=offset, beam=beam, modstate=modstate, task="GEOMETRIC_OFFSET"
+            arrays=offset, beam=beam, modstate=modstate, task=TaskName.geometric_offsets.value
         )
 
     def write_spectral_shifts(self, shifts: np.ndarray, beam: int) -> None:
         """
         Write the spectral shift component of the geometric calibration for a single beam.
 
         Parameters
@@ -1068,9 +1057,9 @@
 
         Returns
         -------
         None
 
         """
         self.intermediate_frame_helpers_write_arrays(
-            arrays=shifts, beam=beam, task="GEOMETRIC_SPEC_SHIFTS"
+            arrays=shifts, beam=beam, task=TaskName.geometric_spectral_shifts.value
         )
```

### Comparing `dkist_processing_visp-2.8.2/dkist_processing_visp/tasks/instrument_polarization.py` & `dkist_processing_visp-2.9.0/dkist_processing_visp/tasks/instrument_polarization.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from collections import defaultdict
 
 import numpy as np
 import scipy.ndimage as spnd
 from astropy.io import fits
 from dkist_processing_common.codecs.fits import fits_access_decoder
 from dkist_processing_common.codecs.fits import fits_array_encoder
+from dkist_processing_common.models.task_name import TaskName
 from dkist_processing_common.tasks.mixin.quality import QualityMixin
 from dkist_processing_math.arithmetic import divide_arrays_by_array
 from dkist_processing_math.arithmetic import subtract_array_from_arrays
 from dkist_processing_math.statistics import average_numpy_arrays
 from dkist_processing_math.transform.binning import resize_arrays
 from dkist_processing_pac.fitter.polcal_fitter import PolcalFitter
 from dkist_processing_pac.input_data.drawer import Drawer
@@ -19,29 +20,29 @@
 from sklearn.pipeline import make_pipeline
 from sklearn.pipeline import Pipeline
 from sklearn.preprocessing import PolynomialFeatures
 from sklearn.preprocessing import RobustScaler
 
 from dkist_processing_visp.models.tags import VispTag
 from dkist_processing_visp.parsers.visp_l0_fits_access import VispL0FitsAccess
+from dkist_processing_visp.tasks.mixin.beam_access import BeamAccessMixin
 from dkist_processing_visp.tasks.mixin.corrections import CorrectionsMixin
 from dkist_processing_visp.tasks.mixin.downsample import DownsampleMixin
-from dkist_processing_visp.tasks.mixin.input_frame_loaders import InputFrameLoadersMixin
 from dkist_processing_visp.tasks.mixin.intermediate_frame_helpers import (
     IntermediateFrameHelpersMixin,
 )
 from dkist_processing_visp.tasks.visp_base import VispTaskBase
 
 __all__ = ["InstrumentPolarizationCalibration"]
 
 
 class InstrumentPolarizationCalibration(
     VispTaskBase,
     IntermediateFrameHelpersMixin,
-    InputFrameLoadersMixin,
+    BeamAccessMixin,
     CorrectionsMixin,
     DownsampleMixin,
     QualityMixin,
 ):
     """
     Task class for instrument polarization for a VISP calibration run.
 
@@ -130,31 +131,31 @@
                 logger.info(f"Shape of resampled demodulation matrices: {demod_matrices.shape}")
 
             with self.apm_writing_step(f"Writing demodulation matrices for {beam = }"):
                 # Save the demod matrices as intermediate products
                 self.intermediate_frame_helpers_write_arrays(
                     demod_matrices,
                     beam=beam,
-                    task="DEMOD_MATRICES",
+                    task=TaskName.demodulation_matrices.value,
                 )
 
             with self.apm_processing_step("Computing and recording polcal quality metrics"):
                 self.record_polcal_quality_metrics(beam, polcal_fitter=pac_fitter)
 
         with self.apm_processing_step("Computing and logging quality metrics"):
             no_of_raw_polcal_frames: int = self.scratch.count_all(
                 tags=[
                     VispTag.input(),
                     VispTag.frame(),
-                    VispTag.task("POLCAL"),
+                    VispTag.task_polcal(),
                 ],
             )
 
             self.quality_store_task_type_counts(
-                task_type="polcal", total_frames=no_of_raw_polcal_frames
+                task_type=TaskName.polcal.value, total_frames=no_of_raw_polcal_frames
             )
 
     def reduce_cs_steps(
         self, beam: int
     ) -> tuple[dict[int, list[VispL0FitsAccess]], dict[int, list[VispL0FitsAccess]]]:
         """
         Reduce all of the data for the cal sequence steps for this beam.
@@ -171,17 +172,17 @@
         """
         # Create the dicts to hold the results
         local_reduced_array_dict = defaultdict(list)
         global_reduced_array_dict = defaultdict(list)
 
         try:
             background_array = self.intermediate_frame_helpers_load_background_array(beam=beam)
-        except StopIteration:
+        except FileNotFoundError as e:
             if self.parameters.background_on:
-                raise ValueError(f"No background light found for {beam = }")
+                raise FileNotFoundError(f"No background light found for {beam = }") from e
             else:
                 logger.info("Skipping background light correction")
                 background_array = None
 
         logger.info(
             f"Data will be downsampled in the spatial dimension to {self.parameters.polcal_num_spatial_bins} pixels."
         )
@@ -191,20 +192,17 @@
                 beam=beam, modstate=modstate
             )
             spec_shift = self.intermediate_frame_helpers_load_spec_shift(beam=beam)
 
             for readout_exp_time in self.constants.polcal_readout_exp_times:
                 # Put this loop here because the geometric objects will be constant across exposure times
                 logger.info(f"Loading dark for {readout_exp_time = } and {beam = }")
-                try:
-                    dark_array = self.intermediate_frame_helpers_load_dark_array(
-                        beam, readout_exp_time=readout_exp_time
-                    )
-                except StopIteration:
-                    raise ValueError(f"No matching dark found for {readout_exp_time = } s")
+                dark_array = self.intermediate_frame_helpers_load_dark_array(
+                    beam=beam, readout_exp_time=readout_exp_time
+                )
 
                 if background_array is None:
                     background_array = np.zeros(dark_array.shape)
 
                 for cs_step in range(self.constants.num_cs_steps):
                     local_obj, global_obj = self.reduce_single_step(
                         beam,
@@ -271,28 +269,28 @@
         logger.info(f"Reducing {apm_str}")
         # Get the iterable of objects for this beam, cal seq step and mod state
 
         # Get the headers and arrays as iterables
         tags = [
             VispTag.frame(),
             VispTag.input(),
-            VispTag.task("POLCAL"),
+            VispTag.task_polcal(),
             VispTag.modstate(modstate),
             VispTag.cs_step(cs_step),
             VispTag.readout_exp_time(readout_exp_time),
         ]
         polcal_objs = list(
             self.read(tags=tags, decoder=fits_access_decoder, fits_access_class=VispL0FitsAccess)
         )
         # Grab the 1st header
         avg_inst_pol_cal_header = polcal_objs[0].header
 
         # Average the arrays (this works for a single array as well)
         readout_normalized_arrays = (
-            self.input_frame_loaders_get_beam(o.data, beam=beam) / o.num_raw_frames_per_fpa
+            self.beam_access_get_beam(o.data, beam=beam) / o.num_raw_frames_per_fpa
             for o in polcal_objs
         )
         avg_inst_pol_cal_array = average_numpy_arrays(readout_normalized_arrays)
 
         with self.apm_processing_step(f"Apply basic corrections for {apm_str}"):
             dark_corrected_array = subtract_array_from_arrays(avg_inst_pol_cal_array, dark_array)
```

### Comparing `dkist_processing_visp-2.8.2/dkist_processing_visp/tasks/lamp.py` & `dkist_processing_visp-2.9.0/dkist_processing_visp/tasks/lamp.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 """ViSP lamp calibration task. See :doc:`this page </gain_correction>` for more information."""
 import numpy as np
 from dkist_processing_common.codecs.fits import fits_access_decoder
+from dkist_processing_common.models.task_name import TaskName
 from dkist_processing_common.tasks.mixin.quality import QualityMixin
 from dkist_processing_math.arithmetic import subtract_array_from_arrays
 from dkist_processing_math.statistics import average_numpy_arrays
 from dkist_service_configuration import logger
 
 from dkist_processing_visp.models.tags import VispTag
 from dkist_processing_visp.parsers.visp_l0_fits_access import VispL0FitsAccess
+from dkist_processing_visp.tasks.mixin.beam_access import BeamAccessMixin
 from dkist_processing_visp.tasks.mixin.corrections import CorrectionsMixin
-from dkist_processing_visp.tasks.mixin.input_frame_loaders import InputFrameLoadersMixin
 from dkist_processing_visp.tasks.mixin.intermediate_frame_helpers import (
     IntermediateFrameHelpersMixin,
 )
 from dkist_processing_visp.tasks.visp_base import VispTaskBase
 
 __all__ = ["LampCalibration"]
 
 
 class LampCalibration(
     VispTaskBase,
     CorrectionsMixin,
     IntermediateFrameHelpersMixin,
-    InputFrameLoadersMixin,
+    BeamAccessMixin,
     QualityMixin,
 ):
     """
     Task class for calculation of the averaged lamp gain frame for a VISP calibration run.
 
     Parameters
     ----------
@@ -57,20 +58,17 @@
         """
         with self.apm_task_step(
             f"Generate lamp gains for {self.constants.num_beams} beams and {len(self.constants.lamp_readout_exp_times)} exposure times"
         ):
             for readout_exp_time in self.constants.lamp_readout_exp_times:
                 for beam in range(1, self.constants.num_beams + 1):
                     logger.info(f"Load dark for beam {beam}")
-                    try:
-                        dark_array = self.intermediate_frame_helpers_load_dark_array(
-                            beam=beam, readout_exp_time=readout_exp_time
-                        )
-                    except StopIteration:
-                        raise ValueError(f"No matching dark found for {readout_exp_time = } s")
+                    dark_array = self.intermediate_frame_helpers_load_dark_array(
+                        beam=beam, readout_exp_time=readout_exp_time
+                    )
 
                     for state_num in range(
                         1, self.constants.num_modstates + 1
                     ):  # modulator states go from 1 to n
                         logger.info(
                             f"Calculating average lamp gain for beam {beam}, modulator state {state_num}"
                         )
@@ -82,20 +80,20 @@
                         )
 
         with self.apm_processing_step("Computing and logging quality metrics"):
             no_of_raw_lamp_frames: int = self.scratch.count_all(
                 tags=[
                     VispTag.input(),
                     VispTag.frame(),
-                    VispTag.task("LAMP_GAIN"),
+                    VispTag.task_lamp_gain(),
                 ],
             )
 
             self.quality_store_task_type_counts(
-                task_type="LAMP_GAIN", total_frames=no_of_raw_lamp_frames
+                task_type=TaskName.lamp_gain.value, total_frames=no_of_raw_lamp_frames
             )
 
     def compute_and_write_master_lamp_gain_for_modstate(
         self,
         modstate: int,
         dark_array: np.ndarray,
         beam: int,
@@ -129,35 +127,35 @@
         None
         """
         apm_str = f"{beam = }, {modstate = }, and {readout_exp_time = }"
         # Get the input lamp gain arrays
         tags = [
             VispTag.input(),
             VispTag.frame(),
-            VispTag.task("LAMP_GAIN"),
+            VispTag.task_lamp_gain(),
             VispTag.modstate(modstate),
             VispTag.readout_exp_time(readout_exp_time),
         ]
         input_lamp_gain_objs = self.read(
             tags=tags, decoder=fits_access_decoder, fits_access_class=VispL0FitsAccess
         )
 
         with self.apm_processing_step(f"Computing gain for {apm_str}"):
 
             readout_normalized_arrays = (
-                self.input_frame_loaders_get_beam(o.data, beam=beam) / o.num_raw_frames_per_fpa
+                self.beam_access_get_beam(o.data, beam=beam) / o.num_raw_frames_per_fpa
                 for o in input_lamp_gain_objs
             )
             averaged_gain_data = average_numpy_arrays(readout_normalized_arrays)
 
             dark_corrected_gain_data = next(
                 subtract_array_from_arrays(averaged_gain_data, dark_array)
             )
             filtered_gain_data = self.corrections_mask_hairlines(dark_corrected_gain_data)
 
         with self.apm_writing_step(f"Writing gain array for {apm_str}"):
             self.intermediate_frame_helpers_write_arrays(
                 filtered_gain_data,
                 beam=beam,
-                task="LAMP_GAIN",
+                task=TaskName.lamp_gain.value,
                 modstate=modstate,
             )
```

### Comparing `dkist_processing_visp-2.8.2/dkist_processing_visp/tasks/make_movie_frames.py` & `dkist_processing_visp-2.9.0/dkist_processing_visp/tasks/make_movie_frames.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """Visp make movie frames task."""
 import numpy as np
 from astropy.io import fits
 from astropy.visualization import ZScaleInterval
+from dkist_processing_common.codecs.fits import fits_access_decoder
+from dkist_processing_common.codecs.fits import fits_array_encoder
 from dkist_service_configuration import logger
 
 from dkist_processing_visp.models.tags import VispTag
 from dkist_processing_visp.parsers.visp_l1_fits_access import VispL1FitsAccess
 from dkist_processing_visp.tasks.visp_base import VispTaskBase
 
 __all__ = ["MakeVispMovieFrames"]
@@ -55,23 +57,24 @@
                             tags=[VispTag.frame(), VispTag.output(), VispTag.stokes(stokes_state)]
                         )
                     )
                     if len(stokes_paths) > 0:
                         # Loop over the raster steps in a single scan
                         for raster_step in range(0, self.constants.num_raster_steps):
                             calibrated_frame: VispL1FitsAccess = next(
-                                self.fits_data_read_fits_access(
+                                self.read(
                                     tags=[
                                         VispTag.frame(),
                                         VispTag.output(),
                                         VispTag.stokes(stokes_state),
                                         VispTag.map_scan(map_scan),
                                         VispTag.raster_step(raster_step),
                                     ],
-                                    cls=VispL1FitsAccess,
+                                    decoder=fits_access_decoder,
+                                    fits_access_class=VispL1FitsAccess,
                                 )
                             )
                             data = calibrated_frame.data
                             if self.constants.num_raster_steps == 1:
                                 logger.info(
                                     "Only a single raster step found. Making a spectral movie."
                                 )
@@ -136,16 +139,16 @@
                         ),
                         axis=0,
                     )
                 else:
                     movie_frame_data = stokes_i_data
 
             with self.apm_writing_step(f"Writing movie frame for {map_scan = }"):
-                self.fits_data_write(
-                    hdu_list=fits.HDUList(
-                        [fits.PrimaryHDU(header=header, data=np.asarray(movie_frame_data))]
-                    ),
+                self.write(
+                    data=np.asarray(movie_frame_data),
                     tags=[
                         VispTag.map_scan(map_scan),
                         VispTag.movie_frame(),
                     ],
+                    encoder=fits_array_encoder,
+                    header=header,
                 )
```

### Comparing `dkist_processing_visp-2.8.2/dkist_processing_visp/tasks/mixin/corrections.py` & `dkist_processing_visp-2.9.0/dkist_processing_visp/tasks/mixin/corrections.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.8.2/dkist_processing_visp/tasks/mixin/downsample.py` & `dkist_processing_visp-2.9.0/dkist_processing_visp/tasks/mixin/downsample.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.8.2/dkist_processing_visp/tasks/mixin/intermediate_frame_helpers.py` & `dkist_processing_visp-2.9.0/dkist_processing_visp/tasks/mixin/intermediate_frame_helpers.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,68 +8,126 @@
 from astropy.io import fits
 from dkist_processing_common.codecs.fits import fits_array_decoder
 from dkist_processing_common.codecs.fits import fits_array_encoder
 from dkist_processing_common.models.fits_access import FitsAccessBase
 from dkist_service_configuration import logger
 
 from dkist_processing_visp.models.tags import VispTag
-from dkist_processing_visp.parsers.visp_l0_fits_access import VispL0FitsAccess
 
 
 class IntermediateFrameHelpersMixin:
     """Mixin for methods that support easy loading and writing of intermediate frames."""
 
     F = TypeVar("F", bound=FitsAccessBase)
 
-    def intermediate_frame_helpers_load_intermediate_arrays(
+    def intermediate_frame_helpers_write_arrays(
         self,
+        arrays: Iterable[np.ndarray] | np.ndarray,
+        headers: Iterable[fits.Header] | fits.Header | None = None,
         beam: int | None = None,
-        task: str | None = None,
         modstate: int | None = None,
+        map_scan: int | None = None,
+        raster_step: int | None = None,
         exposure_time: float | None = None,
         readout_exp_time: float | None = None,
-    ) -> Generator[np.ndarray, None, None]:
+        task: str | None = None,
+        task_tag: str | None = None,
+    ) -> None:
         """
-        Yield a generator that produces ndarrays for the requested tags.
+        Write out intermediate files with requested tags.
 
         Parameters
         ----------
+        arrays
+            pass
+
+        headers
+            pass
+
         beam : int
             The current beam being processed
 
-        task : str
-            The task type of the data currently being processed
-
         modstate : int
             The current modulator state
 
+        map_scan : int
+             The current map scan
+
+        raster_step : int
+            The slit step for this step
+
+        task : str
+            The task type of the data currently being processed
+
         exposure_time : float
             The FPA exposure time
 
         readout_exp_time
             Exposure time of a single readout
 
+        file_id:
+            The unique file_id
+
         Returns
         -------
-        Generator
-            Array(s) of loaded intermediate data with requested tags
+        None
         """
-        # See intermediate_frame_helpers_write_arrays for an explanation of how this works, to add new tags *all* that's needed
-        # is to add a kwarg that has the same name as a tag
-        passed_args = locals()
-        tags = [VispTag.intermediate(), VispTag.frame()]
-        for t, v in passed_args.items():
-            if t not in ["self"] and v is not None:
-                tags.append(getattr(VispTag, t)(v))
+        if task_tag is not None and task is not None:
+            raise ValueError("Cannot specify both the raw 'task' and a formatted 'task_tag'.")
+        if task_tag is None and task is None:
+            raise ValueError("Must specify exactly one of raw 'task' or formatted 'task_tag'.")
+
+        if task is not None:
+            task_tag = VispTag.task(task)
+        tags = [VispTag.intermediate(), VispTag.frame(), task_tag]
+
+        for arg, tag_func in zip(
+            [beam, modstate, map_scan, raster_step, exposure_time, readout_exp_time],
+            [
+                VispTag.beam,
+                VispTag.modstate,
+                VispTag.map_scan,
+                VispTag.raster_step,
+                VispTag.exposure_time,
+                VispTag.readout_exp_time,
+            ],
+        ):
+            if arg is not None:
+                tags.append(tag_func(arg))
+
+        arrays = [arrays] if isinstance(arrays, np.ndarray) else arrays
+        if headers is not None:
+            headers = [headers] if isinstance(headers, fits.Header) else headers
+        else:
+            headers = itertools.repeat(None)
+
+        filenames = []
+        for array, header in zip(arrays, headers):
+            written_path = self.write(
+                data=array, header=header, encoder=fits_array_encoder, tags=tags
+            )
+            filenames.append(str(written_path))
+
+        logger.info(f"Wrote intermediate file(s) for {tags = } to {filenames}")
+
+    def intermediate_frame_helpers_load_intermediate_arrays(
+        self, tags: [str]
+    ) -> Generator[np.ndarray, None, None]:
+        """Yield a generator that produces ndarrays for the requested tags."""
+        tags = list(set([VispTag.intermediate(), VispTag.frame()] + tags))
+
+        if self.scratch.count_all(tags=tags) == 0:
+            raise FileNotFoundError(f"No files found matching {tags =}")
 
         yield from self.read(decoder=fits_array_decoder, tags=tags)
 
     def intermediate_frame_helpers_load_dark_array(
         self,
-        beam: int | None = None,
+        *,
+        beam: int,
         exposure_time: float | None = None,
         readout_exp_time: float | None = None,
     ) -> np.ndarray:
         """
         Produce dark ndarrays for the requested tags.
 
         Parameters
@@ -84,46 +142,44 @@
             Exposure time of a single readout
 
         Returns
         -------
         ndarray
             Array of loaded intermediate dark data with requested tags
         """
-        return next(
-            self.intermediate_frame_helpers_load_intermediate_arrays(
-                beam=beam,
-                task="DARK",
-                exposure_time=exposure_time,
-                readout_exp_time=readout_exp_time,
-            )
-        )
+        tags = [VispTag.task_dark(), VispTag.beam(beam)]
 
-    def intermediate_frame_helpers_load_background_array(
-        self,
-        beam: int | None = None,
-    ) -> np.ndarray:
+        if exposure_time is not None:
+            tags.append(VispTag.exposure_time(exposure_time))
+
+        if readout_exp_time is not None:
+            tags.append(VispTag.readout_exp_time(readout_exp_time))
+
+        return next(self.intermediate_frame_helpers_load_intermediate_arrays(tags=tags))
+
+    def intermediate_frame_helpers_load_background_array(self, *, beam: int) -> np.ndarray:
         """
         Produce background light ndarrays for the requested tags.
 
         Parameters
         ----------
         beam : int
             The current beam being processed
 
         Returns
         -------
         ndarray
             Array of loaded intermediate background light data with requested tags
         """
-        return next(
-            self.intermediate_frame_helpers_load_intermediate_arrays(beam=beam, task="BACKGROUND")
-        )
+        tags = [VispTag.task_background(), VispTag.beam(beam)]
+
+        return next(self.intermediate_frame_helpers_load_intermediate_arrays(tags=tags))
 
     def intermediate_frame_helpers_load_lamp_gain_array(
-        self, beam: int | None = None, modstate: int | None = None
+        self, *, beam: int, modstate: int
     ) -> np.ndarray:
         """
         Produce lamp gain ndarrays for the requested tags.
 
         Parameters
         ----------
         beam : int
@@ -133,22 +189,20 @@
 
 
         Returns
         -------
         ndarray
             Array of loaded intermediate lamp gain data with requested tags
         """
-        return next(
-            self.intermediate_frame_helpers_load_intermediate_arrays(
-                beam=beam, task="LAMP_GAIN", modstate=modstate
-            )
-        )
+        tags = [VispTag.task_lamp_gain(), VispTag.beam(beam), VispTag.modstate(modstate)]
+
+        return next(self.intermediate_frame_helpers_load_intermediate_arrays(tags=tags))
 
     def intermediate_frame_helpers_load_solar_gain_array(
-        self, beam: int | None = None, modstate: int | None = None
+        self, *, beam: int, modstate: int
     ) -> np.ndarray:
         """
         Produce solar gain ndarrays for the requested tags.
 
         Parameters
         ----------
         beam : int
@@ -158,119 +212,19 @@
 
 
         Returns
         -------
         ndarray
             Array of loaded intermediate solar gain data with requested tags
         """
-        return next(
-            self.intermediate_frame_helpers_load_intermediate_arrays(
-                beam=beam, task="SOLAR_GAIN", modstate=modstate
-            )
-        )
-
-    def intermediate_frame_helpers_load_demodulated_arrays(
-        self, beam: int | None = None, modstate: int | None = None
-    ) -> Generator[np.ndarray, None, None]:
-        """
-        Produce demodulated arrays for the requested tags.
-
-        Parameters
-        ----------
-        beam : int
-            The current beam being processed
-        modstate : int
-            The current modulator state
-
-
-        Returns
-        -------
-        Generator
-            Array of loaded intermediate demodulated data with requested tags
-        """
-        return self.intermediate_frame_helpers_load_intermediate_arrays(
-            beam=beam, task="DEMODULATED_ARRAYS", modstate=modstate
-        )
+        tags = [VispTag.task_solar_gain(), VispTag.beam(beam), VispTag.modstate(modstate)]
 
-    def intermediate_frame_helpers_write_arrays(
-        self,
-        arrays: Iterable[np.ndarray] | np.ndarray,
-        headers: Iterable[fits.Header] | fits.Header | None = None,
-        beam: int | None = None,
-        modstate: int | None = None,
-        map_scan: int | None = None,
-        raster_step: int | None = None,
-        task: str | None = None,
-        exposure_time: float | None = None,
-        readout_exp_time: float | None = None,
-        file_id: str | None = None,
-    ) -> None:
-        """
-        Write out intermediate files with requested tags.
-
-        Parameters
-        ----------
-        arrays
-            pass
+        return next(self.intermediate_frame_helpers_load_intermediate_arrays(tags=tags))
 
-        headers
-            pass
-
-        beam : int
-            The current beam being processed
-
-        modstate : int
-            The current modulator state
-
-        map_scan : int
-             The current map scan
-
-        raster_step : int
-            The slit step for this step
-
-        task : str
-            The task type of the data currently being processed
-
-        exposure_time : float
-            The FPA exposure time
-
-        readout_exp_time
-            Exposure time of a single readout
-
-        file_id:
-            The unique file_id
-
-        Returns
-        -------
-        None
-        """
-        # To add a new tag all you need to do is add a kwarg that has the same name as a tag. That's it!
-        ## Construct the tags based on which optional parameters were passed
-        passed_args = locals()
-        tags = [VispTag.intermediate(), VispTag.frame()]
-        for t, v in passed_args.items():
-            # Look at all the arguments passed to this function, ignore those that aren't tags
-            # and update tags with those that aren't None
-            if t not in ["self", "arrays", "headers"] and v is not None:
-                tags.append(getattr(VispTag, t)(v))
-
-        arrays = [arrays] if isinstance(arrays, np.ndarray) else arrays
-        if headers is not None:
-            headers = [headers] if isinstance(headers, fits.Header) else headers
-        else:
-            headers = itertools.repeat(None)
-
-        filenames = []
-        for array, header in zip(arrays, headers):
-            path = self.write(data=array, header=header, encoder=fits_array_encoder, tags=tags)
-            filenames.append(str(path))
-
-        logger.info(f"Wrote intermediate file for {tags = } to {filenames}")
-
-    def intermediate_frame_helpers_load_demod_matrices(self, beam_num: int) -> np.ndarray:
+    def intermediate_frame_helpers_load_demod_matrices(self, *, beam_num: int) -> np.ndarray:
         """
         Load demodulated matrices.
 
         Parameters
         ----------
         beam_num : int
             The current beam being processed
@@ -278,64 +232,41 @@
 
         Returns
         -------
         ndarray
             Demodulated matrix data
         """
         tags = [
-            VispTag.intermediate(),
-            VispTag.task("DEMOD_MATRICES"),
+            VispTag.task_demodulation_matrices(),
             VispTag.beam(beam_num),
         ]
-        array = next(self.read(decoder=fits_array_decoder, tags=tags))
+        array = next(self.intermediate_frame_helpers_load_intermediate_arrays(tags=tags))
         return array
 
-    def intermediate_frame_helpers_fits_access_generator(
-        self,
-        tags: Iterable[str],
-    ) -> Generator[F, None, None]:
-        """
-        Load a generator of intermediate frames.
-
-        Parameters
-        ----------
-        tags : str
-            Requested tags for loading data
-
-        Returns
-        -------
-        Generator
-            generator of intermediate frames
-        """
-        tags += [VispTag.intermediate(), VispTag.frame()]
-        frame_generator = self.fits_data_read_fits_access(tags, cls=VispL0FitsAccess)
-        return frame_generator
-
-    def intermediate_frame_helpers_load_angle(self, beam: int) -> float:
+    def intermediate_frame_helpers_load_angle(self, *, beam: int) -> float:
         """
         Load geometric angle for a given frame (beam).
 
         Parameters
         ----------
         beam : int
             The current beam being processed
 
         Returns
         -------
         float
             angle
         """
-        angle_array = next(
-            self.intermediate_frame_helpers_load_intermediate_arrays(
-                beam=beam, task="GEOMETRIC_ANGLE"
-            )
-        )
+        tags = [VispTag.task_geometric_angle(), VispTag.beam(beam)]
+        angle_array = next(self.intermediate_frame_helpers_load_intermediate_arrays(tags=tags))
         return angle_array[0]
 
-    def intermediate_frame_helpers_load_state_offset(self, beam: int, modstate: int) -> np.ndarray:
+    def intermediate_frame_helpers_load_state_offset(
+        self, *, beam: int, modstate: int
+    ) -> np.ndarray:
         """
         Load state offset for a given beam and modstate.
 
         Parameters
         ----------
         beam : int
             The current beam being processed
@@ -344,35 +275,29 @@
 
 
         Returns
         -------
         ndarray
             state offset array
         """
-        offset = next(
-            self.intermediate_frame_helpers_load_intermediate_arrays(
-                beam=beam, task="GEOMETRIC_OFFSET", modstate=modstate
-            )
-        )
+        tags = [VispTag.task_geometric_offset(), VispTag.beam(beam), VispTag.modstate(modstate)]
+        offset = next(self.intermediate_frame_helpers_load_intermediate_arrays(tags=tags))
         return offset
 
-    def intermediate_frame_helpers_load_spec_shift(self, beam: int) -> np.ndarray:
+    def intermediate_frame_helpers_load_spec_shift(self, *, beam: int) -> np.ndarray:
         """
         Load spectral shift for a given beam.
 
         Parameters
         ----------
         beam : int
             The current beam being processed
 
 
         Returns
         -------
         ndarray
             spectral shift array
         """
-        shifts = next(
-            self.intermediate_frame_helpers_load_intermediate_arrays(
-                beam=beam, task="GEOMETRIC_SPEC_SHIFTS"
-            )
-        )
+        tags = [VispTag.task_geometric_sepectral_shifts(), VispTag.beam(beam)]
+        shifts = next(self.intermediate_frame_helpers_load_intermediate_arrays(tags=tags))
         return shifts
```

### Comparing `dkist_processing_visp-2.8.2/dkist_processing_visp/tasks/mixin/line_zones.py` & `dkist_processing_visp-2.9.0/dkist_processing_visp/tasks/mixin/line_zones.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.8.2/dkist_processing_visp/tasks/parse.py` & `dkist_processing_visp-2.9.0/dkist_processing_visp/tasks/parse.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 """ViSP parse task."""
 from typing import TypeVar
 
 from dkist_processing_common.models.flower_pot import Stem
+from dkist_processing_common.models.task_name import TaskName
 from dkist_processing_common.parsers.cs_step import CSStepFlower
 from dkist_processing_common.parsers.cs_step import NumCSStepBud
+from dkist_processing_common.parsers.task import parse_header_ip_task_with_gains
+from dkist_processing_common.parsers.task import TaskTypeFlower
 from dkist_processing_common.parsers.time import ExposureTimeFlower
+from dkist_processing_common.parsers.time import ObsIpStartTimeBud
 from dkist_processing_common.parsers.time import ReadoutExpTimeFlower
 from dkist_processing_common.parsers.time import TaskExposureTimesBud
 from dkist_processing_common.parsers.time import TaskReadoutExpTimesBud
 from dkist_processing_common.parsers.unique_bud import UniqueBud
+from dkist_processing_common.parsers.wavelength import ObserveWavelengthBud
 from dkist_processing_common.tasks import ParseL0InputDataBase
 from dkist_processing_common.tasks.mixin.input_dataset import InputDatasetMixin
 
 from dkist_processing_visp.models.constants import VispBudName
-from dkist_processing_visp.models.parameters import VispParameters
+from dkist_processing_visp.models.parameters import VispParsingParameters
 from dkist_processing_visp.parsers.map_repeats import MapScanFlower
 from dkist_processing_visp.parsers.map_repeats import NumMapScansBud
 from dkist_processing_visp.parsers.modulator_states import ModulatorStateFlower
 from dkist_processing_visp.parsers.modulator_states import NumberModulatorStatesBud
 from dkist_processing_visp.parsers.polarimeter_mode import PolarimeterModeBud
 from dkist_processing_visp.parsers.raster_step import RasterScanStepFlower
 from dkist_processing_visp.parsers.raster_step import TotalRasterStepsBud
-from dkist_processing_visp.parsers.task import parse_header_ip_task
-from dkist_processing_visp.parsers.task import VispTaskTypeFlower
-from dkist_processing_visp.parsers.time import ObsIpStartTimeBud
+from dkist_processing_visp.parsers.time import DarkReadoutExpTimePickyBud
+from dkist_processing_visp.parsers.time import NonDarkTaskReadoutExpTimesBud
 from dkist_processing_visp.parsers.visp_l0_fits_access import VispL0FitsAccess
-from dkist_processing_visp.parsers.wavelength import ObserveWavelengthBud
 
 S = TypeVar("S", bound=Stem)
 __all__ = ["ParseL0VispInputData"]
 
 
 class ParseL0VispInputData(ParseL0InputDataBase, InputDatasetMixin):
     """
@@ -53,15 +56,15 @@
         workflow_version: str,
     ):
         super().__init__(
             recipe_run_id=recipe_run_id,
             workflow_name=workflow_name,
             workflow_version=workflow_version,
         )
-        self.parameters = VispParameters(self.input_dataset_parameters)
+        self.parameters = VispParsingParameters(self.input_dataset_parameters)
 
     @property
     def fits_parsing_class(self):
         """FITS access class to use in this task."""
         return VispL0FitsAccess
 
     @property
@@ -71,64 +74,66 @@
             NumMapScansBud(),
             TotalRasterStepsBud(),
             NumCSStepBud(self.parameters.max_cs_step_time_sec),
             ObsIpStartTimeBud(),
             NumberModulatorStatesBud(),
             ObserveWavelengthBud(),
             PolarimeterModeBud(),
+            NonDarkTaskReadoutExpTimesBud(),
+            DarkReadoutExpTimePickyBud(),
             TaskExposureTimesBud(
                 stem_name=VispBudName.lamp_exposure_times.value,
-                ip_task_type="LAMP_GAIN",
-                header_task_parsing_func=parse_header_ip_task,
+                ip_task_type=TaskName.lamp_gain.value,
+                header_task_parsing_func=parse_header_ip_task_with_gains,
             ),
             TaskExposureTimesBud(
                 stem_name=VispBudName.solar_exposure_times.value,
-                ip_task_type="SOLAR_GAIN",
-                header_task_parsing_func=parse_header_ip_task,
+                ip_task_type=TaskName.solar_gain.value,
+                header_task_parsing_func=parse_header_ip_task_with_gains,
             ),
             TaskExposureTimesBud(
                 stem_name=VispBudName.observe_exposure_times.value,
-                ip_task_type="OBSERVE",
-                header_task_parsing_func=parse_header_ip_task,
+                ip_task_type=TaskName.observe.value,
+                header_task_parsing_func=parse_header_ip_task_with_gains,
             ),
             TaskExposureTimesBud(
                 stem_name=VispBudName.polcal_exposure_times.value,
-                ip_task_type="POLCAL",
-                header_task_parsing_func=parse_header_ip_task,
+                ip_task_type=TaskName.polcal.value,
+                header_task_parsing_func=parse_header_ip_task_with_gains,
             ),
             TaskReadoutExpTimesBud(
                 stem_name=VispBudName.lamp_readout_exp_times.value,
-                ip_task_type="LAMP_GAIN",
-                header_task_parsing_func=parse_header_ip_task,
+                ip_task_type=TaskName.lamp_gain.value,
+                header_task_parsing_func=parse_header_ip_task_with_gains,
             ),
             TaskReadoutExpTimesBud(
                 stem_name=VispBudName.solar_readout_exp_times.value,
-                ip_task_type="SOLAR_GAIN",
-                header_task_parsing_func=parse_header_ip_task,
+                ip_task_type=TaskName.solar_gain.value,
+                header_task_parsing_func=parse_header_ip_task_with_gains,
             ),
             TaskReadoutExpTimesBud(
                 stem_name=VispBudName.observe_readout_exp_times.value,
-                ip_task_type="OBSERVE",
-                header_task_parsing_func=parse_header_ip_task,
+                ip_task_type=TaskName.observe.value,
+                header_task_parsing_func=parse_header_ip_task_with_gains,
             ),
             TaskReadoutExpTimesBud(
                 stem_name=VispBudName.polcal_readout_exp_times.value,
-                ip_task_type="POLCAL",
-                header_task_parsing_func=parse_header_ip_task,
+                ip_task_type=TaskName.polcal.value,
+                header_task_parsing_func=parse_header_ip_task_with_gains,
             ),
             UniqueBud(constant_name=VispBudName.axis_1_type.value, metadata_key="axis_1_type"),
             UniqueBud(constant_name=VispBudName.axis_2_type.value, metadata_key="axis_2_type"),
             UniqueBud(constant_name=VispBudName.axis_3_type.value, metadata_key="axis_3_type"),
         ]
 
     @property
     def tag_flowers(self) -> list[S]:
         """Add ViSP specific tags to common tags."""
         return super().tag_flowers + [
             CSStepFlower(max_cs_step_time_sec=self.parameters.max_cs_step_time_sec),
             MapScanFlower(),
-            VispTaskTypeFlower(),
+            TaskTypeFlower(header_task_parsing_func=parse_header_ip_task_with_gains),
             RasterScanStepFlower(),
             ModulatorStateFlower(),
             ExposureTimeFlower(),
             ReadoutExpTimeFlower(),
         ]
```

### Comparing `dkist_processing_visp-2.8.2/dkist_processing_visp/tasks/quality_metrics.py` & `dkist_processing_visp-2.9.0/dkist_processing_visp/tasks/quality_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """ViSP quality metrics task."""
 from dataclasses import dataclass
 from dataclasses import field
 
 import numpy as np
 from astropy.time import Time
+from dkist_processing_common.codecs.fits import fits_access_decoder
 from dkist_processing_common.parsers.quality import L1QualityFitsAccess
 from dkist_processing_common.tasks import QualityL0Metrics
 from dkist_processing_common.tasks.mixin.quality import QualityMixin
 
 from dkist_processing_visp.models.constants import VispConstants
 from dkist_processing_visp.models.tags import VispTag
 from dkist_processing_visp.tasks.visp_base import VispTaskBase
@@ -116,43 +117,45 @@
                     polarization_data.U_sensitivity,
                     polarization_data.V_sensitivity,
                 ]
                 for step in range(0, self.constants.num_raster_steps):
 
                     # grab stokes I data
                     stokesI_frame = next(
-                        self.fits_data_read_fits_access(
+                        self.read(
                             tags=[
                                 VispTag.output(),
                                 VispTag.frame(),
                                 VispTag.raster_step(step),
                                 VispTag.map_scan(map_scan),
                                 VispTag.stokes("I"),
                             ],
-                            cls=L1QualityFitsAccess,
+                            decoder=fits_access_decoder,
+                            fits_access_class=L1QualityFitsAccess,
                         )
                     )
                     stokesI_med = np.nanmedian(stokesI_frame.data)
                     polarization_data.datetimes.append(Time(stokesI_frame.time_obs).mjd)
 
                     # grab other stokes data and find and store RMS noise
                     for stokes_param, data_list in zip(
                         ("I", "Q", "U", "V"), poldata_noise_list_list
                     ):
                         try:
                             stokes_frame = next(
-                                self.fits_data_read_fits_access(
+                                self.read(
                                     tags=[
                                         VispTag.output(),
                                         VispTag.frame(),
                                         VispTag.raster_step(step),
                                         VispTag.map_scan(map_scan),
                                         VispTag.stokes(stokes_param),
                                     ],
-                                    cls=L1QualityFitsAccess,
+                                    decoder=fits_access_decoder,
+                                    fits_access_class=L1QualityFitsAccess,
                                 )
                             )
                         except StopIteration:
                             # This stokes parameter doesn't exist. No big deal.
                             continue
 
                         # compute sensitivity for this Stokes parameter
@@ -181,17 +184,18 @@
 
     def compute_noise(self):
         """Compute noise in data."""
         with self.apm_processing_step("Calculating L1 ViSP noise metrics"):
             for stokes in ["I", "Q", "U", "V"]:
                 tags = [VispTag.output(), VispTag.frame(), VispTag.stokes(stokes)]
                 if self.scratch.count_all(tags=tags) > 0:
-                    frames = self.fits_data_read_fits_access(
+                    frames = self.read(
                         tags=tags,
-                        cls=L1QualityFitsAccess,
+                        decoder=fits_access_decoder,
+                        fits_access_class=L1QualityFitsAccess,
                     )
                     noise_values = []
                     datetimes = []
                     for frame in frames:
                         noise_values.append(self.avg_noise(frame.data))
                         datetimes.append(frame.time_obs)
                     self.quality_store_noise(
```

### Comparing `dkist_processing_visp-2.8.2/dkist_processing_visp/tasks/science.py` & `dkist_processing_visp-2.9.0/dkist_processing_visp/tasks/science.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,25 +5,28 @@
 from typing import Iterable
 
 import numpy as np
 from astropy.io import fits
 from astropy.time import Time
 from astropy.time import TimeDelta
 from dkist_processing_common.codecs.fits import fits_access_decoder
+from dkist_processing_common.codecs.fits import fits_hdulist_encoder
+from dkist_processing_common.models.task_name import TaskName
 from dkist_processing_common.tasks.mixin.quality import QualityMixin
 from dkist_processing_math.arithmetic import divide_arrays_by_array
 from dkist_processing_math.arithmetic import subtract_array_from_arrays
+from dkist_processing_math.linear_algebra import nd_left_matrix_multiply
 from dkist_processing_math.statistics import average_numpy_arrays
 from dkist_processing_pac.optics.telescope import Telescope
 from dkist_service_configuration import logger
 
 from dkist_processing_visp.models.tags import VispTag
 from dkist_processing_visp.parsers.visp_l0_fits_access import VispL0FitsAccess
+from dkist_processing_visp.tasks.mixin.beam_access import BeamAccessMixin
 from dkist_processing_visp.tasks.mixin.corrections import CorrectionsMixin
-from dkist_processing_visp.tasks.mixin.input_frame_loaders import InputFrameLoadersMixin
 from dkist_processing_visp.tasks.mixin.intermediate_frame_helpers import (
     IntermediateFrameHelpersMixin,
 )
 from dkist_processing_visp.tasks.visp_base import VispTaskBase
 
 __all__ = ["ScienceCalibration"]
 
@@ -81,15 +84,15 @@
 
         return x_slice, y_slice
 
 
 class ScienceCalibration(
     VispTaskBase,
     IntermediateFrameHelpersMixin,
-    InputFrameLoadersMixin,
+    BeamAccessMixin,
     CorrectionsMixin,
     QualityMixin,
 ):
     """
     Task class for Visp science calibration of polarized and non-polarized data.
 
     Parameters
@@ -129,20 +132,20 @@
             self.process_frames(calibrations=calibrations)
 
         with self.apm_processing_step("Computing and logging quality metrics"):
             no_of_raw_science_frames: int = self.scratch.count_all(
                 tags=[
                     VispTag.input(),
                     VispTag.frame(),
-                    VispTag.task("OBSERVE"),
+                    VispTag.task_observe(),
                 ],
             )
 
             self.quality_store_task_type_counts(
-                task_type="OBSERVE", total_frames=no_of_raw_science_frames
+                task_type=TaskName.observe.value, total_frames=no_of_raw_science_frames
             )
 
     def collect_calibration_objects(self) -> CalibrationCollection:
         """
         Collect *all* calibration for all beams, modstates, and exposure times.
 
         Doing this once here prevents lots of reads as we reduce the science data.
@@ -155,34 +158,33 @@
         spec_shift_dict = dict()
         demod_dict = dict() if self.constants.correct_for_polarization else None
 
         for beam in range(1, self.constants.num_beams + 1):
             for readout_exp_time in self.constants.observe_readout_exp_times:
                 # Dark
                 ######
-                try:
-                    dark_array = self.intermediate_frame_helpers_load_dark_array(
-                        beam=beam, readout_exp_time=readout_exp_time
-                    )
-                except StopIteration:
-                    raise ValueError(f"No matching dark found for {readout_exp_time = } s")
+                dark_array = self.intermediate_frame_helpers_load_dark_array(
+                    beam=beam, readout_exp_time=readout_exp_time
+                )
 
                 dark_dict[VispTag.beam(beam)][
                     VispTag.readout_exp_time(readout_exp_time)
                 ] = dark_array
 
             # Residual background light
             ###########################
             try:
                 background_dict[
                     VispTag.beam(beam)
                 ] = self.intermediate_frame_helpers_load_background_array(beam=beam)
-            except StopIteration:
+            except FileNotFoundError as e:
                 if self.constants.correct_for_polarization and self.parameters.background_on:
-                    raise ValueError(f"No matching background light found for {beam = }")
+                    raise FileNotFoundError(
+                        f"No matching background light found for {beam = }"
+                    ) from e
                 background_dict[VispTag.beam(beam)] = np.zeros(dark_array.shape)
 
             # Angle
             #######
             angle_dict[VispTag.beam(beam)] = self.intermediate_frame_helpers_load_angle(beam=beam)
 
             # Spec shifts
@@ -317,15 +319,15 @@
                     calibrations=calibrations,
                 )
                 # Add this result to the 3D stack
                 array_stack[:, :, modstate - 1] = corrected_array
                 header_stack.append(corrected_header)
 
         with self.apm_processing_step("Applying instrument polarization correction"):
-            intermediate_array = self.nd_left_matrix_multiply(
+            intermediate_array = nd_left_matrix_multiply(
                 vector_stack=array_stack,
                 matrix_stack=calibrations.demod_matrices[VispTag.beam(beam)],
             )
             intermediate_header = self._compute_date_keys(header_stack)
 
         return intermediate_array, intermediate_header
 
@@ -490,15 +492,15 @@
         spec_shift = calibrations.spec_shift[VispTag.beam(beam)]
         state_offset = calibrations.state_offset[VispTag.beam(beam)][VispTag.modstate(modstate)]
 
         # Grab the input observe frame
         tags = [
             VispTag.input(),
             VispTag.frame(),
-            VispTag.task("OBSERVE"),
+            VispTag.task_observe(),
             VispTag.modstate(modstate),
             VispTag.map_scan(map_scan),
             VispTag.raster_step(raster_step),
             VispTag.readout_exp_time(readout_exp_time),
         ]
         observe_object_list = list(
             self.read(tags=tags, decoder=fits_access_decoder, fits_access_class=VispL0FitsAccess)
@@ -509,15 +511,15 @@
                 f"Found more than one observe frame for {map_scan = }, {raster_step = }, {modstate = }, "
                 f"and {readout_exp_time = }. This should NEVER have happened!"
             )
         observe_object = observe_object_list[0]
 
         # Split the beam we want
         readout_normalized_data = observe_object.data / observe_object.num_raw_frames_per_fpa
-        observe_data = self.input_frame_loaders_get_beam(readout_normalized_data, beam=beam)
+        observe_data = self.beam_access_get_beam(readout_normalized_data, beam=beam)
 
         # Dark correction
         dark_corrected_array = next(subtract_array_from_arrays(observe_data, dark_array))
 
         # Residual background correction
         background_corrected_array = next(
             subtract_array_from_arrays(dark_corrected_array, background_array)
@@ -536,46 +538,14 @@
         # Geo correction pt 2: spectral curvature
         spectral_corrected_array = next(
             self.corrections_remove_spec_geometry(geo_corrected_array, spec_shift)
         )
 
         return spectral_corrected_array, observe_object.header
 
-    @staticmethod
-    def nd_left_matrix_multiply(
-        *, vector_stack: np.ndarray, matrix_stack: np.ndarray
-    ) -> np.ndarray:
-        """
-        Left-multiply an arbitrarily dimensioned stack of vectors by a similarly dimensioned stack of matrices.
-
-        In math:
-
-            result = M @ v
-
-        where M is a matrix with dimensions ([n1, ...nn], D1, D2)
-        and v is a vector with dimensions ([n1, ...nn], D2).
-
-        The higher-order dimensions (n1, ...nn) can be anything (or nothing), but they must be the same for M and v.
-
-        Parameters
-        ----------
-        vector_stack : np.ndarray
-            ([n1, ...nn], D2) ND stack of vectors with length D2
-
-        matrix_stack : np.ndarray
-            ([n1, ...nn], D1, D2) ND stack of matrices with shape (D1, D2)
-
-
-        Returns
-        -------
-        np.ndarray
-            ([n1, ...nn], D1) ND stack of vectors with length D1
-        """
-        return np.sum(matrix_stack * vector_stack[:, :, None, :], axis=3)
-
     def telescope_polarization_correction(
         self,
         inst_demod_obj: VispL0FitsAccess,
     ) -> VispL0FitsAccess:
         """
         Apply a telescope polarization correction.
 
@@ -590,15 +560,15 @@
         -------
         FitsAccess object with telescope corrections applied
         """
         tm = Telescope.from_fits_access(inst_demod_obj)
         mueller_matrix = tm.generate_inverse_telescope_model(
             M12=True, rotate_to_fixed_SDO_HINODE_polarized_frame=True, swap_UV_signs=True
         )
-        inst_demod_obj.data = self.nd_left_matrix_multiply(
+        inst_demod_obj.data = nd_left_matrix_multiply(
             vector_stack=inst_demod_obj.data, matrix_stack=mueller_matrix
         )
         return inst_demod_obj
 
     @staticmethod
     def _compute_date_keys(headers: Iterable[fits.Header] | fits.Header) -> fits.Header:
         """
@@ -732,11 +702,11 @@
             VispTag.calibrated(),
             VispTag.frame(),
             VispTag.stokes(stokes),
             VispTag.raster_step(raster_step),
             VispTag.map_scan(map_scan),
         ]
         hdul = fits.HDUList([fits.PrimaryHDU(), fits.CompImageHDU(header=header, data=data)])
-        self.fits_data_write(hdu_list=hdul, tags=tags)
+        self.write(data=hdul, tags=tags, encoder=fits_hdulist_encoder)
 
         filename = next(self.read(tags=tags))
         logger.info(f"Wrote intermediate file for {tags = } to {filename}")
```

### Comparing `dkist_processing_visp-2.8.2/dkist_processing_visp/tasks/solar.py` & `dkist_processing_visp-2.9.0/dkist_processing_visp/tasks/solar.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 """ViSP solar calibration task. See :doc:`this page </gain_correction>` for more information."""
 import numpy as np
 import scipy.ndimage as spnd
 import scipy.optimize as spo
 from dkist_processing_common.codecs.fits import fits_access_decoder
 from dkist_processing_common.codecs.fits import fits_array_encoder
+from dkist_processing_common.models.task_name import TaskName
 from dkist_processing_common.tasks.mixin.quality import QualityMixin
 from dkist_processing_math.arithmetic import divide_arrays_by_array
 from dkist_processing_math.arithmetic import subtract_array_from_arrays
 from dkist_processing_math.statistics import average_numpy_arrays
 from dkist_service_configuration import logger
 
 from dkist_processing_visp.models.tags import VispTag
 from dkist_processing_visp.parsers.visp_l0_fits_access import VispL0FitsAccess
+from dkist_processing_visp.tasks.mixin.beam_access import BeamAccessMixin
 from dkist_processing_visp.tasks.mixin.corrections import CorrectionsMixin
-from dkist_processing_visp.tasks.mixin.input_frame_loaders import InputFrameLoadersMixin
 from dkist_processing_visp.tasks.mixin.intermediate_frame_helpers import (
     IntermediateFrameHelpersMixin,
 )
 from dkist_processing_visp.tasks.mixin.line_zones import LineZonesMixin
 from dkist_processing_visp.tasks.visp_base import VispTaskBase
 
 __all__ = ["SolarCalibration"]
 
 
 class SolarCalibration(
     VispTaskBase,
     IntermediateFrameHelpersMixin,
-    InputFrameLoadersMixin,
+    BeamAccessMixin,
     CorrectionsMixin,
     QualityMixin,
     LineZonesMixin,
 ):
     """
     Task class for generating Solar Gain images for each beam/modstate.
 
@@ -164,20 +165,20 @@
                     )
 
         with self.apm_processing_step("Computing and logging quality metrics"):
             no_of_raw_solar_frames: int = self.scratch.count_all(
                 tags=[
                     VispTag.input(),
                     VispTag.frame(),
-                    VispTag.task("SOLAR_GAIN"),
+                    VispTag.task_solar_gain(),
                 ],
             )
 
             self.quality_store_task_type_counts(
-                task_type="SOLAR_GAIN", total_frames=no_of_raw_solar_frames
+                task_type=TaskName.solar_gain.value, total_frames=no_of_raw_solar_frames
             )
 
     def unshifted_geo_corrected_modstate_data(self, beam: int, modstate: int) -> np.ndarray:
         """
         Array for a single beam/modstate that has dark, lamp, angle, and state offset corrections.
 
         Parameters
@@ -191,17 +192,16 @@
 
         Returns
         -------
         np.ndarray
             Array with dark signal, lamp signal, angle and state offset removed
 
         """
-        array_generator = self.intermediate_frame_helpers_load_intermediate_arrays(
-            beam=beam, task="SC_GEO_NOSHIFT", modstate=modstate
-        )
+        tags = [VispTag.task("SC_GEO_NOSHIFT"), VispTag.beam(beam), VispTag.modstate(modstate)]
+        array_generator = self.intermediate_frame_helpers_load_intermediate_arrays(tags=tags)
         return next(array_generator)
 
     def geo_corrected_modstate_data(self, beam: int, modstate: int) -> np.ndarray:
         """
         Array for a single beam/modstate that has dark, lamp, and ALL of the geometric corrects.
 
         Parameters
@@ -214,30 +214,28 @@
 
 
         Returns
         -------
         np.ndarray
             Array with dark signal, and lamp signal removed, and all geometric corrections made
         """
-        array_generator = self.intermediate_frame_helpers_load_intermediate_arrays(
-            beam=beam, task="SC_GEO_ALL", modstate=modstate
-        )
+        tags = [VispTag.task("SC_GEO_ALL"), VispTag.beam(beam), VispTag.modstate(modstate)]
+        array_generator = self.intermediate_frame_helpers_load_intermediate_arrays(tags=tags)
         return next(array_generator)
 
     def lamp_corrected_modstate_data(self, beam: int, modstate: int) -> np.ndarray:
         """
         Array for a single beam/modstate that has dark, background, and lamp gain applied.
 
         This is used to refine the final shifts in the re-distorted characteristic spectra. Having the lamp gain applied
         removes large optical features that would otherwise pollute the match to the characteristic spectra (which has
         no optical features).
         """
-        array_generator = self.intermediate_frame_helpers_load_intermediate_arrays(
-            beam=beam, task="SC_LAMP_CORR", modstate=modstate
-        )
+        tags = [VispTag.task("SC_LAMP_CORR"), VispTag.beam(beam), VispTag.modstate(modstate)]
+        array_generator = self.intermediate_frame_helpers_load_intermediate_arrays(tags=tags)
         return next(array_generator)
 
     def bg_corrected_modstate_data(self, beam: int, modstate: int) -> np.ndarray:
         """
         Array for a single beam/modstate that has only has dark and background corrects applied.
 
         Parameters
@@ -250,17 +248,16 @@
 
 
         Returns
         -------
         np.ndarray
             Array with dark and background signals removed
         """
-        array_generator = self.intermediate_frame_helpers_load_intermediate_arrays(
-            beam=beam, task="SC_BG_ONLY", modstate=modstate
-        )
+        tags = [VispTag.task("SC_BG_ONLY"), VispTag.beam(beam), VispTag.modstate(modstate)]
+        array_generator = self.intermediate_frame_helpers_load_intermediate_arrays(tags=tags)
         return next(array_generator)
 
     def do_initial_corrections(self, beam: int, modstate: int) -> None:
         """
         Do dark, lamp, and geometric corrections for all data that will be used.
 
         At two intermediate points the current arrays are saved because they'll be needed by various helpers:
@@ -281,47 +278,46 @@
 
 
         Returns
         -------
         None
         """
         for readout_exp_time in self.constants.solar_readout_exp_times:
-            try:
-                dark_array = self.intermediate_frame_helpers_load_dark_array(
-                    beam=beam, readout_exp_time=readout_exp_time
-                )
-            except StopIteration:
-                raise ValueError(f"No matching dark found for {readout_exp_time = } s")
+            dark_array = self.intermediate_frame_helpers_load_dark_array(
+                beam=beam, readout_exp_time=readout_exp_time
+            )
 
             try:
                 background_array = self.intermediate_frame_helpers_load_background_array(beam=beam)
-            except StopIteration:
+            except FileNotFoundError as e:
                 if self.constants.correct_for_polarization and self.parameters.background_on:
-                    raise ValueError(f"No matching background light found for {beam = }")
+                    raise FileNotFoundError(
+                        f"No matching background light found for {beam = }"
+                    ) from e
 
                 logger.info("Skipping background light correction")
                 background_array = np.zeros(dark_array.shape)
 
             logger.info(
                 f"Doing dark, background, lamp, and geo corrections for {beam=} and {modstate=}"
             )
             ## Load frames
             tags = [
                 VispTag.input(),
                 VispTag.frame(),
-                VispTag.task("SOLAR_GAIN"),
+                VispTag.task_solar_gain(),
                 VispTag.modstate(modstate),
                 VispTag.readout_exp_time(readout_exp_time),
             ]
             input_solar_gain_objs = self.read(
                 tags=tags, decoder=fits_access_decoder, fits_access_class=VispL0FitsAccess
             )
 
             readout_normalized_arrays = (
-                self.input_frame_loaders_get_beam(o.data, beam=beam) / o.num_raw_frames_per_fpa
+                self.beam_access_get_beam(o.data, beam=beam) / o.num_raw_frames_per_fpa
                 for o in input_solar_gain_objs
             )
 
             ## Average
             avg_solar_array = average_numpy_arrays(readout_normalized_arrays)
 
             ## Dark correction
@@ -578,15 +574,15 @@
 
         Returns
         -------
         None
         """
         logger.info(f"Writing final SolarGain for {beam=} and {modstate=}")
         self.intermediate_frame_helpers_write_arrays(
-            arrays=gain_array, beam=beam, modstate=modstate, task="SOLAR_GAIN"
+            arrays=gain_array, beam=beam, modstate=modstate, task=TaskName.solar_gain.value
         )
 
     @staticmethod
     def refine_shift(
         spec: np.ndarray, target_spec: np.ndarray, zones: list[tuple[int, int]], x_init: float
     ) -> float:
         """
```

### Comparing `dkist_processing_visp-2.8.2/dkist_processing_visp/tasks/visp_base.py` & `dkist_processing_visp-2.9.0/dkist_processing_visp/tasks/visp_base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 """ViSP base class."""
 from abc import ABC
 
 from dkist_processing_common.tasks import WorkflowTaskBase
-from dkist_processing_common.tasks.mixin.fits import FitsDataMixin
 from dkist_processing_common.tasks.mixin.input_dataset import InputDatasetMixin
 
 from dkist_processing_visp.models.constants import VispConstants
 from dkist_processing_visp.models.parameters import VispParameters
 
 
-class VispTaskBase(WorkflowTaskBase, FitsDataMixin, InputDatasetMixin, ABC):
+class VispTaskBase(WorkflowTaskBase, InputDatasetMixin, ABC):
     """
     Task class for base ViSP tasks.
 
     Parameters
     ----------
     recipe_run_id : int
         id of the recipe run used to identify the workflow run this task is part of
```

### Comparing `dkist_processing_visp-2.8.2/dkist_processing_visp/tasks/write_l1.py` & `dkist_processing_visp-2.9.0/dkist_processing_visp/tasks/write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.8.2/dkist_processing_visp/tests/local_trial_workflows/l0_to_l1.py` & `dkist_processing_visp-2.9.0/dkist_processing_visp/tests/local_trial_workflows/l0_to_l1.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from pathlib import Path
 from random import randint
 from unittest.mock import patch
 
 from astropy.io import fits
 from dkist_header_validator import spec122_validator
 from dkist_header_validator import spec214_validator
+from dkist_processing_common.codecs.fits import fits_access_decoder
 from dkist_processing_common.manual import ManualProcessing
 from dkist_processing_common.tasks import QualityL1Metrics
 from dkist_processing_common.tasks import WorkflowTaskBase
 from dkist_service_configuration import logger
 
 from dkist_processing_visp.models.tags import VispTag
 from dkist_processing_visp.parsers.visp_l0_fits_access import VispL0FitsAccess
@@ -29,15 +30,15 @@
 from dkist_processing_visp.tasks.parse import ParseL0VispInputData
 from dkist_processing_visp.tasks.quality_metrics import VispL0QualityMetrics
 from dkist_processing_visp.tasks.quality_metrics import VispL1QualityMetrics
 from dkist_processing_visp.tasks.science import ScienceCalibration
 from dkist_processing_visp.tasks.solar import SolarCalibration
 from dkist_processing_visp.tasks.visp_base import VispTaskBase
 from dkist_processing_visp.tasks.write_l1 import VispWriteL1Frame
-from dkist_processing_visp.tests.conftest import VispTestingParameters
+from dkist_processing_visp.tests.conftest import VispInputDatasetParameterValues
 from dkist_processing_visp.tests.local_trial_workflows.local_trial_helpers import LoadBackgroundCal
 from dkist_processing_visp.tests.local_trial_workflows.local_trial_helpers import LoadDarkCal
 from dkist_processing_visp.tests.local_trial_workflows.local_trial_helpers import LoadGeometricCal
 from dkist_processing_visp.tests.local_trial_workflows.local_trial_helpers import LoadInputParsing
 from dkist_processing_visp.tests.local_trial_workflows.local_trial_helpers import LoadInstPolCal
 from dkist_processing_visp.tests.local_trial_workflows.local_trial_helpers import LoadLampCal
 from dkist_processing_visp.tests.local_trial_workflows.local_trial_helpers import LoadSolarCal
@@ -125,15 +126,15 @@
         self.tag(doc_path, VispTag.input_dataset_parameters())
         logger.info(f"Wrote input dataset doc to {doc_path}")
 
     @property
     def input_dataset_document_simple_parameters_part(self):
         parameters_list = []
         value_id = randint(1000, 2000)
-        for pn, pv in asdict(VispTestingParameters()).items():
+        for pn, pv in asdict(VispInputDatasetParameterValues()).items():
             values = [
                 {
                     "parameterValueId": value_id,
                     "parameterValue": json.dumps(pv),
                     "parameterValueStartDate": "1946-11-20",
                 }
             ]
@@ -184,23 +185,24 @@
         logger.info(f"Found {self.constants.num_map_scans} map scans")
         step = 0
         logger.info(f"Step {step} is organized thusly:")
         for map in range(1, self.constants.num_map_scans + 1):
             logger.info(f"Map #{map}:")
             for mod in range(1, self.constants.num_modstates + 1):
                 fits_obj = list(
-                    self.fits_data_read_fits_access(
+                    self.read(
                         tags=[
                             VispTag.input(),
                             VispTag.frame(),
                             VispTag.map_scan(map),
                             VispTag.modstate(mod),
                             VispTag.raster_step(step),
                         ],
-                        cls=VispL0FitsAccess,
+                        decoder=fits_access_decoder,
+                        fits_access_class=VispL0FitsAccess,
                     )
                 )
                 logger.info(
                     f"\tModstate {mod} has {len(fits_obj)} files. Date is {fits_obj[0].time_obs}"
                 )
```

### Comparing `dkist_processing_visp-2.8.2/dkist_processing_visp/tests/local_trial_workflows/local_trial_helpers.py` & `dkist_processing_visp-2.9.0/dkist_processing_visp/tests/local_trial_workflows/local_trial_helpers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import os
 import shutil
 from pathlib import Path
 
 import asdf
+from dkist_processing_common.models.task_name import TaskName
 from dkist_processing_common.tasks import WorkflowTaskBase
 from dkist_processing_common.tasks.mixin.globus import GlobusTransferItem
 from dkist_service_configuration import logger
 
 from dkist_processing_visp.models.tags import VispTag
+from dkist_processing_visp.models.task_name import VispTaskName
 from dkist_processing_visp.tasks.trial_output_data import TransferVispTrialData
 
 
 class SaveInputParsing(WorkflowTaskBase):
     """Dump redis db to file"""
 
     @property
@@ -116,20 +118,18 @@
         logger.info(f"Loaded database entries from {full_save_file}")
 
 
 class SaveGeometricCal(WorkflowTaskBase):
     def run(self) -> None:
         relative_save_file = "geometric_cal.asdf"
         file_tag_dict = dict()
-        path_list = list(self.read(tags=[VispTag.task("GEOMETRIC_ANGLE"), VispTag.intermediate()]))
+        path_list = list(self.read(tags=[VispTag.task_geometric_angle(), VispTag.intermediate()]))
+        path_list += list(self.read(tags=[VispTag.task_geometric_offset(), VispTag.intermediate()]))
         path_list += list(
-            self.read(tags=[VispTag.task("GEOMETRIC_OFFSET"), VispTag.intermediate()])
-        )
-        path_list += list(
-            self.read(tags=[VispTag.task("GEOMETRIC_SPEC_SHIFTS"), VispTag.intermediate()])
+            self.read(tags=[VispTag.task_geometric_sepectral_shifts(), VispTag.intermediate()])
         )
         save_dir = self.scratch.workflow_base_path / Path(relative_save_file).stem
         save_dir.mkdir(exist_ok=True)
         for p in path_list:
             copied_path = shutil.copy(str(p), save_dir)
             tags = self.tags(p)
             file_tag_dict[copied_path] = tags
@@ -146,15 +146,15 @@
     def relative_save_file(self) -> str:
         return "geometric_cal.asdf"
 
 
 class SaveDarkCal(SaveTaskTags):
     @property
     def task_str(self) -> str:
-        return "DARK"
+        return TaskName.dark.value
 
     @property
     def relative_save_file(self) -> str:
         return "dark_cal.asdf"
 
 
 class LoadDarkCal(LoadTaskTags):
@@ -162,15 +162,15 @@
     def relative_save_file(self) -> str:
         return "dark_cal.asdf"
 
 
 class SaveBackgroundCal(SaveTaskTags):
     @property
     def task_str(self) -> str:
-        return "BACKGROUND"
+        return VispTaskName.background.value
 
     @property
     def relative_save_file(self) -> str:
         return "background_cal.asdf"
 
 
 class LoadBackgroundCal(LoadTaskTags):
@@ -178,15 +178,15 @@
     def relative_save_file(self) -> str:
         return "background_cal.asdf"
 
 
 class SaveLampCal(SaveTaskTags):
     @property
     def task_str(self) -> str:
-        return "LAMP_GAIN"
+        return TaskName.lamp_gain.value
 
     @property
     def relative_save_file(self) -> str:
         return "lamp_cal.asdf"
 
 
 class LoadLampCal(LoadTaskTags):
@@ -194,15 +194,15 @@
     def relative_save_file(self) -> str:
         return "lamp_cal.asdf"
 
 
 class SaveSolarCal(SaveTaskTags):
     @property
     def task_str(self) -> str:
-        return "SOLAR_GAIN"
+        return TaskName.solar_gain.value
 
     @property
     def relative_save_file(self) -> str:
         return "solar_cal.asdf"
 
 
 class LoadSolarCal(LoadTaskTags):
@@ -210,15 +210,15 @@
     def relative_save_file(self) -> str:
         return "solar_cal.asdf"
 
 
 class SaveInstPolCal(SaveTaskTags):
     @property
     def task_str(self) -> str:
-        return "DEMOD_MATRICES"
+        return TaskName.demodulation_matrices.value
 
     @property
     def relative_save_file(self) -> str:
         return "inst_pol_cal.asdf"
 
 
 class LoadInstPolCal(LoadTaskTags):
```

### Comparing `dkist_processing_visp-2.8.2/dkist_processing_visp/tests/test_assemble_movie.py` & `dkist_processing_visp-2.9.0/dkist_processing_visp/tests/test_quality.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,58 +1,81 @@
+import json
+
 import pytest
 from dkist_processing_common._util.scratch import WorkflowFileSystem
+from dkist_processing_common.codecs.fits import fits_hdulist_encoder
+from dkist_processing_common.models.tags import Tag
 from dkist_processing_common.tests.conftest import FakeGQLClient
 
-from dkist_processing_visp.models.tags import VispTag
-from dkist_processing_visp.tasks.assemble_movie import AssembleVispMovie
-from dkist_processing_visp.tests.conftest import generate_214_l1_fits_frame
-from dkist_processing_visp.tests.conftest import Visp122ObserveFrames
+from dkist_processing_visp.tasks.quality_metrics import VispL1QualityMetrics
 from dkist_processing_visp.tests.conftest import VispConstantsDb
+from dkist_processing_visp.tests.conftest import write_full_sci_outputs_to_task
 
 
 @pytest.fixture(scope="function")
-def assemble_task_with_tagged_movie_frames(tmp_path, recipe_run_id, init_visp_constants_db):
-    num_map_scans = 10
-    init_visp_constants_db(recipe_run_id, VispConstantsDb(NUM_MAP_SCANS=num_map_scans))
-    with AssembleVispMovie(
-        recipe_run_id=recipe_run_id, workflow_name="vbi_make_movie_frames", workflow_version="VX.Y"
+def visp_quality_task(tmp_path, pol_type, recipe_run_id, init_visp_constants_db):
+    num_map_scans = 3
+    num_raster_steps = 2
+    polarimeter_mode = "observe_polarimetric"
+    num_stokes = 4
+    if pol_type == "Stokes-I":
+        polarimeter_mode = "observe_intensity"
+        num_stokes = 1
+    constants_db = VispConstantsDb(
+        POLARIMETER_MODE=polarimeter_mode,
+        NUM_MAP_SCANS=num_map_scans,
+        NUM_RASTER_STEPS=num_raster_steps,
+    )
+    init_visp_constants_db(recipe_run_id, constants_db)
+    with VispL1QualityMetrics(
+        recipe_run_id=recipe_run_id, workflow_name="science_calibration", workflow_version="VX.Y"
     ) as task:
-        try:  # This try... block is here to make sure the dbs get cleaned up if there's a failure in the fixture
-            task._scratch = WorkflowFileSystem(
-                scratch_base_path=tmp_path, recipe_run_id=recipe_run_id
-            )
-            task.testing_num_map_scans = num_map_scans
-            task.num_steps = 1
-            task.num_exp_per_step = 1
-            ds = Visp122ObserveFrames(
-                array_shape=(1, 100, 100),
-                num_steps=task.num_steps,
-                num_exp_per_step=task.num_exp_per_step,
-                num_map_scans=task.testing_num_map_scans,
-            )
-            header_generator = (d.header() for d in ds)
-            for d, header in enumerate(header_generator):
-                hdl = generate_214_l1_fits_frame(s122_header=header)
-                task.fits_data_write(
-                    hdu_list=hdl,
-                    tags=[
-                        VispTag.movie_frame(),
-                        VispTag.map_scan(d + 1),
-                    ],
-                )
-            yield task
-        except:
-            raise
-        finally:
-            task._purge()
+        task.scratch = WorkflowFileSystem(scratch_base_path=tmp_path)
+
+        yield task, num_map_scans, num_raster_steps, num_stokes
+        task._purge()
 
 
-def test_assemble_movie(assemble_task_with_tagged_movie_frames, mocker):
+@pytest.mark.parametrize("pol_type", ["Full Stokes", "Stokes-I"])
+def test_quality_task(visp_quality_task, pol_type, mocker):
+    """
+    Given: A VISPQualityMetrics task
+    When: Calling the task instance
+    Then: A single sensitivity measurement and datetime is recorded for each map scan for each Stokes Q, U, and V,
+            and a single noise measurement and datetime is recorded for L1 file for each Stokes Q, U, and V
+    """
     mocker.patch(
         "dkist_processing_common.tasks.mixin.metadata_store.GraphQLClient", new=FakeGQLClient
     )
-    assemble_task_with_tagged_movie_frames()
-    movie_file = list(assemble_task_with_tagged_movie_frames.read(tags=[VispTag.movie()]))
-    assert len(movie_file) == 1
-    assert movie_file[0].exists()
-    # import os
-    # os.system(f"cp {movie_file[0]} foo.mp4")
+    # When
+    task, num_maps, num_steps, num_stokes = visp_quality_task
+    write_full_sci_outputs_to_task(
+        task, num_maps=num_maps, num_steps=num_steps, data_shape=(10, 10), pol_type=pol_type
+    )
+
+    task()
+    # Then
+    num_map_scans = task.constants.num_map_scans
+    num_steps = task.constants.num_raster_steps
+    sensitivity_files = list(task.read(tags=[Tag.quality("SENSITIVITY")]))
+    assert len(sensitivity_files) == num_stokes
+    for file in sensitivity_files:
+        with file.open() as f:
+            data = json.load(f)
+            assert isinstance(data, dict)
+            for time in range(len(data["x_values"])):
+                assert type(data["x_values"][time]) == str
+            for noise in range(len(data["y_values"])):
+                assert type(data["y_values"][noise]) == float
+            assert len(data["x_values"]) == len(data["y_values"]) == num_map_scans
+
+    noise_files = list(task.read(tags=[Tag.quality("NOISE")]))
+    assert len(noise_files) == num_stokes
+    for file in noise_files:
+        with file.open() as f:
+            data = json.load(f)
+            assert isinstance(data, dict)
+            for time in range(len(data["x_values"])):
+                assert type(data["x_values"][time]) == str
+            for noise in range(len(data["y_values"])):
+                assert type(data["y_values"][noise]) == float
+            assert len(data["x_values"]) == len(data["y_values"]) == num_map_scans * num_steps
```

### Comparing `dkist_processing_visp-2.8.2/dkist_processing_visp/tests/test_background_light.py` & `dkist_processing_visp-2.9.0/dkist_processing_visp/tests/test_background_light.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,70 +1,68 @@
 import datetime
 import json
+from typing import Callable
 
 import numpy as np
 import pytest
 from astropy.io import fits
 from dkist_data_simulator.dataset import key_function
 from dkist_data_simulator.spec122 import Spec122Dataset
 from dkist_header_validator import spec122_validator
 from dkist_header_validator.translator import translate_spec122_to_spec214_l0
 from dkist_processing_common._util.scratch import WorkflowFileSystem
+from dkist_processing_common.codecs.fits import fits_array_encoder
+from dkist_processing_common.models.task_name import TaskName
 from dkist_processing_common.tests.conftest import FakeGQLClient
 from dkist_processing_pac.fitter.fitter_parameters import PolcalDresserParameters
 from dkist_processing_pac.input_data.drawer import Drawer
 from dkist_processing_pac.input_data.dresser import Dresser
 from dkist_processing_pac.optics.calibration_unit import CalibrationUnit
 from dkist_processing_pac.optics.telescope import Telescope
 
 from dkist_processing_visp.models.tags import VispTag
+from dkist_processing_visp.models.task_name import VispTaskName
 from dkist_processing_visp.parsers.visp_l0_fits_access import VispL0FitsAccess
 from dkist_processing_visp.tasks.background_light import BackgroundLightCalibration
 from dkist_processing_visp.tests.conftest import VispConstantsDb
-from dkist_processing_visp.tests.conftest import VispTestingParameters
+from dkist_processing_visp.tests.conftest import VispInputDatasetParameterValues
 from dkist_processing_visp.tests.conftest import WavelengthParameter
 
 
 @pytest.fixture(scope="session")
 def background_full_beam_shape() -> tuple[int, int]:
     """
     One-stop shop for adjusting the shape used for testing.
 
     Bigger takes longer and doesn't add much
     """
     return (100, 3)
 
 
 @pytest.fixture(scope="session")
-def background_testing_parameters(background_full_beam_shape) -> VispTestingParameters:
-    # We do this like this so it can depend on the full_beam_shape fixture for the beam border
-
-    num_wave = background_full_beam_shape[0]
-    cont_idx = list(range(num_wave // 2))
-    return VispTestingParameters(
-        visp_background_num_spatial_bins=WavelengthParameter(values=(1, 1, 1, 1)),
-        visp_background_wavelength_subsample_factor=WavelengthParameter(values=(20, 20, 20, 20)),
-        visp_background_num_fit_iterations=WavelengthParameter(values=(10, 10, 10, 10)),
-        visp_background_continuum_index=WavelengthParameter(
-            values=(cont_idx, cont_idx, cont_idx, cont_idx)
-        ),
-        visp_beam_border=num_wave,
-    )
-
+def background_testing_parameter_values(
+    background_full_beam_shape,
+) -> Callable[[bool], VispInputDatasetParameterValues]:
+    def make_parameters(background_on: bool = True):
+        num_wave = background_full_beam_shape[0]
+        cont_idx = list(range(num_wave // 2))
+        return VispInputDatasetParameterValues(
+            visp_background_on=background_on,
+            visp_background_num_spatial_bins=WavelengthParameter(values=(1, 1, 1, 1)),
+            visp_background_wavelength_subsample_factor=WavelengthParameter(
+                values=(20, 20, 20, 20)
+            ),
+            visp_background_num_fit_iterations=WavelengthParameter(values=(10, 10, 10, 10)),
+            visp_background_continuum_index=WavelengthParameter(
+                values=(cont_idx, cont_idx, cont_idx, cont_idx)
+            ),
+            visp_beam_border=num_wave,
+        )
 
-@pytest.fixture(scope="session")
-def background_testing_parameters_switch_off() -> VispTestingParameters:
-    return VispTestingParameters(
-        visp_background_on=False,
-        visp_background_num_spatial_bins=WavelengthParameter(values=(1, 1, 1, 1)),
-        visp_background_wavelength_subsample_factor=WavelengthParameter(values=(20, 20, 20, 20)),
-        visp_background_num_fit_iterations=WavelengthParameter(values=(10, 10, 10, 10)),
-        visp_background_continuum_index=WavelengthParameter(values=(1, 1, 1, 1)),
-        visp_beam_border=2,
-    )
+    return make_parameters
 
 
 @pytest.fixture(scope="session")
 def background_light(background_full_beam_shape) -> np.ndarray:
     num_wave, num_spatial = background_full_beam_shape
     beam1 = np.arange(num_wave) * 10.0 + 2
     beam2 = np.arange(num_wave) * 2.0 + 10
@@ -100,15 +98,15 @@
         self.ret_status = ret_status
         self.ret_theta = ret_theta
         self.dark_status = dark_status
         dataset_shape = (self.num_mod,) + array_shape[1:]
         super().__init__(
             dataset_shape, array_shape, time_delta, instrument=instrument, start_time=start_time
         )
-        self.add_constant_key("DKIST004", "polcal")
+        self.add_constant_key("DKIST004", TaskName.polcal.value.lower())
         self.add_constant_key("WAVELNTH", 854.0)
 
     @key_function("VISP_011")
     def modstate(self, key: str) -> int:
         return (self.index % self.num_mod) + 1
 
     @key_function("VISP_010")
@@ -278,235 +276,224 @@
                 np.ones(background_light.shape) * observed[m, n] / np.mean(cs_dict[n][m].data)
             )
             cs_dict[n][m].data = full_data + background_light
 
     return cs_dict
 
 
-@pytest.fixture(scope="function")
-def background_light_calibration_task(
-    tmp_path,
-    assign_input_dataset_doc_to_task,
-    init_visp_constants_db,
-    recipe_run_id,
-    fully_realistic_cs,
-    background_full_beam_shape,
-    background_testing_parameters,
-):
-    constants_db = VispConstantsDb(
+@pytest.fixture
+def total_polcal_files(fully_realistic_cs) -> int:
+    num_steps = len(fully_realistic_cs)
+    num_mod = len(fully_realistic_cs[0])
+    return num_steps * num_mod
+
+
+@pytest.fixture
+def num_polcal_dark_files(fully_realistic_cs) -> int:
+    num_mod = len(fully_realistic_cs[0])
+    return num_mod * 2  # Because there are two dark steps
+
+
+@pytest.fixture
+def write_background_input_files_to_task(background_full_beam_shape, fully_realistic_cs):
+    def write_to_task(task):
+        dark_cal = np.zeros(background_full_beam_shape)
+        # Need a dark for each beam
+        for beam in [1, 2]:
+            task.intermediate_frame_helpers_write_arrays(
+                arrays=dark_cal, beam=beam, task=TaskName.dark.value, readout_exp_time=0.02
+            )
+
+        # Now write polcal frames
+        num_steps = len(fully_realistic_cs)
+        num_mod = len(fully_realistic_cs[0])
+        for n in range(num_steps):
+            for m in range(num_mod):
+                hdu = fully_realistic_cs[n][m]._hdu
+                translated_header = translate_spec122_to_spec214_l0(hdu.header)
+                task.write(
+                    data=hdu.data,
+                    header=fits.Header(translated_header),
+                    tags=[
+                        VispTag.input(),
+                        VispTag.task_polcal(),
+                        VispTag.modstate(m + 1),
+                        VispTag.cs_step(n),
+                        VispTag.exposure_time(10.0),
+                        VispTag.readout_exp_time(0.02),
+                        VispTag.frame(),
+                    ],
+                    encoder=fits_array_encoder,
+                )
+
+    return write_to_task
+
+
+@pytest.fixture(scope="session")
+def default_constants(fully_realistic_cs) -> VispConstantsDb:
+    return VispConstantsDb(
         SOLAR_EXPOSURE_TIMES=(10.0,),
         OBSERVE_EXPOSURE_TIMES=(10.0,),
         POLCAL_EXPOSURE_TIMES=(10.0,),
         POLCAL_READOUT_EXP_TIMES=(0.02,),
         NUM_CS_STEPS=len(fully_realistic_cs),
     )
-    init_visp_constants_db(recipe_run_id, constants_db)
-    with BackgroundLightCalibration(
-        recipe_run_id=recipe_run_id,
-        workflow_name="background_light_calibration",
-        workflow_version="vX.Y",
-    ) as task:
-        number_of_beams = 2
-        try:  # This try... block is here to make sure the dbs get cleaned up if there's a failure in the fixture
-            task.scratch = WorkflowFileSystem(
-                scratch_base_path=tmp_path, recipe_run_id=recipe_run_id
-            )
-            assign_input_dataset_doc_to_task(task, background_testing_parameters)
-
-            dark_cal = np.zeros(background_full_beam_shape)
-            # Need a dark for each beam
-            for b in range(number_of_beams):
-                task.intermediate_frame_helpers_write_arrays(
-                    arrays=dark_cal, beam=b + 1, task="DARK", readout_exp_time=0.02
-                )
-
-            # Now write polcal frames
-            num_steps = len(fully_realistic_cs)
-            num_mod = len(fully_realistic_cs[0])
-            total_polcal_files = num_mod * num_steps
-            num_dark_polcal_files = num_mod * 2
-            for n in range(num_steps):
-                for m in range(num_mod):
-                    hdu = fully_realistic_cs[n][m]._hdu
-                    translated_header = translate_spec122_to_spec214_l0(hdu.header)
-                    hdul = fits.HDUList(
-                        [fits.PrimaryHDU(data=hdu.data, header=fits.Header(translated_header))]
-                    )
-                    task.fits_data_write(
-                        hdu_list=hdul,
-                        tags=[
-                            VispTag.input(),
-                            VispTag.task("POLCAL"),
-                            VispTag.modstate(m + 1),
-                            VispTag.cs_step(n),
-                            VispTag.exposure_time(10.0),
-                            VispTag.readout_exp_time(0.02),
-                            VispTag.frame(),
-                        ],
-                    )
-            yield task, total_polcal_files, num_dark_polcal_files
-        except:
-            raise
-        finally:
-            task._purge()
 
 
-@pytest.fixture(scope="function")
-def background_light_calibration_task_with_bad_exposure_times(
-    tmp_path,
-    assign_input_dataset_doc_to_task,
-    init_visp_constants_db,
-    recipe_run_id,
-    background_testing_parameters,
-):
-    constants_db = VispConstantsDb(
+@pytest.fixture(scope="session")
+def constants_bad_exp_times() -> VispConstantsDb:
+    return VispConstantsDb(
         SOLAR_EXPOSURE_TIMES=(1.0,),
         OBSERVE_EXPOSURE_TIMES=(10.0,),
         POLCAL_EXPOSURE_TIMES=(100.0,),
     )
-    init_visp_constants_db(recipe_run_id, constants_db)
-    with BackgroundLightCalibration(
-        recipe_run_id=recipe_run_id,
-        workflow_name="background_light_calibration",
-        workflow_version="vX.Y",
-    ) as task:
-        try:  # This try... block is here to make sure the dbs get cleaned up if there's a failure in the fixture
-            task.scratch = WorkflowFileSystem(
-                scratch_base_path=tmp_path, recipe_run_id=recipe_run_id
-            )
-            assign_input_dataset_doc_to_task(task, background_testing_parameters)
-            yield task
-        except:
-            raise
-        finally:
-            task._purge()
+
+
+@pytest.fixture(scope="session")
+def constatns_nor_polarimetric() -> VispConstantsDb:
+    return VispConstantsDb(
+        SOLAR_EXPOSURE_TIMES=(10.0,),
+        OBSERVE_EXPOSURE_TIMES=(10.0,),
+        POLCAL_EXPOSURE_TIMES=(10.0,),
+        POLARIMETER_MODE="observe_intensity",
+    )
 
 
 @pytest.fixture(scope="function")
-def background_light_calibration_task_non_polarimetric_dataset(
+def background_light_calibration_task(
     tmp_path,
     assign_input_dataset_doc_to_task,
     init_visp_constants_db,
     recipe_run_id,
-    background_testing_parameters,
+    background_testing_parameter_values,
 ):
-    constants_db = VispConstantsDb(
-        SOLAR_EXPOSURE_TIMES=(10.0,),
-        OBSERVE_EXPOSURE_TIMES=(10.0,),
-        POLCAL_EXPOSURE_TIMES=(10.0,),
-        POLARIMETER_MODE="observe_intensity",
-    )
+    constants_db = VispConstantsDb()
     init_visp_constants_db(recipe_run_id, constants_db)
     with BackgroundLightCalibration(
         recipe_run_id=recipe_run_id,
         workflow_name="background_light_calibration",
         workflow_version="vX.Y",
     ) as task:
         try:  # This try... block is here to make sure the dbs get cleaned up if there's a failure in the fixture
             task.scratch = WorkflowFileSystem(
                 scratch_base_path=tmp_path, recipe_run_id=recipe_run_id
             )
-            assign_input_dataset_doc_to_task(task, background_testing_parameters)
+            assign_input_dataset_doc_to_task(task, background_testing_parameter_values())
+
             yield task
         except:
             raise
         finally:
             task._purge()
 
 
 def test_background_light_calibration_task(
-    background_light_calibration_task, background_light, mocker
+    background_light_calibration_task,
+    write_background_input_files_to_task,
+    default_constants,
+    init_visp_constants_db,
+    total_polcal_files,
+    num_polcal_dark_files,
+    background_light,
+    mocker,
 ):
     """
     Give: a BackgroundLightCalibrationTask with a valid set of polcal data
     When: running the task
     Then: BACKGROUND intermediate frames are generated for each beam
     """
     mocker.patch(
         "dkist_processing_common.tasks.mixin.metadata_store.GraphQLClient", new=FakeGQLClient
     )
-    task, total_polcal_files, num_dark_polcal_files = background_light_calibration_task
+    task = background_light_calibration_task
+    init_visp_constants_db(task.recipe_run_id, default_constants)
+    write_background_input_files_to_task(task)
     task()
 
-    beam_1_bg = list(task.read(tags=[VispTag.beam(1), VispTag.task("BACKGROUND")]))
+    beam_1_bg = list(task.read(tags=[VispTag.beam(1), VispTag.task_background()]))
     assert len(beam_1_bg) == 1
     assert beam_1_bg[0].exists()
 
-    beam_2_bg = list(task.read(tags=[VispTag.beam(2), VispTag.task("BACKGROUND")]))
+    beam_2_bg = list(task.read(tags=[VispTag.beam(2), VispTag.task_background()]))
     assert len(beam_2_bg) == 1
     assert beam_2_bg[0].exists()
 
     quality_record = list(task.read(tags=[VispTag.quality("TASK_TYPES")]))
     assert len(quality_record) == 1
     with open(quality_record[0], "r") as f:
         data = json.load(f)
-        assert data["task_type"] == "BACKGROUND"
-        assert data["total_frames"] == total_polcal_files - num_dark_polcal_files
+        assert data["task_type"] == VispTaskName.background.value
+        assert data["total_frames"] == total_polcal_files - num_polcal_dark_files
         assert data["frames_not_used"] == 0
 
     # We don't currently test the actual accuracy of the calibration. We might never want to do this
     # beam_1_data = fits.open(beam_1_bg[0])[0].data
     # np.testing.assert_array_equal(beam_1_data, background_light[0, :1000, :])
     # beam_2_data = fits.open(beam_2_bg[0])[0].data
     # np.testing.assert_array_equal(beam_2_data, background_light[0, 1000:, :])
 
 
 def test_background_light_bad_exposure_times(
-    background_light_calibration_task_with_bad_exposure_times, mocker
+    background_light_calibration_task, constants_bad_exp_times, init_visp_constants_db, mocker
 ):
     """
     Given: A set of data where the polcal exposure times don't match those of solar gain and observe
     When: Trying to run BackgroundLightCalibration
     Then: An error is raised
     """
     mocker.patch(
         "dkist_processing_common.tasks.mixin.metadata_store.GraphQLClient", new=FakeGQLClient
     )
-    task = background_light_calibration_task_with_bad_exposure_times
+    task = background_light_calibration_task
+    init_visp_constants_db(task.recipe_run_id, constants_bad_exp_times)
     with pytest.raises(ValueError, match="do not all have the same FPA exposure time"):
         task()
 
 
 def test_background_light_non_polarimetric_dataset(
-    background_light_calibration_task_non_polarimetric_dataset, mocker
+    background_light_calibration_task, constatns_nor_polarimetric, init_visp_constants_db, mocker
 ):
     """
     Given: A dataset that is non-polarimetric (i.e., Stokes-I only)
     When: Running the BackgroundLightCalibration task
     Then: Nothing is done and no files are written
     """
     mocker.patch(
         "dkist_processing_common.tasks.mixin.metadata_store.GraphQLClient", new=FakeGQLClient
     )
-    task = background_light_calibration_task_non_polarimetric_dataset
+    task = background_light_calibration_task
+    init_visp_constants_db(task.recipe_run_id, constatns_nor_polarimetric)
     task()
 
     # Test that no BACKGROUND files were created
-    beam_1_bg = list(task.read(tags=[VispTag.beam(1), VispTag.task("BACKGROUND")]))
+    beam_1_bg = list(task.read(tags=[VispTag.beam(1), VispTag.task_background()]))
     assert len(beam_1_bg) == 0
-    beam_2_bg = list(task.read(tags=[VispTag.beam(2), VispTag.task("BACKGROUND")]))
+    beam_2_bg = list(task.read(tags=[VispTag.beam(2), VispTag.task_background()]))
     assert len(beam_2_bg) == 0
 
 
 def test_background_light_switch_off(
     background_light_calibration_task,
+    default_constants,
+    init_visp_constants_db,
     assign_input_dataset_doc_to_task,
-    background_testing_parameters_switch_off,
+    background_testing_parameter_values,
     mocker,
 ):
     """
     Given: A task with the background light switch turned off
     When: Running the BackgroundLightCalibration task
     Then: Nothing is done and no files are written
     """
     mocker.patch(
         "dkist_processing_common.tasks.mixin.metadata_store.GraphQLClient", new=FakeGQLClient
     )
-    task, _, _ = background_light_calibration_task
-    assign_input_dataset_doc_to_task(task, background_testing_parameters_switch_off)
+    task = background_light_calibration_task
+    init_visp_constants_db(task.recipe_run_id, default_constants)
+    assign_input_dataset_doc_to_task(task, background_testing_parameter_values(background_on=False))
     task()
 
     # Test that no BACKGROUND files were created
-    beam_1_bg = list(task.read(tags=[VispTag.beam(1), VispTag.task("BACKGROUND")]))
+    beam_1_bg = list(task.read(tags=[VispTag.beam(1), VispTag.task_background()]))
     assert len(beam_1_bg) == 0
-    beam_2_bg = list(task.read(tags=[VispTag.beam(2), VispTag.task("BACKGROUND")]))
+    beam_2_bg = list(task.read(tags=[VispTag.beam(2), VispTag.task_background()]))
     assert len(beam_2_bg) == 0
```

### Comparing `dkist_processing_visp-2.8.2/dkist_processing_visp/tests/test_build_quality_report.py` & `dkist_processing_visp-2.9.0/dkist_processing_visp/tests/test_build_quality_report.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.8.2/dkist_processing_visp/tests/test_dark.py` & `dkist_processing_visp-2.9.0/dkist_processing_visp/tests/test_dark.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,143 +1,167 @@
 import json
-from dataclasses import dataclass
+from functools import partial
 
 import numpy as np
 import pytest
 from astropy.io import fits
-from dkist_header_validator import spec122_validator
 from dkist_processing_common._util.scratch import WorkflowFileSystem
 from dkist_processing_common.models.tags import Tag
 from dkist_processing_common.tests.conftest import FakeGQLClient
 
 from dkist_processing_visp.models.tags import VispTag
 from dkist_processing_visp.tasks.dark import DarkCalibration
-from dkist_processing_visp.tests.conftest import generate_fits_frame
 from dkist_processing_visp.tests.conftest import VispConstantsDb
-from dkist_processing_visp.tests.conftest import VispHeadersValidDarkFrames
-from dkist_processing_visp.tests.conftest import VispTestingParameters
+from dkist_processing_visp.tests.conftest import VispInputDatasetParameterValues
+from dkist_processing_visp.tests.conftest import write_frames_to_task
+from dkist_processing_visp.tests.header_models import VispHeadersInputDarkFrames
 
 
-@dataclass
-class VispDarkTestingParameters(VispTestingParameters):
-    visp_beam_border: int = 10
+class VispHeadersDarksWithNumExp(VispHeadersInputDarkFrames):
+    def __init__(self, *args, num_exp_per_fpa: int, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.add_constant_key("CAM__014", num_exp_per_fpa)
 
 
-@pytest.fixture(scope="function")
-def dark_calibration_task(
-    tmp_path, assign_input_dataset_doc_to_task, init_visp_constants_db, recipe_run_id
+def make_dark_array_data(
+    dataframe: VispHeadersDarksWithNumExp, readout_exp_time: float, beam_border: int
+):
+    array_shape = dataframe.array_shape
+    data = np.zeros(array_shape)
+
+    data[0, :beam_border, :] = 1 * readout_exp_time  # Beam 1
+    data[0, beam_border:, :] = 2 * readout_exp_time  # Beam 2
+
+    return data
+
+
+def write_darks_to_task(
+    task,
+    readout_exp_time: float,
+    num_raw_per_fpa: int,
+    num_frames: int,
+    data_shape: tuple[int, int],
+    beam_border: int,
 ):
+    array_shape = (1, *data_shape)
+    dataset = VispHeadersDarksWithNumExp(
+        array_shape=array_shape,
+        time_delta=10.0,
+        readout_exp_time=readout_exp_time,
+        num_modstates=num_frames,
+        num_exp_per_fpa=num_raw_per_fpa,
+    )
+
+    data_func = partial(
+        make_dark_array_data, readout_exp_time=readout_exp_time, beam_border=beam_border
+    )
+    num_written_frames = write_frames_to_task(
+        task=task,
+        frame_generator=dataset,
+        extra_tags=[
+            VispTag.input(),
+            VispTag.task_dark(),
+            VispTag.readout_exp_time(readout_exp_time),
+        ],
+        data_func=data_func,
+    )
+    return num_written_frames
+
+
+@pytest.fixture(scope="function")
+def dark_calibration_task(tmp_path, init_visp_constants_db, recipe_run_id):
+    readout_exp_times = [0.02, 2.0, 200.0]
     constants_db = VispConstantsDb(
-        LAMP_READOUT_EXP_TIMES=(200.0,),
-        SOLAR_READOUT_EXP_TIMES=(2.0,),
-        OBSERVE_READOUT_EXP_TIMES=(0.02,),
-        POLCAL_READOUT_EXP_TIMES=(),
+        NON_DARK_TASK_READOUT_EXP_TIMES=tuple(readout_exp_times),
     )
     init_visp_constants_db(recipe_run_id, constants_db)
     with DarkCalibration(
         recipe_run_id=recipe_run_id, workflow_name="dark_calibration", workflow_version="VX.Y"
     ) as task:
-        num_beam = 2
-        readout_exp_times = [0.02, 2.0, 200.0]
-        num_raw_values = [3, 4, 5]
-        unused_time = 100.0
-        unused_num_raw = 6
-        num_exp_time = len(readout_exp_times)
-        num_frames_per = 3
-        array_shape = (1, 20, 10)
-        dataset_shape = ((num_exp_time + 1) * num_frames_per, 20, 10)
         try:  # This try... block is here to make sure the dbs get cleaned up if there's a failure in the fixture
             task.scratch = WorkflowFileSystem(
                 scratch_base_path=tmp_path, recipe_run_id=recipe_run_id
             )
-            assign_input_dataset_doc_to_task(task, VispDarkTestingParameters())
-            beam_border = task.parameters.beam_border
-            ds = VispHeadersValidDarkFrames(
-                dataset_shape=dataset_shape,
-                array_shape=array_shape,
-                time_delta=10,
-            )
-            header_generator = (
-                spec122_validator.validate_and_translate_to_214_l0(
-                    d.header(), return_type=fits.HDUList
-                )[0].header
-                for d in ds
-            )
-            for e, n in zip(
-                readout_exp_times + [unused_time], num_raw_values + [unused_num_raw]
-            ):  # Make some darks we won't use
-                for _ in range(num_frames_per):
-                    hdul = generate_fits_frame(header_generator=header_generator, shape=array_shape)
-                    hdul[0].header["NSUMEXP"] = n
-                    hdul[0].data *= 0
-                    # Create combined 2-beam array
-                    beam = 1
-                    hdul[0].data[0, :beam_border, :] = beam * e
-                    beam = 2
-                    hdul[0].data[0, beam_border:, :] = beam * e
-                    task.fits_data_write(
-                        hdu_list=hdul,
-                        tags=[
-                            VispTag.input(),
-                            VispTag.frame(),
-                            VispTag.task("DARK"),
-                            VispTag.readout_exp_time(e),
-                        ],
-                    )
-            yield task, num_beam, readout_exp_times, num_raw_values, unused_time
+            yield task, readout_exp_times
+
         except:
             raise
+
         finally:
             task._purge()
 
 
-def test_dark_calibration_task(dark_calibration_task, mocker):
+def test_dark_calibration_task(dark_calibration_task, assign_input_dataset_doc_to_task, mocker):
     """
     Given: A DarkCalibration task with multiple task exposure times
     When: Calling the task instance
     Then: Only one average intermediate dark frame exists for each exposure time and unused times are not made
     """
     mocker.patch(
         "dkist_processing_common.tasks.mixin.metadata_store.GraphQLClient", new=FakeGQLClient
     )
+    # Given
+    task, readout_exp_times = dark_calibration_task
+    num_beam = 2
+    num_raw_values = [3, 4, 5]
+    unused_time = 100.0
+    unused_num_raw = 6
+    num_frames_per = 3
+    data_shape = (20, 10)
+    beam_border = data_shape[0] // 2
+    assign_input_dataset_doc_to_task(
+        task, VispInputDatasetParameterValues(visp_beam_border=beam_border)
+    )
+    for readout_exp_time, num_exp_per_fpa in zip(
+        readout_exp_times + [unused_time], num_raw_values + [unused_num_raw]
+    ):
+        write_darks_to_task(
+            task=task,
+            readout_exp_time=readout_exp_time,
+            num_raw_per_fpa=num_exp_per_fpa,
+            num_frames=num_frames_per,
+            data_shape=data_shape,
+            beam_border=beam_border,
+        )
+
     # When
-    task, num_beam, readout_exp_times, num_raw_frames, unused_time = dark_calibration_task
     task()
+
     # Then
-    for e, n in zip(readout_exp_times, num_raw_frames):
+    for e, n in zip(readout_exp_times, num_raw_values):
         for b in range(num_beam):
             files = list(
                 task.read(
                     tags=[
-                        VispTag.task("DARK"),
+                        VispTag.task_dark(),
                         VispTag.intermediate(),
                         VispTag.frame(),
                         VispTag.beam(b + 1),
                         VispTag.readout_exp_time(e),
                     ]
                 )
             )
             assert len(files) == 1
-            expected = np.ones((10, 10)) * (b + 1) * e / n
+            expected = np.ones((data_shape[0] // 2, data_shape[1])) * (b + 1) * e / n
             hdul = fits.open(files[0])
             np.testing.assert_allclose(expected, hdul[0].data, rtol=1e-15)
             hdul.close()
 
     unused_time_read = task.read(
         tags=[
-            VispTag.task("DARK"),
+            VispTag.task_dark(),
             VispTag.intermediate(),
             VispTag.frame(),
             VispTag.readout_exp_time(unused_time),
         ]
     )
     assert len(list(unused_time_read)) == 0
 
     quality_files = task.read(tags=[Tag.quality("TASK_TYPES")])
     for file in quality_files:
         with file.open() as f:
             data = json.load(f)
             assert isinstance(data, dict)
             assert data["total_frames"] == task.scratch.count_all(
-                tags=[VispTag.input(), VispTag.frame(), VispTag.task("DARK")]
+                tags=[VispTag.input(), VispTag.frame(), VispTag.task_dark()]
             )
-            assert data["frames_not_used"] == 3
+            assert data["frames_not_used"] == num_frames_per
```

### Comparing `dkist_processing_visp-2.8.2/dkist_processing_visp/tests/test_downsample.py` & `dkist_processing_visp-2.9.0/dkist_processing_visp/tests/test_downsample.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 import pytest
 import skimage.measure as skime
 
 from dkist_processing_visp.tasks.mixin.downsample import DownsampleMixin
 from dkist_processing_visp.tasks.visp_base import VispTaskBase
 from dkist_processing_visp.tests.conftest import VispConstantsDb
-from dkist_processing_visp.tests.conftest import VispTestingParameters
+from dkist_processing_visp.tests.conftest import VispInputDatasetParameterValues
 
 
 @pytest.fixture()
 def task_with_downsample_mixin(
     recipe_run_id, init_visp_constants_db, assign_input_dataset_doc_to_task
 ):
     class TaskWithDownsample(VispTaskBase, DownsampleMixin):
@@ -19,15 +19,15 @@
     constants_db = VispConstantsDb()
     init_visp_constants_db(recipe_run_id, constants_db)
     task = TaskWithDownsample(
         recipe_run_id=recipe_run_id,
         workflow_name="do_stuff",
         workflow_version="VX.Y",
     )
-    assign_input_dataset_doc_to_task(task, VispTestingParameters())
+    assign_input_dataset_doc_to_task(task, VispInputDatasetParameterValues())
 
     yield task
 
 
 @pytest.fixture(scope="session")
 def dummy_array() -> np.ndarray:
     return np.random.random((100, 2560))
```

### Comparing `dkist_processing_visp-2.8.2/dkist_processing_visp/tests/test_geometric.py` & `dkist_processing_visp-2.9.0/dkist_processing_visp/tests/test_geometric.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,288 +1,262 @@
 import json
-from dataclasses import dataclass
+from functools import partial
+from typing import Callable
 
 import numpy as np
 import pytest
 from dkist_processing_common._util.scratch import WorkflowFileSystem
 from dkist_processing_common.models.tags import Tag
 from dkist_processing_common.tests.conftest import FakeGQLClient
 from dkist_processing_math import transform
 
 from dkist_processing_visp.models.tags import VispTag
 from dkist_processing_visp.tasks.geometric import GeometricCalibration
-from dkist_processing_visp.tests.conftest import generate_214_l0_fits_frame
+from dkist_processing_visp.tests.conftest import tag_on_modstate
 from dkist_processing_visp.tests.conftest import VispConstantsDb
-from dkist_processing_visp.tests.conftest import VispHeadersValidLampGainFrames
-from dkist_processing_visp.tests.conftest import VispHeadersValidSolarGainFrames
-from dkist_processing_visp.tests.conftest import VispTestingParameters
+from dkist_processing_visp.tests.conftest import VispInputDatasetParameterValues
+from dkist_processing_visp.tests.conftest import write_frames_to_task
+from dkist_processing_visp.tests.conftest import write_intermediate_darks_to_task
+from dkist_processing_visp.tests.header_models import VispHeadersInputLampGainFrames
+from dkist_processing_visp.tests.header_models import VispHeadersInputSolarGainFrames
 
 
-@dataclass
-class VispGeoTestingParameters30(VispTestingParameters):
-    visp_beam_border: int = 30
+def make_solar_array_data(
+    frame: VispHeadersInputSolarGainFrames,
+    intermediate_shape: tuple[int, int],
+    dark_signal: float,
+    angles: np.ndarray,
+    offsets: np.ndarray,
+):
+    modstate = frame.current_modstate("")  # Weird signature due to key_function
+    num_raw_per_fpa = frame.header()["CAM__014"]
 
+    beam_list = []
+    for beam in [1, 2]:
+        true_solar = 10 * (np.ones(intermediate_shape) + modstate + beam)
+        translated_solar = next(
+            transform.translate_arrays(
+                arrays=true_solar, translation=offsets[beam - 1][modstate - 1]
+            )
+        )
+        translated_solar[translated_solar == 0] = 10 * (modstate + beam + 1)
 
-@pytest.fixture(scope="function")
-def geometric_calibration_task_that_completes(
-    tmp_path, recipe_run_id, assign_input_dataset_doc_to_task, init_visp_constants_db
+        # Hairlines
+        translated_solar[:, 30] = 5.0
+        translated_solar[:, 70] = 5.0
+        distorted_solar = next(
+            transform.rotate_arrays_about_point(arrays=translated_solar, angle=angles[beam - 1])
+        )
+        beam_list.append((distorted_solar + dark_signal) * num_raw_per_fpa)
+
+    raw_solar = np.concatenate(beam_list)
+
+    return raw_solar
+
+
+def make_simple_darked_array_data(
+    frame: VispHeadersInputSolarGainFrames | VispHeadersInputLampGainFrames,
+    dark_signal: float,
+    input_data_shape: tuple[int, int],
+    beam_border: int,
 ):
-    # This fixture makes data that look enough like real data that all of the feature detection stuff at least runs
-    # through (mostly this is an issue for the angle calculation). It would be great to contrive data that
-    # produce a geometric calibration with real numbers that can be checked, but for now we'll rely on the grogu
-    # tests for that. In other words, this fixture just tests if the machinery of the task completes and some object
-    # (ANY object) is written correctly.
-    number_of_modstates = 3
-    number_of_beams = 2
-    solar_exp_time = 40.0  # From VispHeadersValidSolarGainFrames fixture
-    lamp_exp_time = 20.0  # From VispHeadersValidLampGainFrames fixture
-    intermediate_shape = (30, 100)
-    array_shape = (1, 60, 100)
-    dataset_shape = array_shape
-    constants_db = VispConstantsDb(
-        NUM_MODSTATES=number_of_modstates,
-        SOLAR_READOUT_EXP_TIMES=(solar_exp_time,),
-        LAMP_READOUT_EXP_TIMES=(lamp_exp_time,),
+    modstate = frame.current_modstate("")  # Weird signature due to key_function
+    num_raw_per_fpa = frame.header()["CAM__014"]
+
+    true_data = np.ones(input_data_shape) + modstate
+
+    true_data[:beam_border, :] += 1  # Beam 1
+    true_data[beam_border:, :] += 2  # Beam 2
+    raw_data = (true_data + dark_signal) * num_raw_per_fpa
+
+    return raw_data
+
+
+def write_geometric_solar_inputs_to_task(
+    task,
+    num_modstates: int,
+    readout_exp_time: float,
+    data_shape: tuple[int, int],
+    data_func: Callable,
+):
+    array_shape = (1, *data_shape)
+    dataset = VispHeadersInputSolarGainFrames(
+        array_shape=array_shape,
+        time_delta=10,
+        num_modstates=num_modstates,
+        readout_exp_time=readout_exp_time,
+    )
+    write_frames_to_task(
+        task=task,
+        frame_generator=dataset,
+        extra_tags=[
+            VispTag.input(),
+            VispTag.task_solar_gain(),
+            VispTag.readout_exp_time(readout_exp_time),
+        ],
+        tag_func=tag_on_modstate,
+        data_func=data_func,
     )
-    init_visp_constants_db(recipe_run_id, constants_db)
-    with GeometricCalibration(
-        recipe_run_id=recipe_run_id, workflow_name="geometric_calibration", workflow_version="VX.Y"
-    ) as task:
-        try:  # This try... block is here to make sure the dbs get cleaned up if there's a failure in the fixture
-            task.scratch = WorkflowFileSystem(
-                scratch_base_path=tmp_path, recipe_run_id=recipe_run_id
-            )
-            assign_input_dataset_doc_to_task(task, VispGeoTestingParameters30())
-            task.angles = np.array([0.01, -0.01])
-            task.offsets = np.zeros((number_of_beams, number_of_modstates, 2))
-            task.shifts = np.zeros(intermediate_shape[0])
-            for beam in range(1, number_of_beams + 1):
-
-                dark_cal = np.ones(intermediate_shape) * 3.0
-                task.intermediate_frame_helpers_write_arrays(
-                    arrays=dark_cal, beam=beam, task="DARK", readout_exp_time=solar_exp_time
-                )
-
-                task.intermediate_frame_helpers_write_arrays(
-                    arrays=dark_cal, beam=beam, task="DARK", readout_exp_time=lamp_exp_time
-                )
-
-                for modstate in range(1, number_of_modstates + 1):
-                    solar_ds = VispHeadersValidSolarGainFrames(
-                        dataset_shape=dataset_shape,
-                        array_shape=array_shape,
-                        time_delta=10,
-                        num_modstates=number_of_modstates,
-                        modstate=modstate,
-                    )
-                    solar_header = solar_ds.header()
-                    solar_num_raw_per_fpa = solar_header["CAM__014"]
-                    true_solar = 10 * (np.ones(array_shape[1:]) + modstate + beam)
-                    translated_solar = next(
-                        transform.translate_arrays(
-                            arrays=true_solar, translation=task.offsets[beam - 1][modstate - 1]
-                        )
-                    )
-                    translated_solar[translated_solar == 0] = 10 * (modstate + beam + 1)
-
-                    # Hairlines
-                    translated_solar[:, 30] = 5.0
-                    translated_solar[:, 70] = 5.0
-                    distorted_solar = next(
-                        transform.rotate_arrays_about_point(
-                            arrays=translated_solar, angle=task.angles[beam - 1]
-                        )
-                    )
-                    raw_dark = np.concatenate((dark_cal, dark_cal))
-                    raw_solar = (distorted_solar + raw_dark) * solar_num_raw_per_fpa
-                    solar_hdul = generate_214_l0_fits_frame(
-                        data=raw_solar, s122_header=solar_header
-                    )
-                    task.fits_data_write(
-                        hdu_list=solar_hdul,
-                        tags=[
-                            VispTag.input(),
-                            VispTag.task("SOLAR_GAIN"),
-                            VispTag.modstate(modstate),
-                            VispTag.frame(),
-                            VispTag.beam(beam),
-                            VispTag.readout_exp_time(solar_exp_time),
-                        ],
-                    )
-
-                    lamp_ds = VispHeadersValidLampGainFrames(
-                        dataset_shape=dataset_shape,
-                        array_shape=array_shape,
-                        time_delta=10,
-                        num_modstates=number_of_modstates,
-                        modstate=modstate,
-                    )
-                    lamp_header = lamp_ds.header()
-                    lamp_num_raw_per_fpa = lamp_header["CAM__014"]
-                    true_lamp = 10 * (np.ones(array_shape[1:]) + modstate + beam)
-                    translated_lamp = next(
-                        transform.translate_arrays(
-                            arrays=true_lamp, translation=task.offsets[beam - 1][modstate - 1]
-                        )
-                    )
-                    translated_lamp[translated_lamp == 0] = 10 * (modstate + beam + 1)
-
-                    # Hairlines
-                    translated_lamp[:, 30] = 5.0
-                    translated_lamp[:, 70] = 5.0
-                    # Chop out part of the second hairline so the fitter has to skip over these pixels
-                    translated_lamp[5:9, 70] = 10 * (modstate + beam + 1)
-                    distorted_lamp = next(
-                        transform.rotate_arrays_about_point(
-                            arrays=translated_lamp, angle=task.angles[beam - 1]
-                        )
-                    )
-                    raw_lamp = (distorted_lamp + raw_dark) * lamp_num_raw_per_fpa
-                    lamp_hdul = generate_214_l0_fits_frame(data=raw_lamp, s122_header=lamp_header)
-                    task.fits_data_write(
-                        hdu_list=lamp_hdul,
-                        tags=[
-                            VispTag.input(),
-                            VispTag.task("LAMP_GAIN"),
-                            VispTag.modstate(modstate),
-                            VispTag.frame(),
-                            VispTag.beam(beam),
-                            VispTag.readout_exp_time(lamp_exp_time),
-                        ],
-                    )
 
-            yield task
-        except:
-            raise
-        finally:
-            task._purge()
 
+def make_lamp_array_data(
+    frame: VispHeadersInputLampGainFrames,
+    intermediate_shape: tuple[int, int],
+    dark_signal: float,
+    angles: np.ndarray,
+    offsets: np.ndarray,
+):
+    modstate = frame.current_modstate("")  # Weird signature due to key_function
+    num_raw_per_fpa = frame.header()["CAM__014"]
+
+    beam_list = []
+    for beam in [1, 2]:
+        true_lamp = 10 * (np.ones(intermediate_shape) + modstate + beam)
+        translated_lamp = next(
+            transform.translate_arrays(
+                arrays=true_lamp, translation=offsets[beam - 1][modstate - 1]
+            )
+        )
+        translated_lamp[translated_lamp == 0] = 10 * (modstate + beam + 1)
+
+        # Hairlines
+        translated_lamp[:, 30] = 5.0
+        translated_lamp[:, 70] = 5.0
+        # Chop out part of the second hairline so the fitter has to skip over these pixels
+        translated_lamp[5:9, 70] = 10 * (modstate + beam + 1)
+        distorted_lamp = next(
+            transform.rotate_arrays_about_point(arrays=translated_lamp, angle=angles[beam - 1])
+        )
+        beam_list.append((distorted_lamp + dark_signal) * num_raw_per_fpa)
+
+    raw_lamp = np.concatenate(beam_list)
+
+    return raw_lamp
+
+
+def write_geometric_lamp_inputs_to_task(
+    task,
+    num_modstates: int,
+    readout_exp_time: float,
+    data_shape: tuple[int, int],
+    data_func: Callable,
+):
+    array_shape = (1, *data_shape)
+    dataset = VispHeadersInputLampGainFrames(
+        array_shape=array_shape,
+        time_delta=10,
+        num_modstates=num_modstates,
+        readout_exp_time=readout_exp_time,
+    )
 
-@dataclass
-class VispGeoTestingParameters10(VispTestingParameters):
-    visp_beam_border: int = 10
+    write_frames_to_task(
+        task=task,
+        frame_generator=dataset,
+        extra_tags=[
+            VispTag.input(),
+            VispTag.task_lamp_gain(),
+            VispTag.readout_exp_time(readout_exp_time),
+        ],
+        tag_func=tag_on_modstate,
+        data_func=data_func,
+    )
 
 
 @pytest.fixture(scope="function")
-def geometric_calibration_task_with_simple_raw_data(
-    tmp_path, recipe_run_id, assign_input_dataset_doc_to_task, init_visp_constants_db
-):
+def geometric_calibration_task(tmp_path, recipe_run_id, init_visp_constants_db):
     number_of_modstates = 3
-    number_of_beams = 2
-    solar_exp_time = 40.0  # From VispHeadersValidSolarGainFrames fixture
-    lamp_exp_time = 20.0  # From VispHeadersValidLampGainFrames fixture
-    data_shape_int = (10, 10)
-    data_shape_raw = (20, 10)
+    solar_exp_time = 40.0
+    lamp_exp_time = 20.0
+    readout_exp_times = [lamp_exp_time, solar_exp_time]
     constants_db = VispConstantsDb(
         NUM_MODSTATES=number_of_modstates,
         SOLAR_READOUT_EXP_TIMES=(solar_exp_time,),
         LAMP_READOUT_EXP_TIMES=(lamp_exp_time,),
     )
     init_visp_constants_db(recipe_run_id, constants_db)
     with GeometricCalibration(
         recipe_run_id=recipe_run_id, workflow_name="geometric_calibration", workflow_version="VX.Y"
     ) as task:
-        task.scratch = WorkflowFileSystem(scratch_base_path=tmp_path, recipe_run_id=recipe_run_id)
-        assign_input_dataset_doc_to_task(task, VispGeoTestingParameters10())
-
-        # Create the intermediate frames needed
-        for beam in range(1, number_of_beams + 1):
-
-            dark_cal = np.ones(data_shape_int) * 3.0
-            task.intermediate_frame_helpers_write_arrays(
-                arrays=dark_cal, beam=beam, task="DARK", readout_exp_time=solar_exp_time
-            )
-
-            task.intermediate_frame_helpers_write_arrays(
-                arrays=dark_cal, beam=beam, task="DARK", readout_exp_time=lamp_exp_time
-            )
-
-            # Let's write a dark with the wrong exposure time, just to make sure it doesn't get used
-            task.intermediate_frame_helpers_write_arrays(
-                arrays=np.ones(data_shape_int) * 1e6,
-                beam=beam,
-                task="DARK",
-                readout_exp_time=solar_exp_time**2,
-            )
-
-        # Create the raw data, which is based on two beams per frame
-        beam1 = 1
-        beam2 = 2
-        dark_cal_two_beams = np.concatenate((dark_cal, dark_cal))
-        for modstate in range(1, number_of_modstates + 1):
-
-            # Solar
-            solar_ds = VispHeadersValidSolarGainFrames(
-                dataset_shape=(1,) + data_shape_raw,
-                array_shape=(1,) + data_shape_raw,
-                time_delta=10,
-                num_modstates=number_of_modstates,
-                modstate=modstate,
-            )
-            solar_header = solar_ds.header()
-            solar_num_raw_per_fpa = solar_header["CAM__014"]
-            true_solar = np.ones(data_shape_raw) + modstate
-            # Now add the beam number to each beam in the array
-            true_solar[: task.parameters.beam_border, :] += beam1
-            true_solar[task.parameters.beam_border :, :] += beam2
-            raw_solar = (true_solar + dark_cal_two_beams) * solar_num_raw_per_fpa
-            solar_hdul = generate_214_l0_fits_frame(data=raw_solar, s122_header=solar_header)
-            task.fits_data_write(
-                hdu_list=solar_hdul,
-                tags=[
-                    VispTag.input(),
-                    VispTag.task("SOLAR_GAIN"),
-                    VispTag.modstate(modstate),
-                    VispTag.frame(),
-                    VispTag.readout_exp_time(solar_exp_time),
-                ],
-            )
-
-            # Lamp
-            lamp_ds = VispHeadersValidLampGainFrames(
-                dataset_shape=(1,) + data_shape_raw,
-                array_shape=(1,) + data_shape_raw,
-                time_delta=10,
-                num_modstates=number_of_modstates,
-                modstate=modstate,
-            )
-            lamp_header = lamp_ds.header()
-            lamp_num_raw_per_fpa = lamp_header["CAM__014"]
-            true_lamp = np.ones(data_shape_raw) + modstate
-            # Now add the beam number to each beam in the array
-            true_lamp[: task.parameters.beam_border, :] += beam1
-            true_lamp[task.parameters.beam_border :, :] += beam2
-            raw_lamp = (true_lamp + dark_cal_two_beams) * lamp_num_raw_per_fpa
-            lamp_hdul = generate_214_l0_fits_frame(data=raw_lamp, s122_header=lamp_header)
-            task.fits_data_write(
-                hdu_list=lamp_hdul,
-                tags=[
-                    VispTag.input(),
-                    VispTag.task("LAMP_GAIN"),
-                    VispTag.modstate(modstate),
-                    VispTag.frame(),
-                    VispTag.readout_exp_time(lamp_exp_time),
-                ],
+        try:  # This try... block is here to make sure the dbs get cleaned up if there's a failure in the fixture
+            task.scratch = WorkflowFileSystem(
+                scratch_base_path=tmp_path, recipe_run_id=recipe_run_id
             )
 
-        yield task
-        task._purge()
+            yield task, readout_exp_times, number_of_modstates
+        except:
+            raise
+        finally:
+            task._purge()
 
 
-def test_geometric_task(geometric_calibration_task_that_completes, mocker):
+def test_geometric_task(geometric_calibration_task, assign_input_dataset_doc_to_task, mocker):
     """
     Given: A set of raw solar gain images and necessary intermediate calibrations
     When: Running the geometric task
     Then: The damn thing runs and makes outputs that at least are the right type
     """
-    # See the note in the fixture above: this test does NOT test for accuracy of the calibration
+    # This test makes data that look enough like real data that all of the feature detection stuff at least runs
+    # through (mostly this is an issue for the angle calculation). It would be great to contrive data that
+    # produce a geometric calibration with real numbers that can be checked, but for now we'll rely on the grogu
+    # tests for that. In other words, this fixture just tests if the machinery of the task completes and some object
+    # (ANY object) is written correctly.
     mocker.patch(
         "dkist_processing_common.tasks.mixin.metadata_store.GraphQLClient", new=FakeGQLClient
     )
-    task = geometric_calibration_task_that_completes
+    task, readout_exp_times, num_modstates = geometric_calibration_task
+    dark_signal = 3.0
+    input_shape = (60, 100)
+    intermediate_shape = (30, 100)
+    angles = np.array([0.01, -0.01])
+    offsets = np.zeros((2, num_modstates, 2))
+    beam_border = input_shape[0] // 2
+    assign_input_dataset_doc_to_task(
+        task, VispInputDatasetParameterValues(visp_beam_border=beam_border)
+    )
+
+    # Intermediate darks are needed for correction
+    for readout_exp_time in readout_exp_times:
+        write_intermediate_darks_to_task(
+            task=task,
+            dark_signal=dark_signal,
+            readout_exp_time=readout_exp_time,
+            data_shape=intermediate_shape,
+        )
+
+    # Write input lamp and solar data
+    lamp_data_func = partial(
+        make_lamp_array_data,
+        intermediate_shape=intermediate_shape,
+        dark_signal=dark_signal,
+        angles=angles,
+        offsets=offsets,
+    )
+    write_geometric_lamp_inputs_to_task(
+        task=task,
+        num_modstates=num_modstates,
+        readout_exp_time=readout_exp_times[0],
+        data_shape=input_shape,
+        data_func=lamp_data_func,
+    )
+
+    solar_data_func = partial(
+        make_solar_array_data,
+        intermediate_shape=intermediate_shape,
+        dark_signal=dark_signal,
+        angles=angles,
+        offsets=offsets,
+    )
+    write_geometric_solar_inputs_to_task(
+        task=task,
+        num_modstates=num_modstates,
+        readout_exp_time=readout_exp_times[1],
+        data_shape=input_shape,
+        data_func=solar_data_func,
+    )
+
     task()
     for beam in range(1, task.constants.num_beams + 1):
         assert type(task.intermediate_frame_helpers_load_angle(beam=beam)) is np.float64
         assert task.intermediate_frame_helpers_load_spec_shift(beam=beam).shape == (100,)
         for modstate in range(1, task.constants.num_modstates + 1):
             assert task.intermediate_frame_helpers_load_state_offset(
                 beam=beam, modstate=modstate
@@ -290,25 +264,72 @@
 
     quality_files = task.read(tags=[Tag.quality("TASK_TYPES")])
     for file in quality_files:
         with file.open() as f:
             data = json.load(f)
             assert isinstance(data, dict)
             assert data["total_frames"] == task.scratch.count_all(
-                tags=[VispTag.input(), VispTag.frame(), VispTag.task("SOLAR_GAIN")]
+                tags=[VispTag.input(), VispTag.frame(), VispTag.task_solar_gain()]
             )
 
 
-def test_basic_corrections(geometric_calibration_task_with_simple_raw_data):
+def test_basic_corrections(geometric_calibration_task, assign_input_dataset_doc_to_task):
     """
     Given: A set of raw solar gain images and necessary intermediate calibrations
     When: Doing basic dark and lamp gain corrections
     Then: The corrections are applied correctly
     """
-    task = geometric_calibration_task_with_simple_raw_data
+    task, readout_exp_times, num_modstates = geometric_calibration_task
+    intermediate_shape = (10, 10)
+    input_shape = (20, 10)
+    dark_signal = 3.0
+    beam_border = input_shape[0] // 2
+    assign_input_dataset_doc_to_task(
+        task, VispInputDatasetParameterValues(visp_beam_border=beam_border)
+    )
+
+    # Intermediate darks needed for corrections
+    for readout_exp_time in readout_exp_times:
+        write_intermediate_darks_to_task(
+            task=task,
+            dark_signal=dark_signal,
+            readout_exp_time=readout_exp_time,
+            data_shape=intermediate_shape,
+        )
+
+    # Write a crazy dark with the wrong readout_exp_time, just to make sure it doesn't get used
+    write_intermediate_darks_to_task(
+        task=task,
+        dark_signal=1e6,
+        readout_exp_time=readout_exp_times[0] ** 2,
+        data_shape=intermediate_shape,
+    )
+
+    simple_data_func = partial(
+        make_simple_darked_array_data,
+        dark_signal=dark_signal,
+        input_data_shape=input_shape,
+        beam_border=task.parameters.beam_border,
+    )
+    write_geometric_lamp_inputs_to_task(
+        task=task,
+        num_modstates=num_modstates,
+        readout_exp_time=readout_exp_times[0],
+        data_shape=input_shape,
+        data_func=simple_data_func,
+    )
+
+    write_geometric_solar_inputs_to_task(
+        task=task,
+        num_modstates=num_modstates,
+        readout_exp_time=readout_exp_times[1],
+        data_shape=input_shape,
+        data_func=simple_data_func,
+    )
+
     task.do_basic_corrections()
     for beam in range(1, task.constants.num_beams + 1):
         for modstate in range(1, task.constants.num_modstates + 1):
             expected = np.ones((10, 10)) + modstate + beam
             solar_array = task.basic_corrected_solar_data(beam=beam, modstate=modstate)
             lamp_array = task.basic_corrected_lamp_data(beam=beam, modstate=modstate)
             np.testing.assert_equal(expected, solar_array)
```

### Comparing `dkist_processing_visp-2.8.2/dkist_processing_visp/tests/test_map_repeats.py` & `dkist_processing_visp-2.9.0/dkist_processing_visp/tests/test_map_repeats.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,95 +2,48 @@
 import re
 from collections import defaultdict
 
 import numpy as np
 import pytest
 from astropy.io import fits
 from astropy.time import Time
-from astropy.time import TimeDelta
 from dkist_header_validator.translator import translate_spec122_to_spec214_l0
 from dkist_processing_common._util.scratch import WorkflowFileSystem
+from dkist_processing_common.codecs.fits import fits_hdulist_encoder
 from dkist_processing_common.parsers.single_value_single_key_flower import (
     SingleValueSingleKeyFlower,
 )
 
 from dkist_processing_visp.models.constants import VispBudName
 from dkist_processing_visp.models.tags import VispStemName
 from dkist_processing_visp.models.tags import VispTag
 from dkist_processing_visp.parsers.map_repeats import MapScanFlower
 from dkist_processing_visp.parsers.map_repeats import NumMapScansBud
 from dkist_processing_visp.parsers.map_repeats import SingleScanStep
 from dkist_processing_visp.parsers.raster_step import RasterScanStepFlower
 from dkist_processing_visp.parsers.visp_l0_fits_access import VispL0FitsAccess
 from dkist_processing_visp.tasks.parse import ParseL0VispInputData
 from dkist_processing_visp.tasks.parse import S
-from dkist_processing_visp.tests.conftest import VispHeadersValidObserveFrames
-from dkist_processing_visp.tests.conftest import VispTestingParameters
+from dkist_processing_visp.tests.conftest import VispInputDatasetParameterValues
+from dkist_processing_visp.tests.header_models import VispHeadersValidObserveFrames
 
 
 @pytest.fixture(scope="session")
 def complete_map_headers():
     num_steps = 5
     num_modstates = 4
     num_maps = 3
-    start_time = Time("2020-11-20T12:00:00")
-    dt = TimeDelta(10, format="sec")
-    i = 0
-    header_list = []
-    map_number_list = []
-    for map_scan in range(1, num_maps + 1):
-        for step_num in range(0, num_steps):
-            for modstate in range(1, num_modstates + 1):
-                ds = VispHeadersValidObserveFrames(
-                    dataset_shape=(1, 2, 2),
-                    array_shape=(1, 2, 2),
-                    time_delta=10,
-                    num_raster_steps=num_steps,
-                    raster_step=step_num,
-                    num_modstates=num_modstates,
-                    modstate=modstate,
-                    start_time=(start_time + i * dt).to_datetime(),
-                )
-                header = translate_spec122_to_spec214_l0(next(ds).header())
-                header_list.append(header)
-                map_number_list.append(map_scan)
-                i += 1
-
-    return header_list, num_steps, num_modstates, num_maps
-
-
-@pytest.fixture(scope="session")
-def map_headers_with_missing_steps():
-    num_steps = 2
-    num_modstates = 2
-    num_maps = 3
-    start_time = Time("2020-11-20T12:00:00")
-    dt = TimeDelta(10, format="sec")
-    i = 0
-    header_list = []
-    map_number_list = []
-    for map_scan in range(1, num_maps + 1):
-        for step_num in range(0, num_steps):
-            if step_num == 0 and map_scan == 1:
-                continue
-            for modstate in range(1, num_modstates + 1):
-                ds = VispHeadersValidObserveFrames(
-                    dataset_shape=(1, 2, 2),
-                    array_shape=(1, 2, 2),
-                    time_delta=10,
-                    num_raster_steps=num_steps,
-                    raster_step=step_num,
-                    num_modstates=num_modstates,
-                    modstate=modstate,
-                    start_time=(start_time + i * dt).to_datetime(),
-                )
-                header = translate_spec122_to_spec214_l0(next(ds).header())
-                header_list.append(header)
-                map_number_list.append(map_scan)
-                i += 1
+    dataset = VispHeadersValidObserveFrames(
+        array_shape=(1, 2, 2),
+        time_delta=10,
+        num_maps=num_maps,
+        num_raster_steps=num_steps,
+        num_modstates=num_modstates,
+    )
+    header_list = [translate_spec122_to_spec214_l0(d.header()) for d in dataset]
 
     return header_list, num_steps, num_modstates, num_maps
 
 
 @pytest.fixture()
 def organized_fits_access_dict(complete_map_headers):
     all_dict = defaultdict(lambda: defaultdict(list))
@@ -98,14 +51,38 @@
     for header in complete_map_headers[0]:
         fits_obj = VispL0FitsAccess.from_header(header)
         all_dict[fits_obj.raster_scan_step][fits_obj.modulator_state].append(fits_obj)
 
     return all_dict
 
 
+def write_obs_frames_with_multiple_exp_per_step_to_task(task, num_exp: int):
+    array_shape = (1, 2, 2)
+    num_maps = 2
+    num_steps = 3
+    num_modstates = 1
+    dataset = VispHeadersValidObserveFrames(
+        array_shape=array_shape,
+        time_delta=10,
+        num_maps=num_maps,
+        num_raster_steps=num_steps,
+        num_modstates=num_modstates,
+    )
+    header_list = [translate_spec122_to_spec214_l0(d.header()) for d in dataset]
+    for header in header_list:
+        hdu = fits.PrimaryHDU(data=np.ones(array_shape), header=fits.Header(header))
+        hdul = fits.HDUList([hdu])
+
+        # Make multiple exposures by just writing the same header twice
+        for _ in range(num_exp):
+            task.write(
+                data=hdul, tags=[VispTag.input(), VispTag.frame()], encoder=fits_hdulist_encoder
+            )
+
+
 class ParseTaskJustMapStuff(ParseL0VispInputData):
     @property
     def constant_buds(self) -> list[S]:
         return [NumMapScansBud()]
 
     @property
     def tag_flowers(self) -> list[S]:
@@ -115,113 +92,30 @@
             SingleValueSingleKeyFlower(
                 tag_stem_name=VispStemName.modstate.value, metadata_key="modulator_state"
             ),
         ]
 
 
 @pytest.fixture()
-def map_only_parse_task_with_correct_map(
-    complete_map_headers, tmp_path_factory, recipe_run_id, assign_input_dataset_doc_to_task
-):
+def map_only_parse_task(tmp_path_factory, recipe_run_id, assign_input_dataset_doc_to_task):
 
-    complete_headers, num_steps, num_modstates, num_maps = complete_map_headers
     with ParseTaskJustMapStuff(
         recipe_run_id=recipe_run_id, workflow_name="parse_map_scans", workflow_version="X.Y.Z"
     ) as task:
         try:
-            task._scratch = WorkflowFileSystem(
+            task.scratch = WorkflowFileSystem(
                 scratch_base_path=tmp_path_factory.mktemp("map_scan"), recipe_run_id=recipe_run_id
             )
-            assign_input_dataset_doc_to_task(task, VispTestingParameters())
-            for header in complete_headers:
-                hdu = fits.PrimaryHDU(data=np.ones((1, 2, 2)), header=fits.Header(header))
-                hdul = fits.HDUList([hdu])
-                task.fits_data_write(hdu_list=hdul, tags=[VispTag.input(), VispTag.frame()])
-
-            yield task, num_steps, num_modstates, num_maps
-        except:
-            raise
-        finally:
-            task._purge()
-
-
-@pytest.fixture()
-def map_only_parse_task_with_missing_steps(
-    map_headers_with_missing_steps,
-    tmp_path_factory,
-    recipe_run_id,
-    assign_input_dataset_doc_to_task,
-):
+            assign_input_dataset_doc_to_task(task, VispInputDatasetParameterValues())
 
-    complete_headers, num_steps, num_modstates, num_maps = map_headers_with_missing_steps
-    with ParseTaskJustMapStuff(
-        recipe_run_id=recipe_run_id, workflow_name="parse_map_scans", workflow_version="X.Y.Z"
-    ) as task:
-        try:
-            task._scratch = WorkflowFileSystem(
-                scratch_base_path=tmp_path_factory.mktemp("map_scan"), recipe_run_id=recipe_run_id
-            )
-            assign_input_dataset_doc_to_task(task, VispTestingParameters())
-            for header in complete_headers:
-                hdu = fits.PrimaryHDU(data=np.ones((1, 2, 2)), header=fits.Header(header))
-                hdul = fits.HDUList([hdu])
-                task.fits_data_write(hdu_list=hdul, tags=[VispTag.input(), VispTag.frame()])
+            yield task
 
-            yield task, num_steps, num_modstates, num_maps
         except:
             raise
-        finally:
-            task._purge()
-
 
-@pytest.fixture
-def map_only_parse_task_with_multiple_exposures_per_raster_step(
-    tmp_path, recipe_run_id, assign_input_dataset_doc_to_task
-):
-    num_steps = 4
-    num_exp = 3
-    num_modstates = 2
-    start_time = Time("1946-11-20T12:00:00")
-    dt = TimeDelta(10, format="sec")
-    i = 0
-    with ParseTaskJustMapStuff(
-        recipe_run_id=recipe_run_id,
-        workflow_name="parse_visp_input_data",
-        workflow_version="VX.Y",
-    ) as task:
-        try:  # This try... block is here to make sure the dbs get cleaned up if there's a failure in the fixture
-            task._scratch = WorkflowFileSystem(
-                scratch_base_path=tmp_path, recipe_run_id=recipe_run_id
-            )
-            assign_input_dataset_doc_to_task(task, VispTestingParameters())
-            for s in range(num_steps):
-                for m in range(1, num_modstates + 1):
-                    ds = VispHeadersValidObserveFrames(
-                        dataset_shape=(num_exp, 2, 2),
-                        array_shape=(1, 2, 2),
-                        time_delta=0,  # This is where we produce multiple exposures
-                        num_raster_steps=num_steps,
-                        raster_step=s,
-                        num_modstates=num_modstates,
-                        modstate=m,
-                        polarimeter_mode="observe_polarimetric",
-                        start_time=(start_time + i * dt).to_datetime(),
-                    )
-                    for d in ds:
-                        header = d.header()
-                        translated_header = translate_spec122_to_spec214_l0(header)
-                        hdu = fits.PrimaryHDU(
-                            data=np.ones((1, 2, 2)), header=fits.Header(translated_header)
-                        )
-                        hdul = fits.HDUList([hdu])
-                        task.fits_data_write(hdu_list=hdul, tags=[VispTag.input(), VispTag.frame()])
-                    i += 1
-            yield task, num_exp
-        except:
-            raise
         finally:
             task._purge()
 
 
 def test_singlescanstep_correct(organized_fits_access_dict):
     """
     :Given: A group of FitsAccess objects corresponding to multiple map scans with unique frames
@@ -241,21 +135,28 @@
     flat_obj_list = sum(
         sum([list(md.values()) for md in organized_fits_access_dict.values()], []), []
     )
     # I.e., the entire set of values is identical to the unique set of values
     assert len(set(flat_obj_list)) == len(flat_obj_list)
 
 
-def test_parse_map_repeats(map_only_parse_task_with_correct_map):
+def test_parse_map_repeats(map_only_parse_task, complete_map_headers):
     """
     :Given: A map-parsing task with files that represent complete maps
     :When: Parsing the files
     :Then: The correct number of map scans is inferred and each file is tagged correctly
     """
-    task, num_steps, num_modstates, num_maps = map_only_parse_task_with_correct_map
+    task = map_only_parse_task
+    complete_headers, num_steps, num_modstates, num_maps = complete_map_headers
+
+    for header in complete_headers:
+        hdu = fits.PrimaryHDU(data=np.ones((1, 2, 2)), header=fits.Header(header))
+        hdul = fits.HDUList([hdu])
+        task.write(data=hdul, tags=[VispTag.input(), VispTag.frame()], encoder=fits_hdulist_encoder)
+
     task()
 
     assert task.constants._db_dict[VispBudName.num_map_scans.value] == num_maps
     for step in range(0, num_steps):
         for modstate in range(1, num_modstates + 1):
             files = list(
                 task.read(
@@ -279,22 +180,24 @@
             time_list = [Time(VispL0FitsAccess.from_path(f).time_obs) for f in files]
             map_idx = np.argsort(map_scan_tags)
             time_idx = np.argsort(time_list)
             assert np.array_equal(time_idx, map_idx)
 
 
 def test_multiple_exp_per_step_raises_error(
-    map_only_parse_task_with_multiple_exposures_per_raster_step,
+    map_only_parse_task,
 ):
     """
     :Given: A map-parsing task with data that has multiple exposures per (raster, modstate, map_scan)
     :When: Calling the parse task
     :Then: The correct error is raised
     """
-    task, num_exp = map_only_parse_task_with_multiple_exposures_per_raster_step
+    task = map_only_parse_task
+    num_exp = 3
+    write_obs_frames_with_multiple_exp_per_step_to_task(task=task, num_exp=num_exp)
     with pytest.raises(
         ValueError,
         match=re.escape(
             f"More than one exposure detected for a single map scan of a single map step. (Randomly chosen step has {num_exp} exposures)."
         ),
     ):
         task()
```

### Comparing `dkist_processing_visp-2.8.2/dkist_processing_visp/tests/test_parameters.py` & `dkist_processing_visp-2.9.0/dkist_processing_visp/tests/test_parameters.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,69 +1,106 @@
 from dataclasses import asdict
+from dataclasses import dataclass
 
 import numpy as np
 import pytest
 from hypothesis import example
 from hypothesis import given
 from hypothesis import HealthCheck
 from hypothesis import settings
 from hypothesis import strategies as st
 
+from dkist_processing_visp.models.parameters import VispParameters
+from dkist_processing_visp.models.parameters import VispParsingParameters
 from dkist_processing_visp.tasks.visp_base import VispTaskBase
 from dkist_processing_visp.tests.conftest import VispConstantsDb
-from dkist_processing_visp.tests.conftest import VispTestingParameters
+from dkist_processing_visp.tests.conftest import VispInputDatasetParameterValues
+
+# The property names of all parameters on `VispParsingParameters`
+PARSE_PARAMETER_NAMES = [
+    k for k, v in vars(VispParsingParameters).items() if isinstance(v, property)
+]
 
 
 @pytest.fixture(scope="function")
 def basic_science_task_with_parameter_mixin(
     recipe_run_id, assign_input_dataset_doc_to_task, init_visp_constants_db
 ):
-    class Task(VispTaskBase):
-        def run(self):
-            ...
-
-    init_visp_constants_db(recipe_run_id, VispConstantsDb())
-    task = Task(
-        recipe_run_id=recipe_run_id,
-        workflow_name="parse_visp_input_data",
-        workflow_version="VX.Y",
-    )
-    try:  # This try... block is here to make sure the dbs get cleaned up if there's a failure in the fixture
-        assign_input_dataset_doc_to_task(task, VispTestingParameters())
-        yield task, VispTestingParameters()
-    except:
-        raise
-    finally:
-        task._purge()
+    def make_task(parameters_part: dataclass, parameter_class=VispParameters):
+        class Task(VispTaskBase):
+            def run(self):
+                ...
+
+        init_visp_constants_db(recipe_run_id, VispConstantsDb())
+        task = Task(
+            recipe_run_id=recipe_run_id,
+            workflow_name="parse_visp_input_data",
+            workflow_version="VX.Y",
+        )
+        try:  # This try... block is here to make sure the dbs get cleaned up if there's a failure in the fixture
+            assign_input_dataset_doc_to_task(task, parameters_part, parameter_class=parameter_class)
+            yield task, parameters_part
+        except:
+            raise
+        finally:
+            task._purge()
+
+    return make_task
 
 
 def test_non_wave_parameters(basic_science_task_with_parameter_mixin):
     """
     Given: A Science task with the parameter mixin
     When: Accessing properties for parameters that do not depend on wavelength
     Then: The correct value is returned
     """
-    task, expected = basic_science_task_with_parameter_mixin
+    task, expected = next(
+        basic_science_task_with_parameter_mixin(VispInputDatasetParameterValues())
+    )
     task_param_attr = task.parameters
     for pn, pv in asdict(expected).items():
-        if type(pv) is not dict:  # Don't test wavelength dependent parameters
-            assert getattr(task_param_attr, pn.replace("visp_", "")) == pv
+        property_name = pn.removeprefix("visp_")
+        if (
+            type(pv) is not dict and property_name not in PARSE_PARAMETER_NAMES
+        ):  # Don't test wavelength dependent parameters
+            assert getattr(task_param_attr, property_name) == pv
+
+
+def test_parse_parameters(basic_science_task_with_parameter_mixin):
+    """
+    Given: A Science task with the parameter mixin
+    When: Accessing properties for parameters that do not depend on wavelength
+    Then: The correct value is returned
+    """
+    task, expected = next(
+        basic_science_task_with_parameter_mixin(
+            VispInputDatasetParameterValues(), parameter_class=VispParsingParameters
+        )
+    )
+    task_param_attr = task.parameters
+    for pn, pv in asdict(expected).items():
+        property_name = pn.removeprefix("visp_")
+        if property_name in PARSE_PARAMETER_NAMES and type(pv) is not dict:
+            assert getattr(task_param_attr, property_name) == pv
 
 
 @given(wave=st.floats(min_value=500.0, max_value=2000.0))
 @settings(suppress_health_check=[HealthCheck.function_scoped_fixture])
 @example(wave=492.5)
 def test_wave_parameters(basic_science_task_with_parameter_mixin, wave):
     """
     Given: A Science task with the paramter mixin
     When: Accessing properties for parameters that depend on wavelength
     Then: The correct value is returned
     """
-    task, expected = basic_science_task_with_parameter_mixin
+    task, expected = next(
+        basic_science_task_with_parameter_mixin(VispInputDatasetParameterValues())
+    )
     task_param_attr = task.parameters
     task_param_attr._wavelength = wave
     pwaves = np.array(expected.visp_solar_zone_normalization_percentile.wavelength)
     midpoints = 0.5 * (pwaves[1:] + pwaves[:-1])
     idx = np.sum(midpoints < wave)
     for pn, pv in asdict(expected).items():
-        if type(pv) is dict:
-            assert getattr(task_param_attr, pn.replace("visp_", "")) == pv["values"][idx]
+        property_name = pn.removeprefix("visp_")
+        if type(pv) is dict and property_name not in PARSE_PARAMETER_NAMES:
+            assert getattr(task_param_attr, property_name) == pv["values"][idx]
```

### Comparing `dkist_processing_visp-2.8.2/dkist_processing_visp/tests/test_parse.py` & `dkist_processing_visp-2.9.0/dkist_processing_visp/tests/test_science.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,448 +1,573 @@
+import json
+import random
 from datetime import datetime
-from datetime import timedelta
-from itertools import chain
 
 import numpy as np
 import pytest
 from astropy.io import fits
-from dkist_header_validator.translator import translate_spec122_to_spec214_l0
+from astropy.time import Time
+from astropy.time import TimeDelta
+from dkist_header_validator import spec122_validator
 from dkist_processing_common._util.scratch import WorkflowFileSystem
+from dkist_processing_common.codecs.fits import fits_array_encoder
+from dkist_processing_common.codecs.fits import fits_hdu_decoder
 from dkist_processing_common.models.tags import Tag
 from dkist_processing_common.tests.conftest import FakeGQLClient
 
-from dkist_processing_visp.tasks.parse import ParseL0VispInputData
-from dkist_processing_visp.tests.conftest import VispHeadersValidDarkFrames
-from dkist_processing_visp.tests.conftest import VispHeadersValidLampGainFrames
-from dkist_processing_visp.tests.conftest import VispHeadersValidObserveFrames
-from dkist_processing_visp.tests.conftest import VispHeadersValidPolcalFrames
-from dkist_processing_visp.tests.conftest import VispHeadersValidSolarGainFrames
-from dkist_processing_visp.tests.conftest import VispTestingParameters
+from dkist_processing_visp.models.tags import VispStemName
+from dkist_processing_visp.models.tags import VispTag
+from dkist_processing_visp.parsers.visp_l0_fits_access import VispL0FitsAccess
+from dkist_processing_visp.tasks.science import CalibrationCollection
+from dkist_processing_visp.tasks.science import ScienceCalibration
+from dkist_processing_visp.tests.conftest import VispConstantsDb
+from dkist_processing_visp.tests.conftest import VispInputDatasetParameterValues
+from dkist_processing_visp.tests.conftest import write_dummy_intermediate_solar_cals_to_task
+from dkist_processing_visp.tests.conftest import write_frames_to_task
+from dkist_processing_visp.tests.conftest import write_intermediate_background_to_task
+from dkist_processing_visp.tests.conftest import write_intermediate_darks_to_task
+from dkist_processing_visp.tests.conftest import write_intermediate_geometric_to_task
+from dkist_processing_visp.tests.header_models import VispHeadersValidObserveFrames
+
+
+def write_demod_matrices_to_task(task, num_modstates: int):
+    demod_matrices = np.zeros((4, num_modstates)) + np.array([1, 2, 3, 4])[:, None]
+    for beam in [1, 2]:
+        task.write(
+            data=demod_matrices,
+            tags=[
+                VispTag.intermediate(),
+                VispTag.frame(),
+                VispTag.task_demodulation_matrices(),
+                VispTag.beam(beam),
+            ],
+            encoder=fits_array_encoder,
+        )
+
+
+def tag_on_modstate_raster_map(frame: VispHeadersValidObserveFrames) -> list[str]:
+    modstate = frame.current_modstate("")  # Weird signature due to key_function
+    raster_step = frame.current_raster_step("")
+    map_scan = frame.current_map
+
+    return [
+        VispTag.modstate(modstate),
+        VispTag.raster_step(raster_step),
+        VispTag.map_scan(map_scan),
+    ]
+
+
+def write_input_observe_frames_to_task(
+    task,
+    readout_exp_time: float,
+    num_modstates: int,
+    num_raster_steps: int,
+    num_maps: int,
+    data_shape: tuple[int, int],
+):
+    array_shape = (1, *data_shape)
+    dataset = VispHeadersValidObserveFrames(
+        array_shape=array_shape,
+        time_delta=10,
+        num_modstates=num_modstates,
+        num_raster_steps=num_raster_steps,
+        num_maps=num_maps,
+    )
+    write_frames_to_task(
+        task=task,
+        frame_generator=dataset,
+        extra_tags=[
+            VispTag.input(),
+            VispTag.readout_exp_time(readout_exp_time),
+            VispTag.task_observe(),
+        ],
+        tag_func=tag_on_modstate_raster_map,
+    )
 
 
-@pytest.fixture(scope="function")
-def parse_inputs_valid_task(tmp_path, recipe_run_id, assign_input_dataset_doc_to_task):
-    num_maps = 1
-    num_modstates = 2
-    num_steps = 3
-    with ParseL0VispInputData(
-        recipe_run_id=recipe_run_id,
-        workflow_name="parse_visp_input_data",
-        workflow_version="VX.Y",
-    ) as task:
-        try:  # This try... block is here to make sure the dbs get cleaned up if there's a failure in the fixture
-            task._scratch = WorkflowFileSystem(
-                scratch_base_path=tmp_path, recipe_run_id=recipe_run_id
-            )
-            assign_input_dataset_doc_to_task(task, VispTestingParameters())
-            ds1 = VispHeadersValidDarkFrames(
-                dataset_shape=(2, 2, 2), array_shape=(1, 2, 2), time_delta=10
-            )
-            ds2 = VispHeadersValidLampGainFrames(
-                dataset_shape=(2, 2, 2),
-                array_shape=(2, 2, 1),
-                time_delta=10,
-                num_modstates=2,
-                modstate=1,
-            )
-            ds3 = VispHeadersValidSolarGainFrames(
-                dataset_shape=(2, 2, 2),
-                array_shape=(2, 2, 1),
-                time_delta=10,
-                num_modstates=2,
-                modstate=1,
-            )
-            ds4 = VispHeadersValidPolcalFrames(
-                dataset_shape=(2, 2, 2),
-                array_shape=(2, 2, 1),
-                time_delta=30,
-                num_modstates=2,
-                modstate=1,
-            )
-            ds = chain(ds1, ds2, ds3, ds4)
-            for d in ds:
-                header = d.header()
-                translated_header = translate_spec122_to_spec214_l0(header)
-                hdu = fits.PrimaryHDU(
-                    data=np.ones((1, 2, 2)), header=fits.Header(translated_header)
-                )
-                hdul = fits.HDUList([hdu])
-                task.fits_data_write(hdu_list=hdul, tags=[Tag.input(), Tag.frame()])
-
-            start_time = datetime.now()
-            time_delta = timedelta(seconds=10)
-            i = 0
-            for map_scan in range(1, num_maps + 1):
-                for m in range(1, num_modstates + 1):
-                    for s in range(num_steps):
-                        ds = VispHeadersValidObserveFrames(
-                            dataset_shape=(2, 2, 2),
-                            array_shape=(1, 2, 2),
-                            time_delta=10,
-                            num_raster_steps=num_steps,
-                            raster_step=s,
-                            num_modstates=num_modstates,
-                            modstate=m,
-                            polarimeter_mode="observe_polarimetric",
-                            start_time=start_time + i * time_delta,
-                        )
-                        header = next(ds).header()
-                        header["CAM__004"] = [0.02, 0.03][m % 2]
-                        header["CAM__005"] = [0.04, 0.06][m % 2]
-                        translated_header = translate_spec122_to_spec214_l0(header)
-                        hdu = fits.PrimaryHDU(
-                            data=np.ones((1, 2, 2)), header=fits.Header(translated_header)
-                        )
-                        hdul = fits.HDUList([hdu])
-                        task.fits_data_write(hdu_list=hdul, tags=[Tag.input(), Tag.frame()])
-                        i += 1
-            yield task
-        except:
-            raise
-        finally:
-            task._purge()
+def get_input_obs_frame_header(task):
+
+    tags = [VispTag.input(), VispTag.task_observe()]
+    random_hdu = next(task.read(tags=tags, decoder=fits_hdu_decoder))
+    return random_hdu.header
 
 
-@pytest.fixture
-def parse_task_with_multi_num_raster_steps(
-    tmp_path, recipe_run_id, assign_input_dataset_doc_to_task
+@pytest.fixture(scope="function", params=["Full Stokes", "Stokes-I"])
+def science_calibration_task(
+    tmp_path,
+    recipe_run_id,
+    init_visp_constants_db,
+    request,
 ):
-    num_steps = 4
     num_map_scans = 2
-    num_modstates = 2
-    with ParseL0VispInputData(
-        recipe_run_id=recipe_run_id,
-        workflow_name="parse_visp_input_data",
-        workflow_version="VX.Y",
+    num_raster_steps = 2
+    readout_exp_time = 0.04
+    if request.param == "Full Stokes":
+        num_modstates = 2
+        polarimeter_mode = "observe_polarimetric"
+    else:
+        num_modstates = 1
+        polarimeter_mode = "observe_intensity"
+
+    constants_db = VispConstantsDb(
+        POLARIMETER_MODE=polarimeter_mode,
+        NUM_MODSTATES=num_modstates,
+        NUM_MAP_SCANS=num_map_scans,
+        NUM_RASTER_STEPS=num_raster_steps,
+        NUM_BEAMS=2,
+        OBSERVE_READOUT_EXP_TIMES=(readout_exp_time,),
+    )
+    init_visp_constants_db(recipe_run_id, constants_db)
+    with ScienceCalibration(
+        recipe_run_id=recipe_run_id, workflow_name="science_calibration", workflow_version="VX.Y"
     ) as task:
         try:  # This try... block is here to make sure the dbs get cleaned up if there's a failure in the fixture
-            task._scratch = WorkflowFileSystem(
+            task.scratch = WorkflowFileSystem(
                 scratch_base_path=tmp_path, recipe_run_id=recipe_run_id
             )
-            assign_input_dataset_doc_to_task(task, VispTestingParameters())
-            for map_scan in range(1, num_map_scans + 1):
-                for m in range(1, num_modstates + 1):
-                    for s in range(num_steps):
-                        ds = VispHeadersValidObserveFrames(
-                            dataset_shape=(2, 2, 2),
-                            array_shape=(1, 2, 2),
-                            time_delta=10,
-                            num_raster_steps=num_steps,
-                            raster_step=s,
-                            num_modstates=num_modstates,
-                            modstate=m,
-                            polarimeter_mode="observe_polarimetric",
-                        )
-                        header = next(ds).header()
-                        translated_header = translate_spec122_to_spec214_l0(header)
-                        translated_header["VSPNSTP"] = s % 3
-                        hdu = fits.PrimaryHDU(
-                            data=np.ones((1, 2, 2)), header=fits.Header(translated_header)
-                        )
-                        hdul = fits.HDUList([hdu])
-                        task.fits_data_write(hdu_list=hdul, tags=[Tag.input(), Tag.frame()])
-            yield task
+
+            yield task, request.param, readout_exp_time, num_map_scans, num_raster_steps, num_modstates
         except:
             raise
         finally:
             task._purge()
 
 
-@pytest.fixture
-def parse_task_with_incomplete_final_map(tmp_path, recipe_run_id, assign_input_dataset_doc_to_task):
-    num_steps = 4
-    num_map_scans = 3
-    num_modstates = 2
-    with ParseL0VispInputData(
-        recipe_run_id=recipe_run_id,
-        workflow_name="parse_visp_input_data",
-        workflow_version="VX.Y",
-    ) as task:
-        try:  # This try... block is here to make sure the dbs get cleaned up if there's a failure in the fixture
-            task._scratch = WorkflowFileSystem(
-                scratch_base_path=tmp_path, recipe_run_id=recipe_run_id
-            )
-            assign_input_dataset_doc_to_task(task, VispTestingParameters())
-            for map_scan in range(1, num_map_scans):
-                for m in range(1, num_modstates + 1):
-                    for s in range(num_steps):
-                        ds = VispHeadersValidObserveFrames(
-                            dataset_shape=(2, 2, 2),
-                            array_shape=(1, 2, 2),
-                            time_delta=10,
-                            num_raster_steps=num_steps,
-                            raster_step=s,
-                            num_modstates=num_modstates,
-                            modstate=m,
-                            polarimeter_mode="observe_polarimetric",
-                        )
-                        header = next(ds).header()
-                        translated_header = translate_spec122_to_spec214_l0(header)
-                        hdu = fits.PrimaryHDU(
-                            data=np.ones((1, 2, 2)), header=fits.Header(translated_header)
-                        )
-                        hdul = fits.HDUList([hdu])
-                        task.fits_data_write(hdu_list=hdul, tags=[Tag.input(), Tag.frame()])
-            # Now do the incomplete map
-            for map_scan in range(num_map_scans, num_map_scans + 1):
-                for m in range(1, num_modstates + 1):
-                    for s in range(num_steps - 1):  # One step is missing in the last map
-                        ds = VispHeadersValidObserveFrames(
-                            dataset_shape=(2, 2, 2),
-                            array_shape=(1, 2, 2),
-                            time_delta=10,
-                            num_raster_steps=num_steps,
-                            raster_step=s,
-                            num_modstates=num_modstates,
-                            modstate=m,
-                            polarimeter_mode="observe_polarimetric",
-                        )
-                        header = next(ds).header()
-                        translated_header = translate_spec122_to_spec214_l0(header)
-                        hdu = fits.PrimaryHDU(
-                            data=np.ones((1, 2, 2)), header=fits.Header(translated_header)
-                        )
-                        hdul = fits.HDUList([hdu])
-                        task.fits_data_write(hdu_list=hdul, tags=[Tag.input(), Tag.frame()])
-            yield task, num_steps, num_map_scans
-        except:
-            raise
-        finally:
-            task._purge()
+@pytest.fixture(scope="function")
+def dummy_calibration_collection():
+    input_shape = (50, 20)
+    intermediate_shape = (25, 20)
+
+    beam = 1
+    modstate = 1
+
+    dark_dict = {VispTag.beam(beam): {VispTag.readout_exp_time(0.04): np.zeros(intermediate_shape)}}
+    background_dict = {VispTag.beam(beam): np.zeros(intermediate_shape)}
+    solar_dict = {VispTag.beam(beam): {VispTag.modstate(modstate): np.ones(intermediate_shape)}}
+    angle_dict = {VispTag.beam(beam): 0.0}
+    spec_dict = {VispTag.beam(beam): np.zeros(intermediate_shape[1])}
+    offset_dict = {VispTag.beam(beam): {VispTag.modstate(modstate): np.zeros(2)}}
+
+    collection = CalibrationCollection(
+        dark=dark_dict,
+        background=background_dict,
+        solar_gain=solar_dict,
+        angle=angle_dict,
+        spec_shift=spec_dict,
+        state_offset=offset_dict,
+        demod_matrices=None,
+    )
 
+    return collection, input_shape, intermediate_shape
 
-@pytest.fixture
-def parse_task_with_incomplete_raster_scan(
-    tmp_path, recipe_run_id, assign_input_dataset_doc_to_task
-):
-    num_steps = 4
-    num_maps = 1
-    num_modstates = 2
-    with ParseL0VispInputData(
-        recipe_run_id=recipe_run_id,
-        workflow_name="parse_visp_input_data",
-        workflow_version="VX.Y",
-    ) as task:
-        try:  # This try... block is here to make sure the dbs get cleaned up if there's a failure in the fixture
-            task._scratch = WorkflowFileSystem(
-                scratch_base_path=tmp_path, recipe_run_id=recipe_run_id
-            )
-            assign_input_dataset_doc_to_task(task, VispTestingParameters())
-            for map_scan in range(1, num_maps + 1):
-                for m in range(1, num_modstates + 1):
-                    for s in range(num_steps):
-                        ds = VispHeadersValidObserveFrames(
-                            dataset_shape=(2, 2, 2),
-                            array_shape=(1, 2, 2),
-                            time_delta=10,
-                            num_raster_steps=num_steps,
-                            raster_step=s,
-                            num_modstates=num_modstates,
-                            modstate=m,
-                            polarimeter_mode="observe_polarimetric",
-                        )
-                        header = next(ds).header()
-                        translated_header = translate_spec122_to_spec214_l0(header)
-                        translated_header["VSPNSTP"] = num_steps + 10
-                        hdu = fits.PrimaryHDU(
-                            data=np.ones((1, 2, 2)), header=fits.Header(translated_header)
-                        )
-                        hdul = fits.HDUList([hdu])
-                        task.fits_data_write(hdu_list=hdul, tags=[Tag.input(), Tag.frame()])
-            yield task, num_steps, num_maps
-        except:
-            raise
-        finally:
-            task._purge()
 
+@pytest.fixture(scope="session")
+def headers_with_dates() -> tuple[list[fits.Header], str, int, int]:
+    num_headers = 5
+    start_time = "1969-12-06T18:00:00"
+    exp_time = 12
+    time_delta = 10
+    ds = VispHeadersValidObserveFrames(
+        array_shape=(1, 4, 4),
+        time_delta=time_delta,
+        num_maps=num_headers,
+        num_raster_steps=1,
+        num_modstates=1,
+        start_time=datetime.fromisoformat(start_time),
+    )
+    headers = [
+        spec122_validator.validate_and_translate_to_214_l0(d.header(), return_type=fits.HDUList)[
+            0
+        ].header
+        for d in ds
+    ]
+    random.shuffle(headers)  # Shuffle to make sure they're not already in time order
+    for h in headers:
+        h["XPOSURE"] = exp_time  # Exposure time, in ms
+
+    return headers, start_time, exp_time, time_delta
+
+
+@pytest.fixture(scope="session")
+def compressed_headers_with_dates(headers_with_dates) -> tuple[list[fits.Header], str, int, int]:
+    headers, start_time, exp_time, time_delta = headers_with_dates
+    comp_headers = [fits.hdu.compressed.CompImageHeader(h, h) for h in headers]
+    return comp_headers, start_time, exp_time, time_delta
 
-@pytest.fixture
-def parse_task_with_intensity_observes_and_polarmetric_cals(
-    tmp_path, recipe_run_id, assign_input_dataset_doc_to_task
-):
-    num_maps = 1
-    num_observe_modstates = 1
-    num_calibration_modstates = 2
-    num_raster_steps = 3
-    with ParseL0VispInputData(
-        recipe_run_id=recipe_run_id,
-        workflow_name="parse_visp_input_data",
-        workflow_version="VX.Y",
-    ) as task:
-        try:  # This try... block is here to make sure the dbs get cleaned up if there's a failure in the fixture
-            task._scratch = WorkflowFileSystem(
-                scratch_base_path=tmp_path, recipe_run_id=recipe_run_id
-            )
-            assign_input_dataset_doc_to_task(task, VispTestingParameters())
-            for map_scan in range(num_maps + 1):
-                for raster_step in range(num_raster_steps + 1):
-                    for observe_modstate in range(1, num_observe_modstates + 1):
-                        ds = VispHeadersValidObserveFrames(
-                            dataset_shape=(2, 2, 2),
-                            array_shape=(1, 2, 2),
-                            time_delta=10,
-                            num_modstates=num_observe_modstates,
-                            modstate=observe_modstate,
-                            num_raster_steps=num_raster_steps,
-                            raster_step=raster_step,
-                            polarimeter_mode="observe_intensity",
-                        )
-                        header = next(ds).header()
-                        translated_header = translate_spec122_to_spec214_l0(header)
-                        hdu = fits.PrimaryHDU(
-                            data=np.ones((1, 2, 2)), header=fits.Header(translated_header)
-                        )
-                        hdul = fits.HDUList([hdu])
-                        task.fits_data_write(hdu_list=hdul, tags=[Tag.input(), Tag.frame()])
-                    for calibration_modstate in range(1, num_calibration_modstates + 1):
-                        ds = VispHeadersValidLampGainFrames(
-                            dataset_shape=(2, 2, 2),
-                            array_shape=(1, 2, 2),
-                            time_delta=10,
-                            num_modstates=num_calibration_modstates,
-                            modstate=calibration_modstate,
-                            polarimeter_mode="dark_polarimetric",
-                        )
-                        header = next(ds).header()
-                        translated_header = translate_spec122_to_spec214_l0(header)
-                        hdu = fits.PrimaryHDU(
-                            data=np.ones((1, 2, 2)), header=fits.Header(translated_header)
-                        )
-                        hdul = fits.HDUList([hdu])
-                        task.fits_data_write(hdu_list=hdul, tags=[Tag.input(), Tag.frame()])
-            yield task
-        except:
-            raise
-        finally:
-            task._purge()
 
+@pytest.fixture(scope="function")
+def calibration_collection_with_geo_shifts(shifts) -> CalibrationCollection:
+    num_beams, num_mod, _ = shifts.shape
+    geo_shifts = {
+        str(b + 1): {f"m{m + 1}": shifts[b, m, :] for m in range(num_mod)} for b in range(num_beams)
+    }
+    return CalibrationCollection(
+        dark=dict(),
+        background=dict(),
+        solar_gain=dict(),
+        angle=dict(),
+        state_offset=geo_shifts,
+        spec_shift=dict(),
+        demod_matrices=None,
+    )
+
+
+@pytest.fixture(scope="session")
+def calibrated_array_and_header_dicts(
+    headers_with_dates,
+) -> tuple[dict[str, np.ndarray], dict[str, fits.Header]]:
+    headers = headers_with_dates[0]
+    header = headers[0]
+
+    # It's kind of a hack to have the stokes dimension here; spectrographic data will not have this, but it actually
+    # doesn't matter
+    shape = (10, 10, 4)
+    beam1 = np.ones(shape) + np.arange(4)[None, None, :]
+    beam2 = np.ones(shape) + np.arange(4)[::-1][None, None, :]
+
+    array_dict = {VispTag.beam(1): beam1, VispTag.beam(2): beam2}
+    header_dict = {VispTag.beam(1): header, VispTag.beam(2): header}
+
+    return array_dict, header_dict
 
-def test_parse_visp_input_data(parse_inputs_valid_task, mocker):
+
+@pytest.fixture(scope="function")
+def calibration_collection_with_full_overlap_slice() -> CalibrationCollection:
+    shifts = np.array([[[0.0, 0.0]], [[0.0, 0.0]]])
+    num_beams, num_mod, _ = shifts.shape
+    geo_shifts = {
+        str(b + 1): {f"m{m + 1}": shifts[b, m, :] for m in range(num_mod)} for b in range(num_beams)
+    }
+    return CalibrationCollection(
+        dark=dict(),
+        background=dict(),
+        solar_gain=dict(),
+        angle=dict(),
+        state_offset=geo_shifts,
+        spec_shift=dict(),
+        demod_matrices=None,
+    )
+
+
+@pytest.mark.parametrize(
+    "background_on",
+    [pytest.param(True, id="Background on"), pytest.param(False, id="Background off")],
+)
+def test_science_calibration_task(
+    science_calibration_task, background_on, assign_input_dataset_doc_to_task, mocker
+):
     """
-    Given: A ParseVispInputData task
+    Given: A ScienceCalibration task
     When: Calling the task instance
-    Then: All tagged files exist and individual task tags are applied
+    Then: There are the expected number of science frames with the correct tags applied and the headers have been correctly updated
     """
+
     mocker.patch(
         "dkist_processing_common.tasks.mixin.metadata_store.GraphQLClient", new=FakeGQLClient
     )
+
     # When
-    parse_inputs_valid_task()
-    # Then
-    translated_input_files = parse_inputs_valid_task.read(tags=[Tag.input(), Tag.frame()])
-    for filepath in translated_input_files:
-        assert filepath.exists()
+    (
+        task,
+        polarization_mode,
+        readout_exp_time,
+        num_maps,
+        num_raster_steps,
+        num_modstates,
+    ) = science_calibration_task
+    input_shape = (50, 20)
+    intermediate_shape = (25, 20)
+    beam_border = input_shape[0] // 2
+    assign_input_dataset_doc_to_task(
+        task,
+        VispInputDatasetParameterValues(
+            visp_background_on=background_on, visp_beam_border=beam_border
+        ),
+    )
 
-    assert list(parse_inputs_valid_task.read(tags=[Tag.input(), Tag.task("DARK")]))
-    assert list(parse_inputs_valid_task.read(tags=[Tag.input(), Tag.task("LAMP_GAIN")]))
-    assert list(parse_inputs_valid_task.read(tags=[Tag.input(), Tag.task("SOLAR_GAIN")]))
-    assert list(parse_inputs_valid_task.read(tags=[Tag.input(), Tag.task("POLCAL")]))
-    assert list(parse_inputs_valid_task.read(tags=[Tag.input(), Tag.task("OBSERVE")]))
+    offsets = np.tile(np.array([-10.2, 5.1]), (2, num_modstates, 1))
+    offsets[0] = 0.0  # So beam 1 has zero offset
 
+    write_intermediate_darks_to_task(
+        task=task,
+        dark_signal=0,
+        readout_exp_time=readout_exp_time,
+        data_shape=intermediate_shape,
+    )
+    if background_on:
+        write_intermediate_background_to_task(
+            task=task, background_signal=0.0, data_shape=intermediate_shape
+        )
 
-def test_parse_visp_input_data_constants(parse_inputs_valid_task, mocker):
-    """
-    Given: A ParseVispInputData task
-    When: Calling the task instance
-    Then: Constants are in the constants object as expected
-    """
-    mocker.patch(
-        "dkist_processing_common.tasks.mixin.metadata_store.GraphQLClient", new=FakeGQLClient
+    write_intermediate_geometric_to_task(
+        task=task, num_modstates=num_modstates, data_shape=intermediate_shape, offsets=offsets
     )
-    # When
-    parse_inputs_valid_task()
-    # Then
-    assert parse_inputs_valid_task.constants._db_dict["OBS_IP_START_TIME"] == "2022-11-28T13:55:00"
-    assert parse_inputs_valid_task.constants._db_dict["NUM_MODSTATES"] == 2
-    assert parse_inputs_valid_task.constants._db_dict["NUM_MAP_SCANS"] == 1
-    assert parse_inputs_valid_task.constants._db_dict["NUM_RASTER_STEPS"] == 3
-    assert parse_inputs_valid_task.constants._db_dict["WAVELENGTH"] == 656.28
-    assert parse_inputs_valid_task.constants._db_dict["DARK_EXPOSURE_TIMES"] == [1.0]
-    assert parse_inputs_valid_task.constants._db_dict["LAMP_EXPOSURE_TIMES"] == [10.0]
-    assert parse_inputs_valid_task.constants._db_dict["SOLAR_EXPOSURE_TIMES"] == [20.0]
-    assert parse_inputs_valid_task.constants._db_dict["POLCAL_EXPOSURE_TIMES"] == [0.01]
-    assert parse_inputs_valid_task.constants._db_dict["OBSERVE_EXPOSURE_TIMES"] == [0.02, 0.03]
-    assert parse_inputs_valid_task.constants._db_dict["DARK_READOUT_EXP_TIMES"] == [2.0]
-    assert parse_inputs_valid_task.constants._db_dict["LAMP_READOUT_EXP_TIMES"] == [20.0]
-    assert parse_inputs_valid_task.constants._db_dict["SOLAR_READOUT_EXP_TIMES"] == [40.0]
-    assert parse_inputs_valid_task.constants._db_dict["POLCAL_READOUT_EXP_TIMES"] == [0.02]
-    assert parse_inputs_valid_task.constants._db_dict["OBSERVE_READOUT_EXP_TIMES"] == [0.04, 0.06]
-
-
-def test_parse_visp_values(parse_inputs_valid_task, mocker):
-    """
-    :Given: A valid parse input task
-    :When: Calling the task instance
-    :Then: Values are correctly loaded into the constants mutable mapping
-    """
-    mocker.patch(
-        "dkist_processing_common.tasks.mixin.metadata_store.GraphQLClient", new=FakeGQLClient
+    write_dummy_intermediate_solar_cals_to_task(
+        task=task, data_shape=intermediate_shape, num_modstates=num_modstates
+    )
+    write_demod_matrices_to_task(task=task, num_modstates=num_modstates)
+    write_input_observe_frames_to_task(
+        task=task,
+        readout_exp_time=readout_exp_time,
+        num_modstates=num_modstates,
+        num_raster_steps=num_raster_steps,
+        num_maps=num_maps,
+        data_shape=input_shape,
     )
-    parse_inputs_valid_task()
-    assert parse_inputs_valid_task.constants.instrument == "VISP"
-    assert parse_inputs_valid_task.constants.average_cadence == 10
-    assert parse_inputs_valid_task.constants.maximum_cadence == 10
-    assert parse_inputs_valid_task.constants.minimum_cadence == 10
-    assert parse_inputs_valid_task.constants.variance_cadence == 0
 
+    input_header = get_input_obs_frame_header(task=task)
 
-def test_multiple_num_raster_steps_raises_error(parse_task_with_multi_num_raster_steps, mocker):
-    """
-    :Given: A prase task with data that have inconsistent VSPNSTP values
-    :When: Calling the parse task
-    :Then: The correct error is raised
-    """
-    mocker.patch(
-        "dkist_processing_common.tasks.mixin.metadata_store.GraphQLClient", new=FakeGQLClient
+    task()
+
+    # 1 from re-dummification
+    expected_final_shape = (
+        1,
+        # The use of np.abs means we can use np.ceil regardless of whether the offset is negative or positive.
+        intermediate_shape[0] - np.ceil(np.abs(offsets[1, 0, 0])),
+        intermediate_shape[1] - np.ceil(np.abs(offsets[1, 0, 1])),
     )
-    with pytest.raises(ValueError, match="Multiple NUM_RASTER_STEPS values found"):
-        parse_task_with_multi_num_raster_steps()
 
+    # Then
+    tags = [
+        VispTag.calibrated(),
+        VispTag.frame(),
+    ]
+    files = list(task.read(tags=tags))
+    if polarization_mode == "Full Stokes":
+        # 2 raster steps * 2 map scans * 4 stokes params = 16 frames
+        assert len(files) == 16
+    elif polarization_mode == "Stokes-I":
+        # 2 raster steps * 2 map scans * 1 stokes param = 4 frames
+        assert len(files) == 4
+    for file in files:
+        hdul = fits.open(file)
+        assert type(hdul[0]) is fits.PrimaryHDU
+        assert type(hdul[1]) is fits.CompImageHDU
+        assert hdul[1].data.shape == expected_final_shape
+        assert "DATE-BEG" in hdul[1].header.keys()
+        assert "DATE-END" in hdul[1].header.keys()
+
+        # Check that map scan keys were updated
+        map_scan = [
+            int(t.split("_")[-1]) for t in task.tags(file) if VispStemName.map_scan.value in t
+        ][0]
+        assert hdul[1].header["VSPNMAPS"] == 2
+        assert hdul[1].header["VSPMAP"] == map_scan
+
+        # Check that WCS keys were updated
+        if offsets[1, 0, 0] > 0:
+            assert hdul[1].header["CRPIX2"] == input_header["CRPIX2"] - np.ceil(offsets[1, 0, 0])
+        if offsets[1, 0, 1] > 0:
+            assert hdul[1].header["CRPIX1"] == input_header["CRPIX1"] - np.ceil(offsets[1, 0, 1])
+
+    quality_files = task.read(tags=[Tag.quality("TASK_TYPES")])
+    for file in quality_files:
+        with file.open() as f:
+            data = json.load(f)
+            assert isinstance(data, dict)
+            assert data["total_frames"] == task.scratch.count_all(
+                tags=[VispTag.input(), VispTag.frame(), VispTag.task_observe()]
+            )
 
-def test_incomplete_single_map(parse_task_with_incomplete_raster_scan, mocker):
-    """
-    :Given: A parse task with data that has an incomplete raster scan
-    :When: Calling the parse task
-    :Then: The correct number of raster steps are found
+
+def test_readout_normalization_correct(
+    science_calibration_task, dummy_calibration_collection, assign_input_dataset_doc_to_task
+):
     """
-    mocker.patch(
-        "dkist_processing_common.tasks.mixin.metadata_store.GraphQLClient", new=FakeGQLClient
+    Given: A ScienceCalibration task with associated observe frames
+    When: Correcting a single array
+    Then: The correct normalization by the number of readouts per FPA is performed
+    """
+    task = science_calibration_task[0]
+    corrections, input_shape, intermediate_shape = dummy_calibration_collection
+    beam_border = input_shape[0] // 2
+    assign_input_dataset_doc_to_task(
+        task, VispInputDatasetParameterValues(visp_beam_border=beam_border)
     )
-    task, num_steps, num_map_scans = parse_task_with_incomplete_raster_scan
-    task()
-    assert task.constants._db_dict["NUM_RASTER_STEPS"] == num_steps
-    assert task.constants._db_dict["NUM_MAP_SCANS"] == num_map_scans
+
+    # Assign a single input observe frame
+    dataset = VispHeadersValidObserveFrames(
+        array_shape=(1, *input_shape),
+        time_delta=10,
+        num_raster_steps=1,
+        num_modstates=1,
+        num_maps=1,
+        start_time=datetime.now(),
+    )
+    readout_exp_time = task.constants.observe_readout_exp_times[0]
+    data_func = lambda frame: np.ones(frame.array_shape) * 100 * frame.header()["CAM__014"]
+    write_frames_to_task(
+        task=task,
+        frame_generator=dataset,
+        extra_tags=[
+            VispTag.task_observe(),
+            VispTag.raster_step(1),
+            VispTag.map_scan(1),
+            VispTag.modstate(1),
+            VispTag.input(),
+            VispTag.readout_exp_time(readout_exp_time),
+        ],
+        data_func=data_func,
+    )
+
+    # When:
+    corrected_array, _ = task.correct_single_frame(
+        beam=1,
+        modstate=1,
+        raster_step=1,
+        map_scan=1,
+        readout_exp_time=readout_exp_time,
+        calibrations=corrections,
+    )
+
+    expected = np.ones(intermediate_shape) * 100.0
+    np.testing.assert_allclose(corrected_array, expected, rtol=1e-15)
 
 
-def test_incomplete_final_map(parse_task_with_incomplete_final_map, mocker):
+def test_compute_date_keys(headers_with_dates, recipe_run_id, init_visp_constants_db):
     """
-    :Given: A parse task with data that has complete raster scans along with an incomplete raster scan
-    :When: Calling the parse task
-    :Then: The correct number of raster steps and maps are found
+    Given: A set of headers with different DATE-OBS values
+    When: Computing the time over which the headers were taken
+    Then: A header with correct DATE-BEG, DATE-END, and DATE-AVG keys is returned
     """
-    mocker.patch(
-        "dkist_processing_common.tasks.mixin.metadata_store.GraphQLClient", new=FakeGQLClient
-    )
-    task, num_steps, num_map_scans = parse_task_with_incomplete_final_map
-    task()
-    assert task.constants._db_dict["NUM_RASTER_STEPS"] == num_steps
-    assert task.constants._db_dict["NUM_MAP_SCANS"] == num_map_scans - 1
+    headers, start_time, exp_time, time_delta = headers_with_dates
+    constants_db = VispConstantsDb()
+    init_visp_constants_db(recipe_run_id, constants_db)
+    with ScienceCalibration(
+        recipe_run_id=recipe_run_id, workflow_name="science_calibration", workflow_version="VX.Y"
+    ) as task:
+        final_header = task._compute_date_keys(headers)
+        final_header_from_single = task._compute_date_keys(headers[0])
+
+    date_end = (
+        Time(start_time)
+        + (len(headers) - 1) * TimeDelta(time_delta, format="sec")
+        + TimeDelta(exp_time / 1000.0, format="sec")
+    ).isot
+
+    assert final_header["DATE-BEG"] == start_time
+    assert final_header["DATE-END"] == date_end
+
+    date_end_from_single = (
+        Time(headers[0]["DATE-BEG"])
+        # + TimeDelta(time_delta, format="sec")
+        + TimeDelta(exp_time / 1000.0, format="sec")
+    ).isot
+
+    assert final_header_from_single["DATE-BEG"] == headers[0]["DATE-BEG"]
+    assert final_header_from_single["DATE-END"] == date_end_from_single
 
 
-def test_intensity_observes_and_polarmetric_cals(
-    parse_task_with_intensity_observes_and_polarmetric_cals, mocker
+def test_compute_date_keys_compressed_headers(
+    compressed_headers_with_dates, recipe_run_id, init_visp_constants_db
 ):
     """
-    :Given: Data where the observe frames are in intensity mode and the calibration frames are in polarimetric mode
-    :When: Parsing the data
-    :Then: All modulator state keys generated for all frames are in the first modulator state
+    Given: A set of compressed headers with different DATE-OBS values
+    When: Computing the time over which the headers were taken
+    Then: A header with correct DATE-BEG, DATE-END, and DATE-AVG keys is returned
+    """
+    headers, start_time, exp_time, time_delta = compressed_headers_with_dates
+    constants_db = VispConstantsDb()
+    init_visp_constants_db(recipe_run_id, constants_db)
+    with ScienceCalibration(
+        recipe_run_id=recipe_run_id, workflow_name="science_calibration", workflow_version="VX.Y"
+    ) as task:
+        final_header = task._compute_date_keys(headers)
+        final_header_from_single = task._compute_date_keys(headers[0])
+
+    date_end = (
+        Time(start_time)
+        + (len(headers) - 1) * TimeDelta(time_delta, format="sec")
+        + TimeDelta(exp_time / 1000.0, format="sec")
+    ).isot
+
+    assert final_header["DATE-BEG"] == start_time
+    assert final_header["DATE-END"] == date_end
+
+    date_end_from_single = (
+        Time(headers[0]["DATE-BEG"]) + TimeDelta(exp_time / 1000.0, format="sec")
+    ).isot
+
+    assert final_header_from_single["DATE-BEG"] == headers[0]["DATE-BEG"]
+    assert final_header_from_single["DATE-END"] == date_end_from_single
+
+
+@pytest.mark.parametrize(
+    "shifts, expected",
+    # Shifts have shape (num_beams, num_modstates, 2)
+    # So the inner-most lists below (e.g., [5.0, 6.0]) correspond to [x_shift, y_shit]
+    [
+        (
+            np.array(
+                [  # mod1        mod2        mod3
+                    [[0.0, 0.0], [1.0, 2.0], [5.0, 6.0]],  # Beam 1
+                    [[1.0, 2.0], [11.0, 10.0], [3.0, 2.0]],  # Beam 2
+                ]
+            ),
+            [slice(11, None, None), slice(10, None, None)],
+        ),
+        (
+            np.array(
+                [
+                    [[0.0, 0.0], [-1.0, -2.0], [-5.0, -6.0]],  # Beam 1
+                    [[-1.0, -2.0], [-11.0, -10.0], [-3.0, -2.0]],  # Beam 2
+                ]
+            ),
+            [slice(0, -11, None), slice(0, -10, None)],
+        ),
+        (
+            np.array(
+                [
+                    [[0.0, 0.0], [10.0, 2.0], [5.0, 6.0]],  # Beam 1
+                    [[1.0, 2.0], [-11.0, 10.0], [-3.0, -2.0]],  # Beam 2
+                ]
+            ),
+            [slice(10, -11, None), slice(10, -2, None)],
+        ),
+    ],
+    ids=["All positive", "All negative", "Positive and negative"],
+)
+def test_beam_overlap_slice(calibration_collection_with_geo_shifts, expected):
+    """
+    Given: A CalibrationCollection object with populated state_offsets
+    When: Computing the overlapping beam slices
+    Then: The correct values are returned
+    """
+    calibrations = calibration_collection_with_geo_shifts
+    x_slice, y_slice = calibrations.beams_overlap_slice
+
+    assert x_slice == expected[0]
+    assert y_slice == expected[1]
+
+
+def test_combine_beams(
+    science_calibration_task,
+    calibrated_array_and_header_dicts,
+    calibration_collection_with_full_overlap_slice,
+):
     """
-    mocker.patch(
-        "dkist_processing_common.tasks.mixin.metadata_store.GraphQLClient", new=FakeGQLClient
+    Given: A ScienceCalibration task and set of calibrated array data
+    When: Combining the two beams
+    Then: The correct result is returned
+    """
+    task = science_calibration_task[0]
+    array_dict, header_dict = calibrated_array_and_header_dicts
+    result = task.combine_beams(
+        array_dict=array_dict,
+        header_dict=header_dict,
+        calibrations=calibration_collection_with_full_overlap_slice,
     )
-    task = parse_task_with_intensity_observes_and_polarmetric_cals
-    task()
-    assert task.constants._db_dict["NUM_MODSTATES"] == 1
-    assert task.constants._db_dict["POLARIMETER_MODE"] == "observe_intensity"
-    files = list(task.read(tags=[Tag.input(), Tag.frame()]))
-    for file in files:
-        assert "MODSTATE_1" in task.scratch.tags(file)
+    assert isinstance(result, VispL0FitsAccess)
+    data = result.data
+
+    x = np.arange(1, 5)
+    if task.constants.correct_for_polarization:
+        expected_I = np.ones((10, 10)) * 2.5
+        expected_Q = np.ones((10, 10)) * (x[1] / x[0] + x[-2] / x[-1]) / 2.0 * 2.5
+        expected_U = np.ones((10, 10)) * (x[2] / x[0] + x[-3] / x[-1]) / 2.0 * 2.5
+        expected_V = np.ones((10, 10)) * (x[3] / x[0] + x[-4] / x[-1]) / 2.0 * 2.5
+        expected = np.dstack([expected_I, expected_Q, expected_U, expected_V])
+
+    else:
+        expected = np.ones((10, 10, 4)) * 2.5
+
+    np.testing.assert_array_equal(data, expected)
```

### Comparing `dkist_processing_visp-2.8.2/dkist_processing_visp/tests/test_quality.py` & `dkist_processing_visp-2.9.0/dkist_processing_visp/tests/test_visp_base.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,103 +1,149 @@
-import json
-
+import numpy as np
 import pytest
 from astropy.io import fits
-from dkist_header_validator import spec122_validator
-from dkist_processing_common._util.scratch import WorkflowFileSystem
-from dkist_processing_common.models.tags import Tag
-from dkist_processing_common.tests.conftest import FakeGQLClient
+from dkist_processing_common.codecs.fits import fits_array_encoder
+from dkist_processing_common.codecs.fits import fits_hdu_decoder
 
 from dkist_processing_visp.models.tags import VispTag
-from dkist_processing_visp.tasks.quality_metrics import VispL1QualityMetrics
-from dkist_processing_visp.tests.conftest import generate_214_l1_fits_frame
-from dkist_processing_visp.tests.conftest import Visp122ObserveFrames
+from dkist_processing_visp.tasks.mixin.intermediate_frame_helpers import (
+    IntermediateFrameHelpersMixin,
+)
+from dkist_processing_visp.tasks.visp_base import VispTaskBase
 from dkist_processing_visp.tests.conftest import VispConstantsDb
+from dkist_processing_visp.tests.conftest import VispInputDatasetParameterValues
+
+NUM_BEAMS = 2
+NUM_MODSTATES = 8
+NUM_CS_STEPS = 6
+NUM_RASTER_STEPS = 10
+WAVE = 666.0
 
 
 @pytest.fixture(scope="function")
-def visp_quality_task(tmp_path, recipe_run_id, init_visp_constants_db):
-    num_map_scans = 3
-    num_raster_steps = 2
+def visp_science_task(recipe_run_id, assign_input_dataset_doc_to_task, init_visp_constants_db):
+    class Task(VispTaskBase, IntermediateFrameHelpersMixin):
+        def run(self):
+            ...
+
     constants_db = VispConstantsDb(
+        NUM_MODSTATES=NUM_MODSTATES,
+        NUM_CS_STEPS=NUM_CS_STEPS,
+        NUM_RASTER_STEPS=NUM_RASTER_STEPS,
+        WAVELENGTH=WAVE,
         POLARIMETER_MODE="observe_polarimetric",
-        NUM_MAP_SCANS=num_map_scans,
-        NUM_RASTER_STEPS=num_raster_steps,
     )
     init_visp_constants_db(recipe_run_id, constants_db)
-    with VispL1QualityMetrics(
-        recipe_run_id=recipe_run_id, workflow_name="science_calibration", workflow_version="VX.Y"
+    with Task(
+        recipe_run_id=recipe_run_id,
+        workflow_name="parse_visp_input_data",
+        workflow_version="VX.Y",
     ) as task:
-        task.scratch = WorkflowFileSystem(scratch_base_path=tmp_path)
-
-        # Create fake stokes frames
-        for map_scan in range(1, num_map_scans + 1):
-            for raster_step in range(0, num_raster_steps):
-                for stokes_param, index in zip(("I", "Q", "U", "V"), (1, 2, 3, 4)):
-                    ds = Visp122ObserveFrames(
-                        array_shape=(1, 10, 10),
-                        num_steps=num_raster_steps,
-                        num_map_scans=num_map_scans,
-                    )
-                    header_generator = (
-                        spec122_validator.validate_and_translate_to_214_l0(
-                            d.header(), return_type=fits.HDUList
-                        )[0].header
-                        for d in ds
-                    )
-
-                    hdul = generate_214_l1_fits_frame(s122_header=next(header_generator))
-                    hdul[1].header["DINDEX5"] = index
-                    task.fits_data_write(
-                        hdu_list=hdul,
-                        tags=[
-                            VispTag.output(),
-                            VispTag.frame(),
-                            VispTag.stokes(stokes_param),
-                            VispTag.raster_step(raster_step),
-                            VispTag.map_scan(map_scan),
-                        ],
-                    )
+        assign_input_dataset_doc_to_task(task, VispInputDatasetParameterValues())
 
         yield task
+
         task._purge()
 
 
-def test_quality_task(visp_quality_task, mocker):
+def test_write_intermediate_arrays(visp_science_task):
+    """
+    Given: A VispTaskBase task
+    When: Using the helper to write a single intermediate array
+    Then: The array is written and tagged correctly
+    """
+    data = np.random.random((10, 10))
+    head = fits.Header()
+    head["TEST"] = "foo"
+    visp_science_task.intermediate_frame_helpers_write_arrays(
+        arrays=data, headers=head, beam=1, map_scan=2, raster_step=3, task="BAR"
+    )
+    loaded_list = list(
+        visp_science_task.read(
+            tags=[
+                VispTag.intermediate(),
+                VispTag.frame(),
+                VispTag.beam(1),
+                VispTag.map_scan(2),
+                VispTag.raster_step(3),
+                VispTag.task("BAR"),
+            ],
+            decoder=fits_hdu_decoder,
+        )
+    )
+    assert len(loaded_list) == 1
+    hdu = loaded_list[0]
+    np.testing.assert_equal(hdu.data, data)
+    assert hdu.header["TEST"] == "foo"
+
+
+def test_write_intermediate_arrays_none_header(visp_science_task):
     """
-    Given: A VISPQualityMetrics task
-    When: Calling the task instance
-    Then: A single sensitivity measurement and datetime is recorded for each map scan for each Stokes Q, U, and V,
-            and a single noise measurement and datetime is recorded for L1 file for each Stokes Q, U, and V
+    Given: A VispTaskBase task
+    When: Using the helper to write a single intermediate array with no header
+    Then: The array is written and tagged correctly
     """
-    mocker.patch(
-        "dkist_processing_common.tasks.mixin.metadata_store.GraphQLClient", new=FakeGQLClient
+    data = np.random.random((10, 10))
+    visp_science_task.intermediate_frame_helpers_write_arrays(
+        arrays=data, headers=None, beam=1, map_scan=2, raster_step=3, task="BAR"
     )
-    # When
-    task = visp_quality_task
-    task()
-    # Then
-    num_map_scans = task.constants.num_map_scans
-    num_steps = task.constants.num_raster_steps
-    sensitivity_files = list(task.read(tags=[Tag.quality("SENSITIVITY")]))
-    assert len(sensitivity_files) == 4
-    for file in sensitivity_files:
-        with file.open() as f:
-            data = json.load(f)
-            assert isinstance(data, dict)
-            for time in range(len(data["x_values"])):
-                assert type(data["x_values"][time]) == str
-            for noise in range(len(data["y_values"])):
-                assert type(data["y_values"][noise]) == float
-            assert len(data["x_values"]) == len(data["y_values"]) == num_map_scans
-
-    noise_files = list(task.read(tags=[Tag.quality("NOISE")]))
-    assert len(noise_files) == 4
-    for file in noise_files:
-        with file.open() as f:
-            data = json.load(f)
-            assert isinstance(data, dict)
-            for time in range(len(data["x_values"])):
-                assert type(data["x_values"][time]) == str
-            for noise in range(len(data["y_values"])):
-                assert type(data["y_values"][noise]) == float
-            assert len(data["x_values"]) == len(data["y_values"]) == num_map_scans * num_steps
+    loaded_list = list(
+        visp_science_task.read(
+            tags=[
+                VispTag.intermediate(),
+                VispTag.frame(),
+                VispTag.beam(1),
+                VispTag.map_scan(2),
+                VispTag.raster_step(3),
+                VispTag.task("BAR"),
+            ],
+            decoder=fits_hdu_decoder,
+        )
+    )
+    assert len(loaded_list) == 1
+    hdu = loaded_list[0]
+    np.testing.assert_equal(hdu.data, data)
+
+
+def test_load_intermediate_arrays(visp_science_task):
+    """
+    Given: A Visp science task with intermediate frames
+    When: Loading intermediate arrays
+    Then: The correct arrays are returned
+    """
+    task = visp_science_task
+    tag_fcns = [[VispTag.beam], [VispTag.readout_exp_time, VispTag.task], [VispTag.modstate]]
+    tag_vals = [[1], [10.23, "dark"], [3]]
+    tag_list = [[f(v) for f, v in zip(fl, vl)] for fl, vl in zip(tag_fcns, tag_vals)]
+
+    for i, tags in enumerate(tag_list):
+        data = np.ones((2, 2)) * i
+        task.write(
+            data=data,
+            tags=tags + [VispTag.intermediate(), VispTag.frame()],
+            encoder=fits_array_encoder,
+        )
+
+    for i, tags in enumerate(tag_list):
+        arrays = list(task.intermediate_frame_helpers_load_intermediate_arrays(tags=tags))
+        assert len(arrays) == 1
+        np.testing.assert_equal(arrays[0], np.ones((2, 2)) * i)
+
+
+def test_load_intermediate_dark_array():
+    pass
+
+
+def test_load_intermediate_lamp_gain_array():
+    pass
+
+
+def test_load_intermediate_solar_gain_array():
+    pass
+
+
+def test_load_intermediate_geometric_hdu_list():
+    pass
+
+
+def test_load_intermediate_demodulated_arrays():
+    pass
```

### Comparing `dkist_processing_visp-2.8.2/dkist_processing_visp/tests/test_solar.py` & `dkist_processing_visp-2.9.0/dkist_processing_visp/tests/test_solar.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,192 +1,208 @@
 import json
-from collections import defaultdict
-from dataclasses import dataclass
+from functools import partial
+from typing import Callable
 
 import numpy as np
 import pytest
 from dkist_processing_common._util.scratch import WorkflowFileSystem
 from dkist_processing_common.models.tags import Tag
 from dkist_processing_common.tests.conftest import FakeGQLClient
 
 from dkist_processing_visp.models.tags import VispTag
 from dkist_processing_visp.tasks.solar import SolarCalibration
-from dkist_processing_visp.tests.conftest import generate_214_l0_fits_frame
+from dkist_processing_visp.tests.conftest import tag_on_modstate
 from dkist_processing_visp.tests.conftest import VispConstantsDb
-from dkist_processing_visp.tests.conftest import VispHeadersValidSolarGainFrames
-from dkist_processing_visp.tests.conftest import VispTestingParameters
+from dkist_processing_visp.tests.conftest import VispInputDatasetParameterValues
+from dkist_processing_visp.tests.conftest import write_frames_to_task
+from dkist_processing_visp.tests.conftest import write_intermediate_background_to_task
+from dkist_processing_visp.tests.conftest import write_intermediate_darks_to_task
+from dkist_processing_visp.tests.conftest import write_intermediate_geometric_to_task
+from dkist_processing_visp.tests.conftest import write_intermediate_lamp_to_task
+from dkist_processing_visp.tests.header_models import VispHeadersInputSolarGainFrames
+
+
+def lamp_signal_func(beam: int, modstate: int):
+    return 10 * beam * modstate
+
+
+def write_full_set_of_intermediate_lamp_cals_to_task(
+    task,
+    data_shape: tuple[int, int],
+    num_modstates: int,
+    lamp_signal_func: Callable[[int, int], float] = lamp_signal_func,
+):
+    for beam in [1, 2]:
+        for modstate in range(1, num_modstates + 1):
+            lamp_signal = lamp_signal_func(beam, modstate)
+            write_intermediate_lamp_to_task(
+                task=task,
+                lamp_signal=lamp_signal,
+                beam=beam,
+                modstate=modstate,
+                data_shape=data_shape,
+            )
 
 
-@dataclass
-class VispSolarTestingParameters(VispTestingParameters):
-    visp_beam_border: int = 10
+def make_solar_input_array_data(
+    frame: VispHeadersInputSolarGainFrames,
+    dark_signal: float,
+    lamp_signal_func: Callable[[int, int], float] = lamp_signal_func,
+):
+    data_shape = frame.array_shape[1:]
+    beam_shape = (data_shape[0] // 2, data_shape[1])
+    modstate = frame.current_modstate("")  # Weird signature due to key_function
+    num_raw_per_fpa = frame.header()["CAM__014"]
+
+    beam_list = []
+    for beam in [1, 2]:
+        true_gain = np.ones(beam_shape) + modstate + beam
+        true_solar_signal = np.arange(1, beam_shape[0] + 1) / 5
+        true_solar_gain = true_gain * true_solar_signal[:, None]
+        lamp_signal = lamp_signal_func(beam, modstate)
+        raw_beam = (true_solar_gain * lamp_signal) + dark_signal
+        beam_list.append(raw_beam)
+
+    raw_solar = np.concatenate(beam_list) * num_raw_per_fpa
+    return raw_solar
+
+
+def write_input_solar_gains_to_task(
+    task,
+    data_shape: tuple[int, int],
+    dark_signal: float,
+    readout_exp_time: float,
+    num_modstates: int,
+    lamp_signal_func: Callable[[int, int], float] = lamp_signal_func,
+):
+    array_shape = (1, *data_shape)
+    dataset = VispHeadersInputSolarGainFrames(
+        array_shape=array_shape,
+        time_delta=10,
+        num_modstates=num_modstates,
+    )
+    data_func = partial(
+        make_solar_input_array_data, dark_signal=dark_signal, lamp_signal_func=lamp_signal_func
+    )
+    write_frames_to_task(
+        task=task,
+        frame_generator=dataset,
+        extra_tags=[
+            VispTag.input(),
+            VispTag.task_solar_gain(),
+            VispTag.readout_exp_time(readout_exp_time),
+        ],
+        tag_func=tag_on_modstate,
+        data_func=data_func,
+    )
 
 
 @pytest.fixture(scope="function")
-def solar_gain_calibration_task_that_completes(
+def solar_gain_task(
     tmp_path,
     recipe_run_id,
-    assign_input_dataset_doc_to_task,
     init_visp_constants_db,
-    background_on,
 ):
     number_of_modstates = 3
-    number_of_beams = 2
-    readout_exp_time = 40.0  # From VispHeadersValidSolarGainFrames fixture
-    intermediate_shape = (10, 10)
-    dataset_shape = (1, 20, 10)
-    array_shape = (1, 20, 10)
+    readout_exp_time = 40.0
     constants_db = VispConstantsDb(
         NUM_MODSTATES=number_of_modstates, SOLAR_READOUT_EXP_TIMES=(readout_exp_time,)
     )
     init_visp_constants_db(recipe_run_id, constants_db)
     with SolarCalibration(
         recipe_run_id=recipe_run_id, workflow_name="geometric_calibration", workflow_version="VX.Y"
     ) as task:
         try:  # This try... block is here to make sure the dbs get cleaned up if there's a failure in the fixture
             task.scratch = WorkflowFileSystem(
                 scratch_base_path=tmp_path, recipe_run_id=recipe_run_id
             )
-            assign_input_dataset_doc_to_task(
-                task, VispSolarTestingParameters(visp_background_on=background_on)
-            )
-
-            # We use a dictionary to carry the raw frames because we need to compute different cal objects for
-            # every (beam, modstate) tuple, but we write the raw solar arrays as a single, combined array.
-            # I'm so sorry; this is kind of a hack because I didn't want to refactor this whole nested loop.
-            raw_solar_dict = defaultdict(dict)
-            for beam in range(1, number_of_beams + 1):
-
-                # DarkCal object
-                dark_cal = np.ones(intermediate_shape) * 3.0
-                task.intermediate_frame_helpers_write_arrays(
-                    arrays=dark_cal, beam=beam, task="DARK", readout_exp_time=readout_exp_time
-                )
-
-                if background_on:
-                    # BackgroundLight object
-                    bg_cal = np.zeros(intermediate_shape)
-                    task.intermediate_frame_helpers_write_arrays(
-                        arrays=bg_cal, beam=beam, task="BACKGROUND"
-                    )
-
-                # Geo angles and spec_shifts
-                task.intermediate_frame_helpers_write_arrays(
-                    arrays=np.zeros(1), beam=beam, task="GEOMETRIC_ANGLE"
-                )
-                task.intermediate_frame_helpers_write_arrays(
-                    arrays=np.zeros(intermediate_shape[0]), beam=beam, task="GEOMETRIC_SPEC_SHIFTS"
-                )
-
-                for modstate in range(1, number_of_modstates + 1):
-                    # LampCal object
-                    lamp_cal = np.ones(intermediate_shape) * 10 * modstate * beam
-                    task.intermediate_frame_helpers_write_arrays(
-                        arrays=lamp_cal, beam=beam, modstate=modstate, task="LAMP_GAIN"
-                    )
-
-                    # Geo offsets
-                    task.intermediate_frame_helpers_write_arrays(
-                        arrays=np.zeros(2), beam=beam, modstate=modstate, task="GEOMETRIC_OFFSET"
-                    )
-
-                    true_gain = np.ones(intermediate_shape) + modstate + beam
-                    true_solar_signal = np.arange(1, intermediate_shape[0] + 1) / 5
-                    true_solar_gain = true_gain * true_solar_signal[:, None]
-                    raw_solar = (true_solar_gain * lamp_cal) + dark_cal
-                    raw_solar_dict[beam][modstate] = raw_solar
-
-            for modstate in range(1, number_of_modstates + 1):
-                ds = VispHeadersValidSolarGainFrames(
-                    dataset_shape=dataset_shape,
-                    array_shape=array_shape,
-                    time_delta=10,
-                    num_modstates=number_of_modstates,
-                    modstate=modstate,
-                )
-                header = ds.header()
-                num_raw_per_fpa = header["CAM__014"]
-                raw_solar_array = (
-                    np.concatenate((raw_solar_dict[1][modstate], raw_solar_dict[2][modstate]))
-                    * num_raw_per_fpa
-                )
-                solar_hdul = generate_214_l0_fits_frame(data=raw_solar_array, s122_header=header)
-                task.fits_data_write(
-                    hdu_list=solar_hdul,
-                    tags=[
-                        VispTag.input(),
-                        VispTag.task("SOLAR_GAIN"),
-                        VispTag.modstate(modstate),
-                        VispTag.frame(),
-                        VispTag.readout_exp_time(readout_exp_time),
-                    ],
-                )
 
-            yield task
+            yield task, readout_exp_time, number_of_modstates
         except:
             raise
         finally:
             task._purge()
 
 
-@pytest.fixture(scope="function")
-def solar_gain_calibration_task_with_no_data(tmp_path, recipe_run_id, init_visp_constants_db):
-    number_of_modstates = 3
-    constants_db = VispConstantsDb(NUM_MODSTATES=number_of_modstates)
-    init_visp_constants_db(recipe_run_id, constants_db)
-    with SolarCalibration(
-        recipe_run_id=recipe_run_id, workflow_name="geometric_calibration", workflow_version="VX.Y"
-    ) as task:
-        task.scratch = WorkflowFileSystem(scratch_base_path=tmp_path, recipe_run_id=recipe_run_id)
-
-        yield task
-        task._purge()
-
-
 @pytest.mark.parametrize(
     "background_on",
     [pytest.param(True, id="Background on"), pytest.param(False, id="Background off")],
 )
-def test_solar_gain_task(solar_gain_calibration_task_that_completes, mocker):
+def test_solar_gain_task(solar_gain_task, background_on, assign_input_dataset_doc_to_task, mocker):
     """
     Given: A set of raw solar gain images and necessary intermediate calibrations
     When: Running the solargain task
     Then: The task completes and the outputs are correct
     """
     mocker.patch(
         "dkist_processing_common.tasks.mixin.metadata_store.GraphQLClient", new=FakeGQLClient
     )
 
-    # It's way too hard to make data for a unit test that get through the line zones calculation.
+    # It's way too hard to make data for a unit test that will get through the line zones calculation.
     # Leave that for grogu.
     mocker.patch(
         "dkist_processing_visp.tasks.solar.SolarCalibration.compute_line_zones",
         return_value=[(4, 7)],
     )
-    task = solar_gain_calibration_task_that_completes
+
+    task, readout_exp_time, num_modstates = solar_gain_task
+    dark_signal = 3.0
+    input_shape = (20, 10)
+    intermediate_shape = (10, 10)
+    beam_border = input_shape[0] // 2
+    assign_input_dataset_doc_to_task(
+        task,
+        VispInputDatasetParameterValues(
+            visp_background_on=background_on, visp_beam_border=beam_border
+        ),
+    )
+    write_intermediate_darks_to_task(
+        task=task,
+        dark_signal=dark_signal,
+        readout_exp_time=readout_exp_time,
+        data_shape=intermediate_shape,
+    )
+    if background_on:
+        write_intermediate_background_to_task(
+            task=task, background_signal=0.0, data_shape=intermediate_shape
+        )
+    write_full_set_of_intermediate_lamp_cals_to_task(
+        task=task, data_shape=intermediate_shape, num_modstates=num_modstates
+    )
+    write_intermediate_geometric_to_task(
+        task=task, num_modstates=num_modstates, data_shape=intermediate_shape
+    )
+    write_input_solar_gains_to_task(
+        task=task,
+        data_shape=input_shape,
+        dark_signal=dark_signal,
+        readout_exp_time=readout_exp_time,
+        num_modstates=num_modstates,
+    )
+
     task()
     for beam in range(1, task.constants.num_beams + 1):
         equalization_flux = np.nanmedian(
             [
-                np.ones((10, 10))
+                np.ones(intermediate_shape)
                 * (1 + beam + m)
                 * (10 * beam * m)
                 * np.nanpercentile(
                     np.arange(1, 11) / 5,
                     task.parameters.solar_characteristic_spatial_normalization_percentile,
                 )
                 for m in range(1, task.constants.num_modstates + 1)
             ],
             axis=0,
         )
 
         for modstate in range(1, task.constants.num_modstates + 1):
             # Gains aren't normalized so their expected value is weird. This expression comes from the math applied above. Sorry.
             raw = (
-                np.ones((10, 10))
+                np.ones(intermediate_shape)
                 * (1 + beam + modstate)
                 * (10 * beam * modstate)
                 * np.mean(np.arange(1, 11) / 5)
             )
             expected = raw * equalization_flux / np.nanmedian(raw)
             solar_gain = task.intermediate_frame_helpers_load_solar_gain_array(
                 beam=beam, modstate=modstate
@@ -195,19 +211,19 @@
 
     quality_files = task.read(tags=[Tag.quality("TASK_TYPES")])
     for file in quality_files:
         with file.open() as f:
             data = json.load(f)
             assert isinstance(data, dict)
             assert data["total_frames"] == task.scratch.count_all(
-                tags=[VispTag.input(), VispTag.frame(), VispTag.task("SOLAR_GAIN")]
+                tags=[VispTag.input(), VispTag.frame(), VispTag.task_solar_gain()]
             )
 
 
-def test_line_zones(solar_gain_calibration_task_with_no_data):
+def test_line_zones(solar_gain_task):
     """
     Given: A spectrum with some absorption lines
     When: Computing zones around the lines
     Then: Correct results are returned
     """
     # This is here because we mocked it out in the solar gain task test above
     # NOTE that it does not test for removal of overlapping regions
@@ -218,24 +234,26 @@
     x = np.arange(1000.0)
     expected = []
     for m, s in zip([100.0, 300.0, 700], [10.0, 20.0, 5.0]):
         spec -= gaussian(x, 40, m, s)
         hwhm = s * 2.355 / 2
         expected.append((np.floor(m - hwhm).astype(int), np.ceil(m + hwhm).astype(int)))
 
-    zones = solar_gain_calibration_task_with_no_data.compute_line_zones(
-        spec[:, None], bg_order=0, rel_height=0.5
-    )
+    task = solar_gain_task[0]
+
+    zones = task.compute_line_zones(spec[:, None], bg_order=0, rel_height=0.5)
     assert zones == expected
 
 
-def test_identify_overlapping_zones(solar_gain_calibration_task_with_no_data):
+def test_identify_overlapping_zones(solar_gain_task):
     """
     Given: A list of zone borders that contain overlapping zones
     When: Identifying zones that overlap
     Then: The smaller of the overlapping zones are identified for removal
     """
     rips = np.array([100, 110, 220, 200])
     lips = np.array([150, 120, 230, 250])
 
-    idx_to_remove = solar_gain_calibration_task_with_no_data.identify_overlapping_zones(rips, lips)
+    task = solar_gain_task[0]
+
+    idx_to_remove = task.identify_overlapping_zones(rips, lips)
     assert idx_to_remove == [1, 2]
```

### Comparing `dkist_processing_visp-2.8.2/dkist_processing_visp/tests/test_submit_quality.py` & `dkist_processing_visp-2.9.0/dkist_processing_visp/tests/test_submit_quality.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.8.2/dkist_processing_visp/tests/test_trial_output_data.py` & `dkist_processing_visp-2.9.0/dkist_processing_visp/tests/test_trial_output_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import json
 
 import pytest
 from dkist_processing_common._util.scratch import WorkflowFileSystem
 from dkist_processing_common.codecs.str import str_encoder
 from dkist_processing_common.models.graphql import RecipeRunResponse
+from dkist_processing_common.models.task_name import TaskName
 
 from dkist_processing_visp.models.tags import VispTag
+from dkist_processing_visp.models.task_name import VispTaskName
 from dkist_processing_visp.tasks.trial_output_data import TransferVispTrialData
 
 
 @pytest.fixture
 def recipe_run_configuration(debug_switch, intermediate_switch, output_switch, tag_lists):
     class GQLClientWithConfiguration:
         def __init__(self, *args, **kwargs):
@@ -37,21 +39,21 @@
         def execute_gql_mutation(**kwargs):
             ...
 
     return GQLClientWithConfiguration
 
 
 intermediate_task_names = [
-    "DARK",
-    "BACKGROUND",
-    "GEOMETRIC_ANGLE",
-    "GEOMETRIC_OFFSET",
-    "GEOMETRIC_SPEC_SHIFTS",
-    "SOLAR_GAIN",
-    "DEMOD_MATRICES",
+    TaskName.dark.value,
+    VispTaskName.background.value,
+    TaskName.geometric_angle.value,
+    TaskName.geometric_offsets.value,
+    TaskName.geometric_spectral_shifts.value,
+    TaskName.solar_gain.value,
+    TaskName.demodulation_matrices.value,
 ]
 
 tag_lists = [[VispTag.movie()], ["FOO", "BAR"]]
 
 
 def write_debug_frames_to_task(task: TransferVispTrialData) -> int:
     num_debug = 3
@@ -68,15 +70,15 @@
             encoder=str_encoder,
             tags=[VispTag.frame(), VispTag.intermediate(), VispTag.task(task_name)],
         )
 
     return len(intermediate_task_names)
 
 
-def write_output_frames_to_task(task: TransferVispTrialData) -> int:
+def write_dummy_output_frames_to_task(task: TransferVispTrialData) -> int:
     num_output = 2
     for i in range(num_output):
         task.write(
             data=f"output_{i}", encoder=str_encoder, tags=[VispTag.frame(), VispTag.output()]
         )
 
     return num_output
@@ -110,15 +112,15 @@
             recipe_run_id=recipe_run_id,
             scratch_base_path=tmp_path,
         )
         task.constants._update({"PROPOSAL_ID": proposal_id})
         try:
             num_debug = write_debug_frames_to_task(task)
             num_intermediate = write_intermediate_frames_to_task(task)
-            num_output = write_output_frames_to_task(task)
+            num_output = write_dummy_output_frames_to_task(task)
             num_specific = write_specific_tags_to_task(task)
             write_unused_frame_to_task(task)
             yield task, num_debug, num_intermediate, num_output, num_specific
 
         finally:
             task._purge()
```

### Comparing `dkist_processing_visp-2.8.2/dkist_processing_visp/tests/test_visp_base.py` & `dkist_processing_visp-2.9.0/dkist_processing_visp/tests/test_lamp.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,161 +1,163 @@
+import json
+from functools import partial
+
 import numpy as np
 import pytest
 from astropy.io import fits
 from dkist_processing_common._util.scratch import WorkflowFileSystem
+from dkist_processing_common.models.tags import Tag
+from dkist_processing_common.tests.conftest import FakeGQLClient
 
 from dkist_processing_visp.models.tags import VispTag
-from dkist_processing_visp.tasks.mixin.intermediate_frame_helpers import (
-    IntermediateFrameHelpersMixin,
-)
-from dkist_processing_visp.tasks.visp_base import VispTaskBase
+from dkist_processing_visp.tasks.lamp import LampCalibration
+from dkist_processing_visp.tests.conftest import tag_on_modstate
 from dkist_processing_visp.tests.conftest import VispConstantsDb
-from dkist_processing_visp.tests.conftest import VispTestingParameters
-
-NUM_BEAMS = 2
-NUM_MODSTATES = 8
-NUM_CS_STEPS = 6
-NUM_RASTER_STEPS = 10
-WAVE = 666.0
-
-
-@pytest.fixture(scope="function")
-def visp_science_task(recipe_run_id, assign_input_dataset_doc_to_task, init_visp_constants_db):
-    class Task(VispTaskBase, IntermediateFrameHelpersMixin):
-        def run(self):
-            ...
-
-    constants_db = VispConstantsDb(
-        NUM_MODSTATES=NUM_MODSTATES,
-        NUM_CS_STEPS=NUM_CS_STEPS,
-        NUM_RASTER_STEPS=NUM_RASTER_STEPS,
-        WAVELENGTH=WAVE,
-        POLARIMETER_MODE="observe_polarimetric",
-    )
-    init_visp_constants_db(recipe_run_id, constants_db)
-    task = Task(
-        recipe_run_id=recipe_run_id,
-        workflow_name="parse_visp_input_data",
-        workflow_version="VX.Y",
-    )
-    assign_input_dataset_doc_to_task(task, VispTestingParameters())
+from dkist_processing_visp.tests.conftest import VispInputDatasetParameterValues
+from dkist_processing_visp.tests.conftest import write_frames_to_task
+from dkist_processing_visp.tests.conftest import write_intermediate_darks_to_task
+from dkist_processing_visp.tests.header_models import VispHeadersInputLampGainFrames
 
-    yield task
+RNG = np.random.default_rng()
 
-    task._purge()
 
+def make_lamp_array_data(
+    frame: VispHeadersInputLampGainFrames, dark_signal: float, beam_border: int
+):
+    num_raw_frames_per_fpa = frame.header()["CAM__014"]
+    data = np.zeros(frame.array_shape)
+    data[0, :beam_border, :] = (1.1 + dark_signal) * num_raw_frames_per_fpa
+    data[0, beam_border:, :] = (1.2 + dark_signal) * num_raw_frames_per_fpa
+
+    return data
 
-def test_write_intermediate_arrays(visp_science_task):
-    """
-    Given: A VispTaskBase task
-    When: Using the helper to write a single intermediate array
-    Then: The array is written and tagged correctly
-    """
-    data = np.random.random((10, 10))
-    head = fits.Header()
-    head["TEST"] = "foo"
-    visp_science_task.intermediate_frame_helpers_write_arrays(
-        arrays=data, headers=head, beam=1, map_scan=2, raster_step=3, task="BAR"
-    )
-    loaded_list = list(
-        visp_science_task.fits_data_read_hdu(
-            tags=[
-                VispTag.intermediate(),
-                VispTag.frame(),
-                VispTag.beam(1),
-                VispTag.map_scan(2),
-                VispTag.raster_step(3),
-                VispTag.task("BAR"),
-            ]
-        )
-    )
-    assert len(loaded_list) == 1
-    hdu = loaded_list[0]
-    np.testing.assert_equal(hdu.data, data)
-    assert hdu.header["TEST"] == "foo"
 
+def write_lamp_inputs_to_task(
+    task,
+    dark_signal: float,
+    readout_exp_time: float,
+    num_modstates: int,
+    data_shape: tuple[int, int],
+):
+    beam_border = task.parameters.beam_border
+    array_shape = (1, *data_shape)
 
-def test_write_intermediate_arrays_none_header(visp_science_task):
-    """
-    Given: A VispTaskBase task
-    When: Using the helper to write a single intermediate array with no header
-    Then: The array is written and tagged correctly
-    """
-    data = np.random.random((10, 10))
-    visp_science_task.intermediate_frame_helpers_write_arrays(
-        arrays=data, headers=None, beam=1, map_scan=2, raster_step=3, task="BAR"
-    )
-    loaded_list = list(
-        visp_science_task.fits_data_read_hdu(
-            tags=[
-                VispTag.intermediate(),
-                VispTag.frame(),
-                VispTag.beam(1),
-                VispTag.map_scan(2),
-                VispTag.raster_step(3),
-                VispTag.task("BAR"),
-            ]
-        )
+    # These images are for two combined beams
+    dataset = VispHeadersInputLampGainFrames(
+        array_shape=array_shape,
+        time_delta=10,
+        num_modstates=num_modstates,
+    )
+
+    data_func = partial(make_lamp_array_data, dark_signal=dark_signal, beam_border=beam_border)
+    write_frames_to_task(
+        task=task,
+        frame_generator=dataset,
+        extra_tags=[
+            VispTag.input(),
+            VispTag.task_lamp_gain(),
+            VispTag.readout_exp_time(readout_exp_time),
+        ],
+        tag_func=tag_on_modstate,
+        data_func=data_func,
     )
-    assert len(loaded_list) == 1
-    hdu = loaded_list[0]
-    np.testing.assert_equal(hdu.data, data)
 
 
-@pytest.fixture
-def visp_science_task_with_tagged_intermediates(
-    recipe_run_id, tmpdir_factory, init_visp_constants_db
+@pytest.fixture(scope="function")
+def lamp_calibration_task(
+    tmp_path,
+    recipe_run_id,
+    init_visp_constants_db,
 ):
-    class Task(VispTaskBase, IntermediateFrameHelpersMixin):
-        def run(self):
-            ...
-
-    init_visp_constants_db(recipe_run_id, VispConstantsDb())
-    task = Task(
-        recipe_run_id=recipe_run_id,
-        workflow_name="parse_visp_input_data",
-        workflow_version="VX.Y",
+    num_modstates = 2
+    readout_exp_time = 20.0
+    constants_db = VispConstantsDb(
+        NUM_MODSTATES=num_modstates, LAMP_READOUT_EXP_TIMES=(readout_exp_time,)
     )
-    task._scratch = WorkflowFileSystem(scratch_base_path=tmpdir_factory.mktemp("data"))
-    tag_names = [["beam"], ["readout_exp_time", "task"], ["modstate"]]
-    tag_vals = [[1], [10.23, "dark"], [3]]
-    tag_fcns = [[getattr(VispTag, n) for n in nl] for nl in tag_names]
-    tag_list = [[f(v) for f, v in zip(fl, vl)] for fl, vl in zip(tag_fcns, tag_vals)]
-    for i, tags in enumerate(tag_list):
-        hdul = fits.HDUList([fits.PrimaryHDU(data=np.ones((2, 2)) * i)])
-        fname = task.scratch.workflow_base_path / f"file{i}.fits"
-        hdul.writeto(fname)
-        task.tag(fname, tags + [VispTag.intermediate(), VispTag.frame()])
-
-    yield task, tag_names, tag_vals
-
-    task._purge()
-
-
-def test_load_intermediate_arrays(visp_science_task_with_tagged_intermediates):
-
-    task, tag_names, tag_vals = visp_science_task_with_tagged_intermediates
-    kwarg_list = [{k: v for k, v in zip(kl, vl)} for kl, vl in zip(tag_names, tag_vals)]
-    for i, kwargs in enumerate(kwarg_list):
-        arrays = list(task.intermediate_frame_helpers_load_intermediate_arrays(**kwargs))
-        assert len(arrays) == 1
-        np.testing.assert_equal(arrays[0], np.ones((2, 2)) * i)
-
-
-def test_load_intermediate_dark_array():
-    pass
-
-
-def test_load_intermediate_lamp_gain_array():
-    pass
-
+    init_visp_constants_db(recipe_run_id, constants_db)
+    with LampCalibration(
+        recipe_run_id=recipe_run_id, workflow_name="lamp_gain_calibration", workflow_version="VX.Y"
+    ) as task:
+        try:  # This try... block is here to make sure the dbs get cleaned up if there's a failure in the fixture
+            task.scratch = WorkflowFileSystem(
+                scratch_base_path=tmp_path, recipe_run_id=recipe_run_id
+            )
 
-def test_load_intermediate_solar_gain_array():
-    pass
+            yield task, num_modstates, readout_exp_time
 
+        except:
+            raise
 
-def test_load_intermediate_geometric_hdu_list():
-    pass
+        finally:
+            task._purge()
 
 
-def test_load_intermediate_demodulated_arrays():
-    pass
+def test_lamp_calibration_task(lamp_calibration_task, assign_input_dataset_doc_to_task, mocker):
+    """
+    Given: A LampCalibration task
+    When: Calling the task instance
+    Then: The correct number of output lamp gain frames exists, and are tagged correctly
+    """
+    mocker.patch(
+        "dkist_processing_common.tasks.mixin.metadata_store.GraphQLClient", new=FakeGQLClient
+    )
+    # Given
+    task, num_modstates, readout_exp_time = lamp_calibration_task
+    input_shape = (20, 10)
+    intermediate_shape = (10, 10)
+    dark_signal = 3.0
+    beam_border = input_shape[0] // 2
+    assign_input_dataset_doc_to_task(
+        task, VispInputDatasetParameterValues(visp_beam_border=beam_border)
+    )
+    write_intermediate_darks_to_task(
+        task=task,
+        dark_signal=dark_signal,
+        readout_exp_time=readout_exp_time,
+        data_shape=intermediate_shape,
+    )
+    write_lamp_inputs_to_task(
+        task=task,
+        dark_signal=dark_signal,
+        readout_exp_time=readout_exp_time,
+        num_modstates=num_modstates,
+        data_shape=input_shape,
+    )
+
+    # When
+    task()
+
+    # Then
+    tags = [
+        VispTag.task_lamp_gain(),
+        VispTag.intermediate(),
+    ]
+    assert len(list(task.read(tags=tags))) == num_modstates * 2  # 2 from beams
+
+    for i in range(num_modstates):
+        for beam in [1, 2]:
+            tags = [
+                VispTag.task_lamp_gain(),
+                VispTag.intermediate(),
+                VispTag.modstate(i + 1),
+                VispTag.beam(beam),
+            ]
+            files = list(task.read(tags=tags))
+            assert len(files) == 1
+            hdu = fits.open(files[0])[0]
+            np.testing.assert_allclose(hdu.data, np.ones((10, 10)) * (1 + (0.1 * beam)))
+
+    tags = [
+        VispTag.task_lamp_gain(),
+        VispTag.intermediate(),
+    ]
+    for filepath in task.read(tags=tags):
+        assert filepath.exists()
+
+    quality_files = task.read(tags=[Tag.quality("TASK_TYPES")])
+    for file in quality_files:
+        with file.open() as f:
+            data = json.load(f)
+            assert isinstance(data, dict)
+            assert data["total_frames"] == task.scratch.count_all(
+                tags=[VispTag.input(), VispTag.frame(), VispTag.task_lamp_gain()]
+            )
```

### Comparing `dkist_processing_visp-2.8.2/dkist_processing_visp/tests/test_visp_constants.py` & `dkist_processing_visp-2.9.0/dkist_processing_visp/tests/test_visp_constants.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.8.2/dkist_processing_visp/tests/test_write_l1.py` & `dkist_processing_visp-2.9.0/dkist_processing_visp/tests/test_write_l1.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import numpy as np
 import pytest
 from astropy.io import fits
 from astropy.time import Time
 from dkist_fits_specifications import __version__ as spec_version
 from dkist_header_validator import spec214_validator
+from dkist_processing_common.codecs.fits import fits_hdulist_encoder
 from dkist_processing_common.models.tags import Tag
 from dkist_processing_common.tests.conftest import FakeGQLClient
 
 from dkist_processing_visp.tasks.write_l1 import VispWriteL1Frame
 from dkist_processing_visp.tests.conftest import VispConstantsDb
 
 
@@ -16,71 +17,77 @@
     params=[("HPLT-TAN", "AWAV"), ("AWAV", "HPLT-TAN")],
     ids=["correct wcs axis order", "incorrect wcs axis order"],
 )
 def wcs_axis_names(request):
     return request.param
 
 
-@pytest.fixture(scope="function", params=[1, 4], ids=["stokes I only", "stokes IQUV"])
+@pytest.fixture
 def write_l1_task(
-    recipe_run_id, calibrated_visp_dataset, init_visp_constants_db, request, wcs_axis_names
+    recipe_run_id,
+    init_visp_constants_db,
+    pol_type,
 ):
-    num_of_stokes_params = request.param
+    polarimeter_mode = "observe_polarimetric"
+    if pol_type == "Stokes-I":
+        polarimeter_mode = "observe_intensity"
     constants_db = VispConstantsDb(
         INSTRUMENT="VISP",
         AVERAGE_CADENCE=10,
         MINIMUM_CADENCE=10,
         MAXIMUM_CADENCE=10,
         VARIANCE_CADENCE=0,
         NUM_MAP_SCANS=1,
         NUM_RASTER_STEPS=2,
         SPECTRAL_LINE="VISP Ca II H",
-        POLARIMETER_MODE="observe_polarimetric"
-        if num_of_stokes_params == 4
-        else "observe_intensity",
+        POLARIMETER_MODE=polarimeter_mode,
     )
     init_visp_constants_db(recipe_run_id, constants_db)
     with VispWriteL1Frame(
         recipe_run_id=recipe_run_id,
         workflow_name="workflow_name",
         workflow_version="workflow_version",
     ) as task:
-        try:  # This try... block is here to make sure the dbs get cleaned up if there's a failure in the fixture
-            stokes_params = ["I", "Q", "U", "V"]
-            used_stokes_params = []
-            # Random data needed so skew and kurtosis don't barf
-            hdu = fits.PrimaryHDU(
-                data=np.random.random((128, 128, 1)) * 100.0, header=calibrated_visp_dataset
-            )
-            hdul = fits.HDUList([hdu])
-            hdul[0].header["CTYPE1"] = wcs_axis_names[0]
-            hdul[0].header["CTYPE2"] = wcs_axis_names[1]
-            for i in range(num_of_stokes_params):
-                task.fits_data_write(
-                    hdu_list=hdul,
-                    tags=[Tag.calibrated(), Tag.frame(), Tag.stokes(stokes_params[i])],
-                )
-                used_stokes_params.append(stokes_params[i])
-            yield task, used_stokes_params
-        except:
-            raise
-        finally:
-            task._purge()
 
+        yield task
 
-def test_write_l1_frame(write_l1_task, mocker, wcs_axis_names):
+        task._purge()
+
+
+@pytest.mark.parametrize("pol_type", ["Full Stokes", "Stokes-I"])
+def test_write_l1_frame(write_l1_task, calibrated_visp_header, wcs_axis_names, pol_type, mocker):
     """
     :Given: a write L1 task
     :When: running the task
     :Then: no errors are raised
     """
     mocker.patch(
         "dkist_processing_common.tasks.mixin.metadata_store.GraphQLClient", new=FakeGQLClient
     )
-    task, stokes_params = write_l1_task
+    task = write_l1_task
+
+    stokes_params = ["I", "Q", "U", "V"]
+    if pol_type == "Stokes-I":
+        stokes_params = ["I"]
+    num_stokes = len(stokes_params)
+
+    # Random data needed so skew and kurtosis don't barf
+    hdu = fits.PrimaryHDU(
+        data=np.random.random((128, 128, 1)) * 100.0, header=calibrated_visp_header
+    )
+    hdul = fits.HDUList([hdu])
+    hdul[0].header["CTYPE1"] = wcs_axis_names[0]
+    hdul[0].header["CTYPE2"] = wcs_axis_names[1]
+    for i in range(num_stokes):
+        task.write(
+            data=hdul,
+            tags=[Tag.calibrated(), Tag.frame(), Tag.stokes(stokes_params[i])],
+            encoder=fits_hdulist_encoder,
+        )
+
     task()
     for stokes_param in stokes_params:
         files = list(task.read(tags=[Tag.frame(), Tag.output(), Tag.stokes(stokes_param)]))
         assert len(files) == 1
         for file in files:
             assert file.exists
             assert spec214_validator.validate(file, extra=False)
```

### Comparing `dkist_processing_visp-2.8.2/dkist_processing_visp/workflows/l0_processing.py` & `dkist_processing_visp-2.9.0/dkist_processing_visp/workflows/l0_processing.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.8.2/dkist_processing_visp/workflows/trial_workflows.py` & `dkist_processing_visp-2.9.0/dkist_processing_visp/workflows/trial_workflows.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.8.2/dkist_processing_visp.egg-info/PKG-INFO` & `dkist_processing_visp-2.9.0/dkist_processing_visp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-visp
-Version: 2.8.2
+Version: 2.9.0
 Summary: Science processing code for the ViSP instrument on DKIST
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-visp/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/visp
 Classifier: Programming Language :: Python
```

### Comparing `dkist_processing_visp-2.8.2/dkist_processing_visp.egg-info/SOURCES.txt` & `dkist_processing_visp-2.9.0/dkist_processing_visp.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -19,24 +19,23 @@
 dkist_processing_visp.egg-info/requires.txt
 dkist_processing_visp.egg-info/top_level.txt
 dkist_processing_visp/fonts/Lato-Regular.ttf
 dkist_processing_visp/models/__init__.py
 dkist_processing_visp/models/constants.py
 dkist_processing_visp/models/parameters.py
 dkist_processing_visp/models/tags.py
+dkist_processing_visp/models/task_name.py
 dkist_processing_visp/parsers/__init__.py
 dkist_processing_visp/parsers/map_repeats.py
 dkist_processing_visp/parsers/modulator_states.py
 dkist_processing_visp/parsers/polarimeter_mode.py
 dkist_processing_visp/parsers/raster_step.py
-dkist_processing_visp/parsers/task.py
 dkist_processing_visp/parsers/time.py
 dkist_processing_visp/parsers/visp_l0_fits_access.py
 dkist_processing_visp/parsers/visp_l1_fits_access.py
-dkist_processing_visp/parsers/wavelength.py
 dkist_processing_visp/tasks/__init__.py
 dkist_processing_visp/tasks/assemble_movie.py
 dkist_processing_visp/tasks/background_light.py
 dkist_processing_visp/tasks/dark.py
 dkist_processing_visp/tasks/geometric.py
 dkist_processing_visp/tasks/instrument_polarization.py
 dkist_processing_visp/tasks/l1_output_data.py
@@ -46,21 +45,23 @@
 dkist_processing_visp/tasks/quality_metrics.py
 dkist_processing_visp/tasks/science.py
 dkist_processing_visp/tasks/solar.py
 dkist_processing_visp/tasks/trial_output_data.py
 dkist_processing_visp/tasks/visp_base.py
 dkist_processing_visp/tasks/write_l1.py
 dkist_processing_visp/tasks/mixin/__init__.py
+dkist_processing_visp/tasks/mixin/beam_access.py
 dkist_processing_visp/tasks/mixin/corrections.py
 dkist_processing_visp/tasks/mixin/downsample.py
-dkist_processing_visp/tasks/mixin/input_frame_loaders.py
 dkist_processing_visp/tasks/mixin/intermediate_frame_helpers.py
 dkist_processing_visp/tasks/mixin/line_zones.py
+dkist_processing_visp/tests/README.rst
 dkist_processing_visp/tests/__init__.py
 dkist_processing_visp/tests/conftest.py
+dkist_processing_visp/tests/header_models.py
 dkist_processing_visp/tests/test_assemble_movie.py
 dkist_processing_visp/tests/test_background_light.py
 dkist_processing_visp/tests/test_build_quality_report.py
 dkist_processing_visp/tests/test_dark.py
 dkist_processing_visp/tests/test_downsample.py
 dkist_processing_visp/tests/test_geometric.py
 dkist_processing_visp/tests/test_instrument_polarization.py
```

### Comparing `dkist_processing_visp-2.8.2/dkist_processing_visp.egg-info/requires.txt` & `dkist_processing_visp-2.9.0/dkist_processing_visp.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-dkist-processing-common==4.1.5
-dkist-processing-math==2.0.0
+dkist-processing-common==4.2.0
+dkist-processing-math==2.1.0
 dkist-processing-pac==3.0.0
 dkist-header-validator==4.1.0
 dkist-fits-specifications==3.9.0
 astropy==5.3.0
 numpy==1.24.3
 sunpy==5.0.0
 scipy==1.11.0
@@ -22,18 +22,17 @@
 sphinx-autoapi
 pytest
 towncrier
 dkist-sphinx-theme
 packaging
 
 [grogu]
-dkist==1.1.0
+dkist
 pyparsing
-dkist-inventory==1.2.0
-parfive
+dkist-inventory
 
 [test]
 pytest
 pytest-cov
 pytest-xdist
 pytest-mock
 hypothesis
```

### Comparing `dkist_processing_visp-2.8.2/docs/Makefile` & `dkist_processing_visp-2.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.8.2/docs/background_light.rst` & `dkist_processing_visp-2.9.0/docs/background_light.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Background Light Calibration
 ============================
 
+.. note::
+  A hardware fix for background light was implemented in November 2022. Data taken after Dec. 1st, 2022 are NOT
+  processed with the algorithm described here. This page is preserved mainly for historical reasons.
+
+
 **NOTE:** This page presents a general overview of the method used to identify background light. For the sake of brevity
 there are a lot of small details that are not covered here.
 
 Introduction
 ------------
 
 The ViSP instrument has been shown to suffer from highly structured “background” light that affects all exposures.
@@ -29,18 +34,19 @@
 light is additive. A subtle point here is that the background signal will be constant at a particular exposure time;
 a brighter source will not make a brighter background signal. Background light is additive.
 
 POLCAL Frames Differ By a Multiplicative Factor
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 To understand the other piece of the puzzle we need to talk a little about the POLCAL task type. If you want to really
-fall down the rabbit hole then check out the docs of `dkist-processing-pac`, but the important thing to note is that
-every single POLCAL frame (except the darks, but we’ll ignore those) is theoretically an exposure of exactly the same thing.
-Let's say that again: all POLCAL frames *observe* the same thing. They have different values, however, because of
-polarizing optics that are placed in the beam path. Importantly, these optics scale the input light by a constant multiple.
+fall down the rabbit hole then check out `the docs of dkist-processing-pac <https://docs.dkist.nso.edu/projects/pac/en/stable/background.html>`_,
+but the important thing to note is that every single POLCAL frame (except the darks, but we’ll ignore those) is
+theoretically an exposure of exactly the same thing. Let's say that again: all POLCAL frames *observe* the same thing.
+They have different values, however, because of polarizing optics that are placed in the beam path. Importantly, these
+optics scale the input light by a constant multiple.
 
 So to bring it all together, POCAL frames all *observe* the same thing, but *record* differently scaled values of that thing.
 
 The Algorithm
 ^^^^^^^^^^^^^
 
 To put what was just said into math we can say that the recorded signal, :math:`F_i`, for POLCAL frame :math:`i` can be written as
@@ -76,15 +82,15 @@
 following caveats. It is only intended to get data “good enough” not “great”.
 
 **Caveats**:
 
 * Because the algorithm relies on POLCAL data it cannot be done when no POLCAL data exist. This means that
   “intensity only” ViSP observations are uncorrectable.
 
-* The true observed signal, , actually does change over the course of a POCAL run because the Sun itself is changing.
+* The true observed signal, :math:`f`, actually does change over the course of a POCAL run because the Sun itself is changing.
   This is most evident in the spectral lines themselves, and the result is that part of these lines are identified as
   “background light”.
 
 * This algorithm is very expensive and there is a huge trade-off between accuracy and time of execution (which can be
   10s of hours at the most accurate end). We are currently investigating how to get “good enough” in a reasonable time.
 
 * We currently can make absolutely NO assumptions about the shape of the background signal, either spectrally or spatially,
```

### Comparing `dkist_processing_visp-2.8.2/docs/conf.py` & `dkist_processing_visp-2.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.8.2/docs/gain_correction.rst` & `dkist_processing_visp-2.9.0/docs/gain_correction.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.8.2/docs/l0_to_l1_visp.rst` & `dkist_processing_visp-2.9.0/docs/l0_to_l1_visp.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.8.2/docs/make.bat` & `dkist_processing_visp-2.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.8.2/docs/polarization_calibration.rst` & `dkist_processing_visp-2.9.0/docs/polarization_calibration.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.8.2/docs/science_calibration.rst` & `dkist_processing_visp-2.9.0/docs/science_calibration.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.8.2/licenses/LICENSE.rst` & `dkist_processing_visp-2.9.0/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.8.2/pyproject.toml` & `dkist_processing_visp-2.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.8.2/setup.cfg` & `dkist_processing_visp-2.9.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 
 [options]
 python_requires = >=3.11
 setup_requires = setuptools_scm
 packages = find:
 include_package_data = True
 install_requires = 
-	dkist-processing-common == 4.1.5
-	dkist-processing-math == 2.0.0
+	dkist-processing-common == 4.2.0
+	dkist-processing-math == 2.1.0
 	dkist-processing-pac == 3.0.0
 	dkist-header-validator == 4.1.0
 	dkist-fits-specifications == 3.9.0
 	astropy == 5.3.0
 	numpy == 1.24.3
 	sunpy == 5.0.0
 	scipy == 1.11.0
@@ -42,18 +42,17 @@
 	pytest-cov
 	pytest-xdist
 	pytest-mock
 	hypothesis
 	towncrier
 	dkist-data-simulator >= 2.1.0
 grogu = 
-	dkist == 1.1.0
+	dkist
 	pyparsing
-	dkist-inventory == 1.2.0
-	parfive
+	dkist-inventory
 docs = 
 	sphinx
 	sphinx-astropy
 	sphinx-changelog == 1.3.0
 	sphinx-autoapi
 	pytest
 	towncrier
```

