# Comparing `tmp/hdmf_zarr-0.6.0.tar.gz` & `tmp/hdmf_zarr-0.7.0.tar.gz`

## Comparing `hdmf_zarr-0.6.0.tar` & `hdmf_zarr-0.7.0.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/.gitattributes
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/.readthedocs.yaml
--rw-r--r--   0        0        0     6639 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/CHANGELOG.md
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/MANIFEST.in
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/requirements-dev.txt
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/requirements-doc.txt
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/requirements-min.txt
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/requirements-opt.txt
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/requirements.txt
--rw-r--r--   0        0        0     6723 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/test_gallery.py
--rw-r--r--   0        0        0     4845 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/tox.ini
--rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/.github/pull_request_template.md
--rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/.github/ISSUE_TEMPLATE/documentation.yml
--rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/.github/PULL_REQUEST_TEMPLATE/release.md
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/.github/workflows/HDMF_dev.yaml
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/.github/workflows/black.yml
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/.github/workflows/check_external_links.yml
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/.github/workflows/codespell.yml
--rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/.github/workflows/deploy_release.yml
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/.github/workflows/project_action.yml
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/.github/workflows/ruff.yml
--rw-r--r--   0        0        0     9972 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/.github/workflows/run_all_tests.yml
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/.github/workflows/run_coverage.yml
--rw-r--r--   0        0        0     7290 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/.github/workflows/run_tests.yml
--rw-r--r--   0        0        0     8006 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/docs/CONTRIBUTING.rst
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/docs/make.bat
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/docs/gallery/README.txt
--rw-r--r--   0        0        0     5355 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/docs/gallery/plot_convert_nwb_hdf5.py
--rw-r--r--   0        0        0     6033 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/docs/gallery/plot_nwb_zarrio.py
--rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/docs/gallery/plot_zarr_dataset_io.py
--rw-r--r--   0        0        0     7062 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/docs/gallery/plot_zarr_io.py
--rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/docs/gallery/resources/README.rst
--rw-r--r--   0        0        0   591336 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/docs/gallery/resources/sub_anm00239123_ses_20170627T093549_ecephys_and_ogen.nwb
--rw-r--r--   0        0        0     6424 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/docs/source/conf.py
--rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/docs/source/index.rst
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/docs/source/installation.rst
--rw-r--r--   0        0        0     8011 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/docs/source/integrating_data_stores.rst
--rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/docs/source/overview.rst
--rw-r--r--   0        0        0    22871 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/docs/source/storage.rst
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/docs/source/_static/theme_overrides.css
--rw-r--r--   0        0        0   313636 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/docs/source/figures/gallery_thumbnail_plot_convert_nwb.png
--rw-r--r--   0        0        0   919104 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/docs/source/figures/gallery_thumbnail_plot_nwbzarrio.png
--rw-r--r--   0        0        0   138349 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/docs/source/figures/gallery_thumbnail_plot_zarr_dataset_io.png
--rw-r--r--   0        0        0   873188 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/docs/source/figures/gallery_thumbnail_plot_zarr_io.png
--rw-r--r--   0        0        0   300594 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/docs/source/figures/gallery_thumbnails.pptx
--rw-r--r--   0        0        0   206548 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/docs/source/figures/logo_hdmf_zarr.pdf
--rw-r--r--   0        0        0   292818 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/docs/source/figures/logo_hdmf_zarr.png
--rw-r--r--   0        0        0    86114 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/docs/source/figures/logo_hdmf_zarr.pptx
--rw-r--r--   0        0        0    18867 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/docs/source/figures/logo_hdmf_zarr_iconsize.png
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/src/hdmf_zarr/__init__.py
--rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/src/hdmf_zarr/_due.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/src/hdmf_zarr/_version.py
--rw-r--r--   0        0        0    67782 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/src/hdmf_zarr/backend.py
--rw-r--r--   0        0        0     3553 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/src/hdmf_zarr/nwb.py
--rw-r--r--   0        0        0    26003 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/src/hdmf_zarr/utils.py
--rw-r--r--   0        0        0     8895 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/src/hdmf_zarr/zarr_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/tests/unit/__init__.py
--rw-r--r--   0        0        0    80482 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/tests/unit/base_tests_zarrio.py
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/tests/unit/test_fsspec_streaming.py
--rw-r--r--   0        0        0    46274 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/tests/unit/test_io_convert.py
--rw-r--r--   0        0        0    10893 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/tests/unit/test_parallel_write.py
--rw-r--r--   0        0        0    10937 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/tests/unit/test_zarrdataio.py
--rw-r--r--   0        0        0     5617 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/tests/unit/test_zarrio.py
--rw-r--r--   0        0        0    21641 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/tests/unit/utils.py
--rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/.gitignore
--rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/LICENSE.txt
--rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/README.rst
--rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     4729 2020-02-02 00:00:00.000000 hdmf_zarr-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/.gitattributes
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     7647 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/CHANGELOG.md
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/MANIFEST.in
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/requirements-dev.txt
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/requirements-doc.txt
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/requirements-min.txt
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/requirements-opt.txt
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/requirements.txt
+-rw-r--r--   0        0        0     7015 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/test_gallery.py
+-rw-r--r--   0        0        0     5037 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/tox.ini
+-rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/.github/pull_request_template.md
+-rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/.github/ISSUE_TEMPLATE/documentation.yml
+-rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/.github/PULL_REQUEST_TEMPLATE/release.md
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/.github/workflows/HDMF_dev.yaml
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/.github/workflows/black.yml
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/.github/workflows/check_external_links.yml
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/.github/workflows/codespell.yml
+-rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/.github/workflows/deploy_release.yml
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/.github/workflows/project_action.yml
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/.github/workflows/ruff.yml
+-rw-r--r--   0        0        0    10635 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/.github/workflows/run_all_tests.yml
+-rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/.github/workflows/run_coverage.yml
+-rw-r--r--   0        0        0     7290 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/.github/workflows/run_tests.yml
+-rw-r--r--   0        0        0     8006 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/docs/CONTRIBUTING.rst
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/docs/make.bat
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/docs/gallery/README.txt
+-rw-r--r--   0        0        0     5355 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/docs/gallery/plot_convert_nwb_hdf5.py
+-rw-r--r--   0        0        0     6033 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/docs/gallery/plot_nwb_zarrio.py
+-rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/docs/gallery/plot_zarr_dataset_io.py
+-rw-r--r--   0        0        0     7062 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/docs/gallery/plot_zarr_io.py
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/docs/gallery/resources/README.rst
+-rw-r--r--   0        0        0   591336 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/docs/gallery/resources/sub_anm00239123_ses_20170627T093549_ecephys_and_ogen.nwb
+-rw-r--r--   0        0        0     6424 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/docs/source/conf.py
+-rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/docs/source/index.rst
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/docs/source/installation.rst
+-rw-r--r--   0        0        0     8011 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/docs/source/integrating_data_stores.rst
+-rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/docs/source/overview.rst
+-rw-r--r--   0        0        0    22732 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/docs/source/storage.rst
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/docs/source/_static/theme_overrides.css
+-rw-r--r--   0        0        0   313636 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/docs/source/figures/gallery_thumbnail_plot_convert_nwb.png
+-rw-r--r--   0        0        0   919104 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/docs/source/figures/gallery_thumbnail_plot_nwbzarrio.png
+-rw-r--r--   0        0        0   138349 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/docs/source/figures/gallery_thumbnail_plot_zarr_dataset_io.png
+-rw-r--r--   0        0        0   873188 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/docs/source/figures/gallery_thumbnail_plot_zarr_io.png
+-rw-r--r--   0        0        0   300594 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/docs/source/figures/gallery_thumbnails.pptx
+-rw-r--r--   0        0        0   206548 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/docs/source/figures/logo_hdmf_zarr.pdf
+-rw-r--r--   0        0        0   292818 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/docs/source/figures/logo_hdmf_zarr.png
+-rw-r--r--   0        0        0    86114 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/docs/source/figures/logo_hdmf_zarr.pptx
+-rw-r--r--   0        0        0    18867 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/docs/source/figures/logo_hdmf_zarr_iconsize.png
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/src/hdmf_zarr/__init__.py
+-rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/src/hdmf_zarr/_due.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/src/hdmf_zarr/_version.py
+-rw-r--r--   0        0        0    68288 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/src/hdmf_zarr/backend.py
+-rw-r--r--   0        0        0     3553 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/src/hdmf_zarr/nwb.py
+-rw-r--r--   0        0        0    26003 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/src/hdmf_zarr/utils.py
+-rw-r--r--   0        0        0     8895 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/src/hdmf_zarr/zarr_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/tests/unit/__init__.py
+-rw-r--r--   0        0        0    80525 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/tests/unit/base_tests_zarrio.py
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/tests/unit/test_fsspec_streaming.py
+-rw-r--r--   0        0        0    46274 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/tests/unit/test_io_convert.py
+-rw-r--r--   0        0        0    10893 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/tests/unit/test_parallel_write.py
+-rw-r--r--   0        0        0    10937 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/tests/unit/test_zarrdataio.py
+-rw-r--r--   0        0        0     7243 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/tests/unit/test_zarrio.py
+-rw-r--r--   0        0        0    21641 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/tests/unit/utils.py
+-rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/.gitignore
+-rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/LICENSE.txt
+-rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/README.rst
+-rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     4785 2020-02-02 00:00:00.000000 hdmf_zarr-0.7.0/PKG-INFO
```

### Comparing `hdmf_zarr-0.6.0/.readthedocs.yaml` & `hdmf_zarr-0.7.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `hdmf_zarr-0.6.0/CHANGELOG.md` & `hdmf_zarr-0.7.0/CHANGELOG.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,22 @@
 # HDMF-ZARR Changelog
 
+## 0.7.0 (May 2, 2024)
+### Enhancements
+* Added support for python 3.12. @mavaylon1 [#172](https://github.com/hdmf-dev/hdmf-zarr/pull/172)
+* Added support for forcing read of files without consolidated metadata using  `mode=r-` in `ZarrIO`. @oruebel [#183](https://github.com/hdmf-dev/hdmf-zarr/pull/183)
+- Updated testing to not install in editable mode and not run `coverage` by default. @rly [#188](https://github.com/hdmf-dev/hdmf-zarr/pull/188)
+
+### Docs
+* Removed `linkable` from the documentation to keep in line with `hdmf-schema-language`. @mavaylon1 [#180](https://github.com/hdmf-dev/hdmf-zarr/pull/180)
+
+### Bug Fixes
+* Fixed bug in `ZarrIO.__open_file_consolidated` that led to remote files being opened without consolidated metadata. @oruebel  [#184](https://github.com/hdmf-dev/hdmf-zarr/pull/184) 
+* Fixed minor bug where `ZarrIO.__open_file_consolidated` used properties of `ZarrIO` instead of the provided input parameters. @oruebel [#183](https://github.com/hdmf-dev/hdmf-zarr/pull/183) 
+
 ## 0.6.0 (February 21, 2024)
 
 ### Enhancements
 * Enhanced `ZarrIO` and `ZarrDataIO` to infer io settings (e.g., chunking and compression) from HDF5 datasets to preserve storage settings on export if possible @oruebel [#153](https://github.com/hdmf-dev/hdmf-zarr/pull/153)
 * Updated writing references in compound datasets to same-sized array, rather than iteratively as an array of lists. @sneakers-the-rat [#146](https://github.com/hdmf-dev/hdmf-zarr/pull/146)
 
 ### Bug Fixes
```

