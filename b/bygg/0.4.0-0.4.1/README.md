# Comparing `tmp/bygg-0.4.0.tar.gz` & `tmp/bygg-0.4.1.tar.gz`

## Comparing `bygg-0.4.0.tar` & `bygg-0.4.1.tar`

### file list

```diff
@@ -1,86 +1,89 @@
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 bygg-0.4.0/.mise.toml
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 bygg-0.4.0/Vagrantfile
--rwxr-xr-x   0        0        0      981 2020-02-02 00:00:00.000000 bygg-0.4.0/Vagrantsetup.sh
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 bygg-0.4.0/_version.py
--rwxr-xr-x   0        0        0      981 2020-02-02 00:00:00.000000 bygg-0.4.0/bootstrap.py
--rwxr-xr-x   0        0        0      849 2020-02-02 00:00:00.000000 bygg-0.4.0/mypy.py
--rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 bygg-0.4.0/noxfile.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 bygg-0.4.0/requirements-dev.in
--rw-r--r--   0        0        0     7416 2020-02-02 00:00:00.000000 bygg-0.4.0/requirements-dev.txt
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 bygg-0.4.0/requirements.in
--rw-r--r--   0        0        0     9117 2020-02-02 00:00:00.000000 bygg-0.4.0/requirements.txt
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 bygg-0.4.0/.github/workflows/code_quality.yml
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 bygg-0.4.0/.github/workflows/pypi_publish.yml
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 bygg-0.4.0/.vscode/extensions.json
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 bygg-0.4.0/.vscode/launch.json
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 bygg-0.4.0/.vscode/settings.json
--rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 bygg-0.4.0/examples/checks/Byggfile.yml
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 bygg-0.4.0/examples/environments/.gitignore
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 bygg-0.4.0/examples/environments/Byggfile.py
--rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 bygg-0.4.0/examples/environments/Byggfile.yml
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 bygg-0.4.0/examples/environments/Byggfile1.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 bygg-0.4.0/examples/environments/Byggfile2.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 bygg-0.4.0/examples/environments/requirements.txt
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 bygg-0.4.0/examples/environments/requirements1.txt
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 bygg-0.4.0/examples/environments/requirements2.txt
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 bygg-0.4.0/examples/failing_jobs/Byggfile.yml
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 bygg-0.4.0/examples/failing_jobs/testdata/gcc.log
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 bygg-0.4.0/examples/failing_jobs/testdata/go.log
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 bygg-0.4.0/examples/failing_jobs/testdata/make.log
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 bygg-0.4.0/examples/failing_jobs/testdata/npm.log
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 bygg-0.4.0/examples/only_python/Byggfile.py
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 bygg-0.4.0/examples/parametric/.gitignore
--rw-r--r--   0        0        0     5258 2020-02-02 00:00:00.000000 bygg-0.4.0/examples/parametric/Byggfile.py
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 bygg-0.4.0/examples/parametric/Byggfile.yml
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 bygg-0.4.0/examples/parametric/README.md
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 bygg-0.4.0/examples/taskrunner/Byggfile.yml
--rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 bygg-0.4.0/examples/trivial/Byggfile.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 bygg-0.4.0/examples/trivial/Byggfile.yml
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 bygg-0.4.0/examples/trivial/input1.txt
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 bygg-0.4.0/examples/trivial/more_things/MoreActions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bygg-0.4.0/examples/trivial/more_things/__init__.py
--rw-r--r--   0        0        0     6068 2020-02-02 00:00:00.000000 bygg-0.4.0/schemas/Byggfile_yml_schema.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bygg-0.4.0/src/bygg/__init__.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 bygg-0.4.0/src/bygg/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bygg-0.4.0/src/bygg/py.typed
--rw-r--r--   0        0        0     4947 2020-02-02 00:00:00.000000 bygg-0.4.0/src/bygg/system_helpers.py
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 bygg-0.4.0/src/bygg/util.py
--rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 bygg-0.4.0/src/bygg/cmd/apply_configuration.py
--rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 bygg-0.4.0/src/bygg/cmd/argument_unparsing.py
--rw-r--r--   0        0        0     4657 2020-02-02 00:00:00.000000 bygg-0.4.0/src/bygg/cmd/completions.py
--rw-r--r--   0        0        0     4037 2020-02-02 00:00:00.000000 bygg-0.4.0/src/bygg/cmd/configuration.py
--rw-r--r--   0        0        0    18641 2020-02-02 00:00:00.000000 bygg-0.4.0/src/bygg/cmd/dispatcher.py
--rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 bygg-0.4.0/src/bygg/cmd/tree.py
--rw-r--r--   0        0        0     5610 2020-02-02 00:00:00.000000 bygg-0.4.0/src/bygg/core/action.py
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 bygg-0.4.0/src/bygg/core/cache.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 bygg-0.4.0/src/bygg/core/common_types.py
--rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 bygg-0.4.0/src/bygg/core/dag.py
--rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 bygg-0.4.0/src/bygg/core/digest.py
--rw-r--r--   0        0        0     6753 2020-02-02 00:00:00.000000 bygg-0.4.0/src/bygg/core/runner.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 bygg-0.4.0/src/bygg/core/scaffolding.py
--rw-r--r--   0        0        0     8680 2020-02-02 00:00:00.000000 bygg-0.4.0/src/bygg/core/scheduler.py
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 bygg-0.4.0/src/bygg/output/job_output.py
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 bygg-0.4.0/src/bygg/output/output.py
--rw-r--r--   0        0        0     3063 2020-02-02 00:00:00.000000 bygg-0.4.0/src/bygg/output/status_display.py
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 bygg-0.4.0/tests/conftest.py
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 bygg-0.4.0/tests/test_action.py
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 bygg-0.4.0/tests/test_argument_unparsing.py
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 bygg-0.4.0/tests/test_cache.py
--rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 bygg-0.4.0/tests/test_completions.py
--rw-r--r--   0        0        0     7366 2020-02-02 00:00:00.000000 bygg-0.4.0/tests/test_digest.py
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 bygg-0.4.0/tests/test_job_output.py
--rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 bygg-0.4.0/tests/test_main.py
--rw-r--r--   0        0        0    12884 2020-02-02 00:00:00.000000 bygg-0.4.0/tests/test_scheduler.py
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 bygg-0.4.0/tests/test_system_helpers.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 bygg-0.4.0/tests/test_tree.py
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 bygg-0.4.0/tests/test_utils.py
--rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 bygg-0.4.0/tests/__snapshots__/test_completions.ambr
--rw-r--r--   0        0        0     4471 2020-02-02 00:00:00.000000 bygg-0.4.0/tests/__snapshots__/test_job_output.ambr
--rw-r--r--   0        0        0    35252 2020-02-02 00:00:00.000000 bygg-0.4.0/tests/__snapshots__/test_main.ambr
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 bygg-0.4.0/tests/__snapshots__/test_system_helpers.ambr
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 bygg-0.4.0/tests/__snapshots__/test_tree.ambr
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 bygg-0.4.0/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 bygg-0.4.0/LICENSE
--rw-r--r--   0        0        0     6019 2020-02-02 00:00:00.000000 bygg-0.4.0/README.md
--rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 bygg-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     7937 2020-02-02 00:00:00.000000 bygg-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 bygg-0.4.1/.mise.toml
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 bygg-0.4.1/Vagrantfile
+-rwxr-xr-x   0        0        0      981 2020-02-02 00:00:00.000000 bygg-0.4.1/Vagrantsetup.sh
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 bygg-0.4.1/_version.py
+-rwxr-xr-x   0        0        0      981 2020-02-02 00:00:00.000000 bygg-0.4.1/bootstrap.py
+-rwxr-xr-x   0        0        0      849 2020-02-02 00:00:00.000000 bygg-0.4.1/mypy.py
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 bygg-0.4.1/noxfile.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 bygg-0.4.1/requirements-dev.in
+-rw-r--r--   0        0        0     7428 2020-02-02 00:00:00.000000 bygg-0.4.1/requirements-dev.txt
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 bygg-0.4.1/requirements.in
+-rw-r--r--   0        0        0     9301 2020-02-02 00:00:00.000000 bygg-0.4.1/requirements.txt
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 bygg-0.4.1/.github/workflows/code_quality.yml
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 bygg-0.4.1/.github/workflows/pypi_publish.yml
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 bygg-0.4.1/.vscode/extensions.json
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 bygg-0.4.1/.vscode/launch.json
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 bygg-0.4.1/.vscode/settings.json
+-rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 bygg-0.4.1/examples/checks/Byggfile.yml
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 bygg-0.4.1/examples/environments/.gitignore
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 bygg-0.4.1/examples/environments/Byggfile.py
+-rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 bygg-0.4.1/examples/environments/Byggfile.yml
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 bygg-0.4.1/examples/environments/Byggfile1.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 bygg-0.4.1/examples/environments/Byggfile2.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 bygg-0.4.1/examples/environments/requirements.txt
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 bygg-0.4.1/examples/environments/requirements1.txt
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 bygg-0.4.1/examples/environments/requirements2.txt
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 bygg-0.4.1/examples/failing_jobs/Byggfile.yml
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 bygg-0.4.1/examples/failing_jobs/testdata/gcc.log
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 bygg-0.4.1/examples/failing_jobs/testdata/go.log
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 bygg-0.4.1/examples/failing_jobs/testdata/make.log
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 bygg-0.4.1/examples/failing_jobs/testdata/npm.log
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 bygg-0.4.1/examples/only_python/Byggfile.py
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 bygg-0.4.1/examples/parametric/.gitignore
+-rw-r--r--   0        0        0     5258 2020-02-02 00:00:00.000000 bygg-0.4.1/examples/parametric/Byggfile.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 bygg-0.4.1/examples/parametric/Byggfile.yml
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 bygg-0.4.1/examples/parametric/README.md
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 bygg-0.4.1/examples/taskrunner/Byggfile.yml
+-rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 bygg-0.4.1/examples/trivial/Byggfile.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 bygg-0.4.1/examples/trivial/Byggfile.yml
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 bygg-0.4.1/examples/trivial/input1.txt
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 bygg-0.4.1/examples/trivial/more_things/MoreActions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bygg-0.4.1/examples/trivial/more_things/__init__.py
+-rw-r--r--   0        0        0     6068 2020-02-02 00:00:00.000000 bygg-0.4.1/schemas/Byggfile_yml_schema.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bygg-0.4.1/src/bygg/__init__.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 bygg-0.4.1/src/bygg/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bygg-0.4.1/src/bygg/py.typed
+-rw-r--r--   0        0        0     4947 2020-02-02 00:00:00.000000 bygg-0.4.1/src/bygg/system_helpers.py
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 bygg-0.4.1/src/bygg/util.py
+-rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 bygg-0.4.1/src/bygg/cmd/apply_configuration.py
+-rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 bygg-0.4.1/src/bygg/cmd/argument_unparsing.py
+-rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 bygg-0.4.1/src/bygg/cmd/build_clean.py
+-rw-r--r--   0        0        0     4657 2020-02-02 00:00:00.000000 bygg-0.4.1/src/bygg/cmd/completions.py
+-rw-r--r--   0        0        0     4037 2020-02-02 00:00:00.000000 bygg-0.4.1/src/bygg/cmd/configuration.py
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 bygg-0.4.1/src/bygg/cmd/datastructures.py
+-rw-r--r--   0        0        0    12526 2020-02-02 00:00:00.000000 bygg-0.4.1/src/bygg/cmd/dispatcher.py
+-rw-r--r--   0        0        0     2565 2020-02-02 00:00:00.000000 bygg-0.4.1/src/bygg/cmd/list_actions.py
+-rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 bygg-0.4.1/src/bygg/cmd/tree.py
+-rw-r--r--   0        0        0     7207 2020-02-02 00:00:00.000000 bygg-0.4.1/src/bygg/core/action.py
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 bygg-0.4.1/src/bygg/core/cache.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 bygg-0.4.1/src/bygg/core/common_types.py
+-rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 bygg-0.4.1/src/bygg/core/dag.py
+-rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 bygg-0.4.1/src/bygg/core/digest.py
+-rw-r--r--   0        0        0     7056 2020-02-02 00:00:00.000000 bygg-0.4.1/src/bygg/core/runner.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 bygg-0.4.1/src/bygg/core/scaffolding.py
+-rw-r--r--   0        0        0     8748 2020-02-02 00:00:00.000000 bygg-0.4.1/src/bygg/core/scheduler.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 bygg-0.4.1/src/bygg/output/job_output.py
+-rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 bygg-0.4.1/src/bygg/output/output.py
+-rw-r--r--   0        0        0     3063 2020-02-02 00:00:00.000000 bygg-0.4.1/src/bygg/output/status_display.py
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 bygg-0.4.1/tests/conftest.py
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 bygg-0.4.1/tests/test_action.py
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 bygg-0.4.1/tests/test_argument_unparsing.py
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 bygg-0.4.1/tests/test_cache.py
+-rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 bygg-0.4.1/tests/test_completions.py
+-rw-r--r--   0        0        0     7366 2020-02-02 00:00:00.000000 bygg-0.4.1/tests/test_digest.py
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 bygg-0.4.1/tests/test_job_output.py
+-rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 bygg-0.4.1/tests/test_main.py
+-rw-r--r--   0        0        0    12884 2020-02-02 00:00:00.000000 bygg-0.4.1/tests/test_scheduler.py
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 bygg-0.4.1/tests/test_system_helpers.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 bygg-0.4.1/tests/test_tree.py
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 bygg-0.4.1/tests/test_utils.py
+-rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 bygg-0.4.1/tests/__snapshots__/test_completions.ambr
+-rw-r--r--   0        0        0     4471 2020-02-02 00:00:00.000000 bygg-0.4.1/tests/__snapshots__/test_job_output.ambr
+-rw-r--r--   0        0        0    35252 2020-02-02 00:00:00.000000 bygg-0.4.1/tests/__snapshots__/test_main.ambr
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 bygg-0.4.1/tests/__snapshots__/test_system_helpers.ambr
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 bygg-0.4.1/tests/__snapshots__/test_tree.ambr
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 bygg-0.4.1/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 bygg-0.4.1/LICENSE
+-rw-r--r--   0        0        0     6019 2020-02-02 00:00:00.000000 bygg-0.4.1/README.md
+-rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 bygg-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     7966 2020-02-02 00:00:00.000000 bygg-0.4.1/PKG-INFO
```

