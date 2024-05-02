# Comparing `tmp/hpcflow_new2-0.2.0a98.tar.gz` & `tmp/hpcflow_new2-0.2.0a99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hpcflow_new2-0.2.0a98.tar", max compression
+gzip compressed data, was "hpcflow_new2-0.2.0a99.tar", max compression
```

## Comparing `hpcflow_new2-0.2.0a98.tar` & `hpcflow_new2-0.2.0a99.tar`

### file list

```diff
@@ -1,127 +1,131 @@
--rw-r--r--   0        0        0      555 2023-09-18 14:12:10.202592 hpcflow_new2-0.2.0a98/README.md
--rw-r--r--   0        0        0       64 2023-09-18 14:12:10.206592 hpcflow_new2-0.2.0a98/hpcflow/__init__.py
--rw-r--r--   0        0        0       98 2023-09-18 14:12:10.206592 hpcflow_new2-0.2.0a98/hpcflow/__pyinstaller/__init__.py
--rw-r--r--   0        0        0      924 2023-09-18 14:12:10.206592 hpcflow_new2-0.2.0a98/hpcflow/__pyinstaller/hook-hpcflow.py
--rw-r--r--   0        0        0       25 2023-09-18 14:12:10.206592 hpcflow_new2-0.2.0a98/hpcflow/_version.py
--rw-r--r--   0        0        0     1392 2023-09-18 14:12:10.206592 hpcflow_new2-0.2.0a98/hpcflow/app.py
--rw-r--r--   0        0        0       66 2023-09-18 14:12:10.206592 hpcflow_new2-0.2.0a98/hpcflow/cli.py
--rw-r--r--   0        0        0    28553 2023-09-18 14:12:10.206592 hpcflow_new2-0.2.0a98/hpcflow/examples.ipynb
--rw-r--r--   0        0        0     5606 2023-09-18 14:12:10.206592 hpcflow_new2-0.2.0a98/hpcflow/sdk/__init__.py
--rw-r--r--   0        0        0    68808 2023-09-18 14:12:10.206592 hpcflow_new2-0.2.0a98/hpcflow/sdk/app.py
--rw-r--r--   0        0        0    26248 2023-09-18 14:12:10.206592 hpcflow_new2-0.2.0a98/hpcflow/sdk/cli.py
--rw-r--r--   0        0        0     2487 2023-09-18 14:12:10.206592 hpcflow_new2-0.2.0a98/hpcflow/sdk/cli_common.py
--rw-r--r--   0        0        0       70 2023-09-18 14:12:10.206592 hpcflow_new2-0.2.0a98/hpcflow/sdk/config/__init__.py
--rw-r--r--   0        0        0     5339 2023-09-18 14:12:10.206592 hpcflow_new2-0.2.0a98/hpcflow/sdk/config/callbacks.py
--rw-r--r--   0        0        0     9656 2023-09-18 14:12:10.206592 hpcflow_new2-0.2.0a98/hpcflow/sdk/config/cli.py
--rw-r--r--   0        0        0    29176 2023-09-18 14:12:10.206592 hpcflow_new2-0.2.0a98/hpcflow/sdk/config/config.py
--rw-r--r--   0        0        0    12373 2023-09-18 14:12:10.206592 hpcflow_new2-0.2.0a98/hpcflow/sdk/config/config_file.py
--rw-r--r--   0        0        0     6876 2023-09-18 14:12:10.206592 hpcflow_new2-0.2.0a98/hpcflow/sdk/config/errors.py
--rw-r--r--   0        0        0      215 2023-09-18 14:12:10.206592 hpcflow_new2-0.2.0a98/hpcflow/sdk/core/__init__.py
--rw-r--r--   0        0        0    60949 2023-09-18 14:12:10.206592 hpcflow_new2-0.2.0a98/hpcflow/sdk/core/actions.py
--rw-r--r--   0        0        0    17139 2023-09-18 14:12:10.206592 hpcflow_new2-0.2.0a98/hpcflow/sdk/core/command_files.py
--rw-r--r--   0        0        0     5386 2023-09-18 14:12:10.206592 hpcflow_new2-0.2.0a98/hpcflow/sdk/core/commands.py
--rw-r--r--   0        0        0    43184 2023-09-18 14:12:10.206592 hpcflow_new2-0.2.0a98/hpcflow/sdk/core/element.py
--rw-r--r--   0        0        0     4849 2023-09-18 14:12:10.206592 hpcflow_new2-0.2.0a98/hpcflow/sdk/core/environment.py
--rw-r--r--   0        0        0     7669 2023-09-18 14:12:10.206592 hpcflow_new2-0.2.0a98/hpcflow/sdk/core/errors.py
--rw-r--r--   0        0        0    18597 2023-09-18 14:12:10.206592 hpcflow_new2-0.2.0a98/hpcflow/sdk/core/json_like.py
--rw-r--r--   0        0        0    18077 2023-09-18 14:12:10.206592 hpcflow_new2-0.2.0a98/hpcflow/sdk/core/loop.py
--rw-r--r--   0        0        0    18775 2023-09-18 14:12:10.206592 hpcflow_new2-0.2.0a98/hpcflow/sdk/core/object_list.py
--rw-r--r--   0        0        0    58206 2023-09-18 14:12:10.206592 hpcflow_new2-0.2.0a98/hpcflow/sdk/core/parameters.py
--rw-r--r--   0        0        0    92106 2023-09-18 14:12:10.206592 hpcflow_new2-0.2.0a98/hpcflow/sdk/core/task.py
--rw-r--r--   0        0        0    12031 2023-09-18 14:12:10.206592 hpcflow_new2-0.2.0a98/hpcflow/sdk/core/task_schema.py
--rw-r--r--   0        0        0     4685 2023-09-18 14:12:10.206592 hpcflow_new2-0.2.0a98/hpcflow/sdk/core/test_utils.py
--rw-r--r--   0        0        0    19305 2023-09-18 14:12:10.206592 hpcflow_new2-0.2.0a98/hpcflow/sdk/core/utils.py
--rw-r--r--   0        0        0      518 2023-09-18 14:12:10.206592 hpcflow_new2-0.2.0a98/hpcflow/sdk/core/validation.py
--rw-r--r--   0        0        0    87569 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/sdk/core/workflow.py
--rw-r--r--   0        0        0     5724 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/sdk/core/zarr_io.py
--rw-r--r--   0        0        0        0 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/sdk/data/__init__.py
--rw-r--r--   0        0        0      791 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/sdk/data/config_file_schema.yaml
--rw-r--r--   0        0        0     5783 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/sdk/data/config_schema.yaml
--rw-r--r--   0        0        0      790 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/sdk/data/environments_spec_schema.yaml
--rw-r--r--   0        0        0      165 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/sdk/data/files_spec_schema.yaml
--rw-r--r--   0        0        0      148 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/sdk/data/parameters_spec_schema.yaml
--rw-r--r--   0        0        0       93 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/sdk/data/task_schema_spec_schema.yaml
--rw-r--r--   0        0        0       83 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/sdk/data/template_components/__init__.py
--rw-r--r--   0        0        0      356 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/sdk/data/template_components/command_files.yaml
--rw-r--r--   0        0        0       17 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/sdk/data/template_components/environments.yaml
--rw-r--r--   0        0        0      199 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/sdk/data/template_components/parameters.yaml
--rw-r--r--   0        0        0     3261 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/sdk/data/template_components/task_schemas.yaml
--rw-r--r--   0        0        0     1797 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/sdk/data/workflow_spec_schema.yaml
--rw-r--r--   0        0        0        0 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/sdk/demo/__init__.py
--rw-r--r--   0        0        0     4937 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/sdk/demo/cli.py
--rw-r--r--   0        0        0        0 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/sdk/demo/data/__init__.py
--rw-r--r--   0        0        0      138 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/sdk/demo/data/workflow_1.json
--rw-r--r--   0        0        0       88 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/sdk/demo/data/workflow_1.yaml
--rw-r--r--   0        0        0      127 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/sdk/demo/data/workflow_1_slurm.yaml
--rw-r--r--   0        0        0      111 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/sdk/demo/data/workflow_1_wsl.yaml
--rw-r--r--   0        0        0     1376 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/sdk/demo/data/workflow_test_run_abort.yaml
--rw-r--r--   0        0        0       80 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/sdk/demo/scripts/__init__.py
--rw-r--r--   0        0        0      212 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/sdk/demo/scripts/demo_task_1_generate_t1_infile_1.py
--rw-r--r--   0        0        0      212 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/sdk/demo/scripts/demo_task_1_generate_t1_infile_2.py
--rw-r--r--   0        0        0      166 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/sdk/demo/scripts/demo_task_1_parse_p3.py
--rw-r--r--   0        0        0      168 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/sdk/demo/scripts/generate_t1_file_01.py
--rw-r--r--   0        0        0      125 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/sdk/demo/scripts/parse_t1_file_01.py
--rw-r--r--   0        0        0        0 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/sdk/demo/scripts/test_main_script.py
--rw-r--r--   0        0        0        0 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/sdk/demo/workflows/__init__.py
--rw-r--r--   0        0        0      223 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/sdk/demo/workflows/workflow_1.yaml
--rw-r--r--   0        0        0        0 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/sdk/helper/__init__.py
--rw-r--r--   0        0        0     3491 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/sdk/helper/cli.py
--rw-r--r--   0        0        0     8143 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/sdk/helper/helper.py
--rw-r--r--   0        0        0     4003 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/sdk/helper/watcher.py
--rw-r--r--   0        0        0     1925 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/sdk/log.py
--rw-r--r--   0        0        0      900 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/sdk/persistence/__init__.py
--rw-r--r--   0        0        0    55469 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/sdk/persistence/base.py
--rw-r--r--   0        0        0    19415 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/sdk/persistence/json.py
--rw-r--r--   0        0        0    22879 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/sdk/persistence/pending.py
--rw-r--r--   0        0        0     4307 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/sdk/persistence/store_resource.py
--rw-r--r--   0        0        0     1517 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/sdk/persistence/utils.py
--rw-r--r--   0        0        0    38567 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/sdk/persistence/zarr.py
--rw-r--r--   0        0        0     9164 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/sdk/runtime.py
--rw-r--r--   0        0        0      110 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/sdk/scripting/__init__.py
--rw-r--r--   0        0        0        0 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/sdk/submission/__init__.py
--rw-r--r--   0        0        0    43636 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/sdk/submission/jobscript.py
--rw-r--r--   0        0        0     1168 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/sdk/submission/jobscript_info.py
--rw-r--r--   0        0        0     2436 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/sdk/submission/schedulers/__init__.py
--rw-r--r--   0        0        0     5539 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/sdk/submission/schedulers/direct.py
--rw-r--r--   0        0        0    10502 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/sdk/submission/schedulers/sge.py
--rw-r--r--   0        0        0    21278 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/sdk/submission/schedulers/slurm.py
--rw-r--r--   0        0        0      364 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/sdk/submission/schedulers/utils.py
--rw-r--r--   0        0        0     1169 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/sdk/submission/shells/__init__.py
--rw-r--r--   0        0        0     2302 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/sdk/submission/shells/base.py
--rw-r--r--   0        0        0    10307 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/sdk/submission/shells/bash.py
--rw-r--r--   0        0        0     3182 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/sdk/submission/shells/os_version.py
--rw-r--r--   0        0        0     8461 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/sdk/submission/shells/powershell.py
--rw-r--r--   0        0        0    17315 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/sdk/submission/submission.py
--rw-r--r--   0        0        0      327 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/sdk/typing.py
--rw-r--r--   0        0        0     2616 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/tests/conftest.py
--rw-r--r--   0        0        0      459 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/tests/schedulers/direct_linux/test_direct_linux_submission.py
--rw-r--r--   0        0        0      442 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/tests/schedulers/slurm/test_slurm_submission.py
--rw-r--r--   0        0        0      589 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/tests/shells/wsl/test_wsl_submission.py
--rw-r--r--   0        0        0     4987 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/tests/unit/test_action.py
--rw-r--r--   0        0        0     2916 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/tests/unit/test_app.py
--rw-r--r--   0        0        0      288 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/tests/unit/test_cli.py
--rw-r--r--   0        0        0     2471 2023-09-18 14:12:10.210592 hpcflow_new2-0.2.0a98/hpcflow/tests/unit/test_config.py
--rw-r--r--   0        0        0     4375 2023-09-18 14:12:10.214593 hpcflow_new2-0.2.0a98/hpcflow/tests/unit/test_config_file.py
--rw-r--r--   0        0        0     1572 2023-09-18 14:12:10.214593 hpcflow_new2-0.2.0a98/hpcflow/tests/unit/test_element.py
--rw-r--r--   0        0        0     1853 2023-09-18 14:12:10.214593 hpcflow_new2-0.2.0a98/hpcflow/tests/unit/test_element_set.py
--rw-r--r--   0        0        0     9607 2023-09-18 14:12:10.214593 hpcflow_new2-0.2.0a98/hpcflow/tests/unit/test_input_source.py
--rw-r--r--   0        0        0     4564 2023-09-18 14:12:10.214593 hpcflow_new2-0.2.0a98/hpcflow/tests/unit/test_input_value.py
--rw-r--r--   0        0        0    29939 2023-09-18 14:12:10.214593 hpcflow_new2-0.2.0a98/hpcflow/tests/unit/test_json_like.py
--rw-r--r--   0        0        0     8615 2023-09-18 14:12:10.214593 hpcflow_new2-0.2.0a98/hpcflow/tests/unit/test_loop.py
--rw-r--r--   0        0        0     2193 2023-09-18 14:12:10.214593 hpcflow_new2-0.2.0a98/hpcflow/tests/unit/test_object_list.py
--rw-r--r--   0        0        0     7422 2023-09-18 14:12:10.214593 hpcflow_new2-0.2.0a98/hpcflow/tests/unit/test_persistence.py
--rw-r--r--   0        0        0     7310 2023-09-18 14:12:10.214593 hpcflow_new2-0.2.0a98/hpcflow/tests/unit/test_resources.py
--rw-r--r--   0        0        0      313 2023-09-18 14:12:10.214593 hpcflow_new2-0.2.0a98/hpcflow/tests/unit/test_runtime.py
--rw-r--r--   0        0        0     6387 2023-09-18 14:12:10.214593 hpcflow_new2-0.2.0a98/hpcflow/tests/unit/test_schema_input.py
--rw-r--r--   0        0        0     3442 2023-09-18 14:12:10.214593 hpcflow_new2-0.2.0a98/hpcflow/tests/unit/test_shell.py
--rw-r--r--   0        0        0     5825 2023-09-18 14:12:10.214593 hpcflow_new2-0.2.0a98/hpcflow/tests/unit/test_submission.py
--rw-r--r--   0        0        0    53920 2023-09-18 14:12:10.214593 hpcflow_new2-0.2.0a98/hpcflow/tests/unit/test_task.py
--rw-r--r--   0        0        0     3624 2023-09-18 14:12:10.214593 hpcflow_new2-0.2.0a98/hpcflow/tests/unit/test_task_schema.py
--rw-r--r--   0        0        0    11200 2023-09-18 14:12:10.214593 hpcflow_new2-0.2.0a98/hpcflow/tests/unit/test_utils.py
--rw-r--r--   0        0        0     7330 2023-09-18 14:12:10.214593 hpcflow_new2-0.2.0a98/hpcflow/tests/unit/test_value_sequence.py
--rw-r--r--   0        0        0    21596 2023-09-18 14:12:10.214593 hpcflow_new2-0.2.0a98/hpcflow/tests/unit/test_workflow.py
--rw-r--r--   0        0        0      964 2023-09-18 14:12:10.214593 hpcflow_new2-0.2.0a98/hpcflow/tests/unit/test_workflow_template.py
--rw-r--r--   0        0        0     1756 2023-09-18 14:12:10.214593 hpcflow_new2-0.2.0a98/hpcflow/tests/workflows/test_workflows.py
--rw-r--r--   0        0        0     6238 2023-09-18 14:12:10.214593 hpcflow_new2-0.2.0a98/hpcflow/viz_demo.ipynb
--rw-r--r--   0        0        0     1769 2023-09-18 14:12:10.214593 hpcflow_new2-0.2.0a98/pyproject.toml
--rw-r--r--   0        0        0     1878 1970-01-01 00:00:00.000000 hpcflow_new2-0.2.0a98/PKG-INFO
+-rw-r--r--   0        0        0      555 2023-09-19 19:58:05.400182 hpcflow_new2-0.2.0a99/README.md
+-rw-r--r--   0        0        0       64 2023-09-19 19:58:05.404182 hpcflow_new2-0.2.0a99/hpcflow/__init__.py
+-rw-r--r--   0        0        0       98 2023-09-19 19:58:05.404182 hpcflow_new2-0.2.0a99/hpcflow/__pyinstaller/__init__.py
+-rw-r--r--   0        0        0      924 2023-09-19 19:58:05.404182 hpcflow_new2-0.2.0a99/hpcflow/__pyinstaller/hook-hpcflow.py
+-rw-r--r--   0        0        0       25 2023-09-19 19:58:05.404182 hpcflow_new2-0.2.0a99/hpcflow/_version.py
+-rw-r--r--   0        0        0     1392 2023-09-19 19:58:05.404182 hpcflow_new2-0.2.0a99/hpcflow/app.py
+-rw-r--r--   0        0        0       66 2023-09-19 19:58:05.404182 hpcflow_new2-0.2.0a99/hpcflow/cli.py
+-rw-r--r--   0        0        0    28553 2023-09-19 19:58:05.404182 hpcflow_new2-0.2.0a99/hpcflow/examples.ipynb
+-rw-r--r--   0        0        0     5643 2023-09-19 19:58:05.404182 hpcflow_new2-0.2.0a99/hpcflow/sdk/__init__.py
+-rw-r--r--   0        0        0    68808 2023-09-19 19:58:05.404182 hpcflow_new2-0.2.0a99/hpcflow/sdk/app.py
+-rw-r--r--   0        0        0    26931 2023-09-19 19:58:05.404182 hpcflow_new2-0.2.0a99/hpcflow/sdk/cli.py
+-rw-r--r--   0        0        0     2487 2023-09-19 19:58:05.404182 hpcflow_new2-0.2.0a99/hpcflow/sdk/cli_common.py
+-rw-r--r--   0        0        0       70 2023-09-19 19:58:05.404182 hpcflow_new2-0.2.0a99/hpcflow/sdk/config/__init__.py
+-rw-r--r--   0        0        0     5339 2023-09-19 19:58:05.408182 hpcflow_new2-0.2.0a99/hpcflow/sdk/config/callbacks.py
+-rw-r--r--   0        0        0     9656 2023-09-19 19:58:05.408182 hpcflow_new2-0.2.0a99/hpcflow/sdk/config/cli.py
+-rw-r--r--   0        0        0    29176 2023-09-19 19:58:05.408182 hpcflow_new2-0.2.0a99/hpcflow/sdk/config/config.py
+-rw-r--r--   0        0        0    12373 2023-09-19 19:58:05.408182 hpcflow_new2-0.2.0a99/hpcflow/sdk/config/config_file.py
+-rw-r--r--   0        0        0     6876 2023-09-19 19:58:05.408182 hpcflow_new2-0.2.0a99/hpcflow/sdk/config/errors.py
+-rw-r--r--   0        0        0      215 2023-09-19 19:58:05.408182 hpcflow_new2-0.2.0a99/hpcflow/sdk/core/__init__.py
+-rw-r--r--   0        0        0    63058 2023-09-19 19:58:05.408182 hpcflow_new2-0.2.0a99/hpcflow/sdk/core/actions.py
+-rw-r--r--   0        0        0    17139 2023-09-19 19:58:05.408182 hpcflow_new2-0.2.0a99/hpcflow/sdk/core/command_files.py
+-rw-r--r--   0        0        0    11061 2023-09-19 19:58:05.408182 hpcflow_new2-0.2.0a99/hpcflow/sdk/core/commands.py
+-rw-r--r--   0        0        0    44526 2023-09-19 19:58:05.408182 hpcflow_new2-0.2.0a99/hpcflow/sdk/core/element.py
+-rw-r--r--   0        0        0     4849 2023-09-19 19:58:05.408182 hpcflow_new2-0.2.0a99/hpcflow/sdk/core/environment.py
+-rw-r--r--   0        0        0     8048 2023-09-19 19:58:05.408182 hpcflow_new2-0.2.0a99/hpcflow/sdk/core/errors.py
+-rw-r--r--   0        0        0    18597 2023-09-19 19:58:05.408182 hpcflow_new2-0.2.0a99/hpcflow/sdk/core/json_like.py
+-rw-r--r--   0        0        0    18077 2023-09-19 19:58:05.408182 hpcflow_new2-0.2.0a99/hpcflow/sdk/core/loop.py
+-rw-r--r--   0        0        0    18775 2023-09-19 19:58:05.408182 hpcflow_new2-0.2.0a99/hpcflow/sdk/core/object_list.py
+-rw-r--r--   0        0        0    60249 2023-09-19 19:58:05.408182 hpcflow_new2-0.2.0a99/hpcflow/sdk/core/parameters.py
+-rw-r--r--   0        0        0     4461 2023-09-19 19:58:05.408182 hpcflow_new2-0.2.0a99/hpcflow/sdk/core/rule.py
+-rw-r--r--   0        0        0   101965 2023-09-19 19:58:05.408182 hpcflow_new2-0.2.0a99/hpcflow/sdk/core/task.py
+-rw-r--r--   0        0        0    12716 2023-09-19 19:58:05.408182 hpcflow_new2-0.2.0a99/hpcflow/sdk/core/task_schema.py
+-rw-r--r--   0        0        0     6663 2023-09-19 19:58:05.408182 hpcflow_new2-0.2.0a99/hpcflow/sdk/core/test_utils.py
+-rw-r--r--   0        0        0    19836 2023-09-19 19:58:05.408182 hpcflow_new2-0.2.0a99/hpcflow/sdk/core/utils.py
+-rw-r--r--   0        0        0      518 2023-09-19 19:58:05.408182 hpcflow_new2-0.2.0a99/hpcflow/sdk/core/validation.py
+-rw-r--r--   0        0        0    88360 2023-09-19 19:58:05.408182 hpcflow_new2-0.2.0a99/hpcflow/sdk/core/workflow.py
+-rw-r--r--   0        0        0     5724 2023-09-19 19:58:05.408182 hpcflow_new2-0.2.0a99/hpcflow/sdk/core/zarr_io.py
+-rw-r--r--   0        0        0        0 2023-09-19 19:58:05.408182 hpcflow_new2-0.2.0a99/hpcflow/sdk/data/__init__.py
+-rw-r--r--   0        0        0      791 2023-09-19 19:58:05.412182 hpcflow_new2-0.2.0a99/hpcflow/sdk/data/config_file_schema.yaml
+-rw-r--r--   0        0        0     5783 2023-09-19 19:58:05.412182 hpcflow_new2-0.2.0a99/hpcflow/sdk/data/config_schema.yaml
+-rw-r--r--   0        0        0      790 2023-09-19 19:58:05.412182 hpcflow_new2-0.2.0a99/hpcflow/sdk/data/environments_spec_schema.yaml
+-rw-r--r--   0        0        0      165 2023-09-19 19:58:05.412182 hpcflow_new2-0.2.0a99/hpcflow/sdk/data/files_spec_schema.yaml
+-rw-r--r--   0        0        0      148 2023-09-19 19:58:05.412182 hpcflow_new2-0.2.0a99/hpcflow/sdk/data/parameters_spec_schema.yaml
+-rw-r--r--   0        0        0       93 2023-09-19 19:58:05.412182 hpcflow_new2-0.2.0a99/hpcflow/sdk/data/task_schema_spec_schema.yaml
+-rw-r--r--   0        0        0       83 2023-09-19 19:58:05.412182 hpcflow_new2-0.2.0a99/hpcflow/sdk/data/template_components/__init__.py
+-rw-r--r--   0        0        0      356 2023-09-19 19:58:05.412182 hpcflow_new2-0.2.0a99/hpcflow/sdk/data/template_components/command_files.yaml
+-rw-r--r--   0        0        0       17 2023-09-19 19:58:05.412182 hpcflow_new2-0.2.0a99/hpcflow/sdk/data/template_components/environments.yaml
+-rw-r--r--   0        0        0      211 2023-09-19 19:58:05.412182 hpcflow_new2-0.2.0a99/hpcflow/sdk/data/template_components/parameters.yaml
+-rw-r--r--   0        0        0     3217 2023-09-19 19:58:05.412182 hpcflow_new2-0.2.0a99/hpcflow/sdk/data/template_components/task_schemas.yaml
+-rw-r--r--   0        0        0     1797 2023-09-19 19:58:05.412182 hpcflow_new2-0.2.0a99/hpcflow/sdk/data/workflow_spec_schema.yaml
+-rw-r--r--   0        0        0        0 2023-09-19 19:58:05.412182 hpcflow_new2-0.2.0a99/hpcflow/sdk/demo/__init__.py
+-rw-r--r--   0        0        0     4937 2023-09-19 19:58:05.412182 hpcflow_new2-0.2.0a99/hpcflow/sdk/demo/cli.py
+-rw-r--r--   0        0        0        0 2023-09-19 19:58:05.412182 hpcflow_new2-0.2.0a99/hpcflow/sdk/demo/data/__init__.py
+-rw-r--r--   0        0        0      138 2023-09-19 19:58:05.412182 hpcflow_new2-0.2.0a99/hpcflow/sdk/demo/data/workflow_1.json
+-rw-r--r--   0        0        0       88 2023-09-19 19:58:05.412182 hpcflow_new2-0.2.0a99/hpcflow/sdk/demo/data/workflow_1.yaml
+-rw-r--r--   0        0        0      127 2023-09-19 19:58:05.412182 hpcflow_new2-0.2.0a99/hpcflow/sdk/demo/data/workflow_1_slurm.yaml
+-rw-r--r--   0        0        0      111 2023-09-19 19:58:05.412182 hpcflow_new2-0.2.0a99/hpcflow/sdk/demo/data/workflow_1_wsl.yaml
+-rw-r--r--   0        0        0     1280 2023-09-19 19:58:05.412182 hpcflow_new2-0.2.0a99/hpcflow/sdk/demo/data/workflow_test_run_abort.yaml
+-rw-r--r--   0        0        0       80 2023-09-19 19:58:05.412182 hpcflow_new2-0.2.0a99/hpcflow/sdk/demo/scripts/__init__.py
+-rw-r--r--   0        0        0      212 2023-09-19 19:58:05.412182 hpcflow_new2-0.2.0a99/hpcflow/sdk/demo/scripts/demo_task_1_generate_t1_infile_1.py
+-rw-r--r--   0        0        0      212 2023-09-19 19:58:05.412182 hpcflow_new2-0.2.0a99/hpcflow/sdk/demo/scripts/demo_task_1_generate_t1_infile_2.py
+-rw-r--r--   0        0        0      166 2023-09-19 19:58:05.412182 hpcflow_new2-0.2.0a99/hpcflow/sdk/demo/scripts/demo_task_1_parse_p3.py
+-rw-r--r--   0        0        0      168 2023-09-19 19:58:05.412182 hpcflow_new2-0.2.0a99/hpcflow/sdk/demo/scripts/generate_t1_file_01.py
+-rw-r--r--   0        0        0      125 2023-09-19 19:58:05.412182 hpcflow_new2-0.2.0a99/hpcflow/sdk/demo/scripts/parse_t1_file_01.py
+-rw-r--r--   0        0        0        0 2023-09-19 19:58:05.412182 hpcflow_new2-0.2.0a99/hpcflow/sdk/demo/scripts/test_main_script.py
+-rw-r--r--   0        0        0        0 2023-09-19 19:58:05.412182 hpcflow_new2-0.2.0a99/hpcflow/sdk/demo/workflows/__init__.py
+-rw-r--r--   0        0        0      223 2023-09-19 19:58:05.412182 hpcflow_new2-0.2.0a99/hpcflow/sdk/demo/workflows/workflow_1.yaml
+-rw-r--r--   0        0        0        0 2023-09-19 19:58:05.412182 hpcflow_new2-0.2.0a99/hpcflow/sdk/helper/__init__.py
+-rw-r--r--   0        0        0     3491 2023-09-19 19:58:05.412182 hpcflow_new2-0.2.0a99/hpcflow/sdk/helper/cli.py
+-rw-r--r--   0        0        0     8143 2023-09-19 19:58:05.412182 hpcflow_new2-0.2.0a99/hpcflow/sdk/helper/helper.py
+-rw-r--r--   0        0        0     4003 2023-09-19 19:58:05.412182 hpcflow_new2-0.2.0a99/hpcflow/sdk/helper/watcher.py
+-rw-r--r--   0        0        0     1925 2023-09-19 19:58:05.412182 hpcflow_new2-0.2.0a99/hpcflow/sdk/log.py
+-rw-r--r--   0        0        0      900 2023-09-19 19:58:05.412182 hpcflow_new2-0.2.0a99/hpcflow/sdk/persistence/__init__.py
+-rw-r--r--   0        0        0    55469 2023-09-19 19:58:05.412182 hpcflow_new2-0.2.0a99/hpcflow/sdk/persistence/base.py
+-rw-r--r--   0        0        0    19415 2023-09-19 19:58:05.412182 hpcflow_new2-0.2.0a99/hpcflow/sdk/persistence/json.py
+-rw-r--r--   0        0        0    22879 2023-09-19 19:58:05.412182 hpcflow_new2-0.2.0a99/hpcflow/sdk/persistence/pending.py
+-rw-r--r--   0        0        0     4307 2023-09-19 19:58:05.412182 hpcflow_new2-0.2.0a99/hpcflow/sdk/persistence/store_resource.py
+-rw-r--r--   0        0        0     1517 2023-09-19 19:58:05.412182 hpcflow_new2-0.2.0a99/hpcflow/sdk/persistence/utils.py
+-rw-r--r--   0        0        0    38567 2023-09-19 19:58:05.412182 hpcflow_new2-0.2.0a99/hpcflow/sdk/persistence/zarr.py
+-rw-r--r--   0        0        0     9164 2023-09-19 19:58:05.412182 hpcflow_new2-0.2.0a99/hpcflow/sdk/runtime.py
+-rw-r--r--   0        0        0      110 2023-09-19 19:58:05.412182 hpcflow_new2-0.2.0a99/hpcflow/sdk/scripting/__init__.py
+-rw-r--r--   0        0        0        0 2023-09-19 19:58:05.412182 hpcflow_new2-0.2.0a99/hpcflow/sdk/submission/__init__.py
+-rw-r--r--   0        0        0    43636 2023-09-19 19:58:05.412182 hpcflow_new2-0.2.0a99/hpcflow/sdk/submission/jobscript.py
+-rw-r--r--   0        0        0     1168 2023-09-19 19:58:05.412182 hpcflow_new2-0.2.0a99/hpcflow/sdk/submission/jobscript_info.py
+-rw-r--r--   0        0        0     2436 2023-09-19 19:58:05.412182 hpcflow_new2-0.2.0a99/hpcflow/sdk/submission/schedulers/__init__.py
+-rw-r--r--   0        0        0     5539 2023-09-19 19:58:05.412182 hpcflow_new2-0.2.0a99/hpcflow/sdk/submission/schedulers/direct.py
+-rw-r--r--   0        0        0    10502 2023-09-19 19:58:05.412182 hpcflow_new2-0.2.0a99/hpcflow/sdk/submission/schedulers/sge.py
+-rw-r--r--   0        0        0    21278 2023-09-19 19:58:05.416182 hpcflow_new2-0.2.0a99/hpcflow/sdk/submission/schedulers/slurm.py
+-rw-r--r--   0        0        0      364 2023-09-19 19:58:05.416182 hpcflow_new2-0.2.0a99/hpcflow/sdk/submission/schedulers/utils.py
+-rw-r--r--   0        0        0     1169 2023-09-19 19:58:05.416182 hpcflow_new2-0.2.0a99/hpcflow/sdk/submission/shells/__init__.py
+-rw-r--r--   0        0        0     2302 2023-09-19 19:58:05.416182 hpcflow_new2-0.2.0a99/hpcflow/sdk/submission/shells/base.py
+-rw-r--r--   0        0        0    10604 2023-09-19 19:58:05.416182 hpcflow_new2-0.2.0a99/hpcflow/sdk/submission/shells/bash.py
+-rw-r--r--   0        0        0     3182 2023-09-19 19:58:05.416182 hpcflow_new2-0.2.0a99/hpcflow/sdk/submission/shells/os_version.py
+-rw-r--r--   0        0        0     8758 2023-09-19 19:58:05.416182 hpcflow_new2-0.2.0a99/hpcflow/sdk/submission/shells/powershell.py
+-rw-r--r--   0        0        0    17315 2023-09-19 19:58:05.416182 hpcflow_new2-0.2.0a99/hpcflow/sdk/submission/submission.py
+-rw-r--r--   0        0        0      327 2023-09-19 19:58:05.416182 hpcflow_new2-0.2.0a99/hpcflow/sdk/typing.py
+-rw-r--r--   0        0        0     2616 2023-09-19 19:58:05.416182 hpcflow_new2-0.2.0a99/hpcflow/tests/conftest.py
+-rw-r--r--   0        0        0      459 2023-09-19 19:58:05.416182 hpcflow_new2-0.2.0a99/hpcflow/tests/schedulers/direct_linux/test_direct_linux_submission.py
+-rw-r--r--   0        0        0      442 2023-09-19 19:58:05.416182 hpcflow_new2-0.2.0a99/hpcflow/tests/schedulers/slurm/test_slurm_submission.py
+-rw-r--r--   0        0        0      589 2023-09-19 19:58:05.416182 hpcflow_new2-0.2.0a99/hpcflow/tests/shells/wsl/test_wsl_submission.py
+-rw-r--r--   0        0        0     7841 2023-09-19 19:58:05.416182 hpcflow_new2-0.2.0a99/hpcflow/tests/unit/test_action.py
+-rw-r--r--   0        0        0      547 2023-09-19 19:58:05.416182 hpcflow_new2-0.2.0a99/hpcflow/tests/unit/test_action_rule.py
+-rw-r--r--   0        0        0     2916 2023-09-19 19:58:05.416182 hpcflow_new2-0.2.0a99/hpcflow/tests/unit/test_app.py
+-rw-r--r--   0        0        0      288 2023-09-19 19:58:05.416182 hpcflow_new2-0.2.0a99/hpcflow/tests/unit/test_cli.py
+-rw-r--r--   0        0        0    22129 2023-09-19 19:58:05.416182 hpcflow_new2-0.2.0a99/hpcflow/tests/unit/test_command.py
+-rw-r--r--   0        0        0     2471 2023-09-19 19:58:05.416182 hpcflow_new2-0.2.0a99/hpcflow/tests/unit/test_config.py
+-rw-r--r--   0        0        0     4375 2023-09-19 19:58:05.416182 hpcflow_new2-0.2.0a99/hpcflow/tests/unit/test_config_file.py
+-rw-r--r--   0        0        0    13960 2023-09-19 19:58:05.416182 hpcflow_new2-0.2.0a99/hpcflow/tests/unit/test_element.py
+-rw-r--r--   0        0        0     1853 2023-09-19 19:58:05.416182 hpcflow_new2-0.2.0a99/hpcflow/tests/unit/test_element_set.py
+-rw-r--r--   0        0        0    20487 2023-09-19 19:58:05.416182 hpcflow_new2-0.2.0a99/hpcflow/tests/unit/test_input_source.py
+-rw-r--r--   0        0        0     5253 2023-09-19 19:58:05.416182 hpcflow_new2-0.2.0a99/hpcflow/tests/unit/test_input_value.py
+-rw-r--r--   0        0        0    29939 2023-09-19 19:58:05.416182 hpcflow_new2-0.2.0a99/hpcflow/tests/unit/test_json_like.py
+-rw-r--r--   0        0        0     8615 2023-09-19 19:58:05.416182 hpcflow_new2-0.2.0a99/hpcflow/tests/unit/test_loop.py
+-rw-r--r--   0        0        0     2193 2023-09-19 19:58:05.416182 hpcflow_new2-0.2.0a99/hpcflow/tests/unit/test_object_list.py
+-rw-r--r--   0        0        0     2509 2023-09-19 19:58:05.416182 hpcflow_new2-0.2.0a99/hpcflow/tests/unit/test_parameter.py
+-rw-r--r--   0        0        0     7422 2023-09-19 19:58:05.416182 hpcflow_new2-0.2.0a99/hpcflow/tests/unit/test_persistence.py
+-rw-r--r--   0        0        0     7310 2023-09-19 19:58:05.416182 hpcflow_new2-0.2.0a99/hpcflow/tests/unit/test_resources.py
+-rw-r--r--   0        0        0      313 2023-09-19 19:58:05.416182 hpcflow_new2-0.2.0a99/hpcflow/tests/unit/test_runtime.py
+-rw-r--r--   0        0        0     6437 2023-09-19 19:58:05.416182 hpcflow_new2-0.2.0a99/hpcflow/tests/unit/test_schema_input.py
+-rw-r--r--   0        0        0     3442 2023-09-19 19:58:05.416182 hpcflow_new2-0.2.0a99/hpcflow/tests/unit/test_shell.py
+-rw-r--r--   0        0        0     5825 2023-09-19 19:58:05.416182 hpcflow_new2-0.2.0a99/hpcflow/tests/unit/test_submission.py
+-rw-r--r--   0        0        0    67153 2023-09-19 19:58:05.416182 hpcflow_new2-0.2.0a99/hpcflow/tests/unit/test_task.py
+-rw-r--r--   0        0        0     3624 2023-09-19 19:58:05.416182 hpcflow_new2-0.2.0a99/hpcflow/tests/unit/test_task_schema.py
+-rw-r--r--   0        0        0    11200 2023-09-19 19:58:05.416182 hpcflow_new2-0.2.0a99/hpcflow/tests/unit/test_utils.py
+-rw-r--r--   0        0        0     7336 2023-09-19 19:58:05.416182 hpcflow_new2-0.2.0a99/hpcflow/tests/unit/test_value_sequence.py
+-rw-r--r--   0        0        0    22185 2023-09-19 19:58:05.416182 hpcflow_new2-0.2.0a99/hpcflow/tests/unit/test_workflow.py
+-rw-r--r--   0        0        0      964 2023-09-19 19:58:05.416182 hpcflow_new2-0.2.0a99/hpcflow/tests/unit/test_workflow_template.py
+-rw-r--r--   0        0        0    10463 2023-09-19 19:58:05.416182 hpcflow_new2-0.2.0a99/hpcflow/tests/workflows/test_workflows.py
+-rw-r--r--   0        0        0     6238 2023-09-19 19:58:05.416182 hpcflow_new2-0.2.0a99/hpcflow/viz_demo.ipynb
+-rw-r--r--   0        0        0     1769 2023-09-19 19:58:05.420182 hpcflow_new2-0.2.0a99/pyproject.toml
+-rw-r--r--   0        0        0     1878 1970-01-01 00:00:00.000000 hpcflow_new2-0.2.0a99/PKG-INFO
```

### Comparing `hpcflow_new2-0.2.0a98/README.md` & `hpcflow_new2-0.2.0a99/README.md`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/__pyinstaller/hook-hpcflow.py` & `hpcflow_new2-0.2.0a99/hpcflow/__pyinstaller/hook-hpcflow.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/app.py` & `hpcflow_new2-0.2.0a99/hpcflow/app.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/examples.ipynb` & `hpcflow_new2-0.2.0a99/hpcflow/examples.ipynb`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/sdk/__init__.py` & `hpcflow_new2-0.2.0a99/hpcflow/sdk/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 # classes used in the construction of a workflow:
 sdk_classes = {
     "Workflow": "hpcflow.sdk.core.workflow",
     "Task": "hpcflow.sdk.core.task",
     "ActionScopeType": "hpcflow.sdk.core.actions",
     "ActionScope": "hpcflow.sdk.core.actions",
     "ActionRule": "hpcflow.sdk.core.actions",
+    "Rule": "hpcflow.sdk.core.rule",
     "Action": "hpcflow.sdk.core.actions",
     "ActionEnvironment": "hpcflow.sdk.core.actions",
     "ElementActionRun": "hpcflow.sdk.core.actions",
     "ElementAction": "hpcflow.sdk.core.actions",
     "FileSpec": "hpcflow.sdk.core.command_files",
     "FileNameSpec": "hpcflow.sdk.core.command_files",
     "FileNameStem": "hpcflow.sdk.core.command_files",
```

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/sdk/app.py` & `hpcflow_new2-0.2.0a99/hpcflow/sdk/app.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/sdk/cli.py` & `hpcflow_new2-0.2.0a99/hpcflow/sdk/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -483,22 +483,40 @@
         )
 
     @workflow.command()
     @click.pass_context
     @click.argument("name")
     @click.argument("value")
     @click.argument("ear_id", type=click.INT)
+    @click.argument("cmd_idx", type=click.INT)
+    @click.option("--stderr", is_flag=True, default=False)
     def save_parameter(
         ctx,
         name: str,
         value: str,
         ear_id: int,
+        cmd_idx: int,
+        stderr: bool,
     ):
-        app.CLI_logger.info(f"save parameter {name!r} for EAR ID {ear_id!r}.")
-        ctx.exit(ctx.obj["workflow"].save_parameter(name, value, ear_id))
+        app.CLI_logger.info(
+            f"save parameter {name!r} for EAR ID {ear_id!r} and command index "
+            f"{cmd_idx!r} (stderr={stderr!r})"
+        )
+        app.CLI_logger.debug(f"save parameter value is: {value!r}")
+        wk = ctx.obj["workflow"]
+        with wk._store.cached_load():
+            value = wk.process_shell_parameter_output(
+                name=name,
+                value=value,
+                EAR_ID=ear_id,
+                cmd_idx=cmd_idx,
+                stderr=stderr,
+            )
+            app.CLI_logger.debug(f"save parameter processed value is: {value!r}")
+            ctx.exit(wk.save_parameter(name=name, value=value, EAR_ID=ear_id))
 
     @workflow.command()
     @click.pass_context
     @click.argument("ear_id", type=click.INT)
     def set_EAR_start(ctx, ear_id: int):
         app.CLI_logger.info(f"set EAR start for EAR ID {ear_id!r}.")
         ctx.exit(ctx.obj["workflow"].set_EAR_start(ear_id))
```

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/sdk/cli_common.py` & `hpcflow_new2-0.2.0a99/hpcflow/sdk/cli_common.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/sdk/config/callbacks.py` & `hpcflow_new2-0.2.0a99/hpcflow/sdk/config/callbacks.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/sdk/config/cli.py` & `hpcflow_new2-0.2.0a99/hpcflow/sdk/config/cli.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/sdk/config/config.py` & `hpcflow_new2-0.2.0a99/hpcflow/sdk/config/config.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/sdk/config/config_file.py` & `hpcflow_new2-0.2.0a99/hpcflow/sdk/config/config_file.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/sdk/config/errors.py` & `hpcflow_new2-0.2.0a99/hpcflow/sdk/config/errors.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/sdk/core/actions.py` & `hpcflow_new2-0.2.0a99/hpcflow/sdk/core/actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 import h5py
 from pathlib import Path
 import re
 import subprocess
 from textwrap import indent, dedent
 from typing import Any, Dict, List, Optional, Tuple, Union
 
-from valida.rules import Rule
+from valida.conditions import ConditionLike
+
 from watchdog.utils.dirsnapshot import DirectorySnapshotDiff
 
 from hpcflow.sdk import app
 from hpcflow.sdk.core import ABORT_EXIT_CODE
 from hpcflow.sdk.core.errors import MissingCompatibleActionEnvironment
 from hpcflow.sdk.core.json_like import ChildObjectSpec, JSONLike
 from hpcflow.sdk.core.utils import JSONLikeDirSnapShot
@@ -330,21 +331,23 @@
         )
 
     def get(
         self,
         path: str = None,
         default: Any = None,
         raise_on_missing: bool = False,
+        raise_on_unset: bool = False,
     ):
         return self.element_iteration.get(
             path=path,
             action_idx=self.element_action.action_idx,
             run_idx=self.index,
             default=default,
             raise_on_missing=raise_on_missing,
+            raise_on_unset=raise_on_unset,
         )
 
     def get_EAR_dependencies(self, as_objects=False):
         """Get EARs that this EAR depends on."""
 
         out = []
         for src in self.get_parameter_sources(typ="EAR_output").values():
