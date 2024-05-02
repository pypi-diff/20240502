# Comparing `tmp/dkist_processing_cryonirsp-0.0.8.tar.gz` & `tmp/dkist_processing_cryonirsp-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist_processing_cryonirsp-0.0.8.tar", last modified: Thu Sep 21 16:54:14 2023, max compression
+gzip compressed data, was "dkist_processing_cryonirsp-0.0.9.tar", last modified: Fri Sep 29 18:07:03 2023, max compression
```

## Comparing `dkist_processing_cryonirsp-0.0.8.tar` & `dkist_processing_cryonirsp-0.0.9.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-09-21 16:54:14.063020 dkist_processing_cryonirsp-0.0.8/
--rw-rw-rw-   0 root         (0) root         (0)     2461 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      804 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      306 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/.readthedocs.yml
--rw-rw-rw-   0 root         (0) root         (0)     1639 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     6192 2023-09-21 16:54:14.063020 dkist_processing_cryonirsp-0.0.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5677 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/SCIENCE_CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     3479 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-09-21 16:54:14.051020 dkist_processing_cryonirsp-0.0.8/changelog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/changelog/.gitempty
--rwxrwxrwx   0 root         (0) root         (0)      644 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/check_changelog_updated.sh
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-09-21 16:54:14.051020 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/
--rw-rw-rw-   0 root         (0) root         (0)      249 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-09-21 16:54:14.055020 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/models/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5900 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/models/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     1460 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/models/filter.py
--rwxrwxrwx   0 root         (0) root         (0)     9347 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/models/parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     6119 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/models/tags.py
--rw-rw-rw-   0 root         (0) root         (0)      755 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/models/task_name.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-09-21 16:54:14.055020 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/parsers/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/parsers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2832 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/parsers/cryonirsp_l0_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)      886 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/parsers/cryonirsp_l1_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)     6471 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/parsers/map_repeats.py
--rw-rw-rw-   0 root         (0) root         (0)     1872 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/parsers/measurements.py
--rw-rw-rw-   0 root         (0) root         (0)     2001 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/parsers/modstates.py
--rw-rw-rw-   0 root         (0) root         (0)     1104 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/parsers/polarimeter_mode.py
--rw-rw-rw-   0 root         (0) root         (0)     1754 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/parsers/polcal_task.py
--rw-rw-rw-   0 root         (0) root         (0)     2851 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/parsers/scan_step.py
--rw-rw-rw-   0 root         (0) root         (0)     1499 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/parsers/task.py
--rw-rw-rw-   0 root         (0) root         (0)     2547 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/parsers/time.py
--rw-rw-rw-   0 root         (0) root         (0)      883 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/parsers/wavelength.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-09-21 16:54:14.059020 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tasks/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5593 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tasks/assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)     3651 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tasks/bad_pixel_map.py
--rw-rw-rw-   0 root         (0) root         (0)     6863 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tasks/beam_boundaries_base.py
--rw-rw-rw-   0 root         (0) root         (0)     2095 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tasks/ci_beam_boundaries.py
--rw-rw-rw-   0 root         (0) root         (0)     6301 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tasks/ci_science.py
--rw-rw-rw-   0 root         (0) root         (0)     2190 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tasks/cryonirsp_base.py
--rw-rw-rw-   0 root         (0) root         (0)     3674 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tasks/dark.py
--rw-rw-rw-   0 root         (0) root         (0)     7591 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tasks/gain.py
--rw-rw-rw-   0 root         (0) root         (0)    17438 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tasks/instrument_polarization.py
--rw-rw-rw-   0 root         (0) root         (0)      645 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tasks/l1_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)    12315 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tasks/linearity_correction.py
--rw-rw-rw-   0 root         (0) root         (0)    14373 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tasks/make_movie_frames.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-09-21 16:54:14.059020 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tasks/mixin/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tasks/mixin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1629 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tasks/mixin/beam_access.py
--rw-rw-rw-   0 root         (0) root         (0)     4964 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tasks/mixin/corrections.py
--rw-rw-rw-   0 root         (0) root         (0)     7111 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tasks/mixin/intermediate_frame.py
--rw-rw-rw-   0 root         (0) root         (0)     9045 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tasks/mixin/linearized_frame.py
--rw-rw-rw-   0 root         (0) root         (0)     8314 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tasks/parse.py
--rw-rw-rw-   0 root         (0) root         (0)    11113 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tasks/quality_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)    15332 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tasks/science_base.py
--rw-rw-rw-   0 root         (0) root         (0)     9003 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tasks/sp_beam_boundaries.py
--rw-rw-rw-   0 root         (0) root         (0)    24948 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tasks/sp_geometric.py
--rw-rw-rw-   0 root         (0) root         (0)    11014 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tasks/sp_science.py
--rw-rw-rw-   0 root         (0) root         (0)    24415 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tasks/sp_solar_gain.py
--rw-rw-rw-   0 root         (0) root         (0)     1585 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tasks/trial_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)    12230 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tasks/write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-09-21 16:54:14.063020 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tests/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    23677 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tests/ci_e2e_test.py
--rwxrwxrwx   0 root         (0) root         (0)    24472 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     4229 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tests/e2e_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     6104 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tests/e2e_linearize.py
--rw-rw-rw-   0 root         (0) root         (0)    22840 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tests/sp_e2e_test.py
--rw-rw-rw-   0 root         (0) root         (0)     4804 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tests/test_assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)     4774 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tests/test_bad_pixel_maps.py
--rw-rw-rw-   0 root         (0) root         (0)     4458 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tests/test_build_quality_report.py
--rw-rw-rw-   0 root         (0) root         (0)     4484 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tests/test_ci_beam_boundaries.py
--rw-rw-rw-   0 root         (0) root         (0)     4563 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tests/test_ci_make_movie_frames.py
--rw-rw-rw-   0 root         (0) root         (0)    13634 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tests/test_ci_science.py
--rw-rw-rw-   0 root         (0) root         (0)     7010 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tests/test_cryo_base.py
--rw-rw-rw-   0 root         (0) root         (0)     2180 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tests/test_cryo_constants.py
--rw-rw-rw-   0 root         (0) root         (0)    10386 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tests/test_dark.py
--rw-rw-rw-   0 root         (0) root         (0)    11805 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tests/test_gain.py
--rw-rw-rw-   0 root         (0) root         (0)    18444 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tests/test_instrument_polarization.py
--rw-rw-rw-   0 root         (0) root         (0)     5502 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tests/test_linearity_correction.py
--rwxrwxrwx   0 root         (0) root         (0)     8097 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tests/test_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)    26092 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tests/test_parse.py
--rw-rw-rw-   0 root         (0) root         (0)     4309 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tests/test_quality.py
--rw-rw-rw-   0 root         (0) root         (0)     4696 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tests/test_sp_beam_boundaries.py
--rw-rw-rw-   0 root         (0) root         (0)    10776 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tests/test_sp_geometric.py
--rw-rw-rw-   0 root         (0) root         (0)     4553 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tests/test_sp_make_movie_frames.py
--rw-rw-rw-   0 root         (0) root         (0)    15713 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tests/test_sp_science.py
--rw-rw-rw-   0 root         (0) root         (0)     9085 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tests/test_sp_solar.py
--rw-rw-rw-   0 root         (0) root         (0)     1930 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tests/test_submit_qualilty.py
--rw-rw-rw-   0 root         (0) root         (0)      291 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tests/test_workflows.py
--rw-rw-rw-   0 root         (0) root         (0)    10410 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tests/test_write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-09-21 16:54:14.063020 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/workflows/
--rw-rw-rw-   0 root         (0) root         (0)      249 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/workflows/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3892 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/workflows/ci_l0_processing.py
--rw-rw-rw-   0 root         (0) root         (0)     4066 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/workflows/sp_l0_processing.py
--rw-rw-rw-   0 root         (0) root         (0)     7794 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/workflows/trial_workflows.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-09-21 16:54:14.055020 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     6192 2023-09-21 16:54:13.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4800 2023-09-21 16:54:14.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-09-21 16:54:13.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      598 2023-09-21 16:54:13.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-09-21 16:54:13.000000 dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-09-21 16:54:14.063020 dkist_processing_cryonirsp-0.0.8/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4598 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      120 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     2038 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      213 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      657 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/docs/l0_to_l1_cryonirsp_ci.rst
--rw-rw-rw-   0 root         (0) root         (0)      657 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/docs/l0_to_l1_cryonirsp_sp.rst
--rw-rw-rw-   0 root         (0) root         (0)     4513 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)       29 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/docs/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      297 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/docs/requirements_table.rst
--rw-rw-rw-   0 root         (0) root         (0)      300 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/docs/scientific_changelog.rst
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-09-21 16:54:14.063020 dkist_processing_cryonirsp-0.0.8/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1462 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      786 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/pyproject.toml
--rwxrwxrwx   0 root         (0) root         (0)       60 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/science_towncrier.sh
--rw-rw-rw-   0 root         (0) root         (0)     1590 2023-09-21 16:54:14.063020 dkist_processing_cryonirsp-0.0.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      102 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      432 2023-09-21 16:54:06.000000 dkist_processing_cryonirsp-0.0.8/towncrier_science.toml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-09-29 18:07:03.799961 dkist_processing_cryonirsp-0.0.9/
+-rw-rw-rw-   0 root         (0) root         (0)     2461 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      804 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      306 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/.readthedocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2106 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6192 2023-09-29 18:07:03.799961 dkist_processing_cryonirsp-0.0.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5677 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/SCIENCE_CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3479 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-09-29 18:07:03.783961 dkist_processing_cryonirsp-0.0.9/changelog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/changelog/.gitempty
+-rwxrwxrwx   0 root         (0) root         (0)      644 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/check_changelog_updated.sh
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-09-29 18:07:03.783961 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/
+-rw-rw-rw-   0 root         (0) root         (0)      249 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-09-29 18:07:03.787961 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/models/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5900 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/models/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     1460 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/models/filter.py
+-rwxrwxrwx   0 root         (0) root         (0)     9347 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/models/parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     6119 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/models/tags.py
+-rw-rw-rw-   0 root         (0) root         (0)      755 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/models/task_name.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-09-29 18:07:03.787961 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/parsers/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/parsers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2832 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/parsers/cryonirsp_l0_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)      886 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/parsers/cryonirsp_l1_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)     6471 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/parsers/map_repeats.py
+-rw-rw-rw-   0 root         (0) root         (0)     1872 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/parsers/measurements.py
+-rw-rw-rw-   0 root         (0) root         (0)     2001 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/parsers/modstates.py
+-rw-rw-rw-   0 root         (0) root         (0)     1104 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/parsers/polarimeter_mode.py
+-rw-rw-rw-   0 root         (0) root         (0)     1754 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/parsers/polcal_task.py
+-rw-rw-rw-   0 root         (0) root         (0)     2851 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/parsers/scan_step.py
+-rw-rw-rw-   0 root         (0) root         (0)     1499 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/parsers/task.py
+-rw-rw-rw-   0 root         (0) root         (0)     2547 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/parsers/time.py
+-rw-rw-rw-   0 root         (0) root         (0)      883 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/parsers/wavelength.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-09-29 18:07:03.791961 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5593 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tasks/assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)     3651 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tasks/bad_pixel_map.py
+-rw-rw-rw-   0 root         (0) root         (0)     6863 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tasks/beam_boundaries_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2095 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tasks/ci_beam_boundaries.py
+-rw-rw-rw-   0 root         (0) root         (0)     6301 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tasks/ci_science.py
+-rw-rw-rw-   0 root         (0) root         (0)     2104 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tasks/cryonirsp_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3674 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tasks/dark.py
+-rw-rw-rw-   0 root         (0) root         (0)     7591 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tasks/gain.py
+-rw-rw-rw-   0 root         (0) root         (0)    17438 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tasks/instrument_polarization.py
+-rw-rw-rw-   0 root         (0) root         (0)      645 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tasks/l1_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    12342 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tasks/linearity_correction.py
+-rw-rw-rw-   0 root         (0) root         (0)    14814 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tasks/make_movie_frames.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-09-29 18:07:03.795961 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tasks/mixin/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tasks/mixin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1629 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tasks/mixin/beam_access.py
+-rw-rw-rw-   0 root         (0) root         (0)     4964 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tasks/mixin/corrections.py
+-rw-rw-rw-   0 root         (0) root         (0)     7417 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tasks/mixin/intermediate_frame.py
+-rw-rw-rw-   0 root         (0) root         (0)     9259 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tasks/mixin/linearized_frame.py
+-rw-rw-rw-   0 root         (0) root         (0)     8314 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tasks/parse.py
+-rw-rw-rw-   0 root         (0) root         (0)    11292 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tasks/quality_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)    15464 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tasks/science_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     9003 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tasks/sp_beam_boundaries.py
+-rw-rw-rw-   0 root         (0) root         (0)    24948 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tasks/sp_geometric.py
+-rw-rw-rw-   0 root         (0) root         (0)    11014 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tasks/sp_science.py
+-rw-rw-rw-   0 root         (0) root         (0)    24415 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tasks/sp_solar_gain.py
+-rw-rw-rw-   0 root         (0) root         (0)     1585 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tasks/trial_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    12230 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tasks/write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-09-29 18:07:03.799961 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    23677 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tests/ci_e2e_test.py
+-rwxrwxrwx   0 root         (0) root         (0)    24472 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     4229 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tests/e2e_helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     6104 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tests/e2e_linearize.py
+-rw-rw-rw-   0 root         (0) root         (0)    22840 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tests/sp_e2e_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     4949 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tests/test_assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)     4875 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tests/test_bad_pixel_maps.py
+-rw-rw-rw-   0 root         (0) root         (0)     4458 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tests/test_build_quality_report.py
+-rw-rw-rw-   0 root         (0) root         (0)     4585 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tests/test_ci_beam_boundaries.py
+-rw-rw-rw-   0 root         (0) root         (0)     4676 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tests/test_ci_make_movie_frames.py
+-rw-rw-rw-   0 root         (0) root         (0)    13855 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tests/test_ci_science.py
+-rw-rw-rw-   0 root         (0) root         (0)     7172 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tests/test_cryo_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2180 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tests/test_cryo_constants.py
+-rw-rw-rw-   0 root         (0) root         (0)    10535 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tests/test_dark.py
+-rw-rw-rw-   0 root         (0) root         (0)    12048 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tests/test_gain.py
+-rw-rw-rw-   0 root         (0) root         (0)    18573 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tests/test_instrument_polarization.py
+-rw-rw-rw-   0 root         (0) root         (0)     5611 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tests/test_linearity_correction.py
+-rwxrwxrwx   0 root         (0) root         (0)     8097 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tests/test_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)    26626 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tests/test_parse.py
+-rw-rw-rw-   0 root         (0) root         (0)     4418 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tests/test_quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     4797 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tests/test_sp_beam_boundaries.py
+-rw-rw-rw-   0 root         (0) root         (0)    10909 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tests/test_sp_geometric.py
+-rw-rw-rw-   0 root         (0) root         (0)     4666 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tests/test_sp_make_movie_frames.py
+-rw-rw-rw-   0 root         (0) root         (0)    15942 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tests/test_sp_science.py
+-rw-rw-rw-   0 root         (0) root         (0)     9194 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tests/test_sp_solar.py
+-rw-rw-rw-   0 root         (0) root         (0)     1930 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tests/test_submit_qualilty.py
+-rw-rw-rw-   0 root         (0) root         (0)      291 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tests/test_workflows.py
+-rw-rw-rw-   0 root         (0) root         (0)    10527 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tests/test_write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-09-29 18:07:03.799961 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/workflows/
+-rw-rw-rw-   0 root         (0) root         (0)      249 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/workflows/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3892 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/workflows/ci_l0_processing.py
+-rw-rw-rw-   0 root         (0) root         (0)     4066 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/workflows/sp_l0_processing.py
+-rw-rw-rw-   0 root         (0) root         (0)     7794 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/workflows/trial_workflows.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-09-29 18:07:03.783961 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     6192 2023-09-29 18:07:03.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4800 2023-09-29 18:07:03.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-09-29 18:07:03.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      598 2023-09-29 18:07:03.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-09-29 18:07:03.000000 dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-09-29 18:07:03.799961 dkist_processing_cryonirsp-0.0.9/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4598 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2038 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      213 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      657 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/docs/l0_to_l1_cryonirsp_ci.rst
+-rw-rw-rw-   0 root         (0) root         (0)      657 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/docs/l0_to_l1_cryonirsp_sp.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)       29 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/docs/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      297 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/docs/requirements_table.rst
+-rw-rw-rw-   0 root         (0) root         (0)      300 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/docs/scientific_changelog.rst
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-09-29 18:07:03.799961 dkist_processing_cryonirsp-0.0.9/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      786 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/pyproject.toml
+-rwxrwxrwx   0 root         (0) root         (0)       60 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/science_towncrier.sh
+-rw-rw-rw-   0 root         (0) root         (0)     1590 2023-09-29 18:07:03.799961 dkist_processing_cryonirsp-0.0.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      102 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      432 2023-09-29 18:06:47.000000 dkist_processing_cryonirsp-0.0.9/towncrier_science.toml
```

### Comparing `dkist_processing_cryonirsp-0.0.8/.gitignore` & `dkist_processing_cryonirsp-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.8/.pre-commit-config.yaml` & `dkist_processing_cryonirsp-0.0.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.8/CHANGELOG.rst` & `dkist_processing_cryonirsp-0.0.9/CHANGELOG.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+v0.0.9 (2023-09-29)
+===================
+
+Features
+--------
+
+- Removes all references to the FitsDataMixin and its methods, which are deprecated. Uses the new self.read() and self.write() methods with encoder and decoder support. (`#63 <https://bitbucket.org/dkistdc/dkist-processing-cryonirsp/pull-requests/63>`__)
+
+
+Misc
+----
+
+- Update pillow to address security vulnerability. (`#66 <https://bitbucket.org/dkistdc/dkist-processing-cryonirsp/pull-requests/66>`__)
+
+
 v0.0.8 (2023-09-21)
 ===================
 
 Misc
 ----
 
 - Update dkist-fits-specifications to conform to Revision I of SPEC-0122.
