# Comparing `tmp/oper8-0.1.8.tar.gz` & `tmp/oper8-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oper8-0.1.8.tar", last modified: Fri Jan 19 23:03:35 2024, max compression
+gzip compressed data, was "oper8-0.1.9.tar", last modified: Mon Jan 22 18:48:03 2024, max compression
```

## Comparing `oper8-0.1.8.tar` & `oper8-0.1.9.tar`

### file list

```diff
@@ -1,269 +1,269 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 23:03:35.732509 oper8-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-01-19 23:03:22.000000 oper8-0.1.8/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 23:03:35.692508 oper8-0.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 23:03:35.696508 oper8-0.1.8/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-01-19 23:03:22.000000 oper8-0.1.8/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-01-19 23:03:22.000000 oper8-0.1.8/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-01-19 23:03:22.000000 oper8-0.1.8/.github/ISSUE_TEMPLATE/user_story.md
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-01-19 23:03:22.000000 oper8-0.1.8/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-01-19 23:03:22.000000 oper8-0.1.8/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 23:03:35.696508 oper8-0.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-01-19 23:03:22.000000 oper8-0.1.8/.github/workflows/build-library.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-01-19 23:03:22.000000 oper8-0.1.8/.github/workflows/lint-code.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-01-19 23:03:22.000000 oper8-0.1.8/.github/workflows/publish-library.yml
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-01-19 23:03:22.000000 oper8-0.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-01-19 23:03:22.000000 oper8-0.1.8/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-01-19 23:03:22.000000 oper8-0.1.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-01-19 23:03:22.000000 oper8-0.1.8/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-01-19 23:03:22.000000 oper8-0.1.8/.prettierrc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-01-19 23:03:22.000000 oper8-0.1.8/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-01-19 23:03:22.000000 oper8-0.1.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     7403 2024-01-19 23:03:22.000000 oper8-0.1.8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-01-19 23:03:22.000000 oper8-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-01-19 23:03:35.732509 oper8-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-01-19 23:03:22.000000 oper8-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-01-19 23:03:22.000000 oper8-0.1.8/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 23:03:35.700508 oper8-0.1.8/oper8/
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-01-19 23:03:35.000000 oper8-0.1.8/oper8/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 23:03:35.700508 oper8-0.1.8/oper8/cmd/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/cmd/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6727 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/cmd/run_operator_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/cmd/setup_vcs_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    19404 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/component.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 23:03:35.700508 oper8-0.1.8/oper8/config/
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/config/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/config/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/config/config_validation.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    12803 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/config/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    13661 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 23:03:35.704508 oper8-0.1.8/oper8/dag/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/dag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4280 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/dag/completion_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/dag/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/dag/node.py
--rw-r--r--   0 runner    (1001) docker     (127)    12316 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/dag/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 23:03:35.704508 oper8-0.1.8/oper8/deploy_manager/
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/deploy_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6199 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/deploy_manager/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    23661 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/deploy_manager/dry_run_deploy_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/deploy_manager/kube_event.py
--rw-r--r--   0 runner    (1001) docker     (127)    34298 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/deploy_manager/openshift_deploy_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/deploy_manager/owner_references.py
--rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/log_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/managed_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     6918 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/patch_strategic_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)    44049 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/reconcile.py
--rw-r--r--   0 runner    (1001) docker     (127)    16893 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/rollout_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    18365 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     9645 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/setup_vcs.py
--rw-r--r--   0 runner    (1001) docker     (127)    19019 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/status.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 23:03:35.704508 oper8-0.1.8/oper8/temporary_patch/
--rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/temporary_patch/temporary_patch_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     5187 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/temporary_patch/temporary_patch_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 23:03:35.704508 oper8-0.1.8/oper8/test_helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/test_helpers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 23:03:35.708509 oper8-0.1.8/oper8/test_helpers/data/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/test_helpers/data/controller.template
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/test_helpers/data/test_ca.crt
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/test_helpers/data/test_ca.key
--rw-r--r--   0 runner    (1001) docker     (127)    25106 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/test_helpers/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    34967 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/test_helpers/kub_mock.py
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/test_helpers/oper8x_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5865 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/test_helpers/pwm_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    10537 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14314 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/vcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9105 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/verify_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 23:03:35.708509 oper8-0.1.8/oper8/watch_manager/
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/watch_manager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 23:03:35.708509 oper8-0.1.8/oper8/watch_manager/ansible_watch_manager/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/watch_manager/ansible_watch_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13957 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/watch_manager/ansible_watch_manager/ansible_watch_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 23:03:35.708509 oper8-0.1.8/oper8/watch_manager/ansible_watch_manager/modules/
--rw-r--r--   0 runner    (1001) docker     (127)    11913 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/watch_manager/ansible_watch_manager/modules/k8s_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/watch_manager/ansible_watch_manager/modules/log_rotator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 23:03:35.708509 oper8-0.1.8/oper8/watch_manager/ansible_watch_manager/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/watch_manager/ansible_watch_manager/resources/playbook-base.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 23:03:35.688508 oper8-0.1.8/oper8/watch_manager/ansible_watch_manager/resources/roles/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 23:03:35.688508 oper8-0.1.8/oper8/watch_manager/ansible_watch_manager/resources/roles/oper8_app/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 23:03:35.708509 oper8-0.1.8/oper8/watch_manager/ansible_watch_manager/resources/roles/oper8_app/defaults/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/watch_manager/ansible_watch_manager/resources/roles/oper8_app/defaults/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 23:03:35.708509 oper8-0.1.8/oper8/watch_manager/ansible_watch_manager/resources/roles/oper8_app/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/watch_manager/ansible_watch_manager/resources/roles/oper8_app/tasks/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/watch_manager/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4355 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/watch_manager/dry_run_watch_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 23:03:35.708509 oper8-0.1.8/oper8/watch_manager/python_watch_manager/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/watch_manager/python_watch_manager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 23:03:35.708509 oper8-0.1.8/oper8/watch_manager/python_watch_manager/filters/
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/watch_manager/python_watch_manager/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/watch_manager/python_watch_manager/filters/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    13038 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/watch_manager/python_watch_manager/filters/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     9557 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/watch_manager/python_watch_manager/filters/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 23:03:35.712509 oper8-0.1.8/oper8/watch_manager/python_watch_manager/leader_election/
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/watch_manager/python_watch_manager/leader_election/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5883 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/watch_manager/python_watch_manager/leader_election/annotation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8349 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/watch_manager/python_watch_manager/leader_election/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/watch_manager/python_watch_manager/leader_election/dry_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     5041 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/watch_manager/python_watch_manager/leader_election/lease.py
--rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/watch_manager/python_watch_manager/leader_election/life.py
--rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/watch_manager/python_watch_manager/python_watch_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    13668 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/watch_manager/python_watch_manager/reconcile_process_entrypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 23:03:35.712509 oper8-0.1.8/oper8/watch_manager/python_watch_manager/threads/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/watch_manager/python_watch_manager/threads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/watch_manager/python_watch_manager/threads/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    21578 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/watch_manager/python_watch_manager/threads/reconcile.py
--rw-r--r--   0 runner    (1001) docker     (127)     5908 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/watch_manager/python_watch_manager/threads/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)    18357 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/watch_manager/python_watch_manager/threads/watch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 23:03:35.712509 oper8-0.1.8/oper8/watch_manager/python_watch_manager/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/watch_manager/python_watch_manager/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/watch_manager/python_watch_manager/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/watch_manager/python_watch_manager/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/watch_manager/python_watch_manager/utils/log_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8503 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/watch_manager/python_watch_manager/utils/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 23:03:35.712509 oper8-0.1.8/oper8/x/
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/x/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 23:03:35.712509 oper8-0.1.8/oper8/x/datastores/
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/x/datastores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/x/datastores/connection_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 23:03:35.712509 oper8-0.1.8/oper8/x/datastores/cos/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/x/datastores/cos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10931 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/x/datastores/cos/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/x/datastores/cos/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     5169 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/x/datastores/cos/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)    12709 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/x/datastores/factory_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/x/datastores/interfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 23:03:35.716508 oper8-0.1.8/oper8/x/datastores/postgres/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/x/datastores/postgres/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11174 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/x/datastores/postgres/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/x/datastores/postgres/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/x/datastores/postgres/interfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 23:03:35.716508 oper8-0.1.8/oper8/x/datastores/redis/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/x/datastores/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10509 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/x/datastores/redis/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/x/datastores/redis/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4852 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/x/datastores/redis/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     4889 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/x/oper8x_component.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 23:03:35.716508 oper8-0.1.8/oper8/x/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/x/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/x/utils/abc_static.py
--rw-r--r--   0 runner    (1001) docker     (127)    11562 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/x/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/x/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    11395 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/x/utils/deps_annotation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8113 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/x/utils/tls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 23:03:35.716508 oper8-0.1.8/oper8/x/utils/tls_context/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/x/utils/tls_context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4613 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/x/utils/tls_context/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     5799 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/x/utils/tls_context/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    11858 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/x/utils/tls_context/internal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-01-19 23:03:22.000000 oper8-0.1.8/oper8/x/utils/tls_context/public.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 23:03:35.732509 oper8-0.1.8/oper8.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-01-19 23:03:35.000000 oper8-0.1.8/oper8.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8035 2024-01-19 23:03:35.000000 oper8-0.1.8/oper8.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-19 23:03:35.000000 oper8-0.1.8/oper8.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-01-19 23:03:35.000000 oper8-0.1.8/oper8.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-01-19 23:03:35.000000 oper8-0.1.8/oper8.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-01-19 23:03:35.000000 oper8-0.1.8/oper8.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-01-19 23:03:22.000000 oper8-0.1.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 23:03:35.716508 oper8-0.1.8/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)      720 2024-01-19 23:03:22.000000 oper8-0.1.8/scripts/fmt.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      351 2024-01-19 23:03:22.000000 oper8-0.1.8/scripts/lint.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      815 2024-01-19 23:03:22.000000 oper8-0.1.8/scripts/run_tests.sh
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-19 23:03:35.732509 oper8-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-19 23:03:22.000000 oper8-0.1.8/setup_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 23:03:35.720509 oper8-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 23:03:35.720509 oper8-0.1.8/tests/dag/
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/dag/test_completion_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/dag/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/dag/test_node.py
--rw-r--r--   0 runner    (1001) docker     (127)    18443 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/dag/test_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 23:03:35.724509 oper8-0.1.8/tests/deploy_manager/
--rw-r--r--   0 runner    (1001) docker     (127)    18875 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/deploy_manager/test_dry_run_deploy_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    46318 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/deploy_manager/test_openshift_deploy_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5673 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/deploy_manager/test_owner_references.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 23:03:35.724509 oper8-0.1.8/tests/temporary_patch/
--rw-r--r--   0 runner    (1001) docker     (127)    20903 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/temporary_patch/test_temporary_patch_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     8405 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/temporary_patch/test_temporary_patch_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    22181 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/test_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     8741 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    17137 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/test_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3712 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    12303 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)    12019 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/test_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     7786 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/test_patch_strategic_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)    46411 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/test_reconcile.py
--rw-r--r--   0 runner    (1001) docker     (127)    18877 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/test_rollout_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    12579 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     7847 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/test_setup_vcs.py
--rw-r--r--   0 runner    (1001) docker     (127)    19667 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/test_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     9608 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8078 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/test_vcs.py
--rw-r--r--   0 runner    (1001) docker     (127)    13496 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/test_verify_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 23:03:35.724509 oper8-0.1.8/tests/watch_manager/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/watch_manager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 23:03:35.724509 oper8-0.1.8/tests/watch_manager/ansible_watch_manager/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 23:03:35.724509 oper8-0.1.8/tests/watch_manager/ansible_watch_manager/modules/
--rw-r--r--   0 runner    (1001) docker     (127)    13847 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/watch_manager/ansible_watch_manager/modules/test_k8s_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/watch_manager/ansible_watch_manager/modules/test_log_rotator.py
--rw-r--r--   0 runner    (1001) docker     (127)    17630 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/watch_manager/ansible_watch_manager/test_ansible_watch_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 23:03:35.724509 oper8-0.1.8/tests/watch_manager/python_watch_manager/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 23:03:35.724509 oper8-0.1.8/tests/watch_manager/python_watch_manager/filters/
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/watch_manager/python_watch_manager/filters/test_common_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5965 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/watch_manager/python_watch_manager/filters/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/watch_manager/python_watch_manager/filters/test_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 23:03:35.724509 oper8-0.1.8/tests/watch_manager/python_watch_manager/leader_election/
--rw-r--r--   0 runner    (1001) docker     (127)     8447 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/watch_manager/python_watch_manager/leader_election/test_annotation.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/watch_manager/python_watch_manager/leader_election/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     7215 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/watch_manager/python_watch_manager/leader_election/test_lease.py
--rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/watch_manager/python_watch_manager/leader_election/test_life.py
--rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/watch_manager/python_watch_manager/test_python_watch_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     9620 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/watch_manager/python_watch_manager/test_reconcile_process_entrypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 23:03:35.728509 oper8-0.1.8/tests/watch_manager/python_watch_manager/threads/
--rw-r--r--   0 runner    (1001) docker     (127)     8538 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/watch_manager/python_watch_manager/threads/test_reconcile_thread.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/watch_manager/python_watch_manager/threads/test_timer_thread.py
--rw-r--r--   0 runner    (1001) docker     (127)    12897 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/watch_manager/python_watch_manager/threads/test_watch_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 23:03:35.728509 oper8-0.1.8/tests/watch_manager/python_watch_manager/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/watch_manager/python_watch_manager/utils/test_pwm_util_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     5222 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/watch_manager/test_dry_run_watch_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/watch_manager/test_watch_manager_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 23:03:35.692508 oper8-0.1.8/tests/x/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 23:03:35.728509 oper8-0.1.8/tests/x/datastores/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/x/datastores/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 23:03:35.728509 oper8-0.1.8/tests/x/datastores/cos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/x/datastores/cos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17948 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/x/datastores/cos/test_cos_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 23:03:35.728509 oper8-0.1.8/tests/x/datastores/postgres/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/x/datastores/postgres/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/x/datastores/postgres/test_pg_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    18168 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/x/datastores/postgres/test_postgres_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/x/datastores/postgres/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 23:03:35.728509 oper8-0.1.8/tests/x/datastores/redis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/x/datastores/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10592 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/x/datastores/redis/test_redis_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/x/datastores/redis/test_redis_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/x/datastores/redis/test_redis_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)    17114 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/x/datastores/test_factory_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 23:03:35.728509 oper8-0.1.8/tests/x/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/x/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/x/utils/test_abc_static.py
--rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/x/utils/test_common.py
--rw-r--r--   0 runner    (1001) docker     (127)    17656 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/x/utils/test_deps_annotation.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/x/utils/test_tls.py
--rw-r--r--   0 runner    (1001) docker     (127)    15261 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/x/utils/test_tls_context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 23:03:35.728509 oper8-0.1.8/tests/x/utils/tls_context/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 23:03:35.732509 oper8-0.1.8/tests/x/utils/tls_context/snapshots/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/x/utils/tls_context/snapshots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/x/utils/tls_context/test_internal.py
--rw-r--r--   0 runner    (1001) docker     (127)    11303 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/x/utils/tls_context/test_tls_preconditions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-01-19 23:03:22.000000 oper8-0.1.8/tests/x/utils/tls_context/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-01-19 23:03:22.000000 oper8-0.1.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 18:48:03.717494 oper8-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-01-22 18:47:50.000000 oper8-0.1.9/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 18:48:03.677494 oper8-0.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 18:48:03.677494 oper8-0.1.9/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-01-22 18:47:50.000000 oper8-0.1.9/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-01-22 18:47:50.000000 oper8-0.1.9/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-01-22 18:47:50.000000 oper8-0.1.9/.github/ISSUE_TEMPLATE/user_story.md
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-01-22 18:47:50.000000 oper8-0.1.9/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-01-22 18:47:50.000000 oper8-0.1.9/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 18:48:03.677494 oper8-0.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-01-22 18:47:50.000000 oper8-0.1.9/.github/workflows/build-library.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-01-22 18:47:50.000000 oper8-0.1.9/.github/workflows/lint-code.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-01-22 18:47:50.000000 oper8-0.1.9/.github/workflows/publish-library.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-01-22 18:47:50.000000 oper8-0.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-01-22 18:47:50.000000 oper8-0.1.9/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-01-22 18:47:50.000000 oper8-0.1.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-01-22 18:47:50.000000 oper8-0.1.9/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-01-22 18:47:50.000000 oper8-0.1.9/.prettierrc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-01-22 18:47:50.000000 oper8-0.1.9/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-01-22 18:47:50.000000 oper8-0.1.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7403 2024-01-22 18:47:50.000000 oper8-0.1.9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-01-22 18:47:50.000000 oper8-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-01-22 18:48:03.717494 oper8-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-01-22 18:47:50.000000 oper8-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-01-22 18:47:50.000000 oper8-0.1.9/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 18:48:03.681494 oper8-0.1.9/oper8/
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-01-22 18:48:03.000000 oper8-0.1.9/oper8/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 18:48:03.685494 oper8-0.1.9/oper8/cmd/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/cmd/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6727 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/cmd/run_operator_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/cmd/setup_vcs_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19404 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/component.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 18:48:03.685494 oper8-0.1.9/oper8/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/config/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/config/config_validation.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    12803 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/config/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13661 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 18:48:03.685494 oper8-0.1.9/oper8/dag/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/dag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4280 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/dag/completion_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/dag/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/dag/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12316 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/dag/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 18:48:03.689494 oper8-0.1.9/oper8/deploy_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/deploy_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6199 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/deploy_manager/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23661 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/deploy_manager/dry_run_deploy_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/deploy_manager/kube_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34298 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/deploy_manager/openshift_deploy_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/deploy_manager/owner_references.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/log_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/managed_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6918 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/patch_strategic_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44079 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/reconcile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16893 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/rollout_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18365 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9645 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/setup_vcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19019 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 18:48:03.689494 oper8-0.1.9/oper8/temporary_patch/
+-rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/temporary_patch/temporary_patch_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5187 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/temporary_patch/temporary_patch_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 18:48:03.689494 oper8-0.1.9/oper8/test_helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/test_helpers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 18:48:03.689494 oper8-0.1.9/oper8/test_helpers/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/test_helpers/data/controller.template
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/test_helpers/data/test_ca.crt
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/test_helpers/data/test_ca.key
+-rw-r--r--   0 runner    (1001) docker     (127)    25106 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/test_helpers/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34967 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/test_helpers/kub_mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/test_helpers/oper8x_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5865 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/test_helpers/pwm_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10537 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14314 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/vcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9105 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/verify_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 18:48:03.689494 oper8-0.1.9/oper8/watch_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/watch_manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 18:48:03.689494 oper8-0.1.9/oper8/watch_manager/ansible_watch_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/watch_manager/ansible_watch_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13957 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/watch_manager/ansible_watch_manager/ansible_watch_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 18:48:03.689494 oper8-0.1.9/oper8/watch_manager/ansible_watch_manager/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)    11913 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/watch_manager/ansible_watch_manager/modules/k8s_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/watch_manager/ansible_watch_manager/modules/log_rotator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 18:48:03.693494 oper8-0.1.9/oper8/watch_manager/ansible_watch_manager/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/watch_manager/ansible_watch_manager/resources/playbook-base.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 18:48:03.669494 oper8-0.1.9/oper8/watch_manager/ansible_watch_manager/resources/roles/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 18:48:03.669494 oper8-0.1.9/oper8/watch_manager/ansible_watch_manager/resources/roles/oper8_app/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 18:48:03.693494 oper8-0.1.9/oper8/watch_manager/ansible_watch_manager/resources/roles/oper8_app/defaults/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/watch_manager/ansible_watch_manager/resources/roles/oper8_app/defaults/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 18:48:03.693494 oper8-0.1.9/oper8/watch_manager/ansible_watch_manager/resources/roles/oper8_app/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/watch_manager/ansible_watch_manager/resources/roles/oper8_app/tasks/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/watch_manager/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4355 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/watch_manager/dry_run_watch_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 18:48:03.693494 oper8-0.1.9/oper8/watch_manager/python_watch_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/watch_manager/python_watch_manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 18:48:03.693494 oper8-0.1.9/oper8/watch_manager/python_watch_manager/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/watch_manager/python_watch_manager/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/watch_manager/python_watch_manager/filters/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13038 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/watch_manager/python_watch_manager/filters/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9557 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/watch_manager/python_watch_manager/filters/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 18:48:03.693494 oper8-0.1.9/oper8/watch_manager/python_watch_manager/leader_election/
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/watch_manager/python_watch_manager/leader_election/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5883 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/watch_manager/python_watch_manager/leader_election/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8349 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/watch_manager/python_watch_manager/leader_election/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/watch_manager/python_watch_manager/leader_election/dry_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5041 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/watch_manager/python_watch_manager/leader_election/lease.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/watch_manager/python_watch_manager/leader_election/life.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/watch_manager/python_watch_manager/python_watch_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13668 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/watch_manager/python_watch_manager/reconcile_process_entrypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 18:48:03.697494 oper8-0.1.9/oper8/watch_manager/python_watch_manager/threads/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/watch_manager/python_watch_manager/threads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/watch_manager/python_watch_manager/threads/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21578 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/watch_manager/python_watch_manager/threads/reconcile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5908 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/watch_manager/python_watch_manager/threads/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18357 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/watch_manager/python_watch_manager/threads/watch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 18:48:03.697494 oper8-0.1.9/oper8/watch_manager/python_watch_manager/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/watch_manager/python_watch_manager/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/watch_manager/python_watch_manager/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/watch_manager/python_watch_manager/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/watch_manager/python_watch_manager/utils/log_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8503 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/watch_manager/python_watch_manager/utils/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 18:48:03.697494 oper8-0.1.9/oper8/x/
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/x/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 18:48:03.697494 oper8-0.1.9/oper8/x/datastores/
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/x/datastores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/x/datastores/connection_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 18:48:03.697494 oper8-0.1.9/oper8/x/datastores/cos/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/x/datastores/cos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10931 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/x/datastores/cos/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/x/datastores/cos/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5169 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/x/datastores/cos/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12709 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/x/datastores/factory_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/x/datastores/interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 18:48:03.701494 oper8-0.1.9/oper8/x/datastores/postgres/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/x/datastores/postgres/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11174 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/x/datastores/postgres/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/x/datastores/postgres/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/x/datastores/postgres/interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 18:48:03.701494 oper8-0.1.9/oper8/x/datastores/redis/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/x/datastores/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10509 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/x/datastores/redis/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/x/datastores/redis/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4852 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/x/datastores/redis/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4889 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/x/oper8x_component.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 18:48:03.701494 oper8-0.1.9/oper8/x/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/x/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/x/utils/abc_static.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11562 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/x/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/x/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11395 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/x/utils/deps_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8113 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/x/utils/tls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 18:48:03.701494 oper8-0.1.9/oper8/x/utils/tls_context/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/x/utils/tls_context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4613 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/x/utils/tls_context/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5799 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/x/utils/tls_context/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11858 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/x/utils/tls_context/internal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-01-22 18:47:50.000000 oper8-0.1.9/oper8/x/utils/tls_context/public.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 18:48:03.717494 oper8-0.1.9/oper8.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-01-22 18:48:03.000000 oper8-0.1.9/oper8.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8035 2024-01-22 18:48:03.000000 oper8-0.1.9/oper8.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-22 18:48:03.000000 oper8-0.1.9/oper8.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-01-22 18:48:03.000000 oper8-0.1.9/oper8.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-01-22 18:48:03.000000 oper8-0.1.9/oper8.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-01-22 18:48:03.000000 oper8-0.1.9/oper8.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-01-22 18:47:50.000000 oper8-0.1.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 18:48:03.701494 oper8-0.1.9/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      720 2024-01-22 18:47:50.000000 oper8-0.1.9/scripts/fmt.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      351 2024-01-22 18:47:50.000000 oper8-0.1.9/scripts/lint.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      815 2024-01-22 18:47:50.000000 oper8-0.1.9/scripts/run_tests.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-22 18:48:03.717494 oper8-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-22 18:47:50.000000 oper8-0.1.9/setup_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 18:48:03.705494 oper8-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 18:48:03.705494 oper8-0.1.9/tests/dag/
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/dag/test_completion_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/dag/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/dag/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18443 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/dag/test_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 18:48:03.709494 oper8-0.1.9/tests/deploy_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)    18875 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/deploy_manager/test_dry_run_deploy_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46318 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/deploy_manager/test_openshift_deploy_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5673 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/deploy_manager/test_owner_references.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 18:48:03.709494 oper8-0.1.9/tests/temporary_patch/
+-rw-r--r--   0 runner    (1001) docker     (127)    20903 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/temporary_patch/test_temporary_patch_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8405 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/temporary_patch/test_temporary_patch_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22181 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/test_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8741 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17137 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/test_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3712 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12303 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12019 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/test_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7786 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/test_patch_strategic_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46411 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/test_reconcile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18877 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/test_rollout_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12579 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7847 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/test_setup_vcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19667 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/test_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9608 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8078 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/test_vcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13496 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/test_verify_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 18:48:03.709494 oper8-0.1.9/tests/watch_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/watch_manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 18:48:03.709494 oper8-0.1.9/tests/watch_manager/ansible_watch_manager/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 18:48:03.709494 oper8-0.1.9/tests/watch_manager/ansible_watch_manager/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)    13847 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/watch_manager/ansible_watch_manager/modules/test_k8s_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/watch_manager/ansible_watch_manager/modules/test_log_rotator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17630 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/watch_manager/ansible_watch_manager/test_ansible_watch_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 18:48:03.709494 oper8-0.1.9/tests/watch_manager/python_watch_manager/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 18:48:03.709494 oper8-0.1.9/tests/watch_manager/python_watch_manager/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/watch_manager/python_watch_manager/filters/test_common_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5965 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/watch_manager/python_watch_manager/filters/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/watch_manager/python_watch_manager/filters/test_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 18:48:03.709494 oper8-0.1.9/tests/watch_manager/python_watch_manager/leader_election/
+-rw-r--r--   0 runner    (1001) docker     (127)     8447 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/watch_manager/python_watch_manager/leader_election/test_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/watch_manager/python_watch_manager/leader_election/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7215 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/watch_manager/python_watch_manager/leader_election/test_lease.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/watch_manager/python_watch_manager/leader_election/test_life.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/watch_manager/python_watch_manager/test_python_watch_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9620 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/watch_manager/python_watch_manager/test_reconcile_process_entrypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 18:48:03.713494 oper8-0.1.9/tests/watch_manager/python_watch_manager/threads/
+-rw-r--r--   0 runner    (1001) docker     (127)     8538 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/watch_manager/python_watch_manager/threads/test_reconcile_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/watch_manager/python_watch_manager/threads/test_timer_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12897 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/watch_manager/python_watch_manager/threads/test_watch_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 18:48:03.713494 oper8-0.1.9/tests/watch_manager/python_watch_manager/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/watch_manager/python_watch_manager/utils/test_pwm_util_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5222 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/watch_manager/test_dry_run_watch_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/watch_manager/test_watch_manager_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 18:48:03.673494 oper8-0.1.9/tests/x/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 18:48:03.713494 oper8-0.1.9/tests/x/datastores/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/x/datastores/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 18:48:03.713494 oper8-0.1.9/tests/x/datastores/cos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/x/datastores/cos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17948 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/x/datastores/cos/test_cos_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 18:48:03.713494 oper8-0.1.9/tests/x/datastores/postgres/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/x/datastores/postgres/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/x/datastores/postgres/test_pg_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18168 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/x/datastores/postgres/test_postgres_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/x/datastores/postgres/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 18:48:03.713494 oper8-0.1.9/tests/x/datastores/redis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/x/datastores/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10592 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/x/datastores/redis/test_redis_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/x/datastores/redis/test_redis_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/x/datastores/redis/test_redis_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17114 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/x/datastores/test_factory_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 18:48:03.713494 oper8-0.1.9/tests/x/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/x/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/x/utils/test_abc_static.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/x/utils/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17656 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/x/utils/test_deps_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/x/utils/test_tls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15261 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/x/utils/test_tls_context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 18:48:03.717494 oper8-0.1.9/tests/x/utils/tls_context/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 18:48:03.717494 oper8-0.1.9/tests/x/utils/tls_context/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/x/utils/tls_context/snapshots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/x/utils/tls_context/test_internal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11303 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/x/utils/tls_context/test_tls_preconditions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-01-22 18:47:50.000000 oper8-0.1.9/tests/x/utils/tls_context/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-01-22 18:47:50.000000 oper8-0.1.9/tox.ini
```

### Comparing `oper8-0.1.8/.github/ISSUE_TEMPLATE/bug_report.md` & `oper8-0.1.9/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/.github/ISSUE_TEMPLATE/feature_request.md` & `oper8-0.1.9/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/.github/ISSUE_TEMPLATE/user_story.md` & `oper8-0.1.9/.github/ISSUE_TEMPLATE/user_story.md`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/.github/pull_request_template.md` & `oper8-0.1.9/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/.github/workflows/build-library.yml` & `oper8-0.1.9/.github/workflows/build-library.yml`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/.github/workflows/lint-code.yml` & `oper8-0.1.9/.github/workflows/lint-code.yml`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/.github/workflows/publish-library.yml` & `oper8-0.1.9/.github/workflows/publish-library.yml`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/CODE_OF_CONDUCT.md` & `oper8-0.1.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/CONTRIBUTING.md` & `oper8-0.1.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/LICENSE` & `oper8-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/PKG-INFO` & `oper8-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oper8
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python-native Kubernetes operator framework for managing trees of components
 License: Apache-2.0
 Project-URL: Source, https://github.com/IBM/oper8
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `oper8-0.1.8/SECURITY.md` & `oper8-0.1.9/SECURITY.md`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/__init__.py` & `oper8-0.1.9/oper8/__init__.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/__main__.py` & `oper8-0.1.9/oper8/__main__.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/cmd/base.py` & `oper8-0.1.9/oper8/cmd/base.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/cmd/run_operator_cmd.py` & `oper8-0.1.9/oper8/cmd/run_operator_cmd.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/cmd/setup_vcs_cmd.py` & `oper8-0.1.9/oper8/cmd/setup_vcs_cmd.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/component.py` & `oper8-0.1.9/oper8/component.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/config/__init__.py` & `oper8-0.1.9/oper8/config/__init__.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/config/config.py` & `oper8-0.1.9/oper8/config/config.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/config/config.yaml` & `oper8-0.1.9/oper8/config/config.yaml`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/config/config_validation.yaml` & `oper8-0.1.9/oper8/config/config_validation.yaml`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/config/validation.py` & `oper8-0.1.9/oper8/config/validation.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/constants.py` & `oper8-0.1.9/oper8/constants.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/controller.py` & `oper8-0.1.9/oper8/controller.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/dag/completion_state.py` & `oper8-0.1.9/oper8/dag/completion_state.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/dag/graph.py` & `oper8-0.1.9/oper8/dag/graph.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/dag/node.py` & `oper8-0.1.9/oper8/dag/node.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/dag/runner.py` & `oper8-0.1.9/oper8/dag/runner.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/decorator.py` & `oper8-0.1.9/oper8/decorator.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/deploy_manager/base.py` & `oper8-0.1.9/oper8/deploy_manager/base.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/deploy_manager/dry_run_deploy_manager.py` & `oper8-0.1.9/oper8/deploy_manager/dry_run_deploy_manager.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/deploy_manager/kube_event.py` & `oper8-0.1.9/oper8/deploy_manager/kube_event.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/deploy_manager/openshift_deploy_manager.py` & `oper8-0.1.9/oper8/deploy_manager/openshift_deploy_manager.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/deploy_manager/owner_references.py` & `oper8-0.1.9/oper8/deploy_manager/owner_references.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/exceptions.py` & `oper8-0.1.9/oper8/exceptions.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/log_format.py` & `oper8-0.1.9/oper8/log_format.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/managed_object.py` & `oper8-0.1.9/oper8/managed_object.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/patch.py` & `oper8-0.1.9/oper8/patch.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/patch_strategic_merge.py` & `oper8-0.1.9/oper8/patch_strategic_merge.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/reconcile.py` & `oper8-0.1.9/oper8/reconcile.py`

 * *Files 1% similar despite different names*

```diff
@@ -716,15 +716,17 @@
         for i in range(1, len(module_parts)):
             parent_module = ".".join(module_parts[:-i])
             if parent_module in sys.modules:
                 log.debug3("UnImporting module: %s", parent_module)
                 if sys.modules.pop(parent_module, None):
                     reimport_modules.add(parent_module)
         for child_module in [
-            mod_name for mod_name in sys.modules if mod_name.startswith(module_parts[0])
+            mod_name
+            for mod_name in sys.modules
+            if mod_name.startswith(f"{module_parts[0]}.")
         ]:
             log.debug3("UnImporting child module: %s", child_module)
             if sys.modules.pop(child_module, None):
                 reimport_modules.add(child_module)
         return reimport_modules
 
     def _import_controller(
```

### Comparing `oper8-0.1.8/oper8/rollout_manager.py` & `oper8-0.1.9/oper8/rollout_manager.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/session.py` & `oper8-0.1.9/oper8/session.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/setup_vcs.py` & `oper8-0.1.9/oper8/setup_vcs.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/status.py` & `oper8-0.1.9/oper8/status.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/temporary_patch/temporary_patch_component.py` & `oper8-0.1.9/oper8/temporary_patch/temporary_patch_component.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/temporary_patch/temporary_patch_controller.py` & `oper8-0.1.9/oper8/temporary_patch/temporary_patch_controller.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/test_helpers/data/test_ca.crt` & `oper8-0.1.9/oper8/test_helpers/data/test_ca.crt`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/test_helpers/data/test_ca.key` & `oper8-0.1.9/oper8/test_helpers/data/test_ca.key`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/test_helpers/helpers.py` & `oper8-0.1.9/oper8/test_helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/test_helpers/kub_mock.py` & `oper8-0.1.9/oper8/test_helpers/kub_mock.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/test_helpers/oper8x_helpers.py` & `oper8-0.1.9/oper8/test_helpers/oper8x_helpers.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/test_helpers/pwm_helpers.py` & `oper8-0.1.9/oper8/test_helpers/pwm_helpers.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/utils.py` & `oper8-0.1.9/oper8/utils.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/vcs.py` & `oper8-0.1.9/oper8/vcs.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/verify_resources.py` & `oper8-0.1.9/oper8/verify_resources.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/watch_manager/ansible_watch_manager/ansible_watch_manager.py` & `oper8-0.1.9/oper8/watch_manager/ansible_watch_manager/ansible_watch_manager.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/watch_manager/ansible_watch_manager/modules/k8s_application.py` & `oper8-0.1.9/oper8/watch_manager/ansible_watch_manager/modules/k8s_application.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/watch_manager/ansible_watch_manager/modules/log_rotator.py` & `oper8-0.1.9/oper8/watch_manager/ansible_watch_manager/modules/log_rotator.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/watch_manager/ansible_watch_manager/resources/roles/oper8_app/tasks/main.yml` & `oper8-0.1.9/oper8/watch_manager/ansible_watch_manager/resources/roles/oper8_app/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/watch_manager/base.py` & `oper8-0.1.9/oper8/watch_manager/base.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/watch_manager/dry_run_watch_manager.py` & `oper8-0.1.9/oper8/watch_manager/dry_run_watch_manager.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/watch_manager/python_watch_manager/filters/__init__.py` & `oper8-0.1.9/oper8/watch_manager/python_watch_manager/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/watch_manager/python_watch_manager/filters/common.py` & `oper8-0.1.9/oper8/watch_manager/python_watch_manager/filters/common.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/watch_manager/python_watch_manager/filters/filters.py` & `oper8-0.1.9/oper8/watch_manager/python_watch_manager/filters/filters.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/watch_manager/python_watch_manager/filters/manager.py` & `oper8-0.1.9/oper8/watch_manager/python_watch_manager/filters/manager.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/watch_manager/python_watch_manager/leader_election/__init__.py` & `oper8-0.1.9/oper8/watch_manager/python_watch_manager/leader_election/__init__.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/watch_manager/python_watch_manager/leader_election/annotation.py` & `oper8-0.1.9/oper8/watch_manager/python_watch_manager/leader_election/annotation.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/watch_manager/python_watch_manager/leader_election/base.py` & `oper8-0.1.9/oper8/watch_manager/python_watch_manager/leader_election/base.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/watch_manager/python_watch_manager/leader_election/dry_run.py` & `oper8-0.1.9/oper8/watch_manager/python_watch_manager/leader_election/dry_run.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/watch_manager/python_watch_manager/leader_election/lease.py` & `oper8-0.1.9/oper8/watch_manager/python_watch_manager/leader_election/lease.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/watch_manager/python_watch_manager/leader_election/life.py` & `oper8-0.1.9/oper8/watch_manager/python_watch_manager/leader_election/life.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/watch_manager/python_watch_manager/python_watch_manager.py` & `oper8-0.1.9/oper8/watch_manager/python_watch_manager/python_watch_manager.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/watch_manager/python_watch_manager/reconcile_process_entrypoint.py` & `oper8-0.1.9/oper8/watch_manager/python_watch_manager/reconcile_process_entrypoint.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/watch_manager/python_watch_manager/threads/base.py` & `oper8-0.1.9/oper8/watch_manager/python_watch_manager/threads/base.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/watch_manager/python_watch_manager/threads/reconcile.py` & `oper8-0.1.9/oper8/watch_manager/python_watch_manager/threads/reconcile.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/watch_manager/python_watch_manager/threads/timer.py` & `oper8-0.1.9/oper8/watch_manager/python_watch_manager/threads/timer.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/watch_manager/python_watch_manager/threads/watch.py` & `oper8-0.1.9/oper8/watch_manager/python_watch_manager/threads/watch.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/watch_manager/python_watch_manager/utils/__init__.py` & `oper8-0.1.9/oper8/watch_manager/python_watch_manager/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/watch_manager/python_watch_manager/utils/common.py` & `oper8-0.1.9/oper8/watch_manager/python_watch_manager/utils/common.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/watch_manager/python_watch_manager/utils/constants.py` & `oper8-0.1.9/oper8/watch_manager/python_watch_manager/utils/constants.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/watch_manager/python_watch_manager/utils/log_handler.py` & `oper8-0.1.9/oper8/watch_manager/python_watch_manager/utils/log_handler.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/watch_manager/python_watch_manager/utils/types.py` & `oper8-0.1.9/oper8/watch_manager/python_watch_manager/utils/types.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/x/datastores/connection_base.py` & `oper8-0.1.9/oper8/x/datastores/connection_base.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/x/datastores/cos/connection.py` & `oper8-0.1.9/oper8/x/datastores/cos/connection.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/x/datastores/cos/interfaces.py` & `oper8-0.1.9/oper8/x/datastores/cos/interfaces.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/x/datastores/factory_base.py` & `oper8-0.1.9/oper8/x/datastores/factory_base.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/x/datastores/interfaces.py` & `oper8-0.1.9/oper8/x/datastores/interfaces.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/x/datastores/postgres/connection.py` & `oper8-0.1.9/oper8/x/datastores/postgres/connection.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/x/datastores/postgres/interfaces.py` & `oper8-0.1.9/oper8/x/datastores/postgres/interfaces.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/x/datastores/redis/connection.py` & `oper8-0.1.9/oper8/x/datastores/redis/connection.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/x/datastores/redis/interfaces.py` & `oper8-0.1.9/oper8/x/datastores/redis/interfaces.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/x/oper8x_component.py` & `oper8-0.1.9/oper8/x/oper8x_component.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/x/utils/abc_static.py` & `oper8-0.1.9/oper8/x/utils/abc_static.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/x/utils/common.py` & `oper8-0.1.9/oper8/x/utils/common.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/x/utils/deps_annotation.py` & `oper8-0.1.9/oper8/x/utils/deps_annotation.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/x/utils/tls.py` & `oper8-0.1.9/oper8/x/utils/tls.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/x/utils/tls_context/factory.py` & `oper8-0.1.9/oper8/x/utils/tls_context/factory.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/x/utils/tls_context/interface.py` & `oper8-0.1.9/oper8/x/utils/tls_context/interface.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/x/utils/tls_context/internal.py` & `oper8-0.1.9/oper8/x/utils/tls_context/internal.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8/x/utils/tls_context/public.py` & `oper8-0.1.9/oper8/x/utils/tls_context/public.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8.egg-info/PKG-INFO` & `oper8-0.1.9/oper8.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oper8
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python-native Kubernetes operator framework for managing trees of components
 License: Apache-2.0
 Project-URL: Source, https://github.com/IBM/oper8
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `oper8-0.1.8/oper8.egg-info/SOURCES.txt` & `oper8-0.1.9/oper8.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/oper8.egg-info/requires.txt` & `oper8-0.1.9/oper8.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/pyproject.toml` & `oper8-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/scripts/fmt.sh` & `oper8-0.1.9/scripts/fmt.sh`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/scripts/run_tests.sh` & `oper8-0.1.9/scripts/run_tests.sh`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/tests/conftest.py` & `oper8-0.1.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/tests/dag/test_completion_state.py` & `oper8-0.1.9/tests/dag/test_completion_state.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/tests/dag/test_graph.py` & `oper8-0.1.9/tests/dag/test_graph.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/tests/dag/test_node.py` & `oper8-0.1.9/tests/dag/test_node.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/tests/dag/test_runner.py` & `oper8-0.1.9/tests/dag/test_runner.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/tests/deploy_manager/test_dry_run_deploy_manager.py` & `oper8-0.1.9/tests/deploy_manager/test_dry_run_deploy_manager.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/tests/deploy_manager/test_openshift_deploy_manager.py` & `oper8-0.1.9/tests/deploy_manager/test_openshift_deploy_manager.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/tests/deploy_manager/test_owner_references.py` & `oper8-0.1.9/tests/deploy_manager/test_owner_references.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/tests/temporary_patch/test_temporary_patch_component.py` & `oper8-0.1.9/tests/temporary_patch/test_temporary_patch_component.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/tests/temporary_patch/test_temporary_patch_controller.py` & `oper8-0.1.9/tests/temporary_patch/test_temporary_patch_controller.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/tests/test_component.py` & `oper8-0.1.9/tests/test_component.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/tests/test_config.py` & `oper8-0.1.9/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/tests/test_controller.py` & `oper8-0.1.9/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/tests/test_decorator.py` & `oper8-0.1.9/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/tests/test_exceptions.py` & `oper8-0.1.9/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/tests/test_main.py` & `oper8-0.1.9/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/tests/test_patch.py` & `oper8-0.1.9/tests/test_patch.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/tests/test_patch_strategic_merge.py` & `oper8-0.1.9/tests/test_patch_strategic_merge.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/tests/test_reconcile.py` & `oper8-0.1.9/tests/test_reconcile.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/tests/test_rollout_manager.py` & `oper8-0.1.9/tests/test_rollout_manager.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/tests/test_session.py` & `oper8-0.1.9/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/tests/test_setup_vcs.py` & `oper8-0.1.9/tests/test_setup_vcs.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/tests/test_status.py` & `oper8-0.1.9/tests/test_status.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/tests/test_utils.py` & `oper8-0.1.9/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/tests/test_vcs.py` & `oper8-0.1.9/tests/test_vcs.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/tests/test_verify_resources.py` & `oper8-0.1.9/tests/test_verify_resources.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/tests/watch_manager/ansible_watch_manager/modules/test_k8s_application.py` & `oper8-0.1.9/tests/watch_manager/ansible_watch_manager/modules/test_k8s_application.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/tests/watch_manager/ansible_watch_manager/modules/test_log_rotator.py` & `oper8-0.1.9/tests/watch_manager/ansible_watch_manager/modules/test_log_rotator.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/tests/watch_manager/ansible_watch_manager/test_ansible_watch_manager.py` & `oper8-0.1.9/tests/watch_manager/ansible_watch_manager/test_ansible_watch_manager.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/tests/watch_manager/python_watch_manager/filters/test_common_filters.py` & `oper8-0.1.9/tests/watch_manager/python_watch_manager/filters/test_common_filters.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/tests/watch_manager/python_watch_manager/filters/test_filters.py` & `oper8-0.1.9/tests/watch_manager/python_watch_manager/filters/test_filters.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/tests/watch_manager/python_watch_manager/filters/test_manager.py` & `oper8-0.1.9/tests/watch_manager/python_watch_manager/filters/test_manager.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/tests/watch_manager/python_watch_manager/leader_election/test_annotation.py` & `oper8-0.1.9/tests/watch_manager/python_watch_manager/leader_election/test_annotation.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/tests/watch_manager/python_watch_manager/leader_election/test_init.py` & `oper8-0.1.9/tests/watch_manager/python_watch_manager/leader_election/test_init.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/tests/watch_manager/python_watch_manager/leader_election/test_lease.py` & `oper8-0.1.9/tests/watch_manager/python_watch_manager/leader_election/test_lease.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/tests/watch_manager/python_watch_manager/leader_election/test_life.py` & `oper8-0.1.9/tests/watch_manager/python_watch_manager/leader_election/test_life.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/tests/watch_manager/python_watch_manager/test_python_watch_manager.py` & `oper8-0.1.9/tests/watch_manager/python_watch_manager/test_python_watch_manager.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/tests/watch_manager/python_watch_manager/test_reconcile_process_entrypoint.py` & `oper8-0.1.9/tests/watch_manager/python_watch_manager/test_reconcile_process_entrypoint.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/tests/watch_manager/python_watch_manager/threads/test_reconcile_thread.py` & `oper8-0.1.9/tests/watch_manager/python_watch_manager/threads/test_reconcile_thread.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/tests/watch_manager/python_watch_manager/threads/test_timer_thread.py` & `oper8-0.1.9/tests/watch_manager/python_watch_manager/threads/test_timer_thread.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/tests/watch_manager/python_watch_manager/threads/test_watch_thread.py` & `oper8-0.1.9/tests/watch_manager/python_watch_manager/threads/test_watch_thread.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/tests/watch_manager/python_watch_manager/utils/test_pwm_util_common.py` & `oper8-0.1.9/tests/watch_manager/python_watch_manager/utils/test_pwm_util_common.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/tests/watch_manager/test_dry_run_watch_manager.py` & `oper8-0.1.9/tests/watch_manager/test_dry_run_watch_manager.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/tests/watch_manager/test_watch_manager_base.py` & `oper8-0.1.9/tests/watch_manager/test_watch_manager_base.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/tests/x/datastores/cos/test_cos_connection.py` & `oper8-0.1.9/tests/x/datastores/cos/test_cos_connection.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/tests/x/datastores/postgres/test_pg_factory.py` & `oper8-0.1.9/tests/x/datastores/postgres/test_pg_factory.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/tests/x/datastores/postgres/test_postgres_connection.py` & `oper8-0.1.9/tests/x/datastores/postgres/test_postgres_connection.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/tests/x/datastores/postgres/util.py` & `oper8-0.1.9/tests/x/datastores/postgres/util.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/tests/x/datastores/redis/test_redis_connection.py` & `oper8-0.1.9/tests/x/datastores/redis/test_redis_connection.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/tests/x/datastores/redis/test_redis_factory.py` & `oper8-0.1.9/tests/x/datastores/redis/test_redis_factory.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/tests/x/datastores/test_factory_base.py` & `oper8-0.1.9/tests/x/datastores/test_factory_base.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/tests/x/utils/test_abc_static.py` & `oper8-0.1.9/tests/x/utils/test_abc_static.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/tests/x/utils/test_common.py` & `oper8-0.1.9/tests/x/utils/test_common.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/tests/x/utils/test_deps_annotation.py` & `oper8-0.1.9/tests/x/utils/test_deps_annotation.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/tests/x/utils/test_tls_context.py` & `oper8-0.1.9/tests/x/utils/test_tls_context.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/tests/x/utils/tls_context/test_internal.py` & `oper8-0.1.9/tests/x/utils/tls_context/test_internal.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/tests/x/utils/tls_context/test_tls_preconditions.py` & `oper8-0.1.9/tests/x/utils/tls_context/test_tls_preconditions.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/tests/x/utils/tls_context/util.py` & `oper8-0.1.9/tests/x/utils/tls_context/util.py`

 * *Files identical despite different names*

### Comparing `oper8-0.1.8/tox.ini` & `oper8-0.1.9/tox.ini`

 * *Files identical despite different names*