### Comparing `hdmf_zarr-0.6.0/requirements-dev.txt` & `hdmf_zarr-0.7.0/requirements-dev.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # pinned dependencies to reproduce an entire development environment to use HDMF-Zarr,
 # run HDMF-Zarr tests, check code style,
 # compute coverage, and create test environments. note that depending on the version of python installed, different
 # versions of requirements may be installed due to package incompatibilities.
 #
-black==23.10.1
+black==24.3.0
 codespell==2.2.6
 coverage==7.3.2
 hdf5plugin==4.3.0  # hdf5plugin is used to test conversion of plugin filters
 pre-commit==3.5.0
 pytest==7.4.3
 pytest-cov==4.1.0
 python-dateutil==2.8.2
```

### Comparing `hdmf_zarr-0.6.0/test_gallery.py` & `hdmf_zarr-0.7.0/test_gallery.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,14 +69,17 @@
     "is set), then you will need to pop the extra arguments out of kwargs before calling the function."
 )
 
 _deprecation_warning_pandas_pyarrow_re = (
     r"\nPyarrow will become a required dependency of pandas.*"
 )
 
+_deprecation_warning_datetime = (
+    r"datetime.datetime.utcfromtimestamp() *"
+)
 
 def run_gallery_tests():
     global TOTAL, FAILURES, ERRORS
     logging.info("Testing execution of Sphinx Gallery files")
 
     # get all python file names in docs/gallery
     gallery_file_names = list()
@@ -131,14 +134,18 @@
                     # this warning is triggered when downstream code such as pynwb uses pkg_resources>=5.13
                     "ignore", message=_pkg_resources_declare_warning_re, category=DeprecationWarning
                 )
                 warnings.filterwarnings(
                     # this warning is triggered from pandas
                     "ignore", message=_deprecation_warning_pandas_pyarrow_re, category=DeprecationWarning
                 )
+                warnings.filterwarnings(
+                    # this is triggered from datetime
+                    "ignore", message=_deprecation_warning_datetime, category=DeprecationWarning
+                )
                 _import_from_file(script_abs)
         except Exception:
             print(traceback.format_exc())
             FAILURES += 1
             ERRORS += 1
     # Make sure to reset the working directory at the end
     os.chdir(curr_dir)
