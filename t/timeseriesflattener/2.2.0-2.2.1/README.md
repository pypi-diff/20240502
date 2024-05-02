# Comparing `tmp/timeseriesflattener-2.2.0.tar.gz` & `tmp/timeseriesflattener-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timeseriesflattener-2.2.0.tar", last modified: Tue Apr 30 09:05:45 2024, max compression
+gzip compressed data, was "timeseriesflattener-2.2.1.tar", last modified: Thu May  2 08:14:02 2024, max compression
```

## Comparing `timeseriesflattener-2.2.0.tar` & `timeseriesflattener-2.2.1.tar`

### file list

```diff
@@ -1,214 +1,214 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.674690 timeseriesflattener-2.2.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.610690 timeseriesflattener-2.2.0/.devcontainer/
--rw-r--r--   0 root         (0) root         (0)     1639 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/.devcontainer/devcontainer.json
--rw-r--r--   0 root         (0) root         (0)      148 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/.devcontainer/post-start.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.610690 timeseriesflattener-2.2.0/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.602690 timeseriesflattener-2.2.0/.github/actions/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.614690 timeseriesflattener-2.2.0/.github/actions/test/
--rw-r--r--   0 root         (0) root         (0)      901 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/.github/actions/test/action.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.614690 timeseriesflattener-2.2.0/.github/actions/test_tutorials/
--rw-r--r--   0 root         (0) root         (0)      885 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/.github/actions/test_tutorials/action.yml
--rw-r--r--   0 root         (0) root         (0)      529 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/.github/dependabot.yml
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/.github/pull_request_template.md
--rw-r--r--   0 root         (0) root         (0)     1689 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/.github/recommended_repo_setup.md
--rw-r--r--   0 root         (0) root         (0)      465 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/.github/setup_ci.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.614690 timeseriesflattener-2.2.0/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)      636 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/.github/workflows/benchmark.yml
--rw-r--r--   0 root         (0) root         (0)      720 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/.github/workflows/check_for_rej.yml
--rw-r--r--   0 root         (0) root         (0)      849 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/.github/workflows/dependabot_automerge.yml
--rw-r--r--   0 root         (0) root         (0)      898 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/.github/workflows/documentation.yml
--rw-r--r--   0 root         (0) root         (0)      727 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/.github/workflows/generate_paper_pdf.yml
--rw-r--r--   0 root         (0) root         (0)     1939 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/.github/workflows/main_test_and_release.yml
--rw-r--r--   0 root         (0) root         (0)     1025 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/.github/workflows/pre-commit.yml
--rw-r--r--   0 root         (0) root         (0)     1132 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/.github/workflows/stalebot.yml
--rw-r--r--   0 root         (0) root         (0)      788 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/.github/workflows/static_type_checks.yml
--rw-r--r--   0 root         (0) root         (0)     2885 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/.gitignore
--rw-r--r--   0 root         (0) root         (0)      697 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)        7 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/.python-version
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.614690 timeseriesflattener-2.2.0/.vscode/
--rw-r--r--   0 root         (0) root         (0)      346 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/.vscode/extensions.json
--rw-r--r--   0 root         (0) root         (0)      249 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/.vscode/settings.json
--rw-r--r--   0 root         (0) root         (0)     1373 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/.vscode/tasks.json
--rw-r--r--   0 root         (0) root         (0)     1286 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/.zenodo.json
--rw-r--r--   0 root         (0) root         (0)    73705 2024-04-30 09:05:40.000000 timeseriesflattener-2.2.0/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     5238 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 root         (0) root         (0)     4474 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/CONTRIBUTING.md
--rw-r--r--   0 root         (0) root         (0)     1031 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/Dockerfile
--rw-r--r--   0 root         (0) root         (0)     1087 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      262 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/Makefile
--rw-r--r--   0 root         (0) root         (0)    11507 2024-04-30 09:05:45.674690 timeseriesflattener-2.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7631 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/README.md
--rw-r--r--   0 root         (0) root         (0)     1763 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/citation.cff
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.618690 timeseriesflattener-2.2.0/docs/
--rw-r--r--   0 root         (0) root         (0)      633 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.618690 timeseriesflattener-2.2.0/docs/_static/
--rw-r--r--   0 root         (0) root         (0)    15406 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/docs/_static/favicon.ico
--rw-r--r--   0 root         (0) root         (0)    49714 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/docs/_static/icon.png
--rw-r--r--   0 root         (0) root         (0)    49714 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/docs/_static/icon_dark.png
--rw-r--r--   0 root         (0) root         (0)   424821 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/docs/_static/terminology_figure.png
--rw-r--r--   0 root         (0) root         (0)      291 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/docs/aggregators.rst
--rw-r--r--   0 root         (0) root         (0)     4115 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)     2097 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/docs/faq.rst
--rw-r--r--   0 root         (0) root         (0)     1013 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/docs/feature_specifications.rst
--rw-r--r--   0 root         (0) root         (0)      295 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/docs/flattener.rst
--rw-r--r--   0 root         (0) root         (0)     5165 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)      299 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/docs/installation.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.618690 timeseriesflattener-2.2.0/docs/tutorials/
--rw-r--r--   0 root         (0) root         (0)   128585 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/docs/tutorials/01_basic.ipynb
--rw-r--r--   0 root         (0) root         (0)    40071 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/docs/tutorials/02_advanced.ipynb
--rw-r--r--   0 root         (0) root         (0)    24394 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/docs/tutorials/03_text.ipynb
--rw-r--r--   0 root         (0) root         (0)     5314 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/docs/tutorials/04_from_legacy.ipynb
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.622690 timeseriesflattener-2.2.0/docs/tutorials/img/
--rw-r--r--   0 root         (0) root         (0)    78953 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/docs/tutorials/img/term_a.png
--rw-r--r--   0 root         (0) root         (0)   109486 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/docs/tutorials/img/term_b.png
--rw-r--r--   0 root         (0) root         (0)   107613 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/docs/tutorials/img/term_c.png
--rw-r--r--   0 root         (0) root         (0)   250306 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/docs/tutorials/img/term_d.png
--rw-r--r--   0 root         (0) root         (0)      404 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/docs/tutorials.rst
--rw-r--r--   0 root         (0) root         (0)     1833 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/example.py
--rw-r--r--   0 root         (0) root         (0)    49714 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/icon.png
--rw-r--r--   0 root         (0) root         (0)      426 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/lefthook.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.622690 timeseriesflattener-2.2.0/paper/
--rw-r--r--   0 root         (0) root         (0)    14392 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/paper/paper.bib
--rw-r--r--   0 root         (0) root         (0)     9344 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/paper/paper.md
--rw-r--r--   0 root         (0) root         (0)     4633 2024-04-30 09:05:40.000000 timeseriesflattener-2.2.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     2520 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/requirements-dev.lock
--rw-r--r--   0 root         (0) root         (0)     1474 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/requirements.lock
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-30 09:05:45.674690 timeseriesflattener-2.2.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.622690 timeseriesflattener-2.2.0/src/
--rw-r--r--   0 root         (0) root         (0)     1379 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/conftest.py
--rw-r--r--   0 root         (0) root         (0)     5207 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/test_benchmark.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.622690 timeseriesflattener-2.2.0/src/timeseriesflattener/
--rw-r--r--   0 root         (0) root         (0)      721 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1467 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/_frame_validator.py
--rw-r--r--   0 root         (0) root         (0)     3852 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/_intermediary_frames.py
--rw-r--r--   0 root         (0) root         (0)     3922 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/aggregators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.626690 timeseriesflattener-2.2.0/src/timeseriesflattener/feature_specs/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/feature_specs/__init__.py
--rw-r--r--   0 root         (0) root         (0)      215 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/feature_specs/default_column_names.py
--rw-r--r--   0 root         (0) root         (0)     3708 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/feature_specs/from_legacy.py
--rw-r--r--   0 root         (0) root         (0)     2978 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/feature_specs/meta.py
--rw-r--r--   0 root         (0) root         (0)     2498 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/feature_specs/outcome.py
--rw-r--r--   0 root         (0) root         (0)     1875 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/feature_specs/prediction_times.py
--rw-r--r--   0 root         (0) root         (0)     1389 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/feature_specs/predictor.py
--rw-r--r--   0 root         (0) root         (0)     1434 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/feature_specs/static.py
--rw-r--r--   0 root         (0) root         (0)     1349 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/feature_specs/test_from_legacy.py
--rw-r--r--   0 root         (0) root         (0)     1917 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/feature_specs/test_specs.py
--rw-r--r--   0 root         (0) root         (0)     2144 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/feature_specs/timedelta.py
--rw-r--r--   0 root         (0) root         (0)     1241 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/feature_specs/timestamp_frame.py
--rw-r--r--   0 root         (0) root         (0)     6278 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/flattener.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.626690 timeseriesflattener-2.2.0/src/timeseriesflattener/frame_utilities/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/frame_utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)      477 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/frame_utilities/_horisontally_concat.py
--rw-r--r--   0 root         (0) root         (0)      644 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/frame_utilities/anyframe_to_lazyframe.py
--rw-r--r--   0 root         (0) root         (0)     1049 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/process_spec.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.630690 timeseriesflattener-2.2.0/src/timeseriesflattener/spec_processors/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/spec_processors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1025 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/spec_processors/static.py
--rw-r--r--   0 root         (0) root         (0)    10222 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/spec_processors/temporal.py
--rw-r--r--   0 root         (0) root         (0)     1852 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/spec_processors/test_static.py
--rw-r--r--   0 root         (0) root         (0)    10508 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/spec_processors/test_temporal.py
--rw-r--r--   0 root         (0) root         (0)     1524 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/spec_processors/timedelta.py
--rw-r--r--   0 root         (0) root         (0)     4997 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/test_aggregators.py
--rw-r--r--   0 root         (0) root         (0)    11028 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/test_flattener.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.630690 timeseriesflattener-2.2.0/src/timeseriesflattener/testing/
--rw-r--r--   0 root         (0) root         (0)     1519 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/testing/load_synth_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.630690 timeseriesflattener-2.2.0/src/timeseriesflattener/testing/synth_data_generator/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/testing/synth_data_generator/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5619 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/testing/synth_data_generator/synth_col_generators.py
--rw-r--r--   0 root         (0) root         (0)     2746 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/testing/synth_data_generator/synth_prediction_times_generator.py
--rw-r--r--   0 root         (0) root         (0)     1958 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/testing/synth_data_generator/synth_txt_data_generator.py
--rw-r--r--   0 root         (0) root         (0)      983 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/testing/synth_data_generator/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.602690 timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.602690 timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/flattened/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.630690 timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/
--rw-r--r--   0 root         (0) root         (0)     1494 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py
--rw-r--r--   0 root         (0) root         (0)   864795 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.646690 timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/raw/
--rw-r--r--   0 root         (0) root         (0)      754 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/raw/create_synth_birthdays.py
--rw-r--r--   0 root         (0) root         (0)      744 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/raw/create_synth_prediction_times.py
--rw-r--r--   0 root         (0) root         (0)      830 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_binary.py
--rw-r--r--   0 root         (0) root         (0)      807 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_float.py
--rw-r--r--   0 root         (0) root         (0)      731 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/raw/create_synth_sex.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/raw/create_synth_txt_data.py
--rw-r--r--   0 root         (0) root         (0)   200734 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/raw/synth_birthdays.csv
--rw-r--r--   0 root         (0) root         (0)   248865 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/raw/synth_prediction_times.csv
--rw-r--r--   0 root         (0) root         (0)   268962 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_1.csv
--rw-r--r--   0 root         (0) root         (0)   268904 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_2.csv
--rw-r--r--   0 root         (0) root         (0)  4316151 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_1.csv
--rw-r--r--   0 root         (0) root         (0)  4315816 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_2.csv
--rw-r--r--   0 root         (0) root         (0)    68900 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/raw/synth_sex.csv
--rw-r--r--   0 root         (0) root         (0)    84570 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/raw/synth_text_data.csv
--rw-r--r--   0 root         (0) root         (0)     5511 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/testing/utils_for_testing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.650690 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/
--rw-r--r--   0 root         (0) root         (0)      264 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2855 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/aggregation_fns.py
--rw-r--r--   0 root         (0) root         (0)     1070 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/df_transforms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.650690 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/feature_cache/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/feature_cache/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1980 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/feature_cache/abstract_feature_cache.py
--rw-r--r--   0 root         (0) root         (0)     6112 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/feature_cache/cache_to_disk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.650690 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/feature_specs/
--rw-r--r--   0 root         (0) root         (0)     5535 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/feature_specs/group_specs.py
--rw-r--r--   0 root         (0) root         (0)     7823 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/feature_specs/single_specs.py
--rw-r--r--   0 root         (0) root         (0)    35049 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/flattened_dataset.py
--rw-r--r--   0 root         (0) root         (0)     2150 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/flattened_ds_validator.py
--rw-r--r--   0 root         (0) root         (0)     2242 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/logger.py
--rw-r--r--   0 root         (0) root         (0)     7524 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/misc_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.650690 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/
--rw-r--r--   0 root         (0) root         (0)     2981 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/load_synth_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.650690 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/synth_data_generator/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/synth_data_generator/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5527 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/synth_data_generator/synth_col_generators.py
--rw-r--r--   0 root         (0) root         (0)     2697 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/synth_data_generator/synth_prediction_times_generator.py
--rw-r--r--   0 root         (0) root         (0)     1962 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/synth_data_generator/synth_txt_data_generator.py
--rw-r--r--   0 root         (0) root         (0)      923 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/synth_data_generator/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.606690 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.606690 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/flattened/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.650690 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/flattened/generated_with_outcome/
--rw-r--r--   0 root         (0) root         (0)     1461 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py
--rw-r--r--   0 root         (0) root         (0)   864795 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.654690 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/models/
--rw-r--r--   0 root         (0) root         (0)     1877 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/models/create_bow_and_pca_model.py
--rw-r--r--   0 root         (0) root         (0)    25543 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/models/synth_bow_model.pkl
--rw-r--r--   0 root         (0) root         (0)     1015 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/models/synth_pca_model.pkl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.666690 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/raw/
--rw-r--r--   0 root         (0) root         (0)      709 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_prediction_times.py
--rw-r--r--   0 root         (0) root         (0)      795 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_raw_binary.py
--rw-r--r--   0 root         (0) root         (0)      772 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_raw_float.py
--rw-r--r--   0 root         (0) root         (0)      696 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_sex.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_txt_data.py
--rw-r--r--   0 root         (0) root         (0)   200734 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/raw/synth_birthdays.csv
--rw-r--r--   0 root         (0) root         (0)   248865 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/raw/synth_prediction_times.csv
--rw-r--r--   0 root         (0) root         (0)   268962 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_binary_1.csv
--rw-r--r--   0 root         (0) root         (0)   268904 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_binary_2.csv
--rw-r--r--   0 root         (0) root         (0)  4316151 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_float_1.csv
--rw-r--r--   0 root         (0) root         (0)  4315816 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_float_2.csv
--rw-r--r--   0 root         (0) root         (0)    68900 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/raw/synth_sex.csv
--rw-r--r--   0 root         (0) root         (0)    84570 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/raw/synth_text_data.csv
--rw-r--r--   0 root         (0) root         (0)     5446 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/utils_for_testing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.670690 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.670690 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/tests/test_feature_cache/
--rw-r--r--   0 root         (0) root         (0)     3232 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/tests/test_feature_cache/test_cache_to_disk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.670690 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13595 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_aggregation_fns.py
--rw-r--r--   0 root         (0) root         (0)     1295 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_df_transforms.py
--rw-r--r--   0 root         (0) root         (0)     3399 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_feature_spec_objects.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.670690 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23392 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py
--rw-r--r--   0 root         (0) root         (0)     2663 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py
--rw-r--r--   0 root         (0) root         (0)     2308 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py
--rw-r--r--   0 root         (0) root         (0)     2321 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py
--rw-r--r--   0 root         (0) root         (0)     5796 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py
--rw-r--r--   0 root         (0) root         (0)     2420 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.670690 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/utils/
--rw-r--r--   0 root         (0) root         (0)      984 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/src/timeseriesflattener/v1/utils/pydantic_basemodel.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 09:05:45.670690 timeseriesflattener-2.2.0/src/timeseriesflattener.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11507 2024-04-30 09:05:45.000000 timeseriesflattener-2.2.0/src/timeseriesflattener.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8537 2024-04-30 09:05:45.000000 timeseriesflattener-2.2.0/src/timeseriesflattener.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 09:05:45.000000 timeseriesflattener-2.2.0/src/timeseriesflattener.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      650 2024-04-30 09:05:45.000000 timeseriesflattener-2.2.0/src/timeseriesflattener.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       44 2024-04-30 09:05:45.000000 timeseriesflattener-2.2.0/src/timeseriesflattener.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     8330 2024-04-30 09:05:39.000000 timeseriesflattener-2.2.0/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:14:02.199005 timeseriesflattener-2.2.1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:14:02.135005 timeseriesflattener-2.2.1/.devcontainer/
+-rw-r--r--   0 root         (0) root         (0)     1639 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/.devcontainer/devcontainer.json
+-rw-r--r--   0 root         (0) root         (0)      148 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/.devcontainer/post-start.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:14:02.135005 timeseriesflattener-2.2.1/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:14:02.123005 timeseriesflattener-2.2.1/.github/actions/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:14:02.135005 timeseriesflattener-2.2.1/.github/actions/test/
+-rw-r--r--   0 root         (0) root         (0)      901 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/.github/actions/test/action.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:14:02.135005 timeseriesflattener-2.2.1/.github/actions/test_tutorials/
+-rw-r--r--   0 root         (0) root         (0)      885 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/.github/actions/test_tutorials/action.yml
+-rw-r--r--   0 root         (0) root         (0)      529 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/.github/dependabot.yml
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/.github/pull_request_template.md
+-rw-r--r--   0 root         (0) root         (0)     1689 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/.github/recommended_repo_setup.md
+-rw-r--r--   0 root         (0) root         (0)      465 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/.github/setup_ci.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:14:02.139005 timeseriesflattener-2.2.1/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)      636 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/.github/workflows/benchmark.yml
+-rw-r--r--   0 root         (0) root         (0)      720 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/.github/workflows/check_for_rej.yml
+-rw-r--r--   0 root         (0) root         (0)      849 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/.github/workflows/dependabot_automerge.yml
+-rw-r--r--   0 root         (0) root         (0)      898 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/.github/workflows/documentation.yml
+-rw-r--r--   0 root         (0) root         (0)      727 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/.github/workflows/generate_paper_pdf.yml
+-rw-r--r--   0 root         (0) root         (0)     1939 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/.github/workflows/main_test_and_release.yml
+-rw-r--r--   0 root         (0) root         (0)     1025 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/.github/workflows/pre-commit.yml
+-rw-r--r--   0 root         (0) root         (0)     1132 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/.github/workflows/stalebot.yml
+-rw-r--r--   0 root         (0) root         (0)      788 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/.github/workflows/static_type_checks.yml
+-rw-r--r--   0 root         (0) root         (0)     2885 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      697 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)        7 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/.python-version
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:14:02.139005 timeseriesflattener-2.2.1/.vscode/
+-rw-r--r--   0 root         (0) root         (0)      346 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/.vscode/extensions.json
+-rw-r--r--   0 root         (0) root         (0)      249 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/.vscode/settings.json
+-rw-r--r--   0 root         (0) root         (0)     1373 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/.vscode/tasks.json
+-rw-r--r--   0 root         (0) root         (0)     1286 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/.zenodo.json
+-rw-r--r--   0 root         (0) root         (0)    73904 2024-05-02 08:13:56.000000 timeseriesflattener-2.2.1/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     5238 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 root         (0) root         (0)     4474 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)     1031 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)     1087 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      262 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/Makefile
+-rw-r--r--   0 root         (0) root         (0)    11525 2024-05-02 08:14:02.199005 timeseriesflattener-2.2.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7649 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/README.md
+-rw-r--r--   0 root         (0) root         (0)     1763 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/citation.cff
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:14:02.139005 timeseriesflattener-2.2.1/docs/
+-rw-r--r--   0 root         (0) root         (0)      633 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:14:02.143005 timeseriesflattener-2.2.1/docs/_static/
+-rw-r--r--   0 root         (0) root         (0)    15406 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/docs/_static/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)    49714 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/docs/_static/icon.png
+-rw-r--r--   0 root         (0) root         (0)    49714 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/docs/_static/icon_dark.png
+-rw-r--r--   0 root         (0) root         (0)   424821 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/docs/_static/terminology_figure.png
+-rw-r--r--   0 root         (0) root         (0)      291 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/docs/aggregators.rst
+-rw-r--r--   0 root         (0) root         (0)     4115 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)     2097 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/docs/faq.rst
+-rw-r--r--   0 root         (0) root         (0)     1013 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/docs/feature_specifications.rst
+-rw-r--r--   0 root         (0) root         (0)      295 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/docs/flattener.rst
+-rw-r--r--   0 root         (0) root         (0)     5165 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)      299 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/docs/installation.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:14:02.143005 timeseriesflattener-2.2.1/docs/tutorials/
+-rw-r--r--   0 root         (0) root         (0)   128585 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/docs/tutorials/01_basic.ipynb
+-rw-r--r--   0 root         (0) root         (0)    40071 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/docs/tutorials/02_advanced.ipynb
+-rw-r--r--   0 root         (0) root         (0)    24394 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/docs/tutorials/03_text.ipynb
+-rw-r--r--   0 root         (0) root         (0)     5314 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/docs/tutorials/04_from_legacy.ipynb
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:14:02.143005 timeseriesflattener-2.2.1/docs/tutorials/img/
+-rw-r--r--   0 root         (0) root         (0)    78953 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/docs/tutorials/img/term_a.png
+-rw-r--r--   0 root         (0) root         (0)   109486 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/docs/tutorials/img/term_b.png
+-rw-r--r--   0 root         (0) root         (0)   107613 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/docs/tutorials/img/term_c.png
+-rw-r--r--   0 root         (0) root         (0)   250306 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/docs/tutorials/img/term_d.png
+-rw-r--r--   0 root         (0) root         (0)      404 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/docs/tutorials.rst
+-rw-r--r--   0 root         (0) root         (0)     1833 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/example.py
+-rw-r--r--   0 root         (0) root         (0)    49714 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/icon.png
+-rw-r--r--   0 root         (0) root         (0)      426 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/lefthook.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:14:02.147005 timeseriesflattener-2.2.1/paper/
+-rw-r--r--   0 root         (0) root         (0)    14392 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/paper/paper.bib
+-rw-r--r--   0 root         (0) root         (0)     9344 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/paper/paper.md
+-rw-r--r--   0 root         (0) root         (0)     4633 2024-05-02 08:13:56.000000 timeseriesflattener-2.2.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2520 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/requirements-dev.lock
+-rw-r--r--   0 root         (0) root         (0)     1474 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/requirements.lock
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-02 08:14:02.199005 timeseriesflattener-2.2.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:14:02.147005 timeseriesflattener-2.2.1/src/
+-rw-r--r--   0 root         (0) root         (0)     1379 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     5207 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/test_benchmark.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:14:02.147005 timeseriesflattener-2.2.1/src/timeseriesflattener/
+-rw-r--r--   0 root         (0) root         (0)      721 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1467 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/_frame_validator.py
+-rw-r--r--   0 root         (0) root         (0)     3852 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/_intermediary_frames.py
+-rw-r--r--   0 root         (0) root         (0)     3922 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/aggregators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:14:02.151005 timeseriesflattener-2.2.1/src/timeseriesflattener/feature_specs/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/feature_specs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      215 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/feature_specs/default_column_names.py
+-rw-r--r--   0 root         (0) root         (0)     3708 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/feature_specs/from_legacy.py
+-rw-r--r--   0 root         (0) root         (0)     2978 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/feature_specs/meta.py
+-rw-r--r--   0 root         (0) root         (0)     2498 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/feature_specs/outcome.py
+-rw-r--r--   0 root         (0) root         (0)     1875 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/feature_specs/prediction_times.py
+-rw-r--r--   0 root         (0) root         (0)     1389 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/feature_specs/predictor.py
+-rw-r--r--   0 root         (0) root         (0)     1434 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/feature_specs/static.py
+-rw-r--r--   0 root         (0) root         (0)     1349 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/feature_specs/test_from_legacy.py
+-rw-r--r--   0 root         (0) root         (0)     1917 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/feature_specs/test_specs.py
+-rw-r--r--   0 root         (0) root         (0)     2144 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/feature_specs/timedelta.py
+-rw-r--r--   0 root         (0) root         (0)     1241 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/feature_specs/timestamp_frame.py
+-rw-r--r--   0 root         (0) root         (0)     6436 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/flattener.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:14:02.151005 timeseriesflattener-2.2.1/src/timeseriesflattener/frame_utilities/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/frame_utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      477 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/frame_utilities/_horisontally_concat.py
+-rw-r--r--   0 root         (0) root         (0)      644 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/frame_utilities/anyframe_to_lazyframe.py
+-rw-r--r--   0 root         (0) root         (0)     1049 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/process_spec.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:14:02.151005 timeseriesflattener-2.2.1/src/timeseriesflattener/spec_processors/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/spec_processors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1025 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/spec_processors/static.py
+-rw-r--r--   0 root         (0) root         (0)    10222 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/spec_processors/temporal.py
+-rw-r--r--   0 root         (0) root         (0)     1852 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/spec_processors/test_static.py
+-rw-r--r--   0 root         (0) root         (0)    10508 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/spec_processors/test_temporal.py
+-rw-r--r--   0 root         (0) root         (0)     1524 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/spec_processors/timedelta.py
+-rw-r--r--   0 root         (0) root         (0)     4997 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/test_aggregators.py
+-rw-r--r--   0 root         (0) root         (0)    12792 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/test_flattener.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:14:02.155005 timeseriesflattener-2.2.1/src/timeseriesflattener/testing/
+-rw-r--r--   0 root         (0) root         (0)     1519 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/testing/load_synth_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:14:02.155005 timeseriesflattener-2.2.1/src/timeseriesflattener/testing/synth_data_generator/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/testing/synth_data_generator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5619 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/testing/synth_data_generator/synth_col_generators.py
+-rw-r--r--   0 root         (0) root         (0)     2746 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/testing/synth_data_generator/synth_prediction_times_generator.py
+-rw-r--r--   0 root         (0) root         (0)     1958 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/testing/synth_data_generator/synth_txt_data_generator.py
+-rw-r--r--   0 root         (0) root         (0)      983 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/testing/synth_data_generator/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:14:02.127004 timeseriesflattener-2.2.1/src/timeseriesflattener/testing/test_data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:14:02.127004 timeseriesflattener-2.2.1/src/timeseriesflattener/testing/test_data/flattened/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:14:02.155005 timeseriesflattener-2.2.1/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/
+-rw-r--r--   0 root         (0) root         (0)     1494 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py
+-rw-r--r--   0 root         (0) root         (0)   864795 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:14:02.171005 timeseriesflattener-2.2.1/src/timeseriesflattener/testing/test_data/raw/
+-rw-r--r--   0 root         (0) root         (0)      754 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/testing/test_data/raw/create_synth_birthdays.py
+-rw-r--r--   0 root         (0) root         (0)      744 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/testing/test_data/raw/create_synth_prediction_times.py
+-rw-r--r--   0 root         (0) root         (0)      830 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_binary.py
+-rw-r--r--   0 root         (0) root         (0)      807 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_float.py
+-rw-r--r--   0 root         (0) root         (0)      731 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/testing/test_data/raw/create_synth_sex.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/testing/test_data/raw/create_synth_txt_data.py
+-rw-r--r--   0 root         (0) root         (0)   200734 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/testing/test_data/raw/synth_birthdays.csv
+-rw-r--r--   0 root         (0) root         (0)   248865 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/testing/test_data/raw/synth_prediction_times.csv
+-rw-r--r--   0 root         (0) root         (0)   268962 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_1.csv
+-rw-r--r--   0 root         (0) root         (0)   268904 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_2.csv
+-rw-r--r--   0 root         (0) root         (0)  4316151 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_1.csv
+-rw-r--r--   0 root         (0) root         (0)  4315816 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_2.csv
+-rw-r--r--   0 root         (0) root         (0)    68900 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/testing/test_data/raw/synth_sex.csv
+-rw-r--r--   0 root         (0) root         (0)    84570 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/testing/test_data/raw/synth_text_data.csv
+-rw-r--r--   0 root         (0) root         (0)     5511 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/testing/utils_for_testing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:14:02.171005 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/
+-rw-r--r--   0 root         (0) root         (0)      264 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2855 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/aggregation_fns.py
+-rw-r--r--   0 root         (0) root         (0)     1070 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/df_transforms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:14:02.175005 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/feature_cache/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/feature_cache/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1980 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/feature_cache/abstract_feature_cache.py
+-rw-r--r--   0 root         (0) root         (0)     6112 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/feature_cache/cache_to_disk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:14:02.175005 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/feature_specs/
+-rw-r--r--   0 root         (0) root         (0)     5535 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/feature_specs/group_specs.py
+-rw-r--r--   0 root         (0) root         (0)     7823 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/feature_specs/single_specs.py
+-rw-r--r--   0 root         (0) root         (0)    35049 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/flattened_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     2150 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/flattened_ds_validator.py
+-rw-r--r--   0 root         (0) root         (0)     2242 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/logger.py
+-rw-r--r--   0 root         (0) root         (0)     7524 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/misc_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:14:02.175005 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/testing/
+-rw-r--r--   0 root         (0) root         (0)     2981 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/testing/load_synth_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:14:02.175005 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/testing/synth_data_generator/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/testing/synth_data_generator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5527 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/testing/synth_data_generator/synth_col_generators.py
+-rw-r--r--   0 root         (0) root         (0)     2697 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/testing/synth_data_generator/synth_prediction_times_generator.py
+-rw-r--r--   0 root         (0) root         (0)     1962 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/testing/synth_data_generator/synth_txt_data_generator.py
+-rw-r--r--   0 root         (0) root         (0)      923 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/testing/synth_data_generator/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:14:02.131005 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/testing/test_data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:14:02.131005 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/testing/test_data/flattened/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:14:02.175005 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/testing/test_data/flattened/generated_with_outcome/
+-rw-r--r--   0 root         (0) root         (0)     1461 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py
+-rw-r--r--   0 root         (0) root         (0)   864795 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:14:02.179005 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/testing/test_data/models/
+-rw-r--r--   0 root         (0) root         (0)     1877 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/testing/test_data/models/create_bow_and_pca_model.py
+-rw-r--r--   0 root         (0) root         (0)    25543 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/testing/test_data/models/synth_bow_model.pkl
+-rw-r--r--   0 root         (0) root         (0)     1015 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/testing/test_data/models/synth_pca_model.pkl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:14:02.191005 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/testing/test_data/raw/
+-rw-r--r--   0 root         (0) root         (0)      709 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_prediction_times.py
+-rw-r--r--   0 root         (0) root         (0)      795 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_raw_binary.py
+-rw-r--r--   0 root         (0) root         (0)      772 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_raw_float.py
+-rw-r--r--   0 root         (0) root         (0)      696 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_sex.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_txt_data.py
+-rw-r--r--   0 root         (0) root         (0)   200734 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/testing/test_data/raw/synth_birthdays.csv
+-rw-r--r--   0 root         (0) root         (0)   248865 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/testing/test_data/raw/synth_prediction_times.csv
+-rw-r--r--   0 root         (0) root         (0)   268962 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_binary_1.csv
+-rw-r--r--   0 root         (0) root         (0)   268904 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_binary_2.csv
+-rw-r--r--   0 root         (0) root         (0)  4316151 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_float_1.csv
+-rw-r--r--   0 root         (0) root         (0)  4315816 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_float_2.csv
+-rw-r--r--   0 root         (0) root         (0)    68900 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/testing/test_data/raw/synth_sex.csv
+-rw-r--r--   0 root         (0) root         (0)    84570 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/testing/test_data/raw/synth_text_data.csv
+-rw-r--r--   0 root         (0) root         (0)     5446 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/testing/utils_for_testing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:14:02.195006 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:14:02.195006 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/tests/test_feature_cache/
+-rw-r--r--   0 root         (0) root         (0)     3232 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/tests/test_feature_cache/test_cache_to_disk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:14:02.195006 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/tests/test_timeseriesflattener/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/tests/test_timeseriesflattener/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13595 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_aggregation_fns.py
+-rw-r--r--   0 root         (0) root         (0)     1295 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_df_transforms.py
+-rw-r--r--   0 root         (0) root         (0)     3399 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_feature_spec_objects.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:14:02.195006 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23392 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py
+-rw-r--r--   0 root         (0) root         (0)     2663 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py
+-rw-r--r--   0 root         (0) root         (0)     2308 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py
+-rw-r--r--   0 root         (0) root         (0)     2321 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py
+-rw-r--r--   0 root         (0) root         (0)     5796 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     2420 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:14:02.195006 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/utils/
+-rw-r--r--   0 root         (0) root         (0)      984 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/src/timeseriesflattener/v1/utils/pydantic_basemodel.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 08:14:02.195006 timeseriesflattener-2.2.1/src/timeseriesflattener.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11525 2024-05-02 08:14:02.000000 timeseriesflattener-2.2.1/src/timeseriesflattener.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8537 2024-05-02 08:14:02.000000 timeseriesflattener-2.2.1/src/timeseriesflattener.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 08:14:02.000000 timeseriesflattener-2.2.1/src/timeseriesflattener.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      650 2024-05-02 08:14:02.000000 timeseriesflattener-2.2.1/src/timeseriesflattener.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2024-05-02 08:14:02.000000 timeseriesflattener-2.2.1/src/timeseriesflattener.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     8330 2024-05-02 08:13:55.000000 timeseriesflattener-2.2.1/tasks.py
```

### Comparing `timeseriesflattener-2.2.0/.devcontainer/devcontainer.json` & `timeseriesflattener-2.2.1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/.github/actions/test/action.yml` & `timeseriesflattener-2.2.1/.github/actions/test/action.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/.github/actions/test_tutorials/action.yml` & `timeseriesflattener-2.2.1/.github/actions/test_tutorials/action.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/.github/dependabot.yml` & `timeseriesflattener-2.2.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/.github/recommended_repo_setup.md` & `timeseriesflattener-2.2.1/.github/recommended_repo_setup.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/.github/workflows/benchmark.yml` & `timeseriesflattener-2.2.1/.github/workflows/benchmark.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/.github/workflows/check_for_rej.yml` & `timeseriesflattener-2.2.1/.github/workflows/check_for_rej.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/.github/workflows/dependabot_automerge.yml` & `timeseriesflattener-2.2.1/.github/workflows/dependabot_automerge.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/.github/workflows/documentation.yml` & `timeseriesflattener-2.2.1/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/.github/workflows/generate_paper_pdf.yml` & `timeseriesflattener-2.2.1/.github/workflows/generate_paper_pdf.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/.github/workflows/main_test_and_release.yml` & `timeseriesflattener-2.2.1/.github/workflows/main_test_and_release.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/.github/workflows/pre-commit.yml` & `timeseriesflattener-2.2.1/.github/workflows/pre-commit.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/.github/workflows/stalebot.yml` & `timeseriesflattener-2.2.1/.github/workflows/stalebot.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/.github/workflows/static_type_checks.yml` & `timeseriesflattener-2.2.1/.github/workflows/static_type_checks.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/.gitignore` & `timeseriesflattener-2.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/.pre-commit-config.yaml` & `timeseriesflattener-2.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/.vscode/tasks.json` & `timeseriesflattener-2.2.1/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/.zenodo.json` & `timeseriesflattener-2.2.1/.zenodo.json`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/CHANGELOG.md` & `timeseriesflattener-2.2.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v2.2.1 (2024-05-02)
+
+### Fix
+
+* Scrambled features with step size ([`6bdddbd`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/6bdddbdf975b25cee0e37398ea58ac6ba86f2e77))
+
 ## v2.2.0 (2024-04-30)
 
 ### Feature
 
 * Bump release ([`879e752`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/879e752928808f8c3927808cab6a2f9a80a85610))
 
 ## v2.1.2 (2024-04-18)
```