@@ -650,15 +653,15 @@
                 param_id = self.data_idx[f"outputs.{param_name}"]
                 param_cls = self.app.parameters.get(param_name)._value_class
                 if param_cls:
                     param_cls.save_from_HDF5_group(h5_grp, param_id, workflow)
 
     def compose_commands(
         self, jobscript: app.Jobscript, JS_action_idx: int
-    ) -> Tuple[str, List[str]]:
+    ) -> Tuple[str, List[str], List[int]]:
         """
         Returns
         -------
         commands
         shell_vars
             List of shell variable names that must be saved as workflow parameter data
             as strings.
@@ -677,24 +680,26 @@
 
         command_lns = []
         env = self.get_environment()
         if env.setup:
             command_lns += list(env.setup)
 
         shell_vars = []
-        for command in self.action.commands:
+        cmd_indices = []
+        for cmd_idx, command in enumerate(self.action.commands):
             cmd_str, shell_vars_i = command.get_command_line(
                 EAR=self, shell=jobscript.shell, env=env
             )
             shell_vars.extend(shell_vars_i)
+            cmd_indices.append(cmd_idx)
             command_lns.append(cmd_str)
 
         commands = "\n".join(command_lns) + "\n"
 
-        return commands, shell_vars
+        return commands, shell_vars, cmd_indices
 
 
 class ElementAction:
     _app_attr = "app"
 
     def __init__(self, element_iteration, action_idx, runs):
         self._element_iteration = element_iteration
@@ -809,21 +814,23 @@
 
     def get(
         self,
         path: str = None,
         run_idx: int = -1,
         default: Any = None,
         raise_on_missing: bool = False,
+        raise_on_unset: bool = False,
     ):
         return self.element_iteration.get(
             path=path,
             action_idx=self.action_idx,
             run_idx=run_idx,
             default=default,
             raise_on_missing=raise_on_missing,
+            raise_on_unset=raise_on_unset,
         )
 
     def get_parameter_names(self, prefix):
         if prefix == "inputs":
             single_lab_lookup = self.element_iteration._get_single_label_lookup()
             out = list(single_lab_lookup.get(i, i) for i in self.action.get_input_types())
         elif prefix == "outputs":
@@ -1066,49 +1073,68 @@
     scope: Optional[app.ActionScope] = None
 
     def __post_init__(self):
         if self.scope is None:
             self.scope = self.app.ActionScope.any()
 
 
-@dataclass
 class ActionRule(JSONLike):
     """Class to represent a rule/condition that must be True if an action is to be
     included."""
 
-    _app_attr = "app"
-
-    _child_objects = (ChildObjectSpec(name="rule", class_obj=Rule),)
+    _child_objects = (ChildObjectSpec(name="rule", class_name="Rule"),)
 
-    check_exists: Optional[str] = None
-    check_missing: Optional[str] = None
-    rule: Optional[Rule] = None
-
-    def __post_init__(self):
-        if (
-            self.check_exists is not None
-            and self.check_missing is not None
-            and self.rule is not None
-        ) or (
-            self.check_exists is None and self.check_missing is None and self.rule is None
+    def __init__(
+        self,
+        rule: Optional[app.Rule] = None,
+        check_exists: Optional[str] = None,
+        check_missing: Optional[str] = None,
+        path: Optional[str] = None,
+        condition: Optional[Union[Dict, ConditionLike]] = None,
+        cast: Optional[str] = None,
+        doc: Optional[str] = None,
+    ):
+        if rule is None:
+            rule = app.Rule(
+                check_exists=check_exists,
+                check_missing=check_missing,
+                path=path,
+                condition=condition,
+                cast=cast,
+                doc=doc,
+            )
+        elif any(
+            i is not None
+            for i in (check_exists, check_missing, path, condition, cast, doc)
         ):
-            raise ValueError(
-                "Specify exactly one of `check_exists`, `check_missing` and `rule`."
+            raise TypeError(
+                f"{self.__class__.__name__} `rule` specified in addition to rule "
+                f"constructor arguments."
             )
 
-    def __repr__(self):
-        out = f"{self.__class__.__name__}("
-        if self.check_exists:
-            out += f"check_exists={self.check_exists!r}"
-        elif self.check_missing:
-            out += f"check_missing={self.check_missing!r}"
-        else:
-            out += f"rule={self.rule}"
-        out += ")"
-        return out
+        self.rule = rule
+        self.action = None  # assigned by parent action
+
+    def __eq__(self, other):
+        if type(other) is not self.__class__:
+            return False
+        if self.rule == other.rule:
+            return True
+        return False
+
+    def test(self, element_iteration: app.ElementIteration) -> bool:
+        return self.rule.test(element_like=element_iteration, action=self.action)
+
+    @classmethod
+    def check_exists(cls, check_exists):
+        return cls(rule=app.Rule(check_exists=check_exists))
+
+    @classmethod
+    def check_missing(cls, check_missing):
+        return cls(rule=app.Rule(check_missing=check_missing))
 
 
 class Action(JSONLike):
     """"""
 
     _app_attr = "app"
     _child_objects = (
@@ -1146,14 +1172,15 @@
             class_name="ActionEnvironment",
             is_multiple=True,
         ),
         ChildObjectSpec(
             name="rules",
             class_name="ActionRule",
             is_multiple=True,
+            parent_ref="action",
         ),
     )
 
     def __init__(
         self,
         environments: Optional[List[app.ActionEnvironment]] = None,
         commands: Optional[List[app.Command]] = None,
@@ -1182,14 +1209,16 @@
         self.input_files = self._resolve_input_files(input_files or [])
         self.output_files = self._resolve_output_files(output_files or [])
         self.rules = rules or []
 
         self._task_schema = None  # assigned by parent TaskSchema
         self._from_expand = False  # assigned on creation of new Action by `expand`
 
+        self._set_parent_refs()
+
     def __deepcopy__(self, memo):
         kwargs = self.to_dict()
         _from_expand = kwargs.pop("_from_expand")
         _task_schema = kwargs.pop("_task_schema", None)
         obj = self.__class__(**copy.deepcopy(kwargs, memo))
         obj._from_expand = _from_expand
         obj._task_schema = _task_schema
@@ -1379,15 +1408,15 @@
             #   - one or more output files are not passed
             # run IFG if:
             #   - one or more output files are not passed
             #   - AND input file is not passed
             # always run OPs, for now
 
             out_file_rules = [
-                self.app.ActionRule(check_missing=f"output_files.{j.label}")
+                self.app.ActionRule.check_missing(f"output_files.{j.label}")
                 for i in self.output_file_parsers
                 for j in i.output_files
             ]
 
             main_rules = self.rules + out_file_rules
 
             # note we keep the IFG/OPs in the new actions, so we can check the parameters
@@ -1507,25 +1536,37 @@
             main_act._task_schema = self.task_schema
             main_act._from_expand = True
 
             cmd_acts = inp_acts + [main_act] + out_acts
 
             return cmd_acts
 
-    def get_command_input_types(self) -> Tuple[str]:
-        """Get parameter types from commands."""
+    def get_command_input_types(self, sub_parameters: bool = False) -> Tuple[str]:
+        """Get parameter types from commands.
+
+        Parameters
+        ----------
+        sub_parameters
+            If True, sub-parameters (i.e. dot-delimited parameter types) will be returned
+            untouched. If False (default), only return the root parameter type and
+            disregard the sub-parameter part.
+        """
         params = []
         # note: we use "parameter" rather than "input", because it could be a schema input
         # or schema output.
-        vars_regex = r"\<\<parameter:(.*?)\>\>"
+        vars_regex = r"\<\<(?:\w+(?:\[(?:.*)\])?\()?parameter:(.*?)\)?\>\>"
         for command in self.commands:
             for val in re.findall(vars_regex, command.command or ""):
+                if not sub_parameters:
+                    val = val.split(".")[0]
                 params.append(val)
             for arg in command.arguments or []:
                 for val in re.findall(vars_regex, arg):
+                    if not sub_parameters:
+                        val = val.split(".")[0]
                     params.append(val)
             # TODO: consider stdin?
         return tuple(set(params))
 
     def get_command_input_file_labels(self) -> Tuple[str]:
         """Get input files types from commands."""
         files = []
@@ -1547,26 +1588,34 @@
             if out_params["stdout"]:
                 params.append(out_params["stdout"])
             if out_params["stderr"]:
                 params.append(out_params["stderr"])
 
         return tuple(set(params))
 
-    def get_input_types(self) -> Tuple[str]:
+    def get_input_types(self, sub_parameters: bool = False) -> Tuple[str]:
         """Get the input types that are consumed by commands and input file generators of