```

### Comparing `hdmf_zarr-0.6.0/tox.ini` & `hdmf_zarr-0.7.0/tox.ini`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # Tox (https://tox.readthedocs.io/) is a tool for running tests
 # in multiple virtualenvs. This configuration file will run the
 # test suite on all supported python versions. To use it, "python -m pip install tox"
 # and then run "tox" from this directory.
 
 [tox]
-envlist = py38, py39, py310, py311
+envlist = py38, py39, py310, py311, py312
 requires = pip >= 22.0
 
 [testenv]
 download = True
-usedevelop = True
 setenv =
   PYTHONDONTWRITEBYTECODE = 1
   VIRTUALENV_python -m pip = 22.3.1
 install_command =
     python -m pip install {opts} {packages}
 
 deps =
@@ -22,42 +21,42 @@
 
 commands =
     python -m pip check  # Check for conflicting packages
     pytest -v
 
 # Env to create coverage report locally
 [testenv:localcoverage]
-basepython = python3.11
+basepython = python3.12
 commands =
     pytest --cov=hdmf_zarr
     coverage html -d tests/coverage/htmlcov
 
-# Test with python 3.11; pinned dev and optional reqs
-[testenv:py311-optional]
-basepython = python3.11
+# Test with python 3.12; pinned dev and optional reqs
+[testenv:py312-optional]
+basepython = python3.12
 install_command =
     python -m pip install {opts} {packages}
 deps =
     {[testenv]deps}
     -rrequirements-opt.txt
 commands = {[testenv]commands}
 
-# Test with python 3.11; pinned dev and optional reqs; upgraded run reqs
-[testenv:py311-upgraded]
-basepython = python3.11
+# Test with python 3.12; pinned dev and optional reqs; upgraded run reqs
+[testenv:py312-upgraded]
+basepython = python3.12
 install_command =
     python -m pip install -U {opts} {packages}
 deps =
     -rrequirements-dev.txt
     -rrequirements-opt.txt
 commands = {[testenv]commands}
 
-# Test with python 3.11; pinned dev and optional reqs; upgraded, pre-release run reqs
-[testenv:py311-prerelease]
-basepython = python3.11
+# Test with python 3.12; pinned dev and optional reqs; upgraded, pre-release run reqs
+[testenv:py312-prerelease]
+basepython = python3.12
 install_command =
     python -m pip install -U --pre {opts} {packages}
 deps =
     -rrequirements-dev.txt
     -rrequirements-opt.txt
 commands = {[testenv]commands}
 
@@ -87,32 +86,36 @@
 basepython = python3.10
 commands = {[testenv:build]commands}
 
 [testenv:build-py311]
 basepython = python3.11
 commands = {[testenv:build]commands}
 
-[testenv:build-py311-optional]
-basepython = python3.11
+[testenv:build-py312]
+basepython = python3.12
+commands = {[testenv:build]commands}
+
+[testenv:build-py312-optional]
+basepython = python3.12
 deps =
     {[testenv]deps}
     -rrequirements-opt.txt
 commands = {[testenv:build]commands}
 
-[testenv:build-py311-upgraded]
-basepython = python3.11
+[testenv:build-py312-upgraded]
+basepython = python3.12
 install_command =
     python -m pip install -U {opts} {packages}
 deps =
     -rrequirements-dev.txt
     -rrequirements-opt.txt
 commands = {[testenv:build]commands}
 
-[testenv:build-py311-prerelease]
-basepython = python3.11
+[testenv:build-py312-prerelease]
+basepython = python3.12
 install_command =
     python -m pip install -U --pre {opts} {packages}
 deps =
     -rrequirements-dev.txt
     -rrequirements-opt.txt
 commands = {[testenv:build]commands}
 
@@ -157,28 +160,33 @@
 commands = {[testenv:gallery]commands}
 
 [testenv:gallery-py311]
 basepython = python3.11
 deps = {[testenv:gallery]deps}
 commands = {[testenv:gallery]commands}
 
-# Test with python 3.11; pinned dev, doc, and optional reqs; upgraded run reqs
-[testenv:gallery-py311-upgraded]
-basepython = python3.11
+[testenv:gallery-py312]
+basepython = python3.12
+deps = {[testenv:gallery]deps}
+commands = {[testenv:gallery]commands}
+
+# Test with python 3.12; pinned dev, doc, and optional reqs; upgraded run reqs
+[testenv:gallery-py312-upgraded]
+basepython = python3.12
 install_command =
     python -m pip install -U {opts} {packages}
 deps =
     -rrequirements-dev.txt
     -rrequirements-doc.txt
     -rrequirements-opt.txt
 commands = {[testenv:gallery]commands}
 
-# Test with python 3.11; pinned dev, doc, and optional reqs; pre-release run reqs
-[testenv:gallery-py311-prerelease]
-basepython = python3.11
+# Test with python 3.12; pinned dev, doc, and optional reqs; pre-release run reqs
+[testenv:gallery-py312-prerelease]
+basepython = python3.12
 install_command =
     python -m pip install -U --pre {opts} {packages}
 deps =
     -rrequirements-dev.txt
     -rrequirements-doc.txt
     -rrequirements-opt.txt
 commands = {[testenv:gallery]commands}
```

### Comparing `hdmf_zarr-0.6.0/.github/CODE_OF_CONDUCT.md` & `hdmf_zarr-0.7.0/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `hdmf_zarr-0.6.0/.github/pull_request_template.md` & `hdmf_zarr-0.7.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `hdmf_zarr-0.6.0/.github/ISSUE_TEMPLATE/bug_report.yml` & `hdmf_zarr-0.7.0/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files 1% similar despite different names*

```diff
@@ -62,14 +62,15 @@
     attributes:
       label: Python Version
       options:
         - "3.8"
         - "3.9"
         - "3.10"
         - "3.11"
+        - "3.12"
     validations:
       required: true
   - type: textarea
     id: package_versions
     attributes:
       label: Package Versions
       description: |
```

### Comparing `hdmf_zarr-0.6.0/.github/ISSUE_TEMPLATE/documentation.yml` & `hdmf_zarr-0.7.0/.github/ISSUE_TEMPLATE/documentation.yml`

 * *Files identical despite different names*

### Comparing `hdmf_zarr-0.6.0/.github/ISSUE_TEMPLATE/feature_request.yml` & `hdmf_zarr-0.7.0/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `hdmf_zarr-0.6.0/.github/workflows/HDMF_dev.yaml` & `hdmf_zarr-0.7.0/.github/workflows/HDMF_dev.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -12,30 +12,30 @@
           all_but_latest: true
           access_token: ${{ github.token }}
           
       - uses: actions/checkout@v4
         with:
             fetch-depth: 0  # tags are required for versioneer to determine the version
       
-      - name: Set up Python 3.11
-        uses: actions/setup-python@v4
+      - name: Set up Python 3.12
+        uses: actions/setup-python@v5
         with:
-          python-version: "3.11"
+          python-version: "3.12"
 
       - name: Install HDMF_Zarr Requirements
         run: |
           python -m pip install -r requirements-dev.txt -r requirements.txt
-          pip install -e .
+          pip install .
           
       - name: Clone HDMF Dev Branch
         run: |
           git clone https://github.com/hdmf-dev/hdmf.git --recurse-submodules
           cd hdmf
           python -m pip install -r requirements-dev.txt -r requirements.txt
-          python -m pip install -e .
+          python -m pip install .
           cd ..
 
       - name: Run HDMF_Zarr Tests
         run:
           pytest -v tests
```

### Comparing `hdmf_zarr-0.6.0/.github/workflows/check_external_links.yml` & `hdmf_zarr-0.7.0/.github/workflows/check_external_links.yml`

 * *Files 2% similar despite different names*

```diff
@@ -11,22 +11,22 @@
     steps:
       - name: Cancel non-latest runs
         uses: styfle/cancel-workflow-action@0.11.0
         with:
           all_but_latest: true
           access_token: ${{ github.token }}
 
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           submodules: 'recursive'
 
       - name: Set up Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
-          python-version: '3.11'
+          python-version: '3.12'
 
       - name: Install Sphinx dependencies and package
         run: |
           python -m pip install --upgrade pip
           python -m pip install -r requirements-doc.txt -r requirements.txt -r requirements-opt.txt
           python -m pip install .
       - name: Check Sphinx external links
```

### Comparing `hdmf_zarr-0.6.0/.github/workflows/deploy_release.yml` & `hdmf_zarr-0.7.0/.github/workflows/deploy_release.yml`

 * *Files 6% similar despite different names*

```diff
@@ -14,29 +14,29 @@
         with:
           submodules: 'recursive'
           fetch-depth: 0  # tags are required for versioneer to determine the version
 
       - name: Set up Python
         uses: actions/setup-python@v5
         with:
-          python-version: '3.11'
+          python-version: '3.12'
 
       - name: Install build dependencies
         run: |
           python -m pip install --upgrade pip
           python -m pip install tox
           python -m pip list
 
       - name: Run tox tests
         run: |
-          tox -e py311-upgraded
+          tox -e py312-upgraded
 
       - name: Build wheel and source distribution
         run: |
