# Comparing `tmp/seqerakit-0.4.7.tar.gz` & `tmp/seqerakit-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seqerakit-0.4.7.tar", last modified: Fri Apr 26 01:30:57 2024, max compression
+gzip compressed data, was "seqerakit-0.4.8.tar", last modified: Thu May  2 02:19:48 2024, max compression
```

## Comparing `seqerakit-0.4.7.tar` & `seqerakit-0.4.8.tar`

### file list

```diff
@@ -1,98 +1,99 @@
-drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-04-26 01:30:57.718180 seqerakit-0.4.7/
--rw-r--r--   0 eshajoshi   (501) staff       (20)      239 2023-10-13 03:44:10.000000 seqerakit-0.4.7/.dockerignore
-drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-04-26 01:30:57.695945 seqerakit-0.4.7/.github/
--rw-r--r--   0 eshajoshi   (501) staff       (20)     5024 2023-10-13 03:44:10.000000 seqerakit-0.4.7/.github/CONTRIBUTING.md
-drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-04-26 01:30:57.696832 seqerakit-0.4.7/.github/workflows/
--rw-r--r--   0 eshajoshi   (501) staff       (20)     3042 2024-01-10 03:27:27.000000 seqerakit-0.4.7/.github/workflows/e2e-testing.yml
--rw-r--r--   0 eshajoshi   (501) staff       (20)      724 2024-01-10 03:27:27.000000 seqerakit-0.4.7/.github/workflows/python-testing.yml
--rw-r--r--   0 eshajoshi   (501) staff       (20)     1804 2024-01-10 03:27:27.000000 seqerakit-0.4.7/.github/workflows/teardown.yml
--rw-r--r--   0 eshajoshi   (501) staff       (20)      278 2024-04-26 01:13:08.000000 seqerakit-0.4.7/.gitignore
--rw-r--r--   0 eshajoshi   (501) staff       (20)      763 2023-11-10 19:39:47.000000 seqerakit-0.4.7/.pre-commit-config.yaml
--rw-r--r--   0 eshajoshi   (501) staff       (20)      286 2023-11-25 22:33:31.000000 seqerakit-0.4.7/.prettierrc
--rw-r--r--   0 eshajoshi   (501) staff       (20)    11358 2023-11-15 02:34:37.000000 seqerakit-0.4.7/LICENSE.txt
--rw-r--r--   0 eshajoshi   (501) staff       (20)    16525 2024-04-26 01:30:57.717707 seqerakit-0.4.7/PKG-INFO
--rw-r--r--   0 eshajoshi   (501) staff       (20)    16016 2024-04-26 01:30:01.000000 seqerakit-0.4.7/README.md
--rw-r--r--   0 eshajoshi   (501) staff       (20)       25 2023-10-13 03:44:10.000000 seqerakit-0.4.7/__init__.py
-drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-04-26 01:30:57.697478 seqerakit-0.4.7/assets/
--rw-r--r--   0 eshajoshi   (501) staff       (20)    15390 2024-04-26 01:13:08.000000 seqerakit-0.4.7/assets/seqerakit.svg
-drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-04-26 01:30:57.692713 seqerakit-0.4.7/examples/
-drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-04-26 01:30:57.697657 seqerakit-0.4.7/examples/python/
--rwxr-xr-x   0 eshajoshi   (501) staff       (20)      783 2023-10-13 03:44:10.000000 seqerakit-0.4.7/examples/python/launch_hello_world.py
-drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-04-26 01:30:57.697915 seqerakit-0.4.7/examples/yaml/
-drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-04-26 01:30:57.699468 seqerakit-0.4.7/examples/yaml/compute-envs/
--rw-r--r--   0 eshajoshi   (501) staff       (20)      627 2023-10-13 03:44:10.000000 seqerakit-0.4.7/examples/yaml/compute-envs/seqera_aws_ireland_fusionv2_nvme.json
--rw-r--r--   0 eshajoshi   (501) staff       (20)      622 2023-10-13 03:44:10.000000 seqerakit-0.4.7/examples/yaml/compute-envs/seqera_aws_virginia_fusionv2_nvme.json
--rw-r--r--   0 eshajoshi   (501) staff       (20)      335 2023-10-13 03:44:10.000000 seqerakit-0.4.7/examples/yaml/compute-envs/seqera_azure_virginia.json
--rw-r--r--   0 eshajoshi   (501) staff       (20)      257 2023-10-13 03:44:10.000000 seqerakit-0.4.7/examples/yaml/compute-envs/seqera_gcp_finland.json
-drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-04-26 01:30:57.700441 seqerakit-0.4.7/examples/yaml/datasets/
--rw-r--r--   0 eshajoshi   (501) staff       (20)     1012 2023-10-13 03:44:10.000000 seqerakit-0.4.7/examples/yaml/datasets/rnaseq_samples.csv
--rw-r--r--   0 eshajoshi   (501) staff       (20)      314 2023-10-13 03:44:10.000000 seqerakit-0.4.7/examples/yaml/datasets/sarek_samples.csv
--rw-r--r--   0 eshajoshi   (501) staff       (20)     1181 2023-10-13 03:44:10.000000 seqerakit-0.4.7/examples/yaml/datasets/sentieon_samples.csv
--rw-r--r--   0 eshajoshi   (501) staff       (20)      699 2023-10-13 03:44:10.000000 seqerakit-0.4.7/examples/yaml/datasets/viralrecon_illumina_samples.csv
--rw-r--r--   0 eshajoshi   (501) staff       (20)      149 2023-10-13 03:44:10.000000 seqerakit-0.4.7/examples/yaml/datasets/viralrecon_nanopore_samples.csv
-drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-04-26 01:30:57.705041 seqerakit-0.4.7/examples/yaml/e2e/
--rw-r--r--   0 eshajoshi   (501) staff       (20)      376 2024-01-10 03:27:27.000000 seqerakit-0.4.7/examples/yaml/e2e/actions.yml
--rw-r--r--   0 eshajoshi   (501) staff       (20)      709 2024-01-10 03:27:27.000000 seqerakit-0.4.7/examples/yaml/e2e/compute-envs.yml
--rw-r--r--   0 eshajoshi   (501) staff       (20)      994 2024-01-10 03:27:27.000000 seqerakit-0.4.7/examples/yaml/e2e/credentials.yml
--rw-r--r--   0 eshajoshi   (501) staff       (20)     1352 2024-01-10 03:27:27.000000 seqerakit-0.4.7/examples/yaml/e2e/datasets.yml
--rw-r--r--   0 eshajoshi   (501) staff       (20)      108 2024-04-26 01:06:21.000000 seqerakit-0.4.7/examples/yaml/e2e/labels.yml
--rw-r--r--   0 eshajoshi   (501) staff       (20)      111 2024-04-26 01:06:21.000000 seqerakit-0.4.7/examples/yaml/e2e/members.yml
--rw-r--r--   0 eshajoshi   (501) staff       (20)      222 2024-01-10 03:27:27.000000 seqerakit-0.4.7/examples/yaml/e2e/organizations.yml
--rw-r--r--   0 eshajoshi   (501) staff       (20)      265 2024-01-10 03:27:27.000000 seqerakit-0.4.7/examples/yaml/e2e/participants.yml
--rw-r--r--   0 eshajoshi   (501) staff       (20)     1590 2024-01-10 03:27:27.000000 seqerakit-0.4.7/examples/yaml/e2e/pipelines.yml
--rw-r--r--   0 eshajoshi   (501) staff       (20)      143 2024-01-10 03:27:27.000000 seqerakit-0.4.7/examples/yaml/e2e/secrets.yml
--rw-r--r--   0 eshajoshi   (501) staff       (20)      252 2024-01-10 03:27:27.000000 seqerakit-0.4.7/examples/yaml/e2e/teams.yml
--rw-r--r--   0 eshajoshi   (501) staff       (20)      209 2024-01-10 03:27:27.000000 seqerakit-0.4.7/examples/yaml/e2e/workspaces.yml
-drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-04-26 01:30:57.707036 seqerakit-0.4.7/examples/yaml/pipelines/
--rw-r--r--   0 eshajoshi   (501) staff       (20)       22 2023-10-13 03:44:10.000000 seqerakit-0.4.7/examples/yaml/pipelines/nextflow.config
--rw-r--r--   0 eshajoshi   (501) staff       (20)      537 2023-10-13 03:44:10.000000 seqerakit-0.4.7/examples/yaml/pipelines/nf-core-sarek_pipeline.json
--rw-r--r--   0 eshajoshi   (501) staff       (20)       57 2023-10-13 03:44:10.000000 seqerakit-0.4.7/examples/yaml/pipelines/nf_core_rnaseq_params.yml
--rw-r--r--   0 eshajoshi   (501) staff       (20)      581 2023-10-13 03:44:10.000000 seqerakit-0.4.7/examples/yaml/pipelines/nf_core_rnaseq_pipeline.json
--rw-r--r--   0 eshajoshi   (501) staff       (20)       81 2023-10-13 03:44:10.000000 seqerakit-0.4.7/examples/yaml/pipelines/nf_core_viralrecon_illumina_params.yml
--rw-r--r--   0 eshajoshi   (501) staff       (20)      503 2023-10-13 03:44:10.000000 seqerakit-0.4.7/examples/yaml/pipelines/nf_core_viralrecon_illumina_pipeline.json
--rw-r--r--   0 eshajoshi   (501) staff       (20)      512 2023-10-13 03:44:10.000000 seqerakit-0.4.7/examples/yaml/pipelines/nf_core_viralrecon_nanopore_pipeline.json
--rw-r--r--   0 eshajoshi   (501) staff       (20)      576 2023-10-13 03:44:10.000000 seqerakit-0.4.7/examples/yaml/pipelines/nf_sentieon_pipeline.json
--rw-r--r--   0 eshajoshi   (501) staff       (20)       23 2024-01-10 03:27:27.000000 seqerakit-0.4.7/examples/yaml/pipelines/pre_run.txt
--rw-r--r--   0 eshajoshi   (501) staff       (20)     6702 2024-04-26 00:48:24.000000 seqerakit-0.4.7/examples/yaml/seqerakit-e2e.yml
-drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-04-26 01:30:57.710502 seqerakit-0.4.7/seqerakit/
--rw-r--r--   0 eshajoshi   (501) staff       (20)      100 2024-03-18 04:58:40.000000 seqerakit-0.4.7/seqerakit/__init__.py
--rw-r--r--   0 eshajoshi   (501) staff       (20)     6904 2024-04-25 23:44:28.000000 seqerakit-0.4.7/seqerakit/cli.py
--rw-r--r--   0 eshajoshi   (501) staff       (20)     1641 2023-11-15 02:34:37.000000 seqerakit-0.4.7/seqerakit/computeenvs.py
--rw-r--r--   0 eshajoshi   (501) staff       (20)    12973 2024-04-25 23:34:42.000000 seqerakit-0.4.7/seqerakit/dump_yaml.py
--rw-r--r--   0 eshajoshi   (501) staff       (20)    12576 2024-04-25 23:48:34.000000 seqerakit-0.4.7/seqerakit/helper.py
--rw-r--r--   0 eshajoshi   (501) staff       (20)    12623 2024-04-26 00:46:21.000000 seqerakit-0.4.7/seqerakit/overwrite.py
--rw-r--r--   0 eshajoshi   (501) staff       (20)     1619 2023-11-15 02:34:37.000000 seqerakit-0.4.7/seqerakit/pipelines.py
--rw-r--r--   0 eshajoshi   (501) staff       (20)     5069 2024-04-25 23:44:28.000000 seqerakit-0.4.7/seqerakit/seqeraplatform.py
--rw-r--r--   0 eshajoshi   (501) staff       (20)     5112 2024-04-26 00:46:21.000000 seqerakit-0.4.7/seqerakit/utils.py
-drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-04-26 01:30:57.711731 seqerakit-0.4.7/seqerakit.egg-info/
--rw-r--r--   0 eshajoshi   (501) staff       (20)    16525 2024-04-26 01:30:57.000000 seqerakit-0.4.7/seqerakit.egg-info/PKG-INFO
--rw-r--r--   0 eshajoshi   (501) staff       (20)     2528 2024-04-26 01:30:57.000000 seqerakit-0.4.7/seqerakit.egg-info/SOURCES.txt
--rw-r--r--   0 eshajoshi   (501) staff       (20)        1 2024-04-26 01:30:57.000000 seqerakit-0.4.7/seqerakit.egg-info/dependency_links.txt
--rw-r--r--   0 eshajoshi   (501) staff       (20)       49 2024-04-26 01:30:57.000000 seqerakit-0.4.7/seqerakit.egg-info/entry_points.txt
--rw-r--r--   0 eshajoshi   (501) staff       (20)        1 2023-11-29 04:33:12.000000 seqerakit-0.4.7/seqerakit.egg-info/not-zip-safe
--rw-r--r--   0 eshajoshi   (501) staff       (20)       14 2024-04-26 01:30:57.000000 seqerakit-0.4.7/seqerakit.egg-info/requires.txt
--rw-r--r--   0 eshajoshi   (501) staff       (20)       10 2024-04-26 01:30:57.000000 seqerakit-0.4.7/seqerakit.egg-info/top_level.txt
--rw-r--r--   0 eshajoshi   (501) staff       (20)       38 2024-04-26 01:30:57.718229 seqerakit-0.4.7/setup.cfg
--rw-r--r--   0 eshajoshi   (501) staff       (20)      964 2024-04-26 01:17:35.000000 seqerakit-0.4.7/setup.py
-drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-04-26 01:30:57.715416 seqerakit-0.4.7/templates/
--rw-r--r--   0 eshajoshi   (501) staff       (20)     1540 2024-01-10 03:27:27.000000 seqerakit-0.4.7/templates/actions.yml
--rw-r--r--   0 eshajoshi   (501) staff       (20)     2847 2024-01-10 03:27:27.000000 seqerakit-0.4.7/templates/compute-envs.yml
--rw-r--r--   0 eshajoshi   (501) staff       (20)     2163 2024-01-10 03:27:27.000000 seqerakit-0.4.7/templates/credentials.yml
--rw-r--r--   0 eshajoshi   (501) staff       (20)      419 2023-10-13 03:44:10.000000 seqerakit-0.4.7/templates/datasets.yml
--rw-r--r--   0 eshajoshi   (501) staff       (20)      310 2024-04-05 23:44:56.000000 seqerakit-0.4.7/templates/labels.yml
--rw-r--r--   0 eshajoshi   (501) staff       (20)     1394 2024-01-10 03:27:27.000000 seqerakit-0.4.7/templates/launch.yml
--rw-r--r--   0 eshajoshi   (501) staff       (20)      266 2024-04-05 23:44:56.000000 seqerakit-0.4.7/templates/members.yml
--rw-r--r--   0 eshajoshi   (501) staff       (20)      405 2023-10-13 03:44:10.000000 seqerakit-0.4.7/templates/organizations.yml
--rw-r--r--   0 eshajoshi   (501) staff       (20)      541 2024-03-20 19:32:10.000000 seqerakit-0.4.7/templates/participants.yml
--rw-r--r--   0 eshajoshi   (501) staff       (20)     1478 2024-01-10 03:27:27.000000 seqerakit-0.4.7/templates/pipelines.yml
--rw-r--r--   0 eshajoshi   (501) staff       (20)      303 2023-10-13 03:44:10.000000 seqerakit-0.4.7/templates/secrets.yml
--rw-r--r--   0 eshajoshi   (501) staff       (20)      341 2023-10-13 03:44:10.000000 seqerakit-0.4.7/templates/teams.yml
--rw-r--r--   0 eshajoshi   (501) staff       (20)      375 2023-10-13 03:44:10.000000 seqerakit-0.4.7/templates/workspaces.yml
-drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-04-26 01:30:57.693463 seqerakit-0.4.7/tests/
-drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-04-26 01:30:57.715595 seqerakit-0.4.7/tests/e2e/
--rw-r--r--   0 eshajoshi   (501) staff       (20)     2735 2024-01-10 03:27:27.000000 seqerakit-0.4.7/tests/e2e/aws-e2e.yml
-drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-04-26 01:30:57.716897 seqerakit-0.4.7/tests/unit/
--rw-r--r--   0 eshajoshi   (501) staff       (20)       25 2024-02-28 20:36:16.000000 seqerakit-0.4.7/tests/unit/__init__.py
--rw-r--r--   0 eshajoshi   (501) staff       (20)    13003 2024-04-25 23:44:28.000000 seqerakit-0.4.7/tests/unit/test_helper.py
--rw-r--r--   0 eshajoshi   (501) staff       (20)     8359 2024-04-25 23:44:28.000000 seqerakit-0.4.7/tests/unit/test_seqeraplatform.py
--rw-r--r--   0 eshajoshi   (501) staff       (20)     5835 2023-10-13 03:44:10.000000 seqerakit-0.4.7/tests/unit/test_subcommands.py
+drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-05-02 02:19:48.180481 seqerakit-0.4.8/
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      239 2023-10-13 03:44:10.000000 seqerakit-0.4.8/.dockerignore
+drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-05-02 02:19:48.167333 seqerakit-0.4.8/.github/
+-rw-r--r--   0 eshajoshi   (501) staff       (20)     5024 2023-10-13 03:44:10.000000 seqerakit-0.4.8/.github/CONTRIBUTING.md
+drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-05-02 02:19:48.167817 seqerakit-0.4.8/.github/workflows/
+-rw-r--r--   0 eshajoshi   (501) staff       (20)     3042 2024-05-02 02:18:19.000000 seqerakit-0.4.8/.github/workflows/e2e-testing.yml
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      724 2024-05-02 02:18:19.000000 seqerakit-0.4.8/.github/workflows/python-testing.yml
+-rw-r--r--   0 eshajoshi   (501) staff       (20)     1804 2024-05-02 02:18:19.000000 seqerakit-0.4.8/.github/workflows/teardown.yml
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      287 2024-05-02 02:07:22.000000 seqerakit-0.4.8/.gitignore
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      763 2023-11-10 19:39:47.000000 seqerakit-0.4.8/.pre-commit-config.yaml
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      286 2023-11-25 22:33:31.000000 seqerakit-0.4.8/.prettierrc
+-rw-r--r--   0 eshajoshi   (501) staff       (20)    11358 2023-11-15 02:34:37.000000 seqerakit-0.4.8/LICENSE.txt
+-rw-r--r--   0 eshajoshi   (501) staff       (20)       20 2024-05-02 02:09:33.000000 seqerakit-0.4.8/MANIFEST.in
+-rw-r--r--   0 eshajoshi   (501) staff       (20)    16463 2024-05-02 02:19:48.180044 seqerakit-0.4.8/PKG-INFO
+-rw-r--r--   0 eshajoshi   (501) staff       (20)    15954 2024-05-02 02:18:19.000000 seqerakit-0.4.8/README.md
+-rw-r--r--   0 eshajoshi   (501) staff       (20)       25 2023-10-13 03:44:10.000000 seqerakit-0.4.8/__init__.py
+drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-05-02 02:19:48.168315 seqerakit-0.4.8/assets/
+-rw-r--r--   0 eshajoshi   (501) staff       (20)    25426 2024-05-02 02:18:19.000000 seqerakit-0.4.8/assets/seqerakit.png
+-rw-r--r--   0 eshajoshi   (501) staff       (20)    15065 2024-05-02 02:18:19.000000 seqerakit-0.4.8/assets/seqerakit.svg
+drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-05-02 02:19:48.164206 seqerakit-0.4.8/examples/
+drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-05-02 02:19:48.168473 seqerakit-0.4.8/examples/python/
+-rwxr-xr-x   0 eshajoshi   (501) staff       (20)      783 2023-10-13 03:44:10.000000 seqerakit-0.4.8/examples/python/launch_hello_world.py
+drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-05-02 02:19:48.168753 seqerakit-0.4.8/examples/yaml/
+drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-05-02 02:19:48.169674 seqerakit-0.4.8/examples/yaml/compute-envs/
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      627 2023-10-13 03:44:10.000000 seqerakit-0.4.8/examples/yaml/compute-envs/seqera_aws_ireland_fusionv2_nvme.json
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      622 2023-10-13 03:44:10.000000 seqerakit-0.4.8/examples/yaml/compute-envs/seqera_aws_virginia_fusionv2_nvme.json
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      335 2023-10-13 03:44:10.000000 seqerakit-0.4.8/examples/yaml/compute-envs/seqera_azure_virginia.json
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      257 2023-10-13 03:44:10.000000 seqerakit-0.4.8/examples/yaml/compute-envs/seqera_gcp_finland.json
+drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-05-02 02:19:48.170493 seqerakit-0.4.8/examples/yaml/datasets/
+-rw-r--r--   0 eshajoshi   (501) staff       (20)     1012 2023-10-13 03:44:10.000000 seqerakit-0.4.8/examples/yaml/datasets/rnaseq_samples.csv
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      314 2023-10-13 03:44:10.000000 seqerakit-0.4.8/examples/yaml/datasets/sarek_samples.csv
+-rw-r--r--   0 eshajoshi   (501) staff       (20)     1181 2023-10-13 03:44:10.000000 seqerakit-0.4.8/examples/yaml/datasets/sentieon_samples.csv
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      699 2023-10-13 03:44:10.000000 seqerakit-0.4.8/examples/yaml/datasets/viralrecon_illumina_samples.csv
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      149 2023-10-13 03:44:10.000000 seqerakit-0.4.8/examples/yaml/datasets/viralrecon_nanopore_samples.csv
+drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-05-02 02:19:48.172252 seqerakit-0.4.8/examples/yaml/e2e/
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      376 2024-05-02 02:18:19.000000 seqerakit-0.4.8/examples/yaml/e2e/actions.yml
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      709 2024-05-02 02:18:19.000000 seqerakit-0.4.8/examples/yaml/e2e/compute-envs.yml
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      994 2024-05-02 02:18:19.000000 seqerakit-0.4.8/examples/yaml/e2e/credentials.yml
+-rw-r--r--   0 eshajoshi   (501) staff       (20)     1352 2024-05-02 02:18:19.000000 seqerakit-0.4.8/examples/yaml/e2e/datasets.yml
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      108 2024-05-02 02:18:19.000000 seqerakit-0.4.8/examples/yaml/e2e/labels.yml
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      111 2024-05-02 02:18:19.000000 seqerakit-0.4.8/examples/yaml/e2e/members.yml
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      222 2024-05-02 02:18:19.000000 seqerakit-0.4.8/examples/yaml/e2e/organizations.yml
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      265 2024-05-02 02:18:19.000000 seqerakit-0.4.8/examples/yaml/e2e/participants.yml
+-rw-r--r--   0 eshajoshi   (501) staff       (20)     1590 2024-05-02 02:18:19.000000 seqerakit-0.4.8/examples/yaml/e2e/pipelines.yml
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      143 2024-05-02 02:18:19.000000 seqerakit-0.4.8/examples/yaml/e2e/secrets.yml
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      252 2024-05-02 02:18:19.000000 seqerakit-0.4.8/examples/yaml/e2e/teams.yml
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      209 2024-05-02 02:18:19.000000 seqerakit-0.4.8/examples/yaml/e2e/workspaces.yml
+drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-05-02 02:19:48.173922 seqerakit-0.4.8/examples/yaml/pipelines/
+-rw-r--r--   0 eshajoshi   (501) staff       (20)       22 2023-10-13 03:44:10.000000 seqerakit-0.4.8/examples/yaml/pipelines/nextflow.config
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      537 2023-10-13 03:44:10.000000 seqerakit-0.4.8/examples/yaml/pipelines/nf-core-sarek_pipeline.json
+-rw-r--r--   0 eshajoshi   (501) staff       (20)       57 2023-10-13 03:44:10.000000 seqerakit-0.4.8/examples/yaml/pipelines/nf_core_rnaseq_params.yml
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      581 2023-10-13 03:44:10.000000 seqerakit-0.4.8/examples/yaml/pipelines/nf_core_rnaseq_pipeline.json
+-rw-r--r--   0 eshajoshi   (501) staff       (20)       81 2023-10-13 03:44:10.000000 seqerakit-0.4.8/examples/yaml/pipelines/nf_core_viralrecon_illumina_params.yml
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      503 2023-10-13 03:44:10.000000 seqerakit-0.4.8/examples/yaml/pipelines/nf_core_viralrecon_illumina_pipeline.json
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      512 2023-10-13 03:44:10.000000 seqerakit-0.4.8/examples/yaml/pipelines/nf_core_viralrecon_nanopore_pipeline.json
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      576 2023-10-13 03:44:10.000000 seqerakit-0.4.8/examples/yaml/pipelines/nf_sentieon_pipeline.json
+-rw-r--r--   0 eshajoshi   (501) staff       (20)       23 2024-05-02 02:18:19.000000 seqerakit-0.4.8/examples/yaml/pipelines/pre_run.txt
+-rw-r--r--   0 eshajoshi   (501) staff       (20)     6702 2024-04-26 00:48:24.000000 seqerakit-0.4.8/examples/yaml/seqerakit-e2e.yml
+drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-05-02 02:19:48.174962 seqerakit-0.4.8/seqerakit/
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      100 2024-05-02 02:18:19.000000 seqerakit-0.4.8/seqerakit/__init__.py
+-rw-r--r--   0 eshajoshi   (501) staff       (20)     6904 2024-05-02 02:18:19.000000 seqerakit-0.4.8/seqerakit/cli.py
+-rw-r--r--   0 eshajoshi   (501) staff       (20)     1641 2023-11-15 02:34:37.000000 seqerakit-0.4.8/seqerakit/computeenvs.py
+-rw-r--r--   0 eshajoshi   (501) staff       (20)    12786 2024-05-02 02:18:19.000000 seqerakit-0.4.8/seqerakit/helper.py
+-rw-r--r--   0 eshajoshi   (501) staff       (20)    12623 2024-05-02 02:18:19.000000 seqerakit-0.4.8/seqerakit/overwrite.py
+-rw-r--r--   0 eshajoshi   (501) staff       (20)     1619 2023-11-15 02:34:37.000000 seqerakit-0.4.8/seqerakit/pipelines.py
+-rw-r--r--   0 eshajoshi   (501) staff       (20)     5069 2024-05-02 02:18:19.000000 seqerakit-0.4.8/seqerakit/seqeraplatform.py
+-rw-r--r--   0 eshajoshi   (501) staff       (20)     5112 2024-05-02 02:18:19.000000 seqerakit-0.4.8/seqerakit/utils.py
+drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-05-02 02:19:48.176127 seqerakit-0.4.8/seqerakit.egg-info/
+-rw-r--r--   0 eshajoshi   (501) staff       (20)    16463 2024-05-02 02:19:48.000000 seqerakit-0.4.8/seqerakit.egg-info/PKG-INFO
+-rw-r--r--   0 eshajoshi   (501) staff       (20)     2538 2024-05-02 02:19:48.000000 seqerakit-0.4.8/seqerakit.egg-info/SOURCES.txt
+-rw-r--r--   0 eshajoshi   (501) staff       (20)        1 2024-05-02 02:19:48.000000 seqerakit-0.4.8/seqerakit.egg-info/dependency_links.txt
+-rw-r--r--   0 eshajoshi   (501) staff       (20)       49 2024-05-02 02:19:48.000000 seqerakit-0.4.8/seqerakit.egg-info/entry_points.txt
+-rw-r--r--   0 eshajoshi   (501) staff       (20)        1 2023-11-29 04:33:12.000000 seqerakit-0.4.8/seqerakit.egg-info/not-zip-safe
+-rw-r--r--   0 eshajoshi   (501) staff       (20)       14 2024-05-02 02:19:48.000000 seqerakit-0.4.8/seqerakit.egg-info/requires.txt
+-rw-r--r--   0 eshajoshi   (501) staff       (20)       10 2024-05-02 02:19:48.000000 seqerakit-0.4.8/seqerakit.egg-info/top_level.txt
+-rw-r--r--   0 eshajoshi   (501) staff       (20)       38 2024-05-02 02:19:48.180529 seqerakit-0.4.8/setup.cfg
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      964 2024-05-02 02:18:19.000000 seqerakit-0.4.8/setup.py
+drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-05-02 02:19:48.178539 seqerakit-0.4.8/templates/
+-rw-r--r--   0 eshajoshi   (501) staff       (20)     1540 2024-05-02 02:18:19.000000 seqerakit-0.4.8/templates/actions.yml
+-rw-r--r--   0 eshajoshi   (501) staff       (20)     2847 2024-05-02 02:18:19.000000 seqerakit-0.4.8/templates/compute-envs.yml
+-rw-r--r--   0 eshajoshi   (501) staff       (20)     2163 2024-05-02 02:18:19.000000 seqerakit-0.4.8/templates/credentials.yml
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      419 2023-10-13 03:44:10.000000 seqerakit-0.4.8/templates/datasets.yml
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      310 2024-05-02 02:18:19.000000 seqerakit-0.4.8/templates/labels.yml
+-rw-r--r--   0 eshajoshi   (501) staff       (20)     1394 2024-05-02 02:18:19.000000 seqerakit-0.4.8/templates/launch.yml
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      266 2024-05-02 02:18:19.000000 seqerakit-0.4.8/templates/members.yml
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      405 2023-10-13 03:44:10.000000 seqerakit-0.4.8/templates/organizations.yml
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      541 2024-03-20 19:32:10.000000 seqerakit-0.4.8/templates/participants.yml
+-rw-r--r--   0 eshajoshi   (501) staff       (20)     1478 2024-05-02 02:18:19.000000 seqerakit-0.4.8/templates/pipelines.yml
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      303 2023-10-13 03:44:10.000000 seqerakit-0.4.8/templates/secrets.yml
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      341 2023-10-13 03:44:10.000000 seqerakit-0.4.8/templates/teams.yml
+-rw-r--r--   0 eshajoshi   (501) staff       (20)      375 2023-10-13 03:44:10.000000 seqerakit-0.4.8/templates/workspaces.yml
+drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-05-02 02:19:48.164933 seqerakit-0.4.8/tests/
+drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-05-02 02:19:48.178764 seqerakit-0.4.8/tests/e2e/
+-rw-r--r--   0 eshajoshi   (501) staff       (20)     2735 2024-05-02 02:18:19.000000 seqerakit-0.4.8/tests/e2e/aws-e2e.yml
+drwxr-xr-x   0 eshajoshi   (501) staff       (20)        0 2024-05-02 02:19:48.179440 seqerakit-0.4.8/tests/unit/
+-rw-r--r--   0 eshajoshi   (501) staff       (20)       25 2024-02-28 20:36:16.000000 seqerakit-0.4.8/tests/unit/__init__.py
+-rw-r--r--   0 eshajoshi   (501) staff       (20)    13003 2024-05-02 02:18:19.000000 seqerakit-0.4.8/tests/unit/test_helper.py
+-rw-r--r--   0 eshajoshi   (501) staff       (20)     8359 2024-05-02 02:18:19.000000 seqerakit-0.4.8/tests/unit/test_seqeraplatform.py
+-rw-r--r--   0 eshajoshi   (501) staff       (20)     5835 2023-10-13 03:44:10.000000 seqerakit-0.4.8/tests/unit/test_subcommands.py
```

### Comparing `seqerakit-0.4.7/.github/CONTRIBUTING.md` & `seqerakit-0.4.8/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.7/.github/workflows/e2e-testing.yml` & `seqerakit-0.4.8/.github/workflows/e2e-testing.yml`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.7/.github/workflows/python-testing.yml` & `seqerakit-0.4.8/.github/workflows/python-testing.yml`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.7/.github/workflows/teardown.yml` & `seqerakit-0.4.8/.github/workflows/teardown.yml`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.7/.pre-commit-config.yaml` & `seqerakit-0.4.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.7/LICENSE.txt` & `seqerakit-0.4.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.7/PKG-INFO` & `seqerakit-0.4.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: seqerakit
-Version: 0.4.7
+Version: 0.4.8
 Summary: Automate creation of Seqera Platform resources
 Home-page: https://github.com/seqeralabs/seqera-kit
 Author: Esha Joshi, Adam Talbot, Harshil Patel
 Author-email: esha.joshi@seqera.io, adam.talbot@seqera.io, harshil.patel@seqera.io
 License: Apache 2.0
 Keywords: nextflow,bioinformatics,workflow,pipeline,seqera-platform,seqera
 Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pyyaml>=6.0.0
 
-# <img src="https://raw.githubusercontent.com/seqeralabs/seqera-kit/main/assets/seqerakit.svg" width=50 alt="seqerakit logo"> seqerakit
-
+# <img src="assets/seqerakit.svg" width=50 alt="seqerakit logo"> seqerakit
 
 `seqerakit` is a Python wrapper for the [Seqera Platform CLI](https://github.com/seqeralabs/tower-cli). It can be leveraged to automate the creation of all of the entities in Seqera Platform via a simple configuration file in YAML format.
 
 The key features are:
 
 - **Simple configuration**: All of the command-line options available when using the Seqera Platform CLI can be defined in simple YAML format.
 - **Infrastructure as Code**: Enable users to manage and provision their infrastructure specifications.
```