-        this action."""
+        this action.
+
+        Parameters
+        ----------
+        sub_parameters
+            If True, sub-parameters (i.e. dot-delimited parameter types) in command line
+            inputs will be returned untouched. If False (default), only return the root
+            parameter type and disregard the sub-parameter part.
+        """
         is_script = (
             self.script
             and not self.input_file_generators
             and not self.output_file_parsers
         )
         if is_script:
             params = self.task_schema.input_types
         else:
-            params = list(self.get_command_input_types())
+            params = list(self.get_command_input_types(sub_parameters))
             for i in self.input_file_generators:
                 params.extend([j.typ for j in i.inputs])
             for i in self.output_file_parsers:
                 params.extend([j for j in i.inputs or []])
         return tuple(set(params))
 
     def get_output_types(self) -> Tuple[str]:
@@ -1758,7 +1807,11 @@
                 if IFG.input_file not in provided_files:
                     return True
 
         # typ is required if used in any output file parser
         for OFP in self.output_file_parsers:
             if typ in (OFP.inputs or []):
                 return True
+
+    def test_rules(self, element_iter) -> List[bool]:
+        """Test all rules against the specified element iteration."""
+        return [i.test(element_iteration=element_iter) for i in self.rules]
```

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/sdk/core/command_files.py` & `hpcflow_new2-0.2.0a99/hpcflow/sdk/core/command_files.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,15 @@
     script: str = None
     environment: app.Environment = None
     abortable: Optional[bool] = False
 
     def get_action_rule(self):
         """Get the rule that allows testing if this input file generator must be
         run or not for a given element."""
-        return self.app.ActionRule(check_missing=f"input_files.{self.input_file.label}")
+        return self.app.ActionRule.check_missing(f"input_files.{self.input_file.label}")
 
     def compose_source(self, action) -> str:
         """Generate the file contents of this input file generator source."""
 
         script_name = self.script
         script_key = action.get_app_data_script_path(self.script)
         script_path = self.app.scripts.get(script_key)
```

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/sdk/core/element.py` & `hpcflow_new2-0.2.0a99/hpcflow/sdk/core/element.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from __future__ import annotations
 import copy
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 import os
 from typing import Any, Dict, List, Optional, Union
 
 from valida.conditions import ConditionLike
 from valida.rules import Rule
 
 from hpcflow.sdk import app
 from hpcflow.sdk.core.errors import UnsupportedOSError, UnsupportedSchedulerError
-from hpcflow.sdk.core.json_like import JSONLike
+from hpcflow.sdk.core.json_like import ChildObjectSpec, JSONLike
 from hpcflow.sdk.core.parameters import ParallelMode
 from hpcflow.sdk.core.utils import check_valid_py_identifier, get_enum_by_name_or_val
 from hpcflow.sdk.submission.shells import get_shell
 
 
 class _ElementPrefixedParameter:
     _app_attr = "_app"
@@ -92,15 +92,15 @@
 
     @property
     def prefixed_names_unlabelled_str(self):
         return ", ".join(i for i in self.prefixed_names_unlabelled)
 
     def __repr__(self):
         # If there are one or more labels present, then replace with a single name
-        # indicating there could be multiple (using `multi_prefix` prefix):
+        # indicating there could be multiple (using a `*` prefix):
         names = []
         for unlabelled, labels in self.prefixed_names_unlabelled.items():
             name_i = unlabelled
             if labels:
                 name_i = "*" + name_i
             names.append(name_i)
         names_str = ", ".join(i for i in names)
@@ -609,53 +609,72 @@
     def get(
         self,
         path: str = None,
         action_idx: int = None,
         run_idx: int = -1,
         default: Any = None,
         raise_on_missing: bool = False,
+        raise_on_unset: bool = False,
     ) -> Any:
         """Get element data from the persistent store."""
         # TODO include a "stats" parameter which when set we know the run has been
         # executed (or if start time is set but not end time, we know it's running or
         # failed.)
 
         data_idx = self.get_data_idx(action_idx=action_idx, run_idx=run_idx)
         single_label_lookup = self._get_single_label_lookup(prefix="inputs")
 
         if single_label_lookup:
             # For any non-multiple `SchemaParameter`s of this task with non-empty labels,
             # remove the trivial label:
             for key in list(data_idx.keys()):
+                if (path or "").startswith(key):
+                    # `path` uses labelled type, so no need to convert to non-labelled
+                    continue
                 lookup_val = single_label_lookup.get(key)
                 if lookup_val:
                     data_idx[lookup_val] = data_idx.pop(key)
 
         return self.task._get_merged_parameter_data(
             data_index=data_idx,
             path=path,
             raise_on_missing=raise_on_missing,
+            raise_on_unset=raise_on_unset,
             default=default,
         )
 
     def get_EAR_dependencies(
         self,
         as_objects: Optional[bool] = False,
     ) -> List[Union[int, app.ElementActionRun]]:
         """Get EARs that this element iteration depends on (excluding EARs of this element
         iteration)."""
         # TODO: test this includes EARs of upstream iterations of this iteration's element