### Comparing `bygg-0.4.0/Vagrantfile` & `bygg-0.4.1/Vagrantfile`

 * *Files identical despite different names*

### Comparing `bygg-0.4.0/Vagrantsetup.sh` & `bygg-0.4.1/Vagrantsetup.sh`

 * *Files identical despite different names*

### Comparing `bygg-0.4.0/bootstrap.py` & `bygg-0.4.1/bootstrap.py`

 * *Files identical despite different names*

### Comparing `bygg-0.4.0/mypy.py` & `bygg-0.4.1/mypy.py`

 * *Files identical despite different names*

### Comparing `bygg-0.4.0/noxfile.py` & `bygg-0.4.1/noxfile.py`

 * *Files identical despite different names*

### Comparing `bygg-0.4.0/requirements-dev.txt` & `bygg-0.4.1/requirements-dev.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 # This file was autogenerated by uv via the following command:
-#    uv pip compile --generate-hashes requirements-dev.in -o requirements-dev.txt
+#    uv pip compile --generate-hashes requirements-dev.in --output-file requirements-dev.txt
 build==1.2.1 \
     --hash=sha256:526263f4870c26f26c433545579475377b2b7588b6f1eac76a001e873ae3e19d \
     --hash=sha256:75e10f767a433d9a86e50d83f418e83efc18ede923ee5ff7df93b6cb0306c5d4
     # via pip-tools
 click==8.1.7 \
     --hash=sha256:ae74fb96c20a0277a1d615f1e4d73c8414f5a98db8b799a7931d1582f3390c28 \
     --hash=sha256:ca9853ad459e787e2192211578cc907e7594e294c7ccc834310722b41b9ca6de
     # via pip-tools
 iniconfig==2.0.0 \
     --hash=sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3 \
     --hash=sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374
     # via pytest