-          tox -e build-py311-upgraded
+          tox -e build-py312-upgraded
           ls -1 dist
 
       - name: Test installation from a wheel
         run: |
           tox -e wheelinstall --recreate --installpkg dist/*-none-any.whl
 
       - name: Upload wheel and source distributions to PyPI
```

### Comparing `hdmf_zarr-0.6.0/.github/workflows/project_action.yml` & `hdmf_zarr-0.7.0/.github/workflows/project_action.yml`

 * *Files identical despite different names*

### Comparing `hdmf_zarr-0.6.0/.github/workflows/run_all_tests.yml` & `hdmf_zarr-0.7.0/.github/workflows/run_all_tests.yml`

 * *Files 10% similar despite different names*

```diff
@@ -22,45 +22,48 @@
       fail-fast: false
       matrix:
         include:
           - { name: linux-python3.8-minimum      , test-tox-env: py38-minimum    , build-tox-env: build-py38-minimum    , python-ver: "3.8" , os: ubuntu-latest }
           - { name: linux-python3.9              , test-tox-env: py39            , build-tox-env: build-py39            , python-ver: "3.9" , os: ubuntu-latest }
           - { name: linux-python3.10             , test-tox-env: py310           , build-tox-env: build-py310           , python-ver: "3.10", os: ubuntu-latest }
           - { name: linux-python3.11             , test-tox-env: py311           , build-tox-env: build-py311           , python-ver: "3.11", os: ubuntu-latest }
-          - { name: linux-python3.11-optional    , test-tox-env: py311-optional  , build-tox-env: build-py311-optional  , python-ver: "3.11", os: ubuntu-latest }
-          - { name: linux-python3.11-upgraded    , test-tox-env: py311-upgraded  , build-tox-env: build-py311-upgraded  , python-ver: "3.11", os: ubuntu-latest }
-          - { name: linux-python3.11-prerelease  , test-tox-env: py311-prerelease, build-tox-env: build-py311-prerelease, python-ver: "3.11", os: ubuntu-latest }
+          - { name: linux-python3.12             , test-tox-env: py312           , build-tox-env: build-py312           , python-ver: "3.12", os: ubuntu-latest }
+          - { name: linux-python3.12-optional    , test-tox-env: py312-optional  , build-tox-env: build-py312-optional  , python-ver: "3.12", os: ubuntu-latest }
+          - { name: linux-python3.12-upgraded    , test-tox-env: py312-upgraded  , build-tox-env: build-py312-upgraded  , python-ver: "3.12", os: ubuntu-latest }
+          - { name: linux-python3.12-prerelease  , test-tox-env: py312-prerelease, build-tox-env: build-py312-prerelease, python-ver: "3.12", os: ubuntu-latest }
           - { name: windows-python3.8-minimum    , test-tox-env: py38-minimum    , build-tox-env: build-py38-minimum    , python-ver: "3.8" , os: windows-latest }
           - { name: windows-python3.9            , test-tox-env: py39            , build-tox-env: build-py39            , python-ver: "3.9" , os: windows-latest }
           - { name: windows-python3.10           , test-tox-env: py310           , build-tox-env: build-py310           , python-ver: "3.10", os: windows-latest }
           - { name: windows-python3.11           , test-tox-env: py311           , build-tox-env: build-py311           , python-ver: "3.11", os: windows-latest }
-          - { name: windows-python3.11-optional  , test-tox-env: py311-optional  , build-tox-env: build-py311-optional  , python-ver: "3.11", os: windows-latest }
-          - { name: windows-python3.11-upgraded  , test-tox-env: py311-upgraded  , build-tox-env: build-py311-upgraded  , python-ver: "3.11", os: windows-latest }
-          - { name: windows-python3.11-prerelease, test-tox-env: py311-prerelease, build-tox-env: build-py311-prerelease, python-ver: "3.11", os: windows-latest }
+          - { name: windows-python3.12           , test-tox-env: py312           , build-tox-env: build-py312           , python-ver: "3.12", os: windows-latest } 
+          - { name: windows-python3.12-optional  , test-tox-env: py312-optional  , build-tox-env: build-py312-optional  , python-ver: "3.12", os: windows-latest }
+          - { name: windows-python3.12-upgraded  , test-tox-env: py312-upgraded  , build-tox-env: build-py312-upgraded  , python-ver: "3.12", os: windows-latest }
+          - { name: windows-python3.12-prerelease, test-tox-env: py312-prerelease, build-tox-env: build-py312-prerelease, python-ver: "3.12", os: windows-latest }
           - { name: macos-python3.8-minimum      , test-tox-env: py38-minimum    , build-tox-env: build-py38-minimum    , python-ver: "3.8" , os: macos-latest }
           - { name: macos-python3.9              , test-tox-env: py39            , build-tox-env: build-py39            , python-ver: "3.9" , os: macos-latest }
           - { name: macos-python3.10             , test-tox-env: py310           , build-tox-env: build-py310           , python-ver: "3.10", os: macos-latest }
           - { name: macos-python3.11             , test-tox-env: py311           , build-tox-env: build-py311           , python-ver: "3.11", os: macos-latest }
-          - { name: macos-python3.11-optional    , test-tox-env: py311-optional  , build-tox-env: build-py311-optional  , python-ver: "3.11", os: macos-latest }
-          - { name: macos-python3.11-upgraded    , test-tox-env: py311-upgraded  , build-tox-env: build-py311-upgraded  , python-ver: "3.11", os: macos-latest }
-          - { name: macos-python3.11-prerelease  , test-tox-env: py311-prerelease, build-tox-env: build-py311-prerelease, python-ver: "3.11", os: macos-latest }
+          - { name: macos-python3.12             , test-tox-env: py312           , build-tox-env: build-py312           , python-ver: "3.12", os: macos-latest }
+          - { name: macos-python3.12-optional    , test-tox-env: py312-optional  , build-tox-env: build-py312-optional  , python-ver: "3.12", os: macos-latest }
+          - { name: macos-python3.12-upgraded    , test-tox-env: py312-upgraded  , build-tox-env: build-py312-upgraded  , python-ver: "3.12", os: macos-latest }
+          - { name: macos-python3.12-prerelease  , test-tox-env: py312-prerelease, build-tox-env: build-py312-prerelease, python-ver: "3.12", os: macos-latest }
     steps:
       - name: Cancel non-latest runs
         uses: styfle/cancel-workflow-action@0.11.0
         with:
           all_but_latest: true
           access_token: ${{ github.token }}
 
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           submodules: 'recursive'
           fetch-depth: 0  # tags are required for versioneer to determine the version
 
       - name: Set up Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-ver }}
 
       - name: Install build dependencies
         run: |
           python -m pip install --upgrade pip
           python -m pip install tox
@@ -82,36 +85,36 @@
       run:
         shell: bash
     strategy:
       fail-fast: false
       matrix:
         include:
           - { name: linux-gallery-python3.8-minimum      , test-tox-env: gallery-py38-minimum    , python-ver: "3.8" , os: ubuntu-latest }
-          - { name: linux-gallery-python3.11-upgraded    , test-tox-env: gallery-py311-upgraded  , python-ver: "3.11", os: ubuntu-latest }
-          - { name: linux-gallery-python3.11-prerelease  , test-tox-env: gallery-py311-prerelease, python-ver: "3.11", os: ubuntu-latest }
+          - { name: linux-gallery-python3.12-upgraded    , test-tox-env: gallery-py312-upgraded  , python-ver: "3.12", os: ubuntu-latest }
+          - { name: linux-gallery-python3.12-prerelease  , test-tox-env: gallery-py312-prerelease, python-ver: "3.12", os: ubuntu-latest }
           - { name: windows-gallery-python3.8-minimum    , test-tox-env: gallery-py38-minimum    , python-ver: "3.8" , os: windows-latest }
-          - { name: windows-gallery-python3.11-upgraded  , test-tox-env: gallery-py311-upgraded  , python-ver: "3.11", os: windows-latest }
-          - { name: windows-gallery-python3.11-prerelease, test-tox-env: gallery-py311-prerelease, python-ver: "3.11", os: windows-latest }
+          - { name: windows-gallery-python3.12-upgraded  , test-tox-env: gallery-py312-upgraded  , python-ver: "3.12", os: windows-latest }
+          - { name: windows-gallery-python3.12-prerelease, test-tox-env: gallery-py312-prerelease, python-ver: "3.12", os: windows-latest }
           - { name: macos-gallery-python3.8-minimum      , test-tox-env: gallery-py38-minimum    , python-ver: "3.8" , os: macos-latest }
-          - { name: macos-gallery-python3.11-upgraded    , test-tox-env: gallery-py311-upgraded  , python-ver: "3.11", os: macos-latest }
-          - { name: macos-gallery-python3.11-prerelease  , test-tox-env: gallery-py311-prerelease, python-ver: "3.11", os: macos-latest }
+          - { name: macos-gallery-python3.12-upgraded    , test-tox-env: gallery-py312-upgraded  , python-ver: "3.12", os: macos-latest }
+          - { name: macos-gallery-python3.12-prerelease  , test-tox-env: gallery-py312-prerelease, python-ver: "3.12", os: macos-latest }
     steps:
       - name: Cancel non-latest runs
         uses: styfle/cancel-workflow-action@0.11.0
         with:
           all_but_latest: true
           access_token: ${{ github.token }}
 
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           submodules: 'recursive'
           fetch-depth: 0  # tags are required for versioneer to determine the version
 
       - name: Set up Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-ver }}
 
       - name: Install build dependencies
         run: |
           python -m pip install --upgrade pip
           python -m pip install tox
@@ -129,25 +132,26 @@
       fail-fast: false
       matrix:
         include:
           - { name: conda-linux-python3.8-minimum    , test-tox-env: py38-minimum    , build-tox-env: build-py38-minimum    , python-ver: "3.8" , os: ubuntu-latest }
           - { name: conda-linux-python3.9            , test-tox-env: py39            , build-tox-env: build-py39            , python-ver: "3.9" , os: ubuntu-latest }
           - { name: conda-linux-python3.10           , test-tox-env: py310           , build-tox-env: build-py310           , python-ver: "3.10", os: ubuntu-latest }
           - { name: conda-linux-python3.11           , test-tox-env: py311           , build-tox-env: build-py311           , python-ver: "3.11", os: ubuntu-latest }
-          - { name: conda-linux-python3.11-optional  , test-tox-env: py311-optional  , build-tox-env: build-py311-optional  , python-ver: "3.11", os: ubuntu-latest }
-          - { name: conda-linux-python3.11-upgraded  , test-tox-env: py311-upgraded  , build-tox-env: build-py311-upgraded  , python-ver: "3.11", os: ubuntu-latest }
-          - { name: conda-linux-python3.11-prerelease, test-tox-env: py311-prerelease, build-tox-env: build-py311-prerelease, python-ver: "3.11", os: ubuntu-latest }
+          - { name: conda-linux-python3.12           , test-tox-env: py312           , build-tox-env: build-py312           , python-ver: "3.12", os: ubuntu-latest }          
+          - { name: conda-linux-python3.12-optional  , test-tox-env: py312-optional  , build-tox-env: build-py312-optional  , python-ver: "3.12", os: ubuntu-latest }
+          - { name: conda-linux-python3.12-upgraded  , test-tox-env: py312-upgraded  , build-tox-env: build-py312-upgraded  , python-ver: "3.12", os: ubuntu-latest }
+          - { name: conda-linux-python3.12-prerelease, test-tox-env: py312-prerelease, build-tox-env: build-py312-prerelease, python-ver: "3.12", os: ubuntu-latest }
     steps:
       - name: Cancel non-latest runs
         uses: styfle/cancel-workflow-action@0.11.0
         with:
           all_but_latest: true
           access_token: ${{ github.token }}
 
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           submodules: 'recursive'
           fetch-depth: 0  # tags are required for versioneer to determine the version
 
       - name: Set up Conda
         uses: conda-incubator/setup-miniconda@v2
         with:
```

### Comparing `hdmf_zarr-0.6.0/.github/workflows/run_coverage.yml` & `hdmf_zarr-0.7.0/.github/workflows/run_coverage.yml`

 * *Files 13% similar despite different names*

```diff
@@ -24,44 +24,50 @@
         include:
           - { os: ubuntu-latest , opt_req: true }
           - { os: ubuntu-latest , opt_req: false }
           - { os: windows-latest, opt_req: false }
           - { os: macos-latest  , opt_req: false }
     env:
       OS: ${{ matrix.os }}
-      PYTHON: '3.11'
+      PYTHON: '3.12'
     steps:
       - name: Cancel non-latest runs
         uses: styfle/cancel-workflow-action@0.11.0
         with:
           all_but_latest: true
           access_token: ${{ github.token }}
 
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           submodules: 'recursive'
 
       - name: Set up Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ env.PYTHON }}
 
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
-          python -m pip install -r requirements-dev.txt -r requirements.txt -r requirements-opt.txt
+          python -m pip install -r requirements-dev.txt -r requirements.txt
+
+      - name: Install optional dependencies
+        if: ${{ matrix.opt_req }}
+        run: python -m pip install -r requirements-opt.txt
 
       - name: Install package
         run: |
-          python -m pip install -e .  # must install in editable mode for coverage to find sources
+          python -m pip install .
           python -m pip list
+
       - name: Run tests and generate coverage report
         run: |
-          pytest --cov
-          python -m coverage xml  # codecov uploader requires xml format
-          python -m coverage report -m
+          # coverage is configured in pyproject.toml
+          pytest --cov --cov-report=xml --cov-report=term  # codecov uploader requires xml format
+
       - name: Upload coverage to Codecov
         uses: codecov/codecov-action@v4
         with:
           fail_ci_if_error: true
+          file: ./coverage.xml
         env:
           CODECOV_TOKEN: ${{ secrets.CODECOV_TOKEN }}
```

### Comparing `hdmf_zarr-0.6.0/.github/workflows/run_tests.yml` & `hdmf_zarr-0.7.0/.github/workflows/run_tests.yml`

 * *Files 4% similar despite different names*

```diff
@@ -16,35 +16,35 @@
       run:
         shell: bash
     strategy:
       fail-fast: false
       matrix:
         include:
           - { name: linux-python3.8-minimum      , test-tox-env: py38-minimum    , build-tox-env: build-py38-minimum    , python-ver: "3.8" , os: ubuntu-latest }
-          - { name: linux-python3.11             , test-tox-env: py311           , build-tox-env: build-py311           , python-ver: "3.11", os: ubuntu-latest }
+          - { name: linux-python3.12             , test-tox-env: py312           , build-tox-env: build-py312           , python-ver: "3.12", os: ubuntu-latest }
           # NOTE config below with "upload-wheels: true" specifies that wheels should be uploaded as an artifact
-          - { name: linux-python3.11-upgraded    , test-tox-env: py311-upgraded  , build-tox-env: build-py311-upgraded  , python-ver: "3.11", os: ubuntu-latest , upload-wheels: true }
+          - { name: linux-python3.12-upgraded    , test-tox-env: py312-upgraded  , build-tox-env: build-py312-upgraded  , python-ver: "3.12", os: ubuntu-latest , upload-wheels: true }
           - { name: windows-python3.8-minimum    , test-tox-env: py38-minimum    , build-tox-env: build-py38-minimum    , python-ver: "3.8" , os: windows-latest }
-          - { name: windows-python3.11-upgraded  , test-tox-env: py311-upgraded  , build-tox-env: build-py311-upgraded  , python-ver: "3.11", os: windows-latest }
+          - { name: windows-python3.12-upgraded  , test-tox-env: py312-upgraded  , build-tox-env: build-py312-upgraded  , python-ver: "3.12", os: windows-latest }
           - { name: macos-python3.8-minimum      , test-tox-env: py38-minimum    , build-tox-env: build-py38-minimum    , python-ver: "3.8" , os: macos-latest }
-          - { name: macos-python3.11-upgraded    , test-tox-env: py311-upgraded  , build-tox-env: build-py311-upgraded  , python-ver: "3.11", os: macos-latest }
+          - { name: macos-python3.12-upgraded    , test-tox-env: py312-upgraded  , build-tox-env: build-py312-upgraded  , python-ver: "3.12", os: macos-latest }
     steps:
       - name: Cancel non-latest runs
         uses: styfle/cancel-workflow-action@0.11.0
         with:
           all_but_latest: true
           access_token: ${{ github.token }}
 
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           submodules: 'recursive'
           fetch-depth: 0  # tags are required for versioneer to determine the version
 
       - name: Set up Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-ver }}
 
       - name: Install build dependencies
         run: |
           python -m pip install --upgrade pip
           python -m pip install tox
@@ -73,30 +73,30 @@
       run:
         shell: bash
     strategy:
       fail-fast: false
       matrix:
         include:
           - { name: linux-gallery-python3.8-minimum    , test-tox-env: gallery-py38-minimum  , python-ver: "3.8" , os: ubuntu-latest }
-          - { name: linux-gallery-python3.11-upgraded  , test-tox-env: gallery-py311-upgraded, python-ver: "3.11", os: ubuntu-latest }
+          - { name: linux-gallery-python3.12-upgraded  , test-tox-env: gallery-py312-upgraded, python-ver: "3.12", os: ubuntu-latest }
           - { name: windows-gallery-python3.8-minimum  , test-tox-env: gallery-py38-minimum  , python-ver: "3.8" , os: windows-latest }
-          - { name: windows-gallery-python3.11-upgraded, test-tox-env: gallery-py311-upgraded, python-ver: "3.11", os: windows-latest }
+          - { name: windows-gallery-python3.12-upgraded, test-tox-env: gallery-py312-upgraded, python-ver: "3.12", os: windows-latest }
     steps:
       - name: Cancel non-latest runs
         uses: styfle/cancel-workflow-action@0.11.0
         with:
           all_but_latest: true
           access_token: ${{ github.token }}
 
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           submodules: 'recursive'
 
       - name: Set up Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-ver }}
 
       - name: Install build dependencies
         run: |
           python -m pip install --upgrade pip
           python -m pip install tox
@@ -111,23 +111,23 @@
      run:
        shell: bash -l {0}
     strategy:
       fail-fast: false
       matrix:
         include:
           - { name: conda-linux-python3.8-minimum    , test-tox-env: py38-minimum    , build-tox-env: build-py38-minimum    , python-ver: "3.8" , os: ubuntu-latest }
-          - { name: conda-linux-python3.11-upgraded  , test-tox-env: py311-upgraded  , build-tox-env: build-py311-upgraded  , python-ver: "3.11", os: ubuntu-latest }
+          - { name: conda-linux-python3.12-upgraded  , test-tox-env: py312-upgraded  , build-tox-env: build-py312-upgraded  , python-ver: "3.12", os: ubuntu-latest }
     steps:
       - name: Cancel non-latest runs
         uses: styfle/cancel-workflow-action@0.11.0
         with:
           all_but_latest: true
           access_token: ${{ github.token }}
 
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           submodules: 'recursive'
           fetch-depth: 0  # tags are required for versioneer to determine the version
 
       - name: Set up Conda
         uses: conda-incubator/setup-miniconda@v2
         with:
@@ -161,20 +161,20 @@
       - name: Cancel non-latest runs
         uses: styfle/cancel-workflow-action@0.11.0
         with:
           all_but_latest: true
           access_token: ${{ github.token }}
 
       - name: Checkout repo with submodules
-        uses: actions/checkout@v3
+        uses: actions/checkout@v4
         with:
           submodules: 'recursive'
 
       - name: Set up Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: '3.11'
 
       - name: Download wheel and source distributions from artifact
         uses: actions/download-artifact@v3
         with:
           name: distributions
```

### Comparing `hdmf_zarr-0.6.0/docs/CONTRIBUTING.rst` & `hdmf_zarr-0.7.0/docs/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `hdmf_zarr-0.6.0/docs/Makefile` & `hdmf_zarr-0.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hdmf_zarr-0.6.0/docs/make.bat` & `hdmf_zarr-0.7.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hdmf_zarr-0.6.0/docs/gallery/plot_convert_nwb_hdf5.py` & `hdmf_zarr-0.7.0/docs/gallery/plot_convert_nwb_hdf5.py`

 * *Files identical despite different names*

### Comparing `hdmf_zarr-0.6.0/docs/gallery/plot_nwb_zarrio.py` & `hdmf_zarr-0.7.0/docs/gallery/plot_nwb_zarrio.py`

 * *Files identical despite different names*

### Comparing `hdmf_zarr-0.6.0/docs/gallery/plot_zarr_dataset_io.py` & `hdmf_zarr-0.7.0/docs/gallery/plot_zarr_dataset_io.py`

 * *Files identical despite different names*

### Comparing `hdmf_zarr-0.6.0/docs/gallery/plot_zarr_io.py` & `hdmf_zarr-0.7.0/docs/gallery/plot_zarr_io.py`

 * *Files identical despite different names*

### Comparing `hdmf_zarr-0.6.0/docs/gallery/resources/README.rst` & `hdmf_zarr-0.7.0/docs/gallery/resources/README.rst`

 * *Files identical despite different names*

### Comparing `hdmf_zarr-0.6.0/docs/gallery/resources/sub_anm00239123_ses_20170627T093549_ecephys_and_ogen.nwb` & `hdmf_zarr-0.7.0/docs/gallery/resources/sub_anm00239123_ses_20170627T093549_ecephys_and_ogen.nwb`

 * *Files identical despite different names*

### Comparing `hdmf_zarr-0.6.0/docs/source/conf.py` & `hdmf_zarr-0.7.0/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     'gallery_dirs': ['tutorials'],
     'backreferences_dir': 'gen_modules/backreferences',
     'min_reported_time': 5,
     'remove_config_comments': True
 }
 
 intersphinx_mapping = {
-    'python': ('https://docs.python.org/3.11', None),
+    'python': ('https://docs.python.org/3.12', None),
     'numpy': ('https://numpy.org/doc/stable/', None),
     'scipy': ('https://docs.scipy.org/doc/scipy/', None),
     'matplotlib': ('https://matplotlib.org/stable/', None),
     'h5py': ('https://docs.h5py.org/en/latest/', None),
     'pandas': ('https://pandas.pydata.org/pandas-docs/stable/', None),
     'hdmf': ('https://hdmf.readthedocs.io/en/stable/', None),
     'pynwb': ('https://pynwb.readthedocs.io/en/stable/', None),
```

### Comparing `hdmf_zarr-0.6.0/docs/source/index.rst` & `hdmf_zarr-0.7.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `hdmf_zarr-0.6.0/docs/source/installation.rst` & `hdmf_zarr-0.7.0/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `hdmf_zarr-0.6.0/docs/source/integrating_data_stores.rst` & `hdmf_zarr-0.7.0/docs/source/integrating_data_stores.rst`

 * *Files identical despite different names*

### Comparing `hdmf_zarr-0.6.0/docs/source/overview.rst` & `hdmf_zarr-0.7.0/docs/source/overview.rst`

 * *Files identical despite different names*

### Comparing `hdmf_zarr-0.6.0/docs/source/storage.rst` & `hdmf_zarr-0.7.0/docs/source/storage.rst`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,14 @@
     ============================  ======================================================================================
     name                          Name of the Group in Zarr
     doc                           Zarr attribute ``doc`` on the Zarr group
     groups                        Zarr groups within the Zarr group
     datasets                      Zarr datasets within the Zarr group
     attributes                    Zarr attributes on the Zarr group
     links                         Stored as JSON formatted attributes on the Zarr Group
-    linkable                      Not mapped; Stored in schema only
     quantity                      Not mapped; Number of appearances of the group
     neurodata_type                Attribute ``neurodata_type`` on the Zarr Group
     namespace ID                  Attribute ``namespace`` on the Zarr Group
     object ID                     Attribute ``object_id`` on the Zarr Group
     ============================  ======================================================================================
 
 .. _sec-zarr-storage-groups-reserved:
@@ -85,15 +84,14 @@
     ============================  ======================================================================================================================
     name                          Name of the dataset in Zarr
     doc                           Zarr attribute ``doc`` on the Zarr dataset
     dtype                         Data type of the Zarr dataset (see `dtype mappings`_ table) and stored in the ``zarr_dtype`` reserved attribute
     shape                         Shape of the Zarr dataset if the shape is fixed, otherwise shape defines the maxshape
     dims                          Not mapped
     attributes                    Zarr attributes on the Zarr dataset
-    linkable                      Not mapped; Stored in schema only
     quantity                      Not mapped; Number of appearances of the dataset
     neurodata_type                Attribute ``neurodata_type`` on the Zarr dataset
     namespace ID                  Attribute ``namespace`` on the Zarr dataset
     object ID                     Attribute ``object_id`` on the Zarr dataset
     ============================  ======================================================================================================================
 
 .. note::
@@ -400,11 +398,10 @@
 
 Zarr allows users to consolidate all metadata for groups and arrays within the given store. By default, every file
 will consolidate all metadata within into a single `.zmetadata` file, stored in the root group. This reduces the number of read
 operations when retrieving certain metadata in read mode.
 
 .. note::
 
-    When updating a file, the consolidated metadata will also need to be updated via 
-    `zarr.consolidate_metadata(path)` to ensure the consolidated metadata is consistent 
+    When updating a file, the consolidated metadata will also need to be updated via
+    `zarr.consolidate_metadata(path)` to ensure the consolidated metadata is consistent
     with the file.
-
```

### Comparing `hdmf_zarr-0.6.0/docs/source/figures/gallery_thumbnail_plot_convert_nwb.png` & `hdmf_zarr-0.7.0/docs/source/figures/gallery_thumbnail_plot_convert_nwb.png`

 * *Files identical despite different names*

### Comparing `hdmf_zarr-0.6.0/docs/source/figures/gallery_thumbnail_plot_nwbzarrio.png` & `hdmf_zarr-0.7.0/docs/source/figures/gallery_thumbnail_plot_nwbzarrio.png`

 * *Files identical despite different names*

### Comparing `hdmf_zarr-0.6.0/docs/source/figures/gallery_thumbnail_plot_zarr_dataset_io.png` & `hdmf_zarr-0.7.0/docs/source/figures/gallery_thumbnail_plot_zarr_dataset_io.png`

 * *Files identical despite different names*

### Comparing `hdmf_zarr-0.6.0/docs/source/figures/gallery_thumbnail_plot_zarr_io.png` & `hdmf_zarr-0.7.0/docs/source/figures/gallery_thumbnail_plot_zarr_io.png`

 * *Files identical despite different names*

### Comparing `hdmf_zarr-0.6.0/docs/source/figures/gallery_thumbnails.pptx` & `hdmf_zarr-0.7.0/docs/source/figures/gallery_thumbnails.pptx`

 * *Files identical despite different names*

### Comparing `hdmf_zarr-0.6.0/docs/source/figures/logo_hdmf_zarr.pdf` & `hdmf_zarr-0.7.0/docs/source/figures/logo_hdmf_zarr.pdf`

 * *Files identical despite different names*

### Comparing `hdmf_zarr-0.6.0/docs/source/figures/logo_hdmf_zarr.png` & `hdmf_zarr-0.7.0/docs/source/figures/logo_hdmf_zarr.png`

 * *Files identical despite different names*

### Comparing `hdmf_zarr-0.6.0/docs/source/figures/logo_hdmf_zarr.pptx` & `hdmf_zarr-0.7.0/docs/source/figures/logo_hdmf_zarr.pptx`

 * *Files identical despite different names*

### Comparing `hdmf_zarr-0.6.0/docs/source/figures/logo_hdmf_zarr_iconsize.png` & `hdmf_zarr-0.7.0/docs/source/figures/logo_hdmf_zarr_iconsize.png`

 * *Files identical despite different names*

### Comparing `hdmf_zarr-0.6.0/src/hdmf_zarr/__init__.py` & `hdmf_zarr-0.7.0/src/hdmf_zarr/__init__.py`

 * *Files identical despite different names*

### Comparing `hdmf_zarr-0.6.0/src/hdmf_zarr/_due.py` & `hdmf_zarr-0.7.0/src/hdmf_zarr/_due.py`

 * *Files identical despite different names*

### Comparing `hdmf_zarr-0.6.0/src/hdmf_zarr/backend.py` & `hdmf_zarr-0.7.0/src/hdmf_zarr/backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,16 @@
             return False
 
     @docval({'name': 'path',
              'type': (str, *SUPPORTED_ZARR_STORES),
              'doc': 'the path to the Zarr file or a supported Zarr store'},
             {'name': 'manager', 'type': BuildManager, 'doc': 'the BuildManager to use for I/O', 'default': None},
             {'name': 'mode', 'type': str,
-             'doc': 'the mode to open the Zarr file with, one of ("w", "r", "r+", "a", "w-")'},
+             'doc': 'the mode to open the Zarr file with, one of ("w", "r", "r+", "a", "w-") '
+                    'the mode r- is used to force open without consolidated metadata in read only mode.'},
             {'name': 'synchronizer', 'type': (zarr.ProcessSynchronizer, zarr.ThreadSynchronizer, bool),
              'doc': 'Zarr synchronizer to use for parallel I/O. If set to True a ProcessSynchronizer is used.',
              'default': None},
             {'name': 'object_codec_class', 'type': None,
              'doc': 'Set the numcodec object codec class to be used to encode objects.'
                     'Use numcodecs.pickles.Pickle by default.',
              'default': None},
@@ -156,16 +157,19 @@
 
     def open(self):
         """Open the Zarr file"""
         if self.__file is None:
             # Within zarr, open_consolidated only allows the mode to be 'r' or 'r+'.
             # As a result, when in other modes, the file will not use consolidated metadata.
             if self.__mode not in ['r', 'r+']:
+                # r- is only an internal mode in ZarrIO to force the use of regular open. For Zarr we need to
+                # use the regular mode r when r- is specified
+                mode_to_use = self.__mode if self.__mode != 'r-' else 'r'
                 self.__file = zarr.open(store=self.path,
-                                        mode=self.__mode,
+                                        mode=mode_to_use,
                                         synchronizer=self.__synchronizer,
                                         storage_options=self.__storage_options)
             else:
                 self.__file = self.__open_file_consolidated(store=self.path,
                                                             mode=self.__mode,
                                                             synchronizer=self.__synchronizer,
                                                             storage_options=self.__storage_options)
@@ -474,30 +478,27 @@
                                  mode,
                                  synchronizer=None,
                                  storage_options=None):
         """
         This method will check to see if the metadata has been consolidated.
         If so, use open_consolidated.
         """
-        # self.path can be both a string or a one of the `SUPPORTED_ZARR_STORES`.
-        if isinstance(self.path, str):
-            path = self.path
-        else:
-            path = self.path.path
-
-        if os.path.isfile(path+'/.zmetadata'):
+        # This check is just a safeguard for possible errors in the future. But this should never happen
+        if mode == 'r-':
+            raise ValueError('Mode r- not allowed for reading with consolidated metadata')
+        try:
             return zarr.open_consolidated(store=store,
                                           mode=mode,
                                           synchronizer=synchronizer,
                                           storage_options=storage_options)
-        else:
-            return zarr.open(store=self.path,
-                             mode=self.__mode,
-                             synchronizer=self.__synchronizer,
-                             storage_options=self.__storage_options)
+        except KeyError:  # A KeyError is raised when the '/.zmetadata' does not exist
+            return zarr.open(store=store,
+                             mode=mode,
+                             synchronizer=synchronizer,
+                             storage_options=storage_options)
 
     @docval({'name': 'parent', 'type': Group, 'doc': 'the parent Zarr object'},
             {'name': 'builder', 'type': GroupBuilder, 'doc': 'the GroupBuilder to write'},
             {'name': 'link_data', 'type': bool,
              'doc': 'If not specified otherwise link (True) or copy (False) Zarr Datasets', 'default': True},
             {'name': 'exhaust_dci', 'type': bool,
              'doc': 'exhaust DataChunkIterators one at a time. If False, add ' +
@@ -719,15 +720,17 @@
 
         object_path = zarr_ref.get('path', None)
         if object_path:
             target_name = os.path.basename(object_path)
         else:
             target_name = ROOT_NAME
 
-        target_zarr_obj = self.__open_file_consolidated(source_file, mode='r', storage_options=self.__storage_options)
+        target_zarr_obj = self.__open_file_consolidated(store=source_file,
+                                                        mode='r',
+                                                        storage_options=self.__storage_options)
         if object_path is not None:
             try:
                 target_zarr_obj = target_zarr_obj[object_path]
             except Exception:
                 raise ValueError("Found bad link to object %s in file %s" % (object_path, source_file))
         # Return the create path
         return target_name, target_zarr_obj
```

### Comparing `hdmf_zarr-0.6.0/src/hdmf_zarr/nwb.py` & `hdmf_zarr-0.7.0/src/hdmf_zarr/nwb.py`

 * *Files identical despite different names*

### Comparing `hdmf_zarr-0.6.0/src/hdmf_zarr/utils.py` & `hdmf_zarr-0.7.0/src/hdmf_zarr/utils.py`

 * *Files identical despite different names*

### Comparing `hdmf_zarr-0.6.0/src/hdmf_zarr/zarr_utils.py` & `hdmf_zarr-0.7.0/src/hdmf_zarr/zarr_utils.py`

 * *Files identical despite different names*

### Comparing `hdmf_zarr-0.6.0/tests/unit/base_tests_zarrio.py` & `hdmf_zarr-0.7.0/tests/unit/base_tests_zarrio.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,16 @@
     Class that creates a zarr file containing groups, datasets, and references for
     general purpose testing.
     """
     def setUp(self):
         self.store = "tests/unit/test_io.zarr"
 
     def tearDown(self):
-        shutil.rmtree(self.store)
+        if os.path.exists(self.store):
+            shutil.rmtree(self.store)
 
     def createReferenceBuilder(self):
         data_1 = np.arange(100, 200, 10).reshape(2, 5)
         data_2 = np.arange(0, 200, 10).reshape(4, 5)
         dataset_1 = DatasetBuilder('dataset_1', data_1)
         dataset_2 = DatasetBuilder('dataset_2', data_2)
```

### Comparing `hdmf_zarr-0.6.0/tests/unit/test_fsspec_streaming.py` & `hdmf_zarr-0.7.0/tests/unit/test_fsspec_streaming.py`

 * *Files identical despite different names*

### Comparing `hdmf_zarr-0.6.0/tests/unit/test_io_convert.py` & `hdmf_zarr-0.7.0/tests/unit/test_io_convert.py`

 * *Files identical despite different names*

### Comparing `hdmf_zarr-0.6.0/tests/unit/test_parallel_write.py` & `hdmf_zarr-0.7.0/tests/unit/test_parallel_write.py`

 * *Files identical despite different names*

### Comparing `hdmf_zarr-0.6.0/tests/unit/test_zarrdataio.py` & `hdmf_zarr-0.7.0/tests/unit/test_zarrdataio.py`

 * *Files identical despite different names*

### Comparing `hdmf_zarr-0.6.0/tests/unit/test_zarrio.py` & `hdmf_zarr-0.7.0/tests/unit/test_zarrio.py`

 * *Files 19% similar despite different names*

```diff
@@ -148,7 +148,37 @@
     def test_get_store_path_deep(self):
         self.create_zarr()
         zarr_obj = zarr.open_consolidated(self.store, mode='r')
         store = zarr_obj.store
         path = ZarrIO._ZarrIO__get_store_path(store)
         expected_path = os.path.normpath(os.path.join(CUR_DIR, 'test_io.zarr'))
         self.assertEqual(path, expected_path)
+
+    def test_force_open_without_consolidated(self):
+        """Test that read-mode -r forces a regular read with mode r"""
+        self.create_zarr(consolidate_metadata=True)
+        # Confirm that opening the file 'r' mode indeed uses the consolidated metadata
+        with ZarrIO(self.store, mode='r') as read_io:
+            read_io.open()
+            self.assertIsInstance(read_io.file.store, zarr.storage.ConsolidatedMetadataStore)
+        # Confirm that opening the file IN 'r-' mode indeed forces a regular open without consolidated metadata
+        with ZarrIO(self.store, mode='r-') as read_io:
+            read_io.open()
+            self.assertIsInstance(read_io.file.store, zarr.storage.DirectoryStore)
+
+    def test_force_open_without_consolidated_fails(self):
+        """
+        Test that we indeed can't use '_ZarrIO__open_file_consolidated' function in r- read mode, which
+        is used to force read without consolidated metadata.
+        """
+        self.create_zarr(consolidate_metadata=True)
+        with ZarrIO(self.store, mode='r') as read_io:
+            # Check that using 'r-' fails
+            msg = 'Mode r- not allowed for reading with consolidated metadata'
+            with self.assertRaisesWith(ValueError, msg):
+                read_io._ZarrIO__open_file_consolidated(store=self.store, mode='r-')
+            # Check that using 'r' does not fail
+            try:
+                read_io._ZarrIO__open_file_consolidated(store=self.store, mode='r')
+            except ValueError as e:
+                self.fail("ZarrIO.__open_file_consolidated raised an unexpected ValueError: {}".format(e))
+
```

### Comparing `hdmf_zarr-0.6.0/tests/unit/utils.py` & `hdmf_zarr-0.7.0/tests/unit/utils.py`

 * *Files identical despite different names*

### Comparing `hdmf_zarr-0.6.0/.gitignore` & `hdmf_zarr-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `hdmf_zarr-0.6.0/LICENSE.txt` & `hdmf_zarr-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hdmf_zarr-0.6.0/README.rst` & `hdmf_zarr-0.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `hdmf_zarr-0.6.0/pyproject.toml` & `hdmf_zarr-0.7.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -14,27 +14,28 @@
 license = {text = "BSD"}
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: BSD License",
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: MacOS",
     "Operating System :: Unix",
     "Topic :: Scientific/Engineering :: Medical Science Apps."
 ]
 dependencies = [
     'hdmf>=3.9.0',
     'zarr>=2.11.0',
-    'numpy>=1.24',
+    'numpy>=1.24, <2.0', # pin below 2.0 until HDMF supports numpy 2.0
     'numcodecs>=0.9.1',
     'pynwb>=2.5.0',
     'threadpoolctl>=3.1.0',
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
@@ -57,33 +58,31 @@
 
 [tool.hatch.build.targets.sdist]
 exclude = [".git_archival.txt"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/hdmf_zarr"]
 
-[tool.pytest.ini_options]
-addopts = "--cov --cov-report html"
 
 [tool.codespell]
 skip = "htmlcov,.git,.mypy_cache,.pytest_cache,.coverage,*.pdf,*.svg,venvs,.tox,./docs/_build/*,*.ipynb"
 ignore-words-list = "datas"
 
 [tool.coverage.run]
 branch = true
-source = ["src/"]
-omit = [
-    "src/hdmf_zarr/_due.py",
-]
+source = ["hdmf_zarr"]
 
 [tool.coverage.report]
 exclude_lines = [
     "pragma: no cover",
     "@abstract"
 ]
+omit = [
+    "*/hdmf_zarr/_due.py",
+]
 
 [tool.black]
 line-length = 120
 target-version = ['py38']
 include = '\.pyi?$'
 extend-exclude = '''
 /(
```

### Comparing `hdmf_zarr-0.6.0/PKG-INFO` & `hdmf_zarr-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: hdmf_zarr
-Version: 0.6.0
+Version: 0.7.0
 Summary: A package defining a Zarr I/O backend for HDMF
 Project-URL: Homepage, https://github.com/hdmf-dev/hdmf-zarr
 Project-URL: Bug Tracker, https://github.com/hdmf-dev/hdmf-zarr/issues
 Author-email: Oliver Ruebel <oruebel@lbl.gov>, Matthew Avaylon <mavaylon@lbl.gov>
 License: BSD
 License-File: LICENSE.txt
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,19 +15,20 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.8
 Requires-Dist: hdmf>=3.9.0
 Requires-Dist: numcodecs>=0.9.1
-Requires-Dist: numpy>=1.24
+Requires-Dist: numpy<2.0,>=1.24
 Requires-Dist: pynwb>=2.5.0
 Requires-Dist: threadpoolctl>=3.1.0
 Requires-Dist: zarr>=2.11.0
 Provides-Extra: fsspec
 Requires-Dist: fsspec; extra == 'fsspec'
 Provides-Extra: s3fs
 Requires-Dist: s3fs; extra == 's3fs'
```