### Comparing `timeseriesflattener-2.2.0/CODE_OF_CONDUCT.md` & `timeseriesflattener-2.2.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/CONTRIBUTING.md` & `timeseriesflattener-2.2.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/Dockerfile` & `timeseriesflattener-2.2.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/LICENSE` & `timeseriesflattener-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/PKG-INFO` & `timeseriesflattener-2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timeseriesflattener
-Version: 2.2.0
+Version: 2.2.1
 Summary: A package for converting time series data from e.g. electronic health records into wide format data.
 Author: Kenneth Enevoldsen
 Author-email: Lasse Hansen <lasseh0310@gmail.com>, Jakob Grøhn Damgaard <bokajgd@gmail.com>, Martin Bernstorff <martinbernstorff@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 PSYCOP Group, Aarhus University
         
@@ -115,19 +115,19 @@
     {"id": [1, 1, 2], "date": ["2020-01-01", "2020-02-01", "2020-02-01"]}
 )
 # Load a dataframe with raw values you wish to aggregate as predictors
 predictor_df = pl.DataFrame(
     {
         "id": [1, 1, 1, 2],
         "date": ["2020-01-15", "2019-12-10", "2019-12-15", "2020-01-02"],
-        "value": [1, 2, 3, 4],
+        "predictor_value": [1, 2, 3, 4],
     }
 )
 # Load a dataframe specifying when the outcome occurs