-mypy==1.9.0 \
-    --hash=sha256:0235391f1c6f6ce487b23b9dbd1327b4ec33bb93934aa986efe8a9563d9349e6 \
-    --hash=sha256:190da1ee69b427d7efa8aa0d5e5ccd67a4fb04038c380237a0d96829cb157913 \
-    --hash=sha256:2418488264eb41f69cc64a69a745fad4a8f86649af4b1041a4c64ee61fc61129 \
-    --hash=sha256:3a3c007ff3ee90f69cf0a15cbcdf0995749569b86b6d2f327af01fd1b8aee9dc \
-    --hash=sha256:3cc5da0127e6a478cddd906068496a97a7618a21ce9b54bde5bf7e539c7af974 \
-    --hash=sha256:48533cdd345c3c2e5ef48ba3b0d3880b257b423e7995dada04248725c6f77374 \
-    --hash=sha256:49c87c15aed320de9b438ae7b00c1ac91cd393c1b854c2ce538e2a72d55df150 \
-    --hash=sha256:4d3dbd346cfec7cb98e6cbb6e0f3c23618af826316188d587d1c1bc34f0ede03 \
-    --hash=sha256:571741dc4194b4f82d344b15e8837e8c5fcc462d66d076748142327626a1b6e9 \
-    --hash=sha256:587ce887f75dd9700252a3abbc9c97bbe165a4a630597845c61279cf32dfbf02 \
-    --hash=sha256:5d741d3fc7c4da608764073089e5f58ef6352bedc223ff58f2f038c2c4698a89 \
-    --hash=sha256:5e6061f44f2313b94f920e91b204ec600982961e07a17e0f6cd83371cb23f5c2 \
-    --hash=sha256:61758fabd58ce4b0720ae1e2fea5cfd4431591d6d590b197775329264f86311d \
-    --hash=sha256:653265f9a2784db65bfca694d1edd23093ce49740b2244cde583aeb134c008f3 \
-    --hash=sha256:68edad3dc7d70f2f17ae4c6c1b9471a56138ca22722487eebacfd1eb5321d612 \
-    --hash=sha256:81a10926e5473c5fc3da8abb04119a1f5811a236dc3a38d92015cb1e6ba4cb9e \
-    --hash=sha256:85ca5fcc24f0b4aeedc1d02f93707bccc04733f21d41c88334c5482219b1ccb3 \
-    --hash=sha256:a260627a570559181a9ea5de61ac6297aa5af202f06fd7ab093ce74e7181e43e \
-    --hash=sha256:aceb1db093b04db5cd390821464504111b8ec3e351eb85afd1433490163d60cd \
-    --hash=sha256:b685154e22e4e9199fc95f298661deea28aaede5ae16ccc8cbb1045e716b3e04 \
-    --hash=sha256:d357423fa57a489e8c47b7c85dfb96698caba13d66e086b412298a1a0ea3b0ed \
-    --hash=sha256:d4d5ddc13421ba3e2e082a6c2d74c2ddb3979c39b582dacd53dd5d9431237185 \
-    --hash=sha256:e49499be624dead83927e70c756970a0bc8240e9f769389cdf5714b0784ca6bf \
-    --hash=sha256:e54396d70be04b34f31d2edf3362c1edd023246c82f1730bbf8768c28db5361b \
-    --hash=sha256:f88566144752999351725ac623471661c9d1cd8caa0134ff98cceeea181789f4 \
-    --hash=sha256:f8a67616990062232ee4c3952f41c779afac41405806042a8126fe96e098419f \
-    --hash=sha256:fe28657de3bfec596bbeef01cb219833ad9d38dd5393fc649f4b366840baefe6
+mypy==1.10.0 \
+    --hash=sha256:075cbf81f3e134eadaf247de187bd604748171d6b79736fa9b6c9685b4083061 \
+    --hash=sha256:12b6bfc1b1a66095ab413160a6e520e1dc076a28f3e22f7fb25ba3b000b4ef99 \
+    --hash=sha256:1ec404a7cbe9fc0e92cb0e67f55ce0c025014e26d33e54d9e506a0f2d07fe5de \
+    --hash=sha256:28d0e038361b45f099cc086d9dd99c15ff14d0188f44ac883010e172ce86c38a \
+    --hash=sha256:2b0695d605ddcd3eb2f736cd8b4e388288c21e7de85001e9f85df9187f2b50f9 \
+    --hash=sha256:3236a4c8f535a0631f85f5fcdffba71c7feeef76a6002fcba7c1a8e57c8be1ec \
+    --hash=sha256:3be66771aa5c97602f382230165b856c231d1277c511c9a8dd058be4784472e1 \
+    --hash=sha256:3d087fcbec056c4ee34974da493a826ce316947485cef3901f511848e687c131 \
+    --hash=sha256:3f298531bca95ff615b6e9f2fc0333aae27fa48052903a0ac90215021cdcfa4f \
+    --hash=sha256:4a2b5cdbb5dd35aa08ea9114436e0d79aceb2f38e32c21684dcf8e24e1e92821 \
+    --hash=sha256:4cf18f9d0efa1b16478c4c129eabec36148032575391095f73cae2e722fcf9d5 \
+    --hash=sha256:8b2cbaca148d0754a54d44121b5825ae71868c7592a53b7292eeb0f3fdae95ee \
+    --hash=sha256:8f55583b12156c399dce2df7d16f8a5095291354f1e839c252ec6c0611e86e2e \
+    --hash=sha256:92f93b21c0fe73dc00abf91022234c79d793318b8a96faac147cd579c1671746 \
+    --hash=sha256:9e36fb078cce9904c7989b9693e41cb9711e0600139ce3970c6ef814b6ebc2b2 \
+    --hash=sha256:9fd50226364cd2737351c79807775136b0abe084433b55b2e29181a4c3c878c0 \
+    --hash=sha256:a781f6ad4bab20eef8b65174a57e5203f4be627b46291f4589879bf4e257b97b \
+    --hash=sha256:a87dbfa85971e8d59c9cc1fcf534efe664d8949e4c0b6b44e8ca548e746a8d53 \
+    --hash=sha256:b808e12113505b97d9023b0b5e0c0705a90571c6feefc6f215c1df9381256e30 \
+    --hash=sha256:bc6ac273b23c6b82da3bb25f4136c4fd42665f17f2cd850771cb600bdd2ebeda \
+    --hash=sha256:cd777b780312ddb135bceb9bc8722a73ec95e042f911cc279e2ec3c667076051 \
+    --hash=sha256:da1cbf08fb3b851ab3b9523a884c232774008267b1f83371ace57f412fe308c2 \
+    --hash=sha256:e22e1527dc3d4aa94311d246b59e47f6455b8729f4968765ac1eacf9a4760bc7 \
+    --hash=sha256:f8c083976eb530019175aabadb60921e73b4f45736760826aa1689dda8208aee \
+    --hash=sha256:f90cff89eea89273727d8783fef5d4a934be2fdca11b47def50cf5d311aff727 \
+    --hash=sha256:fa7ef5244615a2523b56c034becde4e9e3f9b034854c93639adb667ec9ec2976 \
+    --hash=sha256:fcfc70599efde5c67862a07a1aaf50e55bce629ace26bb19dc17cece5dd31ca4
 mypy-extensions==1.0.0 \
     --hash=sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d \
     --hash=sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782
     # via mypy
 nodeenv==1.8.0 \
     --hash=sha256:d51e0c37e64fbf47d017feac3145cdbb58836d7eee8c6f6d3b6880c5456227d2 \
     --hash=sha256:df865724bb3c3adc86b3876fa209771517b0cfe596beff01a92700e0e8be4cec