### Comparing `seqerakit-0.4.7/README.md` & `seqerakit-0.4.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-# <img src="https://raw.githubusercontent.com/seqeralabs/seqera-kit/main/assets/seqerakit.svg" width=50 alt="seqerakit logo"> seqerakit
-
+# <img src="assets/seqerakit.svg" width=50 alt="seqerakit logo"> seqerakit
 
 `seqerakit` is a Python wrapper for the [Seqera Platform CLI](https://github.com/seqeralabs/tower-cli). It can be leveraged to automate the creation of all of the entities in Seqera Platform via a simple configuration file in YAML format.
 
 The key features are:
 
 - **Simple configuration**: All of the command-line options available when using the Seqera Platform CLI can be defined in simple YAML format.
 - **Infrastructure as Code**: Enable users to manage and provision their infrastructure specifications.
```

### Comparing `seqerakit-0.4.7/assets/seqerakit.svg` & `seqerakit-0.4.8/assets/seqerakit.svg`

 * *Files 11% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 00000040: 6964 7468 3d22 3438 220a 2020 2068 6569  idth="48".   hei
 00000050: 6768 743d 2234 3822 0a20 2020 7669 6577  ght="48".   view
 00000060: 426f 783d 2230 2030 2034 382e 3030 3030  Box="0 0 48.0000
 00000070: 3031 2034 3822 0a20 2020 6669 6c6c 3d22  01 48".   fill="
 00000080: 6e6f 6e65 220a 2020 2076 6572 7369 6f6e  none".   version
 00000090: 3d22 312e 3122 0a20 2020 6964 3d22 7376  ="1.1".   id="sv
 000000a0: 6734 220a 2020 2073 6f64 6970 6f64 693a  g4".   sodipodi:
-000000b0: 646f 636e 616d 653d 2273 656b 6572 616b  docname="sekerak
+000000b0: 646f 636e 616d 653d 2273 6571 6572 616b  docname="seqerak
 000000c0: 6974 2e73 7667 220a 2020 2069 6e6b 7363  it.svg".   inksc
 000000d0: 6170 653a 7665 7273 696f 6e3d 2231 2e33  ape:version="1.3
 000000e0: 2e32 2028 313a 312e 332e 322b 3230 3233  .2 (1:1.3.2+2023
 000000f0: 3131 3235 3231 3530 2b30 3931 6532 3065  11252150+091e20e
 00000100: 6630 6629 220a 2020 2078 6d6c 3a73 7061  f0f)".   xml:spa
 00000110: 6365 3d22 7072 6573 6572 7665 220a 2020  ce="preserve".  
 00000120: 2069 6e6b 7363 6170 653a 6578 706f 7274   inkscape:export
-00000130: 2d66 696c 656e 616d 653d 2273 656b 6572  -filename="seker
+00000130: 2d66 696c 656e 616d 653d 2273 6571 6572  -filename="seqer
 00000140: 616b 6974 2e70 6e67 220a 2020 2069 6e6b  akit.png".   ink
 00000150: 7363 6170 653a 6578 706f 7274 2d78 6470  scape:export-xdp
 00000160: 693d 2238 3530 2e30 3530 3438 220a 2020  i="850.05048".  
 00000170: 2069 6e6b 7363 6170 653a 6578 706f 7274   inkscape:export
 00000180: 2d79 6470 693d 2238 3530 2e30 3530 3438  -ydpi="850.05048
 00000190: 220a 2020 2078 6d6c 6e73 3a69 6e6b 7363  ".   xmlns:inksc
 000001a0: 6170 653d 2268 7474 703a 2f2f 7777 772e  ape="http://www.
@@ -50,913 +50,893 @@
 00000310: 6167 656f 7061 6369 7479 3d22 302e 3022  ageopacity="0.0"
 00000320: 0a20 2020 2020 696e 6b73 6361 7065 3a70  .     inkscape:p
 00000330: 6167 6563 6865 636b 6572 626f 6172 643d  agecheckerboard=
 00000340: 2230 220a 2020 2020 2069 6e6b 7363 6170  "0".     inkscap
 00000350: 653a 6465 736b 636f 6c6f 723d 2223 6431  e:deskcolor="#d1
 00000360: 6431 6431 220a 2020 2020 2069 6e6b 7363  d1d1".     inksc
 00000370: 6170 653a 7a6f 6f6d 3d22 392e 3236 3034  ape:zoom="9.2604
-00000380: 3136 3822 0a20 2020 2020 696e 6b73 6361  168".     inksca
-00000390: 7065 3a63 783d 2231 372e 3338 3538 3237  pe:cx="17.385827
+00000380: 3136 3922 0a20 2020 2020 696e 6b73 6361  169".     inksca
+00000390: 7065 3a63 783d 2232 2e39 3639 3632 3837  pe:cx="2.9696287
 000003a0: 220a 2020 2020 2069 6e6b 7363 6170 653a  ".     inkscape:
-000003b0: 6379 3d22 3232 2e36 3233 3137 3222 0a20  cy="22.623172". 
-000003c0: 2020 2020 696e 6b73 6361 7065 3a77 696e      inkscape:win
-000003d0: 646f 772d 7769 6474 683d 2231 3932 3022  dow-width="1920"
-000003e0: 0a20 2020 2020 696e 6b73 6361 7065 3a77  .     inkscape:w
-000003f0: 696e 646f 772d 6865 6967 6874 3d22 3131  indow-height="11
-00000400: 3238 220a 2020 2020 2069 6e6b 7363 6170  28".     inkscap
-00000410: 653a 7769 6e64 6f77 2d78 3d22 3022 0a20  e:window-x="0". 
-00000420: 2020 2020 696e 6b73 6361 7065 3a77 696e      inkscape:win
-00000430: 646f 772d 793d 2230 220a 2020 2020 2069  dow-y="0".     i
-00000440: 6e6b 7363 6170 653a 7769 6e64 6f77 2d6d  nkscape:window-m
-00000450: 6178 696d 697a 6564 3d22 3122 0a20 2020  aximized="1".   
-00000460: 2020 696e 6b73 6361 7065 3a63 7572 7265    inkscape:curre
-00000470: 6e74 2d6c 6179 6572 3d22 7376 6734 220a  nt-layer="svg4".
-00000480: 2020 2020 2069 6e6b 7363 6170 653a 6578       inkscape:ex
-00000490: 706f 7274 2d62 6763 6f6c 6f72 3d22 2366  port-bgcolor="#f
-000004a0: 6666 6666 6630 3022 0a20 2020 2020 7368  fffff00".     sh
-000004b0: 6f77 6772 6964 3d22 6661 6c73 6522 202f  owgrid="false" /
-000004c0: 3e3c 6465 6673 0a20 2020 2020 6964 3d22  ><defs.     id="
-000004d0: 6465 6673 3422 3e3c 636c 6970 5061 7468  defs4"><clipPath
-000004e0: 0a20 2020 2020 2020 636c 6970 5061 7468  .       clipPath
-000004f0: 556e 6974 733d 2275 7365 7253 7061 6365  Units="userSpace
-00000500: 4f6e 5573 6522 0a20 2020 2020 2020 6964  OnUse".       id
-00000510: 3d22 636c 6970 5061 7468 3522 3e3c 670a  ="clipPath5"><g.
-00000520: 2020 2020 2020 2020 2069 643d 2267 3622           id="g6"
-00000530: 3e3c 7265 6374 0a20 2020 2020 2020 2020  ><rect.         
-00000540: 2020 7769 6474 683d 2234 3822 0a20 2020    width="48".   
-00000550: 2020 2020 2020 2020 6865 6967 6874 3d22          height="
-00000560: 3438 220a 2020 2020 2020 2020 2020 2066  48".           f
-00000570: 696c 6c3d 2223 6666 6666 6666 220a 2020  ill="#ffffff".  
-00000580: 2020 2020 2020 2020 2069 643d 2272 6563           id="rec
-00000590: 7435 220a 2020 2020 2020 2020 2020 2078  t5".           x
-000005a0: 3d22 3022 0a20 2020 2020 2020 2020 2020  ="0".           
-000005b0: 793d 2230 2220 2f3e 3c2f 673e 3c2f 636c  y="0" /></g></cl
-000005c0: 6970 5061 7468 3e3c 636c 6970 5061 7468  ipPath><clipPath
-000005d0: 0a20 2020 2020 2020 636c 6970 5061 7468  .       clipPath
-000005e0: 556e 6974 733d 2275 7365 7253 7061 6365  Units="userSpace
-000005f0: 4f6e 5573 6522 0a20 2020 2020 2020 6964  OnUse".       id
-00000600: 3d22 636c 6970 5061 7468 3622 3e3c 670a  ="clipPath6"><g.
-00000610: 2020 2020 2020 2020 2069 643d 2267 3722           id="g7"
-00000620: 3e3c 7265 6374 0a20 2020 2020 2020 2020  ><rect.         
-00000630: 2020 7769 6474 683d 2234 3822 0a20 2020    width="48".   
-00000640: 2020 2020 2020 2020 6865 6967 6874 3d22          height="
-00000650: 3438 220a 2020 2020 2020 2020 2020 2066  48".           f
-00000660: 696c 6c3d 2223 6666 6666 6666 220a 2020  ill="#ffffff".  
-00000670: 2020 2020 2020 2020 2069 643d 2272 6563           id="rec
-00000680: 7436 220a 2020 2020 2020 2020 2020 2078  t6".           x
-00000690: 3d22 3022 0a20 2020 2020 2020 2020 2020  ="0".           
-000006a0: 793d 2230 2220 2f3e 3c2f 673e 3c2f 636c  y="0" /></g></cl
-000006b0: 6970 5061 7468 3e3c 636c 6970 5061 7468  ipPath><clipPath
-000006c0: 0a20 2020 2020 2020 636c 6970 5061 7468  .       clipPath
-000006d0: 556e 6974 733d 2275 7365 7253 7061 6365  Units="userSpace
-000006e0: 4f6e 5573 6522 0a20 2020 2020 2020 6964  OnUse".       id
-000006f0: 3d22 636c 6970 5061 7468 3722 3e3c 670a  ="clipPath7"><g.
-00000700: 2020 2020 2020 2020 2069 643d 2267 3822           id="g8"
-00000710: 3e3c 7265 6374 0a20 2020 2020 2020 2020  ><rect.         
-00000720: 2020 7769 6474 683d 2234 3822 0a20 2020    width="48".   
-00000730: 2020 2020 2020 2020 6865 6967 6874 3d22          height="
-00000740: 3438 220a 2020 2020 2020 2020 2020 2066  48".           f
-00000750: 696c 6c3d 2223 6666 6666 6666 220a 2020  ill="#ffffff".  
-00000760: 2020 2020 2020 2020 2069 643d 2272 6563           id="rec
-00000770: 7437 220a 2020 2020 2020 2020 2020 2078  t7".           x
-00000780: 3d22 3022 0a20 2020 2020 2020 2020 2020  ="0".           
-00000790: 793d 2230 2220 2f3e 3c2f 673e 3c2f 636c  y="0" /></g></cl
-000007a0: 6970 5061 7468 3e3c 636c 6970 5061 7468  ipPath><clipPath
-000007b0: 0a20 2020 2020 2020 636c 6970 5061 7468  .       clipPath
-000007c0: 556e 6974 733d 2275 7365 7253 7061 6365  Units="userSpace
-000007d0: 4f6e 5573 6522 0a20 2020 2020 2020 6964  OnUse".       id
-000007e0: 3d22 636c 6970 5061 7468 3822 3e3c 670a  ="clipPath8"><g.
-000007f0: 2020 2020 2020 2020 2069 643d 2267 3922           id="g9"
-00000800: 3e3c 7265 6374 0a20 2020 2020 2020 2020  ><rect.         
-00000810: 2020 7769 6474 683d 2234 3822 0a20 2020    width="48".   
-00000820: 2020 2020 2020 2020 6865 6967 6874 3d22          height="
-00000830: 3438 220a 2020 2020 2020 2020 2020 2066  48".           f
-00000840: 696c 6c3d 2223 6666 6666 6666 220a 2020  ill="#ffffff".  
-00000850: 2020 2020 2020 2020 2069 643d 2272 6563           id="rec
-00000860: 7438 220a 2020 2020 2020 2020 2020 2078  t8".           x
-00000870: 3d22 3022 0a20 2020 2020 2020 2020 2020  ="0".           
-00000880: 793d 2230 2220 2f3e 3c2f 673e 3c2f 636c  y="0" /></g></cl
-00000890: 6970 5061 7468 3e3c 636c 6970 5061 7468  ipPath><clipPath
-000008a0: 0a20 2020 2020 2020 6964 3d22 636c 6970  .       id="clip
-000008b0: 305f 3933 345f 3934 3933 223e 3c72 6563  0_934_9493"><rec
-000008c0: 740a 2020 2020 2020 2020 2077 6964 7468  t.         width
-000008d0: 3d22 3235 3022 0a20 2020 2020 2020 2020  ="250".         
-000008e0: 6865 6967 6874 3d22 3235 3022 0a20 2020  height="250".   
-000008f0: 2020 2020 2020 6669 6c6c 3d22 2366 6666        fill="#fff
-00000900: 6666 6622 0a20 2020 2020 2020 2020 6964  fff".         id
-00000910: 3d22 7265 6374 382d 3322 0a20 2020 2020  ="rect8-3".     
-00000920: 2020 2020 783d 2230 220a 2020 2020 2020      x="0".      
-00000930: 2020 2079 3d22 3022 202f 3e3c 2f63 6c69     y="0" /></cli
-00000940: 7050 6174 683e 3c2f 6465 6673 3e3c 7061  pPath></defs><pa
-00000950: 7468 0a20 2020 2020 6964 3d22 7061 7468  th.     id="path
-00000960: 3122 0a20 2020 2020 7374 796c 653d 2266  1".     style="f
-00000970: 696c 6c3a 2366 6666 6666 663b 7374 726f  ill:#ffffff;stro
-00000980: 6b65 2d77 6964 7468 3a31 2e31 3333 3835  ke-width:1.13385
-00000990: 3832 373b 7374 726f 6b65 3a23 6666 6666  827;stroke:#ffff
-000009a0: 6666 3b73 7472 6f6b 652d 6461 7368 6172  ff;stroke-dashar
-000009b0: 7261 793a 6e6f 6e65 220a 2020 2020 2064  ray:none".     d
-000009c0: 3d22 4d20 3239 2e38 3732 3333 2c31 2e31  ="M 29.87233,1.1
-000009d0: 3937 3236 3536 2032 392e 3432 3131 3538  972656 29.421158
-000009e0: 2c31 2e32 3138 3735 2063 202d 302e 3539  ,1.21875 c -0.59
-000009f0: 3832 3535 2c30 2e30 3330 3334 3820 2d31  8255,0.030348 -1
-00000a00: 2e33 3434 3132 392c 302e 3330 3937 3737  .344129,0.309777
-00000a10: 202d 322e 3231 3438 3434 2c30 2e38 3238   -2.214844,0.828
-00000a20: 3132 3520 6c20 2d30 2e37 3130 3933 372c  125 l -0.710937,
-00000a30: 302e 3432 3338 3238 3120 2d30 2e38 3830  0.4238281 -0.880
-00000a40: 3835 392c 302e 3737 3733 3433 3820 2d30  859,0.7773438 -0
-00000a50: 2e38 3832 3831 332c 302e 3737 3733 3433  .882813,0.777343
-00000a60: 3720 2d30 2e33 3531 3536 332c 302e 3435  7 -0.351563,0.45
-00000a70: 3331 3235 2063 202d 302e 3630 3339 3239  3125 c -0.603929
-00000a80: 2c30 2e37 3737 3337 3135 202d 302e 3731  ,0.7773715 -0.71
-00000a90: 3735 3239 2c31 2e36 3030 3230 3735 202d  7529,1.6002075 -
-00000aa0: 302e 3333 3030 3738 2c32 2e33 3733 3034  0.330078,2.37304
-00000ab0: 3639 2030 2e32 3530 3238 372c 302e 3439  69 0.250287,0.49
-00000ac0: 3932 3338 2030 2e32 3334 3539 322c 302e  9238 0.234592,0.
-00000ad0: 3632 3537 3836 3320 2d30 2e31 3636 3031  6257863 -0.16601
-00000ae0: 352c 312e 3430 3233 3433 3720 2d31 2e39  5,1.4023437 -1.9
-00000af0: 3934 3836 312c 332e 3836 3639 3331 3820  94861,3.8669318 
-00000b00: 2d31 2e32 3430 3433 372c 362e 3433 3034  -1.240437,6.4304
-00000b10: 3433 3820 322e 3634 3235 3738 2c38 2e39  438 2.642578,8.9
-00000b20: 3836 3332 3738 206c 2031 2e30 3636 3430  863278 l 1.06640
-00000b30: 362c 302e 3730 3331 3235 2030 2e33 3832  6,0.703125 0.382
-00000b40: 3831 332c 302e 3435 3131 3732 2030 2e33  813,0.451172 0.3
-00000b50: 3834 3736 352c 302e 3435 3331 3235 2030  84765,0.453125 0
-00000b60: 2e31 3338 3637 322c 302e 3338 3437 3636  .138672,0.384766
-00000b70: 2063 2030 2e30 3736 3533 2c30 2e32 3132   c 0.07653,0.212
-00000b80: 3237 3220 302e 3132 3336 3039 2c30 2e35  272 0.123609,0.5
-00000b90: 3738 3739 3220 302e 3130 3534 3639 2c30  78792 0.105469,0
-00000ba0: 2e38 3132 3520 6c20 2d30 2e30 3333 322c  .8125 l -0.0332,
-00000bb0: 302e 3432 3338 3238 202d 302e 3231 3238  0.423828 -0.2128
-00000bc0: 3931 2c30 2e33 3437 3635 3620 6320 2d30  91,0.347656 c -0
-00000bd0: 2e32 3036 3330 322c 302e 3333 3635 3239  .206302,0.336529
-00000be0: 202d 302e 3439 3536 3039 2c30 2e35 3731   -0.495609,0.571
-00000bf0: 3133 3620 2d30 2e38 3333 3938 342c 302e  136 -0.833984,0.
-00000c00: 3730 3530 3738 202d 302e 3030 3139 2c37  705078 -0.0019,7
-00000c10: 2e35 3565 2d34 202d 302e 3030 342c 302e  .55e-4 -0.004,0.
-00000c20: 3030 3132 202d 302e 3030 3539 2c30 2e30  0012 -0.0059,0.0
-00000c30: 3032 202d 302e 3237 3138 3837 2c30 2e31  02 -0.271887,0.1
-00000c40: 3036 3933 3220 2d30 2e35 3735 3737 352c  06932 -0.575775,
-00000c50: 302e 3134 3533 3520 2d30 2e38 3934 3533  0.14535 -0.89453
-00000c60: 312c 302e 3131 3731 3837 202d 302e 3039  1,0.117187 -0.09
-00000c70: 3133 382c 2d30 2e30 3038 3120 2d30 2e31  138,-0.0081 -0.1
-00000c80: 3833 3836 382c 2d30 2e30 3233 3439 202d  83868,-0.02349 -
-00000c90: 302e 3237 3733 3434 2c2d 302e 3034 3239  0.277344,-0.0429
-00000ca0: 3720 2d30 2e30 3331 3234 2c2d 302e 3030  7 -0.03124,-0.00
-00000cb0: 3635 202d 302e 3036 3233 332c 2d30 2e30  65 -0.06233,-0.0
-00000cc0: 3039 3820 2d30 2e30 3933 3735 2c2d 302e  098 -0.09375,-0.
-00000cd0: 3031 3735 3820 2d30 2e31 3135 3533 362c  01758 -0.115536,
-00000ce0: 2d30 2e30 3238 3637 202d 302e 3233 3236  -0.02867 -0.2326
-00000cf0: 3134 2c2d 302e 3036 3930 3320 2d30 2e33  14,-0.06903 -0.3
-00000d00: 3439 3630 392c 2d30 2e31 3135 3233 3420  49609,-0.115234 
-00000d10: 2d30 2e30 3431 3234 2c2d 302e 3031 3632  -0.04124,-0.0162
-00000d20: 3920 2d30 2e30 3831 3735 2c2d 302e 3033  9 -0.08175,-0.03
-00000d30: 3432 3520 2d30 2e31 3233 3034 372c 2d30  425 -0.123047,-0
-00000d40: 2e30 3532 3733 202d 302e 3132 3235 3432  .05273 -0.122542
-00000d50: 2c2d 302e 3035 3438 3620 2d30 2e32 3435  ,-0.05486 -0.245
-00000d60: 3233 322c 2d30 2e31 3135 3032 3920 2d30  232,-0.115029 -0
-00000d70: 2e33 3637 3138 372c 2d30 2e31 3839 3435  .367187,-0.18945
-00000d80: 3320 4c20 3235 2e30 3138 3737 372c 3230  3 L 25.018777,20
-00000d90: 2e39 3830 3531 3720 3234 2e32 3139 3934  .980517 24.21994
-00000da0: 392c 3230 2e31 3634 3131 2063 202d 302e  9,20.16411 c -0.
-00000db0: 3230 3432 3838 2c2d 302e 3230 3932 3332  204288,-0.209232
-00000dc0: 202d 302e 3530 3832 3235 2c2d 302e 3534   -0.508225,-0.54
-00000dd0: 3831 3934 202d 302e 3833 3339 3834 2c2d  8194 -0.833984,-
-00000de0: 302e 3932 3338 3238 202d 302e 3032 3732  0.923828 -0.0272
-00000df0: 312c 2d30 2e30 3331 3334 202d 302e 3034  1,-0.03134 -0.04
-00000e00: 3237 392c 2d30 2e30 3436 3233 202d 302e  279,-0.04623 -0.
-00000e10: 3037 3033 312c 2d30 2e30 3738 3133 202d  07031,-0.07813 -
-00000e20: 332e 3465 2d34 2c2d 332e 3934 652d 3420  3.4e-4,-3.94e-4 
-00000e30: 332e 3431 652d 342c 2d30 2e30 3031 3620  3.41e-4,-0.0016 
-00000e40: 302c 2d30 2e30 3032 202d 302e 3335 3430  0,-0.002 -0.3540
-00000e50: 3631 2c2d 302e 3431 3033 3620 2d30 2e37  61,-0.41036 -0.7
-00000e60: 3331 3538 362c 2d30 2e38 3632 3438 3920  31586,-0.862489 
-00000e70: 2d31 2e30 3438 3832 382c 2d31 2e32 3539  -1.048828,-1.259
-00000e80: 3736 3520 2d30 2e31 3433 3839 312c 2d30  765 -0.143891,-0
-00000e90: 2e31 3830 3139 3420 2d30 2e32 3835 3438  .180194 -0.28548
-00000ea0: 322c 2d30 2e33 3533 3336 3420 2d30 2e34  2,-0.353364 -0.4
-00000eb0: 3235 3738 312c 2d30 2e35 3231 3438 3520  25781,-0.521485 
-00000ec0: 2d30 2e30 3536 3738 2c2d 302e 3036 3830  -0.05678,-0.0680
-00000ed0: 3420 2d30 2e31 3133 3636 322c 2d30 2e31  4 -0.113662,-0.1
-00000ee0: 3335 3037 3220 2d30 2e31 3639 3932 322c  35072 -0.169922,
-00000ef0: 2d30 2e32 3031 3137 3220 2d30 2e34 3930  -0.201172 -0.490
-00000f00: 3131 372c 2d30 2e35 3735 3834 3320 2d30  117,-0.575843 -0
-00000f10: 2e39 3632 3338 342c 2d31 2e30 3738 3033  .962384,-1.07803
-00000f20: 3320 2d31 2e34 3235 3738 312c 2d31 2e35  3 -1.425781,-1.5
-00000f30: 3133 3637 3220 2d30 2e30 3138 3939 2c2d  13672 -0.01899,-
-00000f40: 302e 3031 3738 3520 2d30 2e30 3337 3938  0.01785 -0.03798
-00000f50: 2c2d 302e 3033 3530 3220 2d30 2e30 3536  ,-0.03502 -0.056
-00000f60: 3634 2c2d 302e 3035 3237 3320 2d30 2e33  64,-0.05273 -0.3
-00000f70: 3033 3535 382c 2d30 2e32 3832 3135 3120  03558,-0.282151 
-00000f80: 2d30 2e36 3033 3336 372c 2d30 2e35 3336  -0.603367,-0.536
-00000f90: 3935 3120 2d30 2e39 3034 3239 372c 2d30  951 -0.904297,-0
-00000fa0: 2e37 3633 3637 3220 2d30 2e30 3034 352c  .763672 -0.0045,
-00000fb0: 2d30 2e30 3033 3420 2d30 2e30 3039 322c  -0.0034 -0.0092,
-00000fc0: 2d30 2e30 3036 3420 2d30 2e30 3133 3637  -0.0064 -0.01367
-00000fd0: 2c2d 302e 3030 3938 202d 302e 3137 3534  ,-0.0098 -0.1754
-00000fe0: 3333 2c2d 302e 3133 3137 3031 202d 302e  33,-0.131701 -0.
-00000ff0: 3335 3039 372c 2d30 2e32 3535 3236 3620  35097,-0.255266 
-00001000: 2d30 2e35 3237 3334 342c 2d30 2e33 3639  -0.527344,-0.369
-00001010: 3134 3120 2d30 2e33 3132 3635 392c 2d30  141 -0.312659,-0
-00001020: 2e32 3031 3836 3620 2d30 2e36 3237 3832  .201866 -0.62782
-00001030: 372c 2d30 2e33 3736 3335 3820 2d30 2e39  7,-0.376358 -0.9
-00001040: 3439 3231 392c 2d30 2e35 3235 3339 3120  49219,-0.525391 
-00001050: 2d30 2e31 3632 3133 372c 2d30 2e30 3735  -0.162137,-0.075
-00001060: 3138 202d 302e 3332 3634 3134 2c2d 302e  18 -0.326414,-0.
-00001070: 3134 3235 3620 2d30 2e34 3932 3138 372c  14256 -0.492187,
-00001080: 2d30 2e32 3035 3037 3820 2d30 2e30 3434  -0.205078 -0.044
-00001090: 3833 2c2d 302e 3031 3639 202d 302e 3038  83,-0.0169 -0.08
-000010a0: 3936 332c 2d30 2e30 3334 3738 202d 302e  963,-0.03478 -0.
-000010b0: 3133 3437 3636 2c2d 302e 3035 3037 3820  134766,-0.05078 
-000010c0: 2d30 2e30 3033 332c 2d30 2e30 3031 3220  -0.0033,-0.0012 
-000010d0: 2d30 2e30 3036 352c 2d30 2e30 3032 3720  -0.0065,-0.0027 
-000010e0: 2d30 2e30 3039 382c 2d30 2e30 3033 3920  -0.0098,-0.0039 
-000010f0: 2d30 2e38 3630 3434 332c 2d30 2e33 3033  -0.860443,-0.303
-00001100: 3632 3620 2d31 2e37 3737 3838 322c 2d30  626 -1.777882,-0
-00001110: 2e34 3435 3939 202d 322e 3832 3032 3436  .44599 -2.820246
-00001120: 2c2d 302e 3435 3839 3537 202d 302e 3231  ,-0.458957 -0.21
-00001130: 3137 3536 2c2d 302e 3030 3236 202d 302e  1756,-0.0026 -0.
-00001140: 3432 3938 3534 2c32 2e32 652d 3420 2d30  429854,2.2e-4 -0
-00001150: 2e36 3532 3334 342c 302e 3030 3738 206c  .652344,0.0078 l
-00001160: 202d 302e 3833 3539 3337 2c30 2e30 3239   -0.835937,0.029
-00001170: 3320 2d30 2e36 3831 3634 312c 302e 3231  3 -0.681641,0.21
-00001180: 3637 3937 2063 202d 302e 3832 3736 3837  6797 c -0.827687
-00001190: 2c30 2e32 3634 3338 3520 2d31 2e33 3331  ,0.264385 -1.331
-000011a0: 3039 322c 302e 3533 3738 3033 202d 322e  092,0.537803 -2.
-000011b0: 3034 3638 3735 2c31 2e31 3039 3337 3520  046875,1.109375 
-000011c0: 6c20 2d30 2e35 3432 3936 392c 302e 3433  l -0.542969,0.43
-000011d0: 3335 3920 2d30 2e34 3134 3036 322c 302e  359 -0.414062,0.
-000011e0: 3531 3137 3139 2063 202d 312e 3832 3631  511719 c -1.8261
-000011f0: 3037 2c32 2e32 3632 3333 3720 2d32 2e30  07,2.262337 -2.0
-00001200: 3536 3232 372c 352e 3132 3831 3820 2d30  56227,5.12818 -0
-00001210: 2e36 3031 3536 332c 372e 3439 3830 3620  .601563,7.49806 
-00001220: 6c20 302e 3239 3638 3735 2c30 2e34 3832  l 0.296875,0.482
-00001230: 3432 3220 302e 3630 3534 3639 2c30 2e36  422 0.605469,0.6
-00001240: 3037 3432 3220 6320 312e 3331 3439 3431  07422 c 1.314941
-00001250: 2c31 2e33 3231 3838 2032 2e38 3535 3539  ,1.32188 2.85559
-00001260: 382c 322e 3130 3833 3936 2035 2e38 3930  8,2.108396 5.890
-00001270: 3632 352c 332e 3030 3139 3533 2037 2e32  625,3.001953 7.2
-00001280: 3538 332c 322e 3133 3639 3532 2039 2e32  583,2.136952 9.2
-00001290: 3731 3837 312c 332e 3537 3735 3639 2038  71871,3.577569 8
-000012a0: 2e34 3630 3933 372c 362e 3035 3436 3837  .460937,6.054687
-000012b0: 206c 202d 302e 3134 3036 3235 2c30 2e34   l -0.140625,0.4
-000012c0: 3331 3634 3120 2d30 2e33 3034 3638 372c  31641 -0.304687,
-000012d0: 302e 3336 3532 3334 202d 302e 3330 3436  0.365234 -0.3046
-000012e0: 3838 2c30 2e33 3635 3233 3520 2d30 2e33  88,0.365235 -0.3
-000012f0: 3431 3739 372c 302e 3135 3233 3434 2063  41797,0.152344 c
-00001300: 202d 312e 3337 3035 3036 2c30 2e36 3132   -1.370506,0.612
-00001310: 3939 3120 2d32 2e36 3535 3639 352c 2d30  991 -2.655695,-0
-00001320: 2e30 3130 3133 202d 352e 3533 3332 3033  .01013 -5.533203
-00001330: 2c2d 322e 3638 3136 3431 206c 202d 312e  ,-2.681641 l -1.
-00001340: 3535 3636 342c 2d31 2e34 3435 3331 3320  55664,-1.445313 
-00001350: 2d30 2e35 3937 3635 362c 2d30 2e34 3134  -0.597656,-0.414
-00001360: 3036 3220 4320 3132 2e39 3239 3630 372c  062 C 12.929607,
-00001370: 3238 2e34 3834 3834 3920 3131 2e31 3831  28.484849 11.181
-00001380: 3238 322c 3237 2e39 3831 3638 3120 392e  282,27.981681 9.
-00001390: 3736 3638 3631 2c32 382e 3433 3535 3437  766861,28.435547
-000013a0: 206c 202d 302e 3339 3235 3738 2c30 2e31   l -0.392578,0.1
-000013b0: 3235 202d 302e 3436 3438 3434 2c30 2e34  25 -0.464844,0.4
-000013c0: 3132 3130 3920 2d30 2e34 3632 3839 2c30  12109 -0.46289,0
-000013d0: 2e34 3132 3131 202d 302e 3234 3431 3431  .41211 -0.244141
-000013e0: 2c30 2e34 3339 3435 3320 6320 2d30 2e36  ,0.439453 c -0.6
-000013f0: 3739 3936 342c 312e 3233 3137 3433 202d  79964,1.231743 -
-00001400: 302e 3632 3930 3935 2c32 2e34 3237 3939  0.629095,2.42799
-00001410: 3820 302e 3135 3832 3033 2c33 2e37 3334  8 0.158203,3.734
-00001420: 3337 3520 6c20 302e 3237 3533 3931 2c30  375 l 0.275391,0
-00001430: 2e34 3537 3033 3120 312e 3330 3835 3934  .457031 1.308594
-00001440: 2c31 2e34 3032 3334 3420 312e 3331 3035  ,1.402344 1.3105
-00001450: 3437 2c31 2e34 3034 3239 3720 302e 3234  47,1.404297 0.24
-00001460: 3431 342c 302e 3437 3635 3632 2063 2030  414,0.476562 c 0
-00001470: 2e38 3037 3739 372c 312e 3537 3835 3431  .807797,1.578541
-00001480: 2030 2e35 3437 3633 392c 332e 3437 3033   0.547639,3.4703
-00001490: 3239 202d 302e 3831 3833 3539 2c35 2e39  29 -0.818359,5.9
-000014a0: 3333 3539 3420 2d30 2e35 3739 3737 372c  33594 -0.579777,
-000014b0: 312e 3034 3534 3937 202d 302e 3535 3833  1.045497 -0.5583
-000014c0: 392c 312e 3133 3036 3536 2030 2e31 3139  9,1.130656 0.119
-000014d0: 3134 2c30 2e34 3533 3132 3520 302e 3933  14,0.453125 0.93
-000014e0: 3530 392c 2d30 2e39 3335 3039 2031 2e36  509,-0.93509 1.6
-000014f0: 3132 3332 342c 2d32 2e30 3337 3539 3620  12324,-2.037596 
-00001500: 322e 3037 3033 3133 2c2d 332e 3337 3330  2.070313,-3.3730
-00001510: 3437 206c 2030 2e32 352c 2d30 2e37 3330  47 l 0.25,-0.730
-00001520: 3436 3920 302e 3030 322c 2d30 2e38 3731  469 0.002,-0.871
-00001530: 3039 3320 302e 3030 3139 2c2d 302e 3837  093 0.0019,-0.87
-00001540: 3130 3934 202d 302e 3232 3635 3633 2c2d  1094 -0.226563,-
-00001550: 302e 3639 3732 3636 2043 2031 322e 3533  0.697266 C 12.53
-00001560: 3530 3332 2c33 362e 3032 3731 3639 2031  5032,36.027169 1
-00001570: 322e 3237 3138 3937 2c33 352e 3631 3233  2.271897,35.6123
-00001580: 3620 3130 2e39 3235 3036 342c 3334 2e30  6 10.925064,34.0
-00001590: 3335 3135 3620 392e 3635 3439 3333 2c33  35156 9.654933,3
-000015a0: 322e 3534 3737 3735 2039 2e34 3835 3336  2.547775 9.48536
-000015b0: 362c 3332 2e32 3138 3939 2039 2e35 3931  6,32.21899 9.591
-000015c0: 3038 2c33 312e 3433 3335 3934 206c 2030  08,31.433594 l 0
-000015d0: 2e30 3530 3738 2c2d 302e 3337 3520 302e  .05078,-0.375 0.
-000015e0: 3330 3835 3934 2c2d 302e 3335 3534 3639  308594,-0.355469
-000015f0: 2030 2e33 3036 3634 2c2d 302e 3335 3534   0.30664,-0.3554
-00001600: 3639 2030 2e34 3034 3239 372c 2d30 2e30  69 0.404297,-0.0
-00001610: 3237 3334 2063 2030 2e38 3831 3235 392c  2734 c 0.881259,
-00001620: 2d30 2e30 3537 3234 2032 2e31 3037 3739  -0.05724 2.10779
-00001630: 392c 302e 3537 3530 3437 2033 2e36 3935  9,0.575047 3.695
-00001640: 3331 332c 312e 3930 3233 3434 206c 2030  313,1.902344 l 0
-00001650: 2e37 3533 3930 362c 302e 3632 3839 3036  .753906,0.628906
-00001660: 2031 2e30 3837 3839 312c 312e 3232 3635   1.087891,1.2265
-00001670: 3633 2031 2e30 3839 3834 342c 312e 3232  63 1.089844,1.22
-00001680: 3635 3633 2030 2e36 3133 3238 312c 302e  6563 0.613281,0.
-00001690: 3437 3835 3135 2063 2032 2e35 3436 3835  478515 c 2.54685
-000016a0: 342c 312e 3938 3738 3435 2035 2e34 3437  4,1.987845 5.447
-000016b0: 3639 2c32 2e33 3436 3438 3220 372e 3338  69,2.346482 7.38
-000016c0: 3637 3139 2c30 2e39 3134 3036 3320 302e  6719,0.914063 0.
-000016d0: 3734 3739 312c 2d30 2e35 3532 3530 3620  74791,-0.552506 
-000016e0: 312e 3339 3039 3131 2c2d 312e 3439 3738  1.390911,-1.4978
-000016f0: 3433 2031 2e37 3833 3230 332c 2d32 2e36  43 1.783203,-2.6
-00001700: 3233 3034 3720 6c20 302e 3235 3339 3036  23047 l 0.253906
-00001710: 2c2d 302e 3732 3635 3633 2030 2e30 3033  ,-0.726563 0.003
-00001720: 392c 2d30 2e39 3331 3634 2030 2e30 3033  9,-0.93164 0.003
-00001730: 392c 2d30 2e39 3331 3634 3120 2d30 2e32  9,-0.931641 -0.2
-00001740: 352c 2d30 2e37 3332 3432 3220 4320 3236  5,-0.732422 C 26
-00001750: 2e39 3435 3531 372c 3330 2e33 3439 3835  .945517,30.34985
-00001760: 3520 3236 2e36 3739 362c 3239 2e37 3836  5 26.6796,29.786
-00001770: 3236 3820 3236 2e34 3931 3437 312c 3239  268 26.491471,29
-00001780: 2e34 3938 3034 3720 6c20 2d30 2e33 3433  .498047 l -0.343
-00001790: 3735 2c2d 302e 3532 3533 3931 202d 302e  75,-0.525391 -0.
-000017a0: 3935 3131 3732 2c2d 302e 3839 3435 3331  951172,-0.894531
-000017b0: 202d 302e 3935 3331 3235 2c2d 302e 3839   -0.953125,-0.89
-000017c0: 3435 3331 202d 302e 3538 3030 3738 2c2d  4531 -0.580078,-
-000017d0: 302e 3334 3537 3033 2043 2032 322e 3637  0.345703 C 22.67
-000017e0: 3932 332c 3236 2e32 3439 3436 3120 3231  923,26.249461 21
-000017f0: 2e34 3835 3236 312c 3235 2e37 3730 3539  .485261,25.77059
-00001800: 3620 3138 2e34 3434 3539 362c 3234 2e37  6 18.444596,24.7
-00001810: 3438 3034 3720 3135 2e31 3639 312c 3233  48047 15.1691,23
-00001820: 2e36 3436 3532 3620 3134 2e34 3130 3138  .646526 14.41018
-00001830: 342c 3233 2e33 3434 3039 3620 3133 2e33  4,23.344096 13.3
-00001840: 3231 3534 392c 3232 2e37 3031 3137 3220  21549,22.701172 
-00001850: 4c20 3132 2e35 3637 3634 332c 3232 2e32  L 12.567643,22.2
-00001860: 3535 3835 3920 3132 2e31 3533 3538 2c32  55859 12.15358,2
-00001870: 312e 3738 3930 3632 2031 312e 3733 3735  1.789062 11.7375
-00001880: 3634 2c32 312e 3332 3432 3139 2031 312e  64,21.324219 11.
-00001890: 3535 3938 332c 3230 2e38 3437 3635 3620  55983,20.847656 
-000018a0: 6320 2d30 2e32 3235 3338 342c 2d30 2e36  c -0.225384,-0.6
-000018b0: 3036 3031 3220 2d30 2e32 3536 3835 332c  06012 -0.256853,
-000018c0: 2d31 2e33 3837 3431 3720 2d30 2e30 3830  -1.387417 -0.080
-000018d0: 3038 2c2d 312e 3935 3530 3738 206c 2030  08,-1.955078 l 0
-000018e0: 2e31 3338 3637 322c 2d30 2e34 3433 3335  .138672,-0.44335
-000018f0: 3920 302e 3439 3032 3334 2c2d 302e 3439  9 0.490234,-0.49
-00001900: 3231 3838 2030 2e34 3930 3233 352c 2d30  2188 0.490235,-0
-00001910: 2e34 3932 3138 3720 302e 3437 3635 3632  .492187 0.476562
-00001920: 2c2d 302e 3137 3138 3735 2063 2031 2e32  ,-0.171875 c 1.2
-00001930: 3732 3331 342c 2d30 2e34 3630 3033 3420  72314,-0.460034 
-00001940: 322e 3633 3635 3938 2c2d 302e 3136 3731  2.636598,-0.1671
-00001950: 3637 2034 2e30 3832 3033 312c 302e 3836  67 4.082031,0.86
-00001960: 3931 3420 302e 3034 3830 382c 302e 3033  914 0.04808,0.03
-00001970: 3434 3720 302e 3039 3632 382c 302e 3037  447 0.09628,0.07
-00001980: 3332 3620 302e 3134 3435 3332 2c30 2e31  326 0.144532,0.1
-00001990: 3039 3337 3520 302e 3038 3131 382c 302e  09375 0.08118,0.
-000019a0: 3036 3037 3520 302e 3136 3234 3633 2c30  06075 0.162463,0
-000019b0: 2e31 3232 3130 3320 302e 3234 3431 342c  .122103 0.24414,
-000019c0: 302e 3138 3735 2030 2e30 3630 3138 2c30  0.1875 0.06018,0
-000019d0: 2e30 3438 3138 2030 2e31 3231 3139 332c  .04818 0.121193,
-000019e0: 302e 3039 3737 3320 302e 3138 3136 3431  0.09773 0.181641
-000019f0: 2c30 2e31 3438 3433 3820 302e 3037 3232  ,0.148438 0.0722
-00001a00: 362c 302e 3036 3036 3220 302e 3134 3431  6,0.06062 0.1441
-00001a10: 3439 2c30 2e31 3233 3237 3220 302e 3231  49,0.123272 0.21
-00001a20: 3637 3937 2c30 2e31 3837 3520 302e 3230  6797,0.1875 0.20
-00001a30: 3331 352c 302e 3137 3936 3038 2030 2e34  315,0.179608 0.4
-00001a40: 3037 3136 372c 302e 3337 3232 3432 2030  07167,0.372242 0
-00001a50: 2e36 3133 3238 312c 302e 3538 3030 3738  .613281,0.580078
-00001a60: 2030 2e31 3139 3730 312c 302e 3132 3037   0.119701,0.1207
-00001a70: 3032 2030 2e32 3430 3634 332c 302e 3234  02 0.240643,0.24
-00001a80: 3637 3237 2030 2e33 3631 3332 382c 302e  6727 0.361328,0.
-00001a90: 3337 3639 3533 2030 2e30 3633 3735 2c30  376953 0.06375,0
-00001aa0: 2e30 3638 3739 2030 2e31 3237 3338 362c  .06879 0.127386,
-00001ab0: 302e 3133 3934 3932 2030 2e31 3931 3430  0.139492 0.19140
-00001ac0: 362c 302e 3231 3039 3338 2030 2e32 3631  6,0.210938 0.261
-00001ad0: 3339 372c 302e 3239 3137 3135 2030 2e35  397,0.291715 0.5
-00001ae0: 3235 3135 352c 302e 3630 3334 3038 2030  25155,0.603408 0
-00001af0: 2e37 3931 3031 362c 302e 3933 3934 3533  .791016,0.939453
-00001b00: 2030 2e34 3736 3930 382c 302e 3630 3238   0.476908,0.6028
-00001b10: 3039 2031 2e32 3230 3835 322c 312e 3434  09 1.220852,1.44
-00001b20: 3932 3639 2031 2e36 3534 3239 372c 312e  9269 1.654297,1.
-00001b30: 3838 3238 3132 206c 2030 2e37 3839 3036  882812 l 0.78906
-00001b40: 322c 302e 3738 3930 3633 2030 2e37 3637  2,0.789063 0.767
-00001b50: 3537 382c 302e 3534 3239 3639 2063 2031  578,0.542969 c 1
-00001b60: 2e36 3431 3632 382c 312e 3135 3838 3039  .641628,1.158809
-00001b70: 2033 2e30 3438 3331 342c 312e 3631 3930   3.048314,1.6190
-00001b80: 3439 2034 2e37 3837 3131 2c31 2e35 3638  49 4.78711,1.568
-00001b90: 3335 3920 6c20 302e 3738 3930 3632 2c2d  359 l 0.789062,-
-00001ba0: 302e 3032 3334 3420 302e 3731 3637 3937  0.02344 0.716797
-00001bb0: 2c2d 302e 3234 3431 3420 6320 302e 3131  ,-0.24414 c 0.11
-00001bc0: 3237 3133 2c2d 302e 3033 3833 3720 302e  2713,-0.03837 0.
-00001bd0: 3231 3836 3137 2c2d 302e 3037 3836 3220  218617,-0.07862 
-00001be0: 302e 3332 3033 3133 2c2d 302e 3131 3931  0.320313,-0.1191
-00001bf0: 3431 206c 202d 302e 3030 3339 2c2d 302e  41 l -0.0039,-0.
-00001c00: 3030 3539 2063 2030 2e36 3834 3333 312c  0059 c 0.684331,
-00001c10: 2d30 2e32 3734 3231 3120 312e 3135 3730  -0.274211 1.1570
-00001c20: 3738 2c2d 302e 3631 3038 3733 2031 2e37  78,-0.610873 1.7
-00001c30: 3130 3933 382c 2d31 2e32 3334 3337 3520  10938,-1.234375 
-00001c40: 6c20 302e 3438 3832 3831 2c2d 302e 3535  l 0.488281,-0.55
-00001c50: 3037 3832 2030 2e33 3333 3938 342c 2d30  0782 0.333984,-0
-00001c60: 2e36 3733 3832 3820 6320 302e 3931 3437  .673828 c 0.9147
-00001c70: 3131 2c2d 312e 3834 3734 3138 2030 2e38  11,-1.847418 0.8
-00001c80: 3330 3039 362c 2d33 2e36 3635 3231 202d  30096,-3.66521 -
-00001c90: 302e 3235 2c2d 352e 3336 3332 3831 204c  0.25,-5.363281 L
-00001ca0: 2033 312e 3634 3936 3739 2c31 362e 3931   31.649679,16.91
-00001cb0: 3430 3139 2033 302e 3830 3339 3736 2c31  4019 30.803976,1
-00001cc0: 362e 3133 3038 3136 2032 392e 3935 3832  6.130816 29.9582
-00001cd0: 3733 2c31 352e 3334 3935 3636 2032 392e  73,15.349566 29.
-00001ce0: 3239 3432 312c 3134 2e39 3732 3631 3320  29421,14.972613 
-00001cf0: 4320 3238 2e39 3239 3036 342c 3134 2e37  C 28.929064,14.7
-00001d00: 3636 3138 2032 382e 3337 3139 3238 2c31  6618 28.371928,1
-00001d10: 342e 3436 3639 3831 2032 382e 3035 3539  4.466981 28.0559
-00001d20: 3234 2c31 342e 3330 3636 3431 2032 372e  24,14.306641 27.
-00001d30: 3733 3939 3138 2c31 342e 3134 3633 2032  739918,14.1463 2
-00001d40: 372e 3236 3136 3233 2c31 332e 3835 3839  7.261623,13.8589
-00001d50: 3936 2032 362e 3939 3334 3234 2c31 332e  96 26.993424,13.
-00001d60: 3636 3739 3639 206c 202d 302e 3438 3832  667969 l -0.4882
-00001d70: 3832 2c2d 302e 3334 3736 3537 202d 302e  82,-0.347657 -0.
-00001d80: 3233 3832 3831 2c2d 302e 3336 3731 3837  238281,-0.367187
-00001d90: 2063 202d 302e 3539 3137 3537 2c2d 302e   c -0.591757,-0.
-00001da0: 3931 3438 3636 202d 302e 3536 3235 392c  914866 -0.56259,
-00001db0: 2d32 2e33 3434 3530 3220 302e 3037 3432  -2.344502 0.0742
-00001dc0: 322c 2d33 2e37 3037 3033 3132 204c 2032  2,-3.7070312 L 2
-00001dd0: 362e 3537 3734 3038 2c38 2e37 3338 3238  6.577408,8.73828
-00001de0: 3132 2032 362e 3930 3335 382c 382e 3639  12 26.90358,8.69
-00001df0: 3533 3132 3520 4320 3237 2e30 3833 3539  53125 C 27.08359
-00001e00: 322c 382e 3637 3130 3833 3520 3237 2e34  2,8.6710835 27.4
-00001e10: 3938 3134 2c38 2e35 3535 3130 3238 2032  9814,8.5551028 2
-00001e20: 372e 3832 3335 3032 2c38 2e34 3337 3520  7.823502,8.4375 
-00001e30: 4c20 3238 2e34 3135 3239 392c 382e 3232  L 28.415299,8.22
-00001e40: 3236 3536 3220 3238 2e39 3835 3631 312c  26562 28.985611,
-00001e50: 372e 3639 3732 3635 3620 3239 2e35 3537  7.6972656 29.557
-00001e60: 3837 372c 372e 3136 3939 3231 3920 3239  877,7.1699219 29
-00001e70: 2e38 3636 3437 312c 362e 3535 3436 3837  .866471,6.554687
-00001e80: 3520 4320 3330 2e37 3938 3535 312c 342e  5 C 30.798551,4.
-00001e90: 3639 3530 3930 3320 3331 2e30 3935 3131  6950903 31.09511
-00001ea0: 332c 322e 3730 3935 3137 3220 3330 2e35  3,2.7095172 30.5
-00001eb0: 3737 3430 382c 312e 3739 3638 3735 204c  77408,1.796875 L
-00001ec0: 2033 302e 3431 3133 3932 2c31 2e35 3035   30.411392,1.505
-00001ed0: 3835 3934 2033 302e 3134 3138 3631 2c31  8594 30.141861,1
-00001ee0: 2e33 3531 3536 3235 205a 2220 2f3e 3c70  .3515625 Z" /><p
-00001ef0: 6174 680a 2020 2020 2064 3d22 4d20 3235  ath.     d="M 25
-00001f00: 2e30 3334 392c 382e 3834 3733 3620 4320  .0349,8.84736 C 
-00001f10: 3332 2e36 3039 332c 392e 3335 3034 2033  32.6093,9.3504 3
-00001f20: 382e 3637 3834 2c31 352e 3433 3439 2033  8.6784,15.4349 3
-00001f30: 392e 3135 3436 2c32 332e 3031 3720 4820  9.1546,23.017 H 
-00001f40: 3438 2043 2034 372e 3530 3835 2c31 302e  48 C 47.5085,10.
-00001f50: 3534 3436 2033 372e 3530 3134 2c30 2e35  5446 37.5014,0.5
-00001f60: 3138 3420 3235 2e30 3334 392c 3020 5a22  184 25.0349,0 Z"
-00001f70: 0a20 2020 2020 6669 6c6c 3d22 2331 3630  .     fill="#160
-00001f80: 6632 3622 0a20 2020 2020 6964 3d22 7061  f26".     id="pa
-00001f90: 7468 3422 0a20 2020 2020 636c 6970 2d70  th4".     clip-p
-00001fa0: 6174 683d 2275 726c 2823 636c 6970 5061  ath="url(#clipPa
-00001fb0: 7468 3529 220a 2020 2020 2073 7479 6c65  th5)".     style
-00001fc0: 3d22 6669 6c6c 3a23 6631 3830 3436 3b66  ="fill:#f18046;f
-00001fd0: 696c 6c2d 6f70 6163 6974 793a 3122 0a20  ill-opacity:1". 
-00001fe0: 2020 2020 7472 616e 7366 6f72 6d3d 2272      transform="r
-00001ff0: 6f74 6174 6528 3930 2c33 322e 3936 3135  otate(90,32.9615
-00002000: 3835 2c37 2e39 3738 3538 3529 2220 2f3e  85,7.978585)" />
-00002010: 3c70 6174 680a 2020 2020 2064 3d22 4d20  <path.     d="M 
-00002020: 302c 382e 3834 3534 3420 4820 3233 2e30  0,8.84544 H 23.0
-00002030: 3137 2056 2030 2048 2030 205a 220a 2020  17 V 0 H 0 Z".  
-00002040: 2020 2066 696c 6c3d 2223 3136 3066 3236     fill="#160f26
-00002050: 220a 2020 2020 2069 643d 2270 6174 6839  ".     id="path9
-00002060: 220a 2020 2020 2063 6c69 702d 7061 7468  ".     clip-path
-00002070: 3d22 7572 6c28 2363 6c69 7050 6174 6837  ="url(#clipPath7
-00002080: 2922 0a20 2020 2020 7472 616e 7366 6f72  )".     transfor
-00002090: 6d3d 2272 6f74 6174 6528 3930 2c2d 342e  m="rotate(90,-4.
-000020a0: 3536 3438 3135 2c32 302e 3437 3030 3835  564815,20.470085
-000020b0: 2922 0a20 2020 2020 736f 6469 706f 6469  )".     sodipodi
-000020c0: 3a6e 6f64 6574 7970 6573 3d22 6363 6363  :nodetypes="cccc
-000020d0: 6322 0a20 2020 2020 7374 796c 653d 2266  c".     style="f
-000020e0: 696c 6c3a 2366 6136 3836 333b 6669 6c6c  ill:#fa6863;fill
-000020f0: 2d6f 7061 6369 7479 3a31 2220 2f3e 3c70  -opacity:1" /><p
-00002100: 6174 680a 2020 2020 2064 3d22 4d20 302c  ath.     d="M 0,
-00002110: 382e 3834 3534 3420 4820 3233 2e30 3137  8.84544 H 23.017
-00002120: 2056 2030 2048 2030 205a 220a 2020 2020   V 0 H 0 Z".    
-00002130: 2066 696c 6c3d 2223 3136 3066 3236 220a   fill="#160f26".
-00002140: 2020 2020 2069 643d 2270 6174 6832 220a       id="path2".
-00002150: 2020 2020 2063 6c69 702d 7061 7468 3d22       clip-path="
-00002160: 7572 6c28 2363 6c69 7050 6174 6837 2922  url(#clipPath7)"
-00002170: 0a20 2020 2020 7472 616e 7366 6f72 6d3d  .     transform=
-00002180: 2272 6f74 6174 6528 3930 2c37 2e39 3532  "rotate(90,7.952
-00002190: 3633 352c 372e 3935 3236 3335 2922 0a20  635,7.952635)". 
-000021a0: 2020 2020 736f 6469 706f 6469 3a6e 6f64      sodipodi:nod
-000021b0: 6574 7970 6573 3d22 6363 6363 6322 0a20  etypes="ccccc". 
-000021c0: 2020 2020 7374 796c 653d 2266 696c 6c3a      style="fill:
-000021d0: 2330 6463 3039 643b 6669 6c6c 2d6f 7061  #0dc09d;fill-opa
-000021e0: 6369 7479 3a31 2220 2f3e 3c70 6174 680a  city:1" /><path.
-000021f0: 2020 2020 2064 3d22 4d20 3339 2e31 3532       d="M 39.152
-00002200: 362c 3235 2e30 3334 3920 4320 3338 2e36  6,25.0349 C 38.6
-00002210: 3439 362c 3332 2e36 3039 3320 3332 2e35  496,32.6093 32.5
-00002220: 3635 312c 3338 2e36 3738 3420 3234 2e39  651,38.6784 24.9
-00002230: 3833 2c33 392e 3135 3435 2056 2034 3820  83,39.1545 V 48 
-00002240: 4320 3337 2e34 3535 342c 3437 2e35 3038  C 37.4554,47.508
-00002250: 3520 3437 2e34 3831 362c 3337 2e35 3031  5 47.4816,37.501
-00002260: 3420 3438 2c32 352e 3033 3439 205a 220a  4 48,25.0349 Z".
-00002270: 2020 2020 2066 696c 6c3d 2223 3136 3066       fill="#160f
-00002280: 3236 220a 2020 2020 2069 643d 2270 6174  26".     id="pat
-00002290: 6833 220a 2020 2020 2063 6c69 702d 7061  h3".     clip-pa
-000022a0: 7468 3d22 7572 6c28 2363 6c69 7050 6174  th="url(#clipPat
-000022b0: 6836 2922 0a20 2020 2020 7374 796c 653d  h6)".     style=
-000022c0: 2266 696c 6c3a 2333 6439 3566 643b 6669  "fill:#3d95fd;fi
-000022d0: 6c6c 2d6f 7061 6369 7479 3a31 220a 2020  ll-opacity:1".  
-000022e0: 2020 2074 7261 6e73 666f 726d 3d22 726f     transform="ro
-000022f0: 7461 7465 282d 3930 2c33 322e 3936 3135  tate(-90,32.9615
-00002300: 3835 2c34 302e 3037 3333 3135 2922 202f  85,40.073315)" /
-00002310: 3e3c 7061 7468 0a20 2020 2020 6964 3d22  ><path.     id="
-00002320: 7061 7468 3238 220a 2020 2020 2073 7479  path28".     sty
-00002330: 6c65 3d22 6669 6c6c 3a23 3030 3030 3030  le="fill:#000000
-00002340: 3b73 7472 6f6b 652d 7769 6474 683a 302e  ;stroke-width:0.
-00002350: 3038 3136 3535 3422 0a20 2020 2020 643d  0816554".     d=
-00002360: 224d 2032 392e 3837 3233 332c 312e 3139  "M 29.87233,1.19
-00002370: 3732 3635 3620 3239 2e34 3231 3135 382c  72656 29.421158,
-00002380: 312e 3231 3837 3520 6320 2d30 2e35 3938  1.21875 c -0.598
-00002390: 3235 352c 302e 3033 3033 3438 202d 312e  255,0.030348 -1.
-000023a0: 3334 3431 3239 2c30 2e33 3039 3737 3720  344129,0.309777 
-000023b0: 2d32 2e32 3134 3834 342c 302e 3832 3831  -2.214844,0.8281
-000023c0: 3235 206c 202d 302e 3731 3039 3337 2c30  25 l -0.710937,0
-000023d0: 2e34 3233 3832 3831 202d 302e 3838 3038  .4238281 -0.8808
-000023e0: 3539 2c30 2e37 3737 3334 3338 202d 302e  59,0.7773438 -0.
-000023f0: 3838 3238 3133 2c30 2e37 3737 3334 3337  882813,0.7773437
-00002400: 202d 302e 3335 3135 3633 2c30 2e34 3533   -0.351563,0.453
-00002410: 3132 3520 6320 2d30 2e36 3033 3932 392c  125 c -0.603929,
-00002420: 302e 3737 3733 3731 3520 2d30 2e37 3137  0.7773715 -0.717
-00002430: 3532 392c 312e 3630 3032 3037 3520 2d30  529,1.6002075 -0
-00002440: 2e33 3330 3037 382c 322e 3337 3330 3436  .330078,2.373046
-00002450: 3920 302e 3235 3032 3837 2c30 2e34 3939  9 0.250287,0.499
-00002460: 3233 3820 302e 3233 3435 3932 2c30 2e36  238 0.234592,0.6
-00002470: 3235 3738 3633 202d 302e 3136 3630 3135  257863 -0.166015
-00002480: 2c31 2e34 3032 3334 3337 202d 312e 3939  ,1.4023437 -1.99
-00002490: 3438 3631 2c33 2e38 3636 3933 3138 202d  4861,3.8669318 -
-000024a0: 312e 3234 3034 3337 2c36 2e34 3330 3434  1.240437,6.43044
-000024b0: 3338 2032 2e36 3432 3537 382c 382e 3938  38 2.642578,8.98
-000024c0: 3633 3237 3820 6c20 312e 3036 3634 3036  63278 l 1.066406
-000024d0: 2c30 2e37 3033 3132 3520 302e 3338 3238  ,0.703125 0.3828
-000024e0: 3133 2c30 2e34 3531 3137 3220 302e 3338  13,0.451172 0.38
-000024f0: 3437 3635 2c30 2e34 3533 3132 3520 302e  4765,0.453125 0.
-00002500: 3133 3836 3732 2c30 2e33 3834 3736 3620  138672,0.384766 
-00002510: 6320 302e 3037 3635 332c 302e 3231 3232  c 0.07653,0.2122
-00002520: 3732 2030 2e31 3233 3630 392c 302e 3537  72 0.123609,0.57
-00002530: 3837 3932 2030 2e31 3035 3436 392c 302e  8792 0.105469,0.
-00002540: 3831 3235 206c 202d 302e 3033 3332 2c30  8125 l -0.0332,0
-00002550: 2e34 3233 3832 3820 2d30 2e32 3132 3839  .423828 -0.21289
-00002560: 312c 302e 3334 3736 3536 2063 202d 302e  1,0.347656 c -0.
-00002570: 3230 3633 3032 2c30 2e33 3336 3532 3920  206302,0.336529 
-00002580: 2d30 2e34 3935 3630 392c 302e 3537 3131  -0.495609,0.5711
-00002590: 3336 202d 302e 3833 3339 3834 2c30 2e37  36 -0.833984,0.7
-000025a0: 3035 3037 3820 2d30 2e30 3031 392c 372e  05078 -0.0019,7.
-000025b0: 3535 652d 3420 2d30 2e30 3034 2c30 2e30  55e-4 -0.004,0.0
-000025c0: 3031 3220 2d30 2e30 3035 392c 302e 3030  012 -0.0059,0.00
-000025d0: 3220 2d30 2e32 3731 3838 372c 302e 3130  2 -0.271887,0.10
-000025e0: 3639 3332 202d 302e 3537 3537 3735 2c30  6932 -0.575775,0
-000025f0: 2e31 3435 3335 202d 302e 3839 3435 3331  .14535 -0.894531
-00002600: 2c30 2e31 3137 3138 3720 2d30 2e30 3931  ,0.117187 -0.091
-00002610: 3338 2c2d 302e 3030 3831 202d 302e 3138  38,-0.0081 -0.18
-00002620: 3338 3638 2c2d 302e 3032 3334 3920 2d30  3868,-0.02349 -0
-00002630: 2e32 3737 3334 342c 2d30 2e30 3432 3937  .277344,-0.04297
-00002640: 202d 302e 3033 3132 342c 2d30 2e30 3036   -0.03124,-0.006
-00002650: 3520 2d30 2e30 3632 3333 2c2d 302e 3030  5 -0.06233,-0.00
-00002660: 3938 202d 302e 3039 3337 352c 2d30 2e30  98 -0.09375,-0.0
-00002670: 3137 3538 202d 302e 3131 3535 3336 2c2d  1758 -0.115536,-
-00002680: 302e 3032 3836 3720 2d30 2e32 3332 3631  0.02867 -0.23261
-00002690: 342c 2d30 2e30 3639 3033 202d 302e 3334  4,-0.06903 -0.34
-000026a0: 3936 3039 2c2d 302e 3131 3532 3334 202d  9609,-0.115234 -
-000026b0: 302e 3034 3132 342c 2d30 2e30 3136 3239  0.04124,-0.01629
-000026c0: 202d 302e 3038 3137 352c 2d30 2e30 3334   -0.08175,-0.034
-000026d0: 3235 202d 302e 3132 3330 3437 2c2d 302e  25 -0.123047,-0.
-000026e0: 3035 3237 3320 2d30 2e31 3232 3534 322c  05273 -0.122542,
-000026f0: 2d30 2e30 3534 3836 202d 302e 3234 3532  -0.05486 -0.2452
-00002700: 3332 2c2d 302e 3131 3530 3239 202d 302e  32,-0.115029 -0.
-00002710: 3336 3731 3837 2c2d 302e 3138 3934 3533  367187,-0.189453
-00002720: 204c 2032 352e 3031 3837 3737 2c32 302e   L 25.018777,20.
-00002730: 3938 3035 3137 2032 342e 3231 3939 3439  980517 24.219949
-00002740: 2c32 302e 3136 3431 3120 6320 2d30 2e32  ,20.16411 c -0.2
-00002750: 3034 3238 382c 2d30 2e32 3039 3233 3220  04288,-0.209232 
-00002760: 2d30 2e35 3038 3232 352c 2d30 2e35 3438  -0.508225,-0.548
-00002770: 3139 3420 2d30 2e38 3333 3938 342c 2d30  194 -0.833984,-0
-00002780: 2e39 3233 3832 3820 2d30 2e30 3237 3231  .923828 -0.02721
-00002790: 2c2d 302e 3033 3133 3420 2d30 2e30 3432  ,-0.03134 -0.042
-000027a0: 3739 2c2d 302e 3034 3632 3320 2d30 2e30  79,-0.04623 -0.0
-000027b0: 3730 3331 2c2d 302e 3037 3831 3320 2d33  7031,-0.07813 -3
-000027c0: 2e34 652d 342c 2d33 2e39 3465 2d34 2033  .4e-4,-3.94e-4 3
-000027d0: 2e34 3165 2d34 2c2d 302e 3030 3136 2030  .41e-4,-0.0016 0
-000027e0: 2c2d 302e 3030 3220 2d30 2e33 3534 3036  ,-0.002 -0.35406
-000027f0: 312c 2d30 2e34 3130 3336 202d 302e 3733  1,-0.41036 -0.73
-00002800: 3135 3836 2c2d 302e 3836 3234 3839 202d  1586,-0.862489 -
-00002810: 312e 3034 3838 3238 2c2d 312e 3235 3937  1.048828,-1.2597
-00002820: 3635 202d 302e 3134 3338 3931 2c2d 302e  65 -0.143891,-0.
-00002830: 3138 3031 3934 202d 302e 3238 3534 3832  180194 -0.285482
-00002840: 2c2d 302e 3335 3333 3634 202d 302e 3432  ,-0.353364 -0.42
-00002850: 3537 3831 2c2d 302e 3532 3134 3835 202d  5781,-0.521485 -
-00002860: 302e 3035 3637 382c 2d30 2e30 3638 3034  0.05678,-0.06804
-00002870: 202d 302e 3131 3336 3632 2c2d 302e 3133   -0.113662,-0.13
-00002880: 3530 3732 202d 302e 3136 3939 3232 2c2d  5072 -0.169922,-
-00002890: 302e 3230 3131 3732 202d 302e 3439 3031  0.201172 -0.4901
-000028a0: 3137 2c2d 302e 3537 3538 3433 202d 302e  17,-0.575843 -0.
-000028b0: 3936 3233 3834 2c2d 312e 3037 3830 3333  962384,-1.078033
-000028c0: 202d 312e 3432 3537 3831 2c2d 312e 3531   -1.425781,-1.51
-000028d0: 3336 3732 202d 302e 3031 3839 392c 2d30  3672 -0.01899,-0
-000028e0: 2e30 3137 3835 202d 302e 3033 3739 382c  .01785 -0.03798,
-000028f0: 2d30 2e30 3335 3032 202d 302e 3035 3636  -0.03502 -0.0566
-00002900: 342c 2d30 2e30 3532 3733 202d 302e 3330  4,-0.05273 -0.30
-00002910: 3335 3538 2c2d 302e 3238 3231 3531 202d  3558,-0.282151 -
-00002920: 302e 3630 3333 3637 2c2d 302e 3533 3639  0.603367,-0.5369
-00002930: 3531 202d 302e 3930 3432 3937 2c2d 302e  51 -0.904297,-0.
-00002940: 3736 3336 3732 202d 302e 3030 3435 2c2d  763672 -0.0045,-
-00002950: 302e 3030 3334 202d 302e 3030 3932 2c2d  0.0034 -0.0092,-
-00002960: 302e 3030 3634 202d 302e 3031 3336 372c  0.0064 -0.01367,
-00002970: 2d30 2e30 3039 3820 2d30 2e31 3735 3433  -0.0098 -0.17543
-00002980: 332c 2d30 2e31 3331 3730 3120 2d30 2e33  3,-0.131701 -0.3
-00002990: 3530 3937 2c2d 302e 3235 3532 3636 202d  5097,-0.255266 -
-000029a0: 302e 3532 3733 3434 2c2d 302e 3336 3931  0.527344,-0.3691
-000029b0: 3431 202d 302e 3331 3236 3539 2c2d 302e  41 -0.312659,-0.
-000029c0: 3230 3138 3636 202d 302e 3632 3738 3237  201866 -0.627827
-000029d0: 2c2d 302e 3337 3633 3538 202d 302e 3934  ,-0.376358 -0.94
-000029e0: 3932 3139 2c2d 302e 3532 3533 3931 202d  9219,-0.525391 -
-000029f0: 302e 3136 3231 3337 2c2d 302e 3037 3531  0.162137,-0.0751
-00002a00: 3820 2d30 2e33 3236 3431 342c 2d30 2e31  8 -0.326414,-0.1
-00002a10: 3432 3536 202d 302e 3439 3231 3837 2c2d  4256 -0.492187,-
-00002a20: 302e 3230 3530 3738 202d 302e 3034 3438  0.205078 -0.0448
-00002a30: 332c 2d30 2e30 3136 3920 2d30 2e30 3839  3,-0.0169 -0.089
-00002a40: 3633 2c2d 302e 3033 3437 3820 2d30 2e31  63,-0.03478 -0.1
-00002a50: 3334 3736 362c 2d30 2e30 3530 3738 202d  34766,-0.05078 -
-00002a60: 302e 3030 3333 2c2d 302e 3030 3132 202d  0.0033,-0.0012 -
-00002a70: 302e 3030 3635 2c2d 302e 3030 3237 202d  0.0065,-0.0027 -
-00002a80: 302e 3030 3938 2c2d 302e 3030 3339 202d  0.0098,-0.0039 -
-00002a90: 302e 3836 3034 3433 2c2d 302e 3330 3336  0.860443,-0.3036
-00002aa0: 3236 202d 312e 3737 3738 3832 2c2d 302e  26 -1.777882,-0.
-00002ab0: 3434 3539 3920 2d32 2e38 3230 3234 362c  44599 -2.820246,
-00002ac0: 2d30 2e34 3538 3935 3720 2d30 2e32 3131  -0.458957 -0.211
-00002ad0: 3735 362c 2d30 2e30 3032 3620 2d30 2e34  756,-0.0026 -0.4
-00002ae0: 3239 3835 342c 322e 3265 2d34 202d 302e  29854,2.2e-4 -0.
-00002af0: 3635 3233 3434 2c30 2e30 3037 3820 6c20  652344,0.0078 l 
-00002b00: 2d30 2e38 3335 3933 372c 302e 3032 3933  -0.835937,0.0293
-00002b10: 202d 302e 3638 3136 3431 2c30 2e32 3136   -0.681641,0.216
-00002b20: 3739 3720 6320 2d30 2e38 3237 3638 372c  797 c -0.827687,
-00002b30: 302e 3236 3433 3835 202d 312e 3333 3130  0.264385 -1.3310
-00002b40: 3932 2c30 2e35 3337 3830 3320 2d32 2e30  92,0.537803 -2.0
-00002b50: 3436 3837 352c 312e 3130 3933 3735 206c  46875,1.109375 l
-00002b60: 202d 302e 3534 3239 3639 2c30 2e34 3333   -0.542969,0.433
-00002b70: 3539 202d 302e 3431 3430 3632 2c30 2e35  59 -0.414062,0.5
-00002b80: 3131 3731 3920 6320 2d31 2e38 3236 3130  11719 c -1.82610
-00002b90: 372c 322e 3236 3233 3337 202d 322e 3035  7,2.262337 -2.05
-00002ba0: 3632 3237 2c35 2e31 3238 3138 202d 302e  6227,5.12818 -0.
-00002bb0: 3630 3135 3633 2c37 2e34 3938 3036 206c  601563,7.49806 l
-00002bc0: 2030 2e32 3936 3837 352c 302e 3438 3234   0.296875,0.4824
-00002bd0: 3232 2030 2e36 3035 3436 392c 302e 3630  22 0.605469,0.60
-00002be0: 3734 3232 2063 2031 2e33 3134 3934 312c  7422 c 1.314941,
-00002bf0: 312e 3332 3138 3820 322e 3835 3535 3938  1.32188 2.855598
-00002c00: 2c32 2e31 3038 3339 3620 352e 3839 3036  ,2.108396 5.8906
-00002c10: 3235 2c33 2e30 3031 3935 3320 372e 3235  25,3.001953 7.25
-00002c20: 3833 2c32 2e31 3336 3935 3220 392e 3237  83,2.136952 9.27
-00002c30: 3138 3731 2c33 2e35 3737 3536 3920 382e  1871,3.577569 8.
-00002c40: 3436 3039 3337 2c36 2e30 3534 3638 3720  460937,6.054687 
-00002c50: 6c20 2d30 2e31 3430 3632 352c 302e 3433  l -0.140625,0.43
-00002c60: 3136 3431 202d 302e 3330 3436 3837 2c30  1641 -0.304687,0
-00002c70: 2e33 3635 3233 3420 2d30 2e33 3034 3638  .365234 -0.30468
-00002c80: 382c 302e 3336 3532 3335 202d 302e 3334  8,0.365235 -0.34
-00002c90: 3137 3937 2c30 2e31 3532 3334 3420 6320  1797,0.152344 c 
-00002ca0: 2d31 2e33 3730 3530 362c 302e 3631 3239  -1.370506,0.6129
-00002cb0: 3931 202d 322e 3635 3536 3935 2c2d 302e  91 -2.655695,-0.
-00002cc0: 3031 3031 3320 2d35 2e35 3333 3230 332c  01013 -5.533203,
-00002cd0: 2d32 2e36 3831 3634 3120 6c20 2d31 2e35  -2.681641 l -1.5
-00002ce0: 3536 3634 2c2d 312e 3434 3533 3133 202d  5664,-1.445313 -
-00002cf0: 302e 3539 3736 3536 2c2d 302e 3431 3430  0.597656,-0.4140
-00002d00: 3632 2043 2031 322e 3932 3936 3037 2c32  62 C 12.929607,2
-00002d10: 382e 3438 3438 3439 2031 312e 3138 3132  8.484849 11.1812
-00002d20: 3832 2c32 372e 3938 3136 3831 2039 2e37  82,27.981681 9.7
-00002d30: 3636 3836 312c 3238 2e34 3335 3534 3720  66861,28.435547 
-00002d40: 6c20 2d30 2e33 3932 3537 382c 302e 3132  l -0.392578,0.12
-00002d50: 3520 2d30 2e34 3634 3834 342c 302e 3431  5 -0.464844,0.41
-00002d60: 3231 3039 202d 302e 3436 3238 392c 302e  2109 -0.46289,0.
-00002d70: 3431 3231 3120 2d30 2e32 3434 3134 312c  41211 -0.244141,
-00002d80: 302e 3433 3934 3533 2063 202d 302e 3637  0.439453 c -0.67
-00002d90: 3939 3634 2c31 2e32 3331 3734 3320 2d30  9964,1.231743 -0
-00002da0: 2e36 3239 3039 352c 322e 3432 3739 3938  .629095,2.427998
-00002db0: 2030 2e31 3538 3230 332c 332e 3733 3433   0.158203,3.7343
-00002dc0: 3735 206c 2030 2e32 3735 3339 312c 302e  75 l 0.275391,0.
-00002dd0: 3435 3730 3331 2031 2e33 3038 3539 342c  457031 1.308594,
-00002de0: 312e 3430 3233 3434 2031 2e33 3130 3534  1.402344 1.31054
-00002df0: 372c 312e 3430 3432 3937 2030 2e32 3434  7,1.404297 0.244
-00002e00: 3134 2c30 2e34 3736 3536 3220 6320 302e  14,0.476562 c 0.
-00002e10: 3830 3737 3937 2c31 2e35 3738 3534 3120  807797,1.578541 
-00002e20: 302e 3534 3736 3339 2c33 2e34 3730 3332  0.547639,3.47032
-00002e30: 3920 2d30 2e38 3138 3335 392c 352e 3933  9 -0.818359,5.93
-00002e40: 3335 3934 202d 302e 3537 3937 3737 2c31  3594 -0.579777,1
-00002e50: 2e30 3435 3439 3720 2d30 2e35 3538 3339  .045497 -0.55839
-00002e60: 2c31 2e31 3330 3635 3620 302e 3131 3931  ,1.130656 0.1191
-00002e70: 342c 302e 3435 3331 3235 2030 2e39 3335  4,0.453125 0.935
-00002e80: 3039 2c2d 302e 3933 3530 3920 312e 3631  09,-0.93509 1.61
-00002e90: 3233 3234 2c2d 322e 3033 3735 3936 2032  2324,-2.037596 2
-00002ea0: 2e30 3730 3331 332c 2d33 2e33 3733 3034  .070313,-3.37304
-00002eb0: 3720 6c20 302e 3235 2c2d 302e 3733 3034  7 l 0.25,-0.7304
-00002ec0: 3639 2030 2e30 3032 2c2d 302e 3837 3130  69 0.002,-0.8710
-00002ed0: 3933 2030 2e30 3031 392c 2d30 2e38 3731  93 0.0019,-0.871
-00002ee0: 3039 3420 2d30 2e32 3236 3536 332c 2d30  094 -0.226563,-0
-00002ef0: 2e36 3937 3236 3620 4320 3132 2e35 3335  .697266 C 12.535
-00002f00: 3033 322c 3336 2e30 3237 3136 3920 3132  032,36.027169 12
-00002f10: 2e32 3731 3839 372c 3335 2e36 3132 3336  .271897,35.61236
-00002f20: 2031 302e 3932 3530 3634 2c33 342e 3033   10.925064,34.03
-00002f30: 3531 3536 2039 2e36 3534 3933 332c 3332  5156 9.654933,32
-00002f40: 2e35 3437 3737 3520 392e 3438 3533 3636  .547775 9.485366
-00002f50: 2c33 322e 3231 3839 3920 392e 3539 3130  ,32.21899 9.5910
-00002f60: 382c 3331 2e34 3333 3539 3420 6c20 302e  8,31.433594 l 0.
-00002f70: 3035 3037 382c 2d30 2e33 3735 2030 2e33  05078,-0.375 0.3
-00002f80: 3038 3539 342c 2d30 2e33 3535 3436 3920  08594,-0.355469 
-00002f90: 302e 3330 3636 342c 2d30 2e33 3535 3436  0.30664,-0.35546
-00002fa0: 3920 302e 3430 3432 3937 2c2d 302e 3032  9 0.404297,-0.02
-00002fb0: 3733 3420 6320 302e 3838 3132 3539 2c2d  734 c 0.881259,-
-00002fc0: 302e 3035 3732 3420 322e 3130 3737 3939  0.05724 2.107799
-00002fd0: 2c30 2e35 3735 3034 3720 332e 3639 3533  ,0.575047 3.6953
-00002fe0: 3133 2c31 2e39 3032 3334 3420 6c20 302e  13,1.902344 l 0.
-00002ff0: 3735 3339 3036 2c30 2e36 3238 3930 3620  753906,0.628906 
-00003000: 312e 3038 3738 3931 2c31 2e32 3236 3536  1.087891,1.22656
-00003010: 3320 312e 3038 3938 3434 2c31 2e32 3236  3 1.089844,1.226
-00003020: 3536 3320 302e 3631 3332 3831 2c30 2e34  563 0.613281,0.4
-00003030: 3738 3531 3520 6320 322e 3534 3638 3534  78515 c 2.546854
-00003040: 2c31 2e39 3837 3834 3520 352e 3434 3736  ,1.987845 5.4476
-00003050: 392c 322e 3334 3634 3832 2037 2e33 3836  9,2.346482 7.386
-00003060: 3731 392c 302e 3931 3430 3633 2030 2e37  719,0.914063 0.7
-00003070: 3437 3931 2c2d 302e 3535 3235 3036 2031  4791,-0.552506 1
-00003080: 2e33 3930 3931 312c 2d31 2e34 3937 3834  .390911,-1.49784
-00003090: 3320 312e 3738 3332 3033 2c2d 322e 3632  3 1.783203,-2.62
-000030a0: 3330 3437 206c 2030 2e32 3533 3930 362c  3047 l 0.253906,
-000030b0: 2d30 2e37 3236 3536 3320 302e 3030 3339  -0.726563 0.0039
-000030c0: 2c2d 302e 3933 3136 3420 302e 3030 3339  ,-0.93164 0.0039
-000030d0: 2c2d 302e 3933 3136 3431 202d 302e 3235  ,-0.931641 -0.25
-000030e0: 2c2d 302e 3733 3234 3232 2043 2032 362e  ,-0.732422 C 26.
-000030f0: 3934 3535 3137 2c33 302e 3334 3938 3535  945517,30.349855
-00003100: 2032 362e 3637 3936 2c32 392e 3738 3632   26.6796,29.7862
-00003110: 3638 2032 362e 3439 3134 3731 2c32 392e  68 26.491471,29.
-00003120: 3439 3830 3437 206c 202d 302e 3334 3337  498047 l -0.3437
-00003130: 352c 2d30 2e35 3235 3339 3120 2d30 2e39  5,-0.525391 -0.9
-00003140: 3531 3137 322c 2d30 2e38 3934 3533 3120  51172,-0.894531 
-00003150: 2d30 2e39 3533 3132 352c 2d30 2e38 3934  -0.953125,-0.894
-00003160: 3533 3120 2d30 2e35 3830 3037 382c 2d30  531 -0.580078,-0
-00003170: 2e33 3435 3730 3320 4320 3232 2e36 3739  .345703 C 22.679
-00003180: 3233 2c32 362e 3234 3934 3631 2032 312e  23,26.249461 21.
-00003190: 3438 3532 3631 2c32 352e 3737 3035 3936  485261,25.770596
-000031a0: 2031 382e 3434 3435 3936 2c32 342e 3734   18.444596,24.74
-000031b0: 3830 3437 2031 352e 3136 3931 2c32 332e  8047 15.1691,23.
-000031c0: 3634 3635 3236 2031 342e 3431 3031 3834  646526 14.410184
-000031d0: 2c32 332e 3334 3430 3936 2031 332e 3332  ,23.344096 13.32
-000031e0: 3135 3439 2c32 322e 3730 3131 3732 204c  1549,22.701172 L
-000031f0: 2031 322e 3536 3736 3433 2c32 322e 3235   12.567643,22.25
-00003200: 3538 3539 2031 322e 3135 3335 382c 3231  5859 12.15358,21
-00003210: 2e37 3839 3036 3220 3131 2e37 3337 3536  .789062 11.73756
-00003220: 342c 3231 2e33 3234 3231 3920 3131 2e35  4,21.324219 11.5
-00003230: 3539 3833 2c32 302e 3834 3736 3536 2063  5983,20.847656 c
-00003240: 202d 302e 3232 3533 3834 2c2d 302e 3630   -0.225384,-0.60
-00003250: 3630 3132 202d 302e 3235 3638 3533 2c2d  6012 -0.256853,-
-00003260: 312e 3338 3734 3137 202d 302e 3038 3030  1.387417 -0.0800
-00003270: 382c 2d31 2e39 3535 3037 3820 6c20 302e  8,-1.955078 l 0.
-00003280: 3133 3836 3732 2c2d 302e 3434 3333 3539  138672,-0.443359
-00003290: 2030 2e34 3930 3233 342c 2d30 2e34 3932   0.490234,-0.492
-000032a0: 3138 3820 302e 3439 3032 3335 2c2d 302e  188 0.490235,-0.
-000032b0: 3439 3231 3837 2030 2e34 3736 3536 322c  492187 0.476562,
-000032c0: 2d30 2e31 3731 3837 3520 6320 312e 3237  -0.171875 c 1.27
-000032d0: 3233 3134 2c2d 302e 3436 3030 3334 2032  2314,-0.460034 2
-000032e0: 2e36 3336 3539 382c 2d30 2e31 3637 3136  .636598,-0.16716
-000032f0: 3720 342e 3038 3230 3331 2c30 2e38 3639  7 4.082031,0.869
-00003300: 3134 2030 2e30 3438 3038 2c30 2e30 3334  14 0.04808,0.034
-00003310: 3437 2030 2e30 3936 3238 2c30 2e30 3733  47 0.09628,0.073
-00003320: 3236 2030 2e31 3434 3533 322c 302e 3130  26 0.144532,0.10
-00003330: 3933 3735 2030 2e30 3831 3138 2c30 2e30  9375 0.08118,0.0
-00003340: 3630 3735 2030 2e31 3632 3436 332c 302e  6075 0.162463,0.
-00003350: 3132 3231 3033 2030 2e32 3434 3134 2c30  122103 0.24414,0
-00003360: 2e31 3837 3520 302e 3036 3031 382c 302e  .1875 0.06018,0.
-00003370: 3034 3831 3820 302e 3132 3131 3933 2c30  04818 0.121193,0
-00003380: 2e30 3937 3733 2030 2e31 3831 3634 312c  .09773 0.181641,
-00003390: 302e 3134 3834 3338 2030 2e30 3732 3236  0.148438 0.07226
-000033a0: 2c30 2e30 3630 3632 2030 2e31 3434 3134  ,0.06062 0.14414
-000033b0: 392c 302e 3132 3332 3732 2030 2e32 3136  9,0.123272 0.216
-000033c0: 3739 372c 302e 3138 3735 2030 2e32 3033  797,0.1875 0.203
-000033d0: 3135 2c30 2e31 3739 3630 3820 302e 3430  15,0.179608 0.40
-000033e0: 3731 3637 2c30 2e33 3732 3234 3220 302e  7167,0.372242 0.
-000033f0: 3631 3332 3831 2c30 2e35 3830 3037 3820  613281,0.580078 
-00003400: 302e 3131 3937 3031 2c30 2e31 3230 3730  0.119701,0.12070
-00003410: 3220 302e 3234 3036 3433 2c30 2e32 3436  2 0.240643,0.246
-00003420: 3732 3720 302e 3336 3133 3238 2c30 2e33  727 0.361328,0.3
-00003430: 3736 3935 3320 302e 3036 3337 352c 302e  76953 0.06375,0.
-00003440: 3036 3837 3920 302e 3132 3733 3836 2c30  06879 0.127386,0
-00003450: 2e31 3339 3439 3220 302e 3139 3134 3036  .139492 0.191406
-00003460: 2c30 2e32 3130 3933 3820 302e 3236 3133  ,0.210938 0.2613
-00003470: 3937 2c30 2e32 3931 3731 3520 302e 3532  97,0.291715 0.52
-00003480: 3531 3535 2c30 2e36 3033 3430 3820 302e  5155,0.603408 0.
-00003490: 3739 3130 3136 2c30 2e39 3339 3435 3320  791016,0.939453 
-000034a0: 302e 3437 3639 3038 2c30 2e36 3032 3830  0.476908,0.60280
-000034b0: 3920 312e 3232 3038 3532 2c31 2e34 3439  9 1.220852,1.449
-000034c0: 3236 3920 312e 3635 3432 3937 2c31 2e38  269 1.654297,1.8
-000034d0: 3832 3831 3220 6c20 302e 3738 3930 3632  82812 l 0.789062
-000034e0: 2c30 2e37 3839 3036 3320 302e 3736 3735  ,0.789063 0.7675
-000034f0: 3738 2c30 2e35 3432 3936 3920 6320 312e  78,0.542969 c 1.
-00003500: 3634 3136 3238 2c31 2e31 3538 3830 3920  641628,1.158809 
-00003510: 332e 3034 3833 3134 2c31 2e36 3139 3034  3.048314,1.61904
-00003520: 3920 342e 3738 3731 312c 312e 3536 3833  9 4.78711,1.5683
-00003530: 3539 206c 2030 2e37 3839 3036 322c 2d30  59 l 0.789062,-0
-00003540: 2e30 3233 3434 2030 2e37 3136 3739 372c  .02344 0.716797,
-00003550: 2d30 2e32 3434 3134 2063 2030 2e31 3132  -0.24414 c 0.112
-00003560: 3731 332c 2d30 2e30 3338 3337 2030 2e32  713,-0.03837 0.2
-00003570: 3138 3631 372c 2d30 2e30 3738 3632 2030  18617,-0.07862 0
-00003580: 2e33 3230 3331 332c 2d30 2e31 3139 3134  .320313,-0.11914
-00003590: 3120 6c20 2d30 2e30 3033 392c 2d30 2e30  1 l -0.0039,-0.0
-000035a0: 3035 3920 6320 302e 3638 3433 3331 2c2d  059 c 0.684331,-
-000035b0: 302e 3237 3432 3131 2031 2e31 3537 3037  0.274211 1.15707
-000035c0: 382c 2d30 2e36 3130 3837 3320 312e 3731  8,-0.610873 1.71
-000035d0: 3039 3338 2c2d 312e 3233 3433 3735 206c  0938,-1.234375 l
-000035e0: 2030 2e34 3838 3238 312c 2d30 2e35 3530   0.488281,-0.550
-000035f0: 3738 3220 302e 3333 3339 3834 2c2d 302e  782 0.333984,-0.
-00003600: 3637 3338 3238 2063 2030 2e39 3134 3731  673828 c 0.91471
-00003610: 312c 2d31 2e38 3437 3431 3820 302e 3833  1,-1.847418 0.83
-00003620: 3030 3936 2c2d 332e 3636 3532 3120 2d30  0096,-3.66521 -0
-00003630: 2e32 352c 2d35 2e33 3633 3238 3120 4c20  .25,-5.363281 L 
-00003640: 3331 2e36 3439 3637 392c 3136 2e39 3134  31.649679,16.914
-00003650: 3031 3920 3330 2e38 3033 3937 362c 3136  019 30.803976,16
-00003660: 2e31 3330 3831 3620 3239 2e39 3538 3237  .130816 29.95827
-00003670: 332c 3135 2e33 3439 3536 3620 3239 2e32  3,15.349566 29.2
-00003680: 3934 3231 2c31 342e 3937 3236 3133 2043  9421,14.972613 C
-00003690: 2032 382e 3932 3930 3634 2c31 342e 3736   28.929064,14.76
-000036a0: 3631 3820 3238 2e33 3731 3932 382c 3134  618 28.371928,14
-000036b0: 2e34 3636 3938 3120 3238 2e30 3535 3932  .466981 28.05592
-000036c0: 342c 3134 2e33 3036 3634 3120 3237 2e37  4,14.306641 27.7
-000036d0: 3339 3931 382c 3134 2e31 3436 3320 3237  39918,14.1463 27
-000036e0: 2e32 3631 3632 332c 3133 2e38 3538 3939  .261623,13.85899
-000036f0: 3620 3236 2e39 3933 3432 342c 3133 2e36  6 26.993424,13.6
-00003700: 3637 3936 3920 6c20 2d30 2e34 3838 3238  67969 l -0.48828
-00003710: 322c 2d30 2e33 3437 3635 3720 2d30 2e32  2,-0.347657 -0.2
-00003720: 3338 3238 312c 2d30 2e33 3637 3138 3720  38281,-0.367187 
-00003730: 6320 2d30 2e35 3931 3735 372c 2d30 2e39  c -0.591757,-0.9
-00003740: 3134 3836 3620 2d30 2e35 3632 3539 2c2d  14866 -0.56259,-
-00003750: 322e 3334 3435 3032 2030 2e30 3734 3232  2.344502 0.07422
-00003760: 2c2d 332e 3730 3730 3331 3220 4c20 3236  ,-3.7070312 L 26
-00003770: 2e35 3737 3430 382c 382e 3733 3832 3831  .577408,8.738281
-00003780: 3220 3236 2e39 3033 3538 2c38 2e36 3935  2 26.90358,8.695
-00003790: 3331 3235 2043 2032 372e 3038 3335 3932  3125 C 27.083592
-000037a0: 2c38 2e36 3731 3038 3335 2032 372e 3439  ,8.6710835 27.49
-000037b0: 3831 342c 382e 3535 3531 3032 3820 3237  814,8.5551028 27
-000037c0: 2e38 3233 3530 322c 382e 3433 3735 204c  .823502,8.4375 L
-000037d0: 2032 382e 3431 3532 3939 2c38 2e32 3232   28.415299,8.222
-000037e0: 3635 3632 2032 382e 3938 3536 3131 2c37  6562 28.985611,7
-000037f0: 2e36 3937 3236 3536 2032 392e 3535 3738  .6972656 29.5578
-00003800: 3737 2c37 2e31 3639 3932 3139 2032 392e  77,7.1699219 29.
-00003810: 3836 3634 3731 2c36 2e35 3534 3638 3735  866471,6.5546875
-00003820: 2043 2033 302e 3739 3835 3531 2c34 2e36   C 30.798551,4.6
-00003830: 3935 3039 3033 2033 312e 3039 3531 3133  950903 31.095113
-00003840: 2c32 2e37 3039 3531 3732 2033 302e 3537  ,2.7095172 30.57
-00003850: 3734 3038 2c31 2e37 3936 3837 3520 4c20  7408,1.796875 L 
-00003860: 3330 2e34 3131 3339 322c 312e 3530 3538  30.411392,1.5058
-00003870: 3539 3420 3330 2e31 3431 3836 312c 312e  594 30.141861,1.
-00003880: 3335 3135 3632 3520 5a22 202f 3e3c 7061  3515625 Z" /><pa
-00003890: 7468 0a20 2020 2020 643d 224d 2030 2c38  th.     d="M 0,8
-000038a0: 2e38 3435 3434 2048 2032 332e 3031 3720  .84544 H 23.017 
-000038b0: 5620 3020 4820 3020 5a22 0a20 2020 2020  V 0 H 0 Z".     
-000038c0: 6669 6c6c 3d22 2331 3630 6632 3622 0a20  fill="#160f26". 
-000038d0: 2020 2020 6964 3d22 7061 7468 3239 220a      id="path29".
-000038e0: 2020 2020 2063 6c69 702d 7061 7468 3d22       clip-path="
-000038f0: 7572 6c28 2363 6c69 7050 6174 6837 2922  url(#clipPath7)"
-00003900: 0a20 2020 2020 7472 616e 7366 6f72 6d3d  .     transform=
-00003910: 226d 6174 7269 7828 302c 302e 3131 3433  "matrix(0,0.1143
-00003920: 3031 3434 2c2d 312c 302c 3135 2e39 3035  0144,-1,0,15.905
-00003930: 3237 2c32 352e 3033 3439 2922 0a20 2020  27,25.0349)".   
-00003940: 2020 736f 6469 706f 6469 3a6e 6f64 6574    sodipodi:nodet
-00003950: 7970 6573 3d22 6363 6363 6322 0a20 2020  ypes="ccccc".   
-00003960: 2020 7374 796c 653d 2266 696c 6c3a 2366    style="fill:#f
-00003970: 6136 3836 333b 6669 6c6c 2d6f 7061 6369  a6863;fill-opaci
-00003980: 7479 3a31 2220 2f3e 3c70 6174 680a 2020  ty:1" /><path.  
-00003990: 2020 2069 643d 2270 6174 6833 3022 0a20     id="path30". 
-000039a0: 2020 2020 636c 6970 2d70 6174 683d 2275      clip-path="u
-000039b0: 726c 2823 636c 6970 5061 7468 3629 220a  rl(#clipPath6)".
-000039c0: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
-000039d0: 3a23 3364 3935 6664 3b66 696c 6c2d 6f70  :#3d95fd;fill-op
-000039e0: 6163 6974 793a 3122 0a20 2020 2020 643d  acity:1".     d=
-000039f0: 226d 2034 332e 3939 3937 3434 2c32 352e  "m 43.999744,25.
-00003a00: 3033 3438 3431 2068 202d 342e 3834 3736  034841 h -4.8476
-00003a10: 3536 2063 202d 302e 3037 3933 342c 312e  56 c -0.07934,1.
-00003a20: 3139 3438 3132 202d 302e 3239 3735 3838  194812 -0.297588
-00003a30: 2c32 2e33 3531 3232 3420 2d30 2e36 3338  ,2.351224 -0.638
-00003a40: 3637 322c 332e 3435 3530 3738 2068 2035  672,3.455078 h 5
-00003a50: 2e31 3933 3335 3920 6320 302e 3134 3736  .193359 c 0.1476
-00003a60: 3136 2c2d 312e 3132 3538 3820 302e 3234  16,-1.12588 0.24
-00003a70: 3430 3836 2c2d 322e 3237 3935 3435 2030  4086,-2.279545 0
-00003a80: 2e32 3932 3936 392c 2d33 2e34 3535 3037  .292969,-3.45507
-00003a90: 3820 7a22 0a20 2020 2020 7472 616e 7366  8 z".     transf
-00003aa0: 6f72 6d3d 2272 6f74 6174 6528 2d39 302c  orm="rotate(-90,
-00003ab0: 3332 2e39 3631 3538 352c 3430 2e30 3733  32.961585,40.073
-00003ac0: 3331 3529 2220 2f3e 3c70 6174 680a 2020  315)" /><path.  
-00003ad0: 2020 2069 643d 2270 6174 6833 3122 0a20     id="path31". 
-00003ae0: 2020 2020 636c 6970 2d70 6174 683d 2275      clip-path="u
-00003af0: 726c 2823 636c 6970 5061 7468 3529 220a  rl(#clipPath5)".
-00003b00: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
-00003b10: 3a23 6631 3830 3436 3b66 696c 6c2d 6f70  :#f18046;fill-op
-00003b20: 6163 6974 793a 3122 0a20 2020 2020 643d  acity:1".     d=
-00003b30: 226d 2033 382e 3734 3836 3235 2c32 302e  "m 38.748625,20.
-00003b40: 3336 3836 3231 2063 2030 2e32 3039 392c  368621 c 0.2099,
-00003b50: 302e 3835 3638 3434 2030 2e33 3439 3330  0.856844 0.34930
-00003b60: 372c 312e 3734 3137 3833 2030 2e34 3036  7,1.741783 0.406
-00003b70: 3235 2c32 2e36 3438 3433 3820 6820 382e  25,2.648438 h 8.
-00003b80: 3834 3537 3033 2043 2034 372e 3836 3635  845703 C 47.8665
-00003b90: 3432 2c31 392e 3631 3537 3235 2034 372e  42,19.615725 47.
-00003ba0: 3032 3031 342c 3136 2e33 3939 3630 3620  02014,16.399606 
-00003bb0: 3435 2e36 3133 3835 392c 3133 2e35 3035  45.613859,13.505
-00003bc0: 3334 205a 220a 2020 2020 2074 7261 6e73  34 Z".     trans
-00003bd0: 666f 726d 3d22 726f 7461 7465 2839 302c  form="rotate(90,
-00003be0: 3332 2e39 3631 3538 352c 372e 3937 3835  32.961585,7.9785
-00003bf0: 3835 2922 0a20 2020 2020 736f 6469 706f  85)".     sodipo
-00003c00: 6469 3a6e 6f64 6574 7970 6573 3d22 6363  di:nodetypes="cc
-00003c10: 6363 6322 202f 3e3c 2f73 7667 3e0a       ccc" /></svg>.
+000003b0: 6379 3d22 3336 2e32 3239 3437 220a 2020  cy="36.22947".  
+000003c0: 2020 2069 6e6b 7363 6170 653a 7769 6e64     inkscape:wind
+000003d0: 6f77 2d77 6964 7468 3d22 3139 3230 220a  ow-width="1920".
+000003e0: 2020 2020 2069 6e6b 7363 6170 653a 7769       inkscape:wi
+000003f0: 6e64 6f77 2d68 6569 6768 743d 2231 3132  ndow-height="112
+00000400: 3822 0a20 2020 2020 696e 6b73 6361 7065  8".     inkscape
+00000410: 3a77 696e 646f 772d 783d 2230 220a 2020  :window-x="0".  
+00000420: 2020 2069 6e6b 7363 6170 653a 7769 6e64     inkscape:wind
+00000430: 6f77 2d79 3d22 3022 0a20 2020 2020 696e  ow-y="0".     in
+00000440: 6b73 6361 7065 3a77 696e 646f 772d 6d61  kscape:window-ma
+00000450: 7869 6d69 7a65 643d 2231 220a 2020 2020  ximized="1".    
+00000460: 2069 6e6b 7363 6170 653a 6375 7272 656e   inkscape:curren
+00000470: 742d 6c61 7965 723d 2273 7667 3422 0a20  t-layer="svg4". 
+00000480: 2020 2020 696e 6b73 6361 7065 3a65 7870      inkscape:exp
+00000490: 6f72 742d 6267 636f 6c6f 723d 2223 6666  ort-bgcolor="#ff
+000004a0: 6666 6666 3030 220a 2020 2020 2073 686f  ffff00".     sho
+000004b0: 7767 7269 643d 2266 616c 7365 2220 2f3e  wgrid="false" />
+000004c0: 3c64 6566 730a 2020 2020 2069 643d 2264  <defs.     id="d
+000004d0: 6566 7334 223e 3c63 6c69 7050 6174 680a  efs4"><clipPath.
+000004e0: 2020 2020 2020 2063 6c69 7050 6174 6855         clipPathU
+000004f0: 6e69 7473 3d22 7573 6572 5370 6163 654f  nits="userSpaceO
+00000500: 6e55 7365 220a 2020 2020 2020 2069 643d  nUse".       id=
+00000510: 2263 6c69 7050 6174 6835 223e 3c67 0a20  "clipPath5"><g. 
+00000520: 2020 2020 2020 2020 6964 3d22 6736 223e          id="g6">
+00000530: 3c72 6563 740a 2020 2020 2020 2020 2020  <rect.          
+00000540: 2077 6964 7468 3d22 3438 220a 2020 2020   width="48".    
+00000550: 2020 2020 2020 2068 6569 6768 743d 2234         height="4
+00000560: 3822 0a20 2020 2020 2020 2020 2020 6669  8".           fi
+00000570: 6c6c 3d22 2366 6666 6666 6622 0a20 2020  ll="#ffffff".   
+00000580: 2020 2020 2020 2020 6964 3d22 7265 6374          id="rect
+00000590: 3522 0a20 2020 2020 2020 2020 2020 783d  5".           x=
+000005a0: 2230 220a 2020 2020 2020 2020 2020 2079  "0".           y
+000005b0: 3d22 3022 202f 3e3c 2f67 3e3c 2f63 6c69  ="0" /></g></cli
+000005c0: 7050 6174 683e 3c63 6c69 7050 6174 680a  pPath><clipPath.
+000005d0: 2020 2020 2020 2063 6c69 7050 6174 6855         clipPathU
+000005e0: 6e69 7473 3d22 7573 6572 5370 6163 654f  nits="userSpaceO
+000005f0: 6e55 7365 220a 2020 2020 2020 2069 643d  nUse".       id=
+00000600: 2263 6c69 7050 6174 6836 223e 3c67 0a20  "clipPath6"><g. 
+00000610: 2020 2020 2020 2020 6964 3d22 6737 223e          id="g7">
+00000620: 3c72 6563 740a 2020 2020 2020 2020 2020  <rect.          
+00000630: 2077 6964 7468 3d22 3438 220a 2020 2020   width="48".    
+00000640: 2020 2020 2020 2068 6569 6768 743d 2234         height="4
+00000650: 3822 0a20 2020 2020 2020 2020 2020 6669  8".           fi
+00000660: 6c6c 3d22 2366 6666 6666 6622 0a20 2020  ll="#ffffff".   
+00000670: 2020 2020 2020 2020 6964 3d22 7265 6374          id="rect
+00000680: 3622 0a20 2020 2020 2020 2020 2020 783d  6".           x=
+00000690: 2230 220a 2020 2020 2020 2020 2020 2079  "0".           y
+000006a0: 3d22 3022 202f 3e3c 2f67 3e3c 2f63 6c69  ="0" /></g></cli
+000006b0: 7050 6174 683e 3c63 6c69 7050 6174 680a  pPath><clipPath.
+000006c0: 2020 2020 2020 2063 6c69 7050 6174 6855         clipPathU
+000006d0: 6e69 7473 3d22 7573 6572 5370 6163 654f  nits="userSpaceO
+000006e0: 6e55 7365 220a 2020 2020 2020 2069 643d  nUse".       id=
+000006f0: 2263 6c69 7050 6174 6837 223e 3c67 0a20  "clipPath7"><g. 
+00000700: 2020 2020 2020 2020 6964 3d22 6738 223e          id="g8">
+00000710: 3c72 6563 740a 2020 2020 2020 2020 2020  <rect.          
+00000720: 2077 6964 7468 3d22 3438 220a 2020 2020   width="48".    
+00000730: 2020 2020 2020 2068 6569 6768 743d 2234         height="4
+00000740: 3822 0a20 2020 2020 2020 2020 2020 6669  8".           fi
+00000750: 6c6c 3d22 2366 6666 6666 6622 0a20 2020  ll="#ffffff".   
+00000760: 2020 2020 2020 2020 6964 3d22 7265 6374          id="rect
+00000770: 3722 0a20 2020 2020 2020 2020 2020 783d  7".           x=
+00000780: 2230 220a 2020 2020 2020 2020 2020 2079  "0".           y
+00000790: 3d22 3022 202f 3e3c 2f67 3e3c 2f63 6c69  ="0" /></g></cli
+000007a0: 7050 6174 683e 3c63 6c69 7050 6174 680a  pPath><clipPath.
+000007b0: 2020 2020 2020 2063 6c69 7050 6174 6855         clipPathU
+000007c0: 6e69 7473 3d22 7573 6572 5370 6163 654f  nits="userSpaceO
+000007d0: 6e55 7365 220a 2020 2020 2020 2069 643d  nUse".       id=
+000007e0: 2263 6c69 7050 6174 6838 223e 3c67 0a20  "clipPath8"><g. 
+000007f0: 2020 2020 2020 2020 6964 3d22 6739 223e          id="g9">
+00000800: 3c72 6563 740a 2020 2020 2020 2020 2020  <rect.          
+00000810: 2077 6964 7468 3d22 3438 220a 2020 2020   width="48".    
+00000820: 2020 2020 2020 2068 6569 6768 743d 2234         height="4
+00000830: 3822 0a20 2020 2020 2020 2020 2020 6669  8".           fi
+00000840: 6c6c 3d22 2366 6666 6666 6622 0a20 2020  ll="#ffffff".   
+00000850: 2020 2020 2020 2020 6964 3d22 7265 6374          id="rect
+00000860: 3822 0a20 2020 2020 2020 2020 2020 783d  8".           x=
+00000870: 2230 220a 2020 2020 2020 2020 2020 2079  "0".           y
+00000880: 3d22 3022 202f 3e3c 2f67 3e3c 2f63 6c69  ="0" /></g></cli
+00000890: 7050 6174 683e 3c63 6c69 7050 6174 680a  pPath><clipPath.
+000008a0: 2020 2020 2020 2069 643d 2263 6c69 7030         id="clip0
+000008b0: 5f39 3334 5f39 3439 3322 3e3c 7265 6374  _934_9493"><rect
+000008c0: 0a20 2020 2020 2020 2020 7769 6474 683d  .         width=
+000008d0: 2232 3530 220a 2020 2020 2020 2020 2068  "250".         h
+000008e0: 6569 6768 743d 2232 3530 220a 2020 2020  eight="250".    
+000008f0: 2020 2020 2066 696c 6c3d 2223 6666 6666       fill="#ffff
+00000900: 6666 220a 2020 2020 2020 2020 2069 643d  ff".         id=
+00000910: 2272 6563 7438 2d33 220a 2020 2020 2020  "rect8-3".      
+00000920: 2020 2078 3d22 3022 0a20 2020 2020 2020     x="0".       
+00000930: 2020 793d 2230 2220 2f3e 3c2f 636c 6970    y="0" /></clip
+00000940: 5061 7468 3e3c 2f64 6566 733e 3c70 6174  Path></defs><pat
+00000950: 680a 2020 2020 2069 643d 2270 6174 6831  h.     id="path1
+00000960: 220a 2020 2020 2073 7479 6c65 3d22 6669  ".     style="fi
+00000970: 6c6c 3a6e 6f6e 653b 7374 726f 6b65 2d77  ll:none;stroke-w
+00000980: 6964 7468 3a31 2e31 3333 3835 3832 373b  idth:1.13385827;
+00000990: 7374 726f 6b65 3a23 6666 6666 6666 3b73  stroke:#ffffff;s
+000009a0: 7472 6f6b 652d 6461 7368 6172 7261 793a  troke-dasharray:
+000009b0: 6e6f 6e65 220a 2020 2020 2064 3d22 4d20  none".     d="M 
+000009c0: 3239 2e38 3732 3333 2c31 2e31 3937 3236  29.87233,1.19726
+000009d0: 3536 2032 392e 3432 3131 3538 2c31 2e32  56 29.421158,1.2
+000009e0: 3138 3735 2063 202d 302e 3539 3832 3535  1875 c -0.598255
+000009f0: 2c30 2e30 3330 3334 3820 2d31 2e33 3434  ,0.030348 -1.344
+00000a00: 3132 392c 302e 3330 3937 3737 202d 322e  129,0.309777 -2.
+00000a10: 3231 3438 3434 2c30 2e38 3238 3132 3520  214844,0.828125 
+00000a20: 6c20 2d30 2e37 3130 3933 372c 302e 3432  l -0.710937,0.42
+00000a30: 3338 3238 3120 2d30 2e38 3830 3835 392c  38281 -0.880859,
+00000a40: 302e 3737 3733 3433 3820 2d30 2e38 3832  0.7773438 -0.882
+00000a50: 3831 332c 302e 3737 3733 3433 3720 2d30  813,0.7773437 -0
+00000a60: 2e33 3531 3536 332c 302e 3435 3331 3235  .351563,0.453125
+00000a70: 2063 202d 302e 3630 3339 3239 2c30 2e37   c -0.603929,0.7
+00000a80: 3737 3337 3135 202d 302e 3731 3735 3239  773715 -0.717529
+00000a90: 2c31 2e36 3030 3230 3735 202d 302e 3333  ,1.6002075 -0.33
+00000aa0: 3030 3738 2c32 2e33 3733 3034 3639 2030  0078,2.3730469 0
+00000ab0: 2e32 3530 3238 372c 302e 3439 3932 3338  .250287,0.499238
+00000ac0: 2030 2e32 3334 3539 322c 302e 3632 3537   0.234592,0.6257
+00000ad0: 3836 3320 2d30 2e31 3636 3031 352c 312e  863 -0.166015,1.
+00000ae0: 3430 3233 3433 3720 2d31 2e39 3934 3836  4023437 -1.99486
+00000af0: 312c 332e 3836 3639 3331 3820 2d31 2e32  1,3.8669318 -1.2
+00000b00: 3430 3433 372c 362e 3433 3034 3433 3820  40437,6.4304438 
+00000b10: 322e 3634 3235 3738 2c38 2e39 3836 3332  2.642578,8.98632
+00000b20: 3738 206c 2031 2e30 3636 3430 362c 302e  78 l 1.066406,0.
+00000b30: 3730 3331 3235 2030 2e33 3832 3831 332c  703125 0.382813,
+00000b40: 302e 3435 3131 3732 2030 2e33 3834 3736  0.451172 0.38476
+00000b50: 352c 302e 3435 3331 3235 2030 2e31 3338  5,0.453125 0.138
+00000b60: 3637 322c 302e 3338 3437 3636 2063 2030  672,0.384766 c 0
+00000b70: 2e30 3736 3533 2c30 2e32 3132 3237 3220  .07653,0.212272 
+00000b80: 302e 3132 3336 3039 2c30 2e35 3738 3739  0.123609,0.57879
+00000b90: 3220 302e 3130 3534 3639 2c30 2e38 3132  2 0.105469,0.812
+00000ba0: 3520 6c20 2d30 2e30 3333 322c 302e 3432  5 l -0.0332,0.42
+00000bb0: 3338 3238 202d 302e 3231 3238 3931 2c30  3828 -0.212891,0
+00000bc0: 2e33 3437 3635 3620 6320 2d30 2e32 3036  .347656 c -0.206
+00000bd0: 3330 322c 302e 3333 3635 3239 202d 302e  302,0.336529 -0.
+00000be0: 3439 3536 3039 2c30 2e35 3731 3133 3620  495609,0.571136 
+00000bf0: 2d30 2e38 3333 3938 342c 302e 3730 3530  -0.833984,0.7050
+00000c00: 3738 202d 302e 3030 3139 2c37 2e35 3565  78 -0.0019,7.55e
+00000c10: 2d34 202d 302e 3030 342c 302e 3030 3132  -4 -0.004,0.0012
+00000c20: 202d 302e 3030 3539 2c30 2e30 3032 202d   -0.0059,0.002 -
+00000c30: 302e 3237 3138 3837 2c30 2e31 3036 3933  0.271887,0.10693
+00000c40: 3220 2d30 2e35 3735 3737 352c 302e 3134  2 -0.575775,0.14
+00000c50: 3533 3520 2d30 2e38 3934 3533 312c 302e  535 -0.894531,0.
+00000c60: 3131 3731 3837 202d 302e 3039 3133 382c  117187 -0.09138,
+00000c70: 2d30 2e30 3038 3120 2d30 2e31 3833 3836  -0.0081 -0.18386
+00000c80: 382c 2d30 2e30 3233 3439 202d 302e 3237  8,-0.02349 -0.27
+00000c90: 3733 3434 2c2d 302e 3034 3239 3720 2d30  7344,-0.04297 -0
+00000ca0: 2e30 3331 3234 2c2d 302e 3030 3635 202d  .03124,-0.0065 -
+00000cb0: 302e 3036 3233 332c 2d30 2e30 3039 3820  0.06233,-0.0098 
+00000cc0: 2d30 2e30 3933 3735 2c2d 302e 3031 3735  -0.09375,-0.0175
+00000cd0: 3820 2d30 2e31 3135 3533 362c 2d30 2e30  8 -0.115536,-0.0
+00000ce0: 3238 3637 202d 302e 3233 3236 3134 2c2d  2867 -0.232614,-
+00000cf0: 302e 3036 3930 3320 2d30 2e33 3439 3630  0.06903 -0.34960
+00000d00: 392c 2d30 2e31 3135 3233 3420 2d30 2e30  9,-0.115234 -0.0
+00000d10: 3431 3234 2c2d 302e 3031 3632 3920 2d30  4124,-0.01629 -0
+00000d20: 2e30 3831 3735 2c2d 302e 3033 3432 3520  .08175,-0.03425 
+00000d30: 2d30 2e31 3233 3034 372c 2d30 2e30 3532  -0.123047,-0.052
+00000d40: 3733 202d 302e 3132 3235 3432 2c2d 302e  73 -0.122542,-0.
+00000d50: 3035 3438 3620 2d30 2e32 3435 3233 322c  05486 -0.245232,
+00000d60: 2d30 2e31 3135 3032 3920 2d30 2e33 3637  -0.115029 -0.367
+00000d70: 3138 372c 2d30 2e31 3839 3435 3320 4c20  187,-0.189453 L 
+00000d80: 3235 2e30 3138 3737 372c 3230 2e39 3830  25.018777,20.980
+00000d90: 3531 3720 3234 2e32 3139 3934 392c 3230  517 24.219949,20
+00000da0: 2e31 3634 3131 2063 202d 302e 3230 3432  .16411 c -0.2042
+00000db0: 3838 2c2d 302e 3230 3932 3332 202d 302e  88,-0.209232 -0.
+00000dc0: 3530 3832 3235 2c2d 302e 3534 3831 3934  508225,-0.548194
+00000dd0: 202d 302e 3833 3339 3834 2c2d 302e 3932   -0.833984,-0.92
+00000de0: 3338 3238 202d 302e 3032 3732 312c 2d30  3828 -0.02721,-0
+00000df0: 2e30 3331 3334 202d 302e 3034 3237 392c  .03134 -0.04279,
+00000e00: 2d30 2e30 3436 3233 202d 302e 3037 3033  -0.04623 -0.0703
+00000e10: 312c 2d30 2e30 3738 3133 202d 332e 3465  1,-0.07813 -3.4e
+00000e20: 2d34 2c2d 332e 3934 652d 3420 332e 3431  -4,-3.94e-4 3.41
+00000e30: 652d 342c 2d30 2e30 3031 3620 302c 2d30  e-4,-0.0016 0,-0
+00000e40: 2e30 3032 202d 302e 3335 3430 3631 2c2d  .002 -0.354061,-
+00000e50: 302e 3431 3033 3620 2d30 2e37 3331 3538  0.41036 -0.73158
+00000e60: 362c 2d30 2e38 3632 3438 3920 2d31 2e30  6,-0.862489 -1.0
+00000e70: 3438 3832 382c 2d31 2e32 3539 3736 3520  48828,-1.259765 
+00000e80: 2d30 2e31 3433 3839 312c 2d30 2e31 3830  -0.143891,-0.180
+00000e90: 3139 3420 2d30 2e32 3835 3438 322c 2d30  194 -0.285482,-0
+00000ea0: 2e33 3533 3336 3420 2d30 2e34 3235 3738  .353364 -0.42578
+00000eb0: 312c 2d30 2e35 3231 3438 3520 2d30 2e30  1,-0.521485 -0.0
+00000ec0: 3536 3738 2c2d 302e 3036 3830 3420 2d30  5678,-0.06804 -0
+00000ed0: 2e31 3133 3636 322c 2d30 2e31 3335 3037  .113662,-0.13507
+00000ee0: 3220 2d30 2e31 3639 3932 322c 2d30 2e32  2 -0.169922,-0.2
+00000ef0: 3031 3137 3220 2d30 2e34 3930 3131 372c  01172 -0.490117,
+00000f00: 2d30 2e35 3735 3834 3320 2d30 2e39 3632  -0.575843 -0.962
+00000f10: 3338 342c 2d31 2e30 3738 3033 3320 2d31  384,-1.078033 -1
+00000f20: 2e34 3235 3738 312c 2d31 2e35 3133 3637  .425781,-1.51367
+00000f30: 3220 2d30 2e30 3138 3939 2c2d 302e 3031  2 -0.01899,-0.01
+00000f40: 3738 3520 2d30 2e30 3337 3938 2c2d 302e  785 -0.03798,-0.
+00000f50: 3033 3530 3220 2d30 2e30 3536 3634 2c2d  03502 -0.05664,-
+00000f60: 302e 3035 3237 3320 2d30 2e33 3033 3535  0.05273 -0.30355
+00000f70: 382c 2d30 2e32 3832 3135 3120 2d30 2e36  8,-0.282151 -0.6
+00000f80: 3033 3336 372c 2d30 2e35 3336 3935 3120  03367,-0.536951 
+00000f90: 2d30 2e39 3034 3239 372c 2d30 2e37 3633  -0.904297,-0.763
+00000fa0: 3637 3220 2d30 2e30 3034 352c 2d30 2e30  672 -0.0045,-0.0
+00000fb0: 3033 3420 2d30 2e30 3039 322c 2d30 2e30  034 -0.0092,-0.0
+00000fc0: 3036 3420 2d30 2e30 3133 3637 2c2d 302e  064 -0.01367,-0.
+00000fd0: 3030 3938 202d 302e 3137 3534 3333 2c2d  0098 -0.175433,-
+00000fe0: 302e 3133 3137 3031 202d 302e 3335 3039  0.131701 -0.3509
+00000ff0: 372c 2d30 2e32 3535 3236 3620 2d30 2e35  7,-0.255266 -0.5
+00001000: 3237 3334 342c 2d30 2e33 3639 3134 3120  27344,-0.369141 
+00001010: 2d30 2e33 3132 3635 392c 2d30 2e32 3031  -0.312659,-0.201
+00001020: 3836 3620 2d30 2e36 3237 3832 372c 2d30  866 -0.627827,-0
+00001030: 2e33 3736 3335 3820 2d30 2e39 3439 3231  .376358 -0.94921
+00001040: 392c 2d30 2e35 3235 3339 3120 2d30 2e31  9,-0.525391 -0.1
+00001050: 3632 3133 372c 2d30 2e30 3735 3138 202d  62137,-0.07518 -
+00001060: 302e 3332 3634 3134 2c2d 302e 3134 3235  0.326414,-0.1425
+00001070: 3620 2d30 2e34 3932 3138 372c 2d30 2e32  6 -0.492187,-0.2
+00001080: 3035 3037 3820 2d30 2e30 3434 3833 2c2d  05078 -0.04483,-
+00001090: 302e 3031 3639 202d 302e 3038 3936 332c  0.0169 -0.08963,
+000010a0: 2d30 2e30 3334 3738 202d 302e 3133 3437  -0.03478 -0.1347
+000010b0: 3636 2c2d 302e 3035 3037 3820 2d30 2e30  66,-0.05078 -0.0
+000010c0: 3033 332c 2d30 2e30 3031 3220 2d30 2e30  033,-0.0012 -0.0
+000010d0: 3036 352c 2d30 2e30 3032 3720 2d30 2e30  065,-0.0027 -0.0
+000010e0: 3039 382c 2d30 2e30 3033 3920 2d30 2e38  098,-0.0039 -0.8
+000010f0: 3630 3434 332c 2d30 2e33 3033 3632 3620  60443,-0.303626 
+00001100: 2d31 2e37 3737 3838 322c 2d30 2e34 3435  -1.777882,-0.445
+00001110: 3939 202d 322e 3832 3032 3436 2c2d 302e  99 -2.820246,-0.
+00001120: 3435 3839 3537 202d 302e 3231 3137 3536  458957 -0.211756
+00001130: 2c2d 302e 3030 3236 202d 302e 3432 3938  ,-0.0026 -0.4298
+00001140: 3534 2c32 2e32 652d 3420 2d30 2e36 3532  54,2.2e-4 -0.652
+00001150: 3334 342c 302e 3030 3738 206c 202d 302e  344,0.0078 l -0.
+00001160: 3833 3539 3337 2c30 2e30 3239 3320 2d30  835937,0.0293 -0
+00001170: 2e36 3831 3634 312c 302e 3231 3637 3937  .681641,0.216797
+00001180: 2063 202d 302e 3832 3736 3837 2c30 2e32   c -0.827687,0.2
+00001190: 3634 3338 3520 2d31 2e33 3331 3039 322c  64385 -1.331092,
+000011a0: 302e 3533 3738 3033 202d 322e 3034 3638  0.537803 -2.0468
+000011b0: 3735 2c31 2e31 3039 3337 3520 6c20 2d30  75,1.109375 l -0
+000011c0: 2e35 3432 3936 392c 302e 3433 3335 3920  .542969,0.43359 
+000011d0: 2d30 2e34 3134 3036 322c 302e 3531 3137  -0.414062,0.5117
+000011e0: 3139 2063 202d 312e 3832 3631 3037 2c32  19 c -1.826107,2
+000011f0: 2e32 3632 3333 3720 2d32 2e30 3536 3232  .262337 -2.05622
+00001200: 372c 352e 3132 3831 3820 2d30 2e36 3031  7,5.12818 -0.601
+00001210: 3536 332c 372e 3439 3830 3620 6c20 302e  563,7.49806 l 0.
+00001220: 3239 3638 3735 2c30 2e34 3832 3432 3220  296875,0.482422 
+00001230: 302e 3630 3534 3639 2c30 2e36 3037 3432  0.605469,0.60742
+00001240: 3220 6320 312e 3331 3439 3431 2c31 2e33  2 c 1.314941,1.3
+00001250: 3231 3838 2032 2e38 3535 3539 382c 322e  2188 2.855598,2.
+00001260: 3130 3833 3936 2035 2e38 3930 3632 352c  108396 5.890625,
+00001270: 332e 3030 3139 3533 2037 2e32 3538 332c  3.001953 7.2583,
+00001280: 322e 3133 3639 3532 2039 2e32 3731 3837  2.136952 9.27187
+00001290: 312c 332e 3537 3735 3639 2038 2e34 3630  1,3.577569 8.460
+000012a0: 3933 372c 362e 3035 3436 3837 206c 202d  937,6.054687 l -
+000012b0: 302e 3134 3036 3235 2c30 2e34 3331 3634  0.140625,0.43164
+000012c0: 3120 2d30 2e33 3034 3638 372c 302e 3336  1 -0.304687,0.36
+000012d0: 3532 3334 202d 302e 3330 3436 3838 2c30  5234 -0.304688,0
+000012e0: 2e33 3635 3233 3520 2d30 2e33 3431 3739  .365235 -0.34179
+000012f0: 372c 302e 3135 3233 3434 2063 202d 312e  7,0.152344 c -1.
+00001300: 3337 3035 3036 2c30 2e36 3132 3939 3120  370506,0.612991 
+00001310: 2d32 2e36 3535 3639 352c 2d30 2e30 3130  -2.655695,-0.010
+00001320: 3133 202d 352e 3533 3332 3033 2c2d 322e  13 -5.533203,-2.
+00001330: 3638 3136 3431 206c 202d 312e 3535 3636  681641 l -1.5566
+00001340: 342c 2d31 2e34 3435 3331 3320 2d30 2e35  4,-1.445313 -0.5
+00001350: 3937 3635 362c 2d30 2e34 3134 3036 3220  97656,-0.414062 
+00001360: 4320 3132 2e39 3239 3630 372c 3238 2e34  C 12.929607,28.4
+00001370: 3834 3834 3920 3131 2e31 3831 3238 322c  84849 11.181282,
+00001380: 3237 2e39 3831 3638 3120 392e 3736 3638  27.981681 9.7668
+00001390: 3631 2c32 382e 3433 3535 3437 206c 202d  61,28.435547 l -
+000013a0: 302e 3339 3235 3738 2c30 2e31 3235 202d  0.392578,0.125 -
+000013b0: 302e 3436 3438 3434 2c30 2e34 3132 3130  0.464844,0.41210
+000013c0: 3920 2d30 2e34 3632 3839 2c30 2e34 3132  9 -0.46289,0.412
+000013d0: 3131 202d 302e 3234 3431 3431 2c30 2e34  11 -0.244141,0.4
+000013e0: 3339 3435 3320 6320 2d30 2e36 3739 3936  39453 c -0.67996
+000013f0: 342c 312e 3233 3137 3433 202d 302e 3632  4,1.231743 -0.62
+00001400: 3930 3935 2c32 2e34 3237 3939 3820 302e  9095,2.427998 0.
+00001410: 3135 3832 3033 2c33 2e37 3334 3337 3520  158203,3.734375 
+00001420: 6c20 302e 3237 3533 3931 2c30 2e34 3537  l 0.275391,0.457
+00001430: 3033 3120 312e 3330 3835 3934 2c31 2e34  031 1.308594,1.4
+00001440: 3032 3334 3420 312e 3331 3035 3437 2c31  02344 1.310547,1
+00001450: 2e34 3034 3239 3720 302e 3234 3431 342c  .404297 0.24414,
+00001460: 302e 3437 3635 3632 2063 2030 2e38 3037  0.476562 c 0.807
+00001470: 3739 372c 312e 3537 3835 3431 2030 2e35  797,1.578541 0.5
+00001480: 3437 3633 392c 332e 3437 3033 3239 202d  47639,3.470329 -
+00001490: 302e 3831 3833 3539 2c35 2e39 3333 3539  0.818359,5.93359
+000014a0: 3420 2d30 2e35 3739 3737 372c 312e 3034  4 -0.579777,1.04
+000014b0: 3534 3937 202d 302e 3535 3833 392c 312e  5497 -0.55839,1.
+000014c0: 3133 3036 3536 2030 2e31 3139 3134 2c30  130656 0.11914,0
+000014d0: 2e34 3533 3132 3520 302e 3933 3530 392c  .453125 0.93509,
+000014e0: 2d30 2e39 3335 3039 2031 2e36 3132 3332  -0.93509 1.61232
+000014f0: 342c 2d32 2e30 3337 3539 3620 322e 3037  4,-2.037596 2.07
+00001500: 3033 3133 2c2d 332e 3337 3330 3437 206c  0313,-3.373047 l
+00001510: 2030 2e32 352c 2d30 2e37 3330 3436 3920   0.25,-0.730469 
+00001520: 302e 3030 322c 2d30 2e38 3731 3039 3320  0.002,-0.871093 
+00001530: 302e 3030 3139 2c2d 302e 3837 3130 3934  0.0019,-0.871094
+00001540: 202d 302e 3232 3635 3633 2c2d 302e 3639   -0.226563,-0.69
+00001550: 3732 3636 2043 2031 322e 3533 3530 3332  7266 C 12.535032
+00001560: 2c33 362e 3032 3731 3639 2031 322e 3237  ,36.027169 12.27
+00001570: 3138 3937 2c33 352e 3631 3233 3620 3130  1897,35.61236 10
+00001580: 2e39 3235 3036 342c 3334 2e30 3335 3135  .925064,34.03515
+00001590: 3620 392e 3635 3439 3333 2c33 322e 3534  6 9.654933,32.54
+000015a0: 3737 3735 2039 2e34 3835 3336 362c 3332  7775 9.485366,32
+000015b0: 2e32 3138 3939 2039 2e35 3931 3038 2c33  .21899 9.59108,3
+000015c0: 312e 3433 3335 3934 206c 2030 2e30 3530  1.433594 l 0.050
+000015d0: 3738 2c2d 302e 3337 3520 302e 3330 3835  78,-0.375 0.3085
+000015e0: 3934 2c2d 302e 3335 3534 3639 2030 2e33  94,-0.355469 0.3
+000015f0: 3036 3634 2c2d 302e 3335 3534 3639 2030  0664,-0.355469 0
+00001600: 2e34 3034 3239 372c 2d30 2e30 3237 3334  .404297,-0.02734
+00001610: 2063 2030 2e38 3831 3235 392c 2d30 2e30   c 0.881259,-0.0
+00001620: 3537 3234 2032 2e31 3037 3739 392c 302e  5724 2.107799,0.
+00001630: 3537 3530 3437 2033 2e36 3935 3331 332c  575047 3.695313,
+00001640: 312e 3930 3233 3434 206c 2030 2e37 3533  1.902344 l 0.753
+00001650: 3930 362c 302e 3632 3839 3036 2031 2e30  906,0.628906 1.0
+00001660: 3837 3839 312c 312e 3232 3635 3633 2031  87891,1.226563 1
+00001670: 2e30 3839 3834 342c 312e 3232 3635 3633  .089844,1.226563
+00001680: 2030 2e36 3133 3238 312c 302e 3437 3835   0.613281,0.4785
+00001690: 3135 2063 2032 2e35 3436 3835 342c 312e  15 c 2.546854,1.
+000016a0: 3938 3738 3435 2035 2e34 3437 3639 2c32  987845 5.44769,2
+000016b0: 2e33 3436 3438 3220 372e 3338 3637 3139  .346482 7.386719
+000016c0: 2c30 2e39 3134 3036 3320 302e 3734 3739  ,0.914063 0.7479
+000016d0: 312c 2d30 2e35 3532 3530 3620 312e 3339  1,-0.552506 1.39
+000016e0: 3039 3131 2c2d 312e 3439 3738 3433 2031  0911,-1.497843 1
+000016f0: 2e37 3833 3230 332c 2d32 2e36 3233 3034  .783203,-2.62304
+00001700: 3720 6c20 302e 3235 3339 3036 2c2d 302e  7 l 0.253906,-0.
+00001710: 3732 3635 3633 2030 2e30 3033 392c 2d30  726563 0.0039,-0
+00001720: 2e39 3331 3634 2030 2e30 3033 392c 2d30  .93164 0.0039,-0
+00001730: 2e39 3331 3634 3120 2d30 2e32 352c 2d30  .931641 -0.25,-0
+00001740: 2e37 3332 3432 3220 4320 3236 2e39 3435  .732422 C 26.945
+00001750: 3531 372c 3330 2e33 3439 3835 3520 3236  517,30.349855 26
+00001760: 2e36 3739 362c 3239 2e37 3836 3236 3820  .6796,29.786268 
+00001770: 3236 2e34 3931 3437 312c 3239 2e34 3938  26.491471,29.498
+00001780: 3034 3720 6c20 2d30 2e33 3433 3735 2c2d  047 l -0.34375,-
+00001790: 302e 3532 3533 3931 202d 302e 3935 3131  0.525391 -0.9511
+000017a0: 3732 2c2d 302e 3839 3435 3331 202d 302e  72,-0.894531 -0.
+000017b0: 3935 3331 3235 2c2d 302e 3839 3435 3331  953125,-0.894531
+000017c0: 202d 302e 3538 3030 3738 2c2d 302e 3334   -0.580078,-0.34
+000017d0: 3537 3033 2043 2032 322e 3637 3932 332c  5703 C 22.67923,
+000017e0: 3236 2e32 3439 3436 3120 3231 2e34 3835  26.249461 21.485
+000017f0: 3236 312c 3235 2e37 3730 3539 3620 3138  261,25.770596 18
+00001800: 2e34 3434 3539 362c 3234 2e37 3438 3034  .444596,24.74804
+00001810: 3720 3135 2e31 3639 312c 3233 2e36 3436  7 15.1691,23.646
+00001820: 3532 3620 3134 2e34 3130 3138 342c 3233  526 14.410184,23
+00001830: 2e33 3434 3039 3620 3133 2e33 3231 3534  .344096 13.32154
+00001840: 392c 3232 2e37 3031 3137 3220 4c20 3132  9,22.701172 L 12
+00001850: 2e35 3637 3634 332c 3232 2e32 3535 3835  .567643,22.25585
+00001860: 3920 3132 2e31 3533 3538 2c32 312e 3738  9 12.15358,21.78
+00001870: 3930 3632 2031 312e 3733 3735 3634 2c32  9062 11.737564,2
+00001880: 312e 3332 3432 3139 2031 312e 3535 3938  1.324219 11.5598
+00001890: 332c 3230 2e38 3437 3635 3620 6320 2d30  3,20.847656 c -0
+000018a0: 2e32 3235 3338 342c 2d30 2e36 3036 3031  .225384,-0.60601
+000018b0: 3220 2d30 2e32 3536 3835 332c 2d31 2e33  2 -0.256853,-1.3
+000018c0: 3837 3431 3720 2d30 2e30 3830 3038 2c2d  87417 -0.08008,-
+000018d0: 312e 3935 3530 3738 206c 2030 2e31 3338  1.955078 l 0.138
+000018e0: 3637 322c 2d30 2e34 3433 3335 3920 302e  672,-0.443359 0.
+000018f0: 3439 3032 3334 2c2d 302e 3439 3231 3838  490234,-0.492188
+00001900: 2030 2e34 3930 3233 352c 2d30 2e34 3932   0.490235,-0.492
+00001910: 3138 3720 302e 3437 3635 3632 2c2d 302e  187 0.476562,-0.
+00001920: 3137 3138 3735 2063 2031 2e32 3732 3331  171875 c 1.27231
+00001930: 342c 2d30 2e34 3630 3033 3420 322e 3633  4,-0.460034 2.63
+00001940: 3635 3938 2c2d 302e 3136 3731 3637 2034  6598,-0.167167 4
+00001950: 2e30 3832 3033 312c 302e 3836 3931 3420  .082031,0.86914 
+00001960: 302e 3034 3830 382c 302e 3033 3434 3720  0.04808,0.03447 
+00001970: 302e 3039 3632 382c 302e 3037 3332 3620  0.09628,0.07326 
+00001980: 302e 3134 3435 3332 2c30 2e31 3039 3337  0.144532,0.10937
+00001990: 3520 302e 3038 3131 382c 302e 3036 3037  5 0.08118,0.0607
+000019a0: 3520 302e 3136 3234 3633 2c30 2e31 3232  5 0.162463,0.122
+000019b0: 3130 3320 302e 3234 3431 342c 302e 3138  103 0.24414,0.18
+000019c0: 3735 2030 2e30 3630 3138 2c30 2e30 3438  75 0.06018,0.048
+000019d0: 3138 2030 2e31 3231 3139 332c 302e 3039  18 0.121193,0.09
+000019e0: 3737 3320 302e 3138 3136 3431 2c30 2e31  773 0.181641,0.1
+000019f0: 3438 3433 3820 302e 3037 3232 362c 302e  48438 0.07226,0.
+00001a00: 3036 3036 3220 302e 3134 3431 3439 2c30  06062 0.144149,0
+00001a10: 2e31 3233 3237 3220 302e 3231 3637 3937  .123272 0.216797
+00001a20: 2c30 2e31 3837 3520 302e 3230 3331 352c  ,0.1875 0.20315,
+00001a30: 302e 3137 3936 3038 2030 2e34 3037 3136  0.179608 0.40716
+00001a40: 372c 302e 3337 3232 3432 2030 2e36 3133  7,0.372242 0.613
+00001a50: 3238 312c 302e 3538 3030 3738 2030 2e31  281,0.580078 0.1
+00001a60: 3139 3730 312c 302e 3132 3037 3032 2030  19701,0.120702 0
+00001a70: 2e32 3430 3634 332c 302e 3234 3637 3237  .240643,0.246727
+00001a80: 2030 2e33 3631 3332 382c 302e 3337 3639   0.361328,0.3769
+00001a90: 3533 2030 2e30 3633 3735 2c30 2e30 3638  53 0.06375,0.068
+00001aa0: 3739 2030 2e31 3237 3338 362c 302e 3133  79 0.127386,0.13
+00001ab0: 3934 3932 2030 2e31 3931 3430 362c 302e  9492 0.191406,0.
+00001ac0: 3231 3039 3338 2030 2e32 3631 3339 372c  210938 0.261397,
+00001ad0: 302e 3239 3137 3135 2030 2e35 3235 3135  0.291715 0.52515
+00001ae0: 352c 302e 3630 3334 3038 2030 2e37 3931  5,0.603408 0.791
+00001af0: 3031 362c 302e 3933 3934 3533 2030 2e34  016,0.939453 0.4
+00001b00: 3736 3930 382c 302e 3630 3238 3039 2031  76908,0.602809 1
+00001b10: 2e32 3230 3835 322c 312e 3434 3932 3639  .220852,1.449269
+00001b20: 2031 2e36 3534 3239 372c 312e 3838 3238   1.654297,1.8828
+00001b30: 3132 206c 2030 2e37 3839 3036 322c 302e  12 l 0.789062,0.
+00001b40: 3738 3930 3633 2030 2e37 3637 3537 382c  789063 0.767578,
+00001b50: 302e 3534 3239 3639 2063 2031 2e36 3431  0.542969 c 1.641
+00001b60: 3632 382c 312e 3135 3838 3039 2033 2e30  628,1.158809 3.0
+00001b70: 3438 3331 342c 312e 3631 3930 3439 2034  48314,1.619049 4
+00001b80: 2e37 3837 3131 2c31 2e35 3638 3335 3920  .78711,1.568359 
+00001b90: 6c20 302e 3738 3930 3632 2c2d 302e 3032  l 0.789062,-0.02
+00001ba0: 3334 3420 302e 3731 3637 3937 2c2d 302e  344 0.716797,-0.
+00001bb0: 3234 3431 3420 6320 302e 3131 3237 3133  24414 c 0.112713
+00001bc0: 2c2d 302e 3033 3833 3720 302e 3231 3836  ,-0.03837 0.2186
+00001bd0: 3137 2c2d 302e 3037 3836 3220 302e 3332  17,-0.07862 0.32
+00001be0: 3033 3133 2c2d 302e 3131 3931 3431 206c  0313,-0.119141 l
+00001bf0: 202d 302e 3030 3339 2c2d 302e 3030 3539   -0.0039,-0.0059
+00001c00: 2063 2030 2e36 3834 3333 312c 2d30 2e32   c 0.684331,-0.2
+00001c10: 3734 3231 3120 312e 3135 3730 3738 2c2d  74211 1.157078,-
+00001c20: 302e 3631 3038 3733 2031 2e37 3130 3933  0.610873 1.71093
+00001c30: 382c 2d31 2e32 3334 3337 3520 6c20 302e  8,-1.234375 l 0.
+00001c40: 3438 3832 3831 2c2d 302e 3535 3037 3832  488281,-0.550782
+00001c50: 2030 2e33 3333 3938 342c 2d30 2e36 3733   0.333984,-0.673
+00001c60: 3832 3820 6320 302e 3931 3437 3131 2c2d  828 c 0.914711,-
+00001c70: 312e 3834 3734 3138 2030 2e38 3330 3039  1.847418 0.83009
+00001c80: 362c 2d33 2e36 3635 3231 202d 302e 3235  6,-3.66521 -0.25
+00001c90: 2c2d 352e 3336 3332 3831 204c 2033 312e  ,-5.363281 L 31.
+00001ca0: 3634 3936 3739 2c31 362e 3931 3430 3139  649679,16.914019
+00001cb0: 2033 302e 3830 3339 3736 2c31 362e 3133   30.803976,16.13
+00001cc0: 3038 3136 2032 392e 3935 3832 3733 2c31  0816 29.958273,1
+00001cd0: 352e 3334 3935 3636 2032 392e 3239 3432  5.349566 29.2942
+00001ce0: 312c 3134 2e39 3732 3631 3320 4320 3238  1,14.972613 C 28
+00001cf0: 2e39 3239 3036 342c 3134 2e37 3636 3138  .929064,14.76618
+00001d00: 2032 382e 3337 3139 3238 2c31 342e 3436   28.371928,14.46
+00001d10: 3639 3831 2032 382e 3035 3539 3234 2c31  6981 28.055924,1
+00001d20: 342e 3330 3636 3431 2032 372e 3733 3939  4.306641 27.7399
+00001d30: 3138 2c31 342e 3134 3633 2032 372e 3236  18,14.1463 27.26
+00001d40: 3136 3233 2c31 332e 3835 3839 3936 2032  1623,13.858996 2
+00001d50: 362e 3939 3334 3234 2c31 332e 3636 3739  6.993424,13.6679
+00001d60: 3639 206c 202d 302e 3438 3832 3832 2c2d  69 l -0.488282,-
+00001d70: 302e 3334 3736 3537 202d 302e 3233 3832  0.347657 -0.2382
+00001d80: 3831 2c2d 302e 3336 3731 3837 2063 202d  81,-0.367187 c -
+00001d90: 302e 3539 3137 3537 2c2d 302e 3931 3438  0.591757,-0.9148
+00001da0: 3636 202d 302e 3536 3235 392c 2d32 2e33  66 -0.56259,-2.3
+00001db0: 3434 3530 3220 302e 3037 3432 322c 2d33  44502 0.07422,-3
+00001dc0: 2e37 3037 3033 3132 204c 2032 362e 3537  .7070312 L 26.57
+00001dd0: 3734 3038 2c38 2e37 3338 3238 3132 2032  7408,8.7382812 2
+00001de0: 362e 3930 3335 382c 382e 3639 3533 3132  6.90358,8.695312
+00001df0: 3520 4320 3237 2e30 3833 3539 322c 382e  5 C 27.083592,8.
+00001e00: 3637 3130 3833 3520 3237 2e34 3938 3134  6710835 27.49814
+00001e10: 2c38 2e35 3535 3130 3238 2032 372e 3832  ,8.5551028 27.82
+00001e20: 3335 3032 2c38 2e34 3337 3520 4c20 3238  3502,8.4375 L 28
+00001e30: 2e34 3135 3239 392c 382e 3232 3236 3536  .415299,8.222656
+00001e40: 3220 3238 2e39 3835 3631 312c 372e 3639  2 28.985611,7.69
+00001e50: 3732 3635 3620 3239 2e35 3537 3837 372c  72656 29.557877,
+00001e60: 372e 3136 3939 3231 3920 3239 2e38 3636  7.1699219 29.866
+00001e70: 3437 312c 362e 3535 3436 3837 3520 4320  471,6.5546875 C 
+00001e80: 3330 2e37 3938 3535 312c 342e 3639 3530  30.798551,4.6950
+00001e90: 3930 3320 3331 2e30 3935 3131 332c 322e  903 31.095113,2.
+00001ea0: 3730 3935 3137 3220 3330 2e35 3737 3430  7095172 30.57740
+00001eb0: 382c 312e 3739 3638 3735 204c 2033 302e  8,1.796875 L 30.
+00001ec0: 3431 3133 3932 2c31 2e35 3035 3835 3934  411392,1.5058594
+00001ed0: 2033 302e 3134 3138 3631 2c31 2e33 3531   30.141861,1.351
+00001ee0: 3536 3235 205a 2220 2f3e 3c70 6174 680a  5625 Z" /><path.
+00001ef0: 2020 2020 2069 643d 2270 6174 6837 220a       id="path7".
+00001f00: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
+00001f10: 3a23 6661 3638 3633 3b66 696c 6c2d 6f70  :#fa6863;fill-op
+00001f20: 6163 6974 793a 313b 7374 726f 6b65 2d77  acity:1;stroke-w
+00001f30: 6964 7468 3a30 2e33 3731 3631 3922 0a20  idth:0.371619". 
+00001f40: 2020 2020 643d 224d 2037 2e30 3539 3639      d="M 7.05969
+00001f50: 3838 2c32 352e 3033 3535 3837 2048 2031  88,25.035587 H 1
+00001f60: 352e 3930 3534 3031 2056 2034 382e 3035  5.905401 V 48.05
+00001f70: 3132 3133 2048 2037 2e30 3539 3639 3838  1213 H 7.0596988
+00001f80: 205a 220a 2020 2020 2073 6f64 6970 6f64   Z".     sodipod
+00001f90: 693a 6e6f 6465 7479 7065 733d 2263 6363  i:nodetypes="ccc
+00001fa0: 6363 2220 2f3e 3c70 6174 680a 2020 2020  cc" /><path.    
+00001fb0: 2069 643d 2270 6174 6836 220a 2020 2020   id="path6".    
+00001fc0: 2073 7479 6c65 3d22 6669 6c6c 3a23 6631   style="fill:#f1
+00001fd0: 3830 3436 3b73 7472 6f6b 652d 7769 6474  8046;stroke-widt
+00001fe0: 683a 302e 3337 3136 3139 3b66 696c 6c2d  h:0.371619;fill-
+00001ff0: 6f70 6163 6974 793a 3122 0a20 2020 2020  opacity:1".     
+00002000: 643d 226d 2033 322e 3039 3337 382c 302e  d="m 32.09378,0.
+00002010: 3035 3230 3238 2068 2038 2e38 3435 3730  052028 h 8.84570
+00002020: 3320 4320 3430 2e34 3231 3038 342c 3132  3 C 40.421084,12
+00002030: 2e35 3138 3531 3620 3330 2e33 3936 3234  .518516 30.39624
+00002040: 362c 3232 2e35 3235 3337 3220 3137 2e39  6,22.525372 17.9
+00002050: 3233 3835 382c 3233 2e30 3136 3837 3220  23858,23.016872 
+00002060: 7620 2d38 2e38 3433 3735 2043 2032 352e  v -8.84375 C 25.
+00002070: 3530 3539 3531 2c31 332e 3639 3639 3232  505951,13.696922
+00002080: 2033 312e 3539 3037 3431 2c37 2e36 3236   31.590741,7.626
+00002090: 3432 3120 3332 2e30 3933 3738 2c30 2e30  421 32.09378,0.0
+000020a0: 3532 3032 3820 5a22 0a20 2020 2020 736f  52028 Z".     so
+000020b0: 6469 706f 6469 3a6e 6f64 6574 7970 6573  dipodi:nodetypes
+000020c0: 3d22 6363 6363 6322 202f 3e3c 7061 7468  ="ccccc" /><path
+000020d0: 0a20 2020 2020 6964 3d22 7061 7468 3522  .     id="path5"
+000020e0: 0a20 2020 2020 7374 796c 653d 2266 696c  .     style="fil
+000020f0: 6c3a 2330 6463 3039 643b 7374 726f 6b65  l:#0dc09d;stroke
+00002100: 2d77 6964 7468 3a30 2e33 3731 3631 393b  -width:0.371619;
+00002110: 6669 6c6c 2d6f 7061 6369 7479 3a31 220a  fill-opacity:1".
+00002120: 2020 2020 2064 3d22 4d20 372e 3035 3936       d="M 7.0596
+00002130: 3938 352c 362e 3837 3135 652d 3420 4820  985,6.8715e-4 H 
+00002140: 3135 2e39 3035 3430 3120 5620 3233 2e30  15.905401 V 23.0
+00002150: 3136 3331 3320 4820 372e 3035 3936 3938  16313 H 7.059698
+00002160: 3520 5a22 0a20 2020 2020 736f 6469 706f  5 Z".     sodipo
+00002170: 6469 3a6e 6f64 6574 7970 6573 3d22 6363  di:nodetypes="cc
+00002180: 6363 6322 202f 3e3c 7061 7468 0a20 2020  ccc" /><path.   
+00002190: 2020 6964 3d22 7061 7468 3130 220a 2020    id="path10".  
+000021a0: 2020 2073 7479 6c65 3d22 6669 6c6c 3a23     style="fill:#
+000021b0: 3364 3935 6664 3b73 7472 6f6b 652d 7769  3d95fd;stroke-wi
+000021c0: 6474 683a 302e 3337 3136 3139 3b66 696c  dth:0.371619;fil
+000021d0: 6c2d 6f70 6163 6974 793a 3122 0a20 2020  l-opacity:1".   
+000021e0: 2020 643d 226d 2033 322e 3036 3738 3239    d="m 32.067829
+000021f0: 2c34 382e 3032 3538 3232 2068 2038 2e38  ,48.025822 h 8.8
+00002200: 3435 3730 3320 4320 3430 2e33 3935 3133  45703 C 40.39513
+00002210: 332c 3335 2e35 3539 3333 3220 3330 2e33  3,35.559332 30.3
+00002220: 3730 3239 352c 3235 2e35 3532 3437 3720  70295,25.552477 
+00002230: 3137 2e38 3937 3930 372c 3235 2e30 3630  17.897907,25.060
+00002240: 3937 3720 7620 382e 3834 3337 3435 2063  977 v 8.843745 c
+00002250: 2037 2e35 3832 3039 332c 302e 3437 3632   7.582093,0.4762
+00002260: 3120 3133 2e36 3636 3838 332c 362e 3534  1 13.666883,6.54
+00002270: 3637 3120 3134 2e31 3639 3932 322c 3134  671 14.169922,14
+00002280: 2e31 3231 3120 7a22 0a20 2020 2020 736f  .1211 z".     so
+00002290: 6469 706f 6469 3a6e 6f64 6574 7970 6573  dipodi:nodetypes
+000022a0: 3d22 6363 6363 6322 202f 3e3c 7061 7468  ="ccccc" /><path
+000022b0: 0a20 2020 2020 6964 3d22 7061 7468 3238  .     id="path28
+000022c0: 220a 2020 2020 2073 7479 6c65 3d22 6669  ".     style="fi
+000022d0: 6c6c 3a23 3030 3030 3030 3b73 7472 6f6b  ll:#000000;strok
+000022e0: 652d 7769 6474 683a 302e 3038 3136 3535  e-width:0.081655
+000022f0: 3422 0a20 2020 2020 643d 224d 2032 392e  4".     d="M 29.
+00002300: 3837 3233 332c 312e 3139 3732 3635 3620  87233,1.1972656 
+00002310: 3239 2e34 3231 3135 382c 312e 3231 3837  29.421158,1.2187
+00002320: 3520 6320 2d30 2e35 3938 3235 352c 302e  5 c -0.598255,0.
+00002330: 3033 3033 3438 202d 312e 3334 3431 3239  030348 -1.344129
+00002340: 2c30 2e33 3039 3737 3720 2d32 2e32 3134  ,0.309777 -2.214
+00002350: 3834 342c 302e 3832 3831 3235 206c 202d  844,0.828125 l -
+00002360: 302e 3731 3039 3337 2c30 2e34 3233 3832  0.710937,0.42382
+00002370: 3831 202d 302e 3838 3038 3539 2c30 2e37  81 -0.880859,0.7
+00002380: 3737 3334 3338 202d 302e 3838 3238 3133  773438 -0.882813
+00002390: 2c30 2e37 3737 3334 3337 202d 302e 3335  ,0.7773437 -0.35
+000023a0: 3135 3633 2c30 2e34 3533 3132 3520 6320  1563,0.453125 c 
+000023b0: 2d30 2e36 3033 3932 392c 302e 3737 3733  -0.603929,0.7773
+000023c0: 3731 3520 2d30 2e37 3137 3532 392c 312e  715 -0.717529,1.
+000023d0: 3630 3032 3037 3520 2d30 2e33 3330 3037  6002075 -0.33007
+000023e0: 382c 322e 3337 3330 3436 3920 302e 3235  8,2.3730469 0.25
+000023f0: 3032 3837 2c30 2e34 3939 3233 3820 302e  0287,0.499238 0.
+00002400: 3233 3435 3932 2c30 2e36 3235 3738 3633  234592,0.6257863
+00002410: 202d 302e 3136 3630 3135 2c31 2e34 3032   -0.166015,1.402
+00002420: 3334 3337 202d 312e 3939 3438 3631 2c33  3437 -1.994861,3
+00002430: 2e38 3636 3933 3138 202d 312e 3234 3034  .8669318 -1.2404
+00002440: 3337 2c36 2e34 3330 3434 3338 2032 2e36  37,6.4304438 2.6
+00002450: 3432 3537 382c 382e 3938 3633 3237 3820  42578,8.9863278 
+00002460: 6c20 312e 3036 3634 3036 2c30 2e37 3033  l 1.066406,0.703
+00002470: 3132 3520 302e 3338 3238 3133 2c30 2e34  125 0.382813,0.4
+00002480: 3531 3137 3220 302e 3338 3437 3635 2c30  51172 0.384765,0
+00002490: 2e34 3533 3132 3520 302e 3133 3836 3732  .453125 0.138672
+000024a0: 2c30 2e33 3834 3736 3620 6320 302e 3037  ,0.384766 c 0.07
+000024b0: 3635 332c 302e 3231 3232 3732 2030 2e31  653,0.212272 0.1
+000024c0: 3233 3630 392c 302e 3537 3837 3932 2030  23609,0.578792 0
+000024d0: 2e31 3035 3436 392c 302e 3831 3235 206c  .105469,0.8125 l
+000024e0: 202d 302e 3033 3332 2c30 2e34 3233 3832   -0.0332,0.42382
+000024f0: 3820 2d30 2e32 3132 3839 312c 302e 3334  8 -0.212891,0.34
+00002500: 3736 3536 2063 202d 302e 3230 3633 3032  7656 c -0.206302
+00002510: 2c30 2e33 3336 3532 3920 2d30 2e34 3935  ,0.336529 -0.495
+00002520: 3630 392c 302e 3537 3131 3336 202d 302e  609,0.571136 -0.
+00002530: 3833 3339 3834 2c30 2e37 3035 3037 3820  833984,0.705078 
+00002540: 2d30 2e30 3031 392c 372e 3535 652d 3420  -0.0019,7.55e-4 
+00002550: 2d30 2e30 3034 2c30 2e30 3031 3220 2d30  -0.004,0.0012 -0
+00002560: 2e30 3035 392c 302e 3030 3220 2d30 2e32  .0059,0.002 -0.2
+00002570: 3731 3838 372c 302e 3130 3639 3332 202d  71887,0.106932 -
+00002580: 302e 3537 3537 3735 2c30 2e31 3435 3335  0.575775,0.14535
+00002590: 202d 302e 3839 3435 3331 2c30 2e31 3137   -0.894531,0.117
+000025a0: 3138 3720 2d30 2e30 3931 3338 2c2d 302e  187 -0.09138,-0.
+000025b0: 3030 3831 202d 302e 3138 3338 3638 2c2d  0081 -0.183868,-
+000025c0: 302e 3032 3334 3920 2d30 2e32 3737 3334  0.02349 -0.27734
+000025d0: 342c 2d30 2e30 3432 3937 202d 302e 3033  4,-0.04297 -0.03
+000025e0: 3132 342c 2d30 2e30 3036 3520 2d30 2e30  124,-0.0065 -0.0
+000025f0: 3632 3333 2c2d 302e 3030 3938 202d 302e  6233,-0.0098 -0.
+00002600: 3039 3337 352c 2d30 2e30 3137 3538 202d  09375,-0.01758 -
+00002610: 302e 3131 3535 3336 2c2d 302e 3032 3836  0.115536,-0.0286
+00002620: 3720 2d30 2e32 3332 3631 342c 2d30 2e30  7 -0.232614,-0.0
+00002630: 3639 3033 202d 302e 3334 3936 3039 2c2d  6903 -0.349609,-
+00002640: 302e 3131 3532 3334 202d 302e 3034 3132  0.115234 -0.0412
+00002650: 342c 2d30 2e30 3136 3239 202d 302e 3038  4,-0.01629 -0.08
+00002660: 3137 352c 2d30 2e30 3334 3235 202d 302e  175,-0.03425 -0.
+00002670: 3132 3330 3437 2c2d 302e 3035 3237 3320  123047,-0.05273 
+00002680: 2d30 2e31 3232 3534 322c 2d30 2e30 3534  -0.122542,-0.054
+00002690: 3836 202d 302e 3234 3532 3332 2c2d 302e  86 -0.245232,-0.
+000026a0: 3131 3530 3239 202d 302e 3336 3731 3837  115029 -0.367187
+000026b0: 2c2d 302e 3138 3934 3533 204c 2032 352e  ,-0.189453 L 25.
+000026c0: 3031 3837 3737 2c32 302e 3938 3035 3137  018777,20.980517
+000026d0: 2032 342e 3231 3939 3439 2c32 302e 3136   24.219949,20.16
+000026e0: 3431 3120 6320 2d30 2e32 3034 3238 382c  411 c -0.204288,
+000026f0: 2d30 2e32 3039 3233 3220 2d30 2e35 3038  -0.209232 -0.508
+00002700: 3232 352c 2d30 2e35 3438 3139 3420 2d30  225,-0.548194 -0
+00002710: 2e38 3333 3938 342c 2d30 2e39 3233 3832  .833984,-0.92382
+00002720: 3820 2d30 2e30 3237 3231 2c2d 302e 3033  8 -0.02721,-0.03
+00002730: 3133 3420 2d30 2e30 3432 3739 2c2d 302e  134 -0.04279,-0.
+00002740: 3034 3632 3320 2d30 2e30 3730 3331 2c2d  04623 -0.07031,-
+00002750: 302e 3037 3831 3320 2d33 2e34 652d 342c  0.07813 -3.4e-4,
+00002760: 2d33 2e39 3465 2d34 2033 2e34 3165 2d34  -3.94e-4 3.41e-4
+00002770: 2c2d 302e 3030 3136 2030 2c2d 302e 3030  ,-0.0016 0,-0.00
+00002780: 3220 2d30 2e33 3534 3036 312c 2d30 2e34  2 -0.354061,-0.4
+00002790: 3130 3336 202d 302e 3733 3135 3836 2c2d  1036 -0.731586,-
+000027a0: 302e 3836 3234 3839 202d 312e 3034 3838  0.862489 -1.0488
+000027b0: 3238 2c2d 312e 3235 3937 3635 202d 302e  28,-1.259765 -0.
+000027c0: 3134 3338 3931 2c2d 302e 3138 3031 3934  143891,-0.180194
+000027d0: 202d 302e 3238 3534 3832 2c2d 302e 3335   -0.285482,-0.35
+000027e0: 3333 3634 202d 302e 3432 3537 3831 2c2d  3364 -0.425781,-
+000027f0: 302e 3532 3134 3835 202d 302e 3035 3637  0.521485 -0.0567
+00002800: 382c 2d30 2e30 3638 3034 202d 302e 3131  8,-0.06804 -0.11
+00002810: 3336 3632 2c2d 302e 3133 3530 3732 202d  3662,-0.135072 -
+00002820: 302e 3136 3939 3232 2c2d 302e 3230 3131  0.169922,-0.2011
+00002830: 3732 202d 302e 3439 3031 3137 2c2d 302e  72 -0.490117,-0.
+00002840: 3537 3538 3433 202d 302e 3936 3233 3834  575843 -0.962384
+00002850: 2c2d 312e 3037 3830 3333 202d 312e 3432  ,-1.078033 -1.42
+00002860: 3537 3831 2c2d 312e 3531 3336 3732 202d  5781,-1.513672 -
+00002870: 302e 3031 3839 392c 2d30 2e30 3137 3835  0.01899,-0.01785
+00002880: 202d 302e 3033 3739 382c 2d30 2e30 3335   -0.03798,-0.035
+00002890: 3032 202d 302e 3035 3636 342c 2d30 2e30  02 -0.05664,-0.0
+000028a0: 3532 3733 202d 302e 3330 3335 3538 2c2d  5273 -0.303558,-
+000028b0: 302e 3238 3231 3531 202d 302e 3630 3333  0.282151 -0.6033
+000028c0: 3637 2c2d 302e 3533 3639 3531 202d 302e  67,-0.536951 -0.
+000028d0: 3930 3432 3937 2c2d 302e 3736 3336 3732  904297,-0.763672
+000028e0: 202d 302e 3030 3435 2c2d 302e 3030 3334   -0.0045,-0.0034
+000028f0: 202d 302e 3030 3932 2c2d 302e 3030 3634   -0.0092,-0.0064
+00002900: 202d 302e 3031 3336 372c 2d30 2e30 3039   -0.01367,-0.009
+00002910: 3820 2d30 2e31 3735 3433 332c 2d30 2e31  8 -0.175433,-0.1
+00002920: 3331 3730 3120 2d30 2e33 3530 3937 2c2d  31701 -0.35097,-
+00002930: 302e 3235 3532 3636 202d 302e 3532 3733  0.255266 -0.5273
+00002940: 3434 2c2d 302e 3336 3931 3431 202d 302e  44,-0.369141 -0.
+00002950: 3331 3236 3539 2c2d 302e 3230 3138 3636  312659,-0.201866
+00002960: 202d 302e 3632 3738 3237 2c2d 302e 3337   -0.627827,-0.37
+00002970: 3633 3538 202d 302e 3934 3932 3139 2c2d  6358 -0.949219,-
+00002980: 302e 3532 3533 3931 202d 302e 3136 3231  0.525391 -0.1621
+00002990: 3337 2c2d 302e 3037 3531 3820 2d30 2e33  37,-0.07518 -0.3
+000029a0: 3236 3431 342c 2d30 2e31 3432 3536 202d  26414,-0.14256 -
+000029b0: 302e 3439 3231 3837 2c2d 302e 3230 3530  0.492187,-0.2050
+000029c0: 3738 202d 302e 3034 3438 332c 2d30 2e30  78 -0.04483,-0.0
+000029d0: 3136 3920 2d30 2e30 3839 3633 2c2d 302e  169 -0.08963,-0.
+000029e0: 3033 3437 3820 2d30 2e31 3334 3736 362c  03478 -0.134766,
+000029f0: 2d30 2e30 3530 3738 202d 302e 3030 3333  -0.05078 -0.0033
+00002a00: 2c2d 302e 3030 3132 202d 302e 3030 3635  ,-0.0012 -0.0065
+00002a10: 2c2d 302e 3030 3237 202d 302e 3030 3938  ,-0.0027 -0.0098
+00002a20: 2c2d 302e 3030 3339 202d 302e 3836 3034  ,-0.0039 -0.8604
+00002a30: 3433 2c2d 302e 3330 3336 3236 202d 312e  43,-0.303626 -1.
+00002a40: 3737 3738 3832 2c2d 302e 3434 3539 3920  777882,-0.44599 
+00002a50: 2d32 2e38 3230 3234 362c 2d30 2e34 3538  -2.820246,-0.458
+00002a60: 3935 3720 2d30 2e32 3131 3735 362c 2d30  957 -0.211756,-0
+00002a70: 2e30 3032 3620 2d30 2e34 3239 3835 342c  .0026 -0.429854,
+00002a80: 322e 3265 2d34 202d 302e 3635 3233 3434  2.2e-4 -0.652344
+00002a90: 2c30 2e30 3037 3820 6c20 2d30 2e38 3335  ,0.0078 l -0.835
+00002aa0: 3933 372c 302e 3032 3933 202d 302e 3638  937,0.0293 -0.68
+00002ab0: 3136 3431 2c30 2e32 3136 3739 3720 6320  1641,0.216797 c 
+00002ac0: 2d30 2e38 3237 3638 372c 302e 3236 3433  -0.827687,0.2643
+00002ad0: 3835 202d 312e 3333 3130 3932 2c30 2e35  85 -1.331092,0.5
+00002ae0: 3337 3830 3320 2d32 2e30 3436 3837 352c  37803 -2.046875,
+00002af0: 312e 3130 3933 3735 206c 202d 302e 3534  1.109375 l -0.54
+00002b00: 3239 3639 2c30 2e34 3333 3539 202d 302e  2969,0.43359 -0.
+00002b10: 3431 3430 3632 2c30 2e35 3131 3731 3920  414062,0.511719 
+00002b20: 6320 2d31 2e38 3236 3130 372c 322e 3236  c -1.826107,2.26
+00002b30: 3233 3337 202d 322e 3035 3632 3237 2c35  2337 -2.056227,5
+00002b40: 2e31 3238 3138 202d 302e 3630 3135 3633  .12818 -0.601563
+00002b50: 2c37 2e34 3938 3036 206c 2030 2e32 3936  ,7.49806 l 0.296
+00002b60: 3837 352c 302e 3438 3234 3232 2030 2e36  875,0.482422 0.6
+00002b70: 3035 3436 392c 302e 3630 3734 3232 2063  05469,0.607422 c
+00002b80: 2031 2e33 3134 3934 312c 312e 3332 3138   1.314941,1.3218
+00002b90: 3820 322e 3835 3535 3938 2c32 2e31 3038  8 2.855598,2.108
+00002ba0: 3339 3620 352e 3839 3036 3235 2c33 2e30  396 5.890625,3.0
+00002bb0: 3031 3935 3320 372e 3235 3833 2c32 2e31  01953 7.2583,2.1
+00002bc0: 3336 3935 3220 392e 3237 3138 3731 2c33  36952 9.271871,3
+00002bd0: 2e35 3737 3536 3920 382e 3436 3039 3337  .577569 8.460937
+00002be0: 2c36 2e30 3534 3638 3720 6c20 2d30 2e31  ,6.054687 l -0.1
+00002bf0: 3430 3632 352c 302e 3433 3136 3431 202d  40625,0.431641 -
+00002c00: 302e 3330 3436 3837 2c30 2e33 3635 3233  0.304687,0.36523
+00002c10: 3420 2d30 2e33 3034 3638 382c 302e 3336  4 -0.304688,0.36
+00002c20: 3532 3335 202d 302e 3334 3137 3937 2c30  5235 -0.341797,0
+00002c30: 2e31 3532 3334 3420 6320 2d31 2e33 3730  .152344 c -1.370
+00002c40: 3530 362c 302e 3631 3239 3931 202d 322e  506,0.612991 -2.
+00002c50: 3635 3536 3935 2c2d 302e 3031 3031 3320  655695,-0.01013 
+00002c60: 2d35 2e35 3333 3230 332c 2d32 2e36 3831  -5.533203,-2.681
+00002c70: 3634 3120 6c20 2d31 2e35 3536 3634 2c2d  641 l -1.55664,-
+00002c80: 312e 3434 3533 3133 202d 302e 3539 3736  1.445313 -0.5976
+00002c90: 3536 2c2d 302e 3431 3430 3632 2043 2031  56,-0.414062 C 1
+00002ca0: 322e 3932 3936 3037 2c32 382e 3438 3438  2.929607,28.4848
+00002cb0: 3439 2031 312e 3138 3132 3832 2c32 372e  49 11.181282,27.
+00002cc0: 3938 3136 3831 2039 2e37 3636 3836 312c  981681 9.766861,
+00002cd0: 3238 2e34 3335 3534 3720 6c20 2d30 2e33  28.435547 l -0.3
+00002ce0: 3932 3537 382c 302e 3132 3520 2d30 2e34  92578,0.125 -0.4
+00002cf0: 3634 3834 342c 302e 3431 3231 3039 202d  64844,0.412109 -
+00002d00: 302e 3436 3238 392c 302e 3431 3231 3120  0.46289,0.41211 
+00002d10: 2d30 2e32 3434 3134 312c 302e 3433 3934  -0.244141,0.4394
+00002d20: 3533 2063 202d 302e 3637 3939 3634 2c31  53 c -0.679964,1
+00002d30: 2e32 3331 3734 3320 2d30 2e36 3239 3039  .231743 -0.62909
+00002d40: 352c 322e 3432 3739 3938 2030 2e31 3538  5,2.427998 0.158
+00002d50: 3230 332c 332e 3733 3433 3735 206c 2030  203,3.734375 l 0
+00002d60: 2e32 3735 3339 312c 302e 3435 3730 3331  .275391,0.457031
+00002d70: 2031 2e33 3038 3539 342c 312e 3430 3233   1.308594,1.4023
+00002d80: 3434 2031 2e33 3130 3534 372c 312e 3430  44 1.310547,1.40
+00002d90: 3432 3937 2030 2e32 3434 3134 2c30 2e34  4297 0.24414,0.4
+00002da0: 3736 3536 3220 6320 302e 3830 3737 3937  76562 c 0.807797
+00002db0: 2c31 2e35 3738 3534 3120 302e 3534 3736  ,1.578541 0.5476
+00002dc0: 3339 2c33 2e34 3730 3332 3920 2d30 2e38  39,3.470329 -0.8
+00002dd0: 3138 3335 392c 352e 3933 3335 3934 202d  18359,5.933594 -
+00002de0: 302e 3537 3937 3737 2c31 2e30 3435 3439  0.579777,1.04549
+00002df0: 3720 2d30 2e35 3538 3339 2c31 2e31 3330  7 -0.55839,1.130
+00002e00: 3635 3620 302e 3131 3931 342c 302e 3435  656 0.11914,0.45
+00002e10: 3331 3235 2030 2e39 3335 3039 2c2d 302e  3125 0.93509,-0.
+00002e20: 3933 3530 3920 312e 3631 3233 3234 2c2d  93509 1.612324,-
+00002e30: 322e 3033 3735 3936 2032 2e30 3730 3331  2.037596 2.07031
+00002e40: 332c 2d33 2e33 3733 3034 3720 6c20 302e  3,-3.373047 l 0.
+00002e50: 3235 2c2d 302e 3733 3034 3639 2030 2e30  25,-0.730469 0.0
+00002e60: 3032 2c2d 302e 3837 3130 3933 2030 2e30  02,-0.871093 0.0
+00002e70: 3031 392c 2d30 2e38 3731 3039 3420 2d30  019,-0.871094 -0
+00002e80: 2e32 3236 3536 332c 2d30 2e36 3937 3236  .226563,-0.69726
+00002e90: 3620 4320 3132 2e35 3335 3033 322c 3336  6 C 12.535032,36
+00002ea0: 2e30 3237 3136 3920 3132 2e32 3731 3839  .027169 12.27189
+00002eb0: 372c 3335 2e36 3132 3336 2031 302e 3932  7,35.61236 10.92
+00002ec0: 3530 3634 2c33 342e 3033 3531 3536 2039  5064,34.035156 9
+00002ed0: 2e36 3534 3933 332c 3332 2e35 3437 3737  .654933,32.54777
+00002ee0: 3520 392e 3438 3533 3636 2c33 322e 3231  5 9.485366,32.21
+00002ef0: 3839 3920 392e 3539 3130 382c 3331 2e34  899 9.59108,31.4
+00002f00: 3333 3539 3420 6c20 302e 3035 3037 382c  33594 l 0.05078,
+00002f10: 2d30 2e33 3735 2030 2e33 3038 3539 342c  -0.375 0.308594,
+00002f20: 2d30 2e33 3535 3436 3920 302e 3330 3636  -0.355469 0.3066
+00002f30: 342c 2d30 2e33 3535 3436 3920 302e 3430  4,-0.355469 0.40
+00002f40: 3432 3937 2c2d 302e 3032 3733 3420 6320  4297,-0.02734 c 
+00002f50: 302e 3838 3132 3539 2c2d 302e 3035 3732  0.881259,-0.0572
+00002f60: 3420 322e 3130 3737 3939 2c30 2e35 3735  4 2.107799,0.575
+00002f70: 3034 3720 332e 3639 3533 3133 2c31 2e39  047 3.695313,1.9
+00002f80: 3032 3334 3420 6c20 302e 3735 3339 3036  02344 l 0.753906
+00002f90: 2c30 2e36 3238 3930 3620 312e 3038 3738  ,0.628906 1.0878
+00002fa0: 3931 2c31 2e32 3236 3536 3320 312e 3038  91,1.226563 1.08
+00002fb0: 3938 3434 2c31 2e32 3236 3536 3320 302e  9844,1.226563 0.
+00002fc0: 3631 3332 3831 2c30 2e34 3738 3531 3520  613281,0.478515 
+00002fd0: 6320 322e 3534 3638 3534 2c31 2e39 3837  c 2.546854,1.987
+00002fe0: 3834 3520 352e 3434 3736 392c 322e 3334  845 5.44769,2.34
+00002ff0: 3634 3832 2037 2e33 3836 3731 392c 302e  6482 7.386719,0.
+00003000: 3931 3430 3633 2030 2e37 3437 3931 2c2d  914063 0.74791,-
+00003010: 302e 3535 3235 3036 2031 2e33 3930 3931  0.552506 1.39091
+00003020: 312c 2d31 2e34 3937 3834 3320 312e 3738  1,-1.497843 1.78
+00003030: 3332 3033 2c2d 322e 3632 3330 3437 206c  3203,-2.623047 l
+00003040: 2030 2e32 3533 3930 362c 2d30 2e37 3236   0.253906,-0.726
+00003050: 3536 3320 302e 3030 3339 2c2d 302e 3933  563 0.0039,-0.93
+00003060: 3136 3420 302e 3030 3339 2c2d 302e 3933  164 0.0039,-0.93
+00003070: 3136 3431 202d 302e 3235 2c2d 302e 3733  1641 -0.25,-0.73
+00003080: 3234 3232 2043 2032 362e 3934 3535 3137  2422 C 26.945517
+00003090: 2c33 302e 3334 3938 3535 2032 362e 3637  ,30.349855 26.67
+000030a0: 3936 2c32 392e 3738 3632 3638 2032 362e  96,29.786268 26.
+000030b0: 3439 3134 3731 2c32 392e 3439 3830 3437  491471,29.498047
+000030c0: 206c 202d 302e 3334 3337 352c 2d30 2e35   l -0.34375,-0.5
+000030d0: 3235 3339 3120 2d30 2e39 3531 3137 322c  25391 -0.951172,
+000030e0: 2d30 2e38 3934 3533 3120 2d30 2e39 3533  -0.894531 -0.953
+000030f0: 3132 352c 2d30 2e38 3934 3533 3120 2d30  125,-0.894531 -0
+00003100: 2e35 3830 3037 382c 2d30 2e33 3435 3730  .580078,-0.34570
+00003110: 3320 4320 3232 2e36 3739 3233 2c32 362e  3 C 22.67923,26.
+00003120: 3234 3934 3631 2032 312e 3438 3532 3631  249461 21.485261
+00003130: 2c32 352e 3737 3035 3936 2031 382e 3434  ,25.770596 18.44
+00003140: 3435 3936 2c32 342e 3734 3830 3437 2031  4596,24.748047 1
+00003150: 352e 3136 3931 2c32 332e 3634 3635 3236  5.1691,23.646526
+00003160: 2031 342e 3431 3031 3834 2c32 332e 3334   14.410184,23.34
+00003170: 3430 3936 2031 332e 3332 3135 3439 2c32  4096 13.321549,2
+00003180: 322e 3730 3131 3732 204c 2031 322e 3536  2.701172 L 12.56
+00003190: 3736 3433 2c32 322e 3235 3538 3539 2031  7643,22.255859 1
+000031a0: 322e 3135 3335 382c 3231 2e37 3839 3036  2.15358,21.78906
+000031b0: 3220 3131 2e37 3337 3536 342c 3231 2e33  2 11.737564,21.3
+000031c0: 3234 3231 3920 3131 2e35 3539 3833 2c32  24219 11.55983,2
+000031d0: 302e 3834 3736 3536 2063 202d 302e 3232  0.847656 c -0.22
+000031e0: 3533 3834 2c2d 302e 3630 3630 3132 202d  5384,-0.606012 -
+000031f0: 302e 3235 3638 3533 2c2d 312e 3338 3734  0.256853,-1.3874
+00003200: 3137 202d 302e 3038 3030 382c 2d31 2e39  17 -0.08008,-1.9
+00003210: 3535 3037 3820 6c20 302e 3133 3836 3732  55078 l 0.138672
+00003220: 2c2d 302e 3434 3333 3539 2030 2e34 3930  ,-0.443359 0.490
+00003230: 3233 342c 2d30 2e34 3932 3138 3820 302e  234,-0.492188 0.
+00003240: 3439 3032 3335 2c2d 302e 3439 3231 3837  490235,-0.492187
+00003250: 2030 2e34 3736 3536 322c 2d30 2e31 3731   0.476562,-0.171
+00003260: 3837 3520 6320 312e 3237 3233 3134 2c2d  875 c 1.272314,-
+00003270: 302e 3436 3030 3334 2032 2e36 3336 3539  0.460034 2.63659
+00003280: 382c 2d30 2e31 3637 3136 3720 342e 3038  8,-0.167167 4.08
+00003290: 3230 3331 2c30 2e38 3639 3134 2030 2e30  2031,0.86914 0.0
+000032a0: 3438 3038 2c30 2e30 3334 3437 2030 2e30  4808,0.03447 0.0
+000032b0: 3936 3238 2c30 2e30 3733 3236 2030 2e31  9628,0.07326 0.1
+000032c0: 3434 3533 322c 302e 3130 3933 3735 2030  44532,0.109375 0
+000032d0: 2e30 3831 3138 2c30 2e30 3630 3735 2030  .08118,0.06075 0
+000032e0: 2e31 3632 3436 332c 302e 3132 3231 3033  .162463,0.122103
+000032f0: 2030 2e32 3434 3134 2c30 2e31 3837 3520   0.24414,0.1875 
+00003300: 302e 3036 3031 382c 302e 3034 3831 3820  0.06018,0.04818 
+00003310: 302e 3132 3131 3933 2c30 2e30 3937 3733  0.121193,0.09773
+00003320: 2030 2e31 3831 3634 312c 302e 3134 3834   0.181641,0.1484
+00003330: 3338 2030 2e30 3732 3236 2c30 2e30 3630  38 0.07226,0.060
+00003340: 3632 2030 2e31 3434 3134 392c 302e 3132  62 0.144149,0.12
+00003350: 3332 3732 2030 2e32 3136 3739 372c 302e  3272 0.216797,0.
+00003360: 3138 3735 2030 2e32 3033 3135 2c30 2e31  1875 0.20315,0.1
+00003370: 3739 3630 3820 302e 3430 3731 3637 2c30  79608 0.407167,0
+00003380: 2e33 3732 3234 3220 302e 3631 3332 3831  .372242 0.613281
+00003390: 2c30 2e35 3830 3037 3820 302e 3131 3937  ,0.580078 0.1197
+000033a0: 3031 2c30 2e31 3230 3730 3220 302e 3234  01,0.120702 0.24
+000033b0: 3036 3433 2c30 2e32 3436 3732 3720 302e  0643,0.246727 0.
+000033c0: 3336 3133 3238 2c30 2e33 3736 3935 3320  361328,0.376953 
+000033d0: 302e 3036 3337 352c 302e 3036 3837 3920  0.06375,0.06879 
+000033e0: 302e 3132 3733 3836 2c30 2e31 3339 3439  0.127386,0.13949
+000033f0: 3220 302e 3139 3134 3036 2c30 2e32 3130  2 0.191406,0.210
+00003400: 3933 3820 302e 3236 3133 3937 2c30 2e32  938 0.261397,0.2
+00003410: 3931 3731 3520 302e 3532 3531 3535 2c30  91715 0.525155,0
+00003420: 2e36 3033 3430 3820 302e 3739 3130 3136  .603408 0.791016
+00003430: 2c30 2e39 3339 3435 3320 302e 3437 3639  ,0.939453 0.4769
+00003440: 3038 2c30 2e36 3032 3830 3920 312e 3232  08,0.602809 1.22
+00003450: 3038 3532 2c31 2e34 3439 3236 3920 312e  0852,1.449269 1.
+00003460: 3635 3432 3937 2c31 2e38 3832 3831 3220  654297,1.882812 
+00003470: 6c20 302e 3738 3930 3632 2c30 2e37 3839  l 0.789062,0.789
+00003480: 3036 3320 302e 3736 3735 3738 2c30 2e35  063 0.767578,0.5
+00003490: 3432 3936 3920 6320 312e 3634 3136 3238  42969 c 1.641628
+000034a0: 2c31 2e31 3538 3830 3920 332e 3034 3833  ,1.158809 3.0483
+000034b0: 3134 2c31 2e36 3139 3034 3920 342e 3738  14,1.619049 4.78
+000034c0: 3731 312c 312e 3536 3833 3539 206c 2030  711,1.568359 l 0
+000034d0: 2e37 3839 3036 322c 2d30 2e30 3233 3434  .789062,-0.02344
+000034e0: 2030 2e37 3136 3739 372c 2d30 2e32 3434   0.716797,-0.244
+000034f0: 3134 2063 2030 2e31 3132 3731 332c 2d30  14 c 0.112713,-0
+00003500: 2e30 3338 3337 2030 2e32 3138 3631 372c  .03837 0.218617,
+00003510: 2d30 2e30 3738 3632 2030 2e33 3230 3331  -0.07862 0.32031
+00003520: 332c 2d30 2e31 3139 3134 3120 6c20 2d30  3,-0.119141 l -0
+00003530: 2e30 3033 392c 2d30 2e30 3035 3920 6320  .0039,-0.0059 c 
+00003540: 302e 3638 3433 3331 2c2d 302e 3237 3432  0.684331,-0.2742
+00003550: 3131 2031 2e31 3537 3037 382c 2d30 2e36  11 1.157078,-0.6
+00003560: 3130 3837 3320 312e 3731 3039 3338 2c2d  10873 1.710938,-
+00003570: 312e 3233 3433 3735 206c 2030 2e34 3838  1.234375 l 0.488
+00003580: 3238 312c 2d30 2e35 3530 3738 3220 302e  281,-0.550782 0.
+00003590: 3333 3339 3834 2c2d 302e 3637 3338 3238  333984,-0.673828
+000035a0: 2063 2030 2e39 3134 3731 312c 2d31 2e38   c 0.914711,-1.8
+000035b0: 3437 3431 3820 302e 3833 3030 3936 2c2d  47418 0.830096,-
+000035c0: 332e 3636 3532 3120 2d30 2e32 352c 2d35  3.66521 -0.25,-5
+000035d0: 2e33 3633 3238 3120 4c20 3331 2e36 3439  .363281 L 31.649
+000035e0: 3637 392c 3136 2e39 3134 3031 3920 3330  679,16.914019 30
+000035f0: 2e38 3033 3937 362c 3136 2e31 3330 3831  .803976,16.13081
+00003600: 3620 3239 2e39 3538 3237 332c 3135 2e33  6 29.958273,15.3
+00003610: 3439 3536 3620 3239 2e32 3934 3231 2c31  49566 29.29421,1
+00003620: 342e 3937 3236 3133 2043 2032 382e 3932  4.972613 C 28.92
+00003630: 3930 3634 2c31 342e 3736 3631 3820 3238  9064,14.76618 28
+00003640: 2e33 3731 3932 382c 3134 2e34 3636 3938  .371928,14.46698
+00003650: 3120 3238 2e30 3535 3932 342c 3134 2e33  1 28.055924,14.3
+00003660: 3036 3634 3120 3237 2e37 3339 3931 382c  06641 27.739918,
+00003670: 3134 2e31 3436 3320 3237 2e32 3631 3632  14.1463 27.26162
+00003680: 332c 3133 2e38 3538 3939 3620 3236 2e39  3,13.858996 26.9
+00003690: 3933 3432 342c 3133 2e36 3637 3936 3920  93424,13.667969 
+000036a0: 6c20 2d30 2e34 3838 3238 322c 2d30 2e33  l -0.488282,-0.3
+000036b0: 3437 3635 3720 2d30 2e32 3338 3238 312c  47657 -0.238281,
+000036c0: 2d30 2e33 3637 3138 3720 6320 2d30 2e35  -0.367187 c -0.5
+000036d0: 3931 3735 372c 2d30 2e39 3134 3836 3620  91757,-0.914866 
+000036e0: 2d30 2e35 3632 3539 2c2d 322e 3334 3435  -0.56259,-2.3445
+000036f0: 3032 2030 2e30 3734 3232 2c2d 332e 3730  02 0.07422,-3.70
+00003700: 3730 3331 3220 4c20 3236 2e35 3737 3430  70312 L 26.57740
+00003710: 382c 382e 3733 3832 3831 3220 3236 2e39  8,8.7382812 26.9
+00003720: 3033 3538 2c38 2e36 3935 3331 3235 2043  0358,8.6953125 C
+00003730: 2032 372e 3038 3335 3932 2c38 2e36 3731   27.083592,8.671
+00003740: 3038 3335 2032 372e 3439 3831 342c 382e  0835 27.49814,8.
+00003750: 3535 3531 3032 3820 3237 2e38 3233 3530  5551028 27.82350
+00003760: 322c 382e 3433 3735 204c 2032 382e 3431  2,8.4375 L 28.41
+00003770: 3532 3939 2c38 2e32 3232 3635 3632 2032  5299,8.2226562 2
+00003780: 382e 3938 3536 3131 2c37 2e36 3937 3236  8.985611,7.69726
+00003790: 3536 2032 392e 3535 3738 3737 2c37 2e31  56 29.557877,7.1
+000037a0: 3639 3932 3139 2032 392e 3836 3634 3731  699219 29.866471
+000037b0: 2c36 2e35 3534 3638 3735 2043 2033 302e  ,6.5546875 C 30.
+000037c0: 3739 3835 3531 2c34 2e36 3935 3039 3033  798551,4.6950903
+000037d0: 2033 312e 3039 3531 3133 2c32 2e37 3039   31.095113,2.709
+000037e0: 3531 3732 2033 302e 3537 3734 3038 2c31  5172 30.577408,1
+000037f0: 2e37 3936 3837 3520 4c20 3330 2e34 3131  .796875 L 30.411
+00003800: 3339 322c 312e 3530 3538 3539 3420 3330  392,1.5058594 30
+00003810: 2e31 3431 3836 312c 312e 3335 3135 3632  .141861,1.351562
+00003820: 3520 5a22 202f 3e3c 7061 7468 0a20 2020  5 Z" /><path.   
+00003830: 2020 6964 3d22 7061 7468 3822 0a20 2020    id="path8".   
+00003840: 2020 7374 796c 653d 2266 696c 6c3a 2366    style="fill:#f
+00003850: 6136 3836 333b 6669 6c6c 2d6f 7061 6369  a6863;fill-opaci
+00003860: 7479 3a31 3b73 7472 6f6b 652d 7769 6474  ty:1;stroke-widt
+00003870: 683a 302e 3337 3136 3139 220a 2020 2020  h:0.371619".    
+00003880: 2064 3d22 6d20 372e 3035 3936 3938 382c   d="m 7.0596988,
+00003890: 3235 2e30 3335 3538 3720 6820 382e 3834  25.035587 h 8.84
+000038a0: 3537 3032 3220 7620 332e 3031 3536 3236  57022 v 3.015626
+000038b0: 2048 2037 2e30 3539 3639 3838 205a 220a   H 7.0596988 Z".
+000038c0: 2020 2020 2073 6f64 6970 6f64 693a 6e6f       sodipodi:no
+000038d0: 6465 7479 7065 733d 2263 6363 6363 2220  detypes="ccccc" 
+000038e0: 2f3e 3c70 6174 680a 2020 2020 2069 643d  /><path.     id=
+000038f0: 2270 6174 6839 220a 2020 2020 2073 7479  "path9".     sty
+00003900: 6c65 3d22 6669 6c6c 3a23 6631 3830 3436  le="fill:#f18046
+00003910: 3b66 696c 6c2d 6f70 6163 6974 793a 313b  ;fill-opacity:1;
+00003920: 7374 726f 6b65 2d77 6964 7468 3a30 2e33  stroke-width:0.3
+00003930: 3731 3631 3922 0a20 2020 2020 643d 226d  71619".     d="m
+00003940: 2032 322e 3031 3536 3235 2c31 332e 3333   22.015625,13.33
+00003950: 3738 3931 2063 202d 312e 3239 3238 3431  7891 c -1.292841
+00003960: 2c30 2e34 3538 3037 202d 322e 3636 3538  ,0.45807 -2.6658
+00003970: 3734 2c30 2e37 3436 3338 3120 2d34 2e30  74,0.746381 -4.0
+00003980: 3931 3739 372c 302e 3833 3539 3337 2076  91797,0.835937 v
+00003990: 2038 2e38 3433 3735 2063 2033 2e30 3331   8.84375 c 3.031
+000039a0: 3138 322c 2d30 2e31 3139 3435 2035 2e39  182,-0.11945 5.9
+000039b0: 3135 3931 322c 2d30 2e38 3035 3036 3120  15912,-0.805061 
+000039c0: 382e 3535 3636 3431 2c2d 312e 3934 3732  8.556641,-1.9472
+000039d0: 3636 207a 220a 2020 2020 2073 6f64 6970  66 z".     sodip
+000039e0: 6f64 693a 6e6f 6465 7479 7065 733d 2263  odi:nodetypes="c
+000039f0: 6363 6363 2220 2f3e 3c70 6174 680a 2020  cccc" /><path.  
+00003a00: 2020 2069 643d 2270 6174 6831 3122 0a20     id="path11". 
+00003a10: 2020 2020 7374 796c 653d 2266 696c 6c3a      style="fill:
+00003a20: 2333 6439 3566 643b 6669 6c6c 2d6f 7061  #3d95fd;fill-opa
+00003a30: 6369 7479 3a31 3b73 7472 6f6b 652d 7769  city:1;stroke-wi
+00003a40: 6474 683a 302e 3337 3136 3139 220a 2020  dth:0.371619".  
+00003a50: 2020 2064 3d22 6d20 3137 2e38 3938 3433     d="m 17.89843
+00003a60: 382c 3330 2e30 3734 3231 3920 7620 332e  8,30.074219 v 3.
+00003a70: 3833 3030 3738 2063 2030 2e38 3235 3437  830078 c 0.82547
+00003a80: 372c 302e 3035 3138 3520 312e 3633 3133  7,0.05185 1.6313
+00003a90: 3034 2c30 2e31 3734 3332 3920 322e 3431  04,0.174329 2.41
+00003aa0: 3630 3135 2c30 2e33 3533 3531 3520 7a22  6015,0.353515 z"
+00003ab0: 0a20 2020 2020 736f 6469 706f 6469 3a6e  .     sodipodi:n
+00003ac0: 6f64 6574 7970 6573 3d22 6363 6363 2220  odetypes="cccc" 
+00003ad0: 2f3e 3c2f 7376 673e 0a                   /></svg>.
```

### Comparing `seqerakit-0.4.7/examples/python/launch_hello_world.py` & `seqerakit-0.4.8/examples/python/launch_hello_world.py`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.7/examples/yaml/compute-envs/seqera_aws_ireland_fusionv2_nvme.json` & `seqerakit-0.4.8/examples/yaml/compute-envs/seqera_aws_ireland_fusionv2_nvme.json`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.7/examples/yaml/compute-envs/seqera_aws_virginia_fusionv2_nvme.json` & `seqerakit-0.4.8/examples/yaml/compute-envs/seqera_aws_virginia_fusionv2_nvme.json`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.7/examples/yaml/datasets/rnaseq_samples.csv` & `seqerakit-0.4.8/examples/yaml/datasets/rnaseq_samples.csv`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.7/examples/yaml/datasets/sentieon_samples.csv` & `seqerakit-0.4.8/examples/yaml/datasets/sentieon_samples.csv`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.7/examples/yaml/datasets/viralrecon_illumina_samples.csv` & `seqerakit-0.4.8/examples/yaml/datasets/viralrecon_illumina_samples.csv`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.7/examples/yaml/e2e/compute-envs.yml` & `seqerakit-0.4.8/examples/yaml/e2e/compute-envs.yml`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.7/examples/yaml/e2e/credentials.yml` & `seqerakit-0.4.8/examples/yaml/e2e/credentials.yml`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.7/examples/yaml/e2e/datasets.yml` & `seqerakit-0.4.8/examples/yaml/e2e/datasets.yml`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.7/examples/yaml/e2e/pipelines.yml` & `seqerakit-0.4.8/examples/yaml/e2e/pipelines.yml`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.7/examples/yaml/pipelines/nf-core-sarek_pipeline.json` & `seqerakit-0.4.8/examples/yaml/pipelines/nf-core-sarek_pipeline.json`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.7/examples/yaml/pipelines/nf_core_rnaseq_pipeline.json` & `seqerakit-0.4.8/examples/yaml/pipelines/nf_core_rnaseq_pipeline.json`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.7/examples/yaml/pipelines/nf_core_viralrecon_nanopore_pipeline.json` & `seqerakit-0.4.8/examples/yaml/pipelines/nf_core_viralrecon_nanopore_pipeline.json`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.7/examples/yaml/pipelines/nf_sentieon_pipeline.json` & `seqerakit-0.4.8/examples/yaml/pipelines/nf_sentieon_pipeline.json`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.7/examples/yaml/seqerakit-e2e.yml` & `seqerakit-0.4.8/examples/yaml/seqerakit-e2e.yml`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.7/seqerakit/cli.py` & `seqerakit-0.4.8/seqerakit/cli.py`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.7/seqerakit/computeenvs.py` & `seqerakit-0.4.8/seqerakit/computeenvs.py`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.7/seqerakit/helper.py` & `seqerakit-0.4.8/seqerakit/helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 This file contains helper functions for the library.
 Including handling methods for each block in the YAML file, and parsing
 methods for each block in the YAML file.
 """
 import yaml
 from seqerakit import utils
 import sys
+import json
 
 
 def parse_yaml_block(yaml_data, block_name):
     # Get the name of the specified block/resource.
     block = yaml_data.get(block_name)
 
     # If block is not found in the YAML, return an empty list.
@@ -75,32 +76,36 @@
             with open(file_path, "r") as f:
                 data = yaml.safe_load(f)
                 if not data:
                     raise ValueError(
                         f" The file '{file_path}' is empty or "
                         "does not contain valid data."
                     )
-
+            # Process each key-value pair in YAML data
             for key, new_value in data.items():
-                if key in merged_data:
-                    if isinstance(new_value, list) and all(
-                        isinstance(i, dict) for i in new_value
-                    ):
-                        # Handle list of dictionaries & merge without duplication
-                        existing_items = {
-                            tuple(sorted(d.items())) for d in merged_data[key]
-                        }
-                        for item in new_value:
-                            if tuple(sorted(item.items())) not in existing_items:
-                                merged_data[key].append(item)
-                    else:
-                        # override if not list of dictionaries
-                        merged_data[key] = new_value
+                # Check if key exist in merged_data and
+                # new value is a list of dictionaries
+                if (
+                    key in merged_data
+                    and isinstance(new_value, list)
+                    and all(isinstance(i, dict) for i in new_value)
+                ):
+                    # Serialize dictionaries to JSON strings for comparison
+                    existing_items = {
+                        json.dumps(d, sort_keys=True) for d in merged_data[key]
+                    }
+                    for item in new_value:
+                        # Check if item is not already present in merged data
+                        item_json = json.dumps(item, sort_keys=True)
+                        if item_json not in existing_items:
+                            # Append item to merged data
+                            merged_data[key].append(item)
                 else:
                     merged_data[key] = new_value
+
         except FileNotFoundError:
             print(f"Error: The file '{file_path}' was not found.")
             sys.exit(1)
 
     block_names = list(merged_data.keys())
 
     # Define the order in which the resources should be created.
```

### Comparing `seqerakit-0.4.7/seqerakit/overwrite.py` & `seqerakit-0.4.8/seqerakit/overwrite.py`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.7/seqerakit/pipelines.py` & `seqerakit-0.4.8/seqerakit/pipelines.py`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.7/seqerakit/seqeraplatform.py` & `seqerakit-0.4.8/seqerakit/seqeraplatform.py`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.7/seqerakit/utils.py` & `seqerakit-0.4.8/seqerakit/utils.py`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.7/seqerakit.egg-info/PKG-INFO` & `seqerakit-0.4.8/seqerakit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: seqerakit
-Version: 0.4.7
+Version: 0.4.8
 Summary: Automate creation of Seqera Platform resources
 Home-page: https://github.com/seqeralabs/seqera-kit
 Author: Esha Joshi, Adam Talbot, Harshil Patel
 Author-email: esha.joshi@seqera.io, adam.talbot@seqera.io, harshil.patel@seqera.io
 License: Apache 2.0
 Keywords: nextflow,bioinformatics,workflow,pipeline,seqera-platform,seqera
 Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pyyaml>=6.0.0
 
-# <img src="https://raw.githubusercontent.com/seqeralabs/seqera-kit/main/assets/seqerakit.svg" width=50 alt="seqerakit logo"> seqerakit
-
+# <img src="assets/seqerakit.svg" width=50 alt="seqerakit logo"> seqerakit
 
 `seqerakit` is a Python wrapper for the [Seqera Platform CLI](https://github.com/seqeralabs/tower-cli). It can be leveraged to automate the creation of all of the entities in Seqera Platform via a simple configuration file in YAML format.
 
 The key features are:
 
 - **Simple configuration**: All of the command-line options available when using the Seqera Platform CLI can be defined in simple YAML format.
 - **Infrastructure as Code**: Enable users to manage and provision their infrastructure specifications.
```

### Comparing `seqerakit-0.4.7/seqerakit.egg-info/SOURCES.txt` & `seqerakit-0.4.8/seqerakit.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 .dockerignore
 .gitignore
 .pre-commit-config.yaml
 .prettierrc
 LICENSE.txt
+MANIFEST.in
 README.md
 __init__.py
 setup.py
 .github/CONTRIBUTING.md
 .github/workflows/e2e-testing.yml
 .github/workflows/python-testing.yml
 .github/workflows/teardown.yml
+assets/seqerakit.png
 assets/seqerakit.svg
 examples/python/launch_hello_world.py
 examples/yaml/seqerakit-e2e.yml
 examples/yaml/compute-envs/seqera_aws_ireland_fusionv2_nvme.json
 examples/yaml/compute-envs/seqera_aws_virginia_fusionv2_nvme.json
 examples/yaml/compute-envs/seqera_azure_virginia.json
 examples/yaml/compute-envs/seqera_gcp_finland.json
@@ -42,15 +44,14 @@
 examples/yaml/pipelines/nf_core_viralrecon_illumina_pipeline.json
 examples/yaml/pipelines/nf_core_viralrecon_nanopore_pipeline.json
 examples/yaml/pipelines/nf_sentieon_pipeline.json
 examples/yaml/pipelines/pre_run.txt
 seqerakit/__init__.py
 seqerakit/cli.py
 seqerakit/computeenvs.py
-seqerakit/dump_yaml.py
 seqerakit/helper.py
 seqerakit/overwrite.py
 seqerakit/pipelines.py
 seqerakit/seqeraplatform.py
 seqerakit/utils.py
 seqerakit.egg-info/PKG-INFO
 seqerakit.egg-info/SOURCES.txt
```

### Comparing `seqerakit-0.4.7/setup.py` & `seqerakit-0.4.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 
 from setuptools import find_packages, setup
 
-VERSION = "0.4.7"
+VERSION = "0.4.8"
 
 with open("README.md") as f:
     readme = f.read()
 
 setup(
     name="seqerakit",
     version=VERSION,
```

### Comparing `seqerakit-0.4.7/templates/actions.yml` & `seqerakit-0.4.8/templates/actions.yml`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.7/templates/compute-envs.yml` & `seqerakit-0.4.8/templates/compute-envs.yml`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.7/templates/credentials.yml` & `seqerakit-0.4.8/templates/credentials.yml`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.7/templates/launch.yml` & `seqerakit-0.4.8/templates/launch.yml`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.7/templates/participants.yml` & `seqerakit-0.4.8/templates/participants.yml`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.7/templates/pipelines.yml` & `seqerakit-0.4.8/templates/pipelines.yml`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.7/tests/e2e/aws-e2e.yml` & `seqerakit-0.4.8/tests/e2e/aws-e2e.yml`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.7/tests/unit/test_helper.py` & `seqerakit-0.4.8/tests/unit/test_helper.py`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.7/tests/unit/test_seqeraplatform.py` & `seqerakit-0.4.8/tests/unit/test_seqeraplatform.py`

 * *Files identical despite different names*

### Comparing `seqerakit-0.4.7/tests/unit/test_subcommands.py` & `seqerakit-0.4.8/tests/unit/test_subcommands.py`

 * *Files identical despite different names*