-        out = sorted(
-            set(
-                EAR_ID
-                for i in self.action_runs
-                for EAR_ID in i.get_EAR_dependencies(as_objects=False)
-                if not EAR_ID in self.EAR_IDs_flat
+        if self.action_runs:
+            out = sorted(
+                set(
+                    EAR_ID
+                    for i in self.action_runs
+                    for EAR_ID in i.get_EAR_dependencies(as_objects=False)
+                    if not EAR_ID in self.EAR_IDs_flat
+                )
             )
-        )
+        else:
+            # if an "input-only" task schema, then there will be no action runs, but the
+            # ElementIteration can still depend on other EARs if inputs are sourced from
+            # upstream tasks:
+            out = []
+            for src in self.get_parameter_sources(typ="EAR_output").values():
+                if not isinstance(src, list):
+                    src = [src]
+                for src_i in src:
+                    EAR_ID_i = src_i["EAR_ID"]
+                    out.append(EAR_ID_i)
+            out = sorted(set(out))
+
         if as_objects:
             out = self.workflow.get_EARs_from_IDs(out)
         return out
 
     def get_element_iteration_dependencies(
         self, as_objects: bool = False
     ) -> List[Union[int, app.ElementIteration]]:
@@ -838,16 +857,15 @@
         for scope in action.get_possible_scopes()[::-1]:
             # loop in reverse so higher-specificity scopes take precedence:
             scope_s = scope.to_string()
             scope_res = resource_specs.get(scope_s, {})
             resources.update({k: v for k, v in scope_res.items() if v is not None})
 
         if set_defaults:
-            # this is used in e.g. `WorkflowTask.test_action_rule` if testing action rules
-            # that concern resources:
+            # used in e.g. `Rule.test` if testing resource rules on element iterations:
             if "os_name" not in resources:
                 resources["os_name"] = self.app.ElementResources.get_default_os_name()
             if "shell" not in resources:
                 resources["shell"] = self.app.ElementResources.get_default_shell()
             if "scheduler" not in resources:
                 resources["scheduler"] = self.app.ElementResources.get_default_scheduler(
                     resources["os_name"], resources["shell"]
@@ -1092,22 +1110,24 @@
     def get(
         self,
         path: str = None,
         action_idx: int = None,
         run_idx: int = -1,
         default: Any = None,
         raise_on_missing: bool = False,
+        raise_on_unset: bool = False,
     ) -> Any:
         """Get element data of the most recent iteration from the persistent store."""
         return self.latest_iteration.get(
             path=path,
             action_idx=action_idx,
             run_idx=run_idx,
             default=default,
             raise_on_missing=raise_on_missing,
+            raise_on_unset=raise_on_unset,
         )
 
     def get_EAR_dependencies(
         self, as_objects: bool = False
     ) -> List[Union[int, app.ElementActionRun]]:
         """Get EARs that the most recent iteration of this element depends on."""
         return self.latest_iteration.get_EAR_dependencies(as_objects=as_objects)
@@ -1235,16 +1255,28 @@
     def is_set(self):
         return all(self.data_idx_is_set.values())
 
     def get_size(self, **store_kwargs):
         raise NotImplementedError
 
 
-class ElementFilter(Rule):
-    pass
+@dataclass
+class ElementFilter(JSONLike):
+    _child_objects = (ChildObjectSpec(name="rules", is_multiple=True, class_name="Rule"),)
+
+    rules: List[app.Rule] = field(default_factory=list)
+
+    def filter(
+        self, element_iters: List[app.ElementIteration]
+    ) -> List[app.ElementIteration]:
+        out = []
+        for i in element_iters:
+            if all(rule_j.test(i) for rule_j in self.rules):
+                out.append(i)
+        return out
 
 
 @dataclass
 class ElementGroup(JSONLike):
     name: str
     where: Optional[ElementFilter] = None
     group_by_distinct: Optional[app.ParameterPath] = None
```

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/sdk/core/environment.py` & `hpcflow_new2-0.2.0a99/hpcflow/sdk/core/environment.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/sdk/core/errors.py` & `hpcflow_new2-0.2.0a99/hpcflow/sdk/core/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-from typing import Iterable
+from typing import Iterable, List
 
 
 class InputValueDuplicateSequenceAddress(ValueError):
     pass
 
 
 class TaskTemplateMultipleSchemaObjectives(ValueError):
@@ -331,7 +331,27 @@
 
 class NotSubmitMachineError(RuntimeError):
     pass
 
 
 class RunNotAbortableError(ValueError):
     pass
+
+
+class NoCLIFormatMethodError(AttributeError):
+    pass
+
+
+class ContainerKeyError(KeyError):
+    def __init__(self, path: List[str]) -> None:
+        self.path = path
+        super().__init__()
+
+
+class MayNeedObjectError(Exception):
+    def __init__(self, path):
+        self.path = path
+        super().__init__()
+
+
+class NoAvailableElementSetsError(Exception):
+    pass
```

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/sdk/core/json_like.py` & `hpcflow_new2-0.2.0a99/hpcflow/sdk/core/json_like.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/sdk/core/loop.py` & `hpcflow_new2-0.2.0a99/hpcflow/sdk/core/loop.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/sdk/core/object_list.py` & `hpcflow_new2-0.2.0a99/hpcflow/sdk/core/object_list.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/sdk/core/parameters.py` & `hpcflow_new2-0.2.0a99/hpcflow/sdk/core/parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 Address = List[Union[int, float, str]]
 Numeric = Union[int, float, np.number]
 
 
 class ParameterValue:
     _typ = None
+    _sub_parameters = {}
 
     def to_dict(self):
         if hasattr(self, "__dict__"):
             return dict(self.__dict__)
         elif hasattr(self, "__slots__"):
             return {k: getattr(self, k) for k in self.__slots__}
 
@@ -87,19 +88,23 @@
             f"{self.__class__.__name__}("
             f"typ={self.typ!r}{is_file_str}{sub_parameters_str}{_value_class_str}"
             f")"
         )
 
     def __post_init__(self):
         self.typ = check_valid_py_identifier(self.typ)
+        self._set_value_class()
+
+    def _set_value_class(self):
         # custom parameter classes must inherit from `ParameterValue` not the app
         # subclass:
-        for i in ParameterValue.__subclasses__():
-            if i._typ == self.typ:
-                self._value_class = i
+        if self._value_class is None:
+            for i in ParameterValue.__subclasses__():
+                if i._typ == self.typ:
+                    self._value_class = i
 
     def __lt__(self, other):
         return self.typ < other.typ
 
     def __deepcopy__(self, memo):
         kwargs = self.to_dict()
         _validation = kwargs.pop("_validation")
@@ -1010,14 +1015,15 @@
     def __init__(
         self,
         parameter: Union[app.Parameter, str],
         value: Optional[Any] = None,
         label: Optional[str] = None,
         value_class_method: Optional[str] = None,
         path: Optional[str] = None,
+        __check_obj: Optional[bool] = True,
     ):
         if isinstance(parameter, str):
             parameter = self.app.parameters.get(parameter)
         elif isinstance(parameter, SchemaInput):
             parameter = parameter.parameter
 
         self.parameter = parameter
@@ -1032,22 +1038,45 @@
         # assigned by parent SchemaInput (if this object is a default value of a
         # SchemaInput):
         self._schema_input = None
 
         # record if a ParameterValue sub-class is passed for value, which allows us
         # to re-init the object on `.value`:
         self._value_is_obj = isinstance(value, ParameterValue)
+        if __check_obj:
+            self._check_dict_value_if_object()
+
+    def _check_dict_value_if_object(self):
+        """For non-persistent input values, check that, if a matching `ParameterValue`
+        class exists and the specified value is not of that type, then the specified
+        value is a dict, which can later be passed to the ParameterValue sub-class
+        to initialise the object.
+        """
+        if (
+            self._value_group_idx is None
+            and not self.path
+            and not self._value_is_obj
+            and self.parameter._value_class
+            and not isinstance(self._value, dict)
+        ):
+            # TODO: what about if the value is `None`? Is that an issue?
+            raise ValueError(
+                f"{self.__class__.__name__} with specified value {self._value!r} is "
+                f"associated with a ParameterValue subclass "
+                f"({self.parameter._value_class!r}), but the value data type is not a "
+                f"dict."
+            )
 
     def __deepcopy__(self, memo):
         kwargs = self.to_dict()
         _value = kwargs.pop("_value")
         kwargs.pop("_schema_input", None)
         _value_group_idx = kwargs.pop("_value_group_idx")
         _value_is_obj = kwargs.pop("_value_is_obj")
-        obj = self.__class__(**copy.deepcopy(kwargs, memo))
+        obj = self.__class__(**copy.deepcopy(kwargs, memo), _InputValue__check_obj=False)
         obj._value = _value
         obj._value_group_idx = _value_group_idx
         obj._value_is_obj = _value_is_obj
         obj._element_set = self._element_set
         obj._schema_input = self._schema_input
         return obj
 
@@ -1090,18 +1119,18 @@
         """Invoked by `JSONLike.from_json_like` instead of `__init__`."""
 
         _value_group_idx = json_like.pop("_value_group_idx", None)
         _value_is_obj = json_like.pop("_value_is_obj", None)
         if "_value" in json_like:
             json_like["value"] = json_like.pop("_value")
 
-        obj = cls(**json_like)
+        obj = cls(**json_like, _InputValue__check_obj=False)
         obj._value_group_idx = _value_group_idx
         obj._value_is_obj = _value_is_obj
-
+        obj._check_dict_value_if_object()
         return obj
 
     @property
     def labelled_type(self):
         label = f"[{self.label}]" if self.label else ""
         return f"{self.parameter.typ}{label}"
 
@@ -1551,16 +1580,27 @@
         self,
         source_type,
         import_ref=None,
         task_ref=None,
         task_source_type=None,
         element_iters=None,
         path=None,
-        where=None,
+        where: Optional[
+            Union[dict, app.Rule, List[dict], List[app.Rule], app.ElementFilter]
+        ] = None,
     ):
+        if where is not None and not isinstance(where, app.ElementFilter):
+            rules = where
+            if not isinstance(rules, list):
+                rules = [rules]
+            for idx, i in enumerate(rules):
+                if not isinstance(i, app.Rule):
+                    rules[idx] = app.Rule(**i)
+            where = app.ElementFilter(rules=rules)
+
         self.source_type = self._validate_source_type(source_type)
         self.import_ref = import_ref
         self.task_ref = task_ref
         self.task_source_type = self._validate_task_source_type(task_source_type)
         self.element_iters = element_iters
         self.where = where
         self.path = path
@@ -1589,51 +1629,55 @@
             return True
         else:
             return False
 
     def __repr__(self) -> str:
         cls_method_name = self.source_type.name.lower()
 
+        args_lst = []
+
         if self.source_type is InputSourceType.IMPORT:
             cls_method_name += "_"
-            args = f"import_ref={self.import_ref}"
+            args_lst.append(f"import_ref={self.import_ref}")
 
         elif self.source_type is InputSourceType.TASK:
-            args = (
-                f"task_ref={self.task_ref}, "
-                f"task_source_type={self.task_source_type.name.lower()!r}"
+            args_lst += (
+                f"task_ref={self.task_ref}",
+                f"task_source_type={self.task_source_type.name.lower()!r}",
             )
-            if self.element_iters:
-                args += f", element_iters={self.element_iters}"
-        else:
-            args = ""
 
+        if self.element_iters:
+            args_lst.append(f"element_iters={self.element_iters}")
+
+        if self.where is not None:
+            args_lst.append(f"where={self.where!r}")
+
+        args = ", ".join(args_lst)
         out = f"{self.__class__.__name__}.{cls_method_name}({args})"
 
         return out
 
     def get_task(self, workflow):
         """If source_type is task, then return the referenced task from the given
         workflow."""
         if self.source_type is InputSourceType.TASK:
             for task in workflow.tasks:
                 if task.insert_ID == self.task_ref:
                     return task
 
     def is_in(self, other_input_sources: List[app.InputSource]) -> Union[None, int]:
         """Check if this input source is in a list of other input sources, without
-        considering the `element_iters` attribute."""
+        considering the `element_iters` and `where` attributes."""
 
         for idx, other in enumerate(other_input_sources):
             if (
                 self.source_type == other.source_type
                 and self.import_ref == other.import_ref
                 and self.task_ref == other.task_ref
                 and self.task_source_type == other.task_source_type
-                and self.where == other.where
                 and self.path == other.path
             ):
                 return idx
         return None
 
     def to_string(self):
         out = [self.source_type.name.lower()]
@@ -1736,28 +1780,34 @@
     @classmethod
     def from_json_like(cls, json_like, shared_data=None):
         if isinstance(json_like, str):
             json_like = cls._parse_from_string(json_like)
         return super().from_json_like(json_like, shared_data)
 
     @classmethod
-    def import_(cls, import_ref):
-        return cls(source_type=cls.app.InputSourceType.IMPORT, import_ref=import_ref)
+    def import_(cls, import_ref, element_iters=None, where=None):
+        return cls(
+            source_type=cls.app.InputSourceType.IMPORT,
+            import_ref=import_ref,
+            element_iters=element_iters,
+            where=where,
+        )
 
     @classmethod
     def local(cls):
         return cls(source_type=cls.app.InputSourceType.LOCAL)
 
     @classmethod
     def default(cls):
         return cls(source_type=cls.app.InputSourceType.DEFAULT)
 
     @classmethod
-    def task(cls, task_ref, task_source_type=None, element_iters=None):
+    def task(cls, task_ref, task_source_type=None, element_iters=None, where=None):
         if not task_source_type:
             task_source_type = cls.app.TaskSourceType.OUTPUT
         return cls(
             source_type=cls.app.InputSourceType.TASK,
             task_ref=task_ref,
             task_source_type=cls._validate_task_source_type(task_source_type),
+            where=where,
             element_iters=element_iters,
         )
```

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/sdk/core/task.py` & `hpcflow_new2-0.2.0a99/hpcflow/sdk/core/task.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 from __future__ import annotations
 import copy
 from dataclasses import dataclass
 import os
 from pathlib import Path
-from typing import Any, Dict, Iterator, List, Optional, Tuple, Union
+from typing import Any, Dict, Iterable, Iterator, List, Optional, Tuple, Union
 
 from valida.rules import Rule
 
 
 from hpcflow.sdk import app
 from hpcflow.sdk.core.task_schema import TaskSchema
 from hpcflow.sdk.submission.shells import DEFAULT_SHELL_NAMES
 from .json_like import ChildObjectSpec, JSONLike
 from .element import ElementGroup
 from .errors import (
+    ContainerKeyError,
     ExtraInputs,
+    MayNeedObjectError,
     MissingInputs,
+    NoAvailableElementSetsError,
     TaskTemplateInvalidNesting,
     TaskTemplateMultipleInputValues,
     TaskTemplateMultipleSchemaObjectives,
     TaskTemplateUnexpectedInput,
     TaskTemplateUnexpectedSequenceInput,
     UnrequiredInputSources,
     UnsetParameterDataError,
 )
-from .parameters import InputSourceType
+from .parameters import InputSourceType, ParameterValue, TaskSourceType
 from .utils import (
     get_duplicate_items,
     get_in_container,
     get_item_repeat_index,
     get_relative_path,
     group_by_dict_key_values,
     set_in_container,
@@ -741,14 +744,48 @@
     def output_labels(self):
         return self._output_labels
 
     @property
     def _element_indices(self):
         return self.workflow_template.workflow.tasks[self.index].element_indices
 
+    def _get_task_source_element_iters(
+        self, in_or_out: str, src_task, labelled_path, element_set
+    ) -> List[int]:
+        if in_or_out == "input":
+            # input parameter might not be provided e.g. if it only used
+            # to generate an input file, and that input file is passed
+            # directly, so consider only source task element sets that
+            # provide the input locally:
+            es_idx = src_task.get_param_provided_element_sets(labelled_path)
+        else:
+            # outputs are always available, so consider all source task
+            # element sets:
+            es_idx = list(range(src_task.num_element_sets))
+
+        if not es_idx:
+            raise NoAvailableElementSetsError()
+        else:
+            src_elem_iters = []
+            for es_idx_i in es_idx:
+                es_i = src_task.element_sets[es_idx_i]
+                src_elem_iters += es_i.elem_iter_IDs
+
+        if element_set.sourceable_elem_iters is not None:
+            # can only use a subset of element iterations (this is the
+            # case where this element set is generated from an upstream
+            # element set, in which case we only want to consider newly
+            # added upstream elements when adding elements from this
+            # element set):
+            src_elem_iters = list(
+                set(element_set.sourceable_elem_iters) & set(src_elem_iters)
+            )
+
+        return src_elem_iters
+
     def get_available_task_input_sources(
         self,
         element_set: app.ElementSet,
         source_tasks: Optional[List[app.WorkflowTask]] = None,
     ) -> List[app.InputSource]:
         """For each input parameter of this task, generate a list of possible input sources
         that derive from inputs or outputs of this and other provided tasks.
@@ -780,88 +817,71 @@
                 for in_or_out, labelled_path in sorted(
                     src_task_i.provides_parameters(),
                     key=lambda x: x[0],
                     reverse=True,
                 ):
                     if inputs_path in labelled_path:
                         avail_src_path = labelled_path
-                        if in_or_out == "input":
-                            # input parameter might not be provided e.g. if it only used
-                            # to generate an input file, and that input file is passed
-                            # directly, so consider only source task element sets that
-                            # provide the input locally:
-                            es_idx = src_task_i.get_param_provided_element_sets(
-                                labelled_path
+                        try:
+                            src_elem_iters = self._get_task_source_element_iters(
+                                in_or_out=in_or_out,
+                                src_task=src_task_i,
+                                labelled_path=labelled_path,
+                                element_set=element_set,
                             )
-                        else:
-                            # outputs are always available, so consider all source task
-                            # element sets:
-                            es_idx = list(range(src_task_i.num_element_sets))
-
-                        if not es_idx:
+                        except NoAvailableElementSetsError:
                             continue
-                        else:
-                            src_elem_iters = []
-                            for es_idx_i in es_idx:
-                                es_i = src_task_i.element_sets[es_idx_i]
-                                src_elem_iters += es_i.elem_iter_IDs
-
-                        if element_set.sourceable_elem_iters is not None:
-                            # can only use a subset of element iterations (this is the
-                            # case where this element set is generated from an upstream
-                            # element set, in which case we only want to consider newly
-                            # added upstream elements when adding elements from this
-                            # element set):
-                            src_elem_iters = list(
-                                set(element_set.sourceable_elem_iters)
-                                & set(src_elem_iters)
-                            )
-
-                    elif labelled_path in inputs_path and in_or_out == "output":
+                    elif labelled_path in inputs_path:
                         avail_src_path = inputs_path
-
                         inputs_path_label = None
                         out_label = None
                         try:
                             inputs_path_label = inputs_path.split("[")[1].split("]")[0]
                         except IndexError:
                             pass
                         if inputs_path_label:
                             for out_lab_i in src_task_i.output_labels:
                                 if out_lab_i.label == inputs_path_label:
                                     out_label = out_lab_i
-                        if out_label:
+                        if out_label and in_or_out == "output":
                             # find element iteration IDs that match the output label
                             # filter:
                             param_path = ".".join(
                                 i.condition.callable.kwargs["value"]
                                 for i in out_label.where.path
                             )
                             param_path_split = param_path.split(".")
 
                             src_elem_iters = []
                             for elem_i in src_wk_task_i.elements[:]:
                                 params = getattr(elem_i, param_path_split[0])
                                 param_dat = getattr(params, param_path_split[1]).value
 
-                                # for remaining paths components try both getattr and getitem:
+                                # for remaining paths components try both getattr and
+                                # getitem:
                                 for path_k in param_path_split[2:]:
                                     try:
                                         param_dat = param_dat[path_k]
                                     except TypeError:
                                         param_dat = getattr(param_dat, path_k)
 
                                 rule = Rule(
                                     path=[0],
                                     condition=out_label.where.condition,
                                     cast=out_label.where.cast,
                                 )
                                 if rule.test([param_dat]).is_valid:
                                     src_elem_iters.append(elem_i.iterations[0].id_)
-
+                        else:
+                            src_elem_iters = self._get_task_source_element_iters(
+                                in_or_out=in_or_out,
+                                src_task=src_task_i,
+                                labelled_path=labelled_path,
+                                element_set=element_set,
+                            )
                     else:
                         continue
 
                     if not src_elem_iters:
                         continue
 
                     task_source = self.app.InputSource.task(
@@ -1051,19 +1071,14 @@
         return [
             inp_j
             for schema_i in self.schemas
             for inp_j in schema_i.inputs
             if inp_j.typ in self.undefined_input_types
         ]
 
-    @property
-    def unsourced_inputs(self):
-        """Get schema input types for which no input sources are currently specified."""
-        return self.all_schema_input_types - set(self.input_sources.keys())
-
     def provides_parameters(self) -> Tuple[Tuple[str, str]]:
         """Get all provided parameter labelled types and whether they are inputs and
         outputs, considering all element sets.
 
         """
         out = []
         for schema in self.schemas:
@@ -1371,15 +1386,15 @@
                         source_idx[key] += [inp_src_idx] * len(grp_idx)
 
                     else:
                         input_data_idx[key] = grp_idx
                         source_idx[key] = [inp_src_idx] * len(grp_idx)
 
         # sort smallest to largest path, so more-specific items overwrite less-specific
-        # items parameter retrieval:
+        # items in parameter retrieval in `WorkflowTask._get_merged_parameter_data`:
         input_data_idx = dict(sorted(input_data_idx.items()))
 
         return (input_data_idx, sequence_idx, source_idx)
 
     def ensure_input_sources(self, element_set):
         """Check valid input sources are specified for a new task to be added to the
         workflow in a given position. If none are specified, set them according to the
@@ -1431,53 +1446,93 @@
             for s_idx, specified_source in enumerate(
                 element_set.input_sources.get(path_i, [])
             ):
                 self.workflow._resolve_input_source_task_reference(
                     specified_source, self.unique_name
                 )
                 avail_idx = specified_source.is_in(avail_i)
+                available_source = avail_i[avail_idx]
                 if avail_idx is None:
                     raise ValueError(
                         f"The input source {specified_source.to_string()!r} is not "
                         f"available for input path {path_i!r}. Available "
                         f"input sources are: {[i.to_string() for i in avail_i]}."
                     )
                 else:
-                    # overwrite with the source from available_sources, since it will have
-                    # the `element_iters` attribute assigned:
-                    element_set.input_sources[path_i][s_idx] = avail_i[avail_idx]
+                    # overwrite with the source from available_sources, since it may have
+                    # the `element_iters` attribute assigned, but first check if we need
+                    # to filter:
+                    filtered_IDs = None
+                    if specified_source.where:
+                        elem_iters = self.workflow.get_element_iterations_from_IDs(
+                            available_source.element_iters
+                        )
+                        filtered = specified_source.where.filter(elem_iters)
+                        filtered_IDs = [i.id_ for i in filtered]
+
+                    if filtered_IDs is not None:
+                        available_source.element_iters = filtered_IDs
 
-        unsourced_inputs = req_types - set(element_set.input_sources.keys())
+                    element_set.input_sources[path_i][s_idx] = available_source
+
+        # sorting ensures that root parameters come before sub-parameters, which is
+        # necessary when considering if we want to include a sub-parameter, when setting
+        # missing sources below:
+        unsourced_inputs = sorted(req_types - set(element_set.input_sources.keys()))
 
         extra_types = set(k for k, v in all_stats.items() if v.is_extra)
         if extra_types:
             extra_str = ", ".join(f"{i!r}" for i in extra_types)
             raise ExtraInputs(
                 message=(
                     f"The following inputs are not required, but have been passed: "
                     f"{extra_str}."
                 ),
                 extra_inputs=extra_types,
             )
 
         # set source for any unsourced inputs:
         missing = []
+        # track which root params we have set according to default behaviour (not
+        # specified by user):
+        set_root_params = []
         for input_type in unsourced_inputs:
+            input_split = input_type.split(".")
+            has_root_param = input_split[0] if len(input_split) > 1 else None
             inp_i_sources = available_sources.get(input_type, [])
 
             source = None
             try:
                 # first element is defined by default to take precedence in
                 # `get_available_task_input_sources`:
                 source = inp_i_sources[0]
             except IndexError:
                 missing.append(input_type)
 
             if source is not None:
+                if has_root_param and has_root_param in set_root_params:
+                    # this is a sub-parameter, and the associated root parameter was not
+                    # specified by the user either, so we previously set it according to
+                    # default behaviour
+                    root_src = element_set.input_sources[has_root_param][0]
+                    # do not set a default task-input type source for this sub-parameter
+                    # if the associated root parameter has a default-set task-output
+                    # source from the same task:
+                    if (
+                        source.source_type is InputSourceType.TASK
+                        and source.task_source_type is TaskSourceType.INPUT
+                        and root_src.source_type is InputSourceType.TASK
+                        and root_src.task_source_type is TaskSourceType.OUTPUT
+                        and source.task_ref == root_src.task_ref
+                    ):
+                        continue
+
                 element_set.input_sources.update({input_type: [source]})
+                if not has_root_param:
+                    set_root_params.append(input_type)
 
         # TODO: collate all input sources separately, then can fall back to a different
         # input source (if it was not specified manually) and if the "top" input source
         # results in no available elements due to `allow_non_coincident_task_sources`.
 
         if not element_set.allow_non_coincident_task_sources:
             sources_by_task = {}
@@ -1642,15 +1697,18 @@
             # This might need changing once/if we start caching Element objects.
             for iter_i in element.iterations:
                 if not iter_i.EARs_initialised:
                     try:
                         self._initialise_element_iter_EARs(iter_i)
                         initialised.append(iter_i.id_)
                     except UnsetParameterDataError:
-                        # raised by `test_action_rule`; cannot yet initialise EARs
+                        # raised by `Action.test_rules`; cannot yet initialise EARs
+                        self.app.logger.debug(
+                            f"UnsetParameterDataError raised: cannot yet initialise runs."
+                        )
                         pass
                     else:
                         iter_i._EARs_initialised = True
                         self.workflow.set_EARs_initialised(iter_i.id_)
         return initialised
 
     def _initialise_element_iter_EARs(self, element_iter: app.ElementIteration) -> None:
@@ -1664,21 +1722,18 @@
         count = 0
         for act_idx, action in self.template.all_schema_actions():
             log_common = (
                 f"for action {act_idx} of element iteration {element_iter.index} of "
                 f"element {element_iter.element.index} of task {self.unique_name!r}."
             )
             # TODO: when we support adding new runs, we will probably pass additional
-            # run-specific data index to `test_action_rule` and `generate_data_index`
+            # run-specific data index to `test_rules` and `generate_data_index`
             # (e.g. if we wanted to increase the memory requirements of a action because
             # it previously failed)
-            rules_valid = [
-                self.test_action_rule(action=action, act_rule=i, elem_iter=element_iter)
-                for i in action.rules
-            ]
+            rules_valid = action.test_rules(element_iter=element_iter)
             if all(rules_valid):
                 self.app.logger.info(f"All action rules evaluated to true {log_common}")
                 EAR_ID = self.workflow.num_EARs + count
                 param_source = {
                     "type": "EAR_output",
                     "EAR_ID": EAR_ID,
                 }
@@ -2033,202 +2088,338 @@
             self,
             path=path,
             return_element_parameters=False,
             raise_on_missing=raise_on_missing,
             default=default,
         )
 
-    def _path_to_parameter(self, path):
-        if len(path) != 2 or path[0] == "resources":
-            return
+    def _paths_to_PV_classes(self, paths: Iterable[str]) -> Dict:
+        """Return a dict mapping dot-delimited string input paths to `ParameterValue`
+        classes."""
+
+        params = {}
+        for path in paths:
+            path_split = path.split(".")
+            if len(path_split) == 1 or path_split[0] not in ("inputs", "outputs"):
+                continue
+
+            # top-level parameter can be found via the task schema:
+            key_0 = ".".join(path_split[:2])
 
-        if path[0] == "inputs":
-            try:
-                path_1 = path[1].split("[")[0]
-            except IndexError:
-                path_1 = path[1]
-            for i in self.template.schemas:
-                for j in i.inputs:
-                    if j.parameter.typ == path_1:
-                        return j.parameter
-
-        elif path[0] == "outputs":
-            for i in self.template.schemas:
-                for j in i.outputs:
-                    if j.parameter.typ == path[1]:
-                        return j.parameter
+            if key_0 not in params:
+                if path_split[0] == "inputs":
+                    try:
+                        path_1 = path_split[1].split("[")[0]
+                    except IndexError:
+                        path_1 = path_split[1]
+                    for i in self.template.schemas:
+                        for j in i.inputs:
+                            if j.parameter.typ == path_1 and j.parameter._value_class:
+                                params[key_0] = j.parameter._value_class
+
+                elif path_split[0] == "outputs":
+                    for i in self.template.schemas:
+                        for j in i.outputs:
+                            if (
+                                j.parameter.typ == path_split[1]
+                                and j.parameter._value_class
+                            ):
+                                params[key_0] = j.parameter._value_class
+
+            if path_split[2:]:
+                pv_classes = ParameterValue.__subclasses__()
+
+            # now proceed by searching for sub-parameters in each ParameterValue
+            # sub-class:
+            for idx, part_i in enumerate(path_split[2:], start=2):
+                parent = path_split[:idx]  # e.g. ["inputs", "p1"]
+                child = path_split[: idx + 1]  # e.g. ["inputs", "p1", "sub_param"]
+                key_i = ".".join(child)
+                if key_i in params:
+                    continue
+                parent_param = params.get(".".join(parent))
+                if parent_param:
+                    for attr_name, sub_type in parent_param._sub_parameters.items():
+                        if part_i == attr_name:
+                            # find the class with this `typ` attribute:
+                            for cls_i in pv_classes:
+                                if cls_i._typ == sub_type:
+                                    params[key_i] = cls_i
+                                    break
+
+        return params
 
     def _get_merged_parameter_data(
         self,
         data_index,
         path=None,
         raise_on_missing=False,
         raise_on_unset=False,
         default: Any = None,
     ):
         """Get element data from the persistent store."""
 
-        path = [] if not path else path.split(".")
-
-        parameter = self._path_to_parameter(path)
-        sources = []
-        current_value = None
-        is_cur_val_assigned = False
-        is_obj_multi = False
-        for path_i, data_idx_i in data_index.items():
-            path_i = path_i.split(".")
-            is_parent = False
-            is_update = False
-            try:
-                rel_path = get_relative_path(path, path_i)
-                is_parent = True
-            except ValueError:
+        def _get_relevant_paths(
+            data_index: Dict, path: List[str], children_of: str = None
+        ):
+            relevant_paths = {}
+            # first extract out relevant paths in `data_index`:
+            for path_i in data_index:
+                path_i_split = path_i.split(".")
                 try:
-                    update_path = get_relative_path(path_i, path)
-                    is_update = True
-
+                    rel_path = get_relative_path(path, path_i_split)
+                    relevant_paths[path_i] = {"type": "parent", "relative_path": rel_path}
                 except ValueError:
-                    # no intersection between paths
-                    continue
+                    try:
+                        update_path = get_relative_path(path_i_split, path)
+                        relevant_paths[path_i] = {
+                            "type": "update",
+                            "update_path": update_path,
+                        }
+                    except ValueError:
+                        # no intersection between paths
+                        if children_of and path_i.startswith(children_of):
+                            relevant_paths[path_i] = {"type": "sibling"}
+                        continue
 
-            is_multi = False
-            if isinstance(data_idx_i, list):
-                is_multi = True
-                if path_i == path:
-                    # print(f"{is_obj_multi=}")
-                    is_obj_multi = True
-            else:
-                data_idx_i = [data_idx_i]
+            return relevant_paths
 
-            data = []
-            for data_idx_i_j in data_idx_i:
-                if path_i[0] == "repeats":
-                    # data is an integer repeats index, rather than a parameter ID:
-                    data_j = data_idx_i_j
-                else:
-                    param_j = self.workflow.get_parameter(data_idx_i_j)
-                    if param_j.file:
-                        if param_j.file["store_contents"]:
-                            data_j = Path(self.workflow.path) / param_j.file["path"]
-                        else:
-                            data_j = Path(param_j.file["path"])
-                        data_j = data_j.as_posix()
+        def _get_relevant_data(relevant_data_idx: Dict, raise_on_unset: bool, path: str):
+            relevant_data = {}
+            for path_i, data_idx_i in relevant_data_idx.items():
+                is_multi = isinstance(data_idx_i, list)
+                if not is_multi:
+                    data_idx_i = [data_idx_i]
+
+                data_i = []
+                methods_i = []
+                is_param_set_i = []
+                for data_idx_ij in data_idx_i:
+                    meth_i = None
+                    is_set_i = True
+                    if path_i[0] == "repeats":
+                        # data is an integer repeats index, rather than a parameter ID:
+                        data_j = data_idx_ij
                     else:
-                        data_j = param_j.data
-                        if parameter and len(path_i) == 2:
-                            # retrieve the source if this is a non-sub parameter, so we can,
-                            # in the case that there is an associated `ParameterValue` class,
-                            # get the class method that should be invoked to initialise the
-                            # object:
-                            if is_multi:
-                                sources.append(param_j.source)
+                        param_j = self.workflow.get_parameter(data_idx_ij)
+                        is_set_i = param_j.is_set
+                        if param_j.file:
+                            if param_j.file["store_contents"]:
+                                data_j = Path(self.workflow.path) / param_j.file["path"]
+                            else:
+                                data_j = Path(param_j.file["path"])
+                            data_j = data_j.as_posix()
+                        else:
+                            meth_i = param_j.source.get("value_class_method")
+                            if param_j.is_pending:
+                                # if pending, we need to convert `ParameterValue` objects
+                                # to their dict representation, so they can be merged with
+                                # other data:
+                                try:
+                                    data_j = param_j.data.to_dict()
+                                except AttributeError:
+                                    data_j = param_j.data
                             else:
-                                sources = param_j.source
-                    if raise_on_unset and not param_j.is_set:
-                        raise UnsetParameterDataError(
-                            f"Element data path {path!r} resolves to unset data for (at "
-                            f"least) data index path: {path_i!r}."
+                                # if not pending, data will be the result of an encode-
+                                # decode cycle, and it will not be initialised as an
+                                # object if the parameter is associated with a
+                                # `ParameterValue` class.
+                                data_j = param_j.data
+                        if raise_on_unset and not is_set_i:
+                            raise UnsetParameterDataError(
+                                f"Element data path {path!r} resolves to unset data for "
+                                f"(at least) data-index path: {path_i!r}."
+                            )
+                    if is_multi:
+                        data_i.append(data_j)
+                        methods_i.append(meth_i)
+                        is_param_set_i.append(is_set_i)
+                    else:
+                        data_i = data_j
+                        methods_i = meth_i
+                        is_param_set_i = is_set_i
+
+                relevant_data[path_i] = {
+                    "data": data_i,
+                    "value_class_method": methods_i,
+                    "is_set": is_param_set_i,
+                    "is_multi": is_multi,
+                }
+            if not raise_on_unset:
+                to_remove = []
+                for key, dat_info in relevant_data.items():
+                    if not dat_info["is_set"] and ((path and path in key) or not path):
+                        # remove sub-paths, as they cannot be merged with this parent
+                        to_remove.extend(
+                            k for k in relevant_data if k != key and k.startswith(key)
                         )
-                if not is_multi:
-                    data = data_j
-                else:
-                    data.append(data_j)
-
-            if is_parent:
-                # replace current value:
-                try:
-                    current_value = get_in_container(data, rel_path, cast_indices=True)
-                    is_cur_val_assigned = True
-                except (KeyError, IndexError, ValueError):
-                    continue
+                relevant_data = {
+                    k: v for k, v in relevant_data.items() if k not in to_remove
+                }
 
-            elif is_update:
-                # update sub-part of current value
-                current_value = current_value or {}
-                set_in_container(current_value, update_path, data, ensure_path=True)
-                is_cur_val_assigned = True
+            return relevant_data
 
-        if not is_cur_val_assigned:
-            if raise_on_missing:
-                # TODO: custom exception?
-                raise ValueError(f"Path {path!r} does not exist in the element data.")
-            else:
-                current_value = default
+        def _merge_relevant_data(
+            relevant_data, relevant_paths, PV_classes, path: str, raise_on_missing: bool
+        ):
+            current_val = None
+            assigned_from_parent = False
+            val_cls_method = None
+            path_is_multi = False
+            path_is_set = False
+            for path_i, data_info_i in relevant_data.items():
+                data_i = data_info_i["data"]
+                if path_i == path:
+                    val_cls_method = data_info_i["value_class_method"]
+                    path_is_multi = data_info_i["is_multi"]
+                    path_is_set = data_info_i["is_set"]
+
+                path_info = relevant_paths[path_i]
+                path_type = path_info["type"]
+                if path_type == "parent":
+                    try:
+                        if data_info_i["is_multi"]:
+                            current_val = [
+                                get_in_container(
+                                    i,
+                                    path_info["relative_path"],
+                                    cast_indices=True,
+                                )
+                                for i in data_i
+                            ]
+                            path_is_multi = True
+                            path_is_set = data_info_i["is_set"]
+                            val_cls_method = data_info_i["value_class_method"]
+                        else:
+                            current_val = get_in_container(
+                                data_i,
+                                path_info["relative_path"],
+                                cast_indices=True,
+                            )
+                    except ContainerKeyError as err:
+                        if path_i in PV_classes:
+                            err_path = ".".join([path_i] + err.path[:-1])
+                            raise MayNeedObjectError(path=err_path)
+                        continue
+                    except (IndexError, ValueError) as err:
+                        if raise_on_missing:
+                            raise err
+                        continue
+                    else:
+                        assigned_from_parent = True
+                elif path_type == "update":
+                    current_val = current_val or {}
+                    set_in_container(
+                        current_val,
+                        path_info["update_path"],
+                        data_i,
+                        ensure_path=True,
+                    )
+            if path in PV_classes:
+                if path not in relevant_data:
+                    # requested data must be a sub-path of relevant data, so we can assume
+                    # path is set (if the parent was not set the sub-paths would be
+                    # removed in `_get_relevant_data`):
+                    path_is_set = path_is_set or True
+
+                    if not assigned_from_parent:
+                        # search for unset parents in `relevant_data`:
+                        path_split = path.split(".")
+                        for parent_i_span in range(len(path_split) - 1, 1, -1):
+                            parent_path_i = ".".join(path_split[0:parent_i_span])
+                            relevant_par = relevant_data.get(parent_path_i)
+                            par_is_set = relevant_par["is_set"]
+                            if not par_is_set or any(not i for i in par_is_set):
+                                val_cls_method = relevant_par["value_class_method"]
+                                path_is_multi = relevant_par["is_multi"]
+                                path_is_set = relevant_par["is_set"]
+                                current_val = relevant_par["data"]
+                                break
+
+                # initialise objects
+                PV_cls = PV_classes[path]
+                if path_is_multi:
+                    _current_val = []
+                    for set_i, meth_i, val_i in zip(
+                        path_is_set, val_cls_method, current_val
+                    ):
+                        if set_i and isinstance(val_i, dict):
+                            method_i = getattr(PV_cls, meth_i) if meth_i else PV_cls
+                            _cur_val_i = method_i(**val_i)
+                        else:
+                            _cur_val_i = None
+                        _current_val.append(_cur_val_i)
+                    current_val = _current_val
+                elif path_is_set and isinstance(current_val, dict):
+                    method = getattr(PV_cls, val_cls_method) if val_cls_method else PV_cls
+                    current_val = method(**current_val)
+
+            return current_val
 
-        if parameter and parameter._value_class:
-            # TODO: retrieve value class method case-insensitively!
-            if isinstance(current_value, dict):
-                # return a ParameterValue instance:
-                method_name = sources.get("value_class_method")
-                if method_name:
-                    method = getattr(parameter._value_class, method_name)
-                else:
-                    method = parameter._value_class
-                current_value = method(**current_value)
+        # TODO: custom exception?
+        missing_err = ValueError(f"Path {path!r} does not exist in the element data.")
 
-            elif is_obj_multi and isinstance(current_value[0], dict):
-                # return a list of ParameterValue instances:
-                current_value_ = []
-                for cur_val, src in zip(current_value, sources):
-                    method_name = src.get("value_class_method")
-                    if method_name:
-                        method = getattr(parameter._value_class, method_name)
-                    else:
-                        method = parameter._value_class
-                    current_value_.append(method(**cur_val))
-                current_value = current_value_
+        path_split = [] if not path else path.split(".")
 
-        return current_value
+        relevant_paths = _get_relevant_paths(data_index, path_split)
+        if not relevant_paths:
+            if raise_on_missing:
+                raise missing_err
+            return default
 
-    def test_action_rule(
-        self,
-        action: app.Action,
-        act_rule: app.ActionRule,
-        elem_iter: app.ElementIteration,
-    ) -> bool:
-        schema_data_idx = elem_iter.data_idx
-        check = act_rule.check_exists or act_rule.check_missing
-        if check:
-            param_s = check.split(".")
-            if len(param_s) > 2:
-                # sub-parameter, so need to try to retrieve parameter data
-                try:
-                    self._get_merged_parameter_data(
-                        schema_data_idx, raise_on_missing=True
-                    )
-                    return True if act_rule.check_exists else False
-                except ValueError:
-                    return False if act_rule.check_exists else True
+        relevant_data_idx = {k: v for k, v in data_index.items() if k in relevant_paths}
+        PV_cls_paths = list(relevant_paths.keys()) + ([path] if path else [])
+        PV_classes = self._paths_to_PV_classes(PV_cls_paths)
+        relevant_data = _get_relevant_data(relevant_data_idx, raise_on_unset, path)
+
+        current_val = None
+        is_assigned = False
+        try:
+            current_val = _merge_relevant_data(
+                relevant_data, relevant_paths, PV_classes, path, raise_on_missing
+            )
+        except MayNeedObjectError as err:
+            path_to_init = err.path
+            path_to_init_split = path_to_init.split(".")
+            relevant_paths = _get_relevant_paths(data_index, path_to_init_split)
+            PV_cls_paths = list(relevant_paths.keys()) + [path_to_init]
+            PV_classes = self._paths_to_PV_classes(PV_cls_paths)
+            relevant_data_idx = {
+                k: v for k, v in data_index.items() if k in relevant_paths
+            }
+            relevant_data = _get_relevant_data(relevant_data_idx, raise_on_unset, path)
+            # merge the parent data
+            current_val = _merge_relevant_data(
+                relevant_data, relevant_paths, PV_classes, path_to_init, raise_on_missing
+            )
+            # try to retrieve attributes via the initialised object:
+            rel_path_split = get_relative_path(path_split, path_to_init_split)
+            try:
+                current_val = get_in_container(
+                    current_val,
+                    rel_path_split,
+                    cast_indices=True,
+                    allow_getattr=True,
+                )
+            except (KeyError, IndexError, ValueError):
+                pass
             else:
-                if act_rule.check_exists:
-                    return act_rule.check_exists in schema_data_idx
-                elif act_rule.check_missing:
-                    return act_rule.check_missing not in schema_data_idx
+                is_assigned = True
 
+        except (KeyError, IndexError, ValueError):
+            pass
         else:
-            rule = act_rule.rule
-            param_path = ".".join(i.condition.callable.kwargs["value"] for i in rule.path)
-            if param_path.startswith("resources."):
-                elem_res = elem_iter.get_resources(action=action, set_defaults=True)
-                res_path = param_path.split(".")[1:]
-                element_dat = get_in_container(
-                    cont=elem_res, path=res_path, cast_indices=True
-                )
-            else:
-                element_dat = self._get_merged_parameter_data(
-                    schema_data_idx,
-                    path=param_path,
-                    raise_on_missing=True,
-                    raise_on_unset=True,
-                )
-            # test the rule:
-            # note: valida can't `rule.test` scalars yet, so wrap it in a list and set
-            # path to first element (see: https://github.com/hpcflow/valida/issues/9):
-            rule = Rule(path=[0], condition=rule.condition, cast=rule.cast)
-            return rule.test([element_dat]).is_valid
+            is_assigned = True
+
+        if not is_assigned:
+            if raise_on_missing:
+                raise missing_err
+            current_val = default
+
+        return current_val
 
 
 class Elements:
     __slots__ = ("_task",)
 
     def __init__(self, task: app.WorkflowTask):
         self._task = task
@@ -2298,14 +2489,15 @@
 class Parameters:
     _app_attr = "_app"
 
     task: app.WorkflowTask
     path: str
     return_element_parameters: bool
     raise_on_missing: Optional[bool] = False
+    raise_on_unset: Optional[bool] = False
     default: Optional[Any] = None
 
     def islice(self, start=None, end=None):
         for i in self.task.workflow.pIO.task_parameter_islice(
             self.task, self.path, start, end
         ):
             yield i
@@ -2349,14 +2541,15 @@
                 for i in elements
             ]
         else:
             params = [
                 i.get(
                     path=self.path,
                     raise_on_missing=self.raise_on_missing,
+                    raise_on_unset=self.raise_on_unset,
                     default=self.default,
                 )
                 for i in elements
             ]
 
         if length == 1:
             return params[0]
```

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/sdk/core/task_schema.py` & `hpcflow_new2-0.2.0a99/hpcflow/sdk/core/task_schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from contextlib import contextmanager
 import copy
 from dataclasses import dataclass, field
+from importlib import import_module
 from typing import Dict, List, Optional, Tuple, Union
 
 from rich import print as rich_print
 from rich.table import Table
 
 from hpcflow.sdk import app
 from hpcflow.sdk.core.parameters import Parameter
@@ -75,31 +76,35 @@
         objective: Union[app.TaskObjective, str],
         actions: List[app.Action] = None,
         method: Optional[str] = None,
         implementation: Optional[str] = None,
         inputs: Optional[List[Union[app.Parameter, app.SchemaInput]]] = None,
         outputs: Optional[List[Union[app.Parameter, app.SchemaOutput]]] = None,
         version: Optional[str] = None,
+        parameter_class_modules: Optional[List[str]] = None,
         _hash_value: Optional[str] = None,
     ):
         self.objective = objective
         self.actions = actions or []
         self.method = method
         self.implementation = implementation
         self.inputs = inputs or []
         self.outputs = outputs or []
+        self.parameter_class_modules = parameter_class_modules or []
         self._hash_value = _hash_value
 
         self._set_parent_refs()
 
         self._validate()
         self.actions = self._expand_actions()
         self.version = version
         self._task_template = None  # assigned by parent Task
 
+        self._update_parameter_value_classes()
+
         # if version is not None:  # TODO: this seems fragile
         #     self.assign_versions(
         #         version=version,
         #         app_data_obj_list=self.app.task_schemas
         #         if app.is_data_files_loaded
         #         else [],
         #     )
@@ -263,14 +268,28 @@
                 )
 
     def _expand_actions(self):
         """Create new actions for input file generators and output parsers in existing
         actions."""
         return [j for i in self.actions for j in i.expand()]
 
+    def _update_parameter_value_classes(self):
+        # ensure any referenced parameter_class_modules are imported:
+        for module in self.parameter_class_modules:
+            import_module(module)
+
+        # TODO: support specifying file paths in addition to (instead of?) importable
+        # module paths
+
+        for inp in self.inputs:
+            inp.parameter._set_value_class()
+
+        for out in self.outputs:
+            out.parameter._set_value_class()
+
     def make_persistent(self, workflow: app.Workflow, source: Dict) -> List[int]:
         new_refs = []
         for input_i in self.inputs:
             for lab_info in input_i.labelled_info():
                 if "default_value" in lab_info:
                     _, dat_ref, is_new = lab_info["default_value"].make_persistent(
                         workflow, source
```

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/sdk/core/test_utils.py` & `hpcflow_new2-0.2.0a99/hpcflow/sdk/core/test_utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -151,16 +151,93 @@
         overwrite=overwrite,
         store=store,
     )
     return wk
 
 
 @dataclass
+class P1_sub_parameter_cls(ParameterValue):
+    _typ = "p1_sub"
+
+    e: int
+
+    def CLI_format(self) -> str:
+        return str(self.e)
+
+    @property
+    def twice_e(self):
+        return self.e * 2
+
+
+@dataclass
+class P1_sub_parameter_cls_2(ParameterValue):
+    _typ = "p1_sub_2"
+
+    f: int
+
+
+@dataclass
 class P1_parameter_cls(ParameterValue):
-    _typ = "p1"
+    _typ = "p1c"
+    _sub_parameters = {"sub_param": "p1_sub", "sub_param_2": "p1_sub_2"}
 
     a: int
     d: Optional[int] = None
+    sub_param: Optional[P1_sub_parameter_cls] = None
+
+    def __post_init__(self):
+        if self.sub_param is not None and not isinstance(
+            self.sub_param, P1_sub_parameter_cls
+        ):
+            self.sub_param = P1_sub_parameter_cls(**self.sub_param)
 
     @classmethod
     def from_data(cls, b, c):
         return cls(a=b + c)
+
+    @property
+    def twice_a(self):
+        return self.a * 2
+
+    @property
+    def sub_param_prop(self):
+        return P1_sub_parameter_cls(e=4 * self.a)
+
+    def CLI_format(self) -> str:
+        return str(self.a)
+
+    @staticmethod
+    def CLI_format_group(*objs) -> str:
+        pass
+
+    @staticmethod
+    def sum(*objs, **kwargs) -> str:
+        return str(sum(i.a for i in objs))
+
+    def custom_CLI_format(
+        self, add: Optional[str] = None, sub: Optional[str] = None
+    ) -> str:
+        add = 4 if add is None else int(add)
+        sub = 0 if sub is None else int(sub)
+        return str(self.a + add - sub)
+
+    def custom_CLI_format_prep(self, reps: Optional[str] = None) -> List[int]:
+        """Used for testing custom object CLI formatting.
+
+        For example, with a command like this:
+
+        `<<join[delim=","](parameter:p1c.custom_CLI_format_prep(reps=4))>>`.
+
+        """
+        reps = 1 if reps is None else int(reps)
+        return [self.a] * reps
+
+    @classmethod
+    def CLI_parse(cls, a_str: str, double: Optional[str] = "", e: Optional[str] = None):
+        a = int(a_str)
+        if double.lower() == "true":
+            a *= 2
+        if e:
+            sub_param = P1_sub_parameter_cls(e=int(e))
+        else:
+            sub_param = None
+        return cls(a=a, sub_param=sub_param)
```

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/sdk/core/utils.py` & `hpcflow_new2-0.2.0a99/hpcflow/sdk/core/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,19 @@
 from typing import Type, Union, List, Mapping
 import fsspec
 
 from ruamel.yaml import YAML
 import sentry_sdk
 from watchdog.utils.dirsnapshot import DirectorySnapshot
 
-from hpcflow.sdk.core.errors import FromSpecMissingObjectError, InvalidIdentifier
+from hpcflow.sdk.core.errors import (
+    ContainerKeyError,
+    FromSpecMissingObjectError,
+    InvalidIdentifier,
+)
 from hpcflow.sdk.typing import PathLike
 
 
 def load_config(func):
     """API function decorator to ensure the configuration has been loaded, and load if not."""
 
     @wraps(func)
@@ -141,16 +145,20 @@
 
         if not is_vals_equal:
             grouped.append([lst_item])
 
     return grouped
 
 
-def get_in_container(cont, path, cast_indices=False):
+def get_in_container(cont, path, cast_indices=False, allow_getattr=False):
     cur_data = cont
+    err_msg = (
+        "Data at path {path_comps!r} is not a sequence, but is of type "
+        "{cur_data_type!r} and so sub-data cannot be extracted."
+    )
     for idx, path_comp in enumerate(path):
         if isinstance(cur_data, (list, tuple)):
             if not isinstance(path_comp, int):
                 msg = (
                     f"Path component {path_comp!r} must be an integer index "
                     f"since data is a sequence: {cur_data!r}."
                 )
@@ -158,20 +166,29 @@
                     try:
                         path_comp = int(path_comp)
                     except TypeError:
                         raise TypeError(msg)
                 else:
                     raise TypeError(msg)
             cur_data = cur_data[path_comp]
-        elif isinstance(cur_data, Mapping):
-            cur_data = cur_data[path_comp]
+        elif isinstance(cur_data, dict):
+            try:
+                cur_data = cur_data[path_comp]
+            except KeyError:
+                raise ContainerKeyError(path=path[: idx + 1])
+        elif allow_getattr:
+            try:
+                cur_data = getattr(cur_data, path_comp)
+            except AttributeError:
+                raise ValueError(
+                    err_msg.format(cur_data_type=type(cur_data), path_comps=path[:idx])
+                )
         else:
             raise ValueError(
-                f"Data at path {path[:idx]} is not a sequence, but is of type "
-                f"{type(cur_data)!r} and so sub-data cannot be extracted."
+                err_msg.format(cur_data_type=type(cur_data), path_comps=path[:idx])
             )
     return cur_data
 
 
 def set_in_container(cont, path, value, ensure_path=False, cast_indices=False):
     if ensure_path:
         num_path = len(path)
```

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/sdk/core/validation.py` & `hpcflow_new2-0.2.0a99/hpcflow/sdk/core/validation.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/sdk/core/workflow.py` & `hpcflow_new2-0.2.0a99/hpcflow/sdk/core/workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -2242,34 +2242,49 @@
         JS_action_idx: int,
         EAR_ID: int,
     ) -> None:
         """Write run-time commands for a given EAR."""
         with self._store.cached_load():
             jobscript = self.submissions[submission_idx].jobscripts[jobscript_idx]
             EAR = self.get_EARs_from_IDs([EAR_ID])[0]
-            commands, shell_vars = EAR.compose_commands(jobscript, JS_action_idx)
-            for param_name, shell_var_name in shell_vars:
+            commands, shell_vars, indices = EAR.compose_commands(jobscript, JS_action_idx)
+            for cmd_idx, (param_name, shell_var_name, st_typ) in zip(indices, shell_vars):
                 commands += jobscript.shell.format_save_parameter(
                     workflow_app_alias=jobscript.workflow_app_alias,
                     param_name=param_name,
                     shell_var_name=shell_var_name,
                     EAR_ID=EAR_ID,
+                    cmd_idx=cmd_idx,
+                    stderr=(st_typ == "stderr"),
                 )
             commands = jobscript.shell.wrap_in_subshell(commands, EAR.action.abortable)
             cmd_file_name = jobscript.get_commands_file_name(JS_action_idx)
             with Path(cmd_file_name).open("wt", newline="\n") as fp:
                 # (assuming we have CD'd correctly to the element run directory)
                 fp.write(commands)
 
+    def process_shell_parameter_output(
+        self, name: str, value: str, EAR_ID: int, cmd_idx: int, stderr: bool = False
+    ) -> Any:
+        """Process the shell stdout/stderr stream according to the associated Command
+        object."""
+        with self._store.cached_load():
+            with self.batch_update():
+                EAR = self.get_EARs_from_IDs([EAR_ID])[0]
+                command = EAR.action.commands[cmd_idx]
+                return command.process_std_stream(name, value, stderr)
+
     def save_parameter(
         self,
         name: str,
         value: Any,
         EAR_ID: int,
     ):
+        self.app.logger.info(f"save parameter {name!r} for EAR_ID {EAR_ID}.")
+        self.app.logger.debug(f"save parameter {name!r} value is {value!r}.")
         with self._store.cached_load():
             with self.batch_update():
                 EAR = self.get_EARs_from_IDs([EAR_ID])[0]
                 param_id = EAR.data_idx[name]
                 self.set_parameter_value(param_id, value)
 
     def show_all_EAR_statuses(self):
```

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/sdk/core/zarr_io.py` & `hpcflow_new2-0.2.0a99/hpcflow/sdk/core/zarr_io.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/sdk/data/config_file_schema.yaml` & `hpcflow_new2-0.2.0a99/hpcflow/sdk/data/config_file_schema.yaml`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/sdk/data/config_schema.yaml` & `hpcflow_new2-0.2.0a99/hpcflow/sdk/data/config_schema.yaml`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/sdk/data/environments_spec_schema.yaml` & `hpcflow_new2-0.2.0a99/hpcflow/sdk/data/environments_spec_schema.yaml`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/sdk/data/template_components/task_schemas.yaml` & `hpcflow_new2-0.2.0a99/hpcflow/sdk/data/template_components/task_schemas.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -29,28 +29,26 @@
 - objective: test_t1_conditional_OS
   inputs:
     - parameter: p1
   outputs:
     - parameter: p2
   actions:
     - rules:
-        - rule:
-            path: [resources.os_name]
-            condition: { value.equal_to: posix }
+        - path: resources.os_name
+          condition: { value.equal_to: posix }
       environments:
         - scope:
             type: any
           environment: null_env
       commands:
         - command: echo "$((<<parameter:p1>> + 100))"
           stdout: <<parameter:p2>>
     - rules:
-        - rule:
-            path: [resources.os_name]
-            condition: { value.equal_to: nt }
+        - path: resources.os_name
+          condition: { value.equal_to: nt }
       environments:
         - scope:
             type: any
           environment: null_env
       commands:
         - command: Write-Output ((<<parameter:p1>> + 100))
           stdout: <<parameter:p2>>
```

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/sdk/data/workflow_spec_schema.yaml` & `hpcflow_new2-0.2.0a99/hpcflow/sdk/data/workflow_spec_schema.yaml`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/sdk/demo/cli.py` & `hpcflow_new2-0.2.0a99/hpcflow/sdk/demo/cli.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/sdk/demo/data/workflow_test_run_abort.yaml` & `hpcflow_new2-0.2.0a99/hpcflow/sdk/demo/data/workflow_test_run_abort.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -10,37 +10,33 @@
     inputs:
       - parameter: sleep_time_seconds
     outputs:
       - parameter: is_finished
     actions:
       - abortable: true
         rules:
-          - rule:
-              path: [resources.os_name]
-              condition: { value.equal_to: posix }
+          - path: resources.os_name
+            condition: { value.equal_to: posix }
         commands:
           - command: sleep <<parameter:sleep_time_seconds>>
       - abortable: true
         rules:
-          - rule:
-              path: [resources.os_name]
-              condition: { value.equal_to: nt }
+          - path: resources.os_name
+            condition: { value.equal_to: nt }
         commands:
           - command: Start-Sleep <<parameter:sleep_time_seconds>>
       - rules:
-          - rule:
-              path: [resources.os_name]
-              condition: { value.equal_to: posix }
+          - path: resources.os_name
+            condition: { value.equal_to: posix }
         commands:
           - command: echo "true"
             stdout: <<parameter:is_finished>>
       - rules:
-          - rule:
-              path: [resources.os_name]
-              condition: { value.equal_to: nt }
+          - path: resources.os_name
+            condition: { value.equal_to: nt }
         commands:
           - command: Write-Output "true"
             stdout: <<parameter:is_finished>>
 
 tasks:
   - schemas: [sleep]
     inputs:
```

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/sdk/helper/cli.py` & `hpcflow_new2-0.2.0a99/hpcflow/sdk/helper/cli.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/sdk/helper/helper.py` & `hpcflow_new2-0.2.0a99/hpcflow/sdk/helper/helper.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/sdk/helper/watcher.py` & `hpcflow_new2-0.2.0a99/hpcflow/sdk/helper/watcher.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/sdk/log.py` & `hpcflow_new2-0.2.0a99/hpcflow/sdk/log.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/sdk/persistence/__init__.py` & `hpcflow_new2-0.2.0a99/hpcflow/sdk/persistence/__init__.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/sdk/persistence/base.py` & `hpcflow_new2-0.2.0a99/hpcflow/sdk/persistence/base.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/sdk/persistence/json.py` & `hpcflow_new2-0.2.0a99/hpcflow/sdk/persistence/json.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/sdk/persistence/pending.py` & `hpcflow_new2-0.2.0a99/hpcflow/sdk/persistence/pending.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/sdk/persistence/store_resource.py` & `hpcflow_new2-0.2.0a99/hpcflow/sdk/persistence/store_resource.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/sdk/persistence/utils.py` & `hpcflow_new2-0.2.0a99/hpcflow/sdk/persistence/utils.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/sdk/persistence/zarr.py` & `hpcflow_new2-0.2.0a99/hpcflow/sdk/persistence/zarr.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/sdk/runtime.py` & `hpcflow_new2-0.2.0a99/hpcflow/sdk/runtime.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/sdk/submission/jobscript.py` & `hpcflow_new2-0.2.0a99/hpcflow/sdk/submission/jobscript.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/sdk/submission/jobscript_info.py` & `hpcflow_new2-0.2.0a99/hpcflow/sdk/submission/jobscript_info.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/sdk/submission/schedulers/__init__.py` & `hpcflow_new2-0.2.0a99/hpcflow/sdk/submission/schedulers/__init__.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/sdk/submission/schedulers/direct.py` & `hpcflow_new2-0.2.0a99/hpcflow/sdk/submission/schedulers/direct.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/sdk/submission/schedulers/sge.py` & `hpcflow_new2-0.2.0a99/hpcflow/sdk/submission/schedulers/sge.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/sdk/submission/schedulers/slurm.py` & `hpcflow_new2-0.2.0a99/hpcflow/sdk/submission/schedulers/slurm.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/sdk/submission/shells/__init__.py` & `hpcflow_new2-0.2.0a99/hpcflow/sdk/submission/shells/__init__.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/sdk/submission/shells/base.py` & `hpcflow_new2-0.2.0a99/hpcflow/sdk/submission/shells/base.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/sdk/submission/shells/bash.py` & `hpcflow_new2-0.2.0a99/hpcflow/sdk/submission/shells/bash.py`

 * *Files 3% similar despite different names*

```diff
@@ -168,20 +168,30 @@
         app_invoc_exe = app_invoc_exe.replace(" ", r"\ ")
         return app_invoc_exe
 
     def format_stream_assignment(self, shell_var_name, command):
         return f"{shell_var_name}=`{command}`"
 
     def format_save_parameter(
-        self, workflow_app_alias, param_name, shell_var_name, EAR_ID
+        self,
+        workflow_app_alias: str,
+        param_name: str,
+        shell_var_name: str,
+        EAR_ID: int,
+        cmd_idx: int,
+        stderr: bool,
     ):
+        # TODO: quote shell_var_name as well? e.g. if it's a white-space delimited list?
+        #   and test.
+        stderr_str = " --stderr" if stderr else ""
         return (
-            f"{workflow_app_alias}"
-            f' internal workflow "$WK_PATH_ARG" save-parameter {param_name} ${shell_var_name}'
-            f' {EAR_ID} >> "$app_stream_file" 2>&1'
+            f"{workflow_app_alias} "
+            f'internal workflow "$WK_PATH_ARG" save-parameter '
+            f"{param_name} ${shell_var_name} {EAR_ID} {cmd_idx}{stderr_str} "
+            f'>> "$app_stream_file" 2>&1'
             f"\n"
         )
 
     def wrap_in_subshell(self, commands: str, abortable: bool) -> str:
         """Format commands to run within a subshell.
 
         This assumes commands ends in a newline.
```

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/sdk/submission/shells/os_version.py` & `hpcflow_new2-0.2.0a99/hpcflow/sdk/submission/shells/os_version.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/sdk/submission/shells/powershell.py` & `hpcflow_new2-0.2.0a99/hpcflow/sdk/submission/shells/powershell.py`

 * *Files 5% similar despite different names*

```diff
@@ -171,20 +171,30 @@
             app_invoc_exe = f"& '{app_invoc_exe}'"
         return app_invoc_exe
 
     def format_stream_assignment(self, shell_var_name, command):
         return f"${shell_var_name} = {command}"
 
     def format_save_parameter(
-        self, workflow_app_alias, param_name, shell_var_name, EAR_ID
+        self,
+        workflow_app_alias: str,
+        param_name: str,
+        shell_var_name: str,
+        EAR_ID: int,
+        cmd_idx: int,
+        stderr: bool,
     ):
+        # TODO: quote shell_var_name as well? e.g. if it's a white-space delimited list?
+        #   and test.
+        stderr_str = " --stderr" if stderr else ""
         return (
-            f"{workflow_app_alias}"
-            f" internal workflow $WK_PATH save-parameter {param_name} ${shell_var_name}"
-            f" {EAR_ID} 2>&1 >> $app_stream_file"
+            f"{workflow_app_alias} "
+            f"internal workflow $WK_PATH save-parameter "
+            f"{param_name} ${shell_var_name} {EAR_ID} {cmd_idx}{stderr_str} "
+            f"2>&1 >> $app_stream_file"
             f"\n"
         )
 
     def wrap_in_subshell(self, commands: str, abortable: bool) -> str:
         """Format commands to run within a child scope.
 
         This assumes `commands` ends in a newline.
```

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/sdk/submission/submission.py` & `hpcflow_new2-0.2.0a99/hpcflow/sdk/submission/submission.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/tests/conftest.py` & `hpcflow_new2-0.2.0a99/hpcflow/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/tests/shells/wsl/test_wsl_submission.py` & `hpcflow_new2-0.2.0a99/hpcflow/tests/shells/wsl/test_wsl_submission.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/tests/unit/test_app.py` & `hpcflow_new2-0.2.0a99/hpcflow/tests/unit/test_app.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/tests/unit/test_config.py` & `hpcflow_new2-0.2.0a99/hpcflow/tests/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/tests/unit/test_config_file.py` & `hpcflow_new2-0.2.0a99/hpcflow/tests/unit/test_config_file.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/tests/unit/test_element_set.py` & `hpcflow_new2-0.2.0a99/hpcflow/tests/unit/test_element_set.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/tests/unit/test_input_value.py` & `hpcflow_new2-0.2.0a99/hpcflow/tests/unit/test_input_value.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import pytest
 
 from hpcflow.app import app as hf
 from hpcflow.sdk.core.errors import InputValueDuplicateSequenceAddress
+from hpcflow.sdk.core.test_utils import P1_parameter_cls as P1
 
 
 @pytest.fixture
 def null_config(tmp_path):
     if not hf.is_config_loaded:
         hf.load_config(config_dir=tmp_path)
 
@@ -131,7 +132,24 @@
     inp = hf.InputValue.from_json_like(
         json_like={"parameter": "p1[1]", "value": 101},
         shared_data=hf.template_components,
     )
     assert inp.parameter.typ == hf.Parameter("p1").typ
     assert inp.value == 101
     assert inp.label == "1"
+
+
+def test_value_is_dict_check_success(null_config):
+    # Parameter("p1c") has an associated `ParameterValue` class, so data should be a dict:
+    hf.InputValue("p1c", {"a": 101})
+
+
+def test_value_is_dict_check_raise(null_config):
+    # Parameter("p1c") has an associated `ParameterValue` class so data should be a dict:
+    with pytest.raises(ValueError):
+        hf.InputValue("p1c", 101)
+
+
+def test_value_is_dict_check_no_raise_if_sub_parameter(null_config):
+    # Parameter("p1c") has an associated `ParameterValue` class, but the specified value
+    # is for some sub-data:
+    hf.InputValue("p1c", path="a", value=101)
```

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/tests/unit/test_json_like.py` & `hpcflow_new2-0.2.0a99/hpcflow/tests/unit/test_json_like.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/tests/unit/test_loop.py` & `hpcflow_new2-0.2.0a99/hpcflow/tests/unit/test_loop.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/tests/unit/test_object_list.py` & `hpcflow_new2-0.2.0a99/hpcflow/tests/unit/test_object_list.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/tests/unit/test_persistence.py` & `hpcflow_new2-0.2.0a99/hpcflow/tests/unit/test_persistence.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/tests/unit/test_resources.py` & `hpcflow_new2-0.2.0a99/hpcflow/tests/unit/test_resources.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/tests/unit/test_schema_input.py` & `hpcflow_new2-0.2.0a99/hpcflow/tests/unit/test_schema_input.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,27 +165,29 @@
 
 def test_get_input_values_for_multiple_schema_input_with_object(null_config, tmp_path):
     p1_val = P1(a=101)
     label = "my_label"
     s1 = hf.TaskSchema(
         objective="t1",
         inputs=[
-            hf.SchemaInput(parameter="p1", labels={label: {}}, multiple=True),
+            hf.SchemaInput(parameter="p1c", labels={label: {}}, multiple=True),
             hf.SchemaInput(parameter="p2", default_value=201),
         ],
         actions=[
             hf.Action(
                 environments=[hf.ActionEnvironment(environment=hf.envs.null_env)],
                 commands=[
-                    hf.Command(command=f"echo <<parameter:p1[{label}]>> <<parameter:p2>>")
+                    hf.Command(
+                        command=f"echo <<parameter:p1c[{label}]>> <<parameter:p2>>"
+                    )
                 ],
             ),
         ],
     )
-    t1 = hf.Task(schemas=[s1], inputs=[hf.InputValue("p1", p1_val, label=label)])
+    t1 = hf.Task(schemas=[s1], inputs=[hf.InputValue("p1c", p1_val, label=label)])
     wk = hf.Workflow.from_template_data(
         tasks=[t1],
         path=tmp_path,
         template_name="temp",
     )
     run = wk.tasks[0].elements[0].iterations[0].action_runs[0]
-    assert run.get_input_values() == {"p2": 201, "p1": {label: p1_val}}
+    assert run.get_input_values() == {"p2": 201, "p1c": {label: p1_val}}
```

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/tests/unit/test_shell.py` & `hpcflow_new2-0.2.0a99/hpcflow/tests/unit/test_shell.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/tests/unit/test_submission.py` & `hpcflow_new2-0.2.0a99/hpcflow/tests/unit/test_submission.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/tests/unit/test_task.py` & `hpcflow_new2-0.2.0a99/hpcflow/tests/unit/test_task.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 import copy
 import os
 import pytest
 
-from valida.rules import Rule
 from valida.conditions import Value
 
 from hpcflow.app import app as hf
 from hpcflow.sdk.core.errors import (
     MissingInputs,
     TaskTemplateInvalidNesting,
     TaskTemplateMultipleInputValues,
     TaskTemplateMultipleSchemaObjectives,
     TaskTemplateUnexpectedInput,
+    UnsetParameterDataError,
 )
 from hpcflow.sdk.core.parameters import NullDefault
-from hpcflow.sdk.core.test_utils import make_schemas, make_tasks, make_workflow
+from hpcflow.sdk.core.test_utils import (
+    make_schemas,
+    make_tasks,
+    make_workflow,
+    P1_parameter_cls as P1,
+    P1_sub_parameter_cls as P1_sub_param,
+    P1_sub_parameter_cls_2 as P1_sub_param_2,
+)
 
 
 @pytest.fixture
 def null_config(tmp_path):
     if not hf.is_config_loaded:
         hf.load_config(config_dir=tmp_path)
 
@@ -1471,18 +1478,18 @@
     )
 
 
 @pytest.mark.parametrize("store", ["json", "zarr"])
 def test_conditional_shell_schema_single_initialised_action(null_config, tmp_path, store):
     rules = {
         "posix": hf.ActionRule(
-            rule=Rule(path=["resources.os_name"], condition=Value.equal_to("posix"))
+            rule=hf.Rule(path="resources.os_name", condition=Value.equal_to("posix"))
         ),
         "nt": hf.ActionRule(
-            rule=Rule(path=["resources.os_name"], condition=Value.equal_to("nt"))
+            rule=hf.Rule(path="resources.os_name", condition=Value.equal_to("nt"))
         ),
     }
     s1 = hf.TaskSchema(
         objective="test_conditional_on_shell",
         inputs=[hf.SchemaInput("p1")],
         outputs=[hf.SchemaInput("p2")],
         actions=[
@@ -1604,19 +1611,15 @@
                 environments=[hf.ActionEnvironment(environment=hf.envs.null_env)],
                 commands=[
                     hf.Command(
                         command="echo $((<<parameter:p2>> + 100))",
                         stdout="<<parameter:p3>>",
                     )
                 ],
-                rules=[
-                    hf.ActionRule(
-                        rule=Rule(path=["inputs.p2"], condition=Value.less_than(500))
-                    )
-                ],
+                rules=[hf.ActionRule(path="inputs.p2", condition=Value.less_than(500))],
             ),
         ],
     )
     t1 = hf.Task(schemas=[s1], inputs=[hf.InputValue("p1", 101)])
     t2 = hf.Task(schemas=[s2])
     wk = hf.Workflow.from_template_data(
         tasks=[t1, t2],
@@ -1632,18 +1635,18 @@
 
 @pytest.mark.parametrize("store", ["json", "zarr"])
 def test_element_iteration_EARs_initialised_on_make_workflow_with_no_valid_actions(
     null_config, tmp_path, store
 ):
     rules = {
         "posix": hf.ActionRule(
-            rule=Rule(path=["resources.os_name"], condition=Value.equal_to("posix"))
+            rule=hf.Rule(path="resources.os_name", condition=Value.equal_to("posix"))
         ),
         "nt": hf.ActionRule(
-            rule=Rule(path=["resources.os_name"], condition=Value.equal_to("nt"))
+            rule=hf.Rule(path="resources.os_name", condition=Value.equal_to("nt"))
         ),
     }
     s1 = hf.TaskSchema(
         objective="test_conditional_on_shell",
         inputs=[hf.SchemaInput("p1")],
         outputs=[hf.SchemaInput("p2")],
         actions=[
@@ -1666,7 +1669,417 @@
         overwrite=True,
         path=tmp_path,
         store=store,
     )
     action_runs = wk.tasks[0].elements[0].iterations[0].action_runs
     assert len(action_runs) == 0
     assert wk.tasks[0].elements[0].iterations[0].EARs_initialised
+
+
+@pytest.mark.parametrize("store", ["json", "zarr"])
+def test_get_merged_parameter_data_unset_data_raise(null_config, tmp_path, store):
+    s1 = hf.TaskSchema(
+        objective="t1",
+        inputs=[hf.SchemaInput(parameter=hf.Parameter("p1"))],
+        outputs=[hf.SchemaInput(parameter=hf.Parameter("p2"))],
+        actions=[
+            hf.Action(
+                commands=[
+                    hf.Command(
+                        command="Write-Output (<<parameter:p1>> + 100)",
+                        stdout="<<parameter:p2>>",
+                    )
+                ]
+            )
+        ],
+    )
+    t1 = hf.Task(schemas=s1, inputs=[hf.InputValue("p1", value=1)])
+    wk = hf.Workflow.from_template_data(
+        tasks=[t1],
+        template_name="w1",
+        overwrite=True,
+        path=tmp_path,
+        store=store,
+    )
+    data_idx = wk.tasks.t1.elements[0].get_data_idx()
+    with pytest.raises(UnsetParameterDataError):
+        wk.tasks.t1._get_merged_parameter_data(
+            data_index=data_idx,
+            path="outputs.p2",
+            raise_on_unset=True,
+        )
+
+
+@pytest.mark.parametrize("store", ["json", "zarr"])
+def test_get_merged_parameter_data_unset_data_no_raise(null_config, tmp_path, store):
+    s1 = hf.TaskSchema(
+        objective="t1",
+        inputs=[hf.SchemaInput(parameter=hf.Parameter("p1"))],
+        outputs=[hf.SchemaInput(parameter=hf.Parameter("p2"))],
+        actions=[
+            hf.Action(
+                commands=[
+                    hf.Command(
+                        command="Write-Output (<<parameter:p1>> + 100)",
+                        stdout="<<parameter:p2>>",
+                    )
+                ]
+            )
+        ],
+    )
+    t1 = hf.Task(schemas=s1, inputs=[hf.InputValue("p1", value=1)])
+    wk = hf.Workflow.from_template_data(
+        tasks=[t1],
+        template_name="w1",
+        overwrite=True,
+        path=tmp_path,
+        store=store,
+    )
+    data_idx = wk.tasks.t1.elements[0].get_data_idx()
+    assert None == wk.tasks.t1._get_merged_parameter_data(
+        data_index=data_idx,
+        path="outputs.p2",
+        raise_on_unset=False,
+    )
+
+
+@pytest.mark.parametrize("store", ["json", "zarr"])
+def test_get_merged_parameter_data_missing_data_raise(null_config, tmp_path, store):
+    s1 = hf.TaskSchema(
+        objective="t1",
+        inputs=[hf.SchemaInput(parameter=hf.Parameter("p1"))],
+        outputs=[hf.SchemaInput(parameter=hf.Parameter("p2"))],
+        actions=[
+            hf.Action(
+                commands=[
+                    hf.Command(
+                        command="Write-Output (<<parameter:p1>> + 100)",
+                        stdout="<<parameter:p2>>",
+                    )
+                ]
+            )
+        ],
+    )
+    t1 = hf.Task(schemas=s1, inputs=[hf.InputValue("p1", value=1)])
+    wk = hf.Workflow.from_template_data(
+        tasks=[t1],
+        template_name="w1",
+        overwrite=True,
+        path=tmp_path,
+        store=store,
+    )
+    data_idx = wk.tasks.t1.elements[0].get_data_idx()
+    with pytest.raises(ValueError):
+        wk.tasks.t1._get_merged_parameter_data(
+            data_index=data_idx,
+            path="inputs.p4",
+            raise_on_missing=True,
+        )
+
+
+@pytest.mark.parametrize("store", ["json", "zarr"])
+def test_get_merged_parameter_data_missing_data_no_raise(null_config, tmp_path, store):
+    s1 = hf.TaskSchema(
+        objective="t1",
+        inputs=[hf.SchemaInput(parameter=hf.Parameter("p1"))],
+        outputs=[hf.SchemaInput(parameter=hf.Parameter("p2"))],
+        actions=[
+            hf.Action(
+                commands=[
+                    hf.Command(
+                        command="Write-Output (<<parameter:p1>> + 100)",
+                        stdout="<<parameter:p2>>",
+                    )
+                ]
+            )
+        ],
+    )
+    t1 = hf.Task(schemas=s1, inputs=[hf.InputValue("p1", value=1)])
+    wk = hf.Workflow.from_template_data(
+        tasks=[t1],
+        template_name="w1",
+        overwrite=True,
+        path=tmp_path,
+        store=store,
+    )
+    data_idx = wk.tasks.t1.elements[0].get_data_idx()
+    assert None == wk.tasks.t1._get_merged_parameter_data(
+        data_index=data_idx,
+        path="inputs.p4",
+        raise_on_missing=False,
+    )
+
+
+@pytest.mark.parametrize("store", ["json", "zarr"])
+def test_get_merged_parameter_data_group_unset_data_raise(null_config, tmp_path, store):
+    s1 = hf.TaskSchema(
+        objective="t1",
+        inputs=[hf.SchemaInput(parameter=hf.Parameter("p1"))],
+        outputs=[hf.SchemaInput(parameter=hf.Parameter("p2"))],
+        actions=[
+            hf.Action(
+                commands=[
+                    hf.Command(
+                        command="Write-Output (<<parameter:p1>> + 100)",
+                        stdout="<<parameter:p2>>",
+                    )
+                ]
+            )
+        ],
+    )
+    s2 = hf.TaskSchema(
+        objective="t2",
+        inputs=[hf.SchemaInput(parameter=hf.Parameter("p2"), group="my_group")],
+    )
+    t1 = hf.Task(
+        schemas=s1,
+        sequences=[hf.ValueSequence("inputs.p1", values=[1, 2], nesting_order=0)],
+        groups=[hf.ElementGroup(name="my_group")],
+    )
+    t2 = hf.Task(schemas=s2)
+    wk = hf.Workflow.from_template_data(
+        tasks=[t1, t2],
+        template_name="w1",
+        overwrite=True,
+        path=tmp_path,
+        store=store,
+    )
+    data_idx_t1 = wk.tasks.t1.elements[0].get_data_idx()
+    data_idx_t2 = wk.tasks.t2.elements[0].get_data_idx()
+    with pytest.raises(UnsetParameterDataError):
+        wk.tasks.t1._get_merged_parameter_data(
+            data_index=data_idx_t1,
+            path="outputs.p2",
+            raise_on_unset=True,
+        )
+    with pytest.raises(UnsetParameterDataError):
+        wk.tasks.t2._get_merged_parameter_data(
+            data_index=data_idx_t2,
+            path="inputs.p2",
+            raise_on_unset=True,
+        )
+
+
+@pytest.mark.parametrize("store", ["json", "zarr"])
+def test_get_merged_parameter_data_group_unset_data_no_raise(
+    null_config, tmp_path, store
+):
+    s1 = hf.TaskSchema(
+        objective="t1",
+        inputs=[hf.SchemaInput(parameter=hf.Parameter("p1"))],
+        outputs=[hf.SchemaInput(parameter=hf.Parameter("p2"))],
+        actions=[
+            hf.Action(
+                commands=[
+                    hf.Command(
+                        command="Write-Output (<<parameter:p1>> + 100)",
+                        stdout="<<parameter:p2>>",
+                    )
+                ]
+            )
+        ],
+    )
+    s2 = hf.TaskSchema(
+        objective="t2",
+        inputs=[hf.SchemaInput(parameter=hf.Parameter("p2"), group="my_group")],
+    )
+    t1 = hf.Task(
+        schemas=s1,
+        sequences=[hf.ValueSequence("inputs.p1", values=[1, 2], nesting_order=0)],
+        groups=[hf.ElementGroup(name="my_group")],
+    )
+    t2 = hf.Task(schemas=s2)
+    wk = hf.Workflow.from_template_data(
+        tasks=[t1, t2],
+        template_name="w1",
+        overwrite=True,
+        path=tmp_path,
+        store=store,
+    )
+    data_idx_t1 = wk.tasks.t1.elements[0].get_data_idx()
+    data_idx_t2 = wk.tasks.t2.elements[0].get_data_idx()
+    assert None == wk.tasks.t1._get_merged_parameter_data(
+        data_index=data_idx_t1,
+        path="outputs.p2",
+        raise_on_unset=False,
+    )
+    assert [None, None] == wk.tasks.t2._get_merged_parameter_data(
+        data_index=data_idx_t2,
+        path="inputs.p2",
+        raise_on_unset=False,
+    )
+
+
+@pytest.mark.parametrize("store", ["json", "zarr"])
+def test_get_merged_parameter_data_group_missing_data_raise(null_config, tmp_path, store):
+    s1 = hf.TaskSchema(
+        objective="t1",
+        inputs=[hf.SchemaInput(parameter=hf.Parameter("p1"))],
+        outputs=[hf.SchemaInput(parameter=hf.Parameter("p2"))],
+        actions=[
+            hf.Action(
+                commands=[
+                    hf.Command(
+                        command="Write-Output (<<parameter:p1>> + 100)",
+                        stdout="<<parameter:p2>>",
+                    )
+                ]
+            )
+        ],
+    )
+    s2 = hf.TaskSchema(
+        objective="t2",
+        inputs=[hf.SchemaInput(parameter=hf.Parameter("p2"), group="my_group")],
+    )
+    t1 = hf.Task(
+        schemas=s1,
+        sequences=[hf.ValueSequence("inputs.p1", values=[1, 2], nesting_order=0)],
+        groups=[hf.ElementGroup(name="my_group")],
+    )
+    t2 = hf.Task(schemas=s2)
+    wk = hf.Workflow.from_template_data(
+        tasks=[t1, t2],
+        template_name="w1",
+        overwrite=True,
+        path=tmp_path,
+        store=store,
+    )
+    data_idx_t1 = wk.tasks.t1.elements[0].get_data_idx()
+    data_idx_t2 = wk.tasks.t2.elements[0].get_data_idx()
+    with pytest.raises(ValueError):
+        wk.tasks.t1._get_merged_parameter_data(
+            data_index=data_idx_t1,
+            path="outputs.p4",
+            raise_on_missing=True,
+        )
+    with pytest.raises(ValueError):
+        wk.tasks.t2._get_merged_parameter_data(
+            data_index=data_idx_t2,
+            path="inputs.p4",
+            raise_on_missing=True,
+        )
+
+
+@pytest.mark.parametrize("store", ["json", "zarr"])
+def test_get_merged_parameter_data_group_missing_data_no_raise(
+    null_config, tmp_path, store
+):
+    s1 = hf.TaskSchema(
+        objective="t1",
+        inputs=[hf.SchemaInput(parameter=hf.Parameter("p1"))],
+        outputs=[hf.SchemaInput(parameter=hf.Parameter("p2"))],
+        actions=[
+            hf.Action(
+                commands=[
+                    hf.Command(
+                        command="Write-Output (<<parameter:p1>> + 100)",
+                        stdout="<<parameter:p2>>",
+                    )
+                ]
+            )
+        ],
+    )
+    s2 = hf.TaskSchema(
+        objective="t2",
+        inputs=[hf.SchemaInput(parameter=hf.Parameter("p2"), group="my_group")],
+    )
+    t1 = hf.Task(
+        schemas=s1,
+        sequences=[hf.ValueSequence("inputs.p1", values=[1, 2], nesting_order=0)],
+        groups=[hf.ElementGroup(name="my_group")],
+    )
+    t2 = hf.Task(schemas=s2)
+    wk = hf.Workflow.from_template_data(
+        tasks=[t1, t2],
+        template_name="w1",
+        overwrite=True,
+        path=tmp_path,
+        store=store,
+    )
+    data_idx_t1 = wk.tasks.t1.elements[0].get_data_idx()
+    data_idx_t2 = wk.tasks.t2.elements[0].get_data_idx()
+    assert None == wk.tasks.t1._get_merged_parameter_data(
+        data_index=data_idx_t1,
+        path="outputs.p4",
+        raise_on_missing=False,
+    )
+    assert None == wk.tasks.t2._get_merged_parameter_data(
+        data_index=data_idx_t2,
+        path="inputs.p4",
+        raise_on_missing=False,
+    )
+
+
+@pytest.fixture
+def path_to_PV_classes_workflow(null_config, tmp_path):
+    s1 = hf.TaskSchema(
+        objective="t1",
+        inputs=[hf.SchemaInput(parameter=hf.Parameter("p1c"))],
+        actions=[
+            hf.Action(commands=[hf.Command("Write-Output (<<parameter:p1c>> + 100)")])
+        ],
+    )
+    p1_value = P1(a=10, sub_param=P1_sub_param(e=5))
+    t1 = hf.Task(schemas=s1, inputs=[hf.InputValue("p1c", value=p1_value)])
+    wk = hf.Workflow.from_template_data(
+        tasks=[t1],
+        template_name="w1",
+        overwrite=True,
+        path=tmp_path,
+    )
+    return wk
+
+
+def test_path_to_PV_classes(path_to_PV_classes_workflow):
+    assert path_to_PV_classes_workflow.tasks.t1._paths_to_PV_classes(["inputs.p1c"]) == {
+        "inputs.p1c": P1,
+    }
+
+
+def test_path_to_PV_classes_sub_data(path_to_PV_classes_workflow):
+    assert path_to_PV_classes_workflow.tasks.t1._paths_to_PV_classes(
+        ["inputs.p1c.a"]
+    ) == {
+        "inputs.p1c": P1,
+    }
+
+
+def test_path_to_PV_classes_sub_parameter(path_to_PV_classes_workflow):
+    assert path_to_PV_classes_workflow.tasks.t1._paths_to_PV_classes(
+        ["inputs.p1c.sub_param"]
+    ) == {
+        "inputs.p1c": P1,
+        "inputs.p1c.sub_param": P1_sub_param,
+    }
+
+
+def test_path_to_PV_classes_multiple_sub_parameters(path_to_PV_classes_workflow):
+    paths = ["inputs.p1c.sub_param", "inputs.p1c.sub_param_2"]
+    assert path_to_PV_classes_workflow.tasks.t1._paths_to_PV_classes(paths) == {
+        "inputs.p1c": P1,
+        "inputs.p1c.sub_param": P1_sub_param,
+        "inputs.p1c.sub_param_2": P1_sub_param_2,
+    }
+
+
+def test_path_to_PV_classes_multiple_sub_parameter_attr(path_to_PV_classes_workflow):
+    paths = ["inputs.p1c.sub_param.e"]
+    assert path_to_PV_classes_workflow.tasks.t1._paths_to_PV_classes(paths) == {
+        "inputs.p1c": P1,
+        "inputs.p1c.sub_param": P1_sub_param,
+    }
+
+
+def test_path_to_PV_classes_inputs_only_path_ignored(path_to_PV_classes_workflow):
+    paths_1 = ["inputs", "inputs.p1c"]
+    paths_2 = ["inputs.p1c"]
+    assert path_to_PV_classes_workflow.tasks.t1._paths_to_PV_classes(
+        paths_1
+    ) == path_to_PV_classes_workflow.tasks.t1._paths_to_PV_classes(paths_2)
+
+
+def test_path_to_PV_classes_resources_path_ignored(path_to_PV_classes_workflow):
+    paths_1 = ["resources", "inputs.p1c"]
+    paths_2 = ["inputs.p1c"]
+    assert path_to_PV_classes_workflow.tasks.t1._paths_to_PV_classes(
+        paths_1
+    ) == path_to_PV_classes_workflow.tasks.t1._paths_to_PV_classes(paths_2)
```

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/tests/unit/test_task_schema.py` & `hpcflow_new2-0.2.0a99/hpcflow/tests/unit/test_task_schema.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/tests/unit/test_utils.py` & `hpcflow_new2-0.2.0a99/hpcflow/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/tests/unit/test_value_sequence.py` & `hpcflow_new2-0.2.0a99/hpcflow/tests/unit/test_value_sequence.py`

 * *Files 4% similar despite different names*

```diff
@@ -118,18 +118,18 @@
     assert seq.input_type is None
     assert seq.input_path is None
     assert seq.resource_scope == "main"
 
 
 @pytest.mark.parametrize("store", ["json", "zarr"])
 def test_value_sequence_object_values_during_workflow_init(null_config, tmp_path, store):
-    p1 = hf.Parameter("p1")
+    p1 = hf.Parameter("p1c")
     s1 = hf.TaskSchema(objective="t1", inputs=[hf.SchemaInput(parameter=p1)])
     obj = P1(a=101)
-    seq = hf.ValueSequence(path="inputs.p1", values=[obj], nesting_order=0)
+    seq = hf.ValueSequence(path="inputs.p1c", values=[obj], nesting_order=0)
     values_exp = [P1(a=101, d=None)]
 
     t1 = hf.Task(
         schemas=[s1],
         sequences=[seq],
     )
     # before workflow initialisation:
@@ -151,18 +151,18 @@
     assert wk.tasks[0].template.element_sets[0].sequences[0].values == values_exp
 
 
 @pytest.mark.parametrize("store", ["json", "zarr"])
 def test_value_sequence_object_values_class_method_during_workflow_init(
     null_config, tmp_path, store
 ):
-    p1 = hf.Parameter("p1")
+    p1 = hf.Parameter("p1c")
     s1 = hf.TaskSchema(objective="t1", inputs=[hf.SchemaInput(parameter=p1)])
     obj = P1.from_data(b=50, c=51)
-    seq = hf.ValueSequence(path="inputs.p1", values=[obj], nesting_order=0)
+    seq = hf.ValueSequence(path="inputs.p1c", values=[obj], nesting_order=0)
     values_exp = [P1(a=101, d=None)]
 
     t1 = hf.Task(
         schemas=[s1],
         sequences=[seq],
     )
     # before workflow initialisation:
@@ -184,19 +184,19 @@
     assert wk.tasks[0].template.element_sets[0].sequences[0].values == values_exp
 
 
 @pytest.mark.parametrize("store", ["json", "zarr"])
 def test_value_sequence_object_values_named_class_method_during_workflow_init(
     null_config, tmp_path, store
 ):
-    p1 = hf.Parameter("p1")
+    p1 = hf.Parameter("p1c")
     s1 = hf.TaskSchema(objective="t1", inputs=[hf.SchemaInput(parameter=p1)])
     data = {"b": 50, "c": 51}
     seq = hf.ValueSequence(
-        path="inputs.p1", values=[data], nesting_order=0, value_class_method="from_data"
+        path="inputs.p1c", values=[data], nesting_order=0, value_class_method="from_data"
     )
     values_exp = [data]
 
     t1 = hf.Task(
         schemas=[s1],
         sequences=[seq],
     )
```

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/tests/unit/test_workflow.py` & `hpcflow_new2-0.2.0a99/hpcflow/tests/unit/test_workflow.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,14 +45,19 @@
 
 @pytest.fixture
 def param_p1(null_config):
     return hf.Parameter("p1")
 
 
 @pytest.fixture
+def param_p1c(null_config):
+    return hf.Parameter("p1c")
+
+
+@pytest.fixture
 def param_p2():
     return hf.Parameter("p2")
 
 
 @pytest.fixture
 def param_p3(null_config):
     return hf.Parameter("p3")
@@ -131,14 +136,31 @@
                 commands=[hf.Command("Write-Output '<<parameter:p1>>'")],
             )
         ],
     )
 
 
 @pytest.fixture