@@ -57,54 +57,54 @@
 pip==24.0 \
     --hash=sha256:ba0d021a166865d2265246961bec0152ff124de910c5cc39f1156ce3fa7c69dc \
     --hash=sha256:ea9bd1a847e8c5774a5777bb398c19e80bcd4e2aa16a4b301b718fe6f593aba2
     # via pip-tools
 pip-tools==7.4.1 \
     --hash=sha256:4c690e5fbae2f21e87843e89c26191f0d9454f362d8acdbd695716493ec8b3a9 \
     --hash=sha256:864826f5073864450e24dbeeb85ce3920cdfb09848a3d69ebf537b521f14bcc9
-pluggy==1.4.0 \
-    --hash=sha256:7db9f7b503d67d1c5b95f59773ebb58a8c1c288129a88665838012cfb07b8981 \
-    --hash=sha256:8c85c2876142a764e5b7548e7d9a0e0ddb46f5185161049a79b7e974454223be
+pluggy==1.5.0 \
+    --hash=sha256:2cffa88e94fdc978c4c574f15f9e59b7f4201d439195c3715ca9e2486f1d0cf1 \
+    --hash=sha256:44e1ad92c8ca002de6377e165f3e0f1be63266ab4d554740532335b9d75ea669
     # via pytest
 pyproject-hooks==1.0.0 \
     --hash=sha256:283c11acd6b928d2f6a7c73fa0d01cb2bdc5f07c57a2eeb6e83d5e56b97976f8 \
     --hash=sha256:f271b298b97f5955d53fb12b72c1fb1948c22c1a6b70b315c54cedaca0264ef5
     # via
     #   build
     #   pip-tools
-pyright==1.1.359 \
-    --hash=sha256:5582777be7eab73512277ac7da7b41e15bc0737f488629cb9babd96e0769be61 \
-    --hash=sha256:f0eab50f3dafce8a7302caeafd6a733f39901a2bf5170bb23d77fd607c8a8dbc
-pytest==8.1.1 \
-    --hash=sha256:2a8386cfc11fa9d2c50ee7b2a57e7d898ef90470a7a34c4b949ff59662bb78b7 \
-    --hash=sha256:ac978141a75948948817d360297b7aae0fcb9d6ff6bc9ec6d514b85d5a65c044
+pyright==1.1.361 \
+    --hash=sha256:1d67933315666b05d230c85ea8fb97aaa2056e4092a13df87b7765bb9e8f1a8d \
+    --hash=sha256:c50fc94ce92b5c958cfccbbe34142e7411d474da43d6c14a958667e35b9df7ea
+pytest==8.2.0 \
+    --hash=sha256:1733f0620f6cda4095bbf0d9ff8022486e91892245bb9e7d5542c018f612f233 \
+    --hash=sha256:d507d4482197eac0ba2bae2e9babf0672eb333017bcedaa5fb1a3d42c1174b3f
     # via
     #   pytest-mock
     #   syrupy
 pytest-mock==3.14.0 \
     --hash=sha256:0b72c38033392a5f4621342fe11e9219ac11ec9d375f8e2a0c164539e0d70f6f \
     --hash=sha256:2719255a1efeceadbc056d6bf3df3d1c5015530fb40cf347c0f9afac88410bd0