-outcome_df = pl.DataFrame({"id": [1], "date": ["2020-03-01"], "value": [1]})
+outcome_df = pl.DataFrame({"id": [1], "date": ["2020-03-01"], "outcome_value": [1]})
 
 # Specify how to aggregate the predictors and define the outcome
 from timeseriesflattener import (
     MaxAggregator,
     MinAggregator,
     OutcomeSpec,
     PredictionTimeFrame,
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: timeseriesflattener Version: 2.2.0 Summary: A
+Metadata-Version: 2.1 Name: timeseriesflattener Version: 2.2.1 Summary: A
 package for converting time series data from e.g. electronic health records
 into wide format data. Author: Kenneth Enevoldsen Author-email: Lasse Hansen
 gmail.com>, Jakob GrÃ¸hn Damgaard
 gmail.com>, Martin Bernstorff
 gmail.com> License: MIT License Copyright (c) 2022 PSYCOP Group, Aarhus
 University Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
@@ -77,18 +77,18 @@
 timeseriesflattener simply install it using pip by running the following line
 in your terminal: ``` pip install timeseriesflattener ``` ## â¡ Quick start
 ```py import datetime as dt import numpy as np import polars as pl # Load a
 dataframe with times you wish to make a prediction prediction_times_df =
 pl.DataFrame( {"id": [1, 1, 2], "date": ["2020-01-01", "2020-02-01", "2020-02-
 01"]} ) # Load a dataframe with raw values you wish to aggregate as predictors
 predictor_df = pl.DataFrame( { "id": [1, 1, 1, 2], "date": ["2020-01-15",
-"2019-12-10", "2019-12-15", "2020-01-02"], "value": [1, 2, 3, 4], } ) # Load a
-dataframe specifying when the outcome occurs outcome_df = pl.DataFrame({"id":
-[1], "date": ["2020-03-01"], "value": [1]}) # Specify how to aggregate the
-predictors and define the outcome from timeseriesflattener import
+"2019-12-10", "2019-12-15", "2020-01-02"], "predictor_value": [1, 2, 3, 4], } )
+# Load a dataframe specifying when the outcome occurs outcome_df = pl.DataFrame
+({"id": [1], "date": ["2020-03-01"], "outcome_value": [1]}) # Specify how to
+aggregate the predictors and define the outcome from timeseriesflattener import
 ( MaxAggregator, MinAggregator, OutcomeSpec, PredictionTimeFrame,
 PredictorSpec, ValueFrame, ) predictor_spec = PredictorSpec
 ( value_frame=ValueFrame( init_df=predictor_df.lazy(), entity_id_col_name="id",
 value_timestamp_col_name="date" ), lookbehind_distances=[dt.timedelta(days=1)],
 aggregators=[MaxAggregator(), MinAggregator()], fallback=np.nan,
 column_prefix="pred", ) outcome_spec = OutcomeSpec( value_frame=ValueFrame
 ( init_df=outcome_df.lazy(), entity_id_col_name="id",
```

### Comparing `timeseriesflattener-2.2.0/README.md` & `timeseriesflattener-2.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -36,19 +36,19 @@
     {"id": [1, 1, 2], "date": ["2020-01-01", "2020-02-01", "2020-02-01"]}
 )
 # Load a dataframe with raw values you wish to aggregate as predictors
 predictor_df = pl.DataFrame(
     {
         "id": [1, 1, 1, 2],
         "date": ["2020-01-15", "2019-12-10", "2019-12-15", "2020-01-02"],
-        "value": [1, 2, 3, 4],
+        "predictor_value": [1, 2, 3, 4],
     }
 )
 # Load a dataframe specifying when the outcome occurs