+def schema_s4c(
+    null_config,
+    param_p1c,
+):
+    return hf.TaskSchema(
+        objective="t1",
+        inputs=[hf.SchemaInput(parameter=param_p1c)],
+        actions=[
+            hf.Action(
+                environments=[hf.ActionEnvironment(environment=hf.envs.null_env)],
+                commands=[hf.Command("Write-Output '<<parameter:p1c>>'")],
+            )
+        ],
+    )
+
+
+@pytest.fixture
 def workflow_w1(null_config, tmp_path, schema_s3, param_p1):
     t1 = hf.Task(schemas=schema_s3, inputs=[hf.InputValue(param_p1, 101)])
     wkt = hf.WorkflowTemplate(name="w1", tasks=[t1])
     return hf.Workflow.from_template(wkt, path=tmp_path)
 
 
 def test_make_empty_workflow(null_config, empty_workflow):
@@ -320,90 +342,90 @@
 
 
 @pytest.mark.parametrize("store", ["json", "zarr"])
 def test_equivalent_element_input_parameter_value_class_and_kwargs(
     null_config,
     tmp_path,
     store,
-    schema_s4,
-    param_p1,
+    schema_s4c,
+    param_p1c,
 ):
     a_value = 101
     t1_1 = hf.Task(
-        schemas=[schema_s4],
-        inputs=[hf.InputValue(parameter=param_p1, value=P1(a=a_value))],
+        schemas=[schema_s4c],
+        inputs=[hf.InputValue(parameter=param_p1c, value=P1(a=a_value))],
     )
     t1_2 = hf.Task(
-        schemas=[schema_s4],
-        inputs=[hf.InputValue(parameter=param_p1, value={"a": a_value})],
+        schemas=[schema_s4c],
+        inputs=[hf.InputValue(parameter=param_p1c, value={"a": a_value})],
     )
     wk = hf.Workflow.from_template_data(
         tasks=[t1_1, t1_2],
         path=tmp_path,
         template_name="temp",
         store=store,
     )
     assert (
-        wk.tasks.t1_1.elements[0].inputs.p1.value
-        == wk.tasks.t1_2.elements[0].inputs.p1.value
+        wk.tasks.t1_1.elements[0].inputs.p1c.value
+        == wk.tasks.t1_2.elements[0].inputs.p1c.value
     )
 
 
 @pytest.mark.parametrize("store", ["json", "zarr"])
 def test_equivalent_element_input_parameter_value_class_method_and_kwargs(
     null_config,
     tmp_path,
     store,
-    schema_s4,
-    param_p1,
+    schema_s4c,
+    param_p1c,
 ):
     b_val = 50
     c_val = 51
     expected_a_val = b_val + c_val
     t1_1 = hf.Task(
-        schemas=[schema_s4],
-        inputs=[hf.InputValue(parameter=param_p1, value=P1.from_data(b=b_val, c=c_val))],
+        schemas=[schema_s4c],
+        inputs=[hf.InputValue(parameter=param_p1c, value=P1.from_data(b=b_val, c=c_val))],
     )
     t1_2 = hf.Task(
-        schemas=[schema_s4],
+        schemas=[schema_s4c],
         inputs=[
             hf.InputValue(
-                parameter=param_p1,
+                parameter=param_p1c,
                 value={"b": b_val, "c": c_val},
                 value_class_method="from_data",
             )
         ],
     )
     wk = hf.Workflow.from_template_data(
         tasks=[t1_1, t1_2],
         path=tmp_path,
         template_name="temp",
         store=store,
     )