-ruff==0.4.1 \
-    --hash=sha256:0926cefb57fc5fced629603fbd1a23d458b25418681d96823992ba975f050c2b \
-    --hash=sha256:1c859f294f8633889e7d77de228b203eb0e9a03071b72b5989d89a0cf98ee262 \
-    --hash=sha256:2c6e37f2e3cd74496a74af9a4fa67b547ab3ca137688c484749189bf3a686ceb \
-    --hash=sha256:2d9ef6231e3fbdc0b8c72404a1a0c46fd0dcea84efca83beb4681c318ea6a953 \
-    --hash=sha256:6e68d248ed688b9d69fd4d18737edcbb79c98b251bba5a2b031ce2470224bdf9 \
-    --hash=sha256:9485f54a7189e6f7433e0058cf8581bee45c31a25cd69009d2a040d1bd4bfaef \
-    --hash=sha256:a1eaf03d87e6a7cd5e661d36d8c6e874693cb9bc3049d110bc9a97b350680c43 \
-    --hash=sha256:b34510141e393519a47f2d7b8216fec747ea1f2c81e85f076e9f2910588d4b64 \
-    --hash=sha256:b90506f3d6d1f41f43f9b7b5ff845aeefabed6d2494307bc7b178360a8805252 \
-    --hash=sha256:b92f03b4aa9fa23e1799b40f15f8b95cdc418782a567d6c43def65e1bbb7f1cf \
-    --hash=sha256:baa27d9d72a94574d250f42b7640b3bd2edc4c58ac8ac2778a8c82374bb27984 \
-    --hash=sha256:c7d391e5936af5c9e252743d767c564670dc3889aff460d35c518ee76e4b26d7 \
-    --hash=sha256:d2921ac03ce1383e360e8a95442ffb0d757a6a7ddd9a5be68561a671e0e5807e \
-    --hash=sha256:d592116cdbb65f8b1b7e2a2b48297eb865f6bdc20641879aa9d7b9c11d86db79 \
-    --hash=sha256:eec8d185fe193ad053eda3a6be23069e0c8ba8c5d20bc5ace6e3b9e37d246d3f \
-    --hash=sha256:efd703a5975ac1998c2cc5e9494e13b28f31e66c616b0a76e206de2562e0843c \
-    --hash=sha256:f1ee41580bff1a651339eb3337c20c12f4037f6110a36ae4a2d864c52e5ef954
+ruff==0.4.2 \
+    --hash=sha256:0e2e06459042ac841ed510196c350ba35a9b24a643e23db60d79b2db92af0c2b \
+    --hash=sha256:1f32cadf44c2020e75e0c56c3408ed1d32c024766bd41aedef92aa3ca28eef68 \
+    --hash=sha256:22e306bf15e09af45ca812bc42fa59b628646fa7c26072555f278994890bc7ac \
+    --hash=sha256:24016ed18db3dc9786af103ff49c03bdf408ea253f3cb9e3638f39ac9cf2d483 \
+    --hash=sha256:33bcc160aee2520664bc0859cfeaebc84bb7323becff3f303b8f1f2d81cb4edc \
+    --hash=sha256:3afabaf7ba8e9c485a14ad8f4122feff6b2b93cc53cd4dad2fd24ae35112d5c5 \
+    --hash=sha256:5ec481661fb2fd88a5d6cf1f83403d388ec90f9daaa36e40e2c003de66751798 \
+    --hash=sha256:652e4ba553e421a6dc2a6d4868bc3b3881311702633eb3672f9f244ded8908cd \
+    --hash=sha256:6a2243f8f434e487c2a010c7252150b1fdf019035130f41b77626f5655c9ca22 \
+    --hash=sha256:6ab165ef5d72392b4ebb85a8b0fbd321f69832a632e07a74794c0e598e7a8376 \
+    --hash=sha256:7891ee376770ac094da3ad40c116258a381b86c7352552788377c6eb16d784fe \
+    --hash=sha256:799eb468ea6bc54b95527143a4ceaf970d5aa3613050c6cff54c85fda3fde480 \
+    --hash=sha256:82986bb77ad83a1719c90b9528a9dd663c9206f7c0ab69282af8223566a0c34e \
+    --hash=sha256:8772130a063f3eebdf7095da00c0b9898bd1774c43b336272c3e98667d4fb8fa \
+    --hash=sha256:8d14dc8953f8af7e003a485ef560bbefa5f8cc1ad994eebb5b12136049bbccc5 \
+    --hash=sha256:cbd1e87c71bca14792948c4ccb51ee61c3296e164019d2d484f3eaa2d360dfaf \
+    --hash=sha256:ec4ba9436a51527fb6931a8839af4c36a5481f8c19e8f5e42c2f7ad3a49f5069
 setuptools==69.5.1 \
     --hash=sha256:6c1fccdac05a97e598fb0ae3bbed5904ccb317337a51139dcd51453611bbb987 \
     --hash=sha256:c636ac361bc47580504644275c9ad802c50415c7522212252c033bd15f301f32
     # via
     #   nodeenv
     #   pip-tools
 syrupy==4.6.1 \
```

### Comparing `bygg-0.4.0/requirements.txt` & `bygg-0.4.1/requirements.txt`

 * *Files 3% similar despite different names*

```diff
@@ -3,16 +3,19 @@
 argcomplete==3.3.0 \
     --hash=sha256:c168c3723482c031df3c207d4ba8fa702717ccb9fc0bfe4117166c1f537b4a54 \
     --hash=sha256:fd03ff4a5b9e6580569d34b273f741e85cd9e072f3feeeee3eba4891c70eda62
 dill==0.3.8 \
     --hash=sha256:3ebe3c479ad625c4553aca177444d89b486b1d84982eeacded644afc0cf797ca \
     --hash=sha256:c36ca9ffb54365bdd2f8eb3eff7d2a21237f8452b57ace88b1ac615b7e815bd7
     # via multiprocess
-graph-theory==2023.7.6 \
-    --hash=sha256:9030aee88aa1db6c778f73338c143a4c872eb9ed5fad5eb9a768ebeb75541340
+graph-theory==2023.7.7 \
+    --hash=sha256:4d33f4f73f7dddf1e36166056e93f82accca4854efcc8c25eb85f8c609385a8d
+loguru==0.7.2 \
+    --hash=sha256:003d71e3d3ed35f0f8984898359d65b79e5b21943f78af86aa5491210429b8eb \
+    --hash=sha256:e671a53522515f34fd406340ee968cb9ecafbc4b36c679da03c18fd8d0bd51ac
 msgspec==0.18.6 \
     --hash=sha256:06acbd6edf175bee0e36295d6b0302c6de3aaf61246b46f9549ca0041a9d7177 \
     --hash=sha256:0e24539b25c85c8f0597274f11061c102ad6b0c56af053373ba4629772b407be \
     --hash=sha256:1003c20bfe9c6114cc16ea5db9c5466e49fae3d7f5e2e59cb70693190ad34da0 \
     --hash=sha256:1a76b60e501b3932782a9da039bd1cd552b7d8dec54ce38332b87136c64852dd \
     --hash=sha256:37f67c1d81272131895bb20d388dd8d341390acd0e192a55ab02d4d6468b434c \
     --hash=sha256:3ac4dd63fd5309dd42a8c8c36c1563531069152be7819518be0a9d03be9788e4 \
```

### Comparing `bygg-0.4.0/.github/workflows/code_quality.yml` & `bygg-0.4.1/.github/workflows/code_quality.yml`

 * *Files identical despite different names*

### Comparing `bygg-0.4.0/.github/workflows/pypi_publish.yml` & `bygg-0.4.1/.github/workflows/pypi_publish.yml`

 * *Files identical despite different names*

### Comparing `bygg-0.4.0/.vscode/launch.json` & `bygg-0.4.1/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `bygg-0.4.0/examples/checks/Byggfile.yml` & `bygg-0.4.1/examples/checks/Byggfile.yml`

 * *Files identical despite different names*

### Comparing `bygg-0.4.0/examples/environments/Byggfile.yml` & `bygg-0.4.1/examples/environments/Byggfile.yml`

 * *Files identical despite different names*

### Comparing `bygg-0.4.0/examples/failing_jobs/Byggfile.yml` & `bygg-0.4.1/examples/failing_jobs/Byggfile.yml`

 * *Files identical despite different names*

### Comparing `bygg-0.4.0/examples/failing_jobs/testdata/gcc.log` & `bygg-0.4.1/examples/failing_jobs/testdata/gcc.log`

 * *Files identical despite different names*