-outcome_df = pl.DataFrame({"id": [1], "date": ["2020-03-01"], "value": [1]})
+outcome_df = pl.DataFrame({"id": [1], "date": ["2020-03-01"], "outcome_value": [1]})
 
 # Specify how to aggregate the predictors and define the outcome
 from timeseriesflattener import (
     MaxAggregator,
     MinAggregator,
     OutcomeSpec,
     PredictionTimeFrame,
```

#### html2text {}

```diff
@@ -27,18 +27,18 @@
 timeseriesflattener simply install it using pip by running the following line
 in your terminal: ``` pip install timeseriesflattener ``` ## â¡ Quick start
 ```py import datetime as dt import numpy as np import polars as pl # Load a
 dataframe with times you wish to make a prediction prediction_times_df =
 pl.DataFrame( {"id": [1, 1, 2], "date": ["2020-01-01", "2020-02-01", "2020-02-
 01"]} ) # Load a dataframe with raw values you wish to aggregate as predictors
 predictor_df = pl.DataFrame( { "id": [1, 1, 1, 2], "date": ["2020-01-15",
-"2019-12-10", "2019-12-15", "2020-01-02"], "value": [1, 2, 3, 4], } ) # Load a
-dataframe specifying when the outcome occurs outcome_df = pl.DataFrame({"id":
-[1], "date": ["2020-03-01"], "value": [1]}) # Specify how to aggregate the
-predictors and define the outcome from timeseriesflattener import
+"2019-12-10", "2019-12-15", "2020-01-02"], "predictor_value": [1, 2, 3, 4], } )
+# Load a dataframe specifying when the outcome occurs outcome_df = pl.DataFrame
+({"id": [1], "date": ["2020-03-01"], "outcome_value": [1]}) # Specify how to
+aggregate the predictors and define the outcome from timeseriesflattener import
 ( MaxAggregator, MinAggregator, OutcomeSpec, PredictionTimeFrame,
 PredictorSpec, ValueFrame, ) predictor_spec = PredictorSpec
 ( value_frame=ValueFrame( init_df=predictor_df.lazy(), entity_id_col_name="id",
 value_timestamp_col_name="date" ), lookbehind_distances=[dt.timedelta(days=1)],
 aggregators=[MaxAggregator(), MinAggregator()], fallback=np.nan,
 column_prefix="pred", ) outcome_spec = OutcomeSpec( value_frame=ValueFrame
 ( init_df=outcome_df.lazy(), entity_id_col_name="id",
```

### Comparing `timeseriesflattener-2.2.0/citation.cff` & `timeseriesflattener-2.2.1/citation.cff`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/docs/Makefile` & `timeseriesflattener-2.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/docs/_static/favicon.ico` & `timeseriesflattener-2.2.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/docs/_static/icon.png` & `timeseriesflattener-2.2.1/docs/_static/icon.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/docs/_static/icon_dark.png` & `timeseriesflattener-2.2.1/docs/_static/icon_dark.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/docs/_static/terminology_figure.png` & `timeseriesflattener-2.2.1/docs/_static/terminology_figure.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/docs/conf.py` & `timeseriesflattener-2.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/docs/faq.rst` & `timeseriesflattener-2.2.1/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/docs/feature_specifications.rst` & `timeseriesflattener-2.2.1/docs/feature_specifications.rst`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/docs/index.rst` & `timeseriesflattener-2.2.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/docs/tutorials/01_basic.ipynb` & `timeseriesflattener-2.2.1/docs/tutorials/01_basic.ipynb`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/docs/tutorials/02_advanced.ipynb` & `timeseriesflattener-2.2.1/docs/tutorials/02_advanced.ipynb`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/docs/tutorials/03_text.ipynb` & `timeseriesflattener-2.2.1/docs/tutorials/03_text.ipynb`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/docs/tutorials/04_from_legacy.ipynb` & `timeseriesflattener-2.2.1/docs/tutorials/04_from_legacy.ipynb`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/docs/tutorials/img/term_a.png` & `timeseriesflattener-2.2.1/docs/tutorials/img/term_a.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/docs/tutorials/img/term_b.png` & `timeseriesflattener-2.2.1/docs/tutorials/img/term_b.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/docs/tutorials/img/term_c.png` & `timeseriesflattener-2.2.1/docs/tutorials/img/term_c.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/docs/tutorials/img/term_d.png` & `timeseriesflattener-2.2.1/docs/tutorials/img/term_d.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/example.py` & `timeseriesflattener-2.2.1/example.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/icon.png` & `timeseriesflattener-2.2.1/icon.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/paper/paper.bib` & `timeseriesflattener-2.2.1/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/paper/paper.md` & `timeseriesflattener-2.2.1/paper/paper.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/pyproject.toml` & `timeseriesflattener-2.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "timeseriesflattener"
-version = "2.2.0"
+version = "2.2.1"
 authors = [
   { name = "Lasse Hansen", email = "lasseh0310@gmail.com" },
   { name = "Jakob Grøhn Damgaard", email = "bokajgd@gmail.com" },
   { name = "Kenneth Enevoldsen" },
   { name = "Martin Bernstorff", email = "martinbernstorff@gmail.com" },
 ]
 description = "A package for converting time series data from e.g. electronic health records into wide format data."
```

### Comparing `timeseriesflattener-2.2.0/requirements-dev.lock` & `timeseriesflattener-2.2.1/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/requirements.lock` & `timeseriesflattener-2.2.1/requirements.lock`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/conftest.py` & `timeseriesflattener-2.2.1/src/conftest.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/test_benchmark.py` & `timeseriesflattener-2.2.1/src/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/__init__.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/__init__.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/_frame_validator.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/_frame_validator.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/_intermediary_frames.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/_intermediary_frames.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/aggregators.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/aggregators.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/feature_specs/from_legacy.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/feature_specs/from_legacy.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/feature_specs/meta.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/feature_specs/meta.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/feature_specs/outcome.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/feature_specs/outcome.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/feature_specs/prediction_times.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/feature_specs/prediction_times.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/feature_specs/predictor.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/feature_specs/predictor.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/feature_specs/static.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/feature_specs/static.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/feature_specs/test_from_legacy.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/feature_specs/test_from_legacy.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/feature_specs/test_specs.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/feature_specs/test_specs.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/feature_specs/timedelta.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/feature_specs/timedelta.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/feature_specs/timestamp_frame.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/feature_specs/timestamp_frame.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/flattener.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/flattener.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
+import datetime as dt
 from dataclasses import dataclass
 from functools import partial
 from multiprocessing import Pool
 from typing import TYPE_CHECKING, Union
-import datetime as dt
 
 import polars as pl
 import tqdm
 from iterpy.iter import Iter
 from rich.progress import track
 
 from timeseriesflattener.frame_utilities._horisontally_concat import horizontally_concatenate_dfs
@@ -124,14 +124,18 @@
             for spec in specs:
                 spec.value_frame.df = spec.value_frame.collect()  # type: ignore
         else:
             self.predictiontime_frame.df = self.predictiontime_frame.df.lazy()
             for spec in specs:
                 spec.value_frame.df = spec.value_frame.df.lazy()
 
+        self.predictiontime_frame.df = self.predictiontime_frame.df.sort(
+            self.predictiontime_frame.timestamp_col_name
+        )  # type: ignore
+
         # Process and collect the specs. One-by-one, to get feedback on progress.
         dfs: Sequence[pl.LazyFrame] = []
         if self.n_workers is None:
             for spec in track(specs, description="Processing specs..."):
                 print(f"Processing spec: {spec.value_frame.value_col_names}")
                 processed_spec = process_spec(
                     predictiontime_frame=self.predictiontime_frame, spec=spec, step_size=step_size
```

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/frame_utilities/anyframe_to_lazyframe.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/frame_utilities/anyframe_to_lazyframe.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/process_spec.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/process_spec.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/spec_processors/static.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/spec_processors/static.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/spec_processors/temporal.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/spec_processors/temporal.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/spec_processors/test_static.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/spec_processors/test_static.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/spec_processors/test_temporal.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/spec_processors/test_temporal.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/spec_processors/timedelta.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/spec_processors/timedelta.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/test_aggregators.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/test_aggregators.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/test_flattener.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/test_flattener.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 from . import flattener
 from ._frame_validator import SpecColumnError
 from .feature_specs.meta import ValueFrame
 from .feature_specs.outcome import OutcomeSpec
 from .feature_specs.prediction_times import PredictionTimeFrame
 from .feature_specs.predictor import PredictorSpec
+from .feature_specs.static import StaticSpec, StaticFrame
 
 if TYPE_CHECKING:
     from collections.abc import Sequence
 
 FakePredictiontimeFrame = PredictionTimeFrame(
     init_df=pl.LazyFrame({"entity_id": [1], "pred_timestamp": ["2021-01-03"]})
 )
@@ -311,7 +312,53 @@
         ]
     )
     expected = str_to_pl_df(
         """pred_time_uuid,outc_value_within_5_to_30_days_mean_fallback_nan
 1-2022-01-01 00:00:00.000000,1"""
     )
     assert_frame_equal(result.collect(), expected, ignore_colums=["dw_ek_borger", "pred_timestamp"])