-    assert wk.tasks.t1_1.elements[0].inputs.p1.value.a == expected_a_val
+    assert wk.tasks.t1_1.elements[0].inputs.p1c.value.a == expected_a_val
     assert (
-        wk.tasks.t1_1.elements[0].inputs.p1.value
-        == wk.tasks.t1_2.elements[0].inputs.p1.value
+        wk.tasks.t1_1.elements[0].inputs.p1c.value
+        == wk.tasks.t1_2.elements[0].inputs.p1c.value
     )
 
 
 @pytest.mark.parametrize("store", ["json", "zarr"])
 def test_input_value_class_expected_value(
-    null_config, tmp_path, store, schema_s4, param_p1
+    null_config, tmp_path, store, schema_s4c, param_p1c
 ):
     a_value = 101
     t1_value_exp = P1(a=a_value)
     t2_value_exp = {"a": a_value}
     t1_1 = hf.Task(
-        schemas=[schema_s4],
-        inputs=[hf.InputValue(parameter=param_p1, value=t1_value_exp)],
+        schemas=[schema_s4c],
+        inputs=[hf.InputValue(parameter=param_p1c, value=t1_value_exp)],
     )
     t1_2 = hf.Task(
-        schemas=[schema_s4],
-        inputs=[hf.InputValue(parameter=param_p1, value=t2_value_exp)],
+        schemas=[schema_s4c],
+        inputs=[hf.InputValue(parameter=param_p1c, value=t2_value_exp)],
     )
     wk = hf.Workflow.from_template_data(
         tasks=[t1_1, t1_2],
         path=tmp_path,
         template_name="temp",
         store=store,
     )