### Comparing `bygg-0.4.0/examples/failing_jobs/testdata/make.log` & `bygg-0.4.1/examples/failing_jobs/testdata/make.log`

 * *Files identical despite different names*

### Comparing `bygg-0.4.0/examples/failing_jobs/testdata/npm.log` & `bygg-0.4.1/examples/failing_jobs/testdata/npm.log`

 * *Files identical despite different names*

### Comparing `bygg-0.4.0/examples/parametric/Byggfile.py` & `bygg-0.4.1/examples/parametric/Byggfile.py`

 * *Files identical despite different names*

### Comparing `bygg-0.4.0/examples/trivial/Byggfile.py` & `bygg-0.4.1/examples/trivial/Byggfile.py`

 * *Files identical despite different names*

### Comparing `bygg-0.4.0/examples/trivial/input1.txt` & `bygg-0.4.1/examples/trivial/input1.txt`

 * *Files identical despite different names*

### Comparing `bygg-0.4.0/examples/trivial/more_things/MoreActions.py` & `bygg-0.4.1/examples/trivial/more_things/MoreActions.py`

 * *Files identical despite different names*

### Comparing `bygg-0.4.0/schemas/Byggfile_yml_schema.json` & `bygg-0.4.1/schemas/Byggfile_yml_schema.json`

 * *Files identical despite different names*

### Comparing `bygg-0.4.0/src/bygg/system_helpers.py` & `bygg-0.4.1/src/bygg/system_helpers.py`

 * *Files identical despite different names*

### Comparing `bygg-0.4.0/src/bygg/util.py` & `bygg-0.4.1/src/bygg/util.py`

 * *Files identical despite different names*

### Comparing `bygg-0.4.0/src/bygg/cmd/apply_configuration.py` & `bygg-0.4.1/src/bygg/cmd/apply_configuration.py`

 * *Files identical despite different names*

### Comparing `bygg-0.4.0/src/bygg/cmd/argument_unparsing.py` & `bygg-0.4.1/src/bygg/cmd/argument_unparsing.py`

 * *Files identical despite different names*

### Comparing `bygg-0.4.0/src/bygg/cmd/completions.py` & `bygg-0.4.1/src/bygg/cmd/completions.py`

 * *Files identical despite different names*

### Comparing `bygg-0.4.0/src/bygg/cmd/configuration.py` & `bygg-0.4.1/src/bygg/cmd/configuration.py`

 * *Files identical despite different names*

### Comparing `bygg-0.4.0/src/bygg/cmd/dispatcher.py` & `bygg-0.4.1/src/bygg/cmd/dispatcher.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,271 +1,65 @@
 import argparse
 from dataclasses import dataclass
 import os
-import shutil
-import stat
 import subprocess
 import sys
-import textwrap
-import time
 from typing import Any
 
 from bygg.cmd.apply_configuration import (
     apply_configuration,
     register_actions_from_configuration,
 )
 from bygg.cmd.argument_unparsing import unparse_args
+from bygg.cmd.build_clean import build, clean
 from bygg.cmd.completions import (
     ByggfileDirectoriesCompleter,
     do_completion,
     generate_shell_completions,
 )
 from bygg.cmd.configuration import (
     PYTHON_INPUTFILE,
     YAML_INPUTFILE,
     ByggFile,
     dump_schema,
     read_config_file,
 )
+from bygg.cmd.datastructures import ByggContext, get_entrypoints
+from bygg.cmd.list_actions import list_actions
 from bygg.cmd.tree import display_tree
 from bygg.core.runner import ProcessRunner
 from bygg.core.scheduler import Scheduler
-from bygg.output.job_output import output_job_logs
 from bygg.output.output import (
     TerminalStyle as TS,
 )
 from bygg.output.output import (
     output_error,
     output_info,
-    output_ok,
     output_plain,
     output_warning,
 )
 from bygg.output.status_display import (
-    failed_checks,
     on_job_status,
     on_runner_status,
-    output_check_results,
 )
 from bygg.system_helpers import change_dir
-
-
-@dataclass
-class ByggContext:
-    """Container for various state"""
-
-    runner: ProcessRunner
-    scheduler: Scheduler
-    configuration: ByggFile
-
-
-def get_job_count_limit():
-    try:
-        # Use os.sched_getaffinity where available (on U**X):
-        # https://stackoverflow.com/a/55423170
-        return len(os.sched_getaffinity(0))
-    except AttributeError:
-        count = os.cpu_count()
-        assert count is not None
-        return count
+from loguru import logger
 
 
 def init_bygg_context(configuration: ByggFile):
     scheduler = Scheduler()
     runner = ProcessRunner(scheduler)
 
     # Set up status listeners
     runner.job_status_listener = on_job_status
     runner.runner_status_listener = on_runner_status
 
     return ByggContext(runner, scheduler, configuration)
 
 