```

### Comparing `dkist_processing_cryonirsp-0.0.8/PKG-INFO` & `dkist_processing_cryonirsp-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist_processing_cryonirsp
-Version: 0.0.8
+Version: 0.0.9
 Summary: Science processing code for the Cryo-NIRSP instrument on DKIST
 Home-page: https://bitbucket.org/dkistdc/dkist_processing_cryonirsp/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dkist_processing_cryonirsp-0.0.8/README.rst` & `dkist_processing_cryonirsp-0.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.8/bitbucket-pipelines.yml` & `dkist_processing_cryonirsp-0.0.9/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.8/check_changelog_updated.sh` & `dkist_processing_cryonirsp-0.0.9/check_changelog_updated.sh`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/models/constants.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/models/constants.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/models/filter.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/models/filter.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/models/parameters.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/models/parameters.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/models/tags.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/models/tags.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/models/task_name.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/models/task_name.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/parsers/cryonirsp_l0_fits_access.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/parsers/cryonirsp_l0_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/parsers/cryonirsp_l1_fits_access.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/parsers/cryonirsp_l1_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/parsers/map_repeats.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/parsers/map_repeats.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/parsers/measurements.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/parsers/measurements.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/parsers/modstates.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/parsers/modstates.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/parsers/polarimeter_mode.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/parsers/polarimeter_mode.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/parsers/polcal_task.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/parsers/polcal_task.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/parsers/scan_step.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/parsers/scan_step.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/parsers/task.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/parsers/task.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/parsers/time.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/parsers/time.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/parsers/wavelength.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/parsers/wavelength.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tasks/assemble_movie.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tasks/assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tasks/bad_pixel_map.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tasks/bad_pixel_map.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tasks/beam_boundaries_base.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tasks/beam_boundaries_base.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tasks/ci_beam_boundaries.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tasks/ci_beam_boundaries.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tasks/ci_science.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tasks/ci_science.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tasks/cryonirsp_base.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tasks/cryonirsp_base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """CryoNIRSP base class."""
 from abc import ABC
 
 from dkist_processing_common.tasks import WorkflowTaskBase
-from dkist_processing_common.tasks.mixin.fits import FitsDataMixin
 from dkist_processing_common.tasks.mixin.input_dataset import InputDatasetMixin
 from dkist_processing_common.tasks.mixin.quality import QualityMixin
 
 from dkist_processing_cryonirsp.models.constants import CryonirspConstants
 from dkist_processing_cryonirsp.models.parameters import CryonirspParameters
 from dkist_processing_cryonirsp.tasks.mixin.beam_access import BeamAccessMixin
 from dkist_processing_cryonirsp.tasks.mixin.corrections import CorrectionsMixin