+
+
+@pytest.mark.parametrize("step_size", [None, dt.timedelta(days=30)])
+def test_multiple_features_with_unordered_prediction_times(step_size):
+    prediction_times_df_str = """entity_id,pred_timestamp,
+                            2,2022-01-02 00:00:00
+                            1,2022-01-01 00:00:00
+                            1,2020-01-01 00:00:00
+                            """
+    pred_df_str = """entity_id,timestamp,value,
+                        1,2021-12-31 00:00:01, 1
+                        """
+    static_df_str = """entity_id,static
+                        1,1
+                        2,2
+                        """
+    result = flattener.Flattener(
+        predictiontime_frame=PredictionTimeFrame(init_df=str_to_pl_df(prediction_times_df_str))
+    ).aggregate_timeseries(
+        specs=[
+            PredictorSpec(
+                value_frame=ValueFrame(init_df=str_to_pl_df(pred_df_str)),
+                lookbehind_distances=[dt.timedelta(days=1)],
+                fallback=0,
+                aggregators=[MeanAggregator()],
+            ),
+            StaticSpec(
+                value_frame=StaticFrame(init_df=str_to_pl_df(static_df_str)),
+                column_prefix="pred",
+                fallback=0,
+            ),
+        ],
+        step_size=step_size,
+    )
+    expected = str_to_pl_df(
+        """pred_time_uuid,pred_value_within_0_to_1_days_mean_fallback_0,pred_static_fallback_0
+2-2022-01-02 00:00:00.000000,0.0,2
+1-2022-01-01 00:00:00.000000,1.0,1
+1-2020-01-01 00:00:00.000000,0.0,1
+"""
+    ).sort("pred_time_uuid")
+    assert_frame_equal(
+        result.df.collect().sort("pred_time_uuid"),
+        expected,
+        ignore_colums=["entity_id", "pred_timestamp"],
+    )
```

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/testing/load_synth_data.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/testing/load_synth_data.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/testing/synth_data_generator/synth_col_generators.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/testing/synth_data_generator/synth_col_generators.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/testing/synth_data_generator/synth_prediction_times_generator.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/testing/synth_data_generator/synth_prediction_times_generator.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/testing/synth_data_generator/synth_txt_data_generator.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/testing/synth_data_generator/synth_txt_data_generator.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/testing/synth_data_generator/utils.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/testing/synth_data_generator/utils.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv` & `timeseriesflattener-2.2.1/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/raw/create_synth_birthdays.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/testing/test_data/raw/create_synth_birthdays.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/raw/create_synth_prediction_times.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/testing/test_data/raw/create_synth_prediction_times.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_binary.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_binary.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_float.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_float.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/raw/create_synth_sex.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/testing/test_data/raw/create_synth_sex.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/raw/synth_birthdays.csv` & `timeseriesflattener-2.2.1/src/timeseriesflattener/testing/test_data/raw/synth_birthdays.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/raw/synth_prediction_times.csv` & `timeseriesflattener-2.2.1/src/timeseriesflattener/testing/test_data/raw/synth_prediction_times.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_1.csv` & `timeseriesflattener-2.2.1/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_1.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_2.csv` & `timeseriesflattener-2.2.1/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_2.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_1.csv` & `timeseriesflattener-2.2.1/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_1.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_2.csv` & `timeseriesflattener-2.2.1/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_2.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/raw/synth_sex.csv` & `timeseriesflattener-2.2.1/src/timeseriesflattener/testing/test_data/raw/synth_sex.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/testing/test_data/raw/synth_text_data.csv` & `timeseriesflattener-2.2.1/src/timeseriesflattener/testing/test_data/raw/synth_text_data.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/testing/utils_for_testing.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/testing/utils_for_testing.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/aggregation_fns.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/v1/aggregation_fns.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/df_transforms.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/v1/df_transforms.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/feature_cache/abstract_feature_cache.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/v1/feature_cache/abstract_feature_cache.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/feature_cache/cache_to_disk.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/v1/feature_cache/cache_to_disk.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/feature_specs/group_specs.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/v1/feature_specs/group_specs.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/feature_specs/single_specs.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/v1/feature_specs/single_specs.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/flattened_dataset.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/v1/flattened_dataset.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/flattened_ds_validator.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/v1/flattened_ds_validator.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/logger.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/v1/logger.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/misc_utils.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/v1/misc_utils.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/load_synth_data.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/v1/testing/load_synth_data.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/synth_data_generator/synth_col_generators.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/v1/testing/synth_data_generator/synth_col_generators.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/synth_data_generator/synth_prediction_times_generator.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/v1/testing/synth_data_generator/synth_prediction_times_generator.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/synth_data_generator/synth_txt_data_generator.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/v1/testing/synth_data_generator/synth_txt_data_generator.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/synth_data_generator/utils.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/v1/testing/synth_data_generator/utils.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/v1/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv` & `timeseriesflattener-2.2.1/src/timeseriesflattener/v1/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/models/create_bow_and_pca_model.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/v1/testing/test_data/models/create_bow_and_pca_model.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/models/synth_bow_model.pkl` & `timeseriesflattener-2.2.1/src/timeseriesflattener/v1/testing/test_data/models/synth_bow_model.pkl`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/models/synth_pca_model.pkl` & `timeseriesflattener-2.2.1/src/timeseriesflattener/v1/testing/test_data/models/synth_pca_model.pkl`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_prediction_times.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_prediction_times.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_raw_binary.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_raw_binary.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_raw_float.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_raw_float.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_sex.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/v1/testing/test_data/raw/create_synth_sex.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/raw/synth_birthdays.csv` & `timeseriesflattener-2.2.1/src/timeseriesflattener/v1/testing/test_data/raw/synth_birthdays.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/raw/synth_prediction_times.csv` & `timeseriesflattener-2.2.1/src/timeseriesflattener/v1/testing/test_data/raw/synth_prediction_times.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_binary_1.csv` & `timeseriesflattener-2.2.1/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_binary_1.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_binary_2.csv` & `timeseriesflattener-2.2.1/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_binary_2.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_float_1.csv` & `timeseriesflattener-2.2.1/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_float_1.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_float_2.csv` & `timeseriesflattener-2.2.1/src/timeseriesflattener/v1/testing/test_data/raw/synth_raw_float_2.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/raw/synth_sex.csv` & `timeseriesflattener-2.2.1/src/timeseriesflattener/v1/testing/test_data/raw/synth_sex.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/test_data/raw/synth_text_data.csv` & `timeseriesflattener-2.2.1/src/timeseriesflattener/v1/testing/test_data/raw/synth_text_data.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/testing/utils_for_testing.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/v1/testing/utils_for_testing.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/tests/test_feature_cache/test_cache_to_disk.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/v1/tests/test_feature_cache/test_cache_to_disk.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_aggregation_fns.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_aggregation_fns.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_df_transforms.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_df_transforms.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_feature_spec_objects.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_feature_spec_objects.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/utils.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/v1/tests/test_timeseriesflattener/test_flattened_dataset/utils.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener/v1/utils/pydantic_basemodel.py` & `timeseriesflattener-2.2.1/src/timeseriesflattener/v1/utils/pydantic_basemodel.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener.egg-info/PKG-INFO` & `timeseriesflattener-2.2.1/src/timeseriesflattener.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timeseriesflattener
-Version: 2.2.0
+Version: 2.2.1
 Summary: A package for converting time series data from e.g. electronic health records into wide format data.
 Author: Kenneth Enevoldsen
 Author-email: Lasse Hansen <lasseh0310@gmail.com>, Jakob Grøhn Damgaard <bokajgd@gmail.com>, Martin Bernstorff <martinbernstorff@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 PSYCOP Group, Aarhus University
         
@@ -115,19 +115,19 @@
     {"id": [1, 1, 2], "date": ["2020-01-01", "2020-02-01", "2020-02-01"]}
 )
 # Load a dataframe with raw values you wish to aggregate as predictors
 predictor_df = pl.DataFrame(
     {
         "id": [1, 1, 1, 2],
         "date": ["2020-01-15", "2019-12-10", "2019-12-15", "2020-01-02"],
-        "value": [1, 2, 3, 4],
+        "predictor_value": [1, 2, 3, 4],
     }
 )
 # Load a dataframe specifying when the outcome occurs
-outcome_df = pl.DataFrame({"id": [1], "date": ["2020-03-01"], "value": [1]})
+outcome_df = pl.DataFrame({"id": [1], "date": ["2020-03-01"], "outcome_value": [1]})
 
 # Specify how to aggregate the predictors and define the outcome
 from timeseriesflattener import (
     MaxAggregator,
     MinAggregator,
     OutcomeSpec,
     PredictionTimeFrame,
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: timeseriesflattener Version: 2.2.0 Summary: A
+Metadata-Version: 2.1 Name: timeseriesflattener Version: 2.2.1 Summary: A
 package for converting time series data from e.g. electronic health records
 into wide format data. Author: Kenneth Enevoldsen Author-email: Lasse Hansen
 gmail.com>, Jakob GrÃ¸hn Damgaard
 gmail.com>, Martin Bernstorff
 gmail.com> License: MIT License Copyright (c) 2022 PSYCOP Group, Aarhus
 University Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
@@ -77,18 +77,18 @@
 timeseriesflattener simply install it using pip by running the following line
 in your terminal: ``` pip install timeseriesflattener ``` ## â¡ Quick start
 ```py import datetime as dt import numpy as np import polars as pl # Load a
 dataframe with times you wish to make a prediction prediction_times_df =
 pl.DataFrame( {"id": [1, 1, 2], "date": ["2020-01-01", "2020-02-01", "2020-02-
 01"]} ) # Load a dataframe with raw values you wish to aggregate as predictors
 predictor_df = pl.DataFrame( { "id": [1, 1, 1, 2], "date": ["2020-01-15",
-"2019-12-10", "2019-12-15", "2020-01-02"], "value": [1, 2, 3, 4], } ) # Load a
-dataframe specifying when the outcome occurs outcome_df = pl.DataFrame({"id":
-[1], "date": ["2020-03-01"], "value": [1]}) # Specify how to aggregate the
-predictors and define the outcome from timeseriesflattener import
+"2019-12-10", "2019-12-15", "2020-01-02"], "predictor_value": [1, 2, 3, 4], } )
+# Load a dataframe specifying when the outcome occurs outcome_df = pl.DataFrame
+({"id": [1], "date": ["2020-03-01"], "outcome_value": [1]}) # Specify how to
+aggregate the predictors and define the outcome from timeseriesflattener import
 ( MaxAggregator, MinAggregator, OutcomeSpec, PredictionTimeFrame,
 PredictorSpec, ValueFrame, ) predictor_spec = PredictorSpec
 ( value_frame=ValueFrame( init_df=predictor_df.lazy(), entity_id_col_name="id",
 value_timestamp_col_name="date" ), lookbehind_distances=[dt.timedelta(days=1)],
 aggregators=[MaxAggregator(), MinAggregator()], fallback=np.nan,
 column_prefix="pred", ) outcome_spec = OutcomeSpec( value_frame=ValueFrame
 ( init_df=outcome_df.lazy(), entity_id_col_name="id",
```

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener.egg-info/SOURCES.txt` & `timeseriesflattener-2.2.1/src/timeseriesflattener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/src/timeseriesflattener.egg-info/requires.txt` & `timeseriesflattener-2.2.1/src/timeseriesflattener.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-2.2.0/tasks.py` & `timeseriesflattener-2.2.1/tasks.py`

 * *Files identical despite different names*