@@ -411,29 +433,29 @@
     value_2 = wk.tasks.t1_2.template.element_sets[0].inputs[0].value
     assert value_1 == t1_value_exp
     assert value_2 == t2_value_exp
 
 
 @pytest.mark.parametrize("store", ["json", "zarr"])
 def test_input_value_class_method_expected_value(
-    null_config, tmp_path, store, schema_s4, param_p1
+    null_config, tmp_path, store, schema_s4c, param_p1c
 ):
     b_val = 50
     c_val = 51
     t1_value_exp = P1.from_data(b=b_val, c=c_val)
     t2_value_exp = {"b": b_val, "c": c_val}
     t1_1 = hf.Task(
-        schemas=[schema_s4],
-        inputs=[hf.InputValue(parameter=param_p1, value=t1_value_exp)],
+        schemas=[schema_s4c],
+        inputs=[hf.InputValue(parameter=param_p1c, value=t1_value_exp)],
     )
     t1_2 = hf.Task(
-        schemas=[schema_s4],
+        schemas=[schema_s4c],
         inputs=[
             hf.InputValue(
-                parameter=param_p1,
+                parameter=param_p1c,
                 value=t2_value_exp,
                 value_class_method="from_data",
             )
         ],
     )
     wk = hf.Workflow.from_template_data(
         tasks=[t1_1, t1_2],
@@ -445,80 +467,80 @@
     value_2 = wk.tasks.t1_2.template.element_sets[0].inputs[0].value
     assert value_1 == t1_value_exp
     assert value_2 == t2_value_exp
 
 
 @pytest.mark.parametrize("store", ["json", "zarr"])
 def test_equivalent_element_input_sequence_parameter_value_class_and_kwargs(
-    null_config, tmp_path, store, schema_s4
+    null_config, tmp_path, store, schema_s4c
 ):
     data = {"a": 101}
     obj = P1(**data)
     t1_1 = hf.Task(
-        schemas=[schema_s4],
-        sequences=[hf.ValueSequence(path="inputs.p1", values=[obj], nesting_order=0)],
+        schemas=[schema_s4c],
+        sequences=[hf.ValueSequence(path="inputs.p1c", values=[obj], nesting_order=0)],
     )
     t1_2 = hf.Task(
-        schemas=[schema_s4],
-        sequences=[hf.ValueSequence(path="inputs.p1", values=[data], nesting_order=0)],
+        schemas=[schema_s4c],
+        sequences=[hf.ValueSequence(path="inputs.p1c", values=[data], nesting_order=0)],
     )
     wk = hf.Workflow.from_template_data(
         tasks=[t1_1, t1_2],
         path=tmp_path,
         template_name="temp",
         store=store,
     )
-    val_1 = wk.tasks.t1_1.elements[0].inputs.p1.value
-    val_2 = wk.tasks.t1_2.elements[0].inputs.p1.value
+    val_1 = wk.tasks.t1_1.elements[0].inputs.p1c.value
+    val_2 = wk.tasks.t1_2.elements[0].inputs.p1c.value
     assert val_1 == val_2 == obj
 
 
 @pytest.mark.parametrize("store", ["json", "zarr"])
 def test_equivalent_element_input_sequence_parameter_value_class_method_and_kwargs(
-    null_config, tmp_path, store, schema_s4
+    null_config, tmp_path, store, schema_s4c
 ):
     data = {"b": 50, "c": 51}
     obj = P1.from_data(**data)
     t1_1 = hf.Task(
-        schemas=[schema_s4],
-        sequences=[hf.ValueSequence(path="inputs.p1", values=[obj], nesting_order=0)],
+        schemas=[schema_s4c],
+        sequences=[hf.ValueSequence(path="inputs.p1c", values=[obj], nesting_order=0)],
     )
     t1_2 = hf.Task(
-        schemas=[schema_s4],
+        schemas=[schema_s4c],
         sequences=[
             hf.ValueSequence(
-                path="inputs.p1",
+                path="inputs.p1c",
                 values=[data],
                 value_class_method="from_data",
                 nesting_order=0,
             )
         ],
     )
     wk = hf.Workflow.from_template_data(
         tasks=[t1_1, t1_2],
         path=tmp_path,
         template_name="temp",
         store=store,
     )
-    val_1 = wk.tasks.t1_1.elements[0].inputs.p1.value
-    val_2 = wk.tasks.t1_2.elements[0].inputs.p1.value
+    val_1 = wk.tasks.t1_1.elements[0].inputs.p1c.value
+    val_2 = wk.tasks.t1_2.elements[0].inputs.p1c.value
     assert val_1 == val_2 == obj
 
 
 @pytest.mark.parametrize("store", ["json", "zarr"])
-def test_sequence_value_class_expected_value(null_config, tmp_path, store, schema_s4):
+def test_sequence_value_class_expected_value(null_config, tmp_path, store, schema_s4c):
     data = {"a": 101}
     obj = P1(**data)
     t1_1 = hf.Task(
-        schemas=[schema_s4],
-        sequences=[hf.ValueSequence(path="inputs.p1", values=[obj], nesting_order=0)],
+        schemas=[schema_s4c],
+        sequences=[hf.ValueSequence(path="inputs.p1c", values=[obj], nesting_order=0)],
     )
     t1_2 = hf.Task(
-        schemas=[schema_s4],
-        sequences=[hf.ValueSequence(path="inputs.p1", values=[data], nesting_order=0)],
+        schemas=[schema_s4c],
+        sequences=[hf.ValueSequence(path="inputs.p1c", values=[data], nesting_order=0)],
     )
     wk = hf.Workflow.from_template_data(
         tasks=[t1_1, t1_2],
         path=tmp_path,
         template_name="temp",
         store=store,
     )
@@ -526,27 +548,27 @@
     value_2 = wk.tasks.t1_2.template.element_sets[0].sequences[0].values[0]
     assert value_1 == obj
     assert value_2 == data
 
 
 @pytest.mark.parametrize("store", ["json", "zarr"])
 def test_sequence_value_class_method_expected_value(
-    null_config, tmp_path, store, schema_s4
+    null_config, tmp_path, store, schema_s4c
 ):
     data = {"b": 50, "c": 51}
     obj = P1.from_data(**data)
     t1_1 = hf.Task(
-        schemas=[schema_s4],
-        sequences=[hf.ValueSequence(path="inputs.p1", values=[obj], nesting_order=0)],
+        schemas=[schema_s4c],
+        sequences=[hf.ValueSequence(path="inputs.p1c", values=[obj], nesting_order=0)],
     )
     t1_2 = hf.Task(
-        schemas=[schema_s4],
+        schemas=[schema_s4c],
         sequences=[
             hf.ValueSequence(
-                path="inputs.p1",
+                path="inputs.p1c",
                 values=[data],
                 nesting_order=0,
                 value_class_method="from_data",
             ),
         ],
     )
     wk = hf.Workflow.from_template_data(
@@ -559,60 +581,64 @@
     value_2 = wk.tasks.t1_2.template.element_sets[0].sequences[0].values[0]
     assert value_1 == obj
     assert value_2 == data
 
 
 @pytest.mark.parametrize("store", ["json", "zarr"])
 def test_expected_element_input_parameter_value_class_merge_sequence(
-    null_config, tmp_path, store, schema_s4, param_p1
+    null_config, tmp_path, store, schema_s4c, param_p1c
 ):
     a_val = 101
     d_val = 201
     obj_exp = P1(a=a_val, d=d_val)
 
     t1 = hf.Task(
-        schemas=[schema_s4],
-        inputs=[hf.InputValue(parameter=param_p1, value={"a": a_val})],
-        sequences=[hf.ValueSequence(path="inputs.p1.d", values=[d_val], nesting_order=0)],
+        schemas=[schema_s4c],
+        inputs=[hf.InputValue(parameter=param_p1c, value={"a": a_val})],
+        sequences=[
+            hf.ValueSequence(path="inputs.p1c.d", values=[d_val], nesting_order=0)
+        ],
     )
     wk = hf.Workflow.from_template_data(
         tasks=[t1],
         path=tmp_path,
         template_name="temp",
         store=store,
     )
     wk.tasks.t1.template.element_sets[0].sequences[0].values[0]
-    assert wk.tasks.t1.elements[0].inputs.p1.value == obj_exp
+    assert wk.tasks.t1.elements[0].inputs.p1c.value == obj_exp
 
 
 @pytest.mark.parametrize("store", ["json", "zarr"])
 def test_expected_element_input_parameter_value_class_method_merge_sequence(
-    null_config, tmp_path, store, schema_s4, param_p1
+    null_config, tmp_path, store, schema_s4c, param_p1c
 ):
     b_val = 50
     c_val = 51
     obj_exp = P1.from_data(b=b_val, c=c_val)
 
     t1 = hf.Task(
-        schemas=[schema_s4],
+        schemas=[schema_s4c],
         inputs=[
             hf.InputValue(
-                parameter=param_p1, value={"b": b_val}, value_class_method="from_data"
+                parameter=param_p1c, value={"b": b_val}, value_class_method="from_data"
             )
         ],
-        sequences=[hf.ValueSequence(path="inputs.p1.c", values=[c_val], nesting_order=0)],
+        sequences=[
+            hf.ValueSequence(path="inputs.p1c.c", values=[c_val], nesting_order=0)
+        ],
     )
     wk = hf.Workflow.from_template_data(
         tasks=[t1],
         path=tmp_path,
         template_name="temp",
         store=store,
     )
     wk.tasks.t1.template.element_sets[0].sequences[0].values[0]
-    assert wk.tasks.t1.elements[0].inputs.p1.value == obj_exp
+    assert wk.tasks.t1.elements[0].inputs.p1c.value == obj_exp
 
 
 @pytest.mark.parametrize("store", ["json", "zarr"])
 def test_upstream_input_source_merge_with_current_input_modification(
     null_config, tmp_path, store
 ):
     s1 = hf.TaskSchema(
```

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/tests/unit/test_workflow_template.py` & `hpcflow_new2-0.2.0a99/hpcflow/tests/unit/test_workflow_template.py`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a98/hpcflow/viz_demo.ipynb` & `hpcflow_new2-0.2.0a99/hpcflow/viz_demo.ipynb`

 * *Files identical despite different names*

### Comparing `hpcflow_new2-0.2.0a98/pyproject.toml` & `hpcflow_new2-0.2.0a99/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [tool.poetry]
 name = "hpcflow-new2"
-version = "0.2.0a98"
+version = "0.2.0a99"
 
 description = "Computational workflow management"
 authors = ["aplowman <adam.plowman@manchester.ac.uk>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "hpcflow" }
@@ -64,15 +64,15 @@
 hpcflow = 'hpcflow.cli:cli'
 
 [tool.poetry.plugins.pyinstaller40]
 hook-dirs = "hpcflow.__pyinstaller:get_hook_dirs"
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.2.0a98"
+version = "0.2.0a99"
 tag_format = "v$version"
 version_files = [ 
     "pyproject.toml:version",
     "hpcflow/_version.py"
 ]
 bump_message = "bump: $current_version → $new_version [skip ci]"
```

### Comparing `hpcflow_new2-0.2.0a98/PKG-INFO` & `hpcflow_new2-0.2.0a99/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hpcflow-new2
-Version: 0.2.0a98
+Version: 0.2.0a99
 Summary: Computational workflow management
 License: MIT
 Author: aplowman
 Author-email: adam.plowman@manchester.ac.uk
 Requires-Python: >=3.8,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