@@ -16,15 +15,14 @@
 from dkist_processing_cryonirsp.tasks.mixin.linearized_frame import (
     LinearizedFrameMixin,
 )
 
 
 class CryonirspTaskBase(
     WorkflowTaskBase,
-    FitsDataMixin,
     InputDatasetMixin,
     BeamAccessMixin,
     LinearizedFrameMixin,
     IntermediateFrameMixin,
     CorrectionsMixin,
     QualityMixin,
     ABC,
```

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tasks/dark.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tasks/dark.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tasks/gain.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tasks/gain.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tasks/instrument_polarization.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tasks/instrument_polarization.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tasks/l1_output_data.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tasks/l1_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tasks/linearity_correction.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tasks/linearity_correction.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import sys
 from dataclasses import dataclass
 from typing import Generator
 
 import numpy as np
 from astropy.io import fits
 from dkist_processing_common.codecs.fits import fits_access_decoder
+from dkist_processing_common.codecs.fits import fits_hdulist_encoder
 from dkist_processing_common.models.tags import Tag
 from dkist_processing_common.tasks import WorkflowTaskBase
-from dkist_processing_common.tasks.mixin.fits import FitsDataMixin
 from dkist_processing_common.tasks.mixin.input_dataset import InputDatasetMixin
 from logging42 import logger
 from numba import njit
 from numba import prange
 
 from dkist_processing_cryonirsp.models.constants import CryonirspConstants
 from dkist_processing_cryonirsp.models.parameters import CryonirspParameters
@@ -23,15 +23,15 @@
 @dataclass
 class _RampSet:
     current_ramp_set_num: int
     total_ramp_sets: int
     time_obs: str
 
 
-class LinearityCorrection(WorkflowTaskBase, InputDatasetMixin, FitsDataMixin):
+class LinearityCorrection(WorkflowTaskBase, InputDatasetMixin):
     """Task class for performing linearity correction on all input frames, regardless of task type."""
 
     constants: CryonirspConstants
 
     record_provenance = True
 
     @property
@@ -86,17 +86,18 @@
                     )
                 with self.apm_task_step("Package Linearized Frame With Metadata"):
                     header, tags = self._generate_output_array_metadata(
                         input_ramp_frame=ramp_objs[-1]
                     )
                     hdul = fits.HDUList([fits.PrimaryHDU(header=header, data=output_array)])
                 with self.apm_writing_step("Write Linearized Frame"):
-                    self.fits_data_write(
-                        hdu_list=hdul,
+                    self.write(
+                        data=hdul,
                         tags=tags,
+                        encoder=fits_hdulist_encoder,
                     )
 
     def _identify_ramp_sets(self) -> Generator[_RampSet, None, None]:
         """
         Identify the ramp sets that will be corrected together.
 
         We use date-obs to identify individual ramp sets here.
```

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tasks/make_movie_frames.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tasks/make_movie_frames.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """Cryonirsp make movie frames task."""
 from abc import ABC
 from abc import abstractmethod
 
 import numpy as np
 from astropy.io import fits
 from astropy.visualization import ZScaleInterval
+from dkist_processing_common.codecs.fits import fits_access_decoder
+from dkist_processing_common.codecs.fits import fits_hdulist_encoder
 from logging42 import logger
 
 from dkist_processing_cryonirsp.models.tags import CryonirspTag
 from dkist_processing_cryonirsp.parsers.cryonirsp_l1_fits_access import CryonirspL1FitsAccess
 from dkist_processing_cryonirsp.tasks.cryonirsp_base import CryonirspTaskBase
 
 
@@ -56,24 +58,25 @@
         return result
 
     def get_movie_header(
         self, map_scan: int, scan_step: int, meas_num: int, stokes_state: str
     ) -> fits.Header:
         """Create a header to use on a movie frame based on a calibrated frame."""
         calibrated_frame = next(
-            self.fits_data_read_fits_access(
+            self.read(
                 tags=[
                     CryonirspTag.frame(),
                     CryonirspTag.output(),
                     CryonirspTag.stokes(stokes_state),
                     CryonirspTag.meas_num(meas_num),
                     CryonirspTag.map_scan(map_scan),
                     CryonirspTag.scan_step(scan_step),
                 ],
-                cls=CryonirspL1FitsAccess,
+                decoder=fits_access_decoder,
+                fits_access_class=CryonirspL1FitsAccess,
             )
         )
         header = calibrated_frame.header
         return header
 
 
 class CIMakeCryonirspMovieFrames(MakeCryonirspMovieFramesBase):
@@ -88,21 +91,22 @@
                 ):
                     movie_frame_hdu = self.make_full_stokes_frame(
                         map_scan=map_scan, scan_step=scan_step
                     )
                 with self.apm_writing_step(
                     f"Writing full stokes movie frame for {map_scan=} and {scan_step=}"
                 ):
-                    self.fits_data_write(
-                        hdu_list=fits.HDUList([movie_frame_hdu]),
+                    self.write(
+                        data=fits.HDUList([movie_frame_hdu]),
                         tags=[
                             CryonirspTag.map_scan(map_scan),
                             CryonirspTag.scan_step(scan_step),
                             CryonirspTag.movie_frame(),
                         ],
+                        encoder=fits_hdulist_encoder,
                     )
 
     def make_intensity_movie_frames(self):
         """Make a movie out of stokes I frames."""
         for map_scan in range(1, self.constants.num_map_scans + 1):
             for scan_step in range(1, self.constants.num_scan_steps + 1):
                 with self.apm_processing_step(
@@ -110,21 +114,22 @@
                 ):
                     movie_frame_hdu = self.make_intensity_frame(
                         map_scan=map_scan, scan_step=scan_step
                     )
                 with self.apm_writing_step(
                     f"Writing intensity movie frame for {map_scan=} and {scan_step=}"
                 ):
-                    self.fits_data_write(
-                        hdu_list=fits.HDUList([movie_frame_hdu]),
+                    self.write(
+                        data=fits.HDUList([movie_frame_hdu]),
                         tags=[
                             CryonirspTag.map_scan(map_scan),
                             CryonirspTag.scan_step(scan_step),
                             CryonirspTag.movie_frame(),
                         ],
+                        encoder=fits_hdulist_encoder,
                     )
 
     def make_full_stokes_frame(self, map_scan: int, scan_step: int) -> fits.PrimaryHDU:
         """Create a movie frame (data + header) with the stokes frames (IQUV) combined into top left, top right, bottom left, bottom right quadrants respectively."""
         meas_num = 1  # Use only the first measurement if there are multiple measurements.
         stokes_i = self.get_movie_frame(
             map_scan=map_scan, scan_step=scan_step, meas_num=meas_num, stokes_state="I"
@@ -161,24 +166,25 @@
         return fits.PrimaryHDU(header=movie_header, data=stokes_i)
 
     def get_movie_frame(
         self, map_scan: int, scan_step: int, meas_num: int, stokes_state: str
     ) -> np.ndarray:
         """Retrieve the calibrated frame data for the first frame which matches the input parameters and transform it into a movie frame (i.e. normalize the values)."""
         calibrated_frame = next(
-            self.fits_data_read_fits_access(
+            self.read(
                 tags=[
                     CryonirspTag.frame(),
                     CryonirspTag.output(),
                     CryonirspTag.stokes(stokes_state),
                     CryonirspTag.meas_num(meas_num),
                     CryonirspTag.map_scan(map_scan),
                     CryonirspTag.scan_step(scan_step),
                 ],
-                cls=CryonirspL1FitsAccess,
+                decoder=fits_access_decoder,
+                fits_access_class=CryonirspL1FitsAccess,
             )
         )
         movie_frame = self.scale_for_rendering(calibrated_frame.data)
         return movie_frame
 
 
 class SPMakeCryonirspMovieFrames(MakeCryonirspMovieFramesBase):
@@ -186,34 +192,36 @@
 
     def make_full_stokes_movie_frames(self):
         """Make a movie that combines each of the stokes frames into a single movie frame."""
         for map_scan in range(1, self.constants.num_map_scans + 1):
             with self.apm_processing_step(f"Generate full stokes movie frame for {map_scan=}"):
                 movie_frame_hdu = self.make_full_stokes_frame(map_scan=map_scan)
             with self.apm_writing_step(f"Writing full stokes movie frame for {map_scan=}"):
-                self.fits_data_write(
-                    hdu_list=fits.HDUList([movie_frame_hdu]),
+                self.write(
+                    data=fits.HDUList([movie_frame_hdu]),
                     tags=[
                         CryonirspTag.map_scan(map_scan),
                         CryonirspTag.movie_frame(),
                     ],
+                    encoder=fits_hdulist_encoder,
                 )
 
     def make_intensity_movie_frames(self):
         """Make a movie out of stokes I frames."""
         for map_scan in range(1, self.constants.num_map_scans + 1):
             with self.apm_processing_step(f"Generate intensity movie frame for {map_scan=}"):
                 movie_frame_hdu = self.make_intensity_frame(map_scan=map_scan)
             with self.apm_writing_step(f"Writing intensity movie frame for {map_scan=}"):
-                self.fits_data_write(
-                    hdu_list=fits.HDUList([movie_frame_hdu]),
+                self.write(
+                    data=fits.HDUList([movie_frame_hdu]),
                     tags=[
                         CryonirspTag.map_scan(map_scan),
                         CryonirspTag.movie_frame(),
                     ],
+                    encoder=fits_hdulist_encoder,
                 )
 
     def make_full_stokes_frame(self, map_scan: int) -> fits.PrimaryHDU:
         """Create a movie frame (data + header) with the stokes frames (IQUV) combined into top left, top right, bottom left, bottom right quadrants respectively."""
         meas_num = 1  # Use only the first measurement if there are multiple measurements.
         stokes_i = self.get_movie_frame(map_scan=map_scan, meas_num=meas_num, stokes_state="I")
         stokes_q = self.get_movie_frame(map_scan=map_scan, meas_num=meas_num, stokes_state="Q")
@@ -255,24 +263,25 @@
 
     def get_spectral_calibrated_frame(
         self, map_scan: int, meas_num: int, stokes_state: str
     ) -> np.ndarray:
         """Retrieve a calibrated frame for a single scan step (no integration)."""
         scan_step = 1  # There is only a single scan step in a spectral movie
         calibrated_frame = next(
-            self.fits_data_read_fits_access(
+            self.read(
                 tags=[
                     CryonirspTag.frame(),
                     CryonirspTag.output(),
                     CryonirspTag.stokes(stokes_state),
                     CryonirspTag.meas_num(meas_num),
                     CryonirspTag.map_scan(map_scan),
                     CryonirspTag.scan_step(scan_step),
                 ],
-                cls=CryonirspL1FitsAccess,
+                decoder=fits_access_decoder,
+                fits_access_class=CryonirspL1FitsAccess,
             )
         )
         return calibrated_frame.data
 
     def get_integrated_calibrated_frame(
         self, map_scan: int, meas_num: int, stokes_state: str
     ) -> np.ndarray:
@@ -280,24 +289,25 @@
         data = self.get_spectral_calibrated_frame(
             map_scan=map_scan, meas_num=meas_num, stokes_state=stokes_state
         )
         integrated_data = self.integrate_spectral_frame(data)
         integrated_arrays = [integrated_data]
         for scan_step in range(2, self.constants.num_scan_steps + 1):
             calibrated_frame = next(
-                self.fits_data_read_fits_access(
+                self.read(
                     tags=[
                         CryonirspTag.frame(),
                         CryonirspTag.output(),
                         CryonirspTag.stokes(stokes_state),
                         CryonirspTag.meas_num(meas_num),
                         CryonirspTag.map_scan(map_scan),
                         CryonirspTag.scan_step(scan_step),
                     ],
-                    cls=CryonirspL1FitsAccess,
+                    decoder=fits_access_decoder,
+                    fits_access_class=CryonirspL1FitsAccess,
                 )
             )
             integrated_data = self.integrate_spectral_frame(calibrated_frame.data)
             integrated_arrays.append(integrated_data)
         full_frame = np.vstack(integrated_arrays)
         return full_frame
```

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tasks/mixin/beam_access.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tasks/mixin/beam_access.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tasks/mixin/corrections.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tasks/mixin/corrections.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tasks/mixin/intermediate_frame.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tasks/mixin/intermediate_frame.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """Mixin class providing support for loading and writing intermediate arrays."""
 import logging
 from collections.abc import Generator
 from collections.abc import Iterable
 
 import numpy as np
 from astropy.io import fits
+from dkist_processing_common.codecs.fits import fits_hdu_decoder
+from dkist_processing_common.codecs.fits import fits_hdulist_encoder
 
 from dkist_processing_cryonirsp.models.tags import CryonirspTag
 
 
 class IntermediateFrameMixin:
     """Mixin for methods that support easy loading and writing of intermediate frames."""
 
@@ -17,15 +19,18 @@
         tags: [str],
     ) -> Generator[np.ndarray, None, None]:
         """Yield a generator that produces ndarrays for the requested tags."""
         tags = list(set([CryonirspTag.intermediate(), CryonirspTag.frame()] + tags))
 
         if self.scratch.count_all(tags=tags) == 0:
             raise RuntimeError(f"No files found matching {tags =}")
-        for hdu in self.fits_data_read_hdu(tags=tags):
+        for hdu in self.read(
+            tags=tags,
+            decoder=fits_hdu_decoder,
+        ):
             yield hdu.data
 
     def intermediate_frame_load_beam_boundaries(self, beam: int) -> np.ndarray:
         """Return array containing beam boundaries for a given beam."""
         tags = [CryonirspTag.task_beam_boundaries(), CryonirspTag.beam(beam)]
         return next(self.intermediate_frame_load_intermediate_arrays(tags=tags))
 
@@ -161,10 +166,16 @@
             headers = [headers] if isinstance(headers, fits.Header) else headers
         else:
             headers = [None] * len(list(arrays))
 
         filenames = []
         for array, header in zip(arrays, headers):
             hdul = fits.HDUList([fits.PrimaryHDU(data=array, header=header)])
-            path = str(self.fits_data_write(hdu_list=hdul, tags=tags))
+            path = str(
+                self.write(
+                    data=hdul,
+                    tags=tags,
+                    encoder=fits_hdulist_encoder,
+                )
+            )
             filenames.append(path)
         logging.info(f"Wrote intermediate file(s) for {tags = } to {filenames}")
```

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tasks/mixin/linearized_frame.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tasks/mixin/linearized_frame.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Helper to manage input data."""
 from collections.abc import Generator
 
 import numpy as np
 from astropy.io import fits
+from dkist_processing_common.codecs.fits import fits_access_decoder
 from dkist_processing_common.models.fits_access import FitsAccessBase
 
 from dkist_processing_cryonirsp.models.tags import CryonirspTag
 from dkist_processing_cryonirsp.models.task_name import TaskName
 from dkist_processing_cryonirsp.parsers.cryonirsp_l0_fits_access import CryonirspL0FitsAccess
 
 
@@ -21,28 +22,36 @@
         self,
         tags: [str],
         beam: int,
     ) -> Generator[CryonirspL0FitsAccess, None, None]:
         """Load linearized fits frames based on given tags and extract the desired beam."""
         tags = list(set([CryonirspTag.linearized(), CryonirspTag.frame()] + tags))
 
-        full_frame_generator = self.fits_data_read_fits_access(tags, cls=CryonirspL0FitsAccess)
+        full_frame_generator = self.read(
+            tags=tags,
+            decoder=fits_access_decoder,
+            fits_access_class=CryonirspL0FitsAccess,
+        )
         for item in full_frame_generator:
             header = item.header
             data = self.beam_access_get_beam(array=item.data, beam=beam)
             hdu = fits.PrimaryHDU(header=header, data=data)
             yield CryonirspL0FitsAccess(hdu=hdu)
 
     def linearized_frame_full_array_generator(
         self,
         tags: [str],
     ) -> Generator[np.ndarray, None, None]:
         """Load linearized fits frames based on given tags."""
         tags = list(set([CryonirspTag.linearized(), CryonirspTag.frame()] + tags))
-        frame_generator = self.fits_data_read_fits_access(tags, cls=CryonirspL0FitsAccess)
+        frame_generator = self.read(
+            tags=tags,
+            decoder=fits_access_decoder,
+            fits_access_class=CryonirspL0FitsAccess,
+        )
         for frame in frame_generator:
             yield frame.data
 
     def linearized_frame_dark_array_generator(
         self, exposure_time: float, beam: int
     ) -> Generator[np.ndarray, None, None]:
         """
```

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tasks/parse.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tasks/parse.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tasks/quality_metrics.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tasks/quality_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Cryonirsp quality metrics task."""
 from dataclasses import dataclass
 from dataclasses import field
 from typing import Generator
 
 import numpy as np
 from astropy.time import Time
+from dkist_processing_common.codecs.fits import fits_access_decoder
 from dkist_processing_common.parsers.quality import L1QualityFitsAccess
 from dkist_processing_common.tasks import QualityL0Metrics
 from dkist_processing_common.tasks.mixin.quality import QualityMixin
 from logging42 import logger
 
 from dkist_processing_cryonirsp.models.constants import CryonirspConstants
 from dkist_processing_cryonirsp.models.tags import CryonirspTag
@@ -185,24 +186,25 @@
         """Calculate the sensitivities for each scan step in a map scan."""
         scan_step_sensitivities = _QualityData()
         for step in range(1, self.constants.num_scan_steps + 1):
             avg_stokes_i_data_point = self.get_intensity_frame_average(
                 map_scan=map_scan, step=step, meas_num=1
             )
             frame = next(
-                self.fits_data_read_fits_access(
+                self.read(
                     tags=[
                         CryonirspTag.output(),
                         CryonirspTag.frame(),
                         CryonirspTag.scan_step(step),
                         CryonirspTag.map_scan(map_scan),
                         CryonirspTag.stokes(stokes_state),
                         CryonirspTag.meas_num(meas_num),
                     ],
-                    cls=L1QualityFitsAccess,
+                    decoder=fits_access_decoder,
+                    fits_access_class=L1QualityFitsAccess,
                 )
             )
             scan_step_sensitivity = np.nanstd(frame.data) / avg_stokes_i_data_point.value
             scan_step_sensitivity_data_point = _QualityDataPoint(
                 value=scan_step_sensitivity, datetime=avg_stokes_i_data_point.datetime
             )
             scan_step_sensitivities.data_points.append(scan_step_sensitivity_data_point)
@@ -213,40 +215,42 @@
         return scan_step_sensitivities
 
     def get_intensity_frame_average(
         self, map_scan: int, step: int, meas_num: int
     ) -> _QualityDataPoint:
         """Calculate the average of an intensity frame."""
         frame: L1QualityFitsAccess = next(
-            self.fits_data_read_fits_access(
+            self.read(
                 tags=[
                     CryonirspTag.output(),
                     CryonirspTag.frame(),
                     CryonirspTag.scan_step(step),
                     CryonirspTag.map_scan(map_scan),
                     CryonirspTag.stokes("I"),
                     CryonirspTag.meas_num(meas_num),
                 ],
-                cls=L1QualityFitsAccess,
+                decoder=fits_access_decoder,
+                fits_access_class=L1QualityFitsAccess,
             )
         )
         median = np.nanmedian(frame.data)
         time_obs_mjd = Time(frame.time_obs).mjd
         mean = np.nanmean(frame.data)
         average = median or mean  # TODO: Needs hardening for value of 0
         result = _QualityDataPoint(value=average, datetime=time_obs_mjd)
         logger.info(f"Calculated intensity frame average as {result}")
         return result
 
     def compile_noise_data(self, stokes: str) -> _QualityData:
         """Compile lists of noise values and their observation times."""
         tags = [CryonirspTag.output(), CryonirspTag.frame(), CryonirspTag.stokes(stokes)]
-        frames: Generator[L1QualityFitsAccess, None, None] = self.fits_data_read_fits_access(
+        frames: Generator[L1QualityFitsAccess, None, None] = self.read(
             tags=tags,
-            cls=L1QualityFitsAccess,
+            decoder=fits_access_decoder,
+            fits_access_class=L1QualityFitsAccess,
         )
         result = _QualityData()
         logger.info(f"Compiling noise data for {tags = }")
         for frame in frames:
             data_point = _QualityDataPoint(
                 value=self.avg_noise(frame.data), datetime=frame.time_obs
             )
```

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tasks/science_base.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tasks/science_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from collections.abc import Iterable
 from dataclasses import dataclass
 
 import numpy as np
 from astropy.io import fits
 from astropy.time import Time
 from astropy.time import TimeDelta
+from dkist_processing_common.codecs.fits import fits_hdulist_encoder
 from dkist_processing_math.arithmetic import divide_arrays_by_array
 from dkist_processing_math.arithmetic import subtract_array_from_arrays
 from dkist_processing_math.statistics import average_numpy_arrays
 from dkist_processing_pac.optics.telescope import Telescope
 from logging42 import logger
 
 from dkist_processing_cryonirsp.models.tags import CryonirspTag
@@ -444,11 +445,15 @@
             CryonirspTag.frame(),
             CryonirspTag.stokes(stokes),
             CryonirspTag.meas_num(meas_num),
             CryonirspTag.scan_step(scan_step),
             CryonirspTag.map_scan(map_scan),
         ]
         hdul = fits.HDUList([fits.PrimaryHDU(header=header, data=data)])
-        self.fits_data_write(hdu_list=hdul, tags=tags)
+        self.write(
+            data=hdul,
+            tags=tags,
+            encoder=fits_hdulist_encoder,
+        )
 
         filename = next(self.read(tags=tags))
         logger.info(f"Wrote calibrated frame for {tags = } to {filename}")
```

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tasks/sp_beam_boundaries.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tasks/sp_beam_boundaries.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tasks/sp_geometric.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tasks/sp_geometric.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tasks/sp_science.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tasks/sp_science.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tasks/sp_solar_gain.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tasks/sp_solar_gain.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tasks/trial_output_data.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tasks/trial_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tasks/write_l1.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tasks/write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tests/ci_e2e_test.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tests/ci_e2e_test.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tests/conftest.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tests/e2e_helpers.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tests/e2e_helpers.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tests/e2e_linearize.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tests/e2e_linearize.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tests/sp_e2e_test.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tests/sp_e2e_test.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tests/test_assemble_movie.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tests/test_assemble_movie.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 
 import pytest
 from dkist_processing_common._util.scratch import WorkflowFileSystem
+from dkist_processing_common.codecs.fits import fits_hdulist_encoder
 from dkist_processing_common.tests.conftest import FakeGQLClient
 
 from dkist_processing_cryonirsp.models.tags import CryonirspTag
 from dkist_processing_cryonirsp.tasks.assemble_movie import CIAssembleCryonirspMovie
 from dkist_processing_cryonirsp.tasks.assemble_movie import SPAssembleCryonirspMovie
 from dkist_processing_cryonirsp.tests.conftest import Cryonirsp122ObserveFrames
 from dkist_processing_cryonirsp.tests.conftest import CryonirspConstantsDb
@@ -35,21 +36,22 @@
                 num_exp_per_step=task.num_exp_per_step,
                 num_map_scans=task.testing_num_map_scans,
             )
             header_generator = (d.header() for d in ds)
             for d, header in enumerate(header_generator):
                 for scan_step in range(num_scan_steps + 1):
                     hdl = generate_214_l1_fits_frame(s122_header=header)
-                    task.fits_data_write(
-                        hdu_list=hdl,
+                    task.write(
+                        data=hdl,
                         tags=[
                             CryonirspTag.movie_frame(),
                             CryonirspTag.map_scan(d + 1),
                             CryonirspTag.scan_step(scan_step),
                         ],
+                        encoder=fits_hdulist_encoder,
                     )
             yield task
         finally:
             task._purge()
 
 
 def test_assemble_ci_movie(assemble_ci_task_with_tagged_movie_frames, mocker):
@@ -83,20 +85,21 @@
                 num_steps=task.num_steps,
                 num_exp_per_step=task.num_exp_per_step,
                 num_map_scans=task.testing_num_map_scans,
             )
             header_generator = (d.header() for d in ds)
             for d, header in enumerate(header_generator):
                 hdl = generate_214_l1_fits_frame(s122_header=header)
-                task.fits_data_write(
-                    hdu_list=hdl,
+                task.write(
+                    data=hdl,
                     tags=[
                         CryonirspTag.movie_frame(),
                         CryonirspTag.map_scan(d + 1),
                     ],
+                    encoder=fits_hdulist_encoder,
                 )
             yield task
         finally:
             task._purge()
 
 
 def test_assemble_sp_movie(assemble_sp_task_with_tagged_movie_frames, mocker):
```

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tests/test_bad_pixel_maps.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tests/test_bad_pixel_maps.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from datetime import datetime
 
 import numpy as np
 import pytest
 from astropy.io import fits
 from dkist_header_validator import spec122_validator
 from dkist_processing_common._util.scratch import WorkflowFileSystem
+from dkist_processing_common.codecs.fits import fits_hdulist_encoder
 from dkist_processing_common.tests.conftest import FakeGQLClient
 from logging42 import logger
 
 from dkist_processing_cryonirsp.models.tags import CryonirspTag
 from dkist_processing_cryonirsp.tasks.bad_pixel_map import BadPixelMapCalibration
 from dkist_processing_cryonirsp.tests.conftest import cryonirsp_testing_parameters_factory
 from dkist_processing_cryonirsp.tests.conftest import CryonirspConstantsDb
@@ -73,21 +74,22 @@
             bad_pixel_locs = rng.choice(nelem, size=num_bad_pixels, replace=False)
             hot_pixel_locs = sorted(bad_pixel_locs[:num_hot_pixels])
             zero_pixel_locs = sorted(bad_pixel_locs[num_hot_pixels:])
             array[zero_pixel_locs] = 0.0
             array[hot_pixel_locs] = 2000.0
             array = array.reshape(array_shape[1:])
             hdul[0].data = array
-            task.fits_data_write(
-                hdu_list=hdul,
+            task.write(
+                data=hdul,
                 tags=[
                     CryonirspTag.linearized(),
                     CryonirspTag.task_solar_gain(),
                     CryonirspTag.frame(),
                 ],
+                encoder=fits_hdulist_encoder,
             )
             yield task, num_zero_pixels, num_hot_pixels
         finally:
             task._purge()
 
 
 def test_compute_bad_pixel_map_task(compute_bad_pixel_map_task, mocker):
```

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tests/test_build_quality_report.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tests/test_build_quality_report.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tests/test_ci_beam_boundaries.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tests/test_ci_beam_boundaries.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from datetime import datetime
 
 import numpy as np
 import pytest
 from astropy.io import fits
 from dkist_header_validator import spec122_validator
 from dkist_processing_common._util.scratch import WorkflowFileSystem
+from dkist_processing_common.codecs.fits import fits_hdulist_encoder
 from dkist_processing_common.tests.conftest import FakeGQLClient
 
 from dkist_processing_cryonirsp.models.tags import CryonirspTag
 from dkist_processing_cryonirsp.tasks.ci_beam_boundaries import CIBeamBoundariesCalibration
 from dkist_processing_cryonirsp.tests.conftest import cryonirsp_testing_parameters_factory
 from dkist_processing_cryonirsp.tests.conftest import CryonirspConstantsDb
 from dkist_processing_cryonirsp.tests.conftest import CryonirspHeadersValidSPSolarGainFrames
@@ -67,21 +68,22 @@
             array[:, 7:-5, 3:-8] = 1000.0
             # Put some large vertical streaks in the image to help the shift measurement converge
             minus_streak_pos = array_shape[2] // 4
             plus_streak_pos = 3 * array_shape[2] // 4
             array[:, :, minus_streak_pos - 5 : minus_streak_pos + 5] += 100
             array[:, :, plus_streak_pos - 5 : plus_streak_pos + 5] += 100
             hdul[0].data = array
-            task.fits_data_write(
-                hdu_list=hdul,
+            task.write(
+                data=hdul,
                 tags=[
                     CryonirspTag.linearized(),
                     CryonirspTag.task_solar_gain(),
                     CryonirspTag.frame(),
                 ],
+                encoder=fits_hdulist_encoder,
             )
             yield task, arm_id
         finally:
             task._purge()
 
 
 def test_compute_beam_boundaries_task(compute_beam_boundaries_task, mocker):
```

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tests/test_ci_make_movie_frames.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tests/test_ci_make_movie_frames.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from datetime import datetime
 
 import pytest
 from astropy.io import fits
 from dkist_header_validator import spec122_validator
 from dkist_processing_common._util.scratch import WorkflowFileSystem
+from dkist_processing_common.codecs.fits import fits_hdulist_encoder
 from dkist_processing_common.tests.conftest import FakeGQLClient
 
 from dkist_processing_cryonirsp.models.tags import CryonirspTag
 from dkist_processing_cryonirsp.tasks.make_movie_frames import CIMakeCryonirspMovieFrames
 from dkist_processing_cryonirsp.tests.conftest import CryonirspConstantsDb
 from dkist_processing_cryonirsp.tests.conftest import CryonirspHeadersValidObserveFrames
 from dkist_processing_cryonirsp.tests.conftest import generate_fits_frame
@@ -56,24 +57,25 @@
                                 d.header(), return_type=fits.HDUList
                             )[0].header
                             for d in ds
                         )
                         hdul = generate_fits_frame(
                             header_generator=header_generator, shape=(1, 3, 3)
                         )
-                        task.fits_data_write(
-                            hdu_list=hdul,
+                        task.write(
+                            data=hdul,
                             tags=[
                                 CryonirspTag.output(),
                                 CryonirspTag.frame(),
                                 CryonirspTag.map_scan(map_scan),
                                 CryonirspTag.scan_step(scan_step),
                                 CryonirspTag.stokes(stokes_state),
                                 CryonirspTag.meas_num(meas_num),
                             ],
+                            encoder=fits_hdulist_encoder,
                         )
             yield task, map_scans, scan_steps
         finally:
             task._purge()
 
 
 def test_ci_make_movie_frames(ci_movie_frames_task, mocker):
```

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tests/test_ci_science.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tests/test_sp_science.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,200 +1,234 @@
 import json
 import random
+from dataclasses import dataclass
 from datetime import datetime
 
 import numpy as np
 import pytest
 from astropy.io import fits
 from astropy.time import Time
 from astropy.time import TimeDelta
 from dkist_header_validator import spec122_validator
 from dkist_processing_common._util.scratch import WorkflowFileSystem
+from dkist_processing_common.codecs.fits import fits_hdulist_encoder
 from dkist_processing_common.tests.conftest import FakeGQLClient
 
 from dkist_processing_cryonirsp.models.tags import CryonirspStemName
 from dkist_processing_cryonirsp.models.tags import CryonirspTag
-from dkist_processing_cryonirsp.tasks.ci_science import CIScienceCalibration
+from dkist_processing_cryonirsp.tasks.sp_science import CalibrationCollection
+from dkist_processing_cryonirsp.tasks.sp_science import SPScienceCalibration
 from dkist_processing_cryonirsp.tests.conftest import cryonirsp_testing_parameters_factory
 from dkist_processing_cryonirsp.tests.conftest import CryonirspConstantsDb
 from dkist_processing_cryonirsp.tests.conftest import CryonirspHeadersValidObserveFrames
 from dkist_processing_cryonirsp.tests.conftest import generate_fits_frame
 
 # from dkist_processing_common.models.tags import Tag
 
 
 @pytest.fixture(scope="function", params=["Full Stokes", "Stokes-I"])
-def ci_science_calibration_task(
+def sp_science_calibration_task(
     tmp_path,
     recipe_run_id,
     assign_input_dataset_doc_to_task,
     init_cryonirsp_constants_db,
     request,
 ):
     num_map_scans = 2
+    num_beams = 2
     num_scan_steps = 2
-    num_meas = 1
     exposure_time = 0.02  # From CryonirspHeadersValidObserveFrames fixture
     if request.param == "Full Stokes":
         num_modstates = 2
     else:
         num_modstates = 1
-    array_shape = (1, 20, 20)
-    intermediate_shape = array_shape[1:]
-    dataset_shape = (num_map_scans * num_scan_steps * num_modstates,) + array_shape[1:]
+    array_shape = (1, 30, 60)
+    intermediate_shape = (30, 30)
+    dataset_shape = (num_beams * num_map_scans * num_scan_steps * num_modstates,) + array_shape[1:]
 
     constants_db = CryonirspConstantsDb(
-        ARM_ID="CI",
         NUM_MODSTATES=num_modstates,
         NUM_MAP_SCANS=num_map_scans,
         NUM_SCAN_STEPS=num_scan_steps,
-        NUM_BEAMS=1,
+        NUM_BEAMS=num_beams,
         OBSERVE_EXPOSURE_TIMES=(exposure_time,),
         MODULATOR_SPIN_MODE="Continuous" if request.param == "Full Stokes" else "Off",
     )
     init_cryonirsp_constants_db(recipe_run_id, constants_db)
-    with CIScienceCalibration(
-        recipe_run_id=recipe_run_id, workflow_name="ci_science_calibration", workflow_version="VX.Y"
+    with SPScienceCalibration(
+        recipe_run_id=recipe_run_id, workflow_name="sp_science_calibration", workflow_version="VX.Y"
     ) as task:
         try:  # This try... block is here to make sure the dbs get cleaned up if there's a failure in the fixture
             all_zeros = np.zeros(intermediate_shape)
             all_ones = np.ones(intermediate_shape)
-
             task.scratch = WorkflowFileSystem(
                 scratch_base_path=tmp_path, recipe_run_id=recipe_run_id
             )
-
             param_class = cryonirsp_testing_parameters_factory(param_path=tmp_path)
             assign_input_dataset_doc_to_task(task, param_class())
-
-            # Need a beam boundary file
-            task.intermediate_frame_write_arrays(
-                arrays=np.array([0, intermediate_shape[0], 0, intermediate_shape[1]]),
-                task_tag=CryonirspTag.task_beam_boundaries(),
-                beam=1,
-            )
             # Create fake bad pixel map
             task.intermediate_frame_write_arrays(
-                arrays=np.zeros(array_shape[1:]), task_tag=CryonirspTag.task_bad_pixel_map()
+                arrays=np.zeros((1, 1)),
+                task_tag=CryonirspTag.task_bad_pixel_map(),
             )
-
             # Create fake demodulation matrices
             demod_matrices = np.zeros((1, 1, 4, num_modstates))
             for modstate in range(num_modstates):
                 demod_matrices[0, 0, :, modstate] = [1, 2, 3, 4]
-            demod_hdul = fits.HDUList([fits.PrimaryHDU(data=demod_matrices)])
-            task.fits_data_write(
-                hdu_list=demod_hdul,
-                tags=[
-                    CryonirspTag.intermediate(),
-                    CryonirspTag.frame(),
-                    CryonirspTag.task_demodulation_matrices(),
-                    CryonirspTag.beam(1),
-                ],
-            )
-
-            # Create fake dark intermediate arrays
-            task.intermediate_frame_write_arrays(
-                all_zeros, beam=1, task_tag=CryonirspTag.task_dark(), exposure_time=exposure_time
-            )
-
-            # Create fake lamp and solar gain intermediate arrays
-            for modstate in range(1, num_modstates + 1):
-                gain_hdul = fits.HDUList([fits.PrimaryHDU(data=all_ones)])
-                task.fits_data_write(
-                    hdu_list=gain_hdul,
+            for beam in range(num_beams):
+                demod_hdul = fits.HDUList([fits.PrimaryHDU(data=demod_matrices)])
+                task.write(
+                    data=demod_hdul,
                     tags=[
                         CryonirspTag.intermediate(),
                         CryonirspTag.frame(),
-                        CryonirspTag.task_lamp_gain(),
-                        CryonirspTag.beam(1),
-                        CryonirspTag.modstate(modstate),
+                        CryonirspTag.task_demodulation_matrices(),
+                        CryonirspTag.beam(beam + 1),
                     ],
+                    encoder=fits_hdulist_encoder,
                 )
-                task.fits_data_write(
-                    hdu_list=gain_hdul,
-                    tags=[
-                        CryonirspTag.intermediate(),
-                        CryonirspTag.frame(),
-                        CryonirspTag.task_solar_gain(),
-                        CryonirspTag.beam(1),
-                        CryonirspTag.modstate(modstate),
-                    ],
+
+            # Create fake geometric objects
+            angle = np.array([0.0])
+            offset = np.array([-10.2, 5.1])
+            spec_shift = np.zeros(intermediate_shape[0])
+            for beam in range(1, num_beams + 1):
+                task.intermediate_frame_write_arrays(
+                    arrays=angle, beam=beam, task_tag=CryonirspTag.task_geometric_angle()
                 )
+                task.intermediate_frame_write_arrays(
+                    arrays=spec_shift,
+                    beam=beam,
+                    task_tag=CryonirspTag.task_geometric_sepectral_shifts(),
+                )
+                for modstate in range(1, num_modstates + 1):
+                    task.intermediate_frame_write_arrays(
+                        arrays=offset
+                        * (beam - 1),  # Because we need the fiducial array to have (0, 0) offset
+                        beam=beam,
+                        modstate=modstate,
+                        task_tag=CryonirspTag.task_geometric_offset(),
+                    )
+
+            # Create fake dark intermediate arrays
+            for beam in range(1, num_beams + 1):
+                task.intermediate_frame_write_arrays(
+                    all_zeros,
+                    beam=beam,
+                    task_tag=CryonirspTag.task_dark(),
+                    exposure_time=exposure_time,
+                )
+
+            # And a beam border intermediate array
+            for beam in range(1, num_beams + 1):
+                task.intermediate_frame_write_arrays(
+                    arrays=np.array([0, 30, ((beam - 1) * 30), (30 + (beam - 1) * 30)]),
+                    task_tag=CryonirspTag.task_beam_boundaries(),
+                    beam=beam,
+                )
+
+            # Create fake lamp and solar gain intermediate arrays
+            for beam in range(1, num_beams + 1):
+                for modstate in range(1, num_modstates + 1):
+                    gain_hdul = fits.HDUList([fits.PrimaryHDU(data=all_ones)])
+                    task.write(
+                        data=gain_hdul,
+                        tags=[
+                            CryonirspTag.intermediate(),
+                            CryonirspTag.frame(),
+                            CryonirspTag.task_lamp_gain(),
+                            CryonirspTag.beam(beam),
+                            CryonirspTag.modstate(modstate),
+                        ],
+                        encoder=fits_hdulist_encoder,
+                    )
+
+                    task.write(
+                        data=gain_hdul,
+                        tags=[
+                            CryonirspTag.intermediate(),
+                            CryonirspTag.frame(),
+                            CryonirspTag.task_solar_gain(),
+                            CryonirspTag.beam(beam),
+                            CryonirspTag.modstate(modstate),
+                        ],
+                        encoder=fits_hdulist_encoder,
+                    )
 
             # Create fake observe arrays
             start_time = datetime.now()
             for map_scan in range(1, num_map_scans + 1):
                 for scan_step in range(1, num_scan_steps + 1):
                     for modstate in range(1, num_modstates + 1):
-                        for meas_num in range(1, num_meas + 1):
-                            ds = CryonirspHeadersValidObserveFrames(
-                                dataset_shape=dataset_shape,
-                                array_shape=array_shape,
-                                time_delta=10,
-                                scan_step=scan_step,
-                                num_scan_steps=num_scan_steps,
-                                num_map_scans=num_map_scans,
-                                map_scan=map_scan,
-                                num_modstates=num_modstates,
-                                modstate=modstate,
-                                start_time=start_time,
-                                num_meas=num_meas,
-                                meas_num=meas_num,
-                                arm_id="CI",
-                            )
-                            header_generator = (
-                                spec122_validator.validate_and_translate_to_214_l0(
-                                    d.header(), return_type=fits.HDUList
-                                )[0].header
-                                for d in ds
-                            )
-
-                            hdul = generate_fits_frame(
-                                header_generator=header_generator, shape=array_shape
-                            )
-                            header = hdul[0].header
-                            task.fits_data_write(
-                                hdu_list=hdul,
-                                tags=[
-                                    CryonirspTag.task_observe(),
-                                    CryonirspTag.scan_step(scan_step),
-                                    CryonirspTag.map_scan(map_scan),
-                                    CryonirspTag.modstate(modstate),
-                                    CryonirspTag.linearized(),
-                                    CryonirspTag.frame(),
-                                    CryonirspTag.exposure_time(exposure_time),
-                                    CryonirspTag.meas_num(meas_num),
-                                ],
-                            )
-            yield task, request.param, header, intermediate_shape
+                        ds = CryonirspHeadersValidObserveFrames(
+                            dataset_shape=dataset_shape,
+                            array_shape=array_shape,
+                            time_delta=10,
+                            scan_step=scan_step,
+                            num_scan_steps=num_scan_steps,
+                            num_map_scans=num_map_scans,
+                            map_scan=map_scan,
+                            num_modstates=num_modstates,
+                            modstate=modstate,
+                            start_time=start_time,
+                            num_meas=1,
+                            meas_num=1,
+                            arm_id="SP",
+                        )
+                        header_generator = (
+                            spec122_validator.validate_and_translate_to_214_l0(
+                                d.header(), return_type=fits.HDUList
+                            )[0].header
+                            for d in ds
+                        )
+
+                        hdul = generate_fits_frame(
+                            header_generator=header_generator, shape=array_shape
+                        )
+                        header = hdul[0].header
+                        task.write(
+                            data=hdul,
+                            tags=[
+                                CryonirspTag.task_observe(),
+                                CryonirspTag.meas_num(1),
+                                CryonirspTag.scan_step(scan_step),
+                                CryonirspTag.map_scan(map_scan),
+                                CryonirspTag.modstate(modstate),
+                                CryonirspTag.linearized(),
+                                CryonirspTag.frame(),
+                                CryonirspTag.exposure_time(exposure_time),
+                            ],
+                            encoder=fits_hdulist_encoder,
+                        )
+
+            yield task, request.param, offset, header, intermediate_shape
         finally:
             task._purge()
 
 
 @pytest.fixture(scope="session")
-def ci_headers_with_dates() -> tuple[list[fits.Header], str, int, int]:
+def sp_headers_with_dates() -> tuple[list[fits.Header], str, int, int]:
     num_headers = 5
     start_time = "1969-12-06T18:00:00"
     exp_time = 12
     time_delta = 10
     ds = CryonirspHeadersValidObserveFrames(
         dataset_shape=(num_headers, 4, 4),
         array_shape=(1, 4, 4),
         time_delta=time_delta,
         num_map_scans=1,
         map_scan=1,
         num_scan_steps=1,
         scan_step=1,
-        num_meas=1,
-        meas_num=1,
         num_modstates=num_headers,
         modstate=1,
         start_time=datetime.fromisoformat(start_time),
-        arm_id="CI",
+        num_meas=1,
+        meas_num=1,
+        arm_id="SP",
     )
     headers = [
         spec122_validator.validate_and_translate_to_214_l0(d.header(), return_type=fits.HDUList)[
             0
         ].header
         for d in ds
     ]
@@ -202,51 +236,70 @@
     for h in headers:
         h["XPOSURE"] = exp_time  # Exposure time, in ms
 
     return headers, start_time, exp_time, time_delta
 
 
 @pytest.fixture(scope="session")
-def ci_compressed_headers_with_dates(
-    ci_headers_with_dates,
+def sp_compressed_headers_with_dates(
+    sp_headers_with_dates,
 ) -> tuple[list[fits.Header], str, int, int]:
-    headers, start_time, exp_time, time_delta = ci_headers_with_dates
+    headers, start_time, exp_time, time_delta = sp_headers_with_dates
     comp_headers = [fits.hdu.compressed.CompImageHeader(h, h) for h in headers]
     return comp_headers, start_time, exp_time, time_delta
 
 
-def test_ci_science_calibration_task(ci_science_calibration_task, mocker):
+@pytest.fixture(scope="function")
+def sp_calibration_collection_with_geo_shifts(shifts) -> CalibrationCollection:
+    num_beams, num_mod, _ = shifts.shape
+    geo_shifts = {
+        str(b + 1): {f"m{m + 1}": shifts[b, m, :] for m in range(num_mod)} for b in range(num_beams)
+    }
+    return CalibrationCollection(
+        dark=dict(),
+        angle=dict(),
+        state_offset=geo_shifts,
+        spec_shift=dict(),
+        demod_matrices=None,
+    )
+
+
+def test_sp_science_calibration_task(sp_science_calibration_task, mocker):
     """
-    Given: A CIScienceCalibration task
+    Given: A SPScienceCalibration task
     When: Calling the task instance
     Then: There are the expected number of science frames with the correct tags applied and the headers have been correctly updated
     """
 
     mocker.patch(
         "dkist_processing_common.tasks.mixin.metadata_store.GraphQLClient", new=FakeGQLClient
     )
 
     # When
-    task, polarization_mode, og_header, og_single_beam_shape = ci_science_calibration_task
+    task, polarization_mode, offset, og_header, og_single_beam_shape = sp_science_calibration_task
     task()
 
     # 1 from re-dummification
-    expected_final_shape = (1, og_single_beam_shape[0], og_single_beam_shape[1])
+    expected_final_shape = (
+        1,
+        og_single_beam_shape[0],
+        og_single_beam_shape[1],
+    )
 
     # Then
     tags = [
         CryonirspTag.calibrated(),
         CryonirspTag.frame(),
     ]
     files = list(task.read(tags=tags))
     if polarization_mode == "Full Stokes":
-        # 2 scan steps * 2 map scans * 4 stokes params = 16 frames
+        # 2 raster steps * 2 map scans * 4 stokes params = 16 frames
         assert len(files) == 16
     elif polarization_mode == "Stokes-I":
-        # 2 scan steps * 2 map scans * 1 stokes param = 4 frames
+        # 2 raster steps * 2 map scans * 1 stokes param = 4 frames
         assert len(files) == 4
     for file in files:
         hdul = fits.open(file)
         assert len(hdul) == 1
         hdu = hdul[0]
         assert type(hdul[0]) is fits.PrimaryHDU
         assert hdu.data.shape == expected_final_shape
@@ -257,34 +310,40 @@
         scan_step = [
             int(t.split("_")[-1]) for t in task.tags(file) if CryonirspStemName.scan_step.value in t
         ][0]
 
         assert hdu.header["CNNUMSCN"] == 2
         assert hdu.header["CNCURSCN"] == scan_step
 
+        # Check that WCS keys were updated
+        if offset[0] > 0:
+            assert hdu.header["CRPIX2"] == og_header["CRPIX2"]
+        if offset[1] > 0:
+            assert hdu.header["CRPIX1"] == og_header["CRPIX1"]
+
     quality_files = task.read(tags=[CryonirspTag.quality("TASK_TYPES")])
     for file in quality_files:
         with file.open() as f:
             data = json.load(f)
             assert isinstance(data, dict)
             assert data["total_frames"] == task.scratch.count_all(
                 tags=[CryonirspTag.linearized(), CryonirspTag.frame(), CryonirspTag.task_observe()]
             )
 
 
-def test_compute_ci_date_keys(ci_headers_with_dates, recipe_run_id, init_cryonirsp_constants_db):
+def test_compute_sp_date_keys(sp_headers_with_dates, recipe_run_id, init_cryonirsp_constants_db):
     """
-    Given: A set of CI headers with different DATE-OBS values
+    Given: A set of SP headers with different DATE-OBS values
     When: Computing the time over which the headers were taken
     Then: A header with correct DATE-BEG, DATE-END, and DATE-AVG keys is returned
     """
-    headers, start_time, exp_time, time_delta = ci_headers_with_dates
+    headers, start_time, exp_time, time_delta = sp_headers_with_dates
     constants_db = CryonirspConstantsDb()
     init_cryonirsp_constants_db(recipe_run_id, constants_db)
-    with CIScienceCalibration(
+    with SPScienceCalibration(
         recipe_run_id=recipe_run_id, workflow_name="science_calibration", workflow_version="VX.Y"
     ) as task:
         final_header = task._compute_date_keys(headers)
         final_header_from_single = task._compute_date_keys(headers[0])
 
     date_end = (
         Time(start_time)
@@ -301,26 +360,26 @@
         + TimeDelta(exp_time / 1000.0, format="sec")
     ).isot
 
     assert final_header_from_single["DATE-BEG"] == headers[0]["DATE-BEG"]
     assert final_header_from_single["DATE-END"] == date_end_from_single
 
 
-def test_compute_ci_date_keys_compressed_headers(
-    ci_compressed_headers_with_dates, recipe_run_id, init_cryonirsp_constants_db
+def test_compute_sp_date_keys_compressed_headers(
+    sp_compressed_headers_with_dates, recipe_run_id, init_cryonirsp_constants_db
 ):
     """
-    Given: A set of CI compressed headers with different DATE-OBS values
+    Given: A set of SP compressed headers with different DATE-OBS values
     When: Computing the time over which the headers were taken
     Then: A header with correct DATE-BEG, DATE-END, and DATE-AVG keys is returned
     """
-    headers, start_time, exp_time, time_delta = ci_compressed_headers_with_dates
+    headers, start_time, exp_time, time_delta = sp_compressed_headers_with_dates
     constants_db = CryonirspConstantsDb()
     init_cryonirsp_constants_db(recipe_run_id, constants_db)
-    with CIScienceCalibration(
+    with SPScienceCalibration(
         recipe_run_id=recipe_run_id, workflow_name="science_calibration", workflow_version="VX.Y"
     ) as task:
         final_header = task._compute_date_keys(headers)
         final_header_from_single = task._compute_date_keys(headers[0])
 
     date_end = (
         Time(start_time)
```

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tests/test_cryo_base.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tests/test_cryo_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import numpy as np
 import pytest
 from astropy.io import fits
 from dkist_processing_common._util.scratch import WorkflowFileSystem
+from dkist_processing_common.codecs.fits import fits_hdu_decoder
 
 from dkist_processing_cryonirsp.models.tags import CryonirspTag
 from dkist_processing_cryonirsp.models.task_name import CryonirspTaskName
 from dkist_processing_cryonirsp.tasks.cryonirsp_base import CryonirspTaskBase
 from dkist_processing_cryonirsp.tasks.mixin.intermediate_frame import (
     IntermediateFrameMixin,
 )
@@ -59,23 +60,24 @@
     data = np.random.random((10, 10))
     head = fits.Header()
     head["TEST"] = "foo"
     cryo_science_task.intermediate_frame_write_arrays(
         arrays=data, headers=head, beam=1, map_scan=2, scan_step=3, task="BAR"
     )
     loaded_list = list(
-        cryo_science_task.fits_data_read_hdu(
+        cryo_science_task.read(
             tags=[
                 CryonirspTag.intermediate(),
                 CryonirspTag.frame(),
                 CryonirspTag.beam(1),
                 CryonirspTag.map_scan(2),
                 CryonirspTag.scan_step(3),
                 CryonirspTag.task("BAR"),
-            ]
+            ],
+            decoder=fits_hdu_decoder,
         )
     )
     assert len(loaded_list) == 1
     hdu = loaded_list[0]
     np.testing.assert_equal(hdu.data, data)
     assert hdu.header["TEST"] == "foo"
 
@@ -91,15 +93,18 @@
     head["TEST"] = "foo"
 
     # bad_pixel_map chosen for no particular reason
     cryo_science_task.intermediate_frame_write_arrays(
         arrays=data, headers=head, task_tag=CryonirspTag.task_bad_pixel_map()
     )
     loaded_list = list(
-        cryo_science_task.fits_data_read_hdu(tags=[CryonirspTag.task_bad_pixel_map()])
+        cryo_science_task.read(
+            tags=[CryonirspTag.task_bad_pixel_map()],
+            decoder=fits_hdu_decoder,
+        )
     )
     assert len(loaded_list) == 1
     hdu = loaded_list[0]
     np.testing.assert_equal(hdu.data, data)
     assert hdu.header["TEST"] == "foo"
 
 
@@ -129,23 +134,24 @@
     Then: The array is written and tagged correctly
     """
     data = np.random.random((10, 10))
     cryo_science_task.intermediate_frame_write_arrays(
         arrays=data, headers=None, beam=1, map_scan=2, scan_step=3, task="BAR"
     )
     loaded_list = list(
-        cryo_science_task.fits_data_read_hdu(
+        cryo_science_task.read(
             tags=[
                 CryonirspTag.intermediate(),
                 CryonirspTag.frame(),
                 CryonirspTag.beam(1),
                 CryonirspTag.map_scan(2),
                 CryonirspTag.scan_step(3),
                 CryonirspTag.task("BAR"),
-            ]
+            ],
+            decoder=fits_hdu_decoder,
         )
     )
     assert len(loaded_list) == 1
     hdu = loaded_list[0]
     np.testing.assert_equal(hdu.data, data)
```

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tests/test_cryo_constants.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tests/test_cryo_constants.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tests/test_dark.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tests/test_dark.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import json
 
 import numpy as np
 import pytest
 from astropy.io import fits
 from dkist_header_validator import spec122_validator
 from dkist_processing_common._util.scratch import WorkflowFileSystem
+from dkist_processing_common.codecs.fits import fits_hdulist_encoder
 from dkist_processing_common.tests.conftest import FakeGQLClient
 
 from dkist_processing_cryonirsp.models.tags import CryonirspTag
 from dkist_processing_cryonirsp.tasks.dark import DarkCalibration
 from dkist_processing_cryonirsp.tests.conftest import cryonirsp_testing_parameters_factory
 from dkist_processing_cryonirsp.tests.conftest import CryonirspConstantsDb
 from dkist_processing_cryonirsp.tests.conftest import CryonirspHeadersValidDarkFrames
@@ -75,22 +76,23 @@
                     # data are 1s to start...
                     hdul[0].data.fill(e)
                     # Create combined 2-beam array
                     # beam = 1
                     # hdul[0].data[0, :beam_border, :] = beam * e
                     # beam = 2
                     # hdul[0].data[0, beam_border:, :] = beam * e
-                    task.fits_data_write(
-                        hdu_list=hdul,
+                    task.write(
+                        data=hdul,
                         tags=[
                             CryonirspTag.linearized(),
                             CryonirspTag.frame(),
                             CryonirspTag.task_dark(),
                             CryonirspTag.exposure_time(e),
                         ],
+                        encoder=fits_hdulist_encoder,
                     )
             yield task, num_beams, exp_times, unused_time, beam_boundary_spacing
         finally:
             task._purge()
 
 
 @pytest.fixture(scope="function")
@@ -139,22 +141,23 @@
                 for d in ds
             )
             for e in exp_times + [unused_time]:  # Make some darks we won't use
                 for _ in range(num_frames_per):
                     hdul = generate_fits_frame(header_generator=header_generator, shape=array_shape)
                     # data are 1s to start...
                     hdul[0].data.fill(e)
-                    task.fits_data_write(
-                        hdu_list=hdul,
+                    task.write(
+                        data=hdul,
                         tags=[
                             CryonirspTag.linearized(),
                             CryonirspTag.frame(),
                             CryonirspTag.task_dark(),
                             CryonirspTag.exposure_time(e),
                         ],
+                        encoder=fits_hdulist_encoder,
                     )
             yield task, exp_times, unused_time
         finally:
             task._purge()
 
 
 def test_sp_dark_calibration_task(sp_dark_calibration_task, mocker):
```

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tests/test_gain.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tests/test_gain.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from datetime import datetime
 
 import numpy as np
 import pytest
 from astropy.io import fits
 from dkist_header_validator import spec122_validator
 from dkist_processing_common._util.scratch import WorkflowFileSystem
+from dkist_processing_common.codecs.fits import fits_hdulist_encoder
 from dkist_processing_common.tests.conftest import FakeGQLClient
 
 from dkist_processing_cryonirsp.models.tags import CryonirspTag
 from dkist_processing_cryonirsp.models.task_name import TaskName
 from dkist_processing_cryonirsp.tasks.gain import CISolarGainCalibration
 from dkist_processing_cryonirsp.tasks.gain import LampGainCalibration
 from dkist_processing_cryonirsp.tests.conftest import cryonirsp_testing_parameters_factory
@@ -94,15 +95,19 @@
             tags = [
                 CryonirspTag.linearized(),
                 CryonirspTag.task(request.param),
                 CryonirspTag.modstate(1),
                 CryonirspTag.frame(),
                 CryonirspTag.exposure_time(exposure_time),
             ]
-            task.fits_data_write(hdu_list=hdul, tags=tags)
+            task.write(
+                data=hdul,
+                tags=tags,
+                encoder=fits_hdulist_encoder,
+            )
             yield task, number_of_beams, gain_type, exposure_time
         finally:
             task._purge()
 
 
 @pytest.fixture(scope="function")
 def sp_lamp_calibration_task(
@@ -177,15 +182,19 @@
                     CryonirspTag.beam(b + 1),
                     CryonirspTag.linearized(),
                     CryonirspTag.task(gain_type),
                     CryonirspTag.modstate(1),
                     CryonirspTag.frame(),
                     CryonirspTag.exposure_time(exposure_time),
                 ]
-                task.fits_data_write(hdu_list=hdul, tags=tags)
+                task.write(
+                    data=hdul,
+                    tags=tags,
+                    encoder=fits_hdulist_encoder,
+                )
             yield task, number_of_beams
         finally:
             task._purge()
 
 
 def test_ci_gain_calibration_task(ci_gain_calibration_task, mocker):
     """
```

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tests/test_instrument_polarization.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tests/test_instrument_polarization.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from unittest.mock import patch
 
 import numpy as np
 import pytest
 from astropy.io import fits
 from dkist_header_validator import spec122_validator
 from dkist_processing_common._util.scratch import WorkflowFileSystem
+from dkist_processing_common.codecs.fits import fits_hdulist_encoder
 from dkist_processing_common.tests.conftest import FakeGQLClient
 from dkist_processing_pac.fitter.polcal_fitter import PolcalFitter
 from dkist_processing_pac.input_data.dresser import Dresser
 
 from dkist_processing_cryonirsp.models.tags import CryonirspTag
 from dkist_processing_cryonirsp.models.task_name import CryonirspTaskName
 from dkist_processing_cryonirsp.models.task_name import TaskName
@@ -73,25 +74,26 @@
             0
         ].header
         for d in ds
     )
     hdul = generate_fits_frame(header_generator=header_generator, shape=array_shape)
     cs_step = 1 if polcal_type == CryonirspTaskName.polcal_gain.value else 0
     for m in range(1, num_mod + 1):
-        task.fits_data_write(
-            hdu_list=hdul,
+        task.write(
+            data=hdul,
             tags=[
                 CryonirspTag.task(polcal_type),
                 CryonirspTag.task_polcal(),
                 CryonirspTag.modstate(m),
                 CryonirspTag.cs_step(cs_step),
                 CryonirspTag.linearized(),
                 CryonirspTag.frame(),
                 CryonirspTag.exposure_time(exposure_time),
             ],
+            encoder=fits_hdulist_encoder,
         )
 
 
 def _create_polcal_arrays(
     task,
     dataset_shape,
     array_shape,
@@ -116,24 +118,25 @@
             )[0].header
             for d in ds
         )
         # cs_step does not map to a single keyword, so not needed in the fake headers
         # We start at 2 because dark and gain are 0 and 1
         for cs_step in range(2, num_cs_steps):
             hdul = generate_fits_frame(header_generator=header_generator, shape=array_shape)
-            task.fits_data_write(
-                hdu_list=hdul,
+            task.write(
+                data=hdul,
                 tags=[
                     CryonirspTag.task_polcal(),
                     CryonirspTag.modstate(modstate),
                     CryonirspTag.cs_step(cs_step),
                     CryonirspTag.linearized(),
                     CryonirspTag.frame(),
                     CryonirspTag.exposure_time(exposure_time),
                 ],
+                encoder=fits_hdulist_encoder,
             )
 
 
 @pytest.fixture(scope="function")
 def ci_instrument_polarization_calibration_task(
     tmp_path,
     recipe_run_id,
```

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tests/test_linearity_correction.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tests/test_linearity_correction.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from datetime import datetime
 
 import numpy as np
 import pytest
 from astropy.io import fits
 from dkist_header_validator import spec122_validator
 from dkist_processing_common._util.scratch import WorkflowFileSystem
+from dkist_processing_common.codecs.fits import fits_hdulist_encoder
 from dkist_processing_common.tests.conftest import FakeGQLClient
 
 from dkist_processing_cryonirsp.models.constants import CryonirspBudName
 from dkist_processing_cryonirsp.models.tags import CryonirspTag
 from dkist_processing_cryonirsp.tasks.linearity_correction import LinearityCorrection
 from dkist_processing_cryonirsp.tests.conftest import cryonirsp_testing_parameters_factory
 from dkist_processing_cryonirsp.tests.conftest import CryonirspConstantsDb
@@ -89,23 +90,24 @@
                 hdul = generate_fits_frame(header_generator=header_generator, shape=array_shape)
                 # Now tweak the data...
                 for hdu in hdul:
                     header = hdu.header
                     exp_time = header["XPOSURE"]
                     # Create a simple perfectly linear ramp
                     hdu.data.fill(exp_time)
-                    task.fits_data_write(
-                        hdu_list=hdul,
+                    task.write(
+                        data=hdul,
                         tags=[
                             CryonirspTag.input(),
                             CryonirspTag.frame(),
                             CryonirspTag.curr_frame_in_ramp(header["CNCNDR"]),
                             # All frames in a ramp have the same date-obs
                             CryonirspTag.time_obs(str(start_time)),
                         ],
+                        encoder=fits_hdulist_encoder,
                     )
             task.constants._update({CryonirspBudName.camera_readout_mode.value: "FastUpTheRamp"})
             yield task
         finally:
             task._purge()
```

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tests/test_parameters.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tests/test_parse.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tests/test_parse.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from itertools import chain
 
 import numpy as np
 import pytest
 from astropy.io import fits
 from dkist_header_validator.translator import translate_spec122_to_spec214_l0
 from dkist_processing_common._util.scratch import WorkflowFileSystem
+from dkist_processing_common.codecs.fits import fits_hdulist_encoder
 from dkist_processing_common.tests.conftest import FakeGQLClient
 
 from dkist_processing_cryonirsp.models.constants import CryonirspBudName
 from dkist_processing_cryonirsp.models.tags import CryonirspTag
 from dkist_processing_cryonirsp.tasks.parse import ParseL0CryonirspLinearizedData
 from dkist_processing_cryonirsp.tasks.parse import ParseL0CryonirspRampData
 from dkist_processing_cryonirsp.tests.conftest import cryonirsp_testing_parameters_factory
@@ -65,23 +66,24 @@
                 # Set the frame in ramp
                 translated_header["CNCNDR"] = counter + 1
                 counter += 1
                 hdu = fits.PrimaryHDU(
                     data=np.ones((1, 2, 2)), header=fits.Header(translated_header)
                 )
                 hdul = fits.HDUList([hdu])
-                task.fits_data_write(
-                    hdu_list=hdul,
+                task.write(
+                    data=hdul,
                     tags=[
                         CryonirspTag.input(),
                         CryonirspTag.frame(),
                         CryonirspTag.curr_frame_in_ramp(translated_header["CNCNDR"]),
                         # All frames in a ramp have the same date-obs
                         CryonirspTag.time_obs(str(start_time)),
                     ],
+                    encoder=fits_hdulist_encoder,
                 )
             yield task
         finally:
             task._purge()
 
 
 @pytest.fixture(scope="function", params=["CI", "SP"])
@@ -133,16 +135,18 @@
             for d in ds:
                 header = d.header()
                 translated_header = translate_spec122_to_spec214_l0(header)
                 hdu = fits.PrimaryHDU(
                     data=np.ones((1, 2, 2)), header=fits.Header(translated_header)
                 )
                 hdul = fits.HDUList([hdu])
-                task.fits_data_write(
-                    hdu_list=hdul, tags=[CryonirspTag.linearized(), CryonirspTag.frame()]
+                task.write(
+                    data=hdul,
+                    tags=[CryonirspTag.linearized(), CryonirspTag.frame()],
+                    encoder=fits_hdulist_encoder,
                 )
 
             start_time = datetime.now()
             time_delta = timedelta(seconds=10)
             i = 0
             for map_scan in range(1, num_maps + 1):
                 for m in range(1, num_modstates + 1):
@@ -165,16 +169,18 @@
                         header = next(ds).header()
                         header["CAM__004"] = [0.02, 0.03][m % 2]
                         translated_header = translate_spec122_to_spec214_l0(header)
                         hdu = fits.PrimaryHDU(
                             data=np.ones((1, 2, 2)), header=fits.Header(translated_header)
                         )
                         hdul = fits.HDUList([hdu])
-                        task.fits_data_write(
-                            hdu_list=hdul, tags=[CryonirspTag.linearized(), CryonirspTag.frame()]
+                        task.write(
+                            data=hdul,
+                            tags=[CryonirspTag.linearized(), CryonirspTag.frame()],
+                            encoder=fits_hdulist_encoder,
                         )
                         i += 1
             yield task
         finally:
             task._purge()
 
 
@@ -217,16 +223,18 @@
                         header = next(ds).header()
                         translated_header = translate_spec122_to_spec214_l0(header)
                         translated_header["CNNUMSCN"] = s % 3
                         hdu = fits.PrimaryHDU(
                             data=np.ones((1, 2, 2)), header=fits.Header(translated_header)
                         )
                         hdul = fits.HDUList([hdu])
-                        task.fits_data_write(
-                            hdu_list=hdul, tags=[CryonirspTag.linearized(), CryonirspTag.frame()]
+                        task.write(
+                            data=hdul,
+                            tags=[CryonirspTag.linearized(), CryonirspTag.frame()],
+                            encoder=fits_hdulist_encoder,
                         )
             yield task
         finally:
             task._purge()
 
 
 @pytest.fixture(scope="function", params=["CI", "SP"])
@@ -271,17 +279,18 @@
                             )
                             header = next(ds).header()
                             translated_header = translate_spec122_to_spec214_l0(header)
                             hdu = fits.PrimaryHDU(
                                 data=np.ones((1, 2, 2)), header=fits.Header(translated_header)
                             )
                             hdul = fits.HDUList([hdu])
-                            task.fits_data_write(
-                                hdu_list=hdul,
+                            task.write(
+                                data=hdul,
                                 tags=[CryonirspTag.linearized(), CryonirspTag.frame()],
+                                encoder=fits_hdulist_encoder,
                             )
             # Now do the incomplete map
             for map_scan in range(num_map_scans, num_map_scans + 1):
                 for m in range(1, num_modstates + 1):
                     for s in range(1, num_steps):  # One step is missing in the last map
                         for r in range(1, num_sub_repeats + 1):
                             ds = CryonirspHeadersValidObserveFrames(
@@ -302,17 +311,18 @@
                             )
                             header = next(ds).header()
                             translated_header = translate_spec122_to_spec214_l0(header)
                             hdu = fits.PrimaryHDU(
                                 data=np.ones((1, 2, 2)), header=fits.Header(translated_header)
                             )
                             hdul = fits.HDUList([hdu])
-                            task.fits_data_write(
-                                hdu_list=hdul,
+                            task.write(
+                                data=hdul,
                                 tags=[CryonirspTag.linearized(), CryonirspTag.frame()],
+                                encoder=fits_hdulist_encoder,
                             )
             yield task, num_steps, num_map_scans
         finally:
             task._purge()
 
 
 @pytest.fixture(scope="function", params=["CI", "SP"])
@@ -354,16 +364,18 @@
                         header = next(ds).header()
                         translated_header = translate_spec122_to_spec214_l0(header)
                         translated_header["CNNUMSCN"] = num_steps + 10
                         hdu = fits.PrimaryHDU(
                             data=np.ones((1, 2, 2)), header=fits.Header(translated_header)
                         )
                         hdul = fits.HDUList([hdu])
-                        task.fits_data_write(
-                            hdu_list=hdul, tags=[CryonirspTag.linearized(), CryonirspTag.frame()]
+                        task.write(
+                            data=hdul,
+                            tags=[CryonirspTag.linearized(), CryonirspTag.frame()],
+                            encoder=fits_hdulist_encoder,
                         )
             yield task, num_steps, num_maps
         finally:
             task._purge()
 
 
 @pytest.fixture(scope="function")
@@ -409,16 +421,18 @@
 
             for header in [dark_header, gain_header, data_header]:
                 translated_header = translate_spec122_to_spec214_l0(header)
                 hdu = fits.PrimaryHDU(
                     data=np.ones((1, 2, 2)), header=fits.Header(translated_header)
                 )
                 hdul = fits.HDUList([hdu])
-                task.fits_data_write(
-                    hdu_list=hdul, tags=[CryonirspTag.linearized(), CryonirspTag.frame()]
+                task.write(
+                    data=hdul,
+                    tags=[CryonirspTag.linearized(), CryonirspTag.frame()],
+                    encoder=fits_hdulist_encoder,
                 )
 
             yield task
         finally:
             task._purge()
```

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tests/test_quality.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tests/test_quality.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import json
 
 import pytest
 from astropy.io import fits
 from dkist_header_validator import spec122_validator
 from dkist_processing_common._util.scratch import WorkflowFileSystem
+from dkist_processing_common.codecs.fits import fits_hdulist_encoder
 from dkist_processing_common.tests.conftest import FakeGQLClient
 
 from dkist_processing_cryonirsp.models.tags import CryonirspTag
 from dkist_processing_cryonirsp.tasks.quality_metrics import CryonirspL1QualityMetrics
 from dkist_processing_cryonirsp.tests.conftest import Cryonirsp122ObserveFrames
 from dkist_processing_cryonirsp.tests.conftest import CryonirspConstantsDb
 from dkist_processing_cryonirsp.tests.conftest import generate_214_l1_fits_frame
@@ -41,24 +42,25 @@
                             d.header(), return_type=fits.HDUList
                         )[0].header
                         for d in ds
                     )
 
                     hdul = generate_214_l1_fits_frame(s122_header=next(header_generator))
                     hdul[1].header["DINDEX5"] = index
-                    task.fits_data_write(
-                        hdu_list=hdul,
+                    task.write(
+                        data=hdul,
                         tags=[
                             CryonirspTag.output(),
                             CryonirspTag.frame(),
                             CryonirspTag.stokes(stokes_param),
                             CryonirspTag.scan_step(scan_step),
                             CryonirspTag.map_scan(map_scan),
                             CryonirspTag.meas_num(1),
                         ],
+                        encoder=fits_hdulist_encoder,
                     )
 
         yield task
         task._purge()
 
 
 def test_quality_task(cryo_quality_task, mocker):
```

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tests/test_sp_beam_boundaries.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tests/test_sp_beam_boundaries.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from datetime import datetime
 
 import numpy as np
 import pytest
 from astropy.io import fits
 from dkist_header_validator import spec122_validator
 from dkist_processing_common._util.scratch import WorkflowFileSystem
+from dkist_processing_common.codecs.fits import fits_hdulist_encoder
 from dkist_processing_common.tests.conftest import FakeGQLClient
 
 from dkist_processing_cryonirsp.models.tags import CryonirspTag
 from dkist_processing_cryonirsp.tasks.sp_beam_boundaries import SPBeamBoundariesCalibration
 from dkist_processing_cryonirsp.tests.conftest import cryonirsp_testing_parameters_factory
 from dkist_processing_cryonirsp.tests.conftest import CryonirspConstantsDb
 from dkist_processing_cryonirsp.tests.conftest import CryonirspHeadersValidSPSolarGainFrames
@@ -65,21 +66,22 @@
             array[:, 7:-5, 3:-8] = 1000.0
             # Put some large vertical streaks in the image to help the shift measurement converge
             minus_streak_pos = array_shape[2] // 4
             plus_streak_pos = 3 * array_shape[2] // 4
             array[:, :, minus_streak_pos - 5 : minus_streak_pos + 5] += 100
             array[:, :, plus_streak_pos - 5 : plus_streak_pos + 5] += 100
             hdul[0].data = array
-            task.fits_data_write(
-                hdu_list=hdul,
+            task.write(
+                data=hdul,
                 tags=[
                     CryonirspTag.linearized(),
                     CryonirspTag.task_solar_gain(),
                     CryonirspTag.frame(),
                 ],
+                encoder=fits_hdulist_encoder,
             )
             yield task, arm_id
         finally:
             task._purge()
 
 
 def test_compute_beam_boundaries_task(compute_beam_boundaries_task, mocker):
```

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tests/test_sp_geometric.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tests/test_sp_geometric.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 
 import numpy as np
 import pytest
 from dkist_processing_common._util.scratch import WorkflowFileSystem
+from dkist_processing_common.codecs.fits import fits_hdulist_encoder
 from dkist_processing_common.tests.conftest import FakeGQLClient
 from dkist_processing_math import transform
 
 from dkist_processing_cryonirsp.models.tags import CryonirspTag
 from dkist_processing_cryonirsp.tasks.sp_geometric import SPGeometricCalibration
 from dkist_processing_cryonirsp.tests.conftest import cryonirsp_testing_parameters_factory
 from dkist_processing_cryonirsp.tests.conftest import CryonirspConstantsDb
@@ -95,23 +96,24 @@
                     transform.rotate_arrays_about_point(
                         arrays=translated, angle=task.angles[beam - 1]
                     )
                 )
                 raw_dark = np.concatenate((dark_cal, dark_cal), axis=1)
                 raw_solar = distorted_solar + raw_dark
                 solar_hdul = generate_214_l0_fits_frame(data=raw_solar, s122_header=header)
-                task.fits_data_write(
-                    hdu_list=solar_hdul,
+                task.write(
+                    data=solar_hdul,
                     tags=[
                         CryonirspTag.linearized(),
                         CryonirspTag.task_solar_gain(),
                         CryonirspTag.frame(),
                         CryonirspTag.beam(beam),
                         CryonirspTag.exposure_time(exposure_time),
                     ],
+                    encoder=fits_hdulist_encoder,
                 )
 
             yield task
         finally:
             task._purge()
 
 
@@ -188,22 +190,23 @@
         header = ds.header()
         true_solar = np.ones(data_shape_raw)
         # Now add the beam number to each beam in the array
         true_solar[:, 0:30] += beam1
         true_solar[:, 30:60] += beam2
         raw_solar = true_solar + dark_cal_two_beams
         solar_hdul = generate_214_l0_fits_frame(data=raw_solar, s122_header=header)
-        task.fits_data_write(
-            hdu_list=solar_hdul,
+        task.write(
+            data=solar_hdul,
             tags=[
                 CryonirspTag.linearized(),
                 CryonirspTag.task_solar_gain(),
                 CryonirspTag.frame(),
                 CryonirspTag.exposure_time(exposure_time),
             ],
+            encoder=fits_hdulist_encoder,
         )
 
         yield task
         task._purge()
 
 
 def test_geometric_task(geometric_calibration_task_that_completes, mocker):
```

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tests/test_sp_make_movie_frames.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tests/test_sp_make_movie_frames.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from datetime import datetime
 
 import pytest
 from astropy.io import fits
 from dkist_header_validator import spec122_validator
 from dkist_processing_common._util.scratch import WorkflowFileSystem
+from dkist_processing_common.codecs.fits import fits_hdulist_encoder
 from dkist_processing_common.tests.conftest import FakeGQLClient
 
 from dkist_processing_cryonirsp.models.tags import CryonirspTag
 from dkist_processing_cryonirsp.tasks.make_movie_frames import SPMakeCryonirspMovieFrames
 from dkist_processing_cryonirsp.tests.conftest import CryonirspConstantsDb
 from dkist_processing_cryonirsp.tests.conftest import CryonirspHeadersValidObserveFrames
 from dkist_processing_cryonirsp.tests.conftest import generate_fits_frame
@@ -56,24 +57,25 @@
                                 d.header(), return_type=fits.HDUList
                             )[0].header
                             for d in ds
                         )
                         hdul = generate_fits_frame(
                             header_generator=header_generator, shape=(1, 3, 3)
                         )
-                        task.fits_data_write(
-                            hdu_list=hdul,
+                        task.write(
+                            data=hdul,
                             tags=[
                                 CryonirspTag.output(),
                                 CryonirspTag.frame(),
                                 CryonirspTag.map_scan(map_scan),
                                 CryonirspTag.scan_step(scan_step),
                                 CryonirspTag.stokes(stokes_state),
                                 CryonirspTag.meas_num(meas_num),
                             ],
+                            encoder=fits_hdulist_encoder,
                         )
             yield task, map_scans, scan_steps
         finally:
             task._purge()
 
 
 def test_sp_make_movie_frames(sp_movie_frames_task, mocker):
```

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tests/test_sp_science.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tests/test_ci_science.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,229 +1,205 @@
 import json
 import random
-from dataclasses import dataclass
 from datetime import datetime
 
 import numpy as np
 import pytest
 from astropy.io import fits
 from astropy.time import Time
 from astropy.time import TimeDelta
 from dkist_header_validator import spec122_validator
 from dkist_processing_common._util.scratch import WorkflowFileSystem
+from dkist_processing_common.codecs.fits import fits_hdulist_encoder
 from dkist_processing_common.tests.conftest import FakeGQLClient
 
 from dkist_processing_cryonirsp.models.tags import CryonirspStemName
 from dkist_processing_cryonirsp.models.tags import CryonirspTag
-from dkist_processing_cryonirsp.tasks.sp_science import CalibrationCollection
-from dkist_processing_cryonirsp.tasks.sp_science import SPScienceCalibration
+from dkist_processing_cryonirsp.tasks.ci_science import CIScienceCalibration
 from dkist_processing_cryonirsp.tests.conftest import cryonirsp_testing_parameters_factory
 from dkist_processing_cryonirsp.tests.conftest import CryonirspConstantsDb
 from dkist_processing_cryonirsp.tests.conftest import CryonirspHeadersValidObserveFrames
 from dkist_processing_cryonirsp.tests.conftest import generate_fits_frame
 
 # from dkist_processing_common.models.tags import Tag
 
 
 @pytest.fixture(scope="function", params=["Full Stokes", "Stokes-I"])
-def sp_science_calibration_task(
+def ci_science_calibration_task(
     tmp_path,
     recipe_run_id,
     assign_input_dataset_doc_to_task,
     init_cryonirsp_constants_db,
     request,
 ):
     num_map_scans = 2
-    num_beams = 2
     num_scan_steps = 2
+    num_meas = 1
     exposure_time = 0.02  # From CryonirspHeadersValidObserveFrames fixture
     if request.param == "Full Stokes":
         num_modstates = 2
     else:
         num_modstates = 1
-    array_shape = (1, 30, 60)
-    intermediate_shape = (30, 30)
-    dataset_shape = (num_beams * num_map_scans * num_scan_steps * num_modstates,) + array_shape[1:]
+    array_shape = (1, 20, 20)
+    intermediate_shape = array_shape[1:]
+    dataset_shape = (num_map_scans * num_scan_steps * num_modstates,) + array_shape[1:]
 
     constants_db = CryonirspConstantsDb(
+        ARM_ID="CI",
         NUM_MODSTATES=num_modstates,
         NUM_MAP_SCANS=num_map_scans,
         NUM_SCAN_STEPS=num_scan_steps,
-        NUM_BEAMS=num_beams,
+        NUM_BEAMS=1,
         OBSERVE_EXPOSURE_TIMES=(exposure_time,),
         MODULATOR_SPIN_MODE="Continuous" if request.param == "Full Stokes" else "Off",
     )
     init_cryonirsp_constants_db(recipe_run_id, constants_db)
-    with SPScienceCalibration(
-        recipe_run_id=recipe_run_id, workflow_name="sp_science_calibration", workflow_version="VX.Y"
+    with CIScienceCalibration(
+        recipe_run_id=recipe_run_id, workflow_name="ci_science_calibration", workflow_version="VX.Y"
     ) as task:
         try:  # This try... block is here to make sure the dbs get cleaned up if there's a failure in the fixture
             all_zeros = np.zeros(intermediate_shape)
             all_ones = np.ones(intermediate_shape)
+
             task.scratch = WorkflowFileSystem(
                 scratch_base_path=tmp_path, recipe_run_id=recipe_run_id
             )
+
             param_class = cryonirsp_testing_parameters_factory(param_path=tmp_path)
             assign_input_dataset_doc_to_task(task, param_class())
+
+            # Need a beam boundary file
+            task.intermediate_frame_write_arrays(
+                arrays=np.array([0, intermediate_shape[0], 0, intermediate_shape[1]]),
+                task_tag=CryonirspTag.task_beam_boundaries(),
+                beam=1,
+            )
             # Create fake bad pixel map
             task.intermediate_frame_write_arrays(
-                arrays=np.zeros((1, 1)),
-                task_tag=CryonirspTag.task_bad_pixel_map(),
+                arrays=np.zeros(array_shape[1:]), task_tag=CryonirspTag.task_bad_pixel_map()
             )
+
             # Create fake demodulation matrices
             demod_matrices = np.zeros((1, 1, 4, num_modstates))
             for modstate in range(num_modstates):
                 demod_matrices[0, 0, :, modstate] = [1, 2, 3, 4]
-            for beam in range(num_beams):
-                demod_hdul = fits.HDUList([fits.PrimaryHDU(data=demod_matrices)])
-                task.fits_data_write(
-                    hdu_list=demod_hdul,
+            demod_hdul = fits.HDUList([fits.PrimaryHDU(data=demod_matrices)])
+            task.write(
+                data=demod_hdul,
+                tags=[
+                    CryonirspTag.intermediate(),
+                    CryonirspTag.frame(),
+                    CryonirspTag.task_demodulation_matrices(),
+                    CryonirspTag.beam(1),
+                ],
+                encoder=fits_hdulist_encoder,
+            )
+
+            # Create fake dark intermediate arrays
+            task.intermediate_frame_write_arrays(
+                all_zeros, beam=1, task_tag=CryonirspTag.task_dark(), exposure_time=exposure_time
+            )
+
+            # Create fake lamp and solar gain intermediate arrays
+            for modstate in range(1, num_modstates + 1):
+                gain_hdul = fits.HDUList([fits.PrimaryHDU(data=all_ones)])
+                task.write(
+                    data=gain_hdul,
                     tags=[
                         CryonirspTag.intermediate(),
                         CryonirspTag.frame(),
-                        CryonirspTag.task_demodulation_matrices(),
-                        CryonirspTag.beam(beam + 1),
+                        CryonirspTag.task_lamp_gain(),
+                        CryonirspTag.beam(1),
+                        CryonirspTag.modstate(modstate),
                     ],
+                    encoder=fits_hdulist_encoder,
                 )
-
-            # Create fake geometric objects
-            angle = np.array([0.0])
-            offset = np.array([-10.2, 5.1])
-            spec_shift = np.zeros(intermediate_shape[0])
-            for beam in range(1, num_beams + 1):
-                task.intermediate_frame_write_arrays(
-                    arrays=angle, beam=beam, task_tag=CryonirspTag.task_geometric_angle()
-                )
-                task.intermediate_frame_write_arrays(
-                    arrays=spec_shift,
-                    beam=beam,
-                    task_tag=CryonirspTag.task_geometric_sepectral_shifts(),
-                )
-                for modstate in range(1, num_modstates + 1):
-                    task.intermediate_frame_write_arrays(
-                        arrays=offset
-                        * (beam - 1),  # Because we need the fiducial array to have (0, 0) offset
-                        beam=beam,
-                        modstate=modstate,
-                        task_tag=CryonirspTag.task_geometric_offset(),
-                    )
-
-            # Create fake dark intermediate arrays
-            for beam in range(1, num_beams + 1):
-                task.intermediate_frame_write_arrays(
-                    all_zeros,
-                    beam=beam,
-                    task_tag=CryonirspTag.task_dark(),
-                    exposure_time=exposure_time,
-                )
-
-            # And a beam border intermediate array
-            for beam in range(1, num_beams + 1):
-                task.intermediate_frame_write_arrays(
-                    arrays=np.array([0, 30, ((beam - 1) * 30), (30 + (beam - 1) * 30)]),
-                    task_tag=CryonirspTag.task_beam_boundaries(),
-                    beam=beam,
+                task.write(
+                    data=gain_hdul,
+                    tags=[
+                        CryonirspTag.intermediate(),
+                        CryonirspTag.frame(),
+                        CryonirspTag.task_solar_gain(),
+                        CryonirspTag.beam(1),
+                        CryonirspTag.modstate(modstate),
+                    ],
+                    encoder=fits_hdulist_encoder,
                 )
 
-            # Create fake lamp and solar gain intermediate arrays
-            for beam in range(1, num_beams + 1):
-                for modstate in range(1, num_modstates + 1):
-                    gain_hdul = fits.HDUList([fits.PrimaryHDU(data=all_ones)])
-                    task.fits_data_write(
-                        hdu_list=gain_hdul,
-                        tags=[
-                            CryonirspTag.intermediate(),
-                            CryonirspTag.frame(),
-                            CryonirspTag.task_lamp_gain(),
-                            CryonirspTag.beam(beam),
-                            CryonirspTag.modstate(modstate),
-                        ],
-                    )
-
-                    task.fits_data_write(
-                        hdu_list=gain_hdul,
-                        tags=[
-                            CryonirspTag.intermediate(),
-                            CryonirspTag.frame(),
-                            CryonirspTag.task_solar_gain(),
-                            CryonirspTag.beam(beam),
-                            CryonirspTag.modstate(modstate),
-                        ],
-                    )
-
             # Create fake observe arrays
             start_time = datetime.now()
             for map_scan in range(1, num_map_scans + 1):
                 for scan_step in range(1, num_scan_steps + 1):
                     for modstate in range(1, num_modstates + 1):
-                        ds = CryonirspHeadersValidObserveFrames(
-                            dataset_shape=dataset_shape,
-                            array_shape=array_shape,
-                            time_delta=10,
-                            scan_step=scan_step,
-                            num_scan_steps=num_scan_steps,
-                            num_map_scans=num_map_scans,
-                            map_scan=map_scan,
-                            num_modstates=num_modstates,
-                            modstate=modstate,
-                            start_time=start_time,
-                            num_meas=1,
-                            meas_num=1,
-                            arm_id="SP",
-                        )
-                        header_generator = (
-                            spec122_validator.validate_and_translate_to_214_l0(
-                                d.header(), return_type=fits.HDUList
-                            )[0].header
-                            for d in ds
-                        )
-
-                        hdul = generate_fits_frame(
-                            header_generator=header_generator, shape=array_shape
-                        )
-                        header = hdul[0].header
-                        task.fits_data_write(
-                            hdu_list=hdul,
-                            tags=[
-                                CryonirspTag.task_observe(),
-                                CryonirspTag.meas_num(1),
-                                CryonirspTag.scan_step(scan_step),
-                                CryonirspTag.map_scan(map_scan),
-                                CryonirspTag.modstate(modstate),
-                                CryonirspTag.linearized(),
-                                CryonirspTag.frame(),
-                                CryonirspTag.exposure_time(exposure_time),
-                            ],
-                        )
-
-            yield task, request.param, offset, header, intermediate_shape
+                        for meas_num in range(1, num_meas + 1):
+                            ds = CryonirspHeadersValidObserveFrames(
+                                dataset_shape=dataset_shape,
+                                array_shape=array_shape,
+                                time_delta=10,
+                                scan_step=scan_step,
+                                num_scan_steps=num_scan_steps,
+                                num_map_scans=num_map_scans,
+                                map_scan=map_scan,
+                                num_modstates=num_modstates,
+                                modstate=modstate,
+                                start_time=start_time,
+                                num_meas=num_meas,
+                                meas_num=meas_num,
+                                arm_id="CI",
+                            )
+                            header_generator = (
+                                spec122_validator.validate_and_translate_to_214_l0(
+                                    d.header(), return_type=fits.HDUList
+                                )[0].header
+                                for d in ds
+                            )
+
+                            hdul = generate_fits_frame(
+                                header_generator=header_generator, shape=array_shape
+                            )
+                            header = hdul[0].header
+                            task.write(
+                                data=hdul,
+                                tags=[
+                                    CryonirspTag.task_observe(),
+                                    CryonirspTag.scan_step(scan_step),
+                                    CryonirspTag.map_scan(map_scan),
+                                    CryonirspTag.modstate(modstate),
+                                    CryonirspTag.linearized(),
+                                    CryonirspTag.frame(),
+                                    CryonirspTag.exposure_time(exposure_time),
+                                    CryonirspTag.meas_num(meas_num),
+                                ],
+                                encoder=fits_hdulist_encoder,
+                            )
+            yield task, request.param, header, intermediate_shape
         finally:
             task._purge()
 
 
 @pytest.fixture(scope="session")
-def sp_headers_with_dates() -> tuple[list[fits.Header], str, int, int]:
+def ci_headers_with_dates() -> tuple[list[fits.Header], str, int, int]:
     num_headers = 5
     start_time = "1969-12-06T18:00:00"
     exp_time = 12
     time_delta = 10
     ds = CryonirspHeadersValidObserveFrames(
         dataset_shape=(num_headers, 4, 4),
         array_shape=(1, 4, 4),
         time_delta=time_delta,
         num_map_scans=1,
         map_scan=1,
         num_scan_steps=1,
         scan_step=1,
+        num_meas=1,
+        meas_num=1,
         num_modstates=num_headers,
         modstate=1,
         start_time=datetime.fromisoformat(start_time),
-        num_meas=1,
-        meas_num=1,
-        arm_id="SP",
+        arm_id="CI",
     )
     headers = [
         spec122_validator.validate_and_translate_to_214_l0(d.header(), return_type=fits.HDUList)[
             0
         ].header
         for d in ds
     ]
@@ -231,70 +207,51 @@
     for h in headers:
         h["XPOSURE"] = exp_time  # Exposure time, in ms
 
     return headers, start_time, exp_time, time_delta
 
 
 @pytest.fixture(scope="session")
-def sp_compressed_headers_with_dates(
-    sp_headers_with_dates,
+def ci_compressed_headers_with_dates(
+    ci_headers_with_dates,
 ) -> tuple[list[fits.Header], str, int, int]:
-    headers, start_time, exp_time, time_delta = sp_headers_with_dates
+    headers, start_time, exp_time, time_delta = ci_headers_with_dates
     comp_headers = [fits.hdu.compressed.CompImageHeader(h, h) for h in headers]
     return comp_headers, start_time, exp_time, time_delta
 
 
-@pytest.fixture(scope="function")
-def sp_calibration_collection_with_geo_shifts(shifts) -> CalibrationCollection:
-    num_beams, num_mod, _ = shifts.shape
-    geo_shifts = {
-        str(b + 1): {f"m{m + 1}": shifts[b, m, :] for m in range(num_mod)} for b in range(num_beams)
-    }
-    return CalibrationCollection(
-        dark=dict(),
-        angle=dict(),
-        state_offset=geo_shifts,
-        spec_shift=dict(),
-        demod_matrices=None,
-    )
-
-
-def test_sp_science_calibration_task(sp_science_calibration_task, mocker):
+def test_ci_science_calibration_task(ci_science_calibration_task, mocker):
     """
-    Given: A SPScienceCalibration task
+    Given: A CIScienceCalibration task
     When: Calling the task instance
     Then: There are the expected number of science frames with the correct tags applied and the headers have been correctly updated
     """
 
     mocker.patch(
         "dkist_processing_common.tasks.mixin.metadata_store.GraphQLClient", new=FakeGQLClient
     )
 
     # When
-    task, polarization_mode, offset, og_header, og_single_beam_shape = sp_science_calibration_task
+    task, polarization_mode, og_header, og_single_beam_shape = ci_science_calibration_task
     task()
 
     # 1 from re-dummification
-    expected_final_shape = (
-        1,
-        og_single_beam_shape[0],
-        og_single_beam_shape[1],
-    )
+    expected_final_shape = (1, og_single_beam_shape[0], og_single_beam_shape[1])
 
     # Then
     tags = [
         CryonirspTag.calibrated(),
         CryonirspTag.frame(),
     ]
     files = list(task.read(tags=tags))
     if polarization_mode == "Full Stokes":
-        # 2 raster steps * 2 map scans * 4 stokes params = 16 frames
+        # 2 scan steps * 2 map scans * 4 stokes params = 16 frames
         assert len(files) == 16
     elif polarization_mode == "Stokes-I":
-        # 2 raster steps * 2 map scans * 1 stokes param = 4 frames
+        # 2 scan steps * 2 map scans * 1 stokes param = 4 frames
         assert len(files) == 4
     for file in files:
         hdul = fits.open(file)
         assert len(hdul) == 1
         hdu = hdul[0]
         assert type(hdul[0]) is fits.PrimaryHDU
         assert hdu.data.shape == expected_final_shape
@@ -305,40 +262,34 @@
         scan_step = [
             int(t.split("_")[-1]) for t in task.tags(file) if CryonirspStemName.scan_step.value in t
         ][0]
 
         assert hdu.header["CNNUMSCN"] == 2
         assert hdu.header["CNCURSCN"] == scan_step
 
-        # Check that WCS keys were updated
-        if offset[0] > 0:
-            assert hdu.header["CRPIX2"] == og_header["CRPIX2"]
-        if offset[1] > 0:
-            assert hdu.header["CRPIX1"] == og_header["CRPIX1"]
-
     quality_files = task.read(tags=[CryonirspTag.quality("TASK_TYPES")])
     for file in quality_files:
         with file.open() as f:
             data = json.load(f)
             assert isinstance(data, dict)
             assert data["total_frames"] == task.scratch.count_all(
                 tags=[CryonirspTag.linearized(), CryonirspTag.frame(), CryonirspTag.task_observe()]
             )
 
 
-def test_compute_sp_date_keys(sp_headers_with_dates, recipe_run_id, init_cryonirsp_constants_db):
+def test_compute_ci_date_keys(ci_headers_with_dates, recipe_run_id, init_cryonirsp_constants_db):
     """
-    Given: A set of SP headers with different DATE-OBS values
+    Given: A set of CI headers with different DATE-OBS values
     When: Computing the time over which the headers were taken
     Then: A header with correct DATE-BEG, DATE-END, and DATE-AVG keys is returned
     """
-    headers, start_time, exp_time, time_delta = sp_headers_with_dates
+    headers, start_time, exp_time, time_delta = ci_headers_with_dates
     constants_db = CryonirspConstantsDb()
     init_cryonirsp_constants_db(recipe_run_id, constants_db)
-    with SPScienceCalibration(
+    with CIScienceCalibration(
         recipe_run_id=recipe_run_id, workflow_name="science_calibration", workflow_version="VX.Y"
     ) as task:
         final_header = task._compute_date_keys(headers)
         final_header_from_single = task._compute_date_keys(headers[0])
 
     date_end = (
         Time(start_time)
@@ -355,26 +306,26 @@
         + TimeDelta(exp_time / 1000.0, format="sec")
     ).isot
 
     assert final_header_from_single["DATE-BEG"] == headers[0]["DATE-BEG"]
     assert final_header_from_single["DATE-END"] == date_end_from_single
 
 
-def test_compute_sp_date_keys_compressed_headers(
-    sp_compressed_headers_with_dates, recipe_run_id, init_cryonirsp_constants_db
+def test_compute_ci_date_keys_compressed_headers(
+    ci_compressed_headers_with_dates, recipe_run_id, init_cryonirsp_constants_db
 ):
     """
-    Given: A set of SP compressed headers with different DATE-OBS values
+    Given: A set of CI compressed headers with different DATE-OBS values
     When: Computing the time over which the headers were taken
     Then: A header with correct DATE-BEG, DATE-END, and DATE-AVG keys is returned
     """
-    headers, start_time, exp_time, time_delta = sp_compressed_headers_with_dates
+    headers, start_time, exp_time, time_delta = ci_compressed_headers_with_dates
     constants_db = CryonirspConstantsDb()
     init_cryonirsp_constants_db(recipe_run_id, constants_db)
-    with SPScienceCalibration(
+    with CIScienceCalibration(
         recipe_run_id=recipe_run_id, workflow_name="science_calibration", workflow_version="VX.Y"
     ) as task:
         final_header = task._compute_date_keys(headers)
         final_header_from_single = task._compute_date_keys(headers[0])
 
     date_end = (
         Time(start_time)
```

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tests/test_sp_solar.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tests/test_sp_solar.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import json
 from dataclasses import dataclass
 
 import numpy as np
 import pytest
 from dkist_processing_common._util.scratch import WorkflowFileSystem
+from dkist_processing_common.codecs.fits import fits_hdulist_encoder
 from dkist_processing_common.tests.conftest import FakeGQLClient
 
 from dkist_processing_cryonirsp.models.tags import CryonirspTag
 from dkist_processing_cryonirsp.tasks.sp_solar_gain import SPSolarGainCalibration
 from dkist_processing_cryonirsp.tests.conftest import cryonirsp_testing_parameters_factory
 from dkist_processing_cryonirsp.tests.conftest import CryonirspConstantsDb
 from dkist_processing_cryonirsp.tests.conftest import CryonirspHeadersValidSPSolarGainFrames
@@ -105,24 +106,25 @@
                     true_gain = np.ones(array_shape[1:]) + modstate + beam
                     true_solar_signal = np.arange(1, array_shape[1] + 1) / 5
                     true_solar_gain = true_gain * true_solar_signal[:, None]
                     raw_lamp = np.concatenate((lamp_cal, lamp_cal), axis=1)
                     raw_dark = np.concatenate((dark_cal, dark_cal), axis=1)
                     raw_solar = (true_solar_gain * raw_lamp) + raw_dark
                     solar_hdul = generate_214_l0_fits_frame(data=raw_solar, s122_header=header)
-                    task.fits_data_write(
-                        hdu_list=solar_hdul,
+                    task.write(
+                        data=solar_hdul,
                         tags=[
                             CryonirspTag.linearized(),
                             CryonirspTag.task_solar_gain(),
                             CryonirspTag.modstate(modstate),
                             CryonirspTag.frame(),
                             CryonirspTag.beam(beam),
                             CryonirspTag.exposure_time(exposure_time),
                         ],
+                        encoder=fits_hdulist_encoder,
                     )
 
             yield task
         finally:
             task._purge()
```

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tests/test_submit_qualilty.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tests/test_submit_qualilty.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/tests/test_write_l1.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/tests/test_write_l1.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import numpy as np
 import pytest
 from astropy.io import fits
 from astropy.time import Time
 from dkist_fits_specifications import __version__ as spec_version
 from dkist_header_validator import spec214_validator
+from dkist_processing_common.codecs.fits import fits_hdulist_encoder
 from dkist_processing_common.tests.conftest import FakeGQLClient
 
 from dkist_processing_cryonirsp.models.tags import CryonirspTag
 from dkist_processing_cryonirsp.tasks.write_l1 import CIWriteL1Frame
 from dkist_processing_cryonirsp.tasks.write_l1 import SPWriteL1Frame
 from dkist_processing_cryonirsp.tests.conftest import CryonirspConstantsDb
 
@@ -86,24 +87,25 @@
                 for scan_step in range(1, num_scan_steps + 1):
                     for meas_num in range(1, num_meas + 1):
                         # all stokes files have the same date-beg
                         hdul[0].header["DATE-BEG"] = datetime.now().isoformat("T")
                         for stokes_param in stokes_params:
                             hdul[0].header["CNCMEAS"] = meas_num
                             hdul[0].header["CNMAP"] = map_scan
-                            task.fits_data_write(
-                                hdu_list=hdul,
+                            task.write(
+                                data=hdul,
                                 tags=[
                                     CryonirspTag.calibrated(),
                                     CryonirspTag.frame(),
                                     CryonirspTag.stokes(stokes_param),
                                     CryonirspTag.meas_num(meas_num),
                                     CryonirspTag.map_scan(map_scan),
                                     CryonirspTag.scan_step(scan_step),
                                 ],
+                                encoder=fits_hdulist_encoder,
                             )
             yield task, stokes_params
         finally:
             task._purge()
 
 
 @pytest.mark.parametrize(
```

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/workflows/ci_l0_processing.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/workflows/ci_l0_processing.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/workflows/sp_l0_processing.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/workflows/sp_l0_processing.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp/workflows/trial_workflows.py` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp/workflows/trial_workflows.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp.egg-info/PKG-INFO` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-cryonirsp
-Version: 0.0.8
+Version: 0.0.9
 Summary: Science processing code for the Cryo-NIRSP instrument on DKIST
 Home-page: https://bitbucket.org/dkistdc/dkist_processing_cryonirsp/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp.egg-info/SOURCES.txt` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.8/dkist_processing_cryonirsp.egg-info/requires.txt` & `dkist_processing_cryonirsp-0.0.9/dkist_processing_cryonirsp.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Pillow==10.0.0
+Pillow==10.0.1
 astropy==5.3.2
 dkist-fits-specifications==3.8.1
 dkist-header-validator==4.1.0
 dkist-processing-common==4.1.2
 dkist-processing-math==2.0.0
 dkist-processing-pac==3.0.0
 dkist-spectral-lines==2.0.0
```

### Comparing `dkist_processing_cryonirsp-0.0.8/docs/Makefile` & `dkist_processing_cryonirsp-0.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.8/docs/conf.py` & `dkist_processing_cryonirsp-0.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.8/docs/l0_to_l1_cryonirsp_ci.rst` & `dkist_processing_cryonirsp-0.0.9/docs/l0_to_l1_cryonirsp_ci.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.8/docs/l0_to_l1_cryonirsp_sp.rst` & `dkist_processing_cryonirsp-0.0.9/docs/l0_to_l1_cryonirsp_sp.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.8/docs/make.bat` & `dkist_processing_cryonirsp-0.0.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.8/licenses/LICENSE.rst` & `dkist_processing_cryonirsp-0.0.9/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.8/pyproject.toml` & `dkist_processing_cryonirsp-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.8/setup.cfg` & `dkist_processing_cryonirsp-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 [options]
 python_requires = >=3.11
 setup_requires = setuptools_scm
 packages = find:
 include_package_data = True
 install_requires = 
-	Pillow == 10.0.0
+	Pillow == 10.0.1
 	astropy == 5.3.2
 	dkist-fits-specifications == 3.8.1
 	dkist-header-validator == 4.1.0
 	dkist-processing-common == 4.1.2
 	dkist-processing-math == 2.0.0
 	dkist-processing-pac == 3.0.0
 	dkist-spectral-lines == 2.0.0
```