-def build(
-    ctx: ByggContext,
-    actions: list[str],
-    job_count: int | None,
-    always_make: bool,
-    check: bool,
-) -> bool:
-    """
-    actions: The actions to build.
-
-    job_count: The number of jobs to run simultaneously. None means to use the number of
-    available cores.
-
-    always_make: If True, all actions will be built, even if they are up to date.
-
-    check: If True, apply various checks:
-
-    * Check that the inputs and outputs of all actions will be checked for consistency.
-      A job that runs later must not have files as output that are inputs to a job that
-      runs earlier.
-    """
-    try:
-        max_workers = get_job_count_limit() if job_count is None else job_count
-
-        for action in actions:
-            t1 = time.time()
-            output_info(f"Building action '{action}':")
-
-            ctx.scheduler.start_run(
-                action,
-                always_make=always_make,
-                check=check,
-            )
-            status = ctx.runner.start(max_workers)
-            ctx.scheduler.shutdown()
-
-            if status:
-                output_ok(f"Action '{action}' completed in {time.time() - t1:.2f} s.")
-            else:
-                output_error(
-                    f"Action '{action}' failed after {time.time() - t1:.2f} s."
-                )
-                output_job_logs(ctx.runner.failed_jobs)
-                return False
-
-    except KeyboardInterrupt:
-        output_warning("\nBuild was interrupted by user.")
-        return False
-    except KeyError as e:
-        output_error(f"Error: Action '{e}' not found.")
-        return False
-    finally:
-        ctx.scheduler.shutdown()
-
-    if check and failed_checks:
-        return output_check_results()
-
-    return True
-
-
-def clean(ctx: ByggContext, actions: list[str]):
-    try:
-        for action in actions:
-            output_info(f"Cleaning action '{action}':")
-            ctx.scheduler.prepare_run(action)
-            for job_name in ctx.scheduler.job_graph.get_all_jobs():
-                job = ctx.scheduler.build_actions.get(job_name, None)
-                if job is None:
-                    continue
-                for output in job.outputs:
-                    try:
-                        s = os.stat(output)
-                        if stat.S_ISREG(s.st_mode):
-                            os.unlink(output)
-                        elif stat.S_ISDIR(s.st_mode):
-                            output_info(f"Removing directory: {output}")
-                            shutil.rmtree(output)
-                    except FileNotFoundError:
-                        pass
-            ctx.scheduler.shutdown()
-    except KeyboardInterrupt:
-        output_warning("Build was interrupted by user.")
-        return False
-    except KeyError as e:
-        output_error(f"Error: Action '{e}' not found.")
-        return False
-    finally:
-        ctx.scheduler.shutdown()
-
-    return True
-
-
-@dataclass
-class EntryPoint:
-    name: str
-    description: str
-
-
-NO_DESCRIPTION = "No description"
-
-
-def get_entrypoints(ctx: ByggContext) -> list[EntryPoint]:
-    return [
-        EntryPoint(x.name, x.description or NO_DESCRIPTION)
-        for x in ctx.scheduler.build_actions.values()
-        if x.is_entrypoint
-    ] or [
-        EntryPoint(x.name, x.description or NO_DESCRIPTION)
-        for x in ctx.configuration.actions
-        if x.is_entrypoint
-    ]
-
-
-list_actions_style = "B"
-
-
-def list_actions(ctx: ByggContext) -> bool:
-    entrypoints = get_entrypoints(ctx)
-
-    if not entrypoints:
-        program_name = os.path.basename(sys.argv[0])
-        output_error("Loaded build files but no entrypoints were found.")
-        output_error(f"Type `{program_name} --help` for help.")
-        return False
-
-    terminal_cols, terminal_rows = shutil.get_terminal_size()
-    output = [f"{TS.BOLD}Available actions:{TS.RESET}"]
-
-    sorted_actions = sorted(entrypoints, key=lambda x: x.name)
-    default_action_name = ctx.configuration.settings.default_action
-
-    if default_action_name:
-        default_action_list = [
-            x for x in sorted_actions if x.name == default_action_name
-        ]
-
-        if default_action_list:
-            default_action = default_action_list[0]
-            default_action_name = default_action.name
-            sorted_actions.remove(default_action)
-            sorted_actions.insert(0, default_action)
-
-    if list_actions_style == "A":
-        output.append("")
-        section_indent = 0
-        separator = " : "
-        max_name_width = max([len(x.name) for x in entrypoints])
-        width = min(terminal_cols, 80)
-        subsequent_indent = " " * (section_indent + max_name_width + len(separator))
-        for action in sorted_actions:
-            description = f"{TS.BOLD}{action.name: <{max_name_width}}{TS.RESET}{separator}{action.description}"
-            output.extend(
-                textwrap.wrap(
-                    description,
-                    width=width,
-                    initial_indent=" " * section_indent,
-                    subsequent_indent=subsequent_indent,
-                )
-            )
-            output.append("")
-
-    if list_actions_style == "B":
-        output.append("")
-        for action in sorted_actions:
-            default_action_suffix = (
-                " (default)" if action.name == default_action_name else ""
-            )
-            output.append(f"{TS.BOLD}{action.name}{default_action_suffix}{TS.RESET}")
-            output.append(
-                textwrap.fill(
-                    action.description,
-                    initial_indent="    ",
-                    subsequent_indent="    ",
-                )
-            )
-            output.append("")
-
-    print("\n".join(output))
-
-    return True
-
-
 def print_version():
     import importlib.metadata
 
     output_info(f"bygg {importlib.metadata.version('bygg')}")
 
 
 MAKE_COMPATIBLE_PANEL = "(Roughly) Make-compatible options"
@@ -485,14 +279,16 @@
         # spaces dealt with correctly:
         return {
             x.name: textwrap.fill(x.description, 7000) for x in eligible_entrypoints
         }
 
 
 def create_argument_parser():
+    logger.info("Creating argument parser")
+
     parser = argparse.ArgumentParser(
         formatter_class=argparse.RawDescriptionHelpFormatter,
         description="""
 A build tool written in Python, where all actions can be written in Python.
 
 Build the default action:
  %(prog)s
```

### Comparing `bygg-0.4.0/src/bygg/cmd/tree.py` & `bygg-0.4.1/src/bygg/cmd/tree.py`

 * *Files identical despite different names*

### Comparing `bygg-0.4.0/src/bygg/core/action.py` & `bygg-0.4.1/src/bygg/core/action.py`

 * *Files 16% similar despite different names*

```diff
@@ -112,15 +112,42 @@
     message: Optional[str] = None,
     inputs: Optional[Iterable[str]] = None,
     outputs: Optional[Iterable[str]] = None,
     dependencies: Optional[Iterable[str]] = None,
     dynamic_dependency: Optional[DynamicDependency] = None,
     is_entrypoint: bool = False,
 ):
-    """Decorator for creating an Action from a function."""
+    """Decorator to define a Bygg action.
+
+    Wraps the decorated function in an Action instance.
+
+    Parameters
+    ----------
+    name : str
+        The name of the action
+    message : str, optional
+        A message to display when the action is run, by default None
+    inputs : Iterable[str], optional
+        An iterable of input files, by default None
+    outputs : Iterable[str], optional
+        An iterable of output files, by default None
+    dependencies : Iterable[str], optional
+        An iterable of dependency actions, by default None
+    dynamic_dependency : DynamicDependency, optional
+        A dynamic dependency, by default None
+    is_entrypoint : bool, optional
+        Whether the action is an entrypoint, by default False
+    description : str, optional
+        A description of the action, by default None
+
+    Returns
+    -------
+    Callable[[Callable], Action]
+        A decorator that converts the decorated function into an Action
+    """
 
     def create_action(func: Callable):
         Action(
             name,
             message=message,
             inputs=inputs,
             outputs=outputs,
@@ -142,14 +169,34 @@
     dependencies: Optional[Iterable[str]] = None,
     is_entrypoint: bool = False,
 ):
     """
     Decorator for creating individual Actions from a list of input-output file pairs and
     a function. Creates one Action that depends on all of the individual Actions. It has
     name = base_name, which in turn can be used as a dependency for other Actions.
+
+    Parameters
+    ----------
+    base_name : str
+        Base name to use for generated actions
+    message : str, optional
+        Message for actions, by default None
+    file_pairs : Iterable[tuple[str, str]]
+        Input and output file pairs
+    extra_inputs : Iterable[str], optional
+        Extra input files, by default None
+    dependencies : Iterable[str], optional
+        Dependencies for actions, by default None
+    is_entrypoint : bool, optional
+        Whether the top-most action should be an entrypoint, by default False
+
+    Returns
+    -------
+    Callable[[Callable], None]
+        A decorator that registers actions constructed around the decorated function
     """
 
     def create_actions(func: Callable):
         action_list = []
         for input_file, output_file in file_pairs:
             action_name = f"{base_name}::{output_file}"
             action_list.append(action_name)
```

### Comparing `bygg-0.4.0/src/bygg/core/cache.py` & `bygg-0.4.1/src/bygg/core/cache.py`

 * *Files identical despite different names*

### Comparing `bygg-0.4.0/src/bygg/core/dag.py` & `bygg-0.4.1/src/bygg/core/dag.py`

 * *Files identical despite different names*

### Comparing `bygg-0.4.0/src/bygg/core/digest.py` & `bygg-0.4.1/src/bygg/core/digest.py`

 * *Files identical despite different names*

### Comparing `bygg-0.4.0/src/bygg/core/runner.py` & `bygg-0.4.1/src/bygg/core/runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -160,7 +160,18 @@
         if job.action.command is None:
             job.status = CommandStatus(0, "No command, skipping", None)
         else:
             job.status = job.action.command(job.action)
     except Exception as e:
         job.status = CommandStatus(1, "Job failed with exception.", f"{e}")
     return job
+
+
+def get_job_count_limit():
+    try:
+        # Use os.sched_getaffinity where available (on U**X):
+        # https://stackoverflow.com/a/55423170
+        return len(os.sched_getaffinity(0))
+    except AttributeError:
+        count = os.cpu_count()
+        assert count is not None
+        return count
```

### Comparing `bygg-0.4.0/src/bygg/core/scheduler.py` & `bygg-0.4.1/src/bygg/core/scheduler.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Literal
 
 from bygg.core.action import Action, CommandStatus
 from bygg.core.cache import Cache
 from bygg.core.dag import Dag, create_dag
 from bygg.core.digest import calculate_dependency_digest, calculate_digest
 from bygg.output.status_display import on_check_failed
+from loguru import logger
 import msgspec
 
 
 class Job:
     name: str
     action: Action
     status: CommandStatus | None
@@ -125,30 +126,30 @@
 
         if (
             len(action.inputs) == 0
             and len(action.outputs) == 0
             and not action.dynamic_dependency
         ):
             # An action with neither inputs nor outputs will always be built
-            # print(f"Job {job_name} is dirty (no inputs or outputs)")
+            logger.debug(f"Job '{job_name}' is dirty (no inputs or outputs)")
             return True
 
         if (
             not cached_digests
             or not cached_digests.outputs_digest
             or not cached_digests.inputs_digest
         ):
             # No previous result, so we need to build
-            # print(f"Job {job_name} is dirty (no previous result)")
+            logger.debug(f"Job '{job_name}' is dirty (no previous result)")
             return True
 
         outputs_digest, files_were_missing = calculate_dependency_digest(action.outputs)
         if files_were_missing or cached_digests.outputs_digest != outputs_digest:
             # The output has changed, so we need to rebuild
-            # print(f"Job {job_name} is dirty (output changed)")
+            logger.debug(f"Job '{job_name}' is dirty (output changed)")
             return True
 
         inputs_digest, files_were_missing = calculate_dependency_digest(
             action.dependency_files
         )
 
         # Calculate dynamic dependencies
@@ -157,24 +158,24 @@
                 return True
 
             dd_result = action.dynamic_dependency()
             if (
                 dd_result is None
                 or calculate_digest([dd_result]) != cached_digests.dynamic_digest
             ):
-                # print(f"Job {job_name} is dirty (dynamic dependency changed)")
+                logger.debug(f"Job '{job_name}' is dirty (dynamic dependency changed)")
                 return True
 
         # TODO handle files_were_missing here? abort?
         if cached_digests.inputs_digest != inputs_digest:
             # The inputs have changed, so we need to rebuild
-            # print(f"Job {job_name} is dirty (inputs changed)")
+            logger.debug(f"Job '{job_name}' is dirty (inputs changed)")
             return True
 
-        # print(f"Job {job_name} is clean")
+        logger.debug(f"Job '{job_name}' is clean")
         return False
 
     def get_ready_jobs(self, batch_size: int = 0) -> list[Job]:
         """
         Create a batch of jobs and put them in the running pool. Returns all ready jobs
         if batch_size is 0.
```

### Comparing `bygg-0.4.0/src/bygg/output/job_output.py` & `bygg-0.4.1/src/bygg/output/job_output.py`

 * *Files identical despite different names*

### Comparing `bygg-0.4.0/src/bygg/output/output.py` & `bygg-0.4.1/src/bygg/output/output.py`

 * *Files identical despite different names*

### Comparing `bygg-0.4.0/src/bygg/output/status_display.py` & `bygg-0.4.1/src/bygg/output/status_display.py`

 * *Files identical despite different names*

### Comparing `bygg-0.4.0/tests/conftest.py` & `bygg-0.4.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `bygg-0.4.0/tests/test_action.py` & `bygg-0.4.1/tests/test_action.py`

 * *Files identical despite different names*

### Comparing `bygg-0.4.0/tests/test_argument_unparsing.py` & `bygg-0.4.1/tests/test_argument_unparsing.py`

 * *Files identical despite different names*

### Comparing `bygg-0.4.0/tests/test_cache.py` & `bygg-0.4.1/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `bygg-0.4.0/tests/test_completions.py` & `bygg-0.4.1/tests/test_completions.py`

 * *Files identical despite different names*

### Comparing `bygg-0.4.0/tests/test_digest.py` & `bygg-0.4.1/tests/test_digest.py`

 * *Files identical despite different names*

### Comparing `bygg-0.4.0/tests/test_job_output.py` & `bygg-0.4.1/tests/test_job_output.py`

 * *Files identical despite different names*

### Comparing `bygg-0.4.0/tests/test_main.py` & `bygg-0.4.1/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `bygg-0.4.0/tests/test_scheduler.py` & `bygg-0.4.1/tests/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `bygg-0.4.0/tests/test_system_helpers.py` & `bygg-0.4.1/tests/test_system_helpers.py`

 * *Files identical despite different names*

### Comparing `bygg-0.4.0/tests/test_tree.py` & `bygg-0.4.1/tests/test_tree.py`

 * *Files identical despite different names*

### Comparing `bygg-0.4.0/tests/test_utils.py` & `bygg-0.4.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `bygg-0.4.0/tests/__snapshots__/test_completions.ambr` & `bygg-0.4.1/tests/__snapshots__/test_completions.ambr`

 * *Files identical despite different names*

### Comparing `bygg-0.4.0/tests/__snapshots__/test_job_output.ambr` & `bygg-0.4.1/tests/__snapshots__/test_job_output.ambr`

 * *Files identical despite different names*

### Comparing `bygg-0.4.0/tests/__snapshots__/test_main.ambr` & `bygg-0.4.1/tests/__snapshots__/test_main.ambr`

 * *Files identical despite different names*

### Comparing `bygg-0.4.0/LICENSE` & `bygg-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bygg-0.4.0/README.md` & `bygg-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `bygg-0.4.0/pyproject.toml` & `bygg-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bygg-0.4.0/PKG-INFO` & `bygg-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bygg
-Version: 0.4.0
+Version: 0.4.1
 Summary: A small build system
 Project-URL: Homepage, https://github.com/rikardg/bygg
 Project-URL: Bug Tracker, https://github.com/rikardg/bygg/issues
 Author-email: Rikard Gillemyr <rikard.gillemyr@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 rikardg
@@ -29,15 +29,16 @@
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Requires-Dist: argcomplete==3.3.0
 Requires-Dist: dill==0.3.8
-Requires-Dist: graph-theory==2023.7.6
+Requires-Dist: graph-theory==2023.7.7
+Requires-Dist: loguru==0.7.2
 Requires-Dist: msgspec==0.18.6
 Requires-Dist: multiprocess==0.70.16
 Requires-Dist: pyyaml==6.0.1
 Description-Content-Type: text/markdown
 
 <div align="center">
```

